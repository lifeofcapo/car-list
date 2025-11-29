# 🚗 Car Brands, Models & Parts Database

[![GitHub last commit](https://img.shields.io/github/last-commit/lifeofcapo/car-list)]()
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

**Save hundreds of euros on commercial APIs!** This is a comprehensive, ready-to-use database of car brands, models, and auto parts in structured JSON format.

---

## 📁 About The Project

This repository contains structured JSON data perfect for developing automotive applications, catalogs, e-commerce platforms, and comparison tools.

**What's inside?**

*   **`carBrands.json`**: Complete hierarchy from brand to model to generation
*   **`carParts.json`**: Extensive catalog of auto parts and related products

---

## 🗂️ Data Structure

### `carBrands.json`

Nested structure for accurate representation of automotive lineups.

```json
{
  "brand": "Audi",
  "models": [
    {
      "name": "100",
      "generations": [
        { "name": "C1", "yearFrom": 1968, "yearTo": 1976 },
        { "name": "C2", "yearFrom": 1976, "yearTo": 1982 }
      ]
    }
  ]
}
```

*   **`brand`**: Automotive brand name (e.g., Audi, BMW)
*   **`models`**: List of models for the brand
*   **`generations`**: List of generations with production years

**Statistics:**
*   🏷️ **95+** car brands
*   🚙 **Multiple** models per brand
*   📅 **Generations** with production years

### `carParts.json`

Catalog of auto parts and car care products.

```json
[
  {
    "slug": "absorber-bampera",
    "name": "Абсорбер (наполнитель бампера)"
  }
]
```

*   **`slug`**: Unique English identifier
*   **`name`**: Product name in Russian

**Statistics:**
*   🔧 **1200+** auto parts and car care items

---

## 💡 Use Cases

*   **Car Catalogs**: Building filters by brand, model, and year
*   **Auto Parts E-commerce**: Creating compatible parts finder systems
*   **Automotive Portals**: Enriching content with structured data
*   **Mobile Applications**: For taxi services, car sharing, maintenance
*   **Analytics & Research**: Automotive market analysis

---

## 🚀 Quick Start

1.  **Clone the repository**
    ```bash
    git clone https://github.com/your-username/your-repo-name.git
    ```

2.  **Use data in your project**

    **JavaScript example:**
    ```javascript
    const carBrands = require('./carBrands.json');
    const carParts = require('./carParts.json');

    // Find all Audi models
    const audi = carBrands.find(brand => brand.brand === "Audi");
    console.log(audi.models);

    // Find part by slug
    const absorber = carParts.find(part => part.slug === "absorber-bampera");
    console.log(absorber.name);
    ```

    **Python example:**
    ```python
    import json

    with open('carBrands.json', 'r') as f:
        car_brands = json.load(f)
    
    with open('carParts.json', 'r') as f:
        car_parts = json.load(f)
    ```

---

## 📊 Data Coverage

### Brands Included:
- European (Audi, BMW, Mercedes-Benz, Volkswagen, etc.)
- American (Ford, Chevrolet, Tesla, etc.)
- Asian (Toyota, Honda, Hyundai, etc.)

### Parts Categories:
- Engine components
- Suspension parts
- Electrical systems
- Car care products

---

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Add missing car brands or models
- Extend parts catalog
- Improve data accuracy

---

## 📄 License

MIT License - see the LICENSE file for details.

---

**Happy coding!** 🚀
