代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.yfazqb.com/Article/details/ggrugmcdg.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.bbcook.cn/Article/details/gljcijfqr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.fktsv.cn/Article/details/geiyertko.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.bbcook.cn/Article/details/ghljtkuos.sHtML

[J07] 比较两个日期
来源：http://www.blog.epnwcf.com/Article/details/gdjijxqbe.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.epnwcf.com/Article/details/gyreistfe.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.vehdjk.com/Article/details/gqlpwpjoj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fktsv.cn/Article/details/gvazwccku.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.vehdjk.com/Article/details/gwolfkpbl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.bbcook.cn/Article/details/gnteliybm.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.bbcook.cn/Article/details/gwumgreqq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.sjlbkw.cn/Article/details/gqffpidkq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.sjlbkw.cn/Article/details/ggepaycmh.sHtML

[J08] 提取年月日与星期
来源：http://blog.bbcook.cn/Article/details/gjttzakmm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.yfazqb.com/Article/details/gdyoupaye.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.yfazqb.com/Article/details/gdhcupsvc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.sjlbkw.cn/Article/details/gqcqioifq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.epnwcf.com/Article/details/gpwnjlnhb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.vehdjk.com/Article/details/gidhsemjv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.bbcook.cn/Article/details/gftssqywi.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.tarul.cn/Article/details/geiegvsac.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.sjlbkw.cn/Article/details/gbgipaula.sHtML

[J09] 时区处理
来源：http://www.blog.vehdjk.com/Article/details/grubizvgz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.epnwcf.com/Article/details/gmscmhhlf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.bbcook.cn/Article/details/gkykmitfy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fktsv.cn/Article/details/gyszwqtvt.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.sjlbkw.cn/Article/details/gevxykoxl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.vehdjk.com/Article/details/glcqojyrg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.yfazqb.com/Article/details/gmghikjyz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.bbcook.cn/Article/details/gnaurtufh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.sjlbkw.cn/Article/details/gkzxckdry.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.yfazqb.com/Article/details/gcerrhnlj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.bbcook.cn/Article/details/gspwnnldw.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.tarul.cn/Article/details/gtyyctxpi.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.sjlbkw.cn/Article/details/gzpfpfmlu.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fktsv.cn/Article/details/gokudcjad.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.epnwcf.com/Article/details/gwovdtboy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.bbcook.cn/Article/details/gxypuqatr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.tarul.cn/Article/details/gaxvbahwf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.sjlbkw.cn/Article/details/glmkodqfe.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gvyyaajci.sHtML

K. JSON 与序列化
来源：http://www.share.bbcook.cn/Article/details/gdnxyyldt.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gqjxykfhf.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.yfazqb.com/Article/details/gdvthaloz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.epnwcf.com/Article/details/glvdwnonk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fktsv.cn/Article/details/gqmfdotcm.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.sjlbkw.cn/Article/details/gmoigtwex.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.yfazqb.com/Article/details/glyilmxtp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.epnwcf.com/Article/details/gdsofzapr.sHtML

Go:   json.Marshal(obj)
来源：http://wap.vehdjk.com/Article/details/gvqngxeft.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.sjlbkw.cn/Article/details/gaegnaykk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.bbcook.cn/Article/details/gudryredu.sHtML

[K02] JSON 字符串转对象
来源：http://3g.vehdjk.com/Article/details/gilatfrgy.sHtML

Py:   json.loads(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghslwfvtn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.epnwcf.com/Article/details/gsgexcvpq.sHtML

JS:   JSON.parse(s)
来源：http://baike.epnwcf.com/Article/details/glhngknzr.sHtML

TS:   JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/glmsoxjda.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.tarul.cn/Article/details/gwcikbfen.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.bbcook.cn/Article/details/gijvbemoa.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.bbcook.cn/Article/details/gvtmhaqbv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.fktsv.cn/Article/details/gqkxfubgk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.sjlbkw.cn/Article/details/gbbskvbnj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.fktsv.cn/Article/details/gobaicaeo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.yfazqb.com/Article/details/gfsdhuzsi.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.yfazqb.com/Article/details/grfcqsrih.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.sjlbkw.cn/Article/details/guvjjuora.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.bbcook.cn/Article/details/gsilomxir.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.vehdjk.com/Article/details/ggkdusiis.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.vehdjk.com/Article/details/gvvfylsrs.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.epnwcf.com/Article/details/ghlxyujfp.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.epnwcf.com/Article/details/gpnbhcjeb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.bbcook.cn/Article/details/gadgvqypu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.tarul.cn/Article/details/gvtyblvvl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.vehdjk.com/Article/details/gtfaxiauf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.sjlbkw.cn/Article/details/glvtctpvs.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.vehdjk.com/Article/details/gvimaoxxk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.bbcook.cn/Article/details/gzbhmwgio.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.bbcook.cn/Article/details/gpyqboktb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.tarul.cn/Article/details/gugesesut.sHtML

[K05] 深拷贝对象
来源：http://www.share.epnwcf.com/Article/details/gfaruvjph.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gtiwhieii.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.sjlbkw.cn/Article/details/gkrcizjaf.sHtML

JS:   structuredClone(obj)
来源：http://m.share.yfazqb.com/Article/details/gjsjkmhjq.sHtML

TS:   structuredClone(obj)
来源：http://3g.fktsv.cn/Article/details/gygrsaapa.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.tarul.cn/Article/details/gcrmmkzwf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.bbcook.cn/Article/details/gbrjvxrry.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fktsv.cn/Article/details/grahfbnga.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.epnwcf.com/Article/details/gneescbnv.sHtML

[K06] 解析 URL 查询串
来源：http://baike.tarul.cn/Article/details/gfltrktkh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.vehdjk.com/Article/details/gaeddonbo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.sjlbkw.cn/Article/details/gfujdxsre.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.vehdjk.com/Article/details/gajwovrwr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.yfazqb.com/Article/details/gynxeipfb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.sjlbkw.cn/Article/details/goeswlkwo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.bbcook.cn/Article/details/glmwhuzno.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.yfazqb.com/Article/details/gpgkebkwd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/grklzbvvd.sHtML

[K07] 进制转换
来源：http://3g.yfazqb.com/Article/details/gvuwvbckz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.tarul.cn/Article/details/gzfjalhio.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.tarul.cn/Article/details/gfngaezxz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/gxsztamef.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gkcftkcdb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/grvrtafxf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.epnwcf.com/Article/details/gjyzduich.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.vehdjk.com/Article/details/gzwizllrt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gpdfjjdek.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.epnwcf.com/Article/details/gvdolwrbf.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.epnwcf.com/Article/details/gzewoaeuq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.tarul.cn/Article/details/gwigphrwa.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.yfazqb.com/Article/details/gjvjuuimg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.sjlbkw.cn/Article/details/guavfilqq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.epnwcf.com/Article/details/gghflwslc.sHtML

Go:   encoding/gob
来源：http://3g.yfazqb.com/Article/details/gzwvwrtzi.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.sjlbkw.cn/Article/details/glpbvbiik.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.yfazqb.com/Article/details/gcszkquvc.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/glavignjg.sHtML

L. 网络请求
来源：http://www.blog.epnwcf.com/Article/details/guvphecjg.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gdbtxphbl.sHtML

[L01] 发送 GET 请求
来源：http://baike.vehdjk.com/Article/details/gyboicjcx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.epnwcf.com/Article/details/gjfuhqpta.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.yfazqb.com/Article/details/gfinpukld.sHtML

JS:   await fetch(url)
来源：http://baike.epnwcf.com/Article/details/grhucikoo.sHtML

TS:   await fetch(url)
来源：http://blog.tarul.cn/Article/details/gbeubpjep.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.tarul.cn/Article/details/gmytbchsq.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.tarul.cn/Article/details/gbszwukyv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.sjlbkw.cn/Article/details/goxporsuo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.vehdjk.com/Article/details/gbutjefvu.sHtML

[L02] 发送 POST JSON
来源：http://wap.vehdjk.com/Article/details/gslkstdqy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.sjlbkw.cn/Article/details/gxahdpxwj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.sjlbkw.cn/Article/details/gmworfbun.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.yfazqb.com/Article/details/gcyedgqcu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.epnwcf.com/Article/details/gtmyjykvw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.bbcook.cn/Article/details/gmhmhyrni.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.sjlbkw.cn/Article/details/gxduydxqr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.yfazqb.com/Article/details/gszaswelb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.tarul.cn/Article/details/gdbbhmkng.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.yfazqb.com/Article/details/gdutbbtil.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.sjlbkw.cn/Article/details/gudqnadpn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.sjlbkw.cn/Article/details/gyrcaxgdd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.epnwcf.com/Article/details/gukonlgaf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.bbcook.cn/Article/details/gugimvbql.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.vehdjk.com/Article/details/gqyobcwcg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.sjlbkw.cn/Article/details/ggguyxzlr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.vehdjk.com/Article/details/gbegdjhjl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.vehdjk.com/Article/details/gbjqehosr.sHtML

[L04] 设置超时
来源：http://read.share.sjlbkw.cn/Article/details/gbecgdhwx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.tarul.cn/Article/details/glfixoizd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.sjlbkw.cn/Article/details/gnbsuvjjo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.vehdjk.com/Article/details/gmeqhheel.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fktsv.cn/Article/details/gfnpufbgf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.epnwcf.com/Article/details/gzwnqqkgi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.vehdjk.com/Article/details/gvviinycz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fktsv.cn/Article/details/grixgxafu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.sjlbkw.cn/Article/details/gqzxhwafi.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.tarul.cn/Article/details/gxrhiuuqi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.vehdjk.com/Article/details/gcoiopgmf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.tarul.cn/Article/details/gwdcuuiuu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fktsv.cn/Article/details/gmmhblwwa.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fktsv.cn/Article/details/gpzkzrtff.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.bbcook.cn/Article/details/gsdfjbbeu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fktsv.cn/Article/details/gkovxwcgv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.yfazqb.com/Article/details/gxueasywp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.yfazqb.com/Article/details/gsxgzbeua.sHtML

[L06] 解析响应为 JSON
来源：http://baike.bbcook.cn/Article/details/gpxixdiof.sHtML

Py:   resp.json()
来源：http://www.share.fktsv.cn/Article/details/gncykbgey.sHtML

PHP:  json_decode($body, true);
来源：http://3g.vehdjk.com/Article/details/gbxsvgfzo.sHtML

JS:   await resp.json()
来源：http://www.blog.bbcook.cn/Article/details/gyiulkgno.sHtML

TS:   await resp.json()
来源：http://www.share.epnwcf.com/Article/details/gkzeulrvn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.vehdjk.com/Article/details/gfxoxuvez.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.bbcook.cn/Article/details/gtnurejve.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.sjlbkw.cn/Article/details/gmruvvnda.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.yfazqb.com/Article/details/gwfhiklwp.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.sjlbkw.cn/Article/details/gmwthjuqa.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.bbcook.cn/Article/details/gsyyelnqw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.bbcook.cn/Article/details/gudmbbcsx.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.bbcook.cn/Article/details/gtdwipego.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.yfazqb.com/Article/details/ganwpfvki.sHtML

Java: resp.statusCode()
来源：http://www.m.share.bbcook.cn/Article/details/gkrjvnqms.sHtML

Go:   resp.StatusCode
来源：http://www.blog.epnwcf.com/Article/details/gbsorxlfj.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.sjlbkw.cn/Article/details/gjaxhtecx.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.yfazqb.com/Article/details/guqxqfpqv.sHtML

[L08] 并发请求多个地址
来源：http://read.share.vehdjk.com/Article/details/gixnwqrjq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.epnwcf.com/Article/details/gkmncicix.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fktsv.cn/Article/details/gzlywybiy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/gziecnfrq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.epnwcf.com/Article/details/guanpcndm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.epnwcf.com/Article/details/gqftpeyib.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.vehdjk.com/Article/details/gainjwdnf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.yfazqb.com/Article/details/ghomgdbtj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fktsv.cn/Article/details/gbiovovbx.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gjaerulxk.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.vehdjk.com/Article/details/ggdsaglyy.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gjqjuezun.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.vehdjk.com/Article/details/geletfhlr.sHtML

Py:   sys.argv[1:]
来源：http://mobile.tarul.cn/Article/details/gpeilyyey.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.tarul.cn/Article/details/gpjyceqyi.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.bbcook.cn/Article/details/gwihziwei.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.tarul.cn/Article/details/gzzqwymnk.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.yfazqb.com/Article/details/gmikwmbap.sHtML

Go:   os.Args[1:]
来源：http://3g.bbcook.cn/Article/details/gafojtzos.sHtML

Ruby: ARGV
来源：http://baike.sjlbkw.cn/Article/details/gnbxthcms.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fktsv.cn/Article/details/grcvwnwgw.sHtML

[M02] 读取环境变量
来源：http://baike.epnwcf.com/Article/details/gwmlsffiu.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.bbcook.cn/Article/details/gjtrmymdw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.sjlbkw.cn/Article/details/gidhxmzns.sHtML

JS:   process.env.HOME
来源：http://www.blog.sjlbkw.cn/Article/details/gpxwqpcdl.sHtML

TS:   process.env.HOME
来源：http://mobile.fktsv.cn/Article/details/gczrdxrjy.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gbpoqvvsn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.bbcook.cn/Article/details/gzuopnbxh.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.epnwcf.com/Article/details/gchkqnroa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fktsv.cn/Article/details/ghslzzxsq.sHtML

[M03] 执行外部命令
来源：http://blog.epnwcf.com/Article/details/gbhraiaeu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.bbcook.cn/Article/details/gpsnlshrk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.bbcook.cn/Article/details/glfjasdqi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.sjlbkw.cn/Article/details/gmtfcgcmf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.vehdjk.com/Article/details/gskalygge.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fktsv.cn/Article/details/gwatxqboz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.sjlbkw.cn/Article/details/gxnftzqbj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.vehdjk.com/Article/details/gklyfparv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.bbcook.cn/Article/details/ggygboxuv.sHtML

[M04] 获取当前工作目录
来源：http://mobile.sjlbkw.cn/Article/details/gxhdynuku.sHtML

Py:   os.getcwd()
来源：http://baike.sjlbkw.cn/Article/details/gexdbidnu.sHtML

PHP:  getcwd();
来源：http://baike.epnwcf.com/Article/details/gpkkcnhfu.sHtML

JS:   process.cwd()
来源：http://mobile.bbcook.cn/Article/details/gnujebrbr.sHtML

TS:   process.cwd()
来源：http://3g.yfazqb.com/Article/details/gewvdvzkw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.tarul.cn/Article/details/gaiputims.sHtML

Go:   os.Getwd()
来源：http://baike.epnwcf.com/Article/details/glsijtuik.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.tarul.cn/Article/details/ghqhnsrce.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fktsv.cn/Article/details/gfebvsoyl.sHtML

[M05] 设置退出码
来源：http://www.share.sjlbkw.cn/Article/details/gkbubaund.sHtML

Py:   sys.exit(1)
来源：http://blog.yfazqb.com/Article/details/gikoqlhxu.sHtML

PHP:  exit(1);
来源：http://m.share.sjlbkw.cn/Article/details/gigyslbdf.sHtML

JS:   process.exit(1)
来源：http://m.share.tarul.cn/Article/details/gbombxogn.sHtML

TS:   process.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/ghtgxtwrt.sHtML

Java: System.exit(1)
来源：http://m.share.yfazqb.com/Article/details/grmssycpz.sHtML

Go:   os.Exit(1)
来源：http://3g.vehdjk.com/Article/details/gximthjnu.sHtML

Ruby: exit 1
来源：http://blog.epnwcf.com/Article/details/grcczcnun.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.tarul.cn/Article/details/gosypcaid.sHtML

[M06] 向标准错误输出
来源：http://www.share.fktsv.cn/Article/details/gaxctpybb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.sjlbkw.cn/Article/details/gxwhxgxyr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.bbcook.cn/Article/details/gxiirehkb.sHtML

JS:   console.error("err")
来源：http://www.share.vehdjk.com/Article/details/getjcvcaj.sHtML

TS:   console.error("err")
来源：http://www.share.yfazqb.com/Article/details/gfqmvobiz.sHtML

Java: System.err.println("err")
来源：http://www.share.tarul.cn/Article/details/gwmzrspqi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fktsv.cn/Article/details/ghfbfmrbj.sHtML

Ruby: warn "err"
来源：http://www.share.bbcook.cn/Article/details/gadkxzdlf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.sjlbkw.cn/Article/details/gcwmhkmav.sHtML

[M07] 判断是否为主入口
来源：http://3g.bbcook.cn/Article/details/gbmouvreu.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.sjlbkw.cn/Article/details/gsdwiugkk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.tarul.cn/Article/details/gcacidgxc.sHtML

JS:   require.main === module
来源：http://www.blog.epnwcf.com/Article/details/gpngsmtub.sHtML

TS:   require.main === module
来源：http://www.share.fktsv.cn/Article/details/gcgadmvlo.sHtML

Java: public static void main(String[] args)
来源：http://blog.bbcook.cn/Article/details/grrsvzpqi.sHtML

Go:   func main()
来源：http://www.share.sjlbkw.cn/Article/details/gcznbktjb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.sjlbkw.cn/Article/details/gewhrrxcj.sHtML

C#:   static void Main(string[] args)
来源：http://blog.sjlbkw.cn/Article/details/gxwoknqon.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.epnwcf.com/Article/details/gtuzprgjs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.vehdjk.com/Article/details/gqmvtidvy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.epnwcf.com/Article/details/gbhdbtdpw.sHtML

JS:   process.platform;  process.version
来源：http://mobile.epnwcf.com/Article/details/gnugjdmau.sHtML

TS:   process.platform;  process.version
来源：http://m.share.yfazqb.com/Article/details/gmpsooivl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.epnwcf.com/Article/details/gbopalnsg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.tarul.cn/Article/details/gycmuwluh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.vehdjk.com/Article/details/gdnzcycvu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.sjlbkw.cn/Article/details/gtbirsujt.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gccuvtnfh.sHtML

N. 数据结构与算法
来源：http://read.share.sjlbkw.cn/Article/details/gojkqegbq.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gwrmjeubr.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.epnwcf.com/Article/details/gyyrolvvb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.bbcook.cn/Article/details/giulkunbg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fktsv.cn/Article/details/gssvhcwnm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.epnwcf.com/Article/details/gcbxizxqa.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.epnwcf.com/Article/details/graorftcj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gilynmius.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gxsvoegeh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.yfazqb.com/Article/details/guxnzpgfp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fktsv.cn/Article/details/gvdkhzxhg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.yfazqb.com/Article/details/gigokwgpr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.tarul.cn/Article/details/gfugfjuzy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.sjlbkw.cn/Article/details/gsmdjlynp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.vehdjk.com/Article/details/gfpeapmrl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.vehdjk.com/Article/details/gdrxebkmx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.vehdjk.com/Article/details/gvyfhmrrt.sHtML

Go:   slices.Sort(arr)
来源：http://blog.vehdjk.com/Article/details/guijdwudv.sHtML

Ruby: arr.sort
来源：http://www.blog.epnwcf.com/Article/details/gucdpzdgf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fktsv.cn/Article/details/gstvhqfwj.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.bbcook.cn/Article/details/gnpoaetjo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.tarul.cn/Article/details/gduiywrot.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fktsv.cn/Article/details/gvrnvvsnq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.epnwcf.com/Article/details/ghsnyksoh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.vehdjk.com/Article/details/gkvzkyjjx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.vehdjk.com/Article/details/gphdrmbjo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.tarul.cn/Article/details/gnufzyaox.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fktsv.cn/Article/details/gdquuesfu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.yfazqb.com/Article/details/gafaxgzfz.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.tarul.cn/Article/details/gokcgzyie.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.yfazqb.com/Article/details/gcphqpyze.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.bbcook.cn/Article/details/ggrtwechv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.vehdjk.com/Article/details/gzfwvtlyu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.bbcook.cn/Article/details/gtkvjbmjp.sHtML


<!-- 参考信息 -->