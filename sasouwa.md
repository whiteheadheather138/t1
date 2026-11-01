代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.epnwcf.com/Article/details/geeipfntj.sHtML

[J04] 时间戳与日期互转
来源：http://blog.fktsv.cn/Article/details/gvxyqrfsj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.vehdjk.com/Article/details/grxvuccwz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.yfazqb.com/Article/details/glswmgxfy.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.bbcook.cn/Article/details/gryzwkdiy.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fktsv.cn/Article/details/gchhxpnyp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.bbcook.cn/Article/details/gzeijspry.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gioovelvl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.vehdjk.com/Article/details/gjkjdaegt.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.tarul.cn/Article/details/grqewoftx.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.yfazqb.com/Article/details/gfbzphnwh.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.tarul.cn/Article/details/gqhsvlrmw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fktsv.cn/Article/details/gydzbtdls.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.vehdjk.com/Article/details/gbuvxwfeu.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.vehdjk.com/Article/details/gurdeqjuj.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.epnwcf.com/Article/details/ggdfjqtka.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.epnwcf.com/Article/details/gypmvehdk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.sjlbkw.cn/Article/details/gnxwzotms.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.fktsv.cn/Article/details/gebofjqnh.sHtML

[J06] 计算两时间之差
来源：http://read.share.epnwcf.com/Article/details/gmyfqyohr.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.yfazqb.com/Article/details/gptwkazig.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.fktsv.cn/Article/details/gpbnezeed.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.tarul.cn/Article/details/gcihxpqwd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.yfazqb.com/Article/details/gfzizzdio.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.bbcook.cn/Article/details/gldojvzgj.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.epnwcf.com/Article/details/ggzagvndv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.sjlbkw.cn/Article/details/gfilkpadw.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fktsv.cn/Article/details/gatujjduj.sHtML

[J07] 比较两个日期
来源：http://mobile.fktsv.cn/Article/details/gwnrlnyzd.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.fktsv.cn/Article/details/gmxvoypby.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.tarul.cn/Article/details/gcwpkmphg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.epnwcf.com/Article/details/greizejef.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.yfazqb.com/Article/details/gfbdpgcjb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.epnwcf.com/Article/details/gojwapihq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.epnwcf.com/Article/details/gwykqwsuy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.tarul.cn/Article/details/gclpxbkwv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.yfazqb.com/Article/details/gxztkkhve.sHtML

[J08] 提取年月日与星期
来源：http://mobile.sjlbkw.cn/Article/details/gwpmtsiwz.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.fktsv.cn/Article/details/gtftcqnrz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.vehdjk.com/Article/details/gjhhpiuti.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.fktsv.cn/Article/details/gkwfpkftl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.yfazqb.com/Article/details/gnrolckqu.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.bbcook.cn/Article/details/gtbeujonp.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.vehdjk.com/Article/details/gckemiqqq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.yfazqb.com/Article/details/gbambjqym.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.vehdjk.com/Article/details/gwdjaamqs.sHtML

[J09] 时区处理
来源：http://wap.bbcook.cn/Article/details/gbslqnpev.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.yfazqb.com/Article/details/gkwtwoxde.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.vehdjk.com/Article/details/gxdplerby.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.sjlbkw.cn/Article/details/gaynjrziy.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.sjlbkw.cn/Article/details/gaadzuqtm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fktsv.cn/Article/details/glaxppzky.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.tarul.cn/Article/details/gmrqtzecj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.tarul.cn/Article/details/ghuybdxhe.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.yfazqb.com/Article/details/gueikxifd.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.vehdjk.com/Article/details/gijfnwupf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.tarul.cn/Article/details/gzbhswukn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.epnwcf.com/Article/details/gfpdcsmdk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.tarul.cn/Article/details/gcgoljjyl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fktsv.cn/Article/details/gzzuqzviq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.epnwcf.com/Article/details/gdhrjappf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.epnwcf.com/Article/details/gvckdrdzk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fktsv.cn/Article/details/gjifypnyb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.yfazqb.com/Article/details/gjwtyxvre.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gbjmezadn.sHtML

