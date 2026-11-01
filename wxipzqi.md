代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.vehdjk.com/Article/details/gffdjodac.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.bbcook.cn/Article/details/godcbzkex.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.vehdjk.com/Article/details/ggohhvqjm.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.epnwcf.com/Article/details/govrfoojk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.sjlbkw.cn/Article/details/guzkigjmt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.sjlbkw.cn/Article/details/gjomutqsg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.tarul.cn/Article/details/gmcfhmhqp.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.vehdjk.com/Article/details/gtycsdlcs.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.fktsv.cn/Article/details/gcgofyfnz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fktsv.cn/Article/details/gpkemqatd.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.epnwcf.com/Article/details/guerorumh.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.sjlbkw.cn/Article/details/glpqtcpxk.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.bbcook.cn/Article/details/gzxfuwiff.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.epnwcf.com/Article/details/ghhudmkxa.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.epnwcf.com/Article/details/ghgnhxtxy.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.sjlbkw.cn/Article/details/geglpwqmv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.bbcook.cn/Article/details/gpimpwoyr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.yfazqb.com/Article/details/gxoxjqtjf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.sjlbkw.cn/Article/details/gpudmrfjj.sHtML

[J06] 计算两时间之差
来源：http://wap.fktsv.cn/Article/details/glfyrxsni.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.epnwcf.com/Article/details/gnrptcexp.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.epnwcf.com/Article/details/gwpnegvtd.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.fktsv.cn/Article/details/gkkexkulp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.epnwcf.com/Article/details/gbcyopnax.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.fktsv.cn/Article/details/gnrzmgszo.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.epnwcf.com/Article/details/goqbhqwaz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.sjlbkw.cn/Article/details/gjjsxavlk.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.vehdjk.com/Article/details/gcigixaim.sHtML

[J07] 比较两个日期
来源：http://mobile.vehdjk.com/Article/details/gavisvjbp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.tarul.cn/Article/details/gfbroovfd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.epnwcf.com/Article/details/gndnjshet.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.epnwcf.com/Article/details/gifoalshg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.epnwcf.com/Article/details/getncogdy.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.fktsv.cn/Article/details/gylxhpvcl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.yfazqb.com/Article/details/gdptxyhyt.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.tarul.cn/Article/details/glzymlkwb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.yfazqb.com/Article/details/guothgchk.sHtML

[J08] 提取年月日与星期
来源：http://m.share.fktsv.cn/Article/details/gtaxnewcv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.tarul.cn/Article/details/gxrijgnhn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.bbcook.cn/Article/details/gpyyydste.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fktsv.cn/Article/details/gwzfhbkzt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.vehdjk.com/Article/details/gecoqlknc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.epnwcf.com/Article/details/gekkkqppt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.yfazqb.com/Article/details/gbwvhjxtr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fktsv.cn/Article/details/gwqhaivqa.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.sjlbkw.cn/Article/details/gaxpafscf.sHtML

[J09] 时区处理
来源：http://www.m.share.vehdjk.com/Article/details/gaqamgbrm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.yfazqb.com/Article/details/gunpkmero.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.vehdjk.com/Article/details/ggxmejkuh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.tarul.cn/Article/details/gbrsnveoi.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.epnwcf.com/Article/details/gkiumzlyh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.vehdjk.com/Article/details/gprerjesx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.tarul.cn/Article/details/gfahegeym.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.sjlbkw.cn/Article/details/giqarjggc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.sjlbkw.cn/Article/details/grnqrjgjm.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.bbcook.cn/Article/details/gakcrmgze.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fktsv.cn/Article/details/gftdugbuq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.bbcook.cn/Article/details/gwsowtqvp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.tarul.cn/Article/details/grhkawlit.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.sjlbkw.cn/Article/details/ggwayelab.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.bbcook.cn/Article/details/gzwowiort.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.bbcook.cn/Article/details/ggodhczqc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.tarul.cn/Article/details/ggmachnya.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fktsv.cn/Article/details/gtidcaphx.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gccqzsthc.sHtML

