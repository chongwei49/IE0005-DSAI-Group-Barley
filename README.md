<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a name="readme-top"></a>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->



<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]


<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/chongwei49/IE0005-DSAI-Group-Barley">
    <img src="images/logo.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Flight Price Prediction Project</h3>

  <p align="center">
    <br />
    <a href="https://github.com/chongwei49/IE0005-DSAI-Group-Barley"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/chongwei49/IE0005-DSAI-Group-Barley">View Demo</a>
    ·
    <a href="https://github.com/chongwei49/IE0005-DSAI-Group-Barley/issues">Report Bug</a>
    ·
    <a href="https://github.com/chongwei49/IE0005-DSAI-Group-Barley/issues">Request Feature</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

[![Product Name Screen Shot][product-screenshot]](https://example.com)

The objective of the study is to analyse the flight booking dataset obtained from “Ease My Trip” website and to conduct various statistical hypothesis tests in order to get meaningful information from it. The 'Linear Regression' statistical algorithm would be used to train the dataset and predict a continuous target variable. 'Easemytrip' is an internet platform for booking flight tickets, and hence a platform that potential passengers use to buy tickets. A thorough study of the data will aid in the discovery of valuable insights that will be of enormous value to passengers.

#### Research Questions
* Does price vary with Airlines?
* How is the price affected when tickets are bought in just 1 or 2 days before departure?
* Does ticket price change based on the departure time and arrival time?
* How the price changes with change in Source and Destination?
* How does the ticket price vary between Economy and Business class?

#### DATA COLLECTION AND METHODOLOGY
Octoparse scraping tool was used to extract data from the website. Data was collected in two parts: one for economy class tickets and another for business class tickets. A total of 300261 distinct flight booking options was extracted from the site. Data was collected for 50 days, from February 11th to March 31st, 2022.
Data source was secondary data and was collected from Ease my trip website.


#### Dataset
Dataset contains information about flight booking options from the website Easemytrip for flight travel between India's top 6 metro cities. There are 300261 datapoints and 11 features in the cleaned dataset.

#### FEATURES

The various features of the cleaned dataset are explained below:
* Airline: The name of the airline company is stored in the airline column. It is a categorical feature having 6 different airlines.
* Flight: Flight stores information regarding the plane's flight code. It is a categorical feature.
* Source City: City from which the flight takes off. It is a categorical feature having 6 unique cities.
* Departure Time: This is a derived categorical feature obtained created by grouping time periods into bins. It stores information about the departure time and have 6 unique time labels.
* Stops: A categorical feature with 3 distinct values that stores the number of stops between the source and destination cities.
* Arrival Time: This is a derived categorical feature created by grouping time intervals into bins. It has six distinct time labels and keeps information about the arrival time.
* Destination City: City where the flight will land. It is a categorical feature having 6 unique cities.
* Class: A categorical feature that contains information on seat class; it has two distinct values: Business and Economy.
* Duration: A continuous feature that displays the overall amount of time it takes to travel between cities in hours.
* Days Left: This is a derived characteristic that is calculated by subtracting the trip date by the booking date.
* Price: Target variable stores information of the ticket price.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



### Built With

This section should list any major frameworks/libraries used to bootstrap your project. Leave any add-ons/plugins for the acknowledgements section. Here are a few examples.

* [![Python][Python.org]][Python-url]

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.

### Prerequisites

Have python install in your local system. (Select python version 3.10)
1. Python
  ```sh
  https://www.python.org/
  ```
2. After installation, Open the Run dialog box by pressing the Windows key + R.

   <picture>
     <img alt="Image Alt Text" src="http://i0.wp.com/www.alphr.com/wp-content/uploads/2021/11/1-44.png?w=398&ssl=1">
   </picture>
  
3. Type cmd and hit Enter.

   <picture>
    <img alt="Image Alt Text" src="http://i0.wp.com/www.alphr.com/wp-content/uploads/2021/11/2-45.png?w=398&ssl=1">
   </picture>
  
4. For a list of all the locations added to your PATH variable, type echo %PATH% into the command prompt, then press Enter.

   <picture>
    <img alt="Image Alt Text" src="http://i0.wp.com/www.alphr.com/wp-content/uploads/2021/11/2-46.png?w=398&ssl=1">
   </picture>
   
5. If you find a path like ```C:\Python39\Scripts``` (depending on your Python version), the path was added to the PATH variable.
   If pip hasn’t been added, try the next fix.

#### Fix 2: Add Pip to the PATH Environment Variable
Here’s how to manually add pip to the PATH environment using the Windows GUI and command prompt. Once the path has been added, open a new command window and try to install a pip package to see whether the problem was solved.

Add pip to the PATH using Windows GUI:

1. Open the Run dialog box by pressing the Windows key + R.

   <picture>
      <img alt="Image Alt Text" src="http://i0.wp.com/www.alphr.com/wp-content/uploads/2021/11/2-45.png?w=398&ssl=1">
   </picture>
   
2. Type in ```sysdm.cpl``` and press Enter to access System Properties.

   <picture>
      <img alt="Image Alt Text" src="http://i0.wp.com/www.alphr.com/wp-content/uploads/2021/11/5-27.png?w=394&ssl=1">
   </picture>
   
3. Select the Advanced tab, then Environment Variables.

   <picture>
      <img alt="Image Alt Text" src="http://i0.wp.com/www.alphr.com/wp-content/uploads/2021/11/6-27.png?w=405&ssl=1">
   </picture>
   
4. Go to System variables and select Path.

   <picture>
      <img alt="Image Alt Text" src="http://i0.wp.com/www.alphr.com/wp-content/uploads/2021/11/8-15.png?w=606&ssl=1">
   </picture>
   
5. Click the Edit button.

   <picture>
      <img alt="Image Alt Text" src="http://i0.wp.com/www.alphr.com/wp-content/uploads/2021/11/7-20.png?w=606&ssl=1">
   </picture>
   
6. Click on New to add the pip installation path. The default location is: ```C:\users\“your-username“\AppData\Programs\Python\Python39``` for Python 3.9.

   <picture>
      <img alt="Image Alt Text" src="http://i0.wp.com/www.alphr.com/wp-content/uploads/2021/11/7-20.png?w=606&ssl=1">
   </picture>
   
### Installation

1. Clone the repo
   ```
   git clone https://github.com/chongwei49/IE0005-DSAI-Group-Barley.git
   ```
2. Install Jupyter Notebook
   ```
   pip install notebook
   ```
3. To run the notebook
   ```
   jupyter notebook
   ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->
## Usage

Use this space to show useful examples of how a project can be used. Additional screenshots, code examples and demos work well in this space. You may also link to more resources.

_For more examples, please refer to the [Documentation](https://example.com)_

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ROADMAP -->
## Roadmap

- [x] Add Changelog
- [x] Add back to top links
- [ ] Add Additional Templates w/ Examples
- [ ] Add "components" document to easily copy & paste sections of the readme
- [ ] Multi-language Support
    - [ ] Chinese
    - [ ] Spanish

See the [open issues](https://github.com/othneildrew/Best-README-Template/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Chongwei - chongwei4949@example.com

Project Link: [https://github.com/your_username/repo_name](https://github.com/chongwei49/IE0005-DSAI-Group-Barley)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

Use this space to list resources you find helpful and would like to give credit to. I've included a few of my favorites to kick things off!

* [Choose an Open Source License](https://choosealicense.com)
* [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/tools/emoji-cheat-sheet)
* [Malven's Flexbox Cheatsheet](https://flexbox.malven.co/)
* [Malven's Grid Cheatsheet](https://grid.malven.co/)
* [Img Shields](https://shields.io)
* [GitHub Pages](https://pages.github.com)
* [Font Awesome](https://fontawesome.com)
* [React Icons](https://react-icons.github.io/react-icons/search)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/chongwei49/IE0005-DSAI-Group-Barley.svg?style=for-the-badge
[contributors-url]: https://github.com/chongwei49/IE0005-DSAI-Group-Barley/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/chongwei49/IE0005-DSAI-Group-Barley.svg?style=for-the-badge
[forks-url]: https://github.com/chongwei49/IE0005-DSAI-Group-Barley/network/members
[stars-shield]: https://img.shields.io/github/stars/chongwei49/IE0005-DSAI-Group-Barley.svg?style=for-the-badge
[stars-url]: https://github.com/chongwei49/IE0005-DSAI-Group-Barley/stargazers
[issues-shield]: https://img.shields.io/github/issues/chongwei49/IE0005-DSAI-Group-Barley.svg?style=for-the-badge
[issues-url]: https://github.com/chongwei49/IE0005-DSAI-Group-Barley/issues
[license-shield]: https://img.shields.io/github/license/chongwei49/IE0005-DSAI-Group-Barley.svg?style=for-the-badge
[license-url]: https://github.com/chongwei49/IE0005-DSAI-Group-Barley/blob/master/LICENSE.txt
[product-screenshot]: images/screenshot_flight.png
[Next.js]: https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white
[Next-url]: https://nextjs.org/
[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[Vue.js]: https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D
[Vue-url]: https://vuejs.org/
[Angular.io]: https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white
[Angular-url]: https://angular.io/
[Svelte.dev]: https://img.shields.io/badge/Svelte-4A4A55?style=for-the-badge&logo=svelte&logoColor=FF3E00
[Svelte-url]: https://svelte.dev/
[Laravel.com]: https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white
[Laravel-url]: https://laravel.com
[Bootstrap.com]: https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white
[Bootstrap-url]: https://getbootstrap.com
[JQuery.com]: https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white
[JQuery-url]: https://jquery.com 
[Python.org]: https://img.shields.io/badge/Python-0769AD?style=for-the-badge&logo=python&logoColor=yellow
[Python-url]: https://python.org 
[Pre-reg-1]: https://i0.wp.com/www.alphr.com/wp-content/uploads/2021/11/1-44.png?w=398&ssl=1
[Pre-reg-2]: https://i0.wp.com/www.alphr.com/wp-content/uploads/2021/11/2-45.png?w=398&ssl=1
