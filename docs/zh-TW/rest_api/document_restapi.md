# REST 說明文件

## Datatables API

TEJ REST API提供一套簡易的方式來存取TEJ 資料庫，並輸出json或xml格式。您也可以透過各種程式或工具快速取得需要的資料。

您也可以在此取得 OPEN API(Swagger) 說明文件:

!!! tip "提示"

    您可以直接使用瀏覽器(Browser)來取得資料，也可以透過工具程式例如 curl, wget ...等

### 使用方法

??? info "In"

    ``` html
    GET https://api.tej.com.tw/api/datatables/{datatable_code}/{table_code}.{format}?<row_filter_criteria>
    ```


!!! example "以上市(櫃)未調整股價(日)(TWN/APRCD)為例"

    === "json"

        ``` sh
        GET https://api.tej.com.tw/api/datatables/TWN/APRCD.json?api_key="YOURAPIKEY"
        ```

    === "xml"

        ``` sh
        GET https://api.tej.com.tw/api/datatables/TWN/APRCD.xml?api_key="YOURAPIKEY"
        ```

回應資料如下

??? success "out"
    
    === "json"
        <div style="max-height: 500px; overflow: auto;">
        ``` json
        {
            "datatable":{
                "data":[
                    [
                        "Y9999",
                        "2018-05-15T00:00:00Z",
                        10965.08,
                        10978.38,
                        10874.73,
                        10874.73,
                        7266464,
                        153439891,
                        -0.7091,
                        0.3794,
                        699338771,
                        32392361,
                        null,
                        null,
                        -0.7116,
                        100,
                        100,
                        1259280,
                        null,
                        16.4,
                        null,
                        1.81,
                        "",
                        1.14,
                        null,
                        4,
                        -77.66,
                        "",
                        "",
                        "",
                        "TSE"
                    ],
                    [
                        "Y9999",
                        "2018-05-14T00:00:00Z",
                        10938.3,
                        10970.24,
                        10908.86,
                        10952.39,
                        7222849,
                        145417795,
                        0.8602,
                        0.3677,
                        699338777,
                        32622949,
                        null,
                        null,
                        0.8565,
                        100,
                        100,
                        1168845,
                        null,
                        16.52,
                        null,
                        1.82,
                        "",
                        1.15,
                        null,
                        3.97,
                        93.41,
                        "",
                        "",
                        "",
                        "TSE"
                    ],
                    [
                        "Y9999",
                        "2018-05-11T00:00:00Z",
                        10808.4,
                        10874.63,
                        10808.4,
                        10858.98,
                        7399223,
                        165763227,
                        0.9179,
                        0.4002,
                        699338982,
                        32344168,
                        null,
                        null,
                        0.9137,
                        100,
                        100,
                        1248505,
                        null,
                        16.38,
                        null,
                        1.81,
                        "",
                        1.14,
                        null,
                        4.14,
                        98.77,
                        "",
                        "",
                        "",
                        "TSE"
                    ],
                    [
                        "Y9999",
                        "2018-05-10T00:00:00Z",
                        10731.68,
                        10782.06,
                        10731.68,
                        10760.21,
                        7062376,
                        139276989,
                        0.5312,
                        0.3551,
                        699339661,
                        32049300,
                        null,
                        null,
                        0.5298,
                        100,
                        100,
                        1102455,
                        null,
                        16.23,
                        null,
                        1.79,
                        "",
                        1.12,
                        null,
                        4.17,
                        56.86,
                        "",
                        "",
                        "",
                        "TSE"
                    ],
                    [
                        "Y9999",
                        "2018-05-09T00:00:00Z",
                        10692.89,
                        10748.6,
                        10689.81,
                        10703.35,
                        7074991,
                        135741987,
                        0.112,
                        0.3496,
                        695033357,
                        31547472,
                        null,
                        null,
                        0.1119,
                        100,
                        100,
                        1123979,
                        null,
                        16.14,
                        null,
                        1.78,
                        "",
                        1.12,
                        null,
                        4.2,
                        11.97,
                        "",
                        "",
                        "",
                        "TSE"
                    ],
                    [
                        "Y9999",
                        "2018-05-08T00:00:00Z",
                        10610.44,
                        10691.38,
                        10609.04,
                        10691.38,
                        7064737,
                        133691609,
                        0.8154,
                        0.333,
                        695033357,
                        31509651,
                        null,
                        null,
                        0.8121,
                        100,
                        100,
                        1042424,
                        null,
                        16.12,
                        null,
                        1.78,
                        "",
                        1.12,
                        null,
                        4.21,
                        86.47,
                        "",
                        "",
                        "",
                        "TSE"
                    ],
                    [
                        "Y9999",
                        "2018-05-07T00:00:00Z",
                        10581.78,
                        10632.62,
                        10555.56,
                        10604.91,
                        6108995,
                        126046786,
                        0.7174,
                        0.282,
                        695033431,
                        31247223,
                        null,
                        null,
                        0.7149,
                        100,
                        100,
                        956892,
                        null,
                        15.99,
                        null,
                        1.76,
                        "",
                        1.11,
                        null,
                        4.22,
                        75.54,
                        "",
                        "",
                        "",
                        "TSE"
                    ],
                    [
                        "Y9999",
                        "2018-05-04T00:00:00Z",
                        10516.45,
                        10566.37,
                        10500.97,
                        10529.37,
                        5653857,
                        120828141,
                        0.1445,
                        0.2961,
                        695035128,
                        31017892,
                        null,
                        null,
                        0.1444,
                        100,
                        100,
                        958698,
                        null,
                        15.87,
                        null,
                        1.75,
                        "",
                        1.1,
                        null,
                        4.25,
                        15.19,
                        "",
                        "",
                        "",
                        "TSE"
                    ],
                    [
                        "Y9999",
                        "2018-05-03T00:00:00Z",
                        10578.98,
                        10578.98,
                        10509.03,
                        10514.18,
                        5841156,
                        124397511,
                        -0.9853,
                        0.3034,
                        695035857,
                        30994925,
                        null,
                        null,
                        -0.9902,
                        100,
                        100,
                        993874,
                        null,
                        15.86,
                        null,
                        1.75,
                        "",
                        1.1,
                        null,
                        4.25,
                        -104.63,
                        "",
                        "",
                        "",
                        "TSE"
                    ],
                    [
                        "Y9999",
                        "2018-05-02T00:00:00Z",
                        10665.52,
                        10683.9,
                        10601.1,
                        10618.81,
                        6324416,
                        129078743,
                        -0.3666,
                        0.3245,
                        695043607,
                        31304327,
                        null,
                        null,
                        -0.3673,
                        100,
                        100,
                        1023004,
                        null,
                        16.02,
                        null,
                        1.77,
                        "",
                        1.11,
                        null,
                        4.21,
                        -39.07,
                        "",
                        "",
                        "",
                        "TSE"
                    ]
                ],
                "columns":[
                    {
                        "name":"coid",
                        "type":"char(7)",
                        "description":"交易所及櫃檯買賣中心所訂的代碼",
                        "unit":"-"
                    },
                    {
                        "name":"mdate",
                        "type":"datetime",
                        "description":"年月日",
                        "unit":"-"
                    },
                    {
                        "name":"open_d",
                        "type":"decimal(8,2)",
                        "description":"open_d",
                        "unit":"-"
                    },
                    {
                        "name":"high_d",
                        "type":"decimal(8,2)",
                        "description":"high_d",
                        "unit":"-"
                    },
                    {
                        "name":"low_d",
                        "type":"decimal(8,2)",
                        "description":"low_d",
                        "unit":"-"
                    },
                    {
                        "name":"close_d",
                        "type":"decimal(8,2)",
                        "description":"close_d",
                        "unit":"-"
                    },
                    {
                        "name":"volume",
                        "type":"decimal(9,0)",
                        "description":"當日若成交量為0，表示當日無交易，此時之開高低收價格為前一日之收盤價除加權指數(Y9999)外，產業部分由TEJ衍生，為成分股成交量之加總",
                        "unit":"T"
                    },
                    {
                        "name":"amount",
                        "type":"decimal(12,0)",
                        "description":"未無考慮公眾流通量(free float)；除加權指數(Y9999)外，產業部分由TEJ衍生",
                        "unit":"NTD,T"
                    },
                    {
                        "name":"roi",
                        "type":"decimal(9,4)",
                        "description":"當OTC轉至TSE交易時，報酬率以承銷價計算，若無承銷價，則以OTC最後一天之收盤價來計算。",
                        "unit":"%"
                    },
                    {
                        "name":"turnover",
                        "type":"decimal(9,4)",
                        "description":"個股=成交量/流通股數*100(%)；產業＝產業成交量總額/產業流通股數*100(%)",
                        "unit":"%"
                    },
                    {
                        "name":"outstanding",
                        "type":"decimal(12,0)",
                        "description":"流通在外股數(千股)",
                        "unit":"T"
                    },
                    {
                        "name":"mv",
                        "type":"decimal(12,0)",
                        "description":"個股：流通在外股數(個股)*未調整收盤價；指數：為反映該股票於市場上實際可流通之股數，會將各成分股之公開發行股數扣除長期性、策略性持  股比例，故計算指數市值時，若該指數有考慮公眾流通量(交易所與FTSE合編的指數)，則市值公式=未調整收盤價*流通在外股數(個股)*公眾流通係數(此係數由交易所提供)",
                        "unit":"NTD,T"
                    },
                    {
                        "name":"bid",
                        "type":"decimal(7,2)",
                        "description":"最後揭示買價",
                        "unit":"NTD"
                    },
                    {
                        "name":"offer",
                        "type":"decimal(7,2)",
                        "description":"最後揭示賣價",
                        "unit":"NTD"
                    },
                    {
                        "name":"roib",
                        "type":"decimal(9,4)",
                        "description":"報酬率-Ln",
                        "unit":"-"
                    },
                    {
                        "name":"mv_pct",
                        "type":"decimal(7,3)",
                        "description":"mv_pct",
                        "unit":"-"
                    },
                    {
                        "name":"amt_pct",
                        "type":"decimal(7,3)",
                        "description":"amt_pct",
                        "unit":"-"
                    },
                    {
                        "name":"trn_d",
                        "type":"decimal(9,0)",
                        "description":"成交筆數(筆)",
                        "unit":"-"
                    },
                    {
                        "name":"per_tse",
                        "type":"decimal(7,2)",
                        "description":"per_tse",
                        "unit":"-"
                    },
                    {
                        "name":"per_tej",
                        "type":"decimal(7,2)",
                        "description":"per_tej",
                        "unit":"-"
                    },
                    {
                        "name":"pbr_tse",
                        "type":"decimal(7,2)",
                        "description":"pbr_tse",
                        "unit":"-"
                    },
                    {
                        "name":"pbr_tej",
                        "type":"decimal(7,2)",
                        "description":"pbr_tej",
                        "unit":"-"
                    },
                    {
                        "name":"limit",
                        "type":"char(1)",
                        "description":"股票漲停：”+”；跌停：”-“",
                        "unit":"-"
                    },
                    {
                        "name":"tej_psr",
                        "type":"decimal(7,2)",
                        "description":"=市值/最近4季合計之營收，TEJ提供本欄位需搭配財報發佈時間，目前更新方式為每年6/1、10/1、及12/1更新營收資料，首次上市需滿一年的次一年度1/1始計算。",
                        "unit":"-"
                    },
                    {
                        "name":"div_yid",
                        "type":"decimal(7,2)",
                        "description":"即每股股利與當日名目收盤價之比值，其中每股股利=該公司每股配發之現金股利+盈餘轉增資股票股利。此欄位由交易所提供，其中97/07/17以前之資料交易所計算方式係採取前一筆有發放股利之資料來計算，即當年度公司不發放股利，則以前一年度或更早以前的股利資料計算不合理，故97/07/17交易所已修正為以該年度之資料來計算，故前後期資料會有所差異。",
                        "unit":"%"
                    },
                    {
                        "name":"tej_cdiv",
                        "type":"decimal(7,2)",
                        "description":"=現金股利總額/市值*100%，TEJ提供",
                        "unit":"%"
                    },
                    {
                        "name":"clschg",
                        "type":"decimal(8,2)",
                        "description":"股價漲跌(元)",
                        "unit":"-"
                    },
                    {
                        "name":"xattn1",
                        "type":"char(1)",
                        "description":"公佈異常交易有價證券之交易資訊",
                        "unit":"-"
                    },
                    {
                        "name":"xattn2",
                        "type":"char(1)",
                        "description":"對連續公佈注意交易資訊之有價證券採取之處置措施",
                        "unit":"-"
                    },
                    {
                        "name":"xstat1",
                        "type":"char(1)",
                        "description":"全額交割(Y)",
                        "unit":"-"
                    },
                    {
                        "name":"pmkt",
                        "type":"char(5)",
                        "description":"市場別",
                        "unit":"-"
                    }
                ]
            },
            "meta":{
                "next_cursor_id":"uRKchQOqqW"
            }
        }

        ```
        </div>

    === "xml"
        <div style="max-height: 500px; overflow: auto;">
        ``` xml
        <tej-response>
            <datatable>
                <data type="array">
                    <datum type="array">
                        <datum>Y9999</datum>
                        <datum type="dateTime">2018-05-15T00:00:00Z</datum>
                        <datum type="float">10965.08</datum>
                        <datum type="float">10978.38</datum>
                        <datum type="float">10874.73</datum>
                        <datum type="float">10874.73</datum>
                        <datum type="float">7266464</datum>
                        <datum type="float">153439891</datum>
                        <datum type="float">-0.7091</datum>
                        <datum type="float">0.3794</datum>
                        <datum type="float">699338771</datum>
                        <datum type="float">32392361</datum>
                        <datum nil="true"/>
                        <datum nil="true"/>
                        <datum type="float">-0.7116</datum>
                        <datum type="float">100.000</datum>
                        <datum type="float">100.000</datum>
                        <datum type="float">1259280</datum>
                        <datum nil="true"/>
                        <datum type="float">16.40</datum>
                        <datum nil="true"/>
                        <datum type="float">1.81</datum>
                        <datum/>
                        <datum type="float">1.14</datum>
                        <datum nil="true"/>
                        <datum type="float">4.00</datum>
                        <datum type="float">-77.66</datum>
                        <datum/>
                        <datum/>
                        <datum/>
                        <datum>TSE</datum>
                    </datum>
                    <datum type="array">
                        <datum>Y9999</datum>
                        <datum type="dateTime">2018-05-14T00:00:00Z</datum>
                        <datum type="float">10938.30</datum>
                        <datum type="float">10970.24</datum>
                        <datum type="float">10908.86</datum>
                        <datum type="float">10952.39</datum>
                        <datum type="float">7222849</datum>
                        <datum type="float">145417795</datum>
                        <datum type="float">0.8602</datum>
                        <datum type="float">0.3677</datum>
                        <datum type="float">699338777</datum>
                        <datum type="float">32622949</datum>
                        <datum nil="true"/>
                        <datum nil="true"/>
                        <datum type="float">0.8565</datum>
                        <datum type="float">100.000</datum>
                        <datum type="float">100.000</datum>
                        <datum type="float">1168845</datum>
                        <datum nil="true"/>
                        <datum type="float">16.52</datum>
                        <datum nil="true"/>
                        <datum type="float">1.82</datum>
                        <datum/>
                        <datum type="float">1.15</datum>
                        <datum nil="true"/>
                        <datum type="float">3.97</datum>
                        <datum type="float">93.41</datum>
                        <datum/>
                        <datum/>
                        <datum/>
                        <datum>TSE</datum>
                    </datum>
                    <datum type="array">
                        <datum>Y9999</datum>
                        <datum type="dateTime">2018-05-11T00:00:00Z</datum>
                        <datum type="float">10808.40</datum>
                        <datum type="float">10874.63</datum>
                        <datum type="float">10808.40</datum>
                        <datum type="float">10858.98</datum>
                        <datum type="float">7399223</datum>
                        <datum type="float">165763227</datum>
                        <datum type="float">0.9179</datum>
                        <datum type="float">0.4002</datum>
                        <datum type="float">699338982</datum>
                        <datum type="float">32344168</datum>
                        <datum nil="true"/>
                        <datum nil="true"/>
                        <datum type="float">0.9137</datum>
                        <datum type="float">100.000</datum>
                        <datum type="float">100.000</datum>
                        <datum type="float">1248505</datum>
                        <datum nil="true"/>
                        <datum type="float">16.38</datum>
                        <datum nil="true"/>
                        <datum type="float">1.81</datum>
                        <datum/>
                        <datum type="float">1.14</datum>
                        <datum nil="true"/>
                        <datum type="float">4.14</datum>
                        <datum type="float">98.77</datum>
                        <datum/>
                        <datum/>
                        <datum/>
                        <datum>TSE</datum>
                    </datum>
                    <datum type="array">
                        <datum>Y9999</datum>
                        <datum type="dateTime">2018-05-10T00:00:00Z</datum>
                        <datum type="float">10731.68</datum>
                        <datum type="float">10782.06</datum>
                        <datum type="float">10731.68</datum>
                        <datum type="float">10760.21</datum>
                        <datum type="float">7062376</datum>
                        <datum type="float">139276989</datum>
                        <datum type="float">0.5312</datum>
                        <datum type="float">0.3551</datum>
                        <datum type="float">699339661</datum>
                        <datum type="float">32049300</datum>
                        <datum nil="true"/>
                        <datum nil="true"/>
                        <datum type="float">0.5298</datum>
                        <datum type="float">100.000</datum>
                        <datum type="float">100.000</datum>
                        <datum type="float">1102455</datum>
                        <datum nil="true"/>
                        <datum type="float">16.23</datum>
                        <datum nil="true"/>
                        <datum type="float">1.79</datum>
                        <datum/>
                        <datum type="float">1.12</datum>
                        <datum nil="true"/>
                        <datum type="float">4.17</datum>
                        <datum type="float">56.86</datum>
                        <datum/>
                        <datum/>
                        <datum/>
                        <datum>TSE</datum>
                    </datum>
                    <datum type="array">
                        <datum>Y9999</datum>
                        <datum type="dateTime">2018-05-09T00:00:00Z</datum>
                        <datum type="float">10692.89</datum>
                        <datum type="float">10748.60</datum>
                        <datum type="float">10689.81</datum>
                        <datum type="float">10703.35</datum>
                        <datum type="float">7074991</datum>
                        <datum type="float">135741987</datum>
                        <datum type="float">0.1120</datum>
                        <datum type="float">0.3496</datum>
                        <datum type="float">695033357</datum>
                        <datum type="float">31547472</datum>
                        <datum nil="true"/>
                        <datum nil="true"/>
                        <datum type="float">0.1119</datum>
                        <datum type="float">100.000</datum>
                        <datum type="float">100.000</datum>
                        <datum type="float">1123979</datum>
                        <datum nil="true"/>
                        <datum type="float">16.14</datum>
                        <datum nil="true"/>
                        <datum type="float">1.78</datum>
                        <datum/>
                        <datum type="float">1.12</datum>
                        <datum nil="true"/>
                        <datum type="float">4.20</datum>
                        <datum type="float">11.97</datum>
                        <datum/>
                        <datum/>
                        <datum/>
                        <datum>TSE</datum>
                    </datum>
                    <datum type="array">
                        <datum>Y9999</datum>
                        <datum type="dateTime">2018-05-08T00:00:00Z</datum>
                        <datum type="float">10610.44</datum>
                        <datum type="float">10691.38</datum>
                        <datum type="float">10609.04</datum>
                        <datum type="float">10691.38</datum>
                        <datum type="float">7064737</datum>
                        <datum type="float">133691609</datum>
                        <datum type="float">0.8154</datum>
                        <datum type="float">0.3330</datum>
                        <datum type="float">695033357</datum>
                        <datum type="float">31509651</datum>
                        <datum nil="true"/>
                        <datum nil="true"/>
                        <datum type="float">0.8121</datum>
                        <datum type="float">100.000</datum>
                        <datum type="float">100.000</datum>
                        <datum type="float">1042424</datum>
                        <datum nil="true"/>
                        <datum type="float">16.12</datum>
                        <datum nil="true"/>
                        <datum type="float">1.78</datum>
                        <datum/>
                        <datum type="float">1.12</datum>
                        <datum nil="true"/>
                        <datum type="float">4.21</datum>
                        <datum type="float">86.47</datum>
                        <datum/>
                        <datum/>
                        <datum/>
                        <datum>TSE</datum>
                    </datum>
                    <datum type="array">
                        <datum>Y9999</datum>
                        <datum type="dateTime">2018-05-07T00:00:00Z</datum>
                        <datum type="float">10581.78</datum>
                        <datum type="float">10632.62</datum>
                        <datum type="float">10555.56</datum>
                        <datum type="float">10604.91</datum>
                        <datum type="float">6108995</datum>
                        <datum type="float">126046786</datum>
                        <datum type="float">0.7174</datum>
                        <datum type="float">0.2820</datum>
                        <datum type="float">695033431</datum>
                        <datum type="float">31247223</datum>
                        <datum nil="true"/>
                        <datum nil="true"/>
                        <datum type="float">0.7149</datum>
                        <datum type="float">100.000</datum>
                        <datum type="float">100.000</datum>
                        <datum type="float">956892</datum>
                        <datum nil="true"/>
                        <datum type="float">15.99</datum>
                        <datum nil="true"/>
                        <datum type="float">1.76</datum>
                        <datum/>
                        <datum type="float">1.11</datum>
                        <datum nil="true"/>
                        <datum type="float">4.22</datum>
                        <datum type="float">75.54</datum>
                        <datum/>
                        <datum/>
                        <datum/>
                        <datum>TSE</datum>
                    </datum>
                    <datum type="array">
                        <datum>Y9999</datum>
                        <datum type="dateTime">2018-05-04T00:00:00Z</datum>
                        <datum type="float">10516.45</datum>
                        <datum type="float">10566.37</datum>
                        <datum type="float">10500.97</datum>
                        <datum type="float">10529.37</datum>
                        <datum type="float">5653857</datum>
                        <datum type="float">120828141</datum>
                        <datum type="float">0.1445</datum>
                        <datum type="float">0.2961</datum>
                        <datum type="float">695035128</datum>
                        <datum type="float">31017892</datum>
                        <datum nil="true"/>
                        <datum nil="true"/>
                        <datum type="float">0.1444</datum>
                        <datum type="float">100.000</datum>
                        <datum type="float">100.000</datum>
                        <datum type="float">958698</datum>
                        <datum nil="true"/>
                        <datum type="float">15.87</datum>
                        <datum nil="true"/>
                        <datum type="float">1.75</datum>
                        <datum/>
                        <datum type="float">1.10</datum>
                        <datum nil="true"/>
                        <datum type="float">4.25</datum>
                        <datum type="float">15.19</datum>
                        <datum/>
                        <datum/>
                        <datum/>
                        <datum>TSE</datum>
                    </datum>
                    <datum type="array">
                        <datum>Y9999</datum>
                        <datum type="dateTime">2018-05-03T00:00:00Z</datum>
                        <datum type="float">10578.98</datum>
                        <datum type="float">10578.98</datum>
                        <datum type="float">10509.03</datum>
                        <datum type="float">10514.18</datum>
                        <datum type="float">5841156</datum>
                        <datum type="float">124397511</datum>
                        <datum type="float">-0.9853</datum>
                        <datum type="float">0.3034</datum>
                        <datum type="float">695035857</datum>
                        <datum type="float">30994925</datum>
                        <datum nil="true"/>
                        <datum nil="true"/>
                        <datum type="float">-0.9902</datum>
                        <datum type="float">100.000</datum>
                        <datum type="float">100.000</datum>
                        <datum type="float">993874</datum>
                        <datum nil="true"/>
                        <datum type="float">15.86</datum>
                        <datum nil="true"/>
                        <datum type="float">1.75</datum>
                        <datum/>
                        <datum type="float">1.10</datum>
                        <datum nil="true"/>
                        <datum type="float">4.25</datum>
                        <datum type="float">-104.63</datum>
                        <datum/>
                        <datum/>
                        <datum/>
                        <datum>TSE</datum>
                    </datum>
                    <datum type="array">
                        <datum>Y9999</datum>
                        <datum type="dateTime">2018-05-02T00:00:00Z</datum>
                        <datum type="float">10665.52</datum>
                        <datum type="float">10683.90</datum>
                        <datum type="float">10601.10</datum>
                        <datum type="float">10618.81</datum>
                        <datum type="float">6324416</datum>
                        <datum type="float">129078743</datum>
                        <datum type="float">-0.3666</datum>
                        <datum type="float">0.3245</datum>
                        <datum type="float">695043607</datum>
                        <datum type="float">31304327</datum>
                        <datum nil="true"/>
                        <datum nil="true"/>
                        <datum type="float">-0.3673</datum>
                        <datum type="float">100.000</datum>
                        <datum type="float">100.000</datum>
                        <datum type="float">1023004</datum>
                        <datum nil="true"/>
                        <datum type="float">16.02</datum>
                        <datum nil="true"/>
                        <datum type="float">1.77</datum>
                        <datum/>
                        <datum type="float">1.11</datum>
                        <datum nil="true"/>
                        <datum type="float">4.21</datum>
                        <datum type="float">-39.07</datum>
                        <datum/>
                        <datum/>
                        <datum/>
                        <datum>TSE</datum>
                    </datum>
                </data>
                <columns type="array">
                    <column>
                        <description>交易所及櫃檯買賣中心所訂的代碼</description>
                        <name>coid</name>
                        <type>char(7)</type>
                        <unit>-</unit>
                    </column>
                    <column>
                        <description>年月日</description>
                        <name>mdate</name>
                        <type>datetime</type>
                        <unit>-</unit>
                    </column>
                    <column>
                        <description>open_d</description>
                        <name>open_d</name>
                        <type>decimal(8,2)</type>
                        <unit>-</unit>
                    </column>
                    <column>
                        <description>high_d</description>
                        <name>high_d</name>
                        <type>decimal(8,2)</type>
                        <unit>-</unit>
                    </column>
                    <column>
                        <description>low_d</description>
                        <name>low_d</name>
                        <type>decimal(8,2)</type>
                        <unit>-</unit>
                    </column>
                    <column>
                        <description>close_d</description>
                        <name>close_d</name>
                        <type>decimal(8,2)</type>
                        <unit>-</unit>
                    </column>
                    <column>
                        <description>
                            當日若成交量為0，表示當日無交易，此時之開高低收價格為前一日之收盤價
                            <br />除加權指數(Y9999)外，產業部分由TEJ衍生，為成分股成交量之加總
                        </description>
                        <name>volume</name>
                        <type>decimal(9,0)</type>
                        <unit>T</unit>
                    </column>
                    <column>
                        <description>未無考慮公眾流通量(free float)；除加權指數(Y9999)外，產業部分由TEJ衍生</description>
                        <name>amount</name>
                        <type>decimal(12,0)</type>
                        <unit>NTD,T</unit>
                    </column>
                    <column>
                        <description>當OTC轉至TSE交易時，報酬率以承銷價計算，若無承銷價，則以OTC最後一天之收盤價來計算。</description>
                        <name>roi</name>
                        <type>decimal(9,4)</type>
                        <unit>%</unit>
                    </column>
                    <column>
                        <description>個股=成交量/流通股數*100(%)；產業＝產業成交量總額/產業流通股數*100(%)</description>
                        <name>turnover</name>
                        <type>decimal(9,4)</type>
                        <unit>%</unit>
                    </column>
                    <column>
                        <description>流通在外股數(千股)</description>
                        <name>outstanding</name>
                        <type>decimal(12,0)</type>
                        <unit>T</unit>
                    </column>
                    <column>
                        <description>
                            個股：流通在外股數(個股)*未調整收盤價；
                            <br />指數：為反映該股票於市場上實際可流通之股數，會將各成分股之公開發行股數扣除長期性、策略性持 股比例，故計算指數市值時，若該指數有考慮公眾流通量(交易所與FTSE合編的指數)，則市值公式=未調整收盤價*流通在外股數(個股)*公眾流通係數(此係數由交易所提供)
                        </description>
                        <name>mv</name>
                        <type>decimal(12,0)</type>
                        <unit>NTD,T</unit>
                    </column>
                    <column>
                        <description>最後揭示買價</description>
                        <name>bid</name>
                        <type>decimal(7,2)</type>
                        <unit>NTD</unit>
                    </column>
                    <column>
                        <description>最後揭示賣價</description>
                        <name>offer</name>
                        <type>decimal(7,2)</type>
                        <unit>NTD</unit>
                    </column>
                    <column>
                        <description>報酬率-Ln</description>
                        <name>roib</name>
                        <type>decimal(9,4)</type>
                        <unit>-</unit>
                    </column>
                    <column>
                        <description>mv_pct</description>
                        <name>mv_pct</name>
                        <type>decimal(7,3)</type>
                        <unit>-</unit>
                    </column>
                    <column>
                        <description>amt_pct</description>
                        <name>amt_pct</name>
                        <type>decimal(7,3)</type>
                        <unit>-</unit>
                    </column>
                    <column>
                        <description>成交筆數(筆)</description>
                        <name>trn_d</name>
                        <type>decimal(9,0)</type>
                        <unit>-</unit>
                    </column>
                    <column>
                        <description>per_tse</description>
                        <name>per_tse</name>
                        <type>decimal(7,2)</type>
                        <unit>-</unit>
                    </column>
                    <column>
                        <description>per_tej</description>
                        <name>per_tej</name>
                        <type>decimal(7,2)</type>
                        <unit>-</unit>
                    </column>
                    <column>
                        <description>pbr_tse</description>
                        <name>pbr_tse</name>
                        <type>decimal(7,2)</type>
                        <unit>-</unit>
                    </column>
                    <column>
                        <description>pbr_tej</description>
                        <name>pbr_tej</name>
                        <type>decimal(7,2)</type>
                        <unit>-</unit>
                    </column>
                    <column>
                        <description>股票漲停：”+”；跌停：”-“</description>
                        <name>limit</name>
                        <type>char(1)</type>
                        <unit>-</unit>
                    </column>
                    <column>
                        <description>
                            =市值/最近4季合計之營收，TEJ提供
                            <br />本欄位需搭配財報發佈時間，目前更新方式為每年6/1、10/1、及12/1更新營收資料，首次上市需滿一年的次一年度1/1始計算。
                        </description>
                        <name>tej_psr</name>
                        <type>decimal(7,2)</type>
                        <unit>-</unit>
                    </column>
                    <column>
                        <description>
                            即每股股利與當日名目收盤價之比值，其中每股股利=該公司每股配發之現金股利+盈餘轉增資股票股利。
                            <br />此欄位由交易所提供，其中97/07/17以前之資料交易所計算方式係採取前一筆有發放股利之資料來計算，即當年度公司不發放股利，則以前一年度或更早以前的股利資料計算不合理，故97/07/17交易所已修正為以該年度之資料來計算，故前後期資料會有所差異。
                        </description>
                        <name>div_yid</name>
                        <type>decimal(7,2)</type>
                        <unit>%</unit>
                    </column>
                    <column>
                        <description>=現金股利總額/市值*100%，TEJ提供</description>
                        <name>tej_cdiv</name>
                        <type>decimal(7,2)</type>
                        <unit>%</unit>
                    </column>
                    <column>
                        <description>股價漲跌(元)</description>
                        <name>clschg</name>
                        <type>decimal(8,2)</type>
                        <unit>-</unit>
                    </column>
                    <column>
                        <description>公佈異常交易有價證券之交易資訊</description>
                        <name>xattn1</name>
                        <type>char(1)</type>
                        <unit>-</unit>
                    </column>
                    <column>
                        <description>對連續公佈注意交易資訊之有價證券採取之處置措施</description>
                        <name>xattn2</name>
                        <type>char(1)</type>
                        <unit>-</unit>
                    </column>
                    <column>
                        <description>全額交割(Y)</description>
                        <name>xstat1</name>
                        <type>char(1)</type>
                        <unit>-</unit>
                    </column>
                    <column>
                        <description>市場別</description>
                        <name>pmkt</name>
                        <type>char(5)</type>
                        <unit>-</unit>
                    </column>
                </columns>
            </datatable>
            <meta>
                <nextCursorId>tY5x2zSbCC</nextCursorId>
            </meta>
        </tej-response>
        
        ```
        </div>

??? tip "提示"

    取得的資料是未排序資料，如須排序請取得後自行排序，或指定 opts.sort參數。

### 資料篩選

如果需要針對欄位篩選，例如僅須取得台灣加權股價指數(Y9999)，請直接增加欄位篩選條件 coid=Y9999

!!! info "In" 
    
    <!-- <div style="max-height: 500px; overflow: auto;"> -->

    === "json"

        ``` sh
        GET https://api.tej.com.tw/api/datatables/TWN/APRCD.json?coid=Y9999&api_key="YOURAPIKEY"
        ```

    === "xml"

        ``` sh
        GET https://api.tej.com.tw/api/datatables/TWN/APRCD.xml?coid=Y9999&api_key="YOURAPIKEY"  
        ```  

或是同時取得兩種指數資料Y9999及Y9998，請利用序列條件 coid=Y9999,Y9998

!!! info "In" 

    === "json"

        ``` sh
        GET https://api.tej.com.tw/api/datatables/TWN/APRCD.json?coid=Y9999,Y9998&api_key="YOURAPIKEY"
        ```

    === "xml"

        ``` sh
        GET https://api.tej.com.tw/api/datatables/TWN/APRCD.xml?coid=Y9999,Y9998&api_key="YOURAPIKEY"
        ```

單次取得資料限制最多10,000筆，您可以擷取 next_cursor_id的資訊，並用opts.cursor_id參數來取得下一頁的資料

!!! info "In" 
    
    === "json"

        ``` sh
        GET https://api.tej.com.tw/api/datatables/TWN/APRCD.json?opts.cursor_id=<第一頁取得的cursor_id>&api_key="YOURAPIKEY"
        ```

    === "xml"

        ``` sh
        GET https://api.tej.com.tw/api/datatables/TWN/APRCD.xml?opts.cursor_id=<第一頁取得的cursor_id>&api_key="YOURAPIKEY"
        ```
    <!-- </div> -->

### 欄位篩選

若僅需要取得單一欄位，請利用特殊參數 opts中的columns條件，例如僅須取得開盤價欄位(open_d)

!!! info "In" 

    === "json"

        ``` sh
        GET https://api.tej.com.tw/api/datatables/TWN/APRCD.json?opts.columns=open_d&api_key=<YOURAPIKEY> 
        ```

    === "xml"

        ``` sh
        GET https://api.tej.com.tw/api/datatables/TWN/APRCD.xml?opts.columns=open_d&api_key=<YOURAPIKEY>
        ```

### 資料篩選運算

|   篩選運算    |   是否必要    |   詳細說明               | 使用範例|
| ------------ | ------- | ----------------------------- | ------- |
| `=`         |    是   |   指定欄位等於指定的文字或數值    |`coid=Y9999`|
| `.gt=`      |    否   |   指定欄位大於指定的數值         |`open_d.gt=0`|
| `.lt=`      |    否   |   指定欄位小於指定的數值         |`open_d.lt=0`|
| `.gte=`     |    否   |   指定欄位大於或等於指定的數值    |`open_d.gte=0`|
| `.lte=`     |    否   |   指定欄位小於或等於指定的數值    |`open_d.lte=0`|
| `.ne=`      |    否   |   指定欄位不等於指定的數值        |`open_d.ne=0`|

### 查詢參數

|   參數                |   是否必要    |   詳細說明               | 使用範例|
| ------------          | -------       | ----------------------------- | ------- |
| `opts.columns`        |    是         |   指定需要取得的欄位，欄位名稱用逗號隔開    |`opts.columns=coid,mdate,open_d`|
| `opts.per_page`       |    否         |   指定每次取得的資料數量(上限為10,000)，可利用opts.cursor_id分次取得資料，但總筆數不得超過1,000,000筆         |`opts.per_page=100`|
| `opts.cursor_id`      |    否         |   每次呼叫若還有後續資料，API則產生cursor_id，取用這個id作下一次的呼叫，可取得剩餘或下一頁的資料。         |`opts.cursor_id=LK8whTtt8w`|
| `opts.sort`           |    否         |   指定排序的欄位及排序方式，採用 [欄位名稱].[排序方式]表示，排序方式有正向排序(asc)及反向排序(desc)，預設為正向排序。    |`opts.sort=mdate.desc`|
| `opts.pivot`          |    否         |   轉置表格功能，可讓資料變成欄位。<font color="red">目前僅支援財務相關表格</font>    |`opts.pivot=true`|

### 日期格式

資料輸出的日期格式一率採用`yyyy-MM-ddTHH:mm:ssZ`，例如`2018-05-09T10:20:30Z`。

篩選條件中的日期格式，可支援的格式如下表，其中<font color="red">Z</font>代表時區，例如台灣為
`+08:00`，但可以省略。

|   支援格式    |    使用範例   |
|----------------------------| ----------------------- |
|`yyyy-MM-ddTHH:mm:ss.SSSZ` |`2018-05-09T10:20:30.000Z`|
|`yyyy-MM-ddHH:mm:ss.SSSZ` |`2018-05-0910:20:30.000Z`|
|`yyyyMMddTHHmmss.SSSZ` |`20180509T102030.000Z`|
|`yyyy-MM-ddTHH:mm:ssZ` |`2018-05-09T10:20:30Z`|
|`yyyy-MM-dd HH:mm:ssZ` |`2018-05-09 10:20:30Z`|
|`yyyy-MM-ddHH:mm:ssZ` |`2018-05-0910:20:30Z`|
|`yyyyMMddTHHmmssZ` |`20180509T102030Z`|
|`yyyyMMddTHHmmssZ` |`20180509T102030Z`|
|`yyyy-MM-dd` |`2018-05-09`|
|`yyyy/MM/dd` |`2018/05/09`|
|`yyyyMMdd` |`20180509`|

## 表格資訊

以下文件將說明如何取得表格資訊。

### 使用方法

!!! info "in"

    ``` sh
    https://api.tej.com.tw/api/datatables/{datatable_code}/{table_code}/metadata?api_key="YOURAPIKEY"
    ```

回應資訊說明

|參數 |詳細說明|
|-----------| ------------|
|dbCode |資料庫代碼|
|tableCode |資料表代碼|
|name |資料表名稱|
|description |資料表詳細說明|
|primaryKey| 資料表主鍵列表|
| filters | 資料表可篩選欄位 |
| columns | 資料表欄位說明<br><table><tr><th>參數</th><th>詳細說明</th></tr><tr><td>name</td><td>欄位代碼</td></tr><tr><td>cname</td><td>欄位中文名稱</td></tr><tr><td>description</td><td>欄位說明</td></tr><tr><td>type</td><td>欄位資料格式</td></tr><tr><td>unit</td><td>單位</td></tr></table> |
| pivot | 是否支援轉置 |
| status | 資料表狀態<br><table><tr><th>參數</th><th>詳細說明</th></tr><tr><td>status</td><td>狀態</td></tr><tr><td>refreshed_at</td><td>最新資料時間</td></tr></table> |

### 使用範例

??? example "取得TWN/APRCD表格資訊"

    ``` sh
    GET https://api.tej.com.tw/api/datatables/TWN/APRCD/metadata?api_key="YOURAPIKEY"
    ```

??? success "out"

    <div style="max-height: 500px; overflow: auto;">

    ``` json
    {
    "datatable":{
        "dbCode":"TWN",
        "tableCode":"APRCD",
        "name":"上市(櫃)未調整股價(日)",
        "description":"【資料範圍】上市的證券及指數(TSE及OTC)【資料期間】2000年至今",
        "filters":[
            "coid",
            "mdate",
            "open_d",
            "high_d",
            "low_d",
            "close_d",
            "volume",
            "amount",
            "roi",
            "turnover",
            "outstanding",
            "mv",
            "bid",
            "offer",
            "roib",
            "mv_pct",
            "amt_pct",
            "trn_d",
            "per_tse",
            "per_tej",
            "pbr_tse",
            "pbr_tej",
            "limit",
            "tej_psr",
            "div_yid",
            "tej_cdiv",
            "clschg",
            "xattn1",
            "xattn2",
            "xstat1",
            "pmkt"
        ],
        "primaryKey":[
            "coid",
            "mdate"
        ],
        "status":{
            "status":"OK",
            "refreshed_at":"2020-01-09T00:00:00Z"
        },
        "pivot":false,
        "columns":[
            {
                "name":"coid",
                "type":"char(7)",
                "cname":"證券代碼",
                "description":"交易所及櫃檯買賣中心所訂的代碼",
                "unit":"-"
            },
            {
                "name":"mdate",
                "type":"datetime",
                "cname":"年月日",
                "description":"年月日",
                "unit":"-"
            },
            {
                "name":"open_d",
                "type":"decimal(8,2)",
                "cname":"開盤價(元)",
                "description":"興櫃股票不提供開盤價，本處之開盤價為前一交易日之收盤價。首次上興櫃日當日開盤價以[－]值代入",
                "unit":"NTD"
            },
            {
                "name":"high_d",
                "type":"decimal(8,2)",
                "cname":"最高價(元)",
                "description":"若當日無成交，以前一交易日收盤價代入",
                "unit":"NTD"
            },
            {
                "name":"low_d",
                "type":"decimal(8,2)",
                "cname":"最低價(元)",
                "description":"若當日無成交，以前一交易日收盤價代入",
                "unit":"NTD"
            },
            {
                "name":"close_d",
                "type":"decimal(8,2)",
                "cname":"收盤價(元)",
                "description":"若當日無成交，以前一交易日收盤價代入",
                "unit":"NTD"
            },
            {
                "name":"volume",
                "type":"decimal(9,0)",
                "cname":"成交量(千股)",
                "description":"當日若成交量為0，表示當日無交易，此時之開高低收價格為前一日之收盤價除加權指數(Y9999)外，產業部分由TEJ衍生，為成分股成交量之加總",
                "unit":"T"
            },
            {
                "name":"amount",
                "type":"decimal(12,0)",
                "cname":"成交值(千元)",
                "description":"未無考慮公眾流通量(free float)；除加權指數(Y9999)外，產業部分由TEJ衍生",
                "unit":"NTD,T"
            },
            {
                "name":"roi",
                "type":"decimal(9,4)",
                "cname":"報酬率%",
                "description":"當OTC轉至TSE交易時，報酬率以承銷價計算，若無承銷價，則以OTC最後一天之收盤價來計算。",
                "unit":"%"
            },
            {
                "name":"turnover",
                "type":"decimal(9,4)",
                "cname":"週轉率%",
                "description":"個股=成交量/流通股數*100(%)；產業＝產業成交量總額/產業流通股數*100(%)",
                "unit":"%"
            },
            {
                "name":"outstanding",
                "type":"decimal(12,0)",
                "cname":"流通在外股數(千股)",
                "description":"流通在外股數(千股)",
                "unit":"T"
            },
            {
                "name":"mv",
                "type":"decimal(12,0)",
                "cname":"市值(百萬元)",
                "description":"個股：流通在外股數(個股)*未調整收盤價；指數：為反映該股票於市場上實際可流通之股數，會將各成分股之公開發行股數扣除長期性、策略性持  股比例，故計算指數市值時，若該指數有考慮公眾流通量(交易所與FTSE合編的指數)，則市值公式=未調整收盤價*流通在外股數(個股)*公眾流通係數(此係數由交易所提供)",
                "unit":"NTD,T"
            },
            {
                "name":"bid",
                "type":"decimal(7,2)",
                "cname":"最後揭示買價",
                "description":"最後揭示買價",
                "unit":"NTD"
            },
            {
                "name":"offer",
                "type":"decimal(7,2)",
                "cname":"最後揭示賣價",
                "description":"最後揭示賣價",
                "unit":"NTD"
            },
            {
                "name":"roib",
                "type":"decimal(9,4)",
                "cname":"報酬率-Ln",
                "description":"報酬率-Ln",
                "unit":"-"
            },
            {
                "name":"mv_pct",
                "type":"decimal(7,3)",
                "cname":"市值比重%",
                "description":"=市值/加權指數有效成分股總市值*100(%)(產業之市值比重:產業有效成分股之總市值/加權指數有效成分股總市值*100(%))",
                "unit":"%"
            },
            {
                "name":"amt_pct",
                "type":"decimal(7,3)",
                "cname":"成交值比重%",
                "description":"=成交值/加權指數有效成分股總成交值*100(%)",
                "unit":"%"
            },
            {
                "name":"trn_d",
                "type":"decimal(9,0)",
                "cname":"成交筆數(筆)",
                "description":"成交筆數(筆)",
                "unit":"-"
            },
            {
                "name":"per_tse",
                "type":"decimal(7,2)",
                "cname":"本益比-TSE",
                "description":"=收盤價/最近4季合計之每股淨利，交易所提供",
                "unit":"-"
            },
            {
                "name":"per_tej",
                "type":"decimal(7,2)",
                "cname":"本益比-TEJ",
                "description":"=收盤價/最近4季合計之每股常續性淨利，TEJ提供本欄位需搭配財報發佈時間，目前更新方式為每年6/1、10/1、及12/1更新常續性淨利資料，首次上市需滿一年的次一年度1/1始計算。",
                "unit":"-"
            },
            {
                "name":"pbr_tse",
                "type":"decimal(7,2)",
                "cname":"股價淨值比-TSE",
                "description":"=收盤價/每股淨值，交易所提供(不含興櫃)。TSE自民國94年9月1日開始提供，OTC自民國92年8月開始提供",
                "unit":"-"
            },
            {
                "name":"pbr_tej",
                "type":"decimal(7,2)",
                "cname":"股價淨值比-TEJ",
                "description":"TEJ 衍生，本欄位需搭配財報發佈時間，目前更新方式為每年6/1、10/1、及12/1更新股東權益資料，首次上市需滿一年的次一年度1/1始計算。",
                "unit":"-"
            },
            {
                "name":"limit",
                "type":"char(1)",
                "cname":"漲跌停",
                "description":"股票漲停：”+”；跌停：”-“",
                "unit":"-"
            },
            {
                "name":"tej_psr",
                "type":"decimal(7,2)",
                "cname":"股價營收比-TEJ",
                "description":"=市值/最近4季合計之營收，TEJ提供本欄位需搭配財報發佈時間，目前更新方式為每年6/1、10/1、及12/1更新營收資料，首次上市需滿一年的次一年度1/1始計算。",
                "unit":"-"
            },
            {
                "name":"div_yid",
                "type":"decimal(7,2)",
                "cname":"股利殖利率-TSE",
                "description":"即每股股利與當日名目收盤價之比值，其中每股股利=該公司每股配發之現金股利+盈餘轉增資股票股利。此欄位由交易所提供，其中97/07/17以前之資料交易所計算方式係採取前一筆有發放股利之資料來計算，即當年度公司不發放股利，則以前一年度或更早以前的股利資料計算不合理，故97/07/17交易所已修正為以該年度之資料來計算，故前後期資料會有所差異。",
                "unit":"%"
            },
            {
                "name":"tej_cdiv",
                "type":"decimal(7,2)",
                "cname":"現金股利率",
                "description":"=現金股利總額/市值*100%，TEJ提供",
                "unit":"%"
            },
            {
                "name":"clschg",
                "type":"decimal(8,2)",
                "cname":"股價漲跌(元)",
                "description":"股價漲跌(元)",
                "unit":"-"
            },
            {
                "name":"xattn1",
                "type":"char(1)",
                "cname":"注意股票(A)",
                "description":"公佈異常交易有價證券之交易資訊",
                "unit":"-"
            },
            {
                "name":"xattn2",
                "type":"char(1)",
                "cname":"處置股票(D)",
                "description":"對連續公佈注意交易資訊之有價證券採取之處置措施",
                "unit":"-"
            },
            {
                "name":"xstat1",
                "type":"char(1)",
                "cname":"全額交割(Y)",
                "description":"全額交割(Y)",
                "unit":"-"
            },
            {
                "name":"pmkt",
                "type":"char(5)",
                "cname":"市場別",
                "description":"市場別",
                "unit":"-"
            }
        ]
    }
    }

    ```

    </div>

## 搜尋表格

以下文件將說明利用關鍵字搜尋表格。

#### 使用方法

!!! info "In"

    ``` sh
    GET https://api.tej.com.tw/api/search/table/{關鍵字}?api_key="YOURAPIKEY"
    ```

將回應陣列型態，表示多筆資料，每筆資料資訊如下

|參數 | 詳細說明|
|-------|--------|
|matchType | 匹配類別<ul><li>TABLE_MATCH:關鍵字在表格名稱或說明中</li><li>COLUMN_MATCH:關鍵字在欄位名稱或說明中</li><li>TABLE_MATCH & COLUMN_MATCH:關鍵字在表格及欄位名稱或說明中</li></ul>
|tableId |資料表代碼|
|tableName |資料表名稱|
|tableDesc |資料表詳細說明|
| columns | 資料表欄位說明<br><table><tr><th>參數</th><th>詳細說明</th></tr><tr><td>name</td><td>欄位代碼</td></tr><tr><td>cname</td><td>欄位中文名稱</td></tr><tr><td>description</td><td>欄位說明</td></tr><tr><td>type</td><td>欄位資料格式</td></tr><tr><td>unit</td><td>單位</td></tr></table>|

### 使用範例

!!! example "假設搜尋【市盈率】"

    ``` sh
    GET https://api.tej.com.tw/api/search/table/市盈率?api_key="API_KEY"
    ```

??? success "out"

    <div style="max-height: 500px; overflow: auto;">

    ``` json
    {
        "result":{
            "tables":[
                {
                    "matchType":"COLUMN_MATCH",
                    "tableId":"CHN/CPRCD",
                    "tableName":"中國_日股價_未調整",
                    "tableDesc":"【資料範圍】上海及深圳交易所上市公司（包含A股及B股）【資料期間】1991年起【資料頻率】日資料（衍生週、月、年資料）【資料來源】上海及深圳交易所",
                    "columns":[
                    {
                        "name":"per_tej",
                        "type":"decimal(7,2)",
                        "cname":"市盈率-TEJ",
                        "description":"=(當日未調整收盤價*公司總股數) / 股東權益總額。本欄位需搭配財報發佈時間，目前更新方式為每年5、9、11月第一個交易日股東權益資料",
                        "unit":"-"
                    }
                    ]
                },
                {
                    "matchType":"COLUMN_MATCH",
                    "tableId":"CHN/CPRCD1",
                    "tableName":"中國_日股價_除權息調整",
                    "tableDesc":"【資料範圍】上海及深圳交易所上市公司（包含A股及B股）【資料期間】1991年起【資料頻率】日資料（衍生週、月、年資料）【資料來源】上海及深圳交易所",
                    "columns":[
                    {
                        "name":"per_tej",
                        "type":"decimal(7,2)",
                        "cname":"市盈率-TEJ",
                        "description":"=(當日未調整收盤價*公司總股數) / 股東權益總額。本欄位需搭配財報發佈時間，目前更新方式為每年5、9、11月第一個交易日股東權益資料",
                        "unit":"-"
                    }
                    ]
                }
            ]
        }
    }
    ```

    </div>

## APIKEY資訊

以下文件將說明如何取得APIKEY資訊。

#### 取得使用資訊

!!! info "In"

    ``` sh
    GET https://api.tej.com.tw/api/apiKeyInfo/"YOURAPIKEY"
    ```

回應資訊說明

|參數| 詳細說明|
|----|---------|
|key |您的APIKEY|
|startDate |APIKEY開始使用日|
|endDate |APIKEY結束日|
|reqDayLimit |每日呼叫次數上限|
|rowsDayLimit |每日資料筆數上限|
|rowsMonthLimit |每月資料筆數上限|
|todayReqCount |本日呼叫次數|
|todayRows |本日資料筆數|
|monthRows |本月資料筆數|
|user |使用者資訊<br><table><tr><th>參數</th><th>詳細說明</th></tr><tr><td>userId</td><td>使用者編號</td></tr><tr><td>name</td><td> 使用者名稱</td></tr><tr><td>shortName</td><td> 使用者名稱</td></tr><tr><td>subscritionStartDate</td><td> 訂閱開始日</td></tr><tr><td>subscritionEndDate</td><td> 訂閱結束日</td></tr><tr><td>tables</td><td> 可以使用的表格列表</td></tr></table>|

### 使用範例

!!! example "ex"

    ``` sh
    GET https://api.tej.com.tw/api/apiKeyInfo/"YOURAPIKEY"
    ```

??? success "out"

    <div style="max-height: 500px; overflow: auto;">

    ``` json
    {
        "key":"<YOURAPIKEY>",
        "user":{
            "userId":1,
            "shortName":"測試帳號",
            "name":"測試帳號",
            "subscritionStartDate":"2018-08-20",
            "subscritionEndDate":"2022-08-31",
            "maxKey":1,
            "tables":{
                "TWN/AGIN":{
                    "tableId":"TWN/AGIN",
                    "startUsageDate":"2018-08-01",
                    "endUsageDate":"2019-12-31",
                    "dataStartYear":2008,
                    "dataEndYear":2999
                },
                "CHN/CFDATT":{
                    "tableId":"CHN/CFDATT",
                    "startUsageDate":"2018-12-10",
                    "endUsageDate":"2018-12-25",
                    "dataStartYear":2008,
                    "dataEndYear":2999
                },
                "TWN/ACINV":{
                    "tableId":"TWN/ACINV",
                    "startUsageDate":"2018-08-01",
                    "endUsageDate":"2019-12-31",
                    "dataStartYear":2008,
                    "dataEndYear":2999
                },
                "CHN/CRMBFX":{
                    "tableId":"CHN/CRMBFX",
                    "startUsageDate":"2018-12-10",
                    "endUsageDate":"2018-12-31",
                    "dataStartYear":2008,
                    "dataEndYear":2999
                },
                "TWN/ALANDTR":{
                    "tableId":"TWN/ALANDTR",
                    "startUsageDate":"2018-08-01",
                    "endUsageDate":"2019-12-31",
                    "dataStartYear":2008,
                    "dataEndYear":2999
                },
                "TWN/ASTK1":{
                    "tableId":"TWN/ASTK1",
                    "startUsageDate":"2018-08-01",
                    "endUsageDate":"2019-12-31",
                    "dataStartYear":2008,
                    "dataEndYear":2999
                },
                "TWN/APRCD":{
                    "tableId":"TWN/APRCD",
                    "startUsageDate":"2018-08-01",
                    "endUsageDate":"2019-12-31",
                    "dataStartYear":2008,
                    "dataEndYear":2999
                },
                "CHN/CFDNAV":{
                    "tableId":"CHN/CFDNAV",
                    "startUsageDate":"2018-12-10",
                    "endUsageDate":"2018-12-25",
                    "dataStartYear":2008,
                    "dataEndYear":2999
                },
                "TWN/AMIX":{
                    "tableId":"TWN/AMIX",
                    "startUsageDate":"2018-08-01",
                    "endUsageDate":"2019-12-31",
                    "dataStartYear":2008,
                    "dataEndYear":2999
                },
                "TWN/AOPTION":{
                    "tableId":"TWN/AOPTION",
                    "startUsageDate":"2018-08-01",
                    "endUsageDate":"2019-12-31",
                    "dataStartYear":2008,
                    "dataEndYear":2999
                },
                "TWN/ATINST1":{
                    "tableId":"TWN/ATINST1",
                    "startUsageDate":"2018-08-01",
                    "endUsageDate":"2019-12-31",
                    "dataStartYear":2008,
                    "dataEndYear":2999
                },
                "TWN/AARNT":{
                    "tableId":"TWN/AARNT",
                    "startUsageDate":"2018-08-01",
                    "endUsageDate":"2019-12-31",
                    "dataStartYear":2008,
                    "dataEndYear":2999
                },
                "TWN/AQFII":{
                    "tableId":"TWN/AQFII",
                    "startUsageDate":"2018-08-01",
                    "endUsageDate":"2019-12-31",
                    "dataStartYear":2008,
                    "dataEndYear":2999
                },
                "TWN/AFUTR":{
                    "tableId":"TWN/AFUTR",
                    "startUsageDate":"2018-08-01",
                    "endUsageDate":"2019-12-31",
                    "dataStartYear":2008,
                    "dataEndYear":2999
                },
                "TWN/ANAV":{
                    "tableId":"TWN/ANAV",
                    "startUsageDate":"2018-08-01",
                    "endUsageDate":"2019-12-31",
                    "dataStartYear":2008,
                    "dataEndYear":2999
                },
                "TWN/AATT":{
                    "tableId":"TWN/AATT",
                    "startUsageDate":"2018-08-01",
                    "endUsageDate":"2019-12-31",
                    "dataStartYear":2008,
                    "dataEndYear":2999
                },
                "TWN/ASALE":{
                    "tableId":"TWN/ASALE",
                    "startUsageDate":"2018-08-01",
                    "endUsageDate":"2019-12-31",
                    "dataStartYear":2008,
                    "dataEndYear":2999
                },
                "TWN/AIND":{
                    "tableId":"TWN/AIND",
                    "startUsageDate":"2018-08-01",
                    "endUsageDate":"2019-12-31",
                    "dataStartYear":2008,
                    "dataEndYear":2999
                },
                "TWN/AOFATT":{
                    "tableId":"TWN/AOFATT",
                    "startUsageDate":"2018-08-01",
                    "endUsageDate":"2019-12-31",
                    "dataStartYear":2008,
                    "dataEndYear":2999
                },
                "GLOBAL/ANMAR":{
                    "tableId":"GLOBAL/ANMAR",
                    "startUsageDate":"2018-08-01",
                    "endUsageDate":"2019-12-31",
                    "dataStartYear":2019,
                    "dataEndYear":2020
                },
                "TWN/ABSTN":{
                    "tableId":"TWN/ABSTN",
                    "startUsageDate":"2018-08-01",
                    "endUsageDate":"2019-12-31",
                    "dataStartYear":2008,
                    "dataEndYear":2999
                },
                "TWN/AOFNAV":{
                    "tableId":"TWN/AOFNAV",
                    "startUsageDate":"2018-08-01",
                    "endUsageDate":"2019-12-31",
                    "dataStartYear":2008,
                    "dataEndYear":2999
                },
                "TWN/AAPRTRAN":{
                    "tableId":"TWN/AAPRTRAN",
                    "startUsageDate":"2018-08-01",
                    "endUsageDate":"2019-12-31",
                    "dataStartYear":2008,
                    "dataEndYear":2999
                },
                "GLOBAL/ABMAR":{
                    "tableId":"GLOBAL/ABMAR",
                    "startUsageDate":"2018-08-01",
                    "endUsageDate":"2019-12-31",
                    "dataStartYear":2019,
                    "dataEndYear":2020
                },
                "TWN/AINV":{
                    "tableId":"TWN/AINV",
                    "startUsageDate":"2018-08-01",
                    "endUsageDate":"2019-12-31",
                    "dataStartYear":2008,
                    "dataEndYear":2999
                },
                "TWN/AAPRRENT":{
                    "tableId":"TWN/AAPRRENT",
                    "startUsageDate":"2018-08-01",
                    "endUsageDate":"2019-12-31",
                    "dataStartYear":2008,
                    "dataEndYear":2999
                }
            },
            "emp":false
        },
        "startDate":"2018-11-12",
        "endDate":"2018-11-30",
        "todayRows":0,
        "monthRows":0,
        "todayReqCount":0,
        "rowsDayLimit":10000000,
        "rowsMonthLimit":9223372036854776000,
        "reqDayLimit":100000,
        "varEnabled":false,
        "varMaxAssets":500,
        "varConcurrent":1,
        "varAllowAssetTypes":[

        ],
        "varAdvanced":false
    }
    ```
    </div>
