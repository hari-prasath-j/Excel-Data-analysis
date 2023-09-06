<h2 style="height: 0px; text-align: left;"></h2><h2 style="clear: both; text-align: center;">Analysis of a coffee data set using Microsoft Excel</h2><p style="clear: both; text-align: center;">I have attached all those project files to this GitHub repo.</p><p style="clear: both;"></p><div class="separator" style="clear: both; text-align: center;"><a href="https://blogger.googleusercontent.com/img/a/AVvXsEidLAqmNukgTPFIzWDc5h1Q4WksSEU_PvlqbnDTvUo13k7zdbimDT7I8M6L5EeATXc7ChROZGTnriuoZBMFdob03dzn2R_Lg7oXdvDivSknd3iLxCBqH_iHXjfS5rzn7iQ35kWMdahjBo7WTXSXWswCRyQ_145cGZHBvLPvb75Fy_izfi0Ibxng72KhrBg" style="margin-left: 1em; margin-right: 1em;"><img alt="" data-original-height="338" data-original-width="600" height="342" src="https://blogger.googleusercontent.com/img/a/AVvXsEidLAqmNukgTPFIzWDc5h1Q4WksSEU_PvlqbnDTvUo13k7zdbimDT7I8M6L5EeATXc7ChROZGTnriuoZBMFdob03dzn2R_Lg7oXdvDivSknd3iLxCBqH_iHXjfS5rzn7iQ35kWMdahjBo7WTXSXWswCRyQ_145cGZHBvLPvb75Fy_izfi0Ibxng72KhrBg=w609-h342" width="609" /></a></div>&nbsp;<div><div style="text-align: center;"><b>Note : In case primary image can't load, right-click and view in a new tab.</b></div><br /><p></p><h3 style="clear: both; text-align: left;">1.Introduction</h3><p style="clear: both;">In this project, I'm going to analyse coffee shop sales by country, overall sales, top customers, and coffee types, and create an interactive dashboard for stakeholder presentations.</p><h3 style="clear: both; text-align: left;">2. Data Exploration:</h3><p style="clear: both;">In this data set, we have multiple sheets like order, customers, and product. We need to fill out blank data like customer name, email, country, coffee type, roast type, size, and unit price.</p><p style="clear: both;">Once I understand the dataset, this information (customer name, email, country) is on the customer sheet, and this information (coffee type, roast type, size, unit price) is on the order sheet. So we fill out the data using multiple formula such as VLOOKUP, IF conditions, Multification.</p><h3 style="clear: both; text-align: left;">3. Data Cleaning:</h3><p style="clear: both;">First, we extract the customer sheet using this formula.</p><p style="clear: both;">for customer name <b>=VLOOKUP(C2:C1001,customers!A2:B1001,2,0)</b></p><p style="clear: both;">for email ID <b>=IF(VLOOKUP(C2:C1001,customers!A2:C1001,3,0)=0,","VLOOKUP(C2:C1001,customers!A2:C1001,3,0))</b></p><p style="clear: both;">for country <b>=VLOOKUP(C2:C1001,customers!A2:G1001,7,0)</b></p><p style="clear: both;">Second, we extract the order sheet using this formula.</p><p style="clear: both;">for coffee type <b>=VLOOKUP(D2:D1001,products!A2:B49,2,0)</b></p><p style="clear: both;">for Roast type <b>=VLOOKUP(D2:D1001,products!A2:C49,3,0)</b></p><p style="clear: both;">size <b>=VLOOKUP(D2:D1001,products!A2:D49,4,0)</b></p><p style="clear: both;">Unit price <b>=VLOOKUP(D2:D1001,products!A2:E49,5,0)</b></p><p style="clear: both;">Third, we need to know the total sales.</p><p style="clear: both;">Unit price*quantity = total sales in the formula <b>=L2*E2.</b></p><p style="clear: both;">4th, we need to format the order date in Indian format, like date, month, or year, using the number tab.</p><p style="clear: both;">In addition, we must use the following formula to change the short name of the coffee type column to the full name of the coffee: <b>=IF(I2="Rob","Robusta," IF(I2="Exc","Excelsa"), IF(I2="Ara","Arabica"), IF(I2="Lib","Leberica"))</b></p><p style="clear: both;">and roast type using this formula:&nbsp;<b>=IF(J2="m","Medium",IF(J2="L","Light",IF(J2="D","Dark",)))</b></p><h3 style="clear: both; text-align: left;"><b>4. Data Analysis:</b></h3><div><ul style="text-align: left;"><li>Time Trend analysis</li></ul><div><b><div class="separator" style="clear: both; text-align: center;"><a href="https://blogger.googleusercontent.com/img/a/AVvXsEje4wq_OIJ7sf7xVd0CkWrimcVRhWnQArmfG8RUiVmg3b9yoN_ydEhYRoFrmcWMTkFwrw6LMKfpY9dYPHGFLcI8eeDaqwXUVTUhLArCK5dLi1i1OUh_Te-z1JSlg4tPxuRo9TGVmzzlwl5Si7MXSPNXWkHLNWrdEsGb-ijXfWkXIvZ49Pt8Y62PaRhvXNU" style="margin-left: 1em; margin-right: 1em;"><img alt="" data-original-height="145" data-original-width="470" height="144" src="https://blogger.googleusercontent.com/img/a/AVvXsEje4wq_OIJ7sf7xVd0CkWrimcVRhWnQArmfG8RUiVmg3b9yoN_ydEhYRoFrmcWMTkFwrw6LMKfpY9dYPHGFLcI8eeDaqwXUVTUhLArCK5dLi1i1OUh_Te-z1JSlg4tPxuRo9TGVmzzlwl5Si7MXSPNXWkHLNWrdEsGb-ijXfWkXIvZ49Pt8Y62PaRhvXNU=w465-h144" width="465" /></a></div><br /><br /></b></div></div><p style="clear: both;"></p><ul style="text-align: left;"><li>Top Selling Products</li></ul><p></p><p style="clear: both;"></p><div class="separator" style="clear: both; text-align: center;"><div class="separator" style="clear: both; text-align: center;"><div class="separator" style="clear: both; text-align: center;"><a href="https://blogger.googleusercontent.com/img/a/AVvXsEiNRl6YtfXfFpobohgcVQbczQn753oKsOetUEaYQY_2deRFjNuLkslmoxOY7xKDu-EPrTEoE52mDNyz-alxY41NjTcGvqRLTaymUJTs6XpTtl1JLcSflnFz3wiu09qwzWB8Q74ZRKwaYR1T9fkSVpRGR7CUOBAJZSWf5DxkHQv-1DX6FbZnG9BnVNAeKjI" style="margin-left: 1em; margin-right: 1em;"><img alt="" data-original-height="121" data-original-width="453" height="124" src="https://blogger.googleusercontent.com/img/a/AVvXsEiNRl6YtfXfFpobohgcVQbczQn753oKsOetUEaYQY_2deRFjNuLkslmoxOY7xKDu-EPrTEoE52mDNyz-alxY41NjTcGvqRLTaymUJTs6XpTtl1JLcSflnFz3wiu09qwzWB8Q74ZRKwaYR1T9fkSVpRGR7CUOBAJZSWf5DxkHQv-1DX6FbZnG9BnVNAeKjI=w465-h124" width="465" /></a></div><br /></div><div class="separator" style="clear: both; text-align: left;"><ul style="text-align: left;"><li>Sales By Country</li></ul></div><div class="separator" style="clear: both; text-align: center;"><a href="https://blogger.googleusercontent.com/img/a/AVvXsEiacMEFg6-Jjn92mqs3SfTAaTGFOVvo8xErhrhVLHXa5g6v7-3Fi2L9sPE2VGHWYzU97JC0WHA0akGf-Gr9zWTyNgWU9SUlVd3HRxYZv-Z7t10q2xAdTGFfCs-IRqj4pxpU75nsM4e-36NSBsPG-xnUcVFDPQRLTu8tO4KzUONXYT_8G2TDClAWTuOQ7f4" style="margin-left: 1em; margin-right: 1em;"><img alt="" data-original-height="97" data-original-width="369" height="122" src="https://blogger.googleusercontent.com/img/a/AVvXsEiacMEFg6-Jjn92mqs3SfTAaTGFOVvo8xErhrhVLHXa5g6v7-3Fi2L9sPE2VGHWYzU97JC0WHA0akGf-Gr9zWTyNgWU9SUlVd3HRxYZv-Z7t10q2xAdTGFfCs-IRqj4pxpU75nsM4e-36NSBsPG-xnUcVFDPQRLTu8tO4KzUONXYT_8G2TDClAWTuOQ7f4=w466-h122" width="466" /></a></div><br /><div style="text-align: left;"><ul style="text-align: left;"><li>Top 5 Customers</li></ul><div><div class="separator" style="clear: both; text-align: center;"><a href="https://blogger.googleusercontent.com/img/a/AVvXsEijEkBCYuFPzlYlkDmCWDqMz8DtoeUfNl45878IJDwRjfy_1Bfs7lw7McAwQssEgjrJPidsE_gUPnggmm4kEwfRrmRftZjDflye752mQ-skHO0pFmFiZxlc1rQDZz7hvqUv1zoyzGobxDCfLfy7tXZoVrGj2pqOG2egMER6PL_Qr7nGkIPOt2MRzv7Usag" style="margin-left: 1em; margin-right: 1em;"><img alt="" data-original-height="145" data-original-width="410" height="165" src="https://blogger.googleusercontent.com/img/a/AVvXsEijEkBCYuFPzlYlkDmCWDqMz8DtoeUfNl45878IJDwRjfy_1Bfs7lw7McAwQssEgjrJPidsE_gUPnggmm4kEwfRrmRftZjDflye752mQ-skHO0pFmFiZxlc1rQDZz7hvqUv1zoyzGobxDCfLfy7tXZoVrGj2pqOG2egMER6PL_Qr7nGkIPOt2MRzv7Usag=w468-h165" width="468" /></a></div><br /></div></div><h3 style="text-align: left;">5. Data Visualization:</h3></div><div class="separator" style="clear: both; text-align: center;"><div class="separator" style="clear: both; text-align: left;"><ul><li>Sales By Country</li></ul></div><div class="separator" style="clear: both;"><a href="https://blogger.googleusercontent.com/img/a/AVvXsEiacMEFg6-Jjn92mqs3SfTAaTGFOVvo8xErhrhVLHXa5g6v7-3Fi2L9sPE2VGHWYzU97JC0WHA0akGf-Gr9zWTyNgWU9SUlVd3HRxYZv-Z7t10q2xAdTGFfCs-IRqj4pxpU75nsM4e-36NSBsPG-xnUcVFDPQRLTu8tO4KzUONXYT_8G2TDClAWTuOQ7f4" style="margin-left: 1em; margin-right: 1em;"></a><div class="separator" style="clear: both; text-align: center;"><a href="https://blogger.googleusercontent.com/img/a/AVvXsEiacMEFg6-Jjn92mqs3SfTAaTGFOVvo8xErhrhVLHXa5g6v7-3Fi2L9sPE2VGHWYzU97JC0WHA0akGf-Gr9zWTyNgWU9SUlVd3HRxYZv-Z7t10q2xAdTGFfCs-IRqj4pxpU75nsM4e-36NSBsPG-xnUcVFDPQRLTu8tO4KzUONXYT_8G2TDClAWTuOQ7f4" style="margin-left: 1em; margin-right: 1em;"></a><a href="https://blogger.googleusercontent.com/img/a/AVvXsEiwPe5ZPnc4JduLudCKUmg2U4I52aGk5I3CEHgxz669FSzPb3RRdLZhs9MjVmWC4Z917ZBUPlsntrq3vVfvNGqr-gG_k7iRKzimNe_wII5letWJJSgtjwV8BdCsvhspP8ME1xMKGopmqDI_1BC7i809Mt-7MdqOO0vQH6OOuUwAl5hvgYKcjqCJQ0zXsyE" style="margin-left: 1em; margin-right: 1em;"><img alt="" data-original-height="329" data-original-width="895" height="171" src="https://blogger.googleusercontent.com/img/a/AVvXsEiwPe5ZPnc4JduLudCKUmg2U4I52aGk5I3CEHgxz669FSzPb3RRdLZhs9MjVmWC4Z917ZBUPlsntrq3vVfvNGqr-gG_k7iRKzimNe_wII5letWJJSgtjwV8BdCsvhspP8ME1xMKGopmqDI_1BC7i809Mt-7MdqOO0vQH6OOuUwAl5hvgYKcjqCJQ0zXsyE=w463-h171" width="463" /></a></div><br /></div><br /><div style="text-align: left;"><ul><li>Top 5 Customers</li></ul><div><div class="separator" style="clear: both; text-align: center;"><a href="https://blogger.googleusercontent.com/img/a/AVvXsEijEkBCYuFPzlYlkDmCWDqMz8DtoeUfNl45878IJDwRjfy_1Bfs7lw7McAwQssEgjrJPidsE_gUPnggmm4kEwfRrmRftZjDflye752mQ-skHO0pFmFiZxlc1rQDZz7hvqUv1zoyzGobxDCfLfy7tXZoVrGj2pqOG2egMER6PL_Qr7nGkIPOt2MRzv7Usag" style="margin-left: 1em; margin-right: 1em;"></a><div class="separator" style="clear: both; text-align: center;"><a href="https://blogger.googleusercontent.com/img/a/AVvXsEijEkBCYuFPzlYlkDmCWDqMz8DtoeUfNl45878IJDwRjfy_1Bfs7lw7McAwQssEgjrJPidsE_gUPnggmm4kEwfRrmRftZjDflye752mQ-skHO0pFmFiZxlc1rQDZz7hvqUv1zoyzGobxDCfLfy7tXZoVrGj2pqOG2egMER6PL_Qr7nGkIPOt2MRzv7Usag" style="margin-left: 1em; margin-right: 1em;"></a><a href="https://blogger.googleusercontent.com/img/a/AVvXsEjIzomS36hAwZtozPSN0T7FkFWd958JV1CS3_NAwOOqGMQPeM9WlaezXa1Fj2lqIu2VODwJCevjlgiMINXN994DIVy1mJK54Mh4QCpDSPaNiOf_lJww2EwmTLtmm96dEbgbVggdaAFYIdmaFAelJ6lPIgnI5x_R94TYj_iBn7ID2LcVhTCXl_85c_4cHGk" style="margin-left: 1em; margin-right: 1em;"><img alt="" data-original-height="421" data-original-width="898" height="219" src="https://blogger.googleusercontent.com/img/a/AVvXsEjIzomS36hAwZtozPSN0T7FkFWd958JV1CS3_NAwOOqGMQPeM9WlaezXa1Fj2lqIu2VODwJCevjlgiMINXN994DIVy1mJK54Mh4QCpDSPaNiOf_lJww2EwmTLtmm96dEbgbVggdaAFYIdmaFAelJ6lPIgnI5x_R94TYj_iBn7ID2LcVhTCXl_85c_4cHGk=w468-h219" width="468" /></a></div></div></div><div><br /></div></div></div><p style="clear: both;"></p><ul style="text-align: left;"><li>Total sales overtime</li></ul><div><div class="separator" style="clear: both; text-align: center;"><a href="https://blogger.googleusercontent.com/img/a/AVvXsEhRXcdpbXGPkndWz3kv0eYZpUWhyl4AiCFO37g58JlFjTL_ehz0pDnONmulCS4KFY8yQODbzojpR3Jx7XhjVuqnjZQnoaRehOwdQ3g-JvQuSa40YDXzlVTh0jmqB_v_AHWhQfx6CwBZKUaYAudFlw5IFhxI40nui_Edd439lj6NmgGoLUB2vF72QvSydVM" style="margin-left: 1em; margin-right: 1em;"><img alt="" data-original-height="750" data-original-width="1596" height="219" src="https://blogger.googleusercontent.com/img/a/AVvXsEhRXcdpbXGPkndWz3kv0eYZpUWhyl4AiCFO37g58JlFjTL_ehz0pDnONmulCS4KFY8yQODbzojpR3Jx7XhjVuqnjZQnoaRehOwdQ3g-JvQuSa40YDXzlVTh0jmqB_v_AHWhQfx6CwBZKUaYAudFlw5IFhxI40nui_Edd439lj6NmgGoLUB2vF72QvSydVM=w468-h219" width="468" /></a></div><div><br /></div><h3 style="text-align: left;">6. Creating Dashboard:</h3><p style="text-align: left;">After fine-tuning the data visualization, gather it on a new sheet and add the same slicer and timeline.</p><p style="text-align: left;"></p><div class="separator" style="clear: both; text-align: center;"><a href="https://blogger.googleusercontent.com/img/a/AVvXsEg4zTqanySIeu1qtbzA_pnMei3smzTXI27MSfX7og2KNlektwpwgB-Q_tKRAcu01Iqcpr7-sT08CBI56oEEFErWre4r4nyKJVl8d-d1EtErjI9Cw52O5LJJFmk5bfQiJyv9ZujRa2VoX9HhMPl3LTRWG3EH3tY4LZAP2m-3_6ZKmKf9jMJyKyswAhHCt6M" style="margin-left: 1em; margin-right: 1em;"><img alt="" data-original-height="642" data-original-width="1402" height="215" src="https://blogger.googleusercontent.com/img/a/AVvXsEg4zTqanySIeu1qtbzA_pnMei3smzTXI27MSfX7og2KNlektwpwgB-Q_tKRAcu01Iqcpr7-sT08CBI56oEEFErWre4r4nyKJVl8d-d1EtErjI9Cw52O5LJJFmk5bfQiJyv9ZujRa2VoX9HhMPl3LTRWG3EH3tY4LZAP2m-3_6ZKmKf9jMJyKyswAhHCt6M=w467-h215" width="467" /></a></div><br /><br /><p></p><h3 style="text-align: left;">6. Insights and Findings:</h3></div><ol style="text-align: left;"><li>We need more concentration in Ireland and the United Kingdom to improve our business growth.</li><li>2022 sales dropped 51% compared to 2021.</li></ol><p style="clear: both;"></p><div class="separator" style="clear: both; text-align: center;"><br /></div><br /><br /><p></p><p style="clear: both;"><br /></p><p style="clear: both;"><br /></p><p style="clear: both;"><br /></p><p style="clear: both;"><br /></p><p style="clear: both;"><br /></p><p style="clear: both;"><br /></p><p style="clear: both;"><br /></p><p style="clear: both;"><br /></p><p style="clear: both;"><br /></p></div>