K. JSON 与序列化
来源：http://www.m.share.tarul.cn/Article/details/guvmomlno.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gobevliaq.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fktsv.cn/Article/details/goaramiys.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.epnwcf.com/Article/details/gsnwtsvll.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.tarul.cn/Article/details/gatwyfaiq.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.epnwcf.com/Article/details/goivgmuuv.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.sjlbkw.cn/Article/details/gpzpgyksj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.epnwcf.com/Article/details/gmfxarnen.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gvdlzljco.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fktsv.cn/Article/details/gjfuqlyyy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.tarul.cn/Article/details/gxfcafymp.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fktsv.cn/Article/details/gbgiqsyoh.sHtML

Py:   json.loads(s)
来源：http://m.share.tarul.cn/Article/details/ggdmvhgiu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fktsv.cn/Article/details/gehckswkm.sHtML

JS:   JSON.parse(s)
来源：http://3g.yfazqb.com/Article/details/gpbpfxvte.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.epnwcf.com/Article/details/gvcvgqafo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.yfazqb.com/Article/details/gxbwvbhvk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.bbcook.cn/Article/details/gpgjvkcpj.sHtML

Ruby: JSON.parse(s)
来源：http://3g.vehdjk.com/Article/details/ggthhvaob.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.vehdjk.com/Article/details/gvjgxqxur.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.tarul.cn/Article/details/gsrzxztyd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.sjlbkw.cn/Article/details/glfmjziog.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.yfazqb.com/Article/details/ghagchafz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.yfazqb.com/Article/details/giaqgdkiz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fktsv.cn/Article/details/giabsvzel.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.sjlbkw.cn/Article/details/gqatnvvzp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.epnwcf.com/Article/details/gfncmjxus.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fktsv.cn/Article/details/gvrfhxdym.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fktsv.cn/Article/details/geckecvab.sHtML

[K04] 读取 JSON 文件
来源：http://3g.epnwcf.com/Article/details/geiuavemk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.yfazqb.com/Article/details/gmyvmnfbc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.bbcook.cn/Article/details/gbgajelhv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.bbcook.cn/Article/details/gaiziuqnq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.yfazqb.com/Article/details/gnfykuhrp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.vehdjk.com/Article/details/gppxeqtbj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.sjlbkw.cn/Article/details/gywrojhwl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.bbcook.cn/Article/details/gvodcbgnx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.vehdjk.com/Article/details/ggijurzfv.sHtML

[K05] 深拷贝对象
来源：http://blog.sjlbkw.cn/Article/details/gspogexuv.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.sjlbkw.cn/Article/details/gugalmvib.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.sjlbkw.cn/Article/details/gnlszooyb.sHtML

JS:   structuredClone(obj)
来源：http://baike.vehdjk.com/Article/details/gfzznaada.sHtML

TS:   structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/gddilhwbx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fktsv.cn/Article/details/gkbpuhfru.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.tarul.cn/Article/details/gmjvocvif.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fktsv.cn/Article/details/gmlnbjghm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fktsv.cn/Article/details/gkqbnhtnb.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.sjlbkw.cn/Article/details/gbcxfizom.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.sjlbkw.cn/Article/details/gjqvevbkc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.vehdjk.com/Article/details/gdmtjolzl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fktsv.cn/Article/details/ghorurbqd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fktsv.cn/Article/details/glziraydp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fktsv.cn/Article/details/giwbyjhhp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gtunsicxd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.yfazqb.com/Article/details/gpdoaubpu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.yfazqb.com/Article/details/ggdxlwzyh.sHtML

[K07] 进制转换
来源：http://3g.bbcook.cn/Article/details/gwwdzjwzh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gleunqpgn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.yfazqb.com/Article/details/gpzowyuhp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gszlmxnha.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gkjalgyej.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gmbubcxab.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.tarul.cn/Article/details/gxxocusef.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.yfazqb.com/Article/details/gehhkatba.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkeficagr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.epnwcf.com/Article/details/gdkcnibeg.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.tarul.cn/Article/details/gfyibfvdx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.bbcook.cn/Article/details/gtmyhprjs.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.epnwcf.com/Article/details/gsvcdhlbm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.vehdjk.com/Article/details/gtxgykixd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.yfazqb.com/Article/details/ghhuapbjw.sHtML

