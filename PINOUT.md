Detailed information on the WT32-ETH01 is available in the [unofficial guide to the WT32-ETH01](https://github.com/egnor/wt32-eth01)

# Pins 

<table>
  <tr> <td></td>
    <td align="right">EN ⏻</td>
    <td rowspan=13 align="center">WT32-ETH01<br>(ESP32)</td>
    <td>⭕ IO1 (reserved)</td> <td>💬 TXD</td>
  </tr>
  <tr> <td></td> <td align="right">GND ⏚</td> <td>⭕ IO3 (reserved)</td> <td>🗨️ RXD</td> </tr>
  <tr> <td></td> <td align="right">3.3V ⚡</td> <td>⭕ IO0 (reserved)</td> <td>⏱️ REFCLK and 💻 BOOT</td> </tr>
  <tr> <td align="right">pull low to reset</td> <td align="right">EN ⏻</td> <td>⏚ GND</td> <td></td> </tr>
  <tr> <td align="right">ADC1 CH4 📈</td> <td align="right">IO32 ↔️</td> <td>⬅️ IO39 (in only)</td> <td>📈 ADC1 CH3</td> </tr>
  <tr> <td align="right">ADC1 CH5 📈</td> <td align="right">IO33 ↔️</td> <td>⬅️ IO36 (in only)</td> <td>📈 ADC1 CH0</td> </tr>
  <tr> <td></td> <td align="right">IO5 ↔️</td> <td>↔️ IO15</td> <td>📉 ADC2 CH3</td> </tr>
  <tr> <td></td> <td align="right">IO17 ↔️</td> <td>↔️ IO14</td> <td>📉 ADC2 CH6</td> </tr>
  <tr> <td></td> <td align="right">GND ⏚</td> <td>▶️ IO12</td> <td>⚠️ must float at boot</td> </tr>
  <tr> <td></td> <td align="right">3.3V ⚡</td> <td>⬅️ IO35 (in only)</td> <td>📈 ADC1 CH7</td> </tr>
  <tr> <td></td> <td align="right">GND ⏚</td> <td>↔️ IO4</td> <td>📉 ADC2 CH0</td> </tr>
  <tr> <td></td> <td align="right">5V ⚡</td> <td>▶️ IO2</td> <td>⚠️ must float to program</td> </tr>
  <tr> <td align="right">ethernet link light</td> <td align="right">LINK 🖧</td> <td>⏚ GND</td> <td></td> </tr>
</table>

**LEGEND**<br>
⭕ - Not recommended for application use<br>
▶️ - Recommended output only (avoid driving externally)<br>
⬅️ - Input only<br>
↔️ - General purpose I/O<br>
📈 - Analog input on ADC1<br>
📉 - Analog input on ADC2 (conflicts with wi-fi)<br>
