https://chakra-templates.dev/

# Login

index.js

```
import { ChakraProvider } from '@chakra-ui/react';

ReactDOM.render(
  <ChakraProvider>
    <React.StrictMode>
      <App />
    </React.StrictMode>
  </ChakraProvider>,
  document.getElementById('root')
);

```
App.js

```
import './App.css';
import {Flex, Heading, Input, Button, useColorMode, useColorModeValue} from "@chakra-ui/react"


const App  = () => {
  const { toggleColorMode } = useColorMode();
  const formBackground = useColorModeValue("gray.100", "gray.700");
  return (
    <Flex height="100vh" align="center" justifyContent="center">
          <Flex direction="column" backgroundColor={formBackground} p={12} rouded={6}>
              <Heading mb={6}>Login</Heading>
              <Input placeholder="demo@demo.cl" variant="flushed" mb={3} type="email" />
              <Input placeholder="********" variant="flushed" mb={6} type="passsword" />
            <Button colorScheme="teal">Login</Button>
            <Button colorScheme="teal" mt={3} onClick={toggleColorMode}>Toggle Color Mode</Button>
        </Flex>
    </Flex>
  );
}

export default App;

```