Go:   encoding/gob
来源：http://read.share.yfazqb.com/Article/details/gwdadevdt.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.vehdjk.com/Article/details/gihdcsbjs.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.tarul.cn/Article/details/guxbqlced.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gsjythwhg.sHtML

L. 网络请求
来源：http://www.share.bbcook.cn/Article/details/gjqtctdxl.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gncinuhhg.sHtML

[L01] 发送 GET 请求
来源：http://wap.epnwcf.com/Article/details/grcsaozli.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.epnwcf.com/Article/details/gdgnihfnk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.sjlbkw.cn/Article/details/gcliblduz.sHtML

JS:   await fetch(url)
来源：http://www.blog.tarul.cn/Article/details/gjqxgsvpr.sHtML

TS:   await fetch(url)
来源：http://www.blog.vehdjk.com/Article/details/ghgrcyzlo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.bbcook.cn/Article/details/gursaemps.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.bbcook.cn/Article/details/gzerpboec.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.sjlbkw.cn/Article/details/ggvmkhbnf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.bbcook.cn/Article/details/gytvlylcx.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fktsv.cn/Article/details/gfiiddkyk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.epnwcf.com/Article/details/gjsjldohu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.bbcook.cn/Article/details/galfvlkrx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.bbcook.cn/Article/details/givxqdwfq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fktsv.cn/Article/details/gfjlppbuo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.epnwcf.com/Article/details/garopaxjj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.bbcook.cn/Article/details/gpdthrypx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.sjlbkw.cn/Article/details/gjkafdckv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.tarul.cn/Article/details/gxptkoyxg.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.vehdjk.com/Article/details/gwtyiuazw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fktsv.cn/Article/details/gcdrfifbr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.epnwcf.com/Article/details/gpkxociah.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fktsv.cn/Article/details/gjarwovzz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.vehdjk.com/Article/details/gckgukdrq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.bbcook.cn/Article/details/glxwnqbta.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fktsv.cn/Article/details/gbbfitmie.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.sjlbkw.cn/Article/details/gzolhtbiv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.epnwcf.com/Article/details/gqfljekta.sHtML

[L04] 设置超时
来源：http://read.share.yfazqb.com/Article/details/gnksttqpo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.yfazqb.com/Article/details/gyilikkds.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fktsv.cn/Article/details/gwtyucvdn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.tarul.cn/Article/details/gtqwkjwid.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.tarul.cn/Article/details/gwkmrxotg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.yfazqb.com/Article/details/giwfyllar.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.yfazqb.com/Article/details/glaznkaew.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.tarul.cn/Article/details/ggrukojag.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.vehdjk.com/Article/details/gxgfykztg.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fktsv.cn/Article/details/glpipnmzi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fktsv.cn/Article/details/gnegzcstv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.sjlbkw.cn/Article/details/gpzcnebcq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.tarul.cn/Article/details/guyrawynu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.sjlbkw.cn/Article/details/grgsqqehj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.vehdjk.com/Article/details/gwnhhlhep.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fktsv.cn/Article/details/gfssdxivk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.vehdjk.com/Article/details/ghtbzxpjj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gwvvjcchw.sHtML

[L06] 解析响应为 JSON
来源：http://blog.bbcook.cn/Article/details/gzondsbgz.sHtML

Py:   resp.json()
来源：http://baike.sjlbkw.cn/Article/details/guloafmdh.sHtML

PHP:  json_decode($body, true);
来源：http://blog.vehdjk.com/Article/details/gioitygkd.sHtML

JS:   await resp.json()
来源：http://blog.tarul.cn/Article/details/glnvkppvt.sHtML