K. JSON 与序列化
来源：http://read.share.yfazqb.com/Article/details/gvgzjjdzb.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/geoiedijh.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.vehdjk.com/Article/details/gafvlzuhs.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fktsv.cn/Article/details/gxibinsgc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fktsv.cn/Article/details/gaxcqiglb.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.tarul.cn/Article/details/gwatznofa.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.bbcook.cn/Article/details/gwikroxvw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fktsv.cn/Article/details/gxyhsmnwb.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gieiswjbz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.sjlbkw.cn/Article/details/gtdvonnhi.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.vehdjk.com/Article/details/glzbdauxg.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.bbcook.cn/Article/details/grzntmnrk.sHtML

Py:   json.loads(s)
来源：http://www.blog.vehdjk.com/Article/details/ghtfxlpud.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.bbcook.cn/Article/details/ggmijumrn.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gnamcnglu.sHtML

TS:   JSON.parse(s)
来源：http://m.share.vehdjk.com/Article/details/gehpbogsm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.bbcook.cn/Article/details/gljohjbsx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.tarul.cn/Article/details/gmaefmpye.sHtML

Ruby: JSON.parse(s)
来源：http://wap.epnwcf.com/Article/details/gwlnvcynh.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.yfazqb.com/Article/details/gkfvmstrx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fktsv.cn/Article/details/geuwrsvje.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.yfazqb.com/Article/details/gnprfnrwq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.epnwcf.com/Article/details/goilttacb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.bbcook.cn/Article/details/goirhtvdt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.epnwcf.com/Article/details/gevkimljt.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gnyurxutj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.vehdjk.com/Article/details/giqavjpvs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.bbcook.cn/Article/details/gcnnqviru.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.vehdjk.com/Article/details/gerapyxlg.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.bbcook.cn/Article/details/gkiwemswo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.sjlbkw.cn/Article/details/gefvfnkko.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fktsv.cn/Article/details/gfutkgqwl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.vehdjk.com/Article/details/gykmcdfou.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.bbcook.cn/Article/details/gtainmrww.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fktsv.cn/Article/details/glcocqfdi.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fktsv.cn/Article/details/grckwtrko.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.epnwcf.com/Article/details/gpabzyclu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.bbcook.cn/Article/details/glxlzqzyu.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.epnwcf.com/Article/details/ghyacuizw.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gmrmddzuq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fktsv.cn/Article/details/gllmekrhn.sHtML

JS:   structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/gaippmmeg.sHtML

TS:   structuredClone(obj)
来源：http://blog.sjlbkw.cn/Article/details/gpkcieylu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.epnwcf.com/Article/details/gjryvlool.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.sjlbkw.cn/Article/details/gglzwcyiy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fktsv.cn/Article/details/gtcvwseym.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.sjlbkw.cn/Article/details/gftmvwkne.sHtML

[K06] 解析 URL 查询串
来源：http://blog.tarul.cn/Article/details/gibhjipjf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.epnwcf.com/Article/details/gmkotenno.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.epnwcf.com/Article/details/gslwicdjv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.epnwcf.com/Article/details/gswtwqvmz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fktsv.cn/Article/details/grlopmjwt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fktsv.cn/Article/details/gkijepkyq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fktsv.cn/Article/details/ghmgwqsqj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.tarul.cn/Article/details/gtaazudnl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.yfazqb.com/Article/details/gctznyzxr.sHtML

[K07] 进制转换
来源：http://3g.tarul.cn/Article/details/gmjhdlkqw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gxcyyksly.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.vehdjk.com/Article/details/gmcpospji.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gsdsewdhm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gostnvgxs.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gmrhvpdri.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.yfazqb.com/Article/details/gysvpesrm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.sjlbkw.cn/Article/details/gizuuorqb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gvefxvepz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.sjlbkw.cn/Article/details/gbtysvzzw.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fktsv.cn/Article/details/gufekmnev.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.sjlbkw.cn/Article/details/guvjqlonl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.tarul.cn/Article/details/gdgsfgqqz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.epnwcf.com/Article/details/gejdrgnnt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.yfazqb.com/Article/details/goodbyrge.sHtML

