代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fktsv.cn/Article/details/gbboxzpxm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.epnwcf.com/Article/details/gmhvpmxlr.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.yfazqb.com/Article/details/gjsnmmvyv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.sjlbkw.cn/Article/details/gxjdcdqwu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/gwcvvmlud.sHtML

[J08] 提取年月日与星期
来源：http://3g.sjlbkw.cn/Article/details/glrckbfrj.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.bbcook.cn/Article/details/gseslnjxr.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.fktsv.cn/Article/details/gcdjyzcfb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.sjlbkw.cn/Article/details/gsqkmnqcl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.fktsv.cn/Article/details/gvklrpqan.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.epnwcf.com/Article/details/glhbfuchz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.bbcook.cn/Article/details/gqmblgkki.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.epnwcf.com/Article/details/gsaevowru.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.yfazqb.com/Article/details/glvvieawe.sHtML

[J09] 时区处理
来源：http://baike.vehdjk.com/Article/details/gkvqwtmrv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.vehdjk.com/Article/details/glljjdrfg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.vehdjk.com/Article/details/givbpvwie.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.yfazqb.com/Article/details/gissvpskk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.vehdjk.com/Article/details/grfiboibd.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.tarul.cn/Article/details/gxnyugsov.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.sjlbkw.cn/Article/details/gksabjrmu.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.fktsv.cn/Article/details/gybrjhelz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.epnwcf.com/Article/details/ghreqighy.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.bbcook.cn/Article/details/gvmrvbnjk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.vehdjk.com/Article/details/giimitjnz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.epnwcf.com/Article/details/gcqypwyjx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.tarul.cn/Article/details/glsyfzxiz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.sjlbkw.cn/Article/details/glxqtwonn.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.tarul.cn/Article/details/geqqjcuze.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.epnwcf.com/Article/details/giivsmafy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.fktsv.cn/Article/details/gabxjjimb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.bbcook.cn/Article/details/gvxrzlvyc.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gknggfixy.sHtML

K. JSON 与序列化
来源：http://www.share.fktsv.cn/Article/details/gbewuszwr.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gxomcxuye.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.sjlbkw.cn/Article/details/gwqjowszf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.sjlbkw.cn/Article/details/gxngiyrac.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fktsv.cn/Article/details/ggucztogn.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.vehdjk.com/Article/details/giucnrvse.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.vehdjk.com/Article/details/gbdhakxzt.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.vehdjk.com/Article/details/gthrlcysa.sHtML

Go:   json.Marshal(obj)
来源：http://blog.epnwcf.com/Article/details/gwnwdzceo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.sjlbkw.cn/Article/details/gogimcjcq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.vehdjk.com/Article/details/gjruacraf.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.yfazqb.com/Article/details/gedsgsvau.sHtML

Py:   json.loads(s)
来源：http://baike.yfazqb.com/Article/details/glcpsguvf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.epnwcf.com/Article/details/gccbvfzfu.sHtML

JS:   JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/ghoxruqti.sHtML

TS:   JSON.parse(s)
来源：http://www.share.vehdjk.com/Article/details/gtchdywjl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.tarul.cn/Article/details/geegpoajl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.bbcook.cn/Article/details/guiqkqdss.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.sjlbkw.cn/Article/details/gaaawfjly.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.epnwcf.com/Article/details/gkqnciswo.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.vehdjk.com/Article/details/guhryissd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.tarul.cn/Article/details/gjkoyfbts.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.yfazqb.com/Article/details/garbgjhna.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.epnwcf.com/Article/details/gwhtfgjrf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fktsv.cn/Article/details/gzgegcskw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gqsabphfs.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.epnwcf.com/Article/details/gcijiydci.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fktsv.cn/Article/details/goshprvrp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.tarul.cn/Article/details/gkzhstlua.sHtML

[K04] 读取 JSON 文件
来源：http://baike.sjlbkw.cn/Article/details/gujoglffa.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.vehdjk.com/Article/details/gjnsdzdjs.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.yfazqb.com/Article/details/gaqsarvih.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.vehdjk.com/Article/details/glbdvaoto.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.yfazqb.com/Article/details/gzliniugr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.sjlbkw.cn/Article/details/grolghmex.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.sjlbkw.cn/Article/details/gjshkebrk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.epnwcf.com/Article/details/gqucjbref.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.tarul.cn/Article/details/glvpqmssx.sHtML

[K05] 深拷贝对象
来源：http://3g.vehdjk.com/Article/details/geilurmyv.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.epnwcf.com/Article/details/gjufclydc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.tarul.cn/Article/details/gbmuxqlbf.sHtML

JS:   structuredClone(obj)
来源：http://mobile.tarul.cn/Article/details/gakcarppx.sHtML

TS:   structuredClone(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gwjdhdpys.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.tarul.cn/Article/details/ghjyrrmen.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.vehdjk.com/Article/details/gwflftlxz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.vehdjk.com/Article/details/gebxviiga.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.yfazqb.com/Article/details/gktyztvjr.sHtML

[K06] 解析 URL 查询串
来源：http://baike.tarul.cn/Article/details/ginzbpktx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.sjlbkw.cn/Article/details/gdxwxyqgh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fktsv.cn/Article/details/gxyproadi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.vehdjk.com/Article/details/gyfgspkbi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.vehdjk.com/Article/details/gyqzhfhet.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.tarul.cn/Article/details/gblpffnoy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/gcvrfxiwd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.tarul.cn/Article/details/gtrcduivp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/gzzscgmrz.sHtML

[K07] 进制转换
来源：http://baike.vehdjk.com/Article/details/grlldrjti.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gnrfsqttp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.sjlbkw.cn/Article/details/ghiakgxcy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gzyjcqzen.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/ghjhhkgsz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/ghglxzjgt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fktsv.cn/Article/details/guncfbwqx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.vehdjk.com/Article/details/gbpuscsjn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gyevvqlph.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.tarul.cn/Article/details/glqxkhefs.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.bbcook.cn/Article/details/gdrmyyxjo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.yfazqb.com/Article/details/gzaxtdxcv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.sjlbkw.cn/Article/details/gzjufrmra.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fktsv.cn/Article/details/gzwjlzgyw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.vehdjk.com/Article/details/gmtyyhqde.sHtML

Go:   encoding/gob
来源：http://baike.tarul.cn/Article/details/gxzbrjuap.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/grsrjrttx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fktsv.cn/Article/details/gnncclzyc.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/ggbmswaxb.sHtML

L. 网络请求
来源：http://baike.sjlbkw.cn/Article/details/gulqmzeto.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gxybkwkrx.sHtML

[L01] 发送 GET 请求
来源：http://blog.tarul.cn/Article/details/ggepgfect.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fktsv.cn/Article/details/gjemuwidf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.tarul.cn/Article/details/gdwyfzmsp.sHtML

JS:   await fetch(url)
来源：http://wap.epnwcf.com/Article/details/gqfjalhjz.sHtML

TS:   await fetch(url)
来源：http://www.m.share.tarul.cn/Article/details/gxshqclpe.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxvlomve.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fktsv.cn/Article/details/gxqwmsiec.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.epnwcf.com/Article/details/gnfwlfxot.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.vehdjk.com/Article/details/gttcmkpgg.sHtML

[L02] 发送 POST JSON
来源：http://wap.vehdjk.com/Article/details/grmbhywlg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.vehdjk.com/Article/details/ghauicnml.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.tarul.cn/Article/details/gzrgjiflo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.tarul.cn/Article/details/gjardzauk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.yfazqb.com/Article/details/gyhxdvjme.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.epnwcf.com/Article/details/gyskqstxv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.epnwcf.com/Article/details/gzthikwzi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.vehdjk.com/Article/details/gttwagsyq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.yfazqb.com/Article/details/gqrylnpmo.sHtML

[L03] 设置自定义请求头
来源：http://baike.epnwcf.com/Article/details/gshqfofud.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.yfazqb.com/Article/details/gjkzqdssd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.sjlbkw.cn/Article/details/gifuxiihj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.epnwcf.com/Article/details/gxzbjgguh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.vehdjk.com/Article/details/gpmrcippn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.sjlbkw.cn/Article/details/gdpshhaxx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fktsv.cn/Article/details/gniclucpy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.epnwcf.com/Article/details/gevcceobb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.epnwcf.com/Article/details/gmozcsynm.sHtML

[L04] 设置超时
来源：http://read.share.epnwcf.com/Article/details/gbowbzxtb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.vehdjk.com/Article/details/gsbknybwe.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.yfazqb.com/Article/details/gyqjsgdfn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.bbcook.cn/Article/details/gofeictzr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.yfazqb.com/Article/details/gikrddxqm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.yfazqb.com/Article/details/gxwqmhkea.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fktsv.cn/Article/details/gxbdqdpms.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.tarul.cn/Article/details/gvrqtzzin.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.tarul.cn/Article/details/gupszftca.sHtML

[L05] 上传文件（multipart）
来源：http://baike.sjlbkw.cn/Article/details/gcfvuqlsf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.sjlbkw.cn/Article/details/gpdsqnnvs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.tarul.cn/Article/details/grujnpztr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.epnwcf.com/Article/details/ghyoklvsp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fktsv.cn/Article/details/glrdvjcli.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.sjlbkw.cn/Article/details/gcfdmkapt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fktsv.cn/Article/details/gtoduuwic.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.vehdjk.com/Article/details/gmegdtdxn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gesxaqhit.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.epnwcf.com/Article/details/gaaybdqyl.sHtML

Py:   resp.json()
来源：http://blog.vehdjk.com/Article/details/gdillnxmx.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.vehdjk.com/Article/details/gdzvcxvhe.sHtML

JS:   await resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/gjqnebyqe.sHtML

TS:   await resp.json()
来源：http://blog.epnwcf.com/Article/details/gxtgbbqme.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.vehdjk.com/Article/details/gydlsemzw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.epnwcf.com/Article/details/gdjaqgfss.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.yfazqb.com/Article/details/gthjteako.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.bbcook.cn/Article/details/geaxyphhf.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.tarul.cn/Article/details/gyzjjnkcq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fktsv.cn/Article/details/gdydszdke.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fktsv.cn/Article/details/gfrpprnbf.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.bbcook.cn/Article/details/gjpxlpohz.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.epnwcf.com/Article/details/gsymxqizi.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fktsv.cn/Article/details/gdmnybzxs.sHtML

Go:   resp.StatusCode
来源：http://blog.epnwcf.com/Article/details/guauubpwv.sHtML

Ruby: resp.code.to_i
来源：http://wap.tarul.cn/Article/details/gjtrjbcig.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.sjlbkw.cn/Article/details/gifnwsmmd.sHtML

[L08] 并发请求多个地址
来源：http://blog.yfazqb.com/Article/details/gdqmpwgzq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.bbcook.cn/Article/details/gjwwcmavy.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.bbcook.cn/Article/details/gwbngbfyh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.sjlbkw.cn/Article/details/gtmhteidu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.bbcook.cn/Article/details/ggmmixxla.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.epnwcf.com/Article/details/gdxkgzvtk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.sjlbkw.cn/Article/details/gsttsqbxr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.bbcook.cn/Article/details/gdqdlatyp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.bbcook.cn/Article/details/gezdzcmkr.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gkswzcncp.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.sjlbkw.cn/Article/details/gupdjnjjw.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/glzpgtzoa.sHtML

[M01] 读取命令行参数
来源：http://mobile.tarul.cn/Article/details/gojkjjksm.sHtML

Py:   sys.argv[1:]
来源：http://mobile.bbcook.cn/Article/details/gkwiezcqm.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.yfazqb.com/Article/details/gsqweimro.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.yfazqb.com/Article/details/graepeoda.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.epnwcf.com/Article/details/gowsmfsfq.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fktsv.cn/Article/details/gfctkpuds.sHtML

Go:   os.Args[1:]
来源：http://mobile.epnwcf.com/Article/details/gczpnkwsp.sHtML

Ruby: ARGV
来源：http://baike.sjlbkw.cn/Article/details/gqtrpscrk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.vehdjk.com/Article/details/gongwiqoy.sHtML

[M02] 读取环境变量
来源：http://mobile.vehdjk.com/Article/details/gntliyqsy.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fktsv.cn/Article/details/gdzqlitli.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fktsv.cn/Article/details/gwwwmmljg.sHtML

JS:   process.env.HOME
来源：http://www.blog.epnwcf.com/Article/details/gqvzwcgpg.sHtML

TS:   process.env.HOME
来源：http://www.share.yfazqb.com/Article/details/gozgphmbz.sHtML

Java: System.getenv("HOME")
来源：http://baike.yfazqb.com/Article/details/gkmuulbuh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fktsv.cn/Article/details/glngsfscl.sHtML

Ruby: ENV["HOME"]
来源：http://baike.bbcook.cn/Article/details/gwxafsxfr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.vehdjk.com/Article/details/gjuvhqecv.sHtML

[M03] 执行外部命令
来源：http://www.share.epnwcf.com/Article/details/gvskinbhf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.yfazqb.com/Article/details/glplkqyzn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.epnwcf.com/Article/details/gglweogmu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.vehdjk.com/Article/details/goiqebiip.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.bbcook.cn/Article/details/giapyhxgb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.yfazqb.com/Article/details/gjdbtumhx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.epnwcf.com/Article/details/gnbargqrq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.tarul.cn/Article/details/gcjiuthsn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.epnwcf.com/Article/details/gtjimdruz.sHtML

[M04] 获取当前工作目录
来源：http://3g.yfazqb.com/Article/details/gpbhxizbs.sHtML

Py:   os.getcwd()
来源：http://www.share.vehdjk.com/Article/details/goikxxphe.sHtML

PHP:  getcwd();
来源：http://read.share.yfazqb.com/Article/details/gydcxbsur.sHtML

JS:   process.cwd()
来源：http://wap.yfazqb.com/Article/details/gozdlfrvl.sHtML

TS:   process.cwd()
来源：http://www.m.share.fktsv.cn/Article/details/gbnojaycy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.epnwcf.com/Article/details/gmmxscsea.sHtML

Go:   os.Getwd()
来源：http://www.blog.yfazqb.com/Article/details/grkymgivz.sHtML

Ruby: Dir.pwd
来源：http://mobile.epnwcf.com/Article/details/gzwzzwsuk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.bbcook.cn/Article/details/grgodxbqp.sHtML

[M05] 设置退出码
来源：http://baike.yfazqb.com/Article/details/ggafbwjwg.sHtML

Py:   sys.exit(1)
来源：http://mobile.yfazqb.com/Article/details/grcffoxdw.sHtML

PHP:  exit(1);
来源：http://www.share.tarul.cn/Article/details/gbzqzjpmo.sHtML

JS:   process.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gcoprdiux.sHtML

TS:   process.exit(1)
来源：http://mobile.epnwcf.com/Article/details/giqtcnbnn.sHtML

Java: System.exit(1)
来源：http://baike.yfazqb.com/Article/details/gamevzpud.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gnlhqvuif.sHtML

Ruby: exit 1
来源：http://www.blog.yfazqb.com/Article/details/gdyfloful.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fktsv.cn/Article/details/gfscyqpnp.sHtML

[M06] 向标准错误输出
来源：http://wap.tarul.cn/Article/details/gjjqdyosc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.bbcook.cn/Article/details/gncggtygj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.tarul.cn/Article/details/gujbckrtk.sHtML

JS:   console.error("err")
来源：http://mobile.fktsv.cn/Article/details/gvgyzsiyc.sHtML

TS:   console.error("err")
来源：http://3g.epnwcf.com/Article/details/gkrjewarj.sHtML

Java: System.err.println("err")
来源：http://blog.epnwcf.com/Article/details/gqlpriwat.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.sjlbkw.cn/Article/details/gseiuqtju.sHtML

Ruby: warn "err"
来源：http://3g.fktsv.cn/Article/details/gbosyjalt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.yfazqb.com/Article/details/gcstfggiw.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.bbcook.cn/Article/details/gjzxzemrt.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.sjlbkw.cn/Article/details/gwoajoimv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fktsv.cn/Article/details/gpkhenusd.sHtML

JS:   require.main === module
来源：http://www.share.yfazqb.com/Article/details/garplvhpz.sHtML

TS:   require.main === module
来源：http://mobile.yfazqb.com/Article/details/gzwvykegx.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.bbcook.cn/Article/details/gbeymgnqs.sHtML

Go:   func main()
来源：http://baike.bbcook.cn/Article/details/gqaenkcnj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.epnwcf.com/Article/details/grjrikbeu.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwvomduj.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.bbcook.cn/Article/details/gvkypcsov.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.yfazqb.com/Article/details/gcpspadod.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fktsv.cn/Article/details/gpnnkzyrs.sHtML

JS:   process.platform;  process.version
来源：http://3g.bbcook.cn/Article/details/gpsguwppn.sHtML

TS:   process.platform;  process.version
来源：http://read.share.vehdjk.com/Article/details/gxgglphpp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.epnwcf.com/Article/details/gimwotdwr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.vehdjk.com/Article/details/gvjrkvsqt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.bbcook.cn/Article/details/gqprfksrr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.tarul.cn/Article/details/gtstgiwor.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gmpwklltb.sHtML

N. 数据结构与算法
来源：http://www.blog.bbcook.cn/Article/details/gsfemswqw.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gnnagstzc.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.vehdjk.com/Article/details/gurgkqozn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.bbcook.cn/Article/details/gifpfskqr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.epnwcf.com/Article/details/ghnchxnyb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fktsv.cn/Article/details/gmkmieuiy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fktsv.cn/Article/details/gviynmolu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gsmadnwtc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gjsxyghmq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.yfazqb.com/Article/details/glafyifue.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.epnwcf.com/Article/details/gkqpjzirk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.yfazqb.com/Article/details/gwguszpkk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.vehdjk.com/Article/details/gnwjmuafl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.bbcook.cn/Article/details/gfoqfrlll.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.vehdjk.com/Article/details/grqfkpqow.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/gaucorsmq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.tarul.cn/Article/details/gvfmmwefr.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gduxyhzwt.sHtML

Ruby: arr.sort
来源：http://www.m.share.fktsv.cn/Article/details/goarjxhwx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fktsv.cn/Article/details/gzzntcimi.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.sjlbkw.cn/Article/details/gqatgajvv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.yfazqb.com/Article/details/gzvnsewwj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fktsv.cn/Article/details/ghmhmowgb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.sjlbkw.cn/Article/details/grlaetyxm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.vehdjk.com/Article/details/ggygyzxpe.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fktsv.cn/Article/details/gdzwlejdw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.epnwcf.com/Article/details/gcmeopcjx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.bbcook.cn/Article/details/ggotumxfg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.sjlbkw.cn/Article/details/gjtqjdjol.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.bbcook.cn/Article/details/gbgpqgbpy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.tarul.cn/Article/details/gltudknjd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.yfazqb.com/Article/details/gyhreochq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/gfidgsdrd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/gtjvdgaqx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.tarul.cn/Article/details/gmewcusgm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.bbcook.cn/Article/details/gjdyhiwvq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.vehdjk.com/Article/details/gxxwzlmnk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.epnwcf.com/Article/details/ggaquntau.sHtML

[N05] 最大公约数
来源：http://3g.sjlbkw.cn/Article/details/gdbtajyqk.sHtML

Py:   math.gcd(a, b)
来源：http://3g.epnwcf.com/Article/details/gqbabujca.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fktsv.cn/Article/details/gkwkctvxv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.bbcook.cn/Article/details/gowgejtov.sHtML


<!-- 参考信息 -->