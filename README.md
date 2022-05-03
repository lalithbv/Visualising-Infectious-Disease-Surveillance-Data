# Visualising Infectious Disease Surveillance Data for Public Health

Surveillance is essential to improve public health as the threat of infectious diseases continues to rise. The consequences of an uncontrolled spread of infections can disrupt a country’s economy and social system. It can result in a significant loss of human life, and it poses an unprecedented threat to people’s livelihood, public health and food systems (Chriscaden, 2020). Insights obtained from public health monitoring systems enable authorities to come to a timely resolution and act accordingly. Although the National Notifiable Disease Surveillance System (NNDSS) was established by the Australian Government for the sole purpose of coordinating the national surveillance on an agreed list of communicable diseases, it has limited functionality in terms of reporting such as the lack of any interactive visualizations or forecasting methods. This project aims to demonstrate a robust reporting system for public health using Influenza disease surveillance data sourced from the NNDSS website, as explained below.

## Observations
1. I built an interactive dashboard using PowerBI that visualizes every attribute of the notified cases. As per my findings, children under the age of 15 years are the most affected age group which accounts for over 30% of the cases, Influenza-A virus is the dominant strain, and NSW is the most infected state in Australia.
2. I determined the seasonality of the flu to peak every winter i.e., from June to September by using the Error-Trend-Seasonality Model.
3. I constructed a Phylogenetic tree to visualize the evolution of the virus to be in the order of A(H1N1), B, C and A(H3N2) (Ludmir & Enquist, 2009).
4. I forecasted Influenza cases for 52 weeks by experimenting with the Holt-Winters method, LSTM, Facebook Prophet, and SARIMA model. I found the SARIMA model to be the most accurate model which shows yearly seasonality, peaking during winter.
5. I simulated the influenza epidemic based on a deterministic SEIR (Susceptible-Exposed-Infectious-Recovered) model that visualizes the impact of preventive measures like wearing a mask and incorporating social distancing to help reduce the spread of infection (He, Peng, & Sun, 2020). 

## Limitation
The only limitation of this project is that the dashboard is built on historical data. For the surveillance to be effective, the data should be analysed in near real-time. This can be accomplished by constructing data pipelines to extract, manipulate, and analyse data from the data source using Apache Beam and Python. Additionally, efforts should be made by the Australian government to create an API that streams national public health surveillance data to the population. 

To conclude, I see this project to be an effective public health reporting system that enables quick and informed decision making by the authorities thereby preventing yet another pandemic.

## References
- Chriscaden, K. (2020, October 13). Impact of covid-19 on people's livelihoods, their health and our Food Systems. Retrieved May 02, 2022, from https://www.who.int/news/item/13-10-2020-impact-of-covid-19-on-people's-livelihoods-their-health-and-our-food-systems
- He, S., Peng, Y., & Sun, K. (2020). Seir modeling of the COVID-19 and its dynamics. Nonlinear Dynamics, 101(3), 1667-1680. doi:10.1007/s11071-020-05743-y
- Ludmir, E. B., & Enquist, L. W. (2009). Viral genomes are part of the phylogenetic tree of life. Nature Reviews Microbiology, 7(8), 615-615. doi:10.1038/nrmicro2108-c4
