# Film Award Show Database

<h4>A group of sponsors sign to conduct an award show in the field of movies every year to appreciate the filmmakers, actors, and musicians who work on the movies. The sponsors sign a contract with the members of the jury panel for a certain period. A number of nominees are selected for each award by the popularity and box office collections of their particular films and songs. The jury carefully examines the nominees’ performance and selects a winner among them. Awards of various categories are given to winners, but every award can have only one winner. Each award is identified with a unique Id and its nominees for each award are uniquely identified with a nominee Id. The jury panel is decided by all the sponsors together. The show is made entertaining by performances like dancing, singing, funny anecdotes by the anchor. Each sponsor can hire several performers who act in different categories. Each performer has a unique Id. The awards are presented to the winners by award presenters who reveal the winners to the audience and hand the trophy to them. Each award presenter has a unique Id and he/she can give out one award.</h4>

<h3>Requirements</h3>
<ul>
  <li>
    <strong>Dynamics of the award show for a few years:</strong>
    <ul>
      <li>Overview of changes in format, categories, hosts, and audience engagement over the years.</li>
      <li>Analysis of trends, controversies, and memorable moments.</li>
    </ul>
  </li>
  <li>
    <strong>Winners for a particular award and the nominees:</strong>
    <ul>
      <li>List of winners and nominees for specific awards in different years.</li>
      <li>Details on the selection process, criteria, and any notable achievements.</li>
    </ul>
  </li>
  <li>
    <strong>People behind the screen for the show:</strong>
    <ul>
      <li>Information about sponsors, partners, and supporters.</li>
      <li>Bios of jury members, including their expertise and contributions to the selection process.</li>
    </ul>
  </li>
  <li>
    <strong>People who entertained the audience:</strong>
    <ul>
      <li>Profiles of hosts, performers, and presenters.</li>
      <li>Highlights of musical performances, comedy sketches, and special acts.</li>
    </ul>
  </li>
  <li>
    <strong>Overall view of film award shows over some time:</strong>
    <ul>
      <li>Analysis of the evolution of film award shows in terms of diversity, inclusivity, and representation.</li>
      <li>Comparison of different award ceremonies and their impact on the industry.</li>
    </ul>
  </li>
</ul>

<h3>Data Dictionary</h3>

