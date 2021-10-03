```
const [products, setProducts] = useState([]);

useEffect(() => {
const getProducts = async () => {
  try {
          const res = await axios.get(cat ? `http://localhost:5000/api/products?category=${cat}`
          :`http://localhost:5000/api/products`);
          setProducts(res.data)
      } catch (error) {
        console.log(error)
      }
    };
getProducts();
}, [cat])
```


