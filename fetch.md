```
export async function getAplicationFromApi(limit) {
  try {
    const url = `${BASE_PATH}/products?_limit=${limit}`;
    const response = await fetch(url);
    const result = await response.json();
    return result;
  } catch (error) {
    console.log(error);
    return null;
  }
}
```
