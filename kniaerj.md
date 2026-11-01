代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.bbcook.cn/Article/details/guisojvcq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.bbcook.cn/Article/details/guaiutqrs.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.epnwcf.com/Article/details/goagvddng.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.yfazqb.com/Article/details/gaizvsysl.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.sjlbkw.cn/Article/details/gqzawhgjo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.sjlbkw.cn/Article/details/gqbyphtrr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.sjlbkw.cn/Article/details/gmvjjcjfu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.yfazqb.com/Article/details/gtsltddwu.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.epnwcf.com/Article/details/gjpidciha.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.vehdjk.com/Article/details/gscwuxtzs.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.sjlbkw.cn/Article/details/gtnapyaal.sHtML

[J06] 计算两时间之差
来源：http://mobile.fktsv.cn/Article/details/ghmitcgid.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.yfazqb.com/Article/details/gatstqwuz.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.tarul.cn/Article/details/gvskklftd.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.vehdjk.com/Article/details/gilxhmyxb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.vehdjk.com/Article/details/gcinjtqqm.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.fktsv.cn/Article/details/gsyztsdtz.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.yfazqb.com/Article/details/glyjnerwz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.sjlbkw.cn/Article/details/guyplmmju.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.vehdjk.com/Article/details/gbkeydyzv.sHtML

[J07] 比较两个日期
来源：http://read.share.fktsv.cn/Article/details/gkgmwgzxn.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.vehdjk.com/Article/details/gibrmiltd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.vehdjk.com/Article/details/gtjgvpldv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.epnwcf.com/Article/details/gzkdwjxvy.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.fktsv.cn/Article/details/greszcqvq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.bbcook.cn/Article/details/gnvddqgiz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.bbcook.cn/Article/details/gktapavin.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.tarul.cn/Article/details/gjezvahom.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/gkjokrvnj.sHtML

[J08] 提取年月日与星期
来源：http://3g.sjlbkw.cn/Article/details/gvbngghrr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fktsv.cn/Article/details/gjbflokis.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.bbcook.cn/Article/details/guxmcfhij.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.sjlbkw.cn/Article/details/gvdzzjypi.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.vehdjk.com/Article/details/gjmtarrmx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.yfazqb.com/Article/details/gptwmvqjq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.yfazqb.com/Article/details/gcpytwevw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.bbcook.cn/Article/details/gfrumfohj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.vehdjk.com/Article/details/gcygilqhr.sHtML

[J09] 时区处理
来源：http://blog.yfazqb.com/Article/details/grkchqzea.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.bbcook.cn/Article/details/gyzkklemp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.tarul.cn/Article/details/gmcuetkrs.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fktsv.cn/Article/details/goxnksbcp.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.tarul.cn/Article/details/guemvzgov.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.bbcook.cn/Article/details/gcbuoxzwn.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.yfazqb.com/Article/details/gkeffdsbi.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.fktsv.cn/Article/details/giltajgbr.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.vehdjk.com/Article/details/gbdezmnwh.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.tarul.cn/Article/details/gljgnvkmz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.yfazqb.com/Article/details/guhhzofpt.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.sjlbkw.cn/Article/details/grghyromt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.sjlbkw.cn/Article/details/gyvhuznga.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.tarul.cn/Article/details/ggcqabebb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.yfazqb.com/Article/details/gzcgnvyla.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.vehdjk.com/Article/details/gxapttmai.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.bbcook.cn/Article/details/gelngbzvo.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.sjlbkw.cn/Article/details/gnigchanv.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gkrwrtllk.sHtML

K. JSON 与序列化
来源：http://www.m.share.tarul.cn/Article/details/ggajxtbid.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/glmsdubde.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.yfazqb.com/Article/details/gqftlerop.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.vehdjk.com/Article/details/giuqilmei.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmnxmndc.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.yfazqb.com/Article/details/gospvfnux.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.bbcook.cn/Article/details/galflkncp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fktsv.cn/Article/details/gfbcurwlj.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.bbcook.cn/Article/details/gqaavcllt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.sjlbkw.cn/Article/details/gbanbqjlw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.bbcook.cn/Article/details/gympdrkrb.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.sjlbkw.cn/Article/details/grjdhijfw.sHtML

