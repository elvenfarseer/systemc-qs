---
description: Some important notes
---

# Notes

## Prerequisite knowledge and knowledge for deep understanding

_lvalue, rvalue_ from C++ Reference with solid understanding

_numeric, vector, scalar_ from SystemC LRM

_proxy_ from SystemC LRM - depends on _lvalue, rvalue._

## Material on data types

All native C++ types are supported within SystemC application. SystemC provides additional data types within **sc\_dt** namespace to represent values with application-specific word lengths applicable to digital hardware. These data types are referred as _SystemC data types_.

For definition of _numeric, vector,_ and _scalar_ types refer to the SystemC LRM, here we provide a table for your convinience:

<table>
  <thead>
    <tr>
      <th style="text-align:left">Category</th>
      <th style="text-align:left">Signed</th>
      <th style="text-align:left">Unsigned</th>
      <th style="text-align:left">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Numeric</td>
      <td style="text-align:left">
        <p>sc_int</p>
        <p>sc_bigint</p>
        <p>sc_fixed</p>
        <p>sc_fixed_fast</p>
      </td>
      <td style="text-align:left">
        <p>sc_uint</p>
        <p>sc_biguint</p>
        <p>sc_ufixed</p>
        <p>sc_ufixed_fast</p>
      </td>
      <td style="text-align:left">
        <p>integer fixed-precision</p>
        <p>integer unlimited-precision</p>
        <p>fixed-point unlimited-precision</p>
        <p>fixed-point limited-precision</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Vector</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">
        <p>sc_bv</p>
        <p>sc_lv</p>
      </td>
      <td style="text-align:left">
        <p>bit (2-state)</p>
        <p>logic (4-state)</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Scalar</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">sc_logic</td>
      <td style="text-align:left">logic (4 state)</td>
    </tr>
  </tbody>
</table>

* Equality and bitwise operators can be used for all SystemC data types
* Arithmetic and relational operators can be used with numeric types only
* All SystemC data types implement method `length()`

\`\`