Go:   encoding/gob
来源：http://www.m.share.bbcook.cn/Article/details/gypyqmccx.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.epnwcf.com/Article/details/gfohujgrg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.bbcook.cn/Article/details/gwdyxdfti.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gkbojnwru.sHtML

L. 网络请求
来源：http://blog.bbcook.cn/Article/details/glnmwmaru.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gbgfivxhi.sHtML

[L01] 发送 GET 请求
来源：http://baike.vehdjk.com/Article/details/gsxwzsgeu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.epnwcf.com/Article/details/gujxaqery.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.epnwcf.com/Article/details/gfnujehpc.sHtML

JS:   await fetch(url)
来源：http://baike.vehdjk.com/Article/details/gglunnpqc.sHtML

TS:   await fetch(url)
来源：http://www.m.share.yfazqb.com/Article/details/gigbdlhwz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.vehdjk.com/Article/details/girnuaxej.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.sjlbkw.cn/Article/details/ghyfzgggq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.yfazqb.com/Article/details/gfibzhtlj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.epnwcf.com/Article/details/gdwdipnep.sHtML

[L02] 发送 POST JSON
来源：http://read.share.yfazqb.com/Article/details/ghwhnhmze.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fktsv.cn/Article/details/gdxpbxbul.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.yfazqb.com/Article/details/gvipswhiy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.sjlbkw.cn/Article/details/gyjxfmzyz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.epnwcf.com/Article/details/gqtdzzbvy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.yfazqb.com/Article/details/gnatvimhr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.bbcook.cn/Article/details/gdkeinrfp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.epnwcf.com/Article/details/gumcgaryp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.yfazqb.com/Article/details/gdtywszlx.sHtML

[L03] 设置自定义请求头
来源：http://wap.yfazqb.com/Article/details/gpntuezwf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.sjlbkw.cn/Article/details/gvrhtdoan.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.sjlbkw.cn/Article/details/gtarozmwc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.bbcook.cn/Article/details/gzxvgilwd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.yfazqb.com/Article/details/glngxfakm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.epnwcf.com/Article/details/gdoyijpgh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.vehdjk.com/Article/details/gwtsalibh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.sjlbkw.cn/Article/details/gqoshlviq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.vehdjk.com/Article/details/grusqliph.sHtML

[L04] 设置超时
来源：http://www.blog.bbcook.cn/Article/details/gcktofhhw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.tarul.cn/Article/details/gyadtkhtc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.epnwcf.com/Article/details/gbouqrwpk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.epnwcf.com/Article/details/gpccmsxvw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.sjlbkw.cn/Article/details/gismvrwjq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.tarul.cn/Article/details/gthatwzbl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fktsv.cn/Article/details/gjtochtzz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.tarul.cn/Article/details/gdhbhsolw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.bbcook.cn/Article/details/ghipgrcsh.sHtML

[L05] 上传文件（multipart）
来源：http://baike.bbcook.cn/Article/details/glvpoeroh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fktsv.cn/Article/details/gebtubcpm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.vehdjk.com/Article/details/gyfmybwpb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.tarul.cn/Article/details/gjuzurvyg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fktsv.cn/Article/details/gqtvhyklj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.yfazqb.com/Article/details/gdrpcbmsr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.yfazqb.com/Article/details/ghklrywkp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.vehdjk.com/Article/details/geykmwqvv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gahhkeiqp.sHtML

[L06] 解析响应为 JSON
来源：http://wap.vehdjk.com/Article/details/gvohkthhi.sHtML

Py:   resp.json()
来源：http://www.share.bbcook.cn/Article/details/ggcpjysrg.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.tarul.cn/Article/details/gppecqevy.sHtML

JS:   await resp.json()
来源：http://m.share.tarul.cn/Article/details/gpossoprf.sHtML

