<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <title>Treasure Map with Dropdown</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f1e8;
        }
        .toolbar {
            background: rgba(0,0,0,0.85);
            color: #fff;
            padding: 12px 16px;
            position: sticky;
            top: 0;
            z-index: 10;
            display: flex;
            gap: 12px;
            align-items: center;
        }
        .map-wrapper {
            position: relative;
            width: 100%;
            overflow: auto;
        }
        .map-image {
            display: block;
            width: 100%;
            height: auto;
        }
        .pin {
            position: absolute;
            width: 34px;
            height: 34px;
            border-radius: 50%;
            border: 2px solid #222;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            color: #000;
            transform: translate(-50%, -50%);
            cursor: pointer;
            transition: transform 0.2s ease, box-shadow 0.2s ease;
        }
        .pin.easy {
            background: rgba(92, 184, 92, 0.9);
            color: #0b2e13;
        }
        .pin.medium {
            background: rgba(66, 139, 202, 0.9);
            color: #091e3a;
        }
        .pin.hard {
            background: rgba(240, 173, 78, 0.9);
            color: #4c2f05;
        }
        .pin.elite {
            background: rgba(217, 83, 79, 0.95);
            color: #420303;
        }
        .pin:hover, .pin.active {
            transform: translate(-50%, -50%) scale(1.2);
            box-shadow: 0 0 12px rgba(0,0,0,0.6);
        }
        .zoom-overlay {
            position: fixed;
            inset: 0;
            background: rgba(0,0,0,0.65);
            display: none;
            align-items: center;
            justify-content: center;
            z-index: 20;
            padding: 20px;
        }
        .zoom-overlay.visible {
            display: flex;
        }
        .zoom-card {
            background: #fff5df;
            border-radius: 12px;
            padding: 20px;
            box-shadow: 0 15px 35px rgba(0,0,0,0.35);
            display: flex;
            flex-direction: column;
            gap: 12px;
            max-width: 520px;
            width: 100%;
        }
        #zoom-canvas {
            width: 100%;
            height: auto;
            border-radius: 8px;
            border: 2px solid #7a5a32;
        }
        .zoom-footer {
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            gap: 8px;
        }
        #zoom-info {
            font-weight: bold;
            color: #4a351d;
        }
        #zoom-close {
            border: none;
            background: #4a351d;
            color: #fff;
            padding: 8px 16px;
            border-radius: 4px;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <div class="toolbar">
        <label for="treasure-select">Jump to treasure:</label>
        <select id="treasure-select">
            <option value="">-- choose location --</option>
            <option value="1">#1 (Medium)</option>
