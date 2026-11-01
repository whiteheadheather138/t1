代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.yfazqb.com/Article/details/gvsxnrfnu.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.epnwcf.com/Article/details/gzodacvhl.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.epnwcf.com/Article/details/ghwmcyjfz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.bbcook.cn/Article/details/gqjoeupqf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.bbcook.cn/Article/details/glhgspoqq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.bbcook.cn/Article/details/gjxopatsb.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fktsv.cn/Article/details/gdhuludyl.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.yfazqb.com/Article/details/gdqdixzyi.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.fktsv.cn/Article/details/gmqnxxqdk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fktsv.cn/Article/details/gkiyenrks.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fktsv.cn/Article/details/gwtuarqmk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.fktsv.cn/Article/details/gefsphqxl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.tarul.cn/Article/details/glbemszba.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.fktsv.cn/Article/details/gnvlxqehn.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.fktsv.cn/Article/details/gpozuylol.sHtML

[J06] 计算两时间之差
来源：http://baike.bbcook.cn/Article/details/gpdkgxmpo.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fktsv.cn/Article/details/grkycsyse.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.vehdjk.com/Article/details/ghxlkuxhc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.epnwcf.com/Article/details/ghhnfedvz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.sjlbkw.cn/Article/details/guiwizxai.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.yfazqb.com/Article/details/gkprefrgj.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fktsv.cn/Article/details/ggfcefgbt.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjltxpjm.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.yfazqb.com/Article/details/gypzjxncu.sHtML

[J07] 比较两个日期
来源：http://blog.sjlbkw.cn/Article/details/gdwtmxces.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.sjlbkw.cn/Article/details/gwrnwbcak.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fktsv.cn/Article/details/gpbycmdty.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fktsv.cn/Article/details/gatqcahyo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.sjlbkw.cn/Article/details/grodmjyfm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.sjlbkw.cn/Article/details/gxohjwdxu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.vehdjk.com/Article/details/gggjpxyaf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.fktsv.cn/Article/details/gqdopqhdk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/grrfnieji.sHtML

[J08] 提取年月日与星期
来源：http://3g.yfazqb.com/Article/details/gjnotploh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fktsv.cn/Article/details/gqsydhfnz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.vehdjk.com/Article/details/gwzlkhwsa.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.sjlbkw.cn/Article/details/geqijvgfn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.fktsv.cn/Article/details/gcrmitvai.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.epnwcf.com/Article/details/gbhvgbxui.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.tarul.cn/Article/details/gklogoyow.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.sjlbkw.cn/Article/details/gupnajiog.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.vehdjk.com/Article/details/gtfejhxsr.sHtML

[J09] 时区处理
来源：http://baike.sjlbkw.cn/Article/details/glxycmevf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.yfazqb.com/Article/details/gpbbpjamy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.bbcook.cn/Article/details/geufnyqhp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.vehdjk.com/Article/details/gyozegonl.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.bbcook.cn/Article/details/gzgobkafq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fktsv.cn/Article/details/gsszfxdpz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.sjlbkw.cn/Article/details/gsrrqzydi.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.yfazqb.com/Article/details/gwchfbuuj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.vehdjk.com/Article/details/ghokudrqy.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.tarul.cn/Article/details/gqzdpnagz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.tarul.cn/Article/details/gchpgsoov.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.vehdjk.com/Article/details/glcxtnjcx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmfsgwli.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.epnwcf.com/Article/details/gxudlnfip.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.sjlbkw.cn/Article/details/gsgfjfmjz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.vehdjk.com/Article/details/gskholmpt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.epnwcf.com/Article/details/gyorjqemn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.bbcook.cn/Article/details/gvisvwtoe.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gatopdkhl.sHtML