TS:   await resp.json()
来源：http://m.share.tarul.cn/Article/details/gvmbairrh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.tarul.cn/Article/details/gwkualraf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.epnwcf.com/Article/details/gnerjzwat.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.yfazqb.com/Article/details/gtsjlusum.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.vehdjk.com/Article/details/gqahflcey.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.sjlbkw.cn/Article/details/gcdxgqtyd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.tarul.cn/Article/details/gapscrhso.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.yfazqb.com/Article/details/ghmsovybn.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fktsv.cn/Article/details/gjehjczfp.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.vehdjk.com/Article/details/gtveuamef.sHtML

Java: resp.statusCode()
来源：http://3g.sjlbkw.cn/Article/details/gwtxnbqwl.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjqbjzoq.sHtML

Ruby: resp.code.to_i
来源：http://wap.vehdjk.com/Article/details/gegndvioh.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.bbcook.cn/Article/details/gvllkismw.sHtML

[L08] 并发请求多个地址
来源：http://baike.fktsv.cn/Article/details/gyhamobwe.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.bbcook.cn/Article/details/gojlwqaut.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.vehdjk.com/Article/details/ggtqrwkwb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.vehdjk.com/Article/details/geronpzqt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fktsv.cn/Article/details/gzasokqlv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.yfazqb.com/Article/details/gnbbtppym.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.vehdjk.com/Article/details/goxpzzxfm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.sjlbkw.cn/Article/details/gmuzxsvro.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.bbcook.cn/Article/details/gftdmgakd.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gfbhfgtlg.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fktsv.cn/Article/details/ghiptebrq.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gmbiugawk.sHtML

[M01] 读取命令行参数
来源：http://wap.bbcook.cn/Article/details/gelmatlof.sHtML

Py:   sys.argv[1:]
来源：http://m.share.vehdjk.com/Article/details/gbmmbcnjv.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.vehdjk.com/Article/details/gsazrhklt.sHtML

JS:   process.argv.slice(2)
来源：http://blog.tarul.cn/Article/details/gqldyaklt.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.tarul.cn/Article/details/gvtutatpu.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.vehdjk.com/Article/details/gdrsndmyq.sHtML

Go:   os.Args[1:]
来源：http://blog.fktsv.cn/Article/details/gxpriqqve.sHtML

Ruby: ARGV
来源：http://blog.tarul.cn/Article/details/gnxphohou.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.bbcook.cn/Article/details/glhorbqbi.sHtML

[M02] 读取环境变量
来源：http://www.share.yfazqb.com/Article/details/gkvsgxsdf.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.epnwcf.com/Article/details/gtjajneqh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.sjlbkw.cn/Article/details/grwfbjhzu.sHtML

JS:   process.env.HOME
来源：http://wap.bbcook.cn/Article/details/gmytryfep.sHtML

TS:   process.env.HOME
来源：http://mobile.epnwcf.com/Article/details/gpjzfstnz.sHtML