<option value="2">#2 (Medium)</option>
<option value="3">#3 (Easy)</option>
<option value="4">#4 (Easy)</option>
<option value="5">#5 (Medium)</option>
<option value="6">#6 (Hard)</option>
<option value="7">#7 (Easy)</option>
<option value="8">#8 (Hard)</option>
<option value="9">#9 (Medium)</option>
<option value="10">#10 (Medium)</option>
<option value="11">#11 (Medium)</option>
<option value="12">#12 (Hard)</option>
<option value="13">#13 (Medium)</option>
<option value="14">#14 (Easy)</option>
<option value="15">#15 (Medium)</option>
<option value="16">#16 (Easy)</option>
<option value="17">#17 (Elite)</option>
<option value="18">#18 (Medium)</option>
<option value="19">#19 (Easy)</option>
<option value="20">#20 (Easy)</option>
<option value="21">#21 (Hard)</option>
<option value="22">#22 (Medium)</option>
<option value="23">#23 (Medium)</option>
<option value="24">#24 (Medium)</option>
<option value="25">#25 (Easy)</option>
<option value="26">#26 (Medium)</option>
<option value="27">#27 (Hard)</option>
<option value="28">#28 (Easy)</option>
<option value="29">#29 (Hard)</option>
<option value="30">#30 (Hard)</option>
<option value="31">#31 (Hard)</option>
<option value="32">#32 (Hard)</option>
<option value="33">#33 (Medium)</option>
<option value="34">#34 (Hard)</option>
<option value="35">#35 (Hard)</option>
<option value="36">#36 (Elite)</option>
<option value="37">#37 (Medium)</option>
<option value="38">#38 (Medium)</option>
<option value="39">#39 (Easy)</option>
<option value="40">#40 (Hard)</option>
<option value="41">#41 (Elite)</option>
<option value="42">#42 (Hard)</option>
<option value="43">#43 (Medium)</option>
<option value="44">#44 (Hard)</option>
<option value="45">#45 (Medium)</option>
<option value="46">#46 (Hard)</option>
<option value="47">#47 (Hard)</option>
<option value="48">#48 (Hard)</option>
<option value="49">#49 (Hard)</option>
<option value="50">#50 (Medium)</option>
<option value="51">#51 (Easy)</option>
<option value="52">#52 (Medium)</option>
<option value="53">#53 (Medium)</option>
<option value="54">#54 (Medium)</option>
<option value="55">#55 (Elite)</option>
<option value="56">#56 (Medium)</option>
<option value="57">#57 (Medium)</option>
<option value="58">#58 (Medium)</option>
<option value="59">#59 (Easy)</option>
<option value="60">#60 (Elite)</option>
<option value="61">#61 (Medium)</option>
<option value="62">#62 (Hard)</option>
<option value="63">#63 (Medium)</option>
<option value="64">#64 (Hard)</option>
<option value="65">#65 (Hard)</option>
<option value="66">#66 (Hard)</option>
<option value="67">#67 (Hard)</option>
<option value="68">#68 (Hard)</option>
<option value="69">#69 (Medium)</option>
<option value="70">#70 (Elite)</option>
<option value="71">#71 (Medium)</option>
<option value="72">#72 (Medium)</option>
<option value="73">#73 (Hard)</option>
<option value="74">#74 (Medium)</option>
<option value="75">#75 (Elite)</option>
<option value="76">#76 (Hard)</option>
<option value="77">#77 (Hard)</option>
<option value="78">#78 (Medium)</option>
<option value="79">#79 (Elite)</option>
<option value="80">#80 (Elite)</option>
<option value="81">#81 (Hard)</option>
<option value="82">#82 (Hard)</option>
<option value="83">#83 (Easy)</option>
<option value="84">#84 (Medium)</option>
        </select>
        <span>Total locations: 84</span>
    </div>
    <div class="map-wrapper">
        <img src="zly2ggbzzey41.jpg" alt="Treasure Map" class="map-image" />
        <div class="pin medium" data-id="1" data-difficulty="Medium" data-px="8894.264551456918" data-py="3816.731892235582" style="left:88.94264551456918%;top:40.53023141377914%;"><span>1</span></div>