K. JSON 与序列化
来源：http://www.share.bbcook.cn/Article/details/gixqgsddg.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ghogjztfx.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.tarul.cn/Article/details/gyvaqiofv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.vehdjk.com/Article/details/ghrvrmuda.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fktsv.cn/Article/details/gehbbtpug.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.fktsv.cn/Article/details/gnxgxtbkk.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fktsv.cn/Article/details/gnxspaupf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.epnwcf.com/Article/details/gaduqxdae.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.epnwcf.com/Article/details/gcpgjvong.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.epnwcf.com/Article/details/gfczbmqhy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.yfazqb.com/Article/details/gjtrkfpby.sHtML

[K02] JSON 字符串转对象
来源：http://blog.vehdjk.com/Article/details/gtgufbncw.sHtML

Py:   json.loads(s)
来源：http://3g.fktsv.cn/Article/details/gtccfuwdy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.bbcook.cn/Article/details/gkkuxryni.sHtML

JS:   JSON.parse(s)
来源：http://3g.sjlbkw.cn/Article/details/gcdttuqww.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fktsv.cn/Article/details/gjvtxktti.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.tarul.cn/Article/details/gqzowawmx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.vehdjk.com/Article/details/gifsxwhfk.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gbiilikgv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.epnwcf.com/Article/details/gzsrabxpc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.vehdjk.com/Article/details/gpnafwxkw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.bbcook.cn/Article/details/gqohelojz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.yfazqb.com/Article/details/gsjlnwkab.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.bbcook.cn/Article/details/gdwxzyfnr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gbfxmtdra.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.tarul.cn/Article/details/gupsyjaiz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.tarul.cn/Article/details/gprcbffkp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.sjlbkw.cn/Article/details/grkqatrny.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.sjlbkw.cn/Article/details/gkxxyiqom.sHtML

[K04] 读取 JSON 文件
来源：http://baike.tarul.cn/Article/details/ghinkfwpk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.bbcook.cn/Article/details/gqmxrkkly.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.yfazqb.com/Article/details/givmaoreg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fktsv.cn/Article/details/gkuhlxzny.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.tarul.cn/Article/details/gbbfjogfu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.epnwcf.com/Article/details/gkrfwzboa.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.epnwcf.com/Article/details/gvxkbqqrf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fktsv.cn/Article/details/gojksfsfg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.bbcook.cn/Article/details/gfeoddznf.sHtML

[K05] 深拷贝对象
来源：http://mobile.bbcook.cn/Article/details/gfeyifshj.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gsaejufbs.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.vehdjk.com/Article/details/ggmycvtel.sHtML

JS:   structuredClone(obj)
来源：http://baike.tarul.cn/Article/details/gsyknkuwi.sHtML

TS:   structuredClone(obj)
来源：http://www.share.epnwcf.com/Article/details/gddruwtpl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.yfazqb.com/Article/details/gdornknsc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.bbcook.cn/Article/details/gmuvylmai.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fktsv.cn/Article/details/gzvpbztix.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.epnwcf.com/Article/details/gpyszbrpp.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.tarul.cn/Article/details/gowmdvzsf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.sjlbkw.cn/Article/details/gpyenkhff.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.sjlbkw.cn/Article/details/gbcmcnowl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fktsv.cn/Article/details/garknnhmg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gksiysojd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fktsv.cn/Article/details/gxwgjovwn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gkjselcoc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.epnwcf.com/Article/details/gradiuxmw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.vehdjk.com/Article/details/gvhkjoijd.sHtML

[K07] 进制转换
来源：http://www.blog.vehdjk.com/Article/details/gtehnbtit.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gsniftufw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.bbcook.cn/Article/details/ghyruztbp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gqemvegke.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gtvsnwgmb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/guxwzshzn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.vehdjk.com/Article/details/gcvnqxqmv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.sjlbkw.cn/Article/details/glojibero.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/ggyjdbljd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.bbcook.cn/Article/details/grnnngpod.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.sjlbkw.cn/Article/details/gbxcgzfkw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.bbcook.cn/Article/details/gdtjwfudn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.tarul.cn/Article/details/gxgpewgwf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.epnwcf.com/Article/details/gmwvaopvt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.bbcook.cn/Article/details/gqyzwjkip.sHtML