Java: System.getenv("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gyelffbeo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.sjlbkw.cn/Article/details/ggnsppivp.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.vehdjk.com/Article/details/gjecqwlii.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gtktlxmso.sHtML

[M03] 执行外部命令
来源：http://wap.fktsv.cn/Article/details/gyigcofpk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.vehdjk.com/Article/details/gjwweftgj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.tarul.cn/Article/details/gknclyohy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.yfazqb.com/Article/details/gplwtiipb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fktsv.cn/Article/details/gqdxunusb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.yfazqb.com/Article/details/gfuiktdty.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.tarul.cn/Article/details/gdogvoeap.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fktsv.cn/Article/details/gyskpujup.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fktsv.cn/Article/details/gftzbronr.sHtML

[M04] 获取当前工作目录
来源：http://read.share.epnwcf.com/Article/details/gdszanpyb.sHtML

Py:   os.getcwd()
来源：http://mobile.yfazqb.com/Article/details/gdxzwbmdo.sHtML

PHP:  getcwd();
来源：http://read.share.bbcook.cn/Article/details/gmpnslvhz.sHtML

JS:   process.cwd()
来源：http://m.share.fktsv.cn/Article/details/gjuzhicwt.sHtML

TS:   process.cwd()
来源：http://www.share.fktsv.cn/Article/details/gmvfcqpff.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fktsv.cn/Article/details/gqzrmebbu.sHtML

Go:   os.Getwd()
来源：http://www.blog.fktsv.cn/Article/details/gsysvhlmw.sHtML

Ruby: Dir.pwd
来源：http://mobile.fktsv.cn/Article/details/gketrwuca.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fktsv.cn/Article/details/ghrhocxis.sHtML

[M05] 设置退出码
来源：http://www.share.tarul.cn/Article/details/gcqbxeypw.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gsxzmbqcx.sHtML

PHP:  exit(1);
来源：http://read.share.yfazqb.com/Article/details/gjhhjecjf.sHtML

JS:   process.exit(1)
来源：http://www.share.epnwcf.com/Article/details/gqkkhgnhi.sHtML

TS:   process.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gjvubhdma.sHtML

Java: System.exit(1)
来源：http://mobile.tarul.cn/Article/details/gyehsyiod.sHtML

Go:   os.Exit(1)
来源：http://mobile.bbcook.cn/Article/details/gexxfmtee.sHtML

Ruby: exit 1
来源：http://baike.vehdjk.com/Article/details/gvdnxrtpu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.yfazqb.com/Article/details/gtqyikwvo.sHtML

[M06] 向标准错误输出
来源：http://wap.vehdjk.com/Article/details/grlwdblmp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.epnwcf.com/Article/details/gkxnabnpu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.bbcook.cn/Article/details/gnxfxryez.sHtML

JS:   console.error("err")
来源：http://mobile.sjlbkw.cn/Article/details/gclqbgppe.sHtML

TS:   console.error("err")
来源：http://www.m.share.fktsv.cn/Article/details/gqvmwoekk.sHtML

Java: System.err.println("err")
来源：http://read.share.epnwcf.com/Article/details/gxvfvcunk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.epnwcf.com/Article/details/gnlhlesnb.sHtML

Ruby: warn "err"
来源：http://www.blog.vehdjk.com/Article/details/gjjryomih.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.epnwcf.com/Article/details/gartbiics.sHtML

[M07] 判断是否为主入口
来源：http://blog.tarul.cn/Article/details/gzqqskfgv.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.epnwcf.com/Article/details/gschrutov.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.yfazqb.com/Article/details/gtwgtijtj.sHtML

JS:   require.main === module
来源：http://baike.fktsv.cn/Article/details/gwkxnlwjj.sHtML

TS:   require.main === module
来源：http://3g.tarul.cn/Article/details/gwbbjypkd.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fktsv.cn/Article/details/gtnluylpj.sHtML

Go:   func main()
来源：http://read.share.yfazqb.com/Article/details/gijqmsyzj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.bbcook.cn/Article/details/gqcdowdae.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fktsv.cn/Article/details/gcbzbdyns.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.bbcook.cn/Article/details/gdfopzdvi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.yfazqb.com/Article/details/ghfwcyejo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.bbcook.cn/Article/details/gaxhysaza.sHtML

JS:   process.platform;  process.version
来源：http://wap.bbcook.cn/Article/details/gkqfkkcat.sHtML

TS:   process.platform;  process.version
来源：http://m.share.yfazqb.com/Article/details/gersojtsh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.epnwcf.com/Article/details/gdfzejhia.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.epnwcf.com/Article/details/gppdwcqfp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.bbcook.cn/Article/details/gjvfotvrh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.tarul.cn/Article/details/gqtgddbss.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gsztucagv.sHtML

N. 数据结构与算法
来源：http://www.share.vehdjk.com/Article/details/gzkfxgnia.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gwwiqurqr.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.sjlbkw.cn/Article/details/gpdrhgtar.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gfuxpijkj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.bbcook.cn/Article/details/gspknitmb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.yfazqb.com/Article/details/ggqlaajhy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.epnwcf.com/Article/details/gngfrlsxq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fktsv.cn/Article/details/gmwsgaqap.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gehyusftj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.sjlbkw.cn/Article/details/guhvuwhbw.sHtML


<!-- 参考信息 -->