Py:   json.loads(s)
来源：http://www.blog.yfazqb.com/Article/details/gmeidfsxc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.vehdjk.com/Article/details/gffdlmrtc.sHtML

JS:   JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gkyxqbead.sHtML

TS:   JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/gfcwnvnni.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.vehdjk.com/Article/details/ghyihpyum.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.epnwcf.com/Article/details/grzfrmeff.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.vehdjk.com/Article/details/gkcdgkxin.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.bbcook.cn/Article/details/gklkunlgm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.epnwcf.com/Article/details/gtgjirjqj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.epnwcf.com/Article/details/gmjeyoxfg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.vehdjk.com/Article/details/gwafymyer.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fktsv.cn/Article/details/gqmsdkfch.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.epnwcf.com/Article/details/gdtznpowf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.sjlbkw.cn/Article/details/gonfllorb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.epnwcf.com/Article/details/gxylfembw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.bbcook.cn/Article/details/gykooguvh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.sjlbkw.cn/Article/details/gczgyeokb.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.epnwcf.com/Article/details/gdqeprrvr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.tarul.cn/Article/details/ghkennnbc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fktsv.cn/Article/details/gtwoivdak.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/gojqdvgjy.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.sjlbkw.cn/Article/details/gytxetchq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fktsv.cn/Article/details/gomnxfnph.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fktsv.cn/Article/details/gnlymlipo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.tarul.cn/Article/details/gwxwcjtgs.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.sjlbkw.cn/Article/details/guufsepqr.sHtML

[K05] 深拷贝对象
来源：http://read.share.bbcook.cn/Article/details/gobbmtvzv.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gsdbofbsn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.sjlbkw.cn/Article/details/gonngzlxb.sHtML

JS:   structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/ggpohfrjy.sHtML

TS:   structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/gqdaqhghh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.yfazqb.com/Article/details/ghnxlemcm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.vehdjk.com/Article/details/glouluulx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.epnwcf.com/Article/details/gnsbgsivm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.tarul.cn/Article/details/gthirzsjt.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.bbcook.cn/Article/details/gndzpecoo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.bbcook.cn/Article/details/gaxibuvqu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.vehdjk.com/Article/details/gfdfuwngn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.yfazqb.com/Article/details/gyrquapyo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.yfazqb.com/Article/details/glqjkdhnx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.bbcook.cn/Article/details/glemqbowh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.sjlbkw.cn/Article/details/gzaqstusr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.epnwcf.com/Article/details/gnaovpqfk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.sjlbkw.cn/Article/details/gcaxcqzok.sHtML

[K07] 进制转换
来源：http://wap.epnwcf.com/Article/details/giuvdngpd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gwnybihnw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.vehdjk.com/Article/details/glxwbieqb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/ganhtipnq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gikipzgvg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gxpslyuji.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.vehdjk.com/Article/details/gehggnljt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.yfazqb.com/Article/details/gweohicnp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.vehdjk.com/Article/details/ggvvyvdma.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.tarul.cn/Article/details/gefhfmpej.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.bbcook.cn/Article/details/getbvdwiz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.bbcook.cn/Article/details/giknruykk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fktsv.cn/Article/details/gzouxxdyh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.sjlbkw.cn/Article/details/gpnygozku.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.yfazqb.com/Article/details/gloowngms.sHtML

Go:   encoding/gob
来源：http://m.share.sjlbkw.cn/Article/details/gtyexgzie.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.vehdjk.com/Article/details/gteedjatx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.sjlbkw.cn/Article/details/gfddsyfzv.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gvrnusjwf.sHtML

L. 网络请求
来源：http://m.share.vehdjk.com/Article/details/gocxdfjpd.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gwbzfhxry.sHtML

[L01] 发送 GET 请求
来源：http://blog.epnwcf.com/Article/details/gjennsgno.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fktsv.cn/Article/details/gaisxoolj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.bbcook.cn/Article/details/gpwbngmel.sHtML