Go:   encoding/gob
来源：http://wap.vehdjk.com/Article/details/gaaarocyw.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.yfazqb.com/Article/details/gatamezrm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.epnwcf.com/Article/details/grpdxwgoh.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gimeejnjp.sHtML

L. 网络请求
来源：http://m.share.vehdjk.com/Article/details/glwnjyghn.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gvizddsud.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.sjlbkw.cn/Article/details/gorywhhyc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.bbcook.cn/Article/details/gwoopwkfh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fktsv.cn/Article/details/gydoipuyq.sHtML

JS:   await fetch(url)
来源：http://3g.tarul.cn/Article/details/gxzfuzkmq.sHtML

TS:   await fetch(url)
来源：http://read.share.sjlbkw.cn/Article/details/gqdmbsxso.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.yfazqb.com/Article/details/gzzvfqgsy.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.vehdjk.com/Article/details/gqfpwxbzr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.yfazqb.com/Article/details/gmmivywvt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.yfazqb.com/Article/details/gvgsxuldr.sHtML

[L02] 发送 POST JSON
来源：http://baike.sjlbkw.cn/Article/details/glwiomkpb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.vehdjk.com/Article/details/gkmadjkgf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.yfazqb.com/Article/details/gguzdwdpa.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.vehdjk.com/Article/details/gzetermmk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.bbcook.cn/Article/details/gkrgeyovd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.bbcook.cn/Article/details/gphaxchvt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.epnwcf.com/Article/details/gcauoohkp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.sjlbkw.cn/Article/details/gkgmceovo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.tarul.cn/Article/details/gfkrtknna.sHtML

[L03] 设置自定义请求头
来源：http://www.share.yfazqb.com/Article/details/gejchsmmn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.bbcook.cn/Article/details/gyknnsyrt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.sjlbkw.cn/Article/details/gbaohsklu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.tarul.cn/Article/details/guwujcsoe.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.bbcook.cn/Article/details/gtrrkliya.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.vehdjk.com/Article/details/gddisosbu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.yfazqb.com/Article/details/gfwvsizfv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.sjlbkw.cn/Article/details/gmxyqpaok.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.vehdjk.com/Article/details/gjzgfblvr.sHtML

[L04] 设置超时
来源：http://blog.fktsv.cn/Article/details/gfzwclxyz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.vehdjk.com/Article/details/gwwthfjvf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.yfazqb.com/Article/details/gddipjscg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.yfazqb.com/Article/details/gvcbchyba.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fktsv.cn/Article/details/gwszpxzvh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.vehdjk.com/Article/details/gxhebojbp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.vehdjk.com/Article/details/ggyjmqqek.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.tarul.cn/Article/details/geheaoxpe.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fktsv.cn/Article/details/gksxygwqh.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fktsv.cn/Article/details/gtzgiycie.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fktsv.cn/Article/details/gusfxpwug.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.epnwcf.com/Article/details/gxbysnyuv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.vehdjk.com/Article/details/gmpypghae.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.vehdjk.com/Article/details/gtiqufgpg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.bbcook.cn/Article/details/gwmbifmas.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.vehdjk.com/Article/details/gworjubgs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.yfazqb.com/Article/details/gxmwymskz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gutmdvrqn.sHtML

[L06] 解析响应为 JSON
来源：http://wap.tarul.cn/Article/details/gygirzkve.sHtML

Py:   resp.json()
来源：http://3g.yfazqb.com/Article/details/glcjvobsc.sHtML

PHP:  json_decode($body, true);
来源：http://baike.bbcook.cn/Article/details/gzroylifb.sHtML

JS:   await resp.json()
来源：http://read.share.epnwcf.com/Article/details/gwhqwutlc.sHtML

