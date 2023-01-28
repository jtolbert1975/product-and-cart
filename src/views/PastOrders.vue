<template>
   <main className="wrapper">
        <h1>Past Orders</h1>

        <table className="product-table">
          <thead>
            <tr>
              <td><span className="sr-only">Product Image</span></td>
              <td>Product</td>
              <td>Price</td>
              <td>Quantity</td>
              <td>Total</td>
              <td><span className="sr-only">Actions</span></td>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td><i className="icofont-carrot icofont-4x" /></td>
              <td>Carrot</td>
              <td>$1.00</td>
              <td>1</td>
              <td>$1.00</td>
              <td><button className="btn btn-dark">Add</button></td>
            </tr>
            <tr>
              <td><i className="icofont-banana icofont-4x" /></td>
              <td>Banana</td>
              <td>$0.50</td>
              <td>10</td>
              <td>$5.00</td>
              <td><button className="btn btn-dark">Add</button></td>
            </tr>
          </tbody>
        </table>
      </main>
</template>