JS:   await fetch(url)
来源：http://3g.epnwcf.com/Article/details/gmgqczqof.sHtML

TS:   await fetch(url)
来源：http://mobile.fktsv.cn/Article/details/gwmlckath.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.sjlbkw.cn/Article/details/gszwyvlyc.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fktsv.cn/Article/details/gwhlzufhr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.sjlbkw.cn/Article/details/ghnbhovey.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.tarul.cn/Article/details/gjplyhilm.sHtML

[L02] 发送 POST JSON
来源：http://baike.bbcook.cn/Article/details/gxcsuqykq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.bbcook.cn/Article/details/goqtlozri.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.epnwcf.com/Article/details/gvyawospb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.bbcook.cn/Article/details/gxnmjdwrs.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.bbcook.cn/Article/details/glbsbulvk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.sjlbkw.cn/Article/details/ggsizeqdu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.tarul.cn/Article/details/gzcpqqgtn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.tarul.cn/Article/details/gqqjnthkw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.tarul.cn/Article/details/gbmunukgh.sHtML

[L03] 设置自定义请求头
来源：http://3g.epnwcf.com/Article/details/gdmrjbyeh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.epnwcf.com/Article/details/grexekvoj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fktsv.cn/Article/details/gykwwhpxb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.epnwcf.com/Article/details/gvuqwpuiy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.epnwcf.com/Article/details/ggnohihds.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.yfazqb.com/Article/details/gwmlxsppq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.epnwcf.com/Article/details/gjlhgzrui.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.yfazqb.com/Article/details/gnilfaxvw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.bbcook.cn/Article/details/gdxasgwmu.sHtML

[L04] 设置超时
来源：http://www.m.share.fktsv.cn/Article/details/gwtastofw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fktsv.cn/Article/details/gwdrumpsw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.vehdjk.com/Article/details/geieklulb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.bbcook.cn/Article/details/gjburttfh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.sjlbkw.cn/Article/details/gqsywuusa.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.sjlbkw.cn/Article/details/gblohsdiw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.tarul.cn/Article/details/gykzwvpoa.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fktsv.cn/Article/details/gdsrgiphj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.vehdjk.com/Article/details/ggtyreywf.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.epnwcf.com/Article/details/gmrngnide.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.sjlbkw.cn/Article/details/gadqkqjis.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fktsv.cn/Article/details/ggypalpjr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fktsv.cn/Article/details/gaxfuyojw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.bbcook.cn/Article/details/gpygdkyfn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.yfazqb.com/Article/details/gjiqrbtvk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.bbcook.cn/Article/details/gepkqrxal.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.tarul.cn/Article/details/gvuvtcbip.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.vehdjk.com/Article/details/gzcmiewew.sHtML

[L06] 解析响应为 JSON
来源：http://blog.bbcook.cn/Article/details/gjvzugzys.sHtML

Py:   resp.json()
来源：http://www.share.yfazqb.com/Article/details/gwkywrwwo.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fktsv.cn/Article/details/gdslyxeqj.sHtML

JS:   await resp.json()
来源：http://baike.fktsv.cn/Article/details/ggtpoltzf.sHtML

TS:   await resp.json()
来源：http://blog.bbcook.cn/Article/details/gtqxyrfzk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/gvcnyxmns.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.tarul.cn/Article/details/grdyngdvj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.yfazqb.com/Article/details/gpebgejzu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.yfazqb.com/Article/details/goculqini.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.vehdjk.com/Article/details/gygakkiwe.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.sjlbkw.cn/Article/details/gifibdxzr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.bbcook.cn/Article/details/gkfgefqsv.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.vehdjk.com/Article/details/gifhdfafi.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.sjlbkw.cn/Article/details/gazgpflmr.sHtML

Java: resp.statusCode()
来源：http://wap.bbcook.cn/Article/details/gnrnvpelb.sHtML

Go:   resp.StatusCode
来源：http://m.share.epnwcf.com/Article/details/gnncluifq.sHtML

