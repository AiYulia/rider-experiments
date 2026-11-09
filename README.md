# Rider Experiments Dashboard

**Live:** https://aiyulia.github.io/rider-experiments/dashboard.html

Test read-outs for a ride-pooling service: four experiments on the rider journey, each with its design, sample size, 95% confidence interval, and the SQL behind the result. It is one self-contained HTML file that opens in any browser with no server, login, or external libraries, in light or dark mode and on a phone.

> **Demo on synthetic data.** The service, the city of Halvenport, its eight districts, the riders, and every number are made up. None of it is real data from any company.

## What's inside

- **Overview:** the headline result of each test, a test calendar drawn as route lines, and a summary card per test.
- **Recovery campaign:** the 30-day rebook rate for lapsed riders who got an offer against a random holdout, with confidence intervals, a day-by-day comeback curve, and the lift by time since the last ride.
- **Midday discount:** an 8-week test in four districts, after four baseline weeks. Weekly midday ride share and unfilled rush-hour requests for test and control districts, read as a difference-in-differences.
- **Alternatives:** the acceptance rate for each option shown after "No car available" (later pickup, nearby pickup point, shared ride with a short walk), split by rush hour and tracked by week.
- **Onboarding:** the 6-screen and 4-screen sign-up flows as screen-by-screen funnels, and the 7-day first-ride rate by weekly cohort.
- **Data & SQL:** a plain-language data dictionary grouped by journey stage, the Snowflake SQL behind every headline result, and a sample of raw rows.

## Built with

Python (pandas, numpy) for the data and the statistics, Snowflake-style SQL, and vanilla JavaScript with inline SVG charts.