<div class="pin medium" data-id="2" data-difficulty="Medium" data-px="5242.481804507124" data-py="2729.641872940323" style="left:52.42481804507124%;top:28.98632125879073%;"><span>2</span></div>
<div class="pin easy" data-id="3" data-difficulty="Easy" data-px="5493.233599940469" data-py="3999.5440347127683" style="left:54.93233599940469%;top:42.47153057993807%;"><span>3</span></div>
<div class="pin easy" data-id="4" data-difficulty="Easy" data-px="6707.580186748883" data-py="4857.757995934065" style="left:67.07580186748882%;top:51.58498455913841%;"><span>4</span></div>
<div class="pin medium" data-id="5" data-difficulty="Medium" data-px="8148.968619204294" data-py="1934.060125899713" style="left:81.48968619204294%;top:20.53796459487855%;"><span>5</span></div>
<div class="pin hard" data-id="6" data-difficulty="Hard" data-px="3946.3317538759466" data-py="4068.630713713602" style="left:39.46331753875947%;top:43.20516845825212%;"><span>6</span></div>
<div class="pin easy" data-id="7" data-difficulty="Easy" data-px="8627.0564512087" data-py="4974.995718044742" style="left:86.270564512087%;top:52.8299428485159%;"><span>7</span></div>
<div class="pin hard" data-id="8" data-difficulty="Hard" data-px="4690.919789217539" data-py="1328.535704068876" style="left:46.90919789217539%;top:14.107844367302494%;"><span>8</span></div>
<div class="pin medium" data-id="9" data-difficulty="Medium" data-px="5819.822299517888" data-py="3783.1999361115413" style="left:58.198222995178874%;top:40.17415244888544%;"><span>9</span></div>
<div class="pin medium" data-id="10" data-difficulty="Medium" data-px="6634.271485858489" data-py="3497.337021975938" style="left:66.34271485858488%;top:37.13854754142443%;"><span>10</span></div>
<div class="pin medium" data-id="11" data-difficulty="Medium" data-px="5093.621196930344" data-py="4594.458125485984" style="left:50.936211969303436%;top:48.78897871387898%;"><span>11</span></div>
<div class="pin hard" data-id="12" data-difficulty="Hard" data-px="4397.997563512784" data-py="5091.461111031642" style="left:43.979975635127836%;top:54.0666997030014%;"><span>12</span></div>
<div class="pin medium" data-id="13" data-difficulty="Medium" data-px="4211.397776458318" data-py="5045.305251491558" style="left:42.113977764583176%;top:53.57656633207558%;"><span>13</span></div>
<div class="pin easy" data-id="14" data-difficulty="Easy" data-px="4591.61196541292" data-py="2482.9562730478065" style="left:45.9161196541292%;top:26.366743899838657%;"><span>14</span></div>
<div class="pin medium" data-id="15" data-difficulty="Medium" data-px="3745.528061268977" data-py="6033.950890688078" style="left:37.455280612689776%;top:64.07508644672484%;"><span>15</span></div>
<div class="pin easy" data-id="16" data-difficulty="Easy" data-px="8222.727799947163" data-py="4349.353961418347" style="left:82.22727799947162%;top:46.18619476922955%;"><span>16</span></div>
<div class="pin elite" data-id="17" data-difficulty="Elite" data-px="5384.631181628678" data-py="3313.798522346627" style="left:53.846311816286786%;top:35.18953512102184%;"><span>17</span></div>
<div class="pin medium" data-id="18" data-difficulty="Medium" data-px="7725.489977479414" data-py="5448.001334387289" style="left:77.25489977479414%;top:57.85283353920876%;"><span>18</span></div>
<div class="pin easy" data-id="19" data-difficulty="Easy" data-px="8904.009625816563" data-py="4724.420889350342" style="left:89.04009625816563%;top:50.1690654067149%;"><span>19</span></div>
<div class="pin easy" data-id="20" data-difficulty="Easy" data-px="8614.516563070438" data-py="4675.515905905381" style="left:86.14516563070438%;top:49.64973883301881%;"><span>20</span></div>
<div class="pin hard" data-id="21" data-difficulty="Hard" data-px="4054.1895014111983" data-py="5115.063121278533" style="left:40.54189501411199%;top:54.31733164785529%;"><span>21</span></div>
<div class="pin medium" data-id="22" data-difficulty="Medium" data-px="5187.256651980339" data-py="5621.784581631733" style="left:51.872566519803385%;top:59.69825402603518%;"><span>22</span></div>
<div class="pin medium" data-id="23" data-difficulty="Medium" data-px="7751.939580246113" data-py="2245.3455403596845" style="left:77.51939580246113%;top:23.843533400867415%;"><span>23</span></div>
<div class="pin medium" data-id="24" data-difficulty="Medium" data-px="5963.33230966324" data-py="3448.965313402158" style="left:59.63332309663241%;top:36.624883863248996%;"><span>24</span></div>
<div class="pin easy" data-id="25" data-difficulty="Easy" data-px="8679.201792499181" data-py="3288.587493091865" style="left:86.79201792499181%;top:34.921816853476315%;"><span>25</span></div>
<div class="pin medium" data-id="26" data-difficulty="Medium" data-px="4123.103725373374" data-py="4682.476062413717" style="left:41.23103725373374%;top:49.72364938317635%;"><span>26</span></div>
<div class="pin hard" data-id="27" data-difficulty="Hard" data-px="8075.22782539418" data-py="2898.9198669627276" style="left:80.7522782539418%;top:30.783900042080575%;"><span>27</span></div>
<div class="pin easy" data-id="28" data-difficulty="Easy" data-px="6040.244849373427" data-py="3858.2261938500033" style="left:60.402448493734276%;top:40.97086326696404%;"><span>28</span></div>
<div class="pin hard" data-id="29" data-difficulty="Hard" data-px="4221.446235208405" data-py="3691.642157366492" style="left:42.21446235208405%;top:39.201891869666476%;"><span>29</span></div>
<div class="pin hard" data-id="30" data-difficulty="Hard" data-px="8814.354941707821" data-py="1892.2716036667093" style="left:88.14354941707822%;top:20.094208385544327%;"><span>30</span></div>
<div class="pin hard" data-id="31" data-difficulty="Hard" data-px="8961.505564538475" data-py="4783.568428079696" style="left:89.61505564538474%;top:50.797158628859464%;"><span>31</span></div>
<div class="pin hard" data-id="32" data-difficulty="Hard" data-px="3557.5216738588256" data-py="5559.943085363486" style="left:35.57521673858825%;top:59.04155341789833%;"><span>32</span></div>
<div class="pin medium" data-id="33" data-difficulty="Medium" data-px="780.0099989649343" data-py="6689.428456917574" style="left:7.800099989649343%;top:71.03566376677895%;"><span>33</span></div>
<div class="pin hard" data-id="34" data-difficulty="Hard" data-px="970.1952379064405" data-py="7234.50893041843" style="left:9.701952379064405%;top:76.82392407792747%;"><span>34</span></div>
<div class="pin hard" data-id="35" data-difficulty="Hard" data-px="5220.463452534151" data-py="3275.1728717633823" style="left:52.20463452534151%;top:34.7793657402929%;"><span>35</span></div>
<div class="pin elite" data-id="36" data-difficulty="Elite" data-px="4702.089850865624" data-py="1254.897799874349" style="left:47.02089850865624%;top:13.325876604803536%;"><span>36</span></div>
<div class="pin medium" data-id="37" data-difficulty="Medium" data-px="5483.175947724004" data-py="4867.623581050899" style="left:54.83175947724004%;top:51.689748126270565%;"><span>37</span></div>
<div class="pin medium" data-id="38" data-difficulty="Medium" data-px="4368.238312850355" data-py="3692.4420696732623" style="left:43.68238312850355%;top:39.21038621294746%;"><span>38</span></div>
<div class="pin easy" data-id="39" data-difficulty="Easy" data-px="3852.5216229647885" data-py="3137.20179043699" style="left:38.52521622964788%;top:33.31423797851747%;"><span>39</span></div>
<div class="pin hard" data-id="40" data-difficulty="Hard" data-px="6412.304433651609" data-py="2417.133604034369" style="left:64.12304433651609%;top:25.667766847556216%;"><span>40</span></div>
<div class="pin elite" data-id="41" data-difficulty="Elite" data-px="6737.017666088115" data-py="2067.8201746226478" style="left:67.37017666088116%;top:21.958375009266728%;"><span>41</span></div>
<div class="pin hard" data-id="42" data-difficulty="Hard" data-px="7430.21422438214" data-py="2157.612629656204" style="left:74.30214224382141%;top:22.91188945158972%;"><span>42</span></div>
<div class="pin medium" data-id="43" data-difficulty="Medium" data-px="6719.485725707129" data-py="2290.4532389460687" style="left:67.19485725707129%;top:24.322536253011243%;"><span>43</span></div>
<div class="pin hard" data-id="44" data-difficulty="Hard" data-px="8898.530319855856" data-py="4927.745725579307" style="left:88.98530319855857%;top:52.32819077815979%;"><span>44</span></div>
<div class="pin medium" data-id="45" data-difficulty="Medium" data-px="9497.273204592333" data-py="2455.786837800606" style="left:94.97273204592334%;top:26.078229136674164%;"><span>45</span></div>
<div class="pin hard" data-id="46" data-difficulty="Hard" data-px="8475.474577584318" data-py="2311.361291654067" style="left:84.75474577584319%;top:24.544560811872856%;"><span>46</span></div>
<div class="pin hard" data-id="47" data-difficulty="Hard" data-px="3972.0091054669765" data-py="3852.314198295367" style="left:39.720091054669766%;top:40.90808323558848%;"><span>47</span></div>
<div class="pin hard" data-id="48" data-difficulty="Hard" data-px="6650.240536955381" data-py="2188.395461875367" style="left:66.50240536955381%;top:23.238775213713144%;"><span>48</span></div>
<div class="pin hard" data-id="49" data-difficulty="Hard" data-px="8267.702237463565" data-py="3041.8099492560414" style="left:82.67702237463565%;top:32.30126313322758%;"><span>49</span></div>
<div class="pin medium" data-id="50" data-difficulty="Medium" data-px="8681.362257097784" data-py="2669.758782664514" style="left:86.81362257097784%;top:28.35041714627285%;"><span>50</span></div>
<div class="pin easy" data-id="51" data-difficulty="Easy" data-px="7980.130609190239" data-py="4266.089526359583" style="left:79.80130609190239%;top:45.30200197896977%;"><span>51</span></div>
<div class="pin medium" data-id="52" data-difficulty="Medium" data-px="7869.0183745575205" data-py="5678.762243299043" style="left:78.6901837455752%;top:60.303305121578454%;"><span>52</span></div>
<div class="pin medium" data-id="53" data-difficulty="Medium" data-px="5873.631658222612" data-py="4555.326783214551" style="left:58.736316582226124%;top:48.37343934601838%;"><span>53</span></div>
<div class="pin medium" data-id="54" data-difficulty="Medium" data-px="2090.694919938187" data-py="6800.588684375663" style="left:20.90694919938187%;top:72.2160845744469%;"><span>54</span></div>
<div class="pin elite" data-id="55" data-difficulty="Elite" data-px="1775.478538269148" data-py="7491.409502412347" style="left:17.75478538269148%;top:79.55197517693901%;"><span>55</span></div>
<div class="pin medium" data-id="56" data-difficulty="Medium" data-px="3449.4432831305257" data-py="5897.579633975227" style="left:34.494432831305254%;top:62.626947371511385%;"><span>56</span></div>
<div class="pin medium" data-id="57" data-difficulty="Medium" data-px="4262.541029913706" data-py="5631.714527508882" style="left:42.62541029913706%;top:59.803701046075%;"><span>57</span></div>
<div class="pin medium" data-id="58" data-difficulty="Medium" data-px="5078.166979950565" data-py="5055.2627805516995" style="left:50.78166979950566%;top:53.6823062605044%;"><span>58</span></div>
<div class="pin easy" data-id="59" data-difficulty="Easy" data-px="4706.3831996636945" data-py="3288.909296893439" style="left:47.06383199663694%;top:34.92523411801465%;"><span>59</span></div>
<div class="pin elite" data-id="60" data-difficulty="Elite" data-px="7479.509591095746" data-py="5752.896644787428" style="left:74.79509591095747%;top:61.09054523507941%;"><span>60</span></div>
<div class="pin medium" data-id="61" data-difficulty="Medium" data-px="7789.660372791044" data-py="2680.0013379489064" style="left:77.89660372791045%;top:28.459183794721316%;"><span>61</span></div>
<div class="pin hard" data-id="62" data-difficulty="Hard" data-px="6667.652962273465" data-py="2578.265364679779" style="left:66.67652962273465%;top:27.378840019961547%;"><span>62</span></div>
<div class="pin medium" data-id="63" data-difficulty="Medium" data-px="6687.869394836542" data-py="3780.4416178123333" style="left:66.87869394836542%;top:40.14486160998549%;"><span>63</span></div>
<div class="pin hard" data-id="64" data-difficulty="Hard" data-px="4023.31784131715" data-py="4230.093472554917" style="left:40.2331784131715%;top:44.91975653132545%;"><span>64</span></div>
<div class="pin hard" data-id="65" data-difficulty="Hard" data-px="4375.712601014877" data-py="5850.430779847428" style="left:43.75712601014877%;top:62.12626929858159%;"><span>65</span></div>
<div class="pin hard" data-id="66" data-difficulty="Hard" data-px="6911.371755928385" data-py="2777.9492207537887" style="left:69.11371755928386%;top:29.4993014840585%;"><span>66</span></div>
<div class="pin hard" data-id="67" data-difficulty="Hard" data-px="8436.917179599079" data-py="4232.952929191762" style="left:84.36917179599078%;top:44.95012136765172%;"><span>67</span></div>
<div class="pin hard" data-id="68" data-difficulty="Hard" data-px="8596.524949370601" data-py="1527.1805935835173" style="left:85.96524949370603%;top:16.21727294874713%;"><span>68</span></div>
<div class="pin medium" data-id="69" data-difficulty="Medium" data-px="8000.935423601445" data-py="3823.397828125335" style="left:80.00935423601445%;top:40.60101760778735%;"><span>69</span></div>
<div class="pin elite" data-id="70" data-difficulty="Elite" data-px="4136.011352166716" data-py="2959.915478952551" style="left:41.36011352166717%;top:31.431618126288107%;"><span>70</span></div>
<div class="pin medium" data-id="71" data-difficulty="Medium" data-px="8818.225391052547" data-py="2539.5661589418887" style="left:88.18225391052546%;top:26.967889550195274%;"><span>71</span></div>
<div class="pin medium" data-id="72" data-difficulty="Medium" data-px="8449.659323997636" data-py="4353.509827655821" style="left:84.49659323997636%;top:46.230326299838815%;"><span>72</span></div>
<div class="pin hard" data-id="73" data-difficulty="Hard" data-px="5998.77312254667" data-py="4068.1066332367523" style="left:59.9877312254667%;top:43.199603198861126%;"><span>73</span></div>
<div class="pin medium" data-id="74" data-difficulty="Medium" data-px="9644.800759544445" data-py="2441.1677508148027" style="left:96.44800759544445%;top:25.922987690504435%;"><span>74</span></div>
<div class="pin elite" data-id="75" data-difficulty="Elite" data-px="949.7673556166919" data-py="6308.063368869054" style="left:9.49767355616692%;top:66.98591238047206%;"><span>75</span></div>
<div class="pin hard" data-id="76" data-difficulty="Hard" data-px="1475.7715343781483" data-py="6477.451695623427" style="left:14.757715343781483%;top:68.7846627973179%;"><span>76</span></div>
<div class="pin hard" data-id="77" data-difficulty="Hard" data-px="5005.3915001100395" data-py="2964.898840679787" style="left:50.05391500110039%;top:31.484536908567346%;"><span>77</span></div>
<div class="pin medium" data-id="78" data-difficulty="Medium" data-px="9006.406454323862" data-py="4010.8623341338525" style="left:90.06406454323862%;top:42.59172065555753%;"><span>78</span></div>
<div class="pin elite" data-id="79" data-difficulty="Elite" data-px="7837.50317181708" data-py="2398.7264265843196" style="left:78.3750317181708%;top:25.47229931596389%;"><span>79</span></div>
<div class="pin elite" data-id="80" data-difficulty="Elite" data-px="8321.796593625977" data-py="4937.1423965852755" style="left:83.21796593625977%;top:52.42797490267894%;"><span>80</span></div>
<div class="pin hard" data-id="81" data-difficulty="Hard" data-px="7491.0749717980425" data-py="4682.641561511669" style="left:74.91074971798042%;top:49.72540683351035%;"><span>81</span></div>
<div class="pin hard" data-id="82" data-difficulty="Hard" data-px="6118.757052233216" data-py="2685.4352249983467" style="left:61.18757052233216%;top:28.51688674735422%;"><span>82</span></div>
<div class="pin easy" data-id="83" data-difficulty="Easy" data-px="5644.291445981358" data-py="4943.771554897706" style="left:56.442914459813586%;top:52.49837055216848%;"><span>83</span></div>
<div class="pin medium" data-id="84" data-difficulty="Medium" data-px="8148.665234813852" data-py="4400.079434940785" style="left:81.48665234813852%;top:46.72485329659961%;"><span>84</span></div>
    </div>
    <div class="zoom-overlay" id="zoom-overlay">
        <div class="zoom-card">
            <canvas id="zoom-canvas" width="480" height="480"></canvas>
            <div class="zoom-footer">
                <span id="zoom-info">Select a treasure to preview</span>
                <button id="zoom-close">Close</button>
            </div>
        </div>
    </div>
    <script>
        const selectEl = document.getElementById('treasure-select');
        const pins = document.querySelectorAll('.pin');
        const mapImgEl = document.querySelector('.map-image');
        const zoomOverlay = document.getElementById('zoom-overlay');
        const zoomCanvas = document.getElementById('zoom-canvas');
        const zoomCtx = zoomCanvas.getContext('2d');
        const zoomInfo = document.getElementById('zoom-info');
        const zoomClose = document.getElementById('zoom-close');

        const mapBitmap = new Image();
        mapBitmap.src = mapImgEl.src;
        let bitmapReady = false;
        mapBitmap.onload = () => { bitmapReady = true; };

        const SAMPLE_SIZE = 600;

        function clearActive() {
            pins.forEach(pin => pin.classList.remove('active'));
        }

        function showZoom(px, py, label, difficulty) {
            if (!bitmapReady) return;
            const half = SAMPLE_SIZE / 2;
            const sx = Math.min(Math.max(px - half, 0), Math.max(mapBitmap.width - SAMPLE_SIZE, 0));
            const sy = Math.min(Math.max(py - half, 0), Math.max(mapBitmap.height - SAMPLE_SIZE, 0));
            zoomCtx.clearRect(0, 0, zoomCanvas.width, zoomCanvas.height);
            zoomCtx.drawImage(
                mapBitmap,
                sx, sy, SAMPLE_SIZE, SAMPLE_SIZE,
                0, 0, zoomCanvas.width, zoomCanvas.height
            );
            // draw crosshair marker
            zoomCtx.strokeStyle = '#ff3030';
            zoomCtx.lineWidth = 3;
            zoomCtx.beginPath();
            zoomCtx.moveTo(zoomCanvas.width / 2, 20);
            zoomCtx.lineTo(zoomCanvas.width / 2, zoomCanvas.height - 20);
            zoomCtx.moveTo(20, zoomCanvas.height / 2);
            zoomCtx.lineTo(zoomCanvas.width - 20, zoomCanvas.height / 2);
            zoomCtx.stroke();
            zoomCtx.beginPath();
            zoomCtx.arc(zoomCanvas.width / 2, zoomCanvas.height / 2, 18, 0, Math.PI * 2);
            zoomCtx.stroke();
            zoomInfo.textContent = `Treasure #${label} (${difficulty})`;
            zoomOverlay.classList.add('visible');
        }

        function focusPin(pin, shouldScroll = true) {
            if (!pin) return;
            clearActive();
            pin.classList.add('active');
            if (shouldScroll) {
                pin.scrollIntoView({ behavior: 'smooth', block: 'center', inline: 'center' });
            }
            const id = pin.dataset.id;
            const diff = pin.dataset.difficulty;
            const px = parseFloat(pin.dataset.px);
            const py = parseFloat(pin.dataset.py);
            selectEl.value = id;
            showZoom(px, py, id, diff);
        }

        selectEl.addEventListener('change', (event) => {
            const targetId = event.target.value;
            if (!targetId) {
                clearActive();
                zoomOverlay.classList.remove('visible');
                return;
            }
            const pin = document.querySelector(`.pin[data-id="{targetId}"]`.replace('{targetId}', targetId));
            if (pin) {
                focusPin(pin);
            }
        });

        pins.forEach(pin => {
            pin.addEventListener('click', () => {
                focusPin(pin, false);
            });
        });

        zoomClose.addEventListener('click', () => {
            zoomOverlay.classList.remove('visible');
        });

        zoomOverlay.addEventListener('click', (event) => {
            if (event.target === zoomOverlay) {
                zoomOverlay.classList.remove('visible');
            }
        });
    </script>
</body>
</html>