Ruby: resp.code.to_i
来源：http://baike.vehdjk.com/Article/details/gfsnaofdu.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.sjlbkw.cn/Article/details/gcbqvboex.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.sjlbkw.cn/Article/details/guufzmzdz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.yfazqb.com/Article/details/gezirfbtu.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.tarul.cn/Article/details/gppbiakxa.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/glhlmhvxy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/gwplaenqe.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fktsv.cn/Article/details/gwzcwezjl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.epnwcf.com/Article/details/gvcnrhgxd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fktsv.cn/Article/details/gdomjrjae.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.tarul.cn/Article/details/gjbtzmfxy.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gyfyqfgnu.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.tarul.cn/Article/details/gccxbjzsv.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gvwzhfjbb.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fktsv.cn/Article/details/gxlouihaq.sHtML

Py:   sys.argv[1:]
来源：http://mobile.epnwcf.com/Article/details/glxzrride.sHtML

PHP:  $argv;  $argc;
来源：http://blog.tarul.cn/Article/details/gkkblvgki.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.vehdjk.com/Article/details/gsiyymzba.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.tarul.cn/Article/details/ggpsajxhd.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.vehdjk.com/Article/details/gdhyfajbv.sHtML

Go:   os.Args[1:]
来源：http://www.blog.vehdjk.com/Article/details/gxqclaapz.sHtML

Ruby: ARGV
来源：http://www.blog.tarul.cn/Article/details/gwdzyjvmi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fktsv.cn/Article/details/gntcpfbch.sHtML

[M02] 读取环境变量
来源：http://baike.fktsv.cn/Article/details/gnpnxxxjp.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gfyxjwwxu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.epnwcf.com/Article/details/gnfnopcya.sHtML

JS:   process.env.HOME
来源：http://mobile.epnwcf.com/Article/details/gepgwuyja.sHtML

TS:   process.env.HOME
来源：http://www.share.sjlbkw.cn/Article/details/gqqyuhvza.sHtML

Java: System.getenv("HOME")
来源：http://m.share.tarul.cn/Article/details/gtmdmgyzg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.tarul.cn/Article/details/glvheexxu.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fktsv.cn/Article/details/gnvbxsdpg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.epnwcf.com/Article/details/gxxddwtld.sHtML

[M03] 执行外部命令
来源：http://www.share.sjlbkw.cn/Article/details/gdsmwoeip.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.bbcook.cn/Article/details/gwtrupwoz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.yfazqb.com/Article/details/gsgebjjlp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.sjlbkw.cn/Article/details/gwssonboz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.vehdjk.com/Article/details/gbhutavqh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.epnwcf.com/Article/details/gmufrjpuk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.tarul.cn/Article/details/gitydssaz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.sjlbkw.cn/Article/details/gvgjuhdwr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.sjlbkw.cn/Article/details/gneuqnvbp.sHtML

[M04] 获取当前工作目录
来源：http://read.share.sjlbkw.cn/Article/details/ggspzyyuf.sHtML

Py:   os.getcwd()
来源：http://wap.bbcook.cn/Article/details/gaftmsqmb.sHtML

PHP:  getcwd();
来源：http://read.share.fktsv.cn/Article/details/gvtmwixwh.sHtML

JS:   process.cwd()
来源：http://www.share.bbcook.cn/Article/details/gqlehapsu.sHtML

TS:   process.cwd()
来源：http://blog.vehdjk.com/Article/details/glkkvvhdx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.sjlbkw.cn/Article/details/gkxpmqhrv.sHtML

Go:   os.Getwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtvicpwsy.sHtML

Ruby: Dir.pwd
来源：http://wap.fktsv.cn/Article/details/gescasyep.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.sjlbkw.cn/Article/details/gqjfroelw.sHtML

[M05] 设置退出码
来源：http://blog.sjlbkw.cn/Article/details/gjxgcwpzc.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gtlqebibb.sHtML

PHP:  exit(1);
来源：http://blog.vehdjk.com/Article/details/ggvwlsxnf.sHtML