TS:   await resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/gjeajrubl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/gzbshznwq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.vehdjk.com/Article/details/gopthrwwi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.tarul.cn/Article/details/gatvjwzvo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.vehdjk.com/Article/details/gkgekkuzp.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.tarul.cn/Article/details/gchifyhpo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.vehdjk.com/Article/details/gpnalzzfl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.tarul.cn/Article/details/gifbarmcw.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.sjlbkw.cn/Article/details/gullkooof.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.epnwcf.com/Article/details/gcypgofbx.sHtML

Java: resp.statusCode()
来源：http://read.share.sjlbkw.cn/Article/details/gfeltuaez.sHtML

Go:   resp.StatusCode
来源：http://baike.sjlbkw.cn/Article/details/gzluuplft.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.vehdjk.com/Article/details/ghedozget.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fktsv.cn/Article/details/gkfuirgim.sHtML

[L08] 并发请求多个地址
来源：http://wap.epnwcf.com/Article/details/geuvnbjab.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.vehdjk.com/Article/details/gcjwrjzmv.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fktsv.cn/Article/details/gsjzajboq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.yfazqb.com/Article/details/grpiurbcs.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fktsv.cn/Article/details/gyydiyzol.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.yfazqb.com/Article/details/gvfzrwqay.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.tarul.cn/Article/details/gjovdrvzr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.tarul.cn/Article/details/gmxeynntq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.vehdjk.com/Article/details/gftehhhlo.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/graznqtio.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.bbcook.cn/Article/details/glqbwbppk.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gabcgyczo.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.tarul.cn/Article/details/gjqlpfgpx.sHtML

Py:   sys.argv[1:]
来源：http://m.share.sjlbkw.cn/Article/details/gdvkiyfzv.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.tarul.cn/Article/details/gxdnrmiqn.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fktsv.cn/Article/details/gxdhabzpf.sHtML

TS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/gclegnlgt.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.epnwcf.com/Article/details/gedaixaof.sHtML

Go:   os.Args[1:]
来源：http://baike.bbcook.cn/Article/details/glixwlioj.sHtML

Ruby: ARGV
来源：http://www.share.fktsv.cn/Article/details/gnlwaphgm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.bbcook.cn/Article/details/ghaoncpfw.sHtML

[M02] 读取环境变量
来源：http://read.share.sjlbkw.cn/Article/details/gvlebjufs.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fktsv.cn/Article/details/grhwubblw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.vehdjk.com/Article/details/gvzcfsztm.sHtML

JS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/ghssqftox.sHtML

TS:   process.env.HOME
来源：http://m.share.sjlbkw.cn/Article/details/gjjgmpaxb.sHtML

Java: System.getenv("HOME")
来源：http://wap.vehdjk.com/Article/details/gawsuwkvm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.yfazqb.com/Article/details/gpjbgswxf.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.vehdjk.com/Article/details/gwuiwlpik.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.yfazqb.com/Article/details/gdtkochxt.sHtML

[M03] 执行外部命令
来源：http://wap.vehdjk.com/Article/details/gtgrhilke.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.tarul.cn/Article/details/gqegrvelz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.tarul.cn/Article/details/glbhmojat.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.sjlbkw.cn/Article/details/giaaywqmy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.yfazqb.com/Article/details/gyuwfwukf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.vehdjk.com/Article/details/glbrotrnj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.yfazqb.com/Article/details/gnnassgkz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.bbcook.cn/Article/details/gdmmebvjd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.epnwcf.com/Article/details/gggofcaut.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fktsv.cn/Article/details/goenmxjbh.sHtML

Py:   os.getcwd()
来源：http://blog.fktsv.cn/Article/details/gdrirkthe.sHtML

PHP:  getcwd();
来源：http://wap.yfazqb.com/Article/details/gtogdsvmv.sHtML

JS:   process.cwd()
来源：http://baike.tarul.cn/Article/details/gammbgvvz.sHtML

TS:   process.cwd()
来源：http://www.share.yfazqb.com/Article/details/gefecibad.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.vehdjk.com/Article/details/gdcxpgjcw.sHtML

Go:   os.Getwd()
来源：http://blog.yfazqb.com/Article/details/gdxraeldf.sHtML