<table border="1">
    <tr>
        <th>Sl. No</th>
        <th>Object (Entity)</th>
        <th>Name (Attribute)</th>
        <th>Type (Data type)</th>
        <th>Description</th>
        <th>Primary Key</th>
        <th>Foreign Key</th>
    </tr>
    <tr>
        <td>1</td>
        <td>Nominees</td>
        <td>NId</td>
        <td>Integer</td>
        <td>Unique Identification number for nominees</td>
        <td>Yes</td>
        <td>No</td>
    </tr>
    <tr>
        <td>2</td>
        <td>Nominees</td>
        <td>Nname</td>
        <td>String</td>
        <td>Name of the nominee</td>
        <td>No</td>
        <td>No</td>
    </tr>
    <tr>
        <td>3</td>
        <td>Nominees</td>
        <td>Gender</td>
        <td>String</td>
        <td>Gender of the nominee</td>
        <td>No</td>
        <td>No</td>
    </tr>
    <tr>
        <td>4</td>
        <td>Nominees</td>
        <td>Age</td>
        <td>Integer</td>
        <td>Age of the nominee</td>
        <td>No</td>
        <td>No</td>
    </tr>
    <tr>
        <td>5</td>
        <td>Nominees</td>
        <td>AId</td>
        <td>Integer</td>
        <td>Unique Identification number for awards</td>
        <td>No</td>
        <td>Yes</td>
    </tr>
    <tr>
        <td>6</td>
        <td>Awards</td>
        <td>AId</td>
        <td>Integer</td>
        <td>Unique Identification number for awards</td>
        <td>Yes</td>
        <td>No</td>
    </tr>
    <tr>
        <td>7</td>
        <td>Awards</td>
        <td>Aname</td>
        <td>String</td>
        <td>Name of the award</td>
        <td>No</td>
        <td>No</td>
    </tr>
    <tr>
        <td>8</td>
        <td>Awards</td>
        <td>Acat</td>
        <td>String</td>
        <td>Award belonging to the category</td>
        <td>No</td>
        <td>No</td>
    </tr>
    <tr>
        <td>9</td>
        <td>Sponsors</td>
        <td>Sid</td>
        <td>Integer</td>
        <td>Unique Identification number for sponsors</td>
        <td>Yes</td>
        <td>No</td>
    </tr>
    <tr>
        <td>10</td>
        <td>Sponsors</td>
        <td>Sname</td>
        <td>String</td>
        <td>Name of sponsors</td>
        <td>No</td>
        <td>No</td>
    </tr>
    <tr>
        <td>11</td>
        <td>Sponsors</td>
        <td>Speriod</td>
        <td>Integer</td>
        <td>The award show was sponsored for these number of years</td>
        <td>No</td>
        <td>No</td>
    </tr>
    <tr>
        <td>12</td>
        <td>Sponsors</td>
        <td>Syear</td>
        <td>Integer</td>
        <td>Year in which it was sponsored</td>
        <td>No</td>
        <td>No</td>
    </tr>
    <tr>
        <td>13</td>
        <td>Jury Panel</td>
        <td>JId</td>
        <td>Integer</td>
        <td>Unique Identification number for jury panel</td>
        <td>Yes</td>
        <td>No</td>
    </tr>
    <tr>
        <td>14</td>
        <td>Jury Panel</td>
        <td>Jname</td>
        <td>String</td>
        <td>Name of the jury</td>
        <td>No</td>
        <td>No</td>
    </tr>
    <tr>
        <td>15</td>
        <td>Jury Panel</td>
        <td>Jocc</td>
        <td>String</td>
        <td>Occupation of the jury</td>
        <td>No</td>
        <td>No</td>
    </tr>
    <tr>
        <td>16</td>
        <td>Performers</td>
        <td>PId</td>
        <td>Integer</td>
        <td>Unique Identification number for performers</td>
        <td>Yes</td>
        <td>No</td>
    </tr>
    <tr>
        <td>17</td>
        <td>Performers</td>
        <td>Pname</td>
        <td>String</td>
        <td>Name of performers</td>
        <td>No</td>
        <td>No</td>
    </tr>
    <tr>
        <td>18</td>
        <td>Performers</td>
        <td>Pcat</td>
        <td>String</td>
        <td>Category that performer belonging to</td>
        <td>No</td>
        <td>No</td>
    </tr>
    <tr>
        <td>19</td>
        <td>Performers</td>
        <td>Pyear</td>
        <td>Integer</td>
        <td>Year the performer had performed</td>
        <td>No</td>
        <td>No</td>
    </tr>
    <tr>
        <td>20</td>
        <td>Performers</td>
        <td>SId</td>
        <td>Integer</td>
        <td>Unique Identification Number for Sponsors</td>
        <td>No</td>
        <td>Yes</td>
    </tr>
    <tr>
        <td>21</td>
        <td>Award Presenters</td>
        <td>Id</td>
        <td>Integer</td>
        <td>Unique Identification number for award presenters</td>
        <td>Yes</td>
        <td>No</td>
    </tr>
    <tr>
        <td>22</td>
        <td>Award Presenters</td>
        <td>Name</td>
        <td>String</td>
        <td>Name of the award presenter</td>
        <td>No</td>
        <td>No</td>
    </tr>
    <tr>
        <td>23</td>
        <td>Award Presenters</td>
        <td>Occupation</td>
        <td>String</td>
        <td>Occupation of the award presenter</td>
        <td>No</td>
        <td>No</td>
    </tr>
    <tr>
        <td>24</td>
        <td>Award Presenters</td>
        <td>AId</td>
        <td>Integer</td>
        <td>Unique Identification number for awards</td>
        <td>No</td>
        <td>Yes</td>
    </tr>
    <tr>
        <td>25</td>
        <td>Winners</td>
        <td>NId</td>
        <td>Integer</td>
        <td>Unique Identification number for nominees</td>
        <td>Yes</td>
        <td>No</td>
    </tr>
    <tr>
        <td>26</td>
        <td>Winners</td>
        <td>Wyear</td>
        <td>Integer</td>
        <td>Winner won the award on that year</td>
        <td>Yes</td>
        <td>No</td>
    </tr>
    <tr>
        <td>27</td>
        <td>Winners</td>
        <td>JId</td>
        <td>Integer</td>
        <td>Unique Identification number for Jury panel</td>
        <td>No</td>
        <td>Yes</td>
    </tr>
    <tr>
        <td>28</td>
        <td>Winners</td>
        <td>Id</td>
        <td>Integer</td>
        <td>Unique Identification number for Award presenters</td>
        <td>No</td>
        <td>Yes</td>
    </tr>
    <tr>
        <td>29</td>
        <td>Funds</td>
        <td>Fyear</td>
        <td>Integer</td>
        <td>The Funds collected in that year</td>
        <td>Yes</td>
        <td>No</td>
    </tr>
    <tr>
        <td>30</td>
        <td>Funds</td>
        <td>Famount</td>
        <td>Integer</td>
        <td>The Amount given to funds</td>
        <td>Yes</td>
        <td>No</td>
    </tr>
    <tr>
        <td>31</td>
        <td>Funds</td>
        <td>Sid</td>
        <td>Integer</td>
        <td>Unique Identification number for Sponsors</td>
        <td>No</td>
        <td>Yes</td>
    </tr>
    <tr>
        <td>32</td>
        <td>Funds</td>
        <td>PId</td>
        <td>Integer</td>
        <td>Unique Identification number for Performers</td>
        <td>No</td>
        <td>Yes</td>
    </tr>
</table>

