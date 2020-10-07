# Datamatiker opgave

## Obligatorisk Opgave Studieaktivitet

`Fagene -> Programmering Teknik -> Sep 2020`

Her kan du finde de forskellig links til de forskellige opgaver.

1. C# og Unit tests
2. **HTML, CSS og Bootstrap**
3. TypeScript
4. Simple REST Service
5. TCP-server

## HTML, CSS og Bootstrap

Denne opgaver er opgave 2 ud af 5 opgaver, i denne opgave skal vi bevise at vi kan finde ud af at arbejde med HTML, CSS og Boostrap.

### Opgave Beskrivelse

Du skal modernisere web-siden http://pele-easj.dk/ så den får et mere moderne udseende og bliver responsive.Du skal anvende HTML, CSS og Bootstrap.

- [x] Du skal bruge både internt og eksternt CSS.
- [x] Bootstrap skal anvende grid systemet og antagelig også andre features.
- [ ] Links til andre web-sider skal hardcodes, så de fører til de “gamle” side (du skal kun modernisere forsiden, ikke de underliggende sider).
- [x] HTML og CSS skal være valid - brug en validator.
- [x] Web-siden skal være tilgængelig i Azure.
- [ ] Hjælp til Azure: Use FTP, or use the Kudu console (“Upload files and folder using drag and drop”).

Tekst-dokumentet, som du afleverer i Wiseflow, skal foruden link til GitHub repository også indeholde link til Azure web-sted.

Hjælp til GitHub: Adding a file to a repository

### Opgave Besparelse

[Github Repositorie pele-easj.dk](https://github.com/taxidriver2192/Pele-easj.dk)

Valgte at gøre dette lidt modsat, da jeg var meget uenig i opsætningen af http://pele-easj.dk/ HTML, derfor valgte jeg ikke bare at tage source koden, hvor alle links i forvejen var sat ind og bygge boostrap på hans hjemmeside.

Valgte startet for starten af, Boostraps get startet template, som ser således ud.

```html
<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <!-- The above 3 meta tags *must* come first in the head; any other head content must come *after* these tags -->
    <title>Bootstrap 101 Template</title>

    <!-- Bootstrap -->
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/3.4.1/css/bootstrap.min.css" integrity="sha384-HSMxcRTRxnN+Bdg0JdbxYKrThecOKuH5zCYotlSAcp1+c8xmyTe9GYg1l9a69psu" crossorigin="anonymous">

    <!-- HTML5 shim and Respond.js for IE8 support of HTML5 elements and media queries -->
    <!-- WARNING: Respond.js doesn't work if you view the page via file:// -->
    <!--[if lt IE 9]>
      <script src="https://oss.maxcdn.com/html5shiv/3.7.3/html5shiv.min.js"></script>
      <script src="https://oss.maxcdn.com/respond/1.4.2/respond.min.js"></script>
    <![endif]-->
  </head>
  <body>
    <h1>Hello, world!</h1>

    <!-- jQuery (necessary for Bootstrap's JavaScript plugins) -->
    <script src="https://code.jquery.com/jquery-1.12.4.min.js" integrity="sha384-nvAa0+6Qg9clwYCGGPpDQLVpLNn0fRaROjHqs13t4Ggj3Ez50XnGQqc/r8MhnRDZ" crossorigin="anonymous"></script>
    <!-- Include all compiled plugins (below), or include individual files as needed -->
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/3.4.1/js/bootstrap.min.js" integrity="sha384-aJ21OjlMXNL5UyIl/XNwTMqvzeRMZH2w8c5cRVpzpU8Y5bApTppSuUkhZXN0VxHd" crossorigin="anonymous"></script>
  </body>
</html>
```

### Tog hans Tekster

Derfra valgte jeg at tage hans tekster, og sætte dem ind i forskellige elemeter i body taget.

Valgte kort sagt at lave et redesign, samt en bedre menu struktur. kort sagt var dette en opgave der blev lavet en del for hurtigt.

## Hvorfor tog det så lang tid?

Valgte at bruge største delen af tiden til at prøve at lave et script i python, der lavet en kopi af hans hjemmeside i plain tekst uden nogle HTML tags, hvor derefter at den ville autogenerer de rigtig HTML 5 tags og style det der efter.

Problemet var bare måde jeg prøvet at ramme de forskellige html elementer på, krævet at siden skulle havde en fast strugtur.

eksempel se dette billeder der beskriver en mulig struktur.

![](https://github.com/taxidriver2192/Pele-easj.dk/blob/master/problem.png?raw=true)

Her ville det være muligt at få fat i disse 3 links hver gang. med hjælp af `document.querySelector`

Så længe at han overholdte samme regler hver gang, men hans struktur skifter på hver eneste side, så da jeg har lavet unikke selekterer for at få fat i et element på forsiden `document.querySelector("body > p:nth-child(20)")` er det sjovt nok slet ikke samme struktur på nogle af de andre sider.

### Valgte at opgive

Jeg opgav fordi at der var en dead line, håber også i kan forså dette når i ser på denne HTML Strugtur.

```html
<html><head>
    <title>Peter Levinsky</title>
    <meta http-equiv="Content-Type" content="text/html; charset=iso-8859-1">
    <meta content="peterl" name="Author">
    <meta http-equiv="Cache-Control" content="max-age=3600">
    <link rel="stylesheet" type="text/css" href="./basic/lvstyle.css">
</head>
<body style="">
    <hr align="left" width="100%" size="2">
    <p align="center">Efterår / Autumn 2020</p>
    <hr align="left" width="100%" size="2">
    <p style="background-color: #00BFFF">

    &nbsp;<img src="downs/Icons/png/Tech.png" width="120" height="80" alt="SWC">
         &nbsp;&nbsp;&nbsp;&nbsp;<b>3 Semester : Teknik-faget</b><br>
    </p>
    <h1>DAT-3C</h1>
    <p>
        <a href="2020e-tek/SEMESTER.htm" style="font-size: 24px"><strong>Semester Plan (ugeplan)</strong></a>
    </p>
    <p>
        <a href="2020e-tek/General-information.htm">Information</a> |
        <a href="2020e-tek/GuidelinesAndObjectives.htm">formål</a> | Intranet<br>
        <br>
        <br>
    </p>
    <p></p>
    <hr align="left" width="100%" size="1">
    <p style="background-color: #ff9933">
    &nbsp;<img src="downs/Icons/png/elec.png" width="120" height="80" alt="Advanced Software Construction">
        &nbsp;&nbsp;&nbsp;&nbsp;<b>4<sup>th</sup> Semester : Elective - Advanced C# programming</b><br>
    </p>
    <h1>DAT E20 4.sem, VF Adv. softwar</h1>
    <p><a href="2020e-AvanceretCsharp/SEMESTER.htm" style="font-size: 24px"><strong>Semester Plan (ugeplan)</strong></a> </p>
    <p> <a href="2020e-AvanceretCsharp/General-information.htm">Information</a> | <a href="2020e-AvanceretCsharp/GuidelinesAndObjectives.htm">formål</a> | Intranet</p>
    <p>&nbsp;</p>
  <hr align="left" width="100%" size="1">
    <p style="background-color: #00FFFF">
    &nbsp;<img src="downs/Icons/png/SWC1.png" width="120" height="80" alt="Software Construction">
        &nbsp;&nbsp;&nbsp;&nbsp;<b>1<sup>ste</sup> Semester : Programming (SWC)</b><br>
    </p>
    <h1>DAT E20 1.sem, Programmering</h1>
    <p><a href="2020e-swc1/SEMESTER.htm" style="font-size: 24px"><strong>Semester Plan (ugeplan)</strong></a> </p>
    <p> <a href="2020e-swc1/General-information.htm">Information</a> | <a href="2020e-swc1/GuidelinesAndObjectives.htm">formål</a> | Intranet</p>
    <p>&nbsp;</p>
    <hr align="left" width="100%" size="2">
    <br>
    <table>
        <tbody>
            <tr>
                <td width="35%">
                    <p align="center">
                        <b>Programming link</b>
                    </p>
                </td>
                <td>
                    <p align="center">
                        <b>Study Link&nbsp;</b>
                    </p>
                </td>
                <td>
                    <p align="center">
                        <b>Archive&nbsp;</b>
                    </p>
                </td>
            </tr>
            <tr>
                <td valign="top">

                    <ul>
                        <li><a href="http://msdn.microsoft.com/en-us/library/618ayhy6.aspx">Microsoft C# reference</a></li>
                        <li>
                            <a href="http://msdn.microsoft.com/en-us/library/67ef8sbd.aspx">Microsoft C# programming guide</a><br>
                            <br>
                        </li>
                        <li>
                            &nbsp;<a href="https://docs.oracle.com/javase/8/docs/api/">
                                JAVA Documentation
                                (version8)
                            </a>
                        </li>
                        <li>
                            <a href="http://www.oracle.com/technetwork/java/javase/downloads/index.html">
                                &nbsp;Java
                                developement Kit downloads
                            </a>
                        </li>
                    </ul>
                    <p>&nbsp;
                    </p>
                </td>
                <td>
                    <ul>
                        <li><a href="https://helpdesk.easj.dk">Vejledninger,Mail,office365</a></li>
                        <li><a href="https://moodle.zealand.dk">Intranet / Moodle</a> (incl schedule / inkl skema)<br>
                        </li>
                    </ul>
                </td>
                <td>
                    <ul>
                        <li><a href="archive.htm">Tidligere undervisning</a>
                        </li><li><a href="archive.htm">Previous courses</a><br>
                        &nbsp;</li>
                        <li>HF brobygning <a href="downs/BigDataHFBro.pdf">Slides</a> | <a href="downs/Opgaver-BigData.pdf">Opgave</a> | <a href="downs/HF-Case-Opgave.pdf">Case opgave</a></li>
                    </ul>
                </td>
            </tr>
        </tbody>
    </table>
</body></html>
```

## Færdig kode

Derfor færdig gjorde jeg bare side via indsætte hans tekster til en kedelig boodstrap templet.

```html
<!doctype html>
<html lang="en">
  <head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" integrity="sha384-JcKb8q3iqJ61gNV9KGb8thSsNjpSL0n8PARn9HuZOnIxN0hoP+VmmDGMN5t9UJ0Z" crossorigin="anonymous">
    <link rel="stylesheet" href="css/style.css">
    <title>Hello, world!</title>
  </head>
  <body>
      <!-- Nav Start-->
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
        <div class="container">
        <a class="navbar-brand logo" href="#">Peter Levinsky</a>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarCollapse" aria-controls="navbarCollapse" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarCollapse">
          <ul class="navbar-nav mr-auto">
            <li class="nav-item active">
              <a class="nav-link" href="index.html">Forside <span class="sr-only">(current)</span></a>
            </li>
            <li class="nav-item">
                <a class="nav-link" href="#">Aktive hold</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#">Site Map</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#">Nyttige links</a>
              </li>
          </ul>
        </div>
    </div>
    </nav>
    <!--Nav slut-->

    <!-- Container start-->

    <main role="main" class="flex-shrink-0">
        <div class="container">
        <div class="col mb-5 pt-3">
          <h1 class="mt-5">Peter Levinsky (PELE)</h1>
          <span class="mb-5">Teacher at Datamatikeruddannelsen</span>
          <div class="pt-5">
          <h2>Mine informatiner</h2>
          <p>Mobil <a href="tel:+4550762600">50762600</a></p>
          <p>Adresse <a href="https://www.google.dk/maps/place/Magleg%C3%A5rdsvej+2,+4000+Roskilde/@55.6307194,12.0764997,17z/data=!3m1!4b1!4m5!3m4!1s0x46525fdd5598c3cd:0x66f8d04284c946b5!8m2!3d55.6307194!4d12.0786884">Maglegårdsvej 2</a></p>              
          </div>
        </div>
          
          <div class="jumbotron mt-3">
            <h3>DAT E20 4.Sem, VF Adv. Softwar</h3>
            <p class="lead">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam id dui congue magna egestas iaculis vel quis urna.<br> Quisque luctus odio non pretium dictum. Fusce fringilla, urna a ultrices elementum.</p>
            <a class="btn btn-sm btn-primary" href="#" role="button">Information</a>
            <a class="btn btn-sm btn-primary" href="#" role="button">Formål</a>
            <a class="btn btn-sm btn-primary" href="#" role="button">Intranet</a>

          </div>
          <div class="jumbotron mt-3">
            <h3>DAT E20 1.Sem, Programmering</h3>
            <p class="lead">Morbi convallis libero sem, eu vehicula justo varius vitae. Pellentesque nec tristique justo. Maecenas vitae sem vitae felis congue pretium nec a nisi. Aenean semper metus et ipsum venenatis ornare. Ut feugiat, lorem ut convallis laoreet, erat tortor bibendum lacus, vel finibus mauris erat vel nibh. Donec velit odio, consectetur sodales convallis porttitor, porta nec lectus.</p>
            <a class="btn btn-sm btn-primary" href="#" role="button">Information</a>
            <a class="btn btn-sm btn-primary" href="#" role="button">Formål</a>
            <a class="btn btn-sm btn-primary" href="#" role="button">Intranet</a>
          </div>
          <div class="jumbotron mt-3">
            <h3>DAT-3C</h3>
            <p class="lead">Vestibulum arcu lacus, tempor quis ornare sed, lobortis a est. Praesent pulvinar tincidunt quam quis pellentesque. Maecenas ultricies facilisis luctus. Maecenas venenatis nibh egestas egestas malesuada. Nam laoreet leo eu dolor finibus, nec volutpat lorem porttitor. Ut consectetur, ipsum sed placerat malesuada, eros diam placerat eros, quis fringilla nibh lacus eu nisi.<br><br>Donec sit amet facilisis lectus. Nullam eget aliquet augue, a dignissim quam. Integer mattis diam et diam aliquet blandit. Cras congue massa non blandit suscipit. Donec maximus sodales bibendum. Ut elit odio, interdum vitae augue a, blandit commodo leo. Vestibulum finibus sed nulla eu tincidunt. Donec sodales nunc arcu, quis fringilla est suscipit eget.</p>
            <a class="btn btn-sm btn-primary" href="#" role="button">Information</a>
            <a class="btn btn-sm btn-primary" href="#" role="button">Formål</a>
            <a class="btn btn-sm btn-primary" href="#" role="button">Intranet</a>
          </div>
        </div>
        
      </main>

    <!-- Container Slut-->

    <!-- Footer Start-->
    <footer class="footer mt-auto py-3" style="background-color: #f6f6f6;">
        <div class="container">
            <div class="row">
            <div class="col-lg-4 mb-5">
                <h4>Programming link</h4>
                <p><a href="#">Microsoft C# reference</a></p>
                <p><a href="#">Microsoft C# programming guide</a></p>
                <p><a href="#">JAVA Documentation (version8)</a></p>
                <p><a href="#">Java developement Kit downloads</a></p>
            </div>
            <div class="col-lg-4 mb-5">
                <h4>Programming link</h4>
                <p><a href="#">Microsoft C# reference</a></p>
                <p><a href="#">Microsoft C# programming guide</a></p>
                <p><a href="#">JAVA Documentation (version8)</a></p>
                <p><a href="#">Java developement Kit downloads</a></p>
            </div>
            <div class="col-lg-4">
                <h4>Programming link</h4>
                <p><a href="#">Microsoft C# reference</a></p>
                <p><a href="#">Microsoft C# programming guide</a></p>
                <p><a href="#">JAVA Documentation (version8)</a></p>
                <p><a href="#">Java developement Kit downloads</a></p>
            </div>
        </div>
        </div>
      </footer>
    <!-- Foooter Slut -->

    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js" integrity="sha384-DfXdz2htPH0lsSSs5nCTpuj/zy4C+OGpamoFVy38MVBnE+IbbVYUew+OrCXaRkfj" crossorigin="anonymous"></script>
    <script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.1/dist/umd/popper.min.js" integrity="sha384-9/reFTGAW83EW2RDu2S0VKaIzap3H66lZH81PoYlFhbGU+6BZp6G7niu735Sk7lN" crossorigin="anonymous"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js" integrity="sha384-B4gt1jrGC7Jh4AgTPSdUtOBvfO8shuf57BaghqFfPlYxofvL8/KUEfYiJOMMV+rV" crossorigin="anonymous"></script>
  </body>
</html>
```

Har ikke lavet noget link til Azure, men her er linket til [opgavens repositories](https://github.com/taxidriver2192/Pele-easj.dk).

## Billeder af færdig resulteret.

PC

![](https://github.com/taxidriver2192/Pele-easj.dk/blob/master/website-lg.png?raw=true)

Mobile

![](https://github.com/taxidriver2192/Pele-easj.dk/blob/master/website-xs.png?raw=true)