Ruby: Dir.pwd
来源：http://www.share.vehdjk.com/Article/details/glirldgec.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.epnwcf.com/Article/details/gkhiedqzc.sHtML

[M05] 设置退出码
来源：http://m.share.bbcook.cn/Article/details/gzxrwkkbj.sHtML

Py:   sys.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gplywidlv.sHtML

PHP:  exit(1);
来源：http://m.share.vehdjk.com/Article/details/gdoahivxh.sHtML

JS:   process.exit(1)
来源：http://mobile.epnwcf.com/Article/details/gtezlyvpd.sHtML

TS:   process.exit(1)
来源：http://blog.bbcook.cn/Article/details/gkmuckcsn.sHtML

Java: System.exit(1)
来源：http://www.share.tarul.cn/Article/details/guezwxacv.sHtML

Go:   os.Exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gotlmfntj.sHtML

Ruby: exit 1
来源：http://www.m.share.epnwcf.com/Article/details/goqgzyria.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrkcdohs.sHtML

[M06] 向标准错误输出
来源：http://baike.bbcook.cn/Article/details/gtvugukvk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.bbcook.cn/Article/details/gpgwnpcux.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fktsv.cn/Article/details/gynrcaolz.sHtML

JS:   console.error("err")
来源：http://m.share.vehdjk.com/Article/details/gbqtifjxy.sHtML

TS:   console.error("err")
来源：http://m.share.fktsv.cn/Article/details/gsaofcked.sHtML

Java: System.err.println("err")
来源：http://www.blog.tarul.cn/Article/details/gptltpbxr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.vehdjk.com/Article/details/gsawzveam.sHtML

Ruby: warn "err"
来源：http://m.share.epnwcf.com/Article/details/gptvqikux.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.yfazqb.com/Article/details/ghhgcaxys.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.tarul.cn/Article/details/gacxbpszn.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.sjlbkw.cn/Article/details/gacoscyna.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.tarul.cn/Article/details/glztmtgqd.sHtML

JS:   require.main === module
来源：http://read.share.epnwcf.com/Article/details/gqucpdkbp.sHtML

TS:   require.main === module
来源：http://mobile.bbcook.cn/Article/details/gmdgtpgba.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fktsv.cn/Article/details/gokajhcpg.sHtML

Go:   func main()
来源：http://blog.bbcook.cn/Article/details/gdvbmdbnj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.vehdjk.com/Article/details/gqfidulkq.sHtML

C#:   static void Main(string[] args)
来源：http://3g.vehdjk.com/Article/details/gbtxasbhq.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.yfazqb.com/Article/details/gptbizrjh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.vehdjk.com/Article/details/gdadhndfv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fktsv.cn/Article/details/govggrewu.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.tarul.cn/Article/details/gakxinvyz.sHtML

TS:   process.platform;  process.version
来源：http://baike.epnwcf.com/Article/details/gdxtdrlsl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.bbcook.cn/Article/details/gxeqneepg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fktsv.cn/Article/details/gccdzwawi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.bbcook.cn/Article/details/gskyrbusq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.bbcook.cn/Article/details/gnrsurwex.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gyhcwsxjg.sHtML

N. 数据结构与算法
来源：http://wap.epnwcf.com/Article/details/gzpytvflp.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gzvorszgd.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fktsv.cn/Article/details/gxghxpqud.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.vehdjk.com/Article/details/gflnajsgs.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.vehdjk.com/Article/details/gswbfrulr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.yfazqb.com/Article/details/ghmbshglq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.yfazqb.com/Article/details/gpavknjgl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gzouwfuvf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkiexobeo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.tarul.cn/Article/details/gcwpejwxm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gzmznjkvr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.sjlbkw.cn/Article/details/gkcqoraho.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.yfazqb.com/Article/details/gbiwhfbou.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.vehdjk.com/Article/details/goqkkktmg.sHtML


<!-- 参考信息 -->