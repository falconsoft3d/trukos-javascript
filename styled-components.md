yarn add styled-components

```
import styled from "styled-components";

const Wrapper = styled.div`
  padding: 20px;
  ${mobile({ padding: "10px" })}
`;

<Container>
      <Wrapper>
        <Title>SIGN IN</Title>
        <Form>
          <Input placeholder="username" />
          <Input placeholder="password" />
          <Button>LOGIN</Button>
          <Link>DO NOT YOU REMEMBER THE PASSWORD?</Link>
          <Link>CREATE A NEW ACCOUNT</Link>
        </Form>
      </Wrapper>
    </Container>
```    
    