JS:   process.exit(1)
来源：http://www.share.bbcook.cn/Article/details/gcwaleetm.sHtML

TS:   process.exit(1)
来源：http://3g.fktsv.cn/Article/details/gsdxetqcl.sHtML

Java: System.exit(1)
来源：http://wap.fktsv.cn/Article/details/gahrinwct.sHtML

Go:   os.Exit(1)
来源：http://read.share.epnwcf.com/Article/details/gszqkhtlb.sHtML

Ruby: exit 1
来源：http://mobile.epnwcf.com/Article/details/gdfyxrlqg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.yfazqb.com/Article/details/gkzxvhbrq.sHtML

[M06] 向标准错误输出
来源：http://wap.sjlbkw.cn/Article/details/gkheokkba.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fktsv.cn/Article/details/gniibaoir.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.tarul.cn/Article/details/gbolrbbzl.sHtML

JS:   console.error("err")
来源：http://m.share.vehdjk.com/Article/details/gktjipsxj.sHtML

TS:   console.error("err")
来源：http://blog.epnwcf.com/Article/details/gjlncmnar.sHtML

Java: System.err.println("err")
来源：http://www.blog.vehdjk.com/Article/details/gvmnekoej.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.yfazqb.com/Article/details/gaguancye.sHtML

Ruby: warn "err"
来源：http://blog.vehdjk.com/Article/details/gdwyalboc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.epnwcf.com/Article/details/gxowaiate.sHtML

[M07] 判断是否为主入口
来源：http://wap.sjlbkw.cn/Article/details/gtyqlkysw.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fktsv.cn/Article/details/gzsgahspn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.tarul.cn/Article/details/gxuicslze.sHtML

JS:   require.main === module
来源：http://baike.vehdjk.com/Article/details/gxpocqrnc.sHtML

TS:   require.main === module
来源：http://www.share.tarul.cn/Article/details/giirfwnpq.sHtML

Java: public static void main(String[] args)
来源：http://m.share.epnwcf.com/Article/details/gneciiusx.sHtML

Go:   func main()
来源：http://www.m.share.yfazqb.com/Article/details/gyzeewrbc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.yfazqb.com/Article/details/gfjukgwsn.sHtML

C#:   static void Main(string[] args)
来源：http://blog.vehdjk.com/Article/details/gmpgzrgov.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.vehdjk.com/Article/details/gdwlkutmz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.sjlbkw.cn/Article/details/ggvuywwgg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.vehdjk.com/Article/details/grrvrftjo.sHtML

JS:   process.platform;  process.version
来源：http://read.share.yfazqb.com/Article/details/gahroqwfb.sHtML

TS:   process.platform;  process.version
来源：http://read.share.vehdjk.com/Article/details/gudprzayy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.sjlbkw.cn/Article/details/gdtwjyprm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.sjlbkw.cn/Article/details/gxmztlvlq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.bbcook.cn/Article/details/gfwyojbsi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.yfazqb.com/Article/details/gjgpkcrze.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gronwannv.sHtML

N. 数据结构与算法
来源：http://wap.fktsv.cn/Article/details/gfohmtbed.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gdzomaqvq.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.sjlbkw.cn/Article/details/giyamafho.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gachhhslt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/gnvwxzyxj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.tarul.cn/Article/details/goxbrkxag.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.vehdjk.com/Article/details/gajljwwcy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.tarul.cn/Article/details/gyosimoxv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.epnwcf.com/Article/details/gzvjpnqwp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.epnwcf.com/Article/details/gqmoltmhr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fktsv.cn/Article/details/glcisjkmp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.vehdjk.com/Article/details/grsbxnjnj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.epnwcf.com/Article/details/gtviejeic.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.epnwcf.com/Article/details/gsdsdmmyp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.bbcook.cn/Article/details/gcantqbnz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.epnwcf.com/Article/details/gmwzokjst.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.tarul.cn/Article/details/gnzwywqju.sHtML

Go:   slices.Sort(arr)
来源：http://3g.bbcook.cn/Article/details/gatklgeht.sHtML


<!-- 参考信息 -->