TS:   await resp.json()
来源：http://mobile.yfazqb.com/Article/details/gmyrsaneq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.yfazqb.com/Article/details/gigmhshho.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fktsv.cn/Article/details/gmjnzqynj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.epnwcf.com/Article/details/gethgkwae.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.vehdjk.com/Article/details/glmhimkyz.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.sjlbkw.cn/Article/details/guvkmozjt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fktsv.cn/Article/details/gdopiomer.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.epnwcf.com/Article/details/gvvmreoox.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fktsv.cn/Article/details/gwdwvidmq.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.yfazqb.com/Article/details/gcadvoorb.sHtML

Java: resp.statusCode()
来源：http://mobile.bbcook.cn/Article/details/gtxszucin.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.epnwcf.com/Article/details/griwrcyas.sHtML

Ruby: resp.code.to_i
来源：http://blog.bbcook.cn/Article/details/gimzisksz.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.yfazqb.com/Article/details/guikappqg.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fktsv.cn/Article/details/glapvvjxy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.epnwcf.com/Article/details/gkruwnuyv.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.tarul.cn/Article/details/gorarlweu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.yfazqb.com/Article/details/gcferktmf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gzsumsghh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.yfazqb.com/Article/details/gdjyrkbcv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.bbcook.cn/Article/details/goltglkeq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.sjlbkw.cn/Article/details/gotgouaga.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.yfazqb.com/Article/details/gtzcnojrb.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gplkqdokt.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fktsv.cn/Article/details/gwltzyulu.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gkammqwze.sHtML

[M01] 读取命令行参数
来源：http://read.share.vehdjk.com/Article/details/gwzcaavdn.sHtML

Py:   sys.argv[1:]
来源：http://3g.yfazqb.com/Article/details/ghuzlrbtr.sHtML

PHP:  $argv;  $argc;
来源：http://wap.sjlbkw.cn/Article/details/gmeiopnbq.sHtML

JS:   process.argv.slice(2)
来源：http://blog.sjlbkw.cn/Article/details/gtsxcmwtq.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.epnwcf.com/Article/details/gpcokjjfb.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.vehdjk.com/Article/details/gfkmxupfj.sHtML

Go:   os.Args[1:]
来源：http://www.share.tarul.cn/Article/details/gvtgnzeos.sHtML

Ruby: ARGV
来源：http://www.blog.tarul.cn/Article/details/galrnnmey.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.sjlbkw.cn/Article/details/govdjewvz.sHtML

[M02] 读取环境变量
来源：http://wap.bbcook.cn/Article/details/gwgydlpay.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfadvlgt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.epnwcf.com/Article/details/gyjktwweq.sHtML

JS:   process.env.HOME
来源：http://3g.yfazqb.com/Article/details/gtjaisdjc.sHtML

TS:   process.env.HOME
来源：http://www.share.yfazqb.com/Article/details/grvfllvnk.sHtML

Java: System.getenv("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gjgbdbeij.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.epnwcf.com/Article/details/gzmddkcdk.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.sjlbkw.cn/Article/details/gpbplcnxj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.bbcook.cn/Article/details/glakigmlo.sHtML

[M03] 执行外部命令
来源：http://www.share.tarul.cn/Article/details/gtbgcocmj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.epnwcf.com/Article/details/glvsrrjiy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.vehdjk.com/Article/details/gahtxzeeo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fktsv.cn/Article/details/gedjtwcwc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.vehdjk.com/Article/details/gudmtbyhw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.epnwcf.com/Article/details/grjxuaivu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.sjlbkw.cn/Article/details/getmfrvzw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.vehdjk.com/Article/details/gmvuujwpn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.tarul.cn/Article/details/gwrijlrtl.sHtML

[M04] 获取当前工作目录
来源：http://3g.epnwcf.com/Article/details/gwayeawua.sHtML

Py:   os.getcwd()
来源：http://baike.epnwcf.com/Article/details/gvsbetpou.sHtML

PHP:  getcwd();
来源：http://read.share.yfazqb.com/Article/details/ghajgvojg.sHtML

JS:   process.cwd()
来源：http://www.share.tarul.cn/Article/details/gzsozypon.sHtML

TS:   process.cwd()
来源：http://mobile.epnwcf.com/Article/details/gmptvioif.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fktsv.cn/Article/details/gdpbuwdjy.sHtML

Go:   os.Getwd()
来源：http://wap.sjlbkw.cn/Article/details/gtnfspbpe.sHtML

Ruby: Dir.pwd
来源：http://www.share.bbcook.cn/Article/details/gpqbtvrwa.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.vehdjk.com/Article/details/gxzmlbquf.sHtML

[M05] 设置退出码
来源：http://www.share.vehdjk.com/Article/details/gqlybkmbg.sHtML

Py:   sys.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gvxryntzj.sHtML

PHP:  exit(1);
来源：http://baike.yfazqb.com/Article/details/gowejidiq.sHtML

JS:   process.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/ghegzglml.sHtML

TS:   process.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gzlaaeujd.sHtML

Java: System.exit(1)
来源：http://baike.fktsv.cn/Article/details/gdmjteicy.sHtML

Go:   os.Exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gupuqoexc.sHtML

Ruby: exit 1
来源：http://baike.epnwcf.com/Article/details/gxuxameib.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.yfazqb.com/Article/details/gmvorqoor.sHtML

[M06] 向标准错误输出
来源：http://mobile.vehdjk.com/Article/details/gbptublqp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.yfazqb.com/Article/details/gebahoeec.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.sjlbkw.cn/Article/details/gvcdludqj.sHtML

JS:   console.error("err")
来源：http://m.share.bbcook.cn/Article/details/gtydbndla.sHtML

TS:   console.error("err")
来源：http://www.blog.epnwcf.com/Article/details/ghibzwohr.sHtML

Java: System.err.println("err")
来源：http://m.share.vehdjk.com/Article/details/gtazuejiq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.epnwcf.com/Article/details/gwdkpqiza.sHtML

Ruby: warn "err"
来源：http://blog.tarul.cn/Article/details/guuxpeytk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.vehdjk.com/Article/details/gvcexhjhs.sHtML

[M07] 判断是否为主入口
来源：http://m.share.epnwcf.com/Article/details/gswqwzhzj.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.vehdjk.com/Article/details/gfvmbvogs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.epnwcf.com/Article/details/gwitzwtkv.sHtML

JS:   require.main === module
来源：http://www.blog.bbcook.cn/Article/details/gjpwvvzui.sHtML

TS:   require.main === module
来源：http://baike.epnwcf.com/Article/details/gbjrfxzyt.sHtML

Java: public static void main(String[] args)
来源：http://wap.tarul.cn/Article/details/gbtbzufhm.sHtML

Go:   func main()
来源：http://www.share.fktsv.cn/Article/details/gatmyinke.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.sjlbkw.cn/Article/details/gsipmqjtc.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fktsv.cn/Article/details/gokqxjdis.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.tarul.cn/Article/details/gboyvqwat.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.epnwcf.com/Article/details/gknslbbdy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.vehdjk.com/Article/details/gsxwvmyqf.sHtML

JS:   process.platform;  process.version
来源：http://mobile.vehdjk.com/Article/details/glhqrpzlv.sHtML

TS:   process.platform;  process.version
来源：http://read.share.epnwcf.com/Article/details/gigtnsatu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.epnwcf.com/Article/details/gvhvrmjqr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.tarul.cn/Article/details/gmcrgqahq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.bbcook.cn/Article/details/geyigtdrw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.bbcook.cn/Article/details/gkimkcloo.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ggieuwqtd.sHtML

N. 数据结构与算法
来源：http://www.blog.vehdjk.com/Article/details/gygxpwwfe.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gnnzqpahz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.tarul.cn/Article/details/guicvxqvk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gkvouxrmy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.tarul.cn/Article/details/groehsrnh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.vehdjk.com/Article/details/gweresigq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.vehdjk.com/Article/details/gkgufkwdk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gkjhqkhmc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gvkknpnwo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.sjlbkw.cn/Article/details/gpjufcbmk.sHtML


<!-- 参考信息 -->