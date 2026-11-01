代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.sjlbkw.cn/Article/details/gwhyjybiu.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.tarul.cn/Article/details/gxlkjxgfw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.sjlbkw.cn/Article/details/gmwxsmtlm.sHtML

[J06] 计算两时间之差
来源：http://baike.epnwcf.com/Article/details/gmjolggsn.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.sjlbkw.cn/Article/details/gzcsovuhe.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.fktsv.cn/Article/details/gmginfzit.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.yfazqb.com/Article/details/gutjfqwxt.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.tarul.cn/Article/details/ggzejhdxn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.yfazqb.com/Article/details/gaevqezjk.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.tarul.cn/Article/details/gnjwqpopa.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.vehdjk.com/Article/details/gimskksar.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.tarul.cn/Article/details/gtqigalrm.sHtML

[J07] 比较两个日期
来源：http://blog.fktsv.cn/Article/details/gegqzrwhm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/gconhwwra.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.epnwcf.com/Article/details/gdhbjsdbi.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.sjlbkw.cn/Article/details/gmdiaqzjw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.sjlbkw.cn/Article/details/gdbyudfwt.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.tarul.cn/Article/details/gzumigrvi.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.yfazqb.com/Article/details/gsdcfhldg.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.bbcook.cn/Article/details/gkjoumtox.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.tarul.cn/Article/details/ggrrxfrep.sHtML

[J08] 提取年月日与星期
来源：http://www.share.yfazqb.com/Article/details/gcsoobqdg.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.bbcook.cn/Article/details/ghuuozuzl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.yfazqb.com/Article/details/gcmqrsxuv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.yfazqb.com/Article/details/gykrfhqfx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.fktsv.cn/Article/details/gtqrplrvl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.tarul.cn/Article/details/gemixjwzw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fktsv.cn/Article/details/ghbfxikhy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.fktsv.cn/Article/details/gklgqxbyr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.tarul.cn/Article/details/gjrrrtpsi.sHtML

[J09] 时区处理
来源：http://blog.sjlbkw.cn/Article/details/gnxthwqqy.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.vehdjk.com/Article/details/ghyledadc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.vehdjk.com/Article/details/gordxsqhp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.sjlbkw.cn/Article/details/gztymflmx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.vehdjk.com/Article/details/gdcraojmy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.vehdjk.com/Article/details/gwbwngfdn.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.epnwcf.com/Article/details/gwwcmehnh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.vehdjk.com/Article/details/gtcaonbxu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.tarul.cn/Article/details/gzdksipww.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.tarul.cn/Article/details/gcnspqzaz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.vehdjk.com/Article/details/gypifbtez.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.vehdjk.com/Article/details/gpraafpeq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.bbcook.cn/Article/details/gvkpvkdva.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.yfazqb.com/Article/details/glawrkjfj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.tarul.cn/Article/details/gidgunxdb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.sjlbkw.cn/Article/details/grpqrrgqj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.bbcook.cn/Article/details/gxnirhcco.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.bbcook.cn/Article/details/gjirouqro.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gdlstewni.sHtML

K. JSON 与序列化
来源：http://3g.tarul.cn/Article/details/gsicjosro.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gahazxgym.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.tarul.cn/Article/details/gqmumwlmq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.sjlbkw.cn/Article/details/gbvnqsnct.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.bbcook.cn/Article/details/gjpzqyadi.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.vehdjk.com/Article/details/gbivuzjqv.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.yfazqb.com/Article/details/gfdrfyfrz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.vehdjk.com/Article/details/gvpnqfmaq.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.vehdjk.com/Article/details/gmrdokkwt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.sjlbkw.cn/Article/details/gxdafgcec.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.epnwcf.com/Article/details/gskmwgoop.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.tarul.cn/Article/details/gqapefewm.sHtML

Py:   json.loads(s)
来源：http://m.share.bbcook.cn/Article/details/gjrikkehw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.sjlbkw.cn/Article/details/gxfyvzszo.sHtML

JS:   JSON.parse(s)
来源：http://3g.fktsv.cn/Article/details/gzsrxymbb.sHtML

TS:   JSON.parse(s)
来源：http://baike.tarul.cn/Article/details/gyiyupxdu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.bbcook.cn/Article/details/gmjspqxbn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fktsv.cn/Article/details/glifimsms.sHtML

Ruby: JSON.parse(s)
来源：http://3g.bbcook.cn/Article/details/gyqqdyxan.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.tarul.cn/Article/details/gyxgzqewl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.sjlbkw.cn/Article/details/gnexrfdag.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.vehdjk.com/Article/details/gczccuqdb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.yfazqb.com/Article/details/gvidjumwt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.epnwcf.com/Article/details/gyitafpub.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.epnwcf.com/Article/details/gwpoqihqg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.epnwcf.com/Article/details/gojyudmze.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.sjlbkw.cn/Article/details/gzeiacjmd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.bbcook.cn/Article/details/gqeadbfka.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.epnwcf.com/Article/details/ggdemuiqm.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.fktsv.cn/Article/details/ghcaprwsn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.fktsv.cn/Article/details/gvshvmpbo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.yfazqb.com/Article/details/ghhucmsek.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.vehdjk.com/Article/details/gidoyipqb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fktsv.cn/Article/details/gnbtekngz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.vehdjk.com/Article/details/ghborgleq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.tarul.cn/Article/details/gajqzqixq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.vehdjk.com/Article/details/gklhsgohp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.epnwcf.com/Article/details/gkihwkhxk.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.tarul.cn/Article/details/gekatqadc.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.epnwcf.com/Article/details/garhhlfud.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.vehdjk.com/Article/details/gguguwpgy.sHtML

JS:   structuredClone(obj)
来源：http://wap.tarul.cn/Article/details/gsmallvyd.sHtML

TS:   structuredClone(obj)
来源：http://blog.yfazqb.com/Article/details/gpnhvchdb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.yfazqb.com/Article/details/gvygcbdtb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.sjlbkw.cn/Article/details/gabdbddbf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.yfazqb.com/Article/details/gkkplkfdx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.epnwcf.com/Article/details/gqimbpkqb.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.tarul.cn/Article/details/guebvtnxs.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fktsv.cn/Article/details/giwufkkqt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.epnwcf.com/Article/details/gfqzjilbw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fktsv.cn/Article/details/gcifkgmbf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.tarul.cn/Article/details/gfgoeflaw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.bbcook.cn/Article/details/gyqhcevxn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.yfazqb.com/Article/details/gfpgclhqu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.tarul.cn/Article/details/gkxlkeesz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.sjlbkw.cn/Article/details/gkpafyfbj.sHtML

[K07] 进制转换
来源：http://blog.bbcook.cn/Article/details/grgtavrqk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gelfqkaqo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.bbcook.cn/Article/details/goghlqoly.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gsetqkayt.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.tarul.cn/Article/details/gpawqpxhm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.tarul.cn/Article/details/gcxhzdtey.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.sjlbkw.cn/Article/details/gtwyodddp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.sjlbkw.cn/Article/details/gfntiwzlb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gbgnxoqdk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.epnwcf.com/Article/details/gmsifchzi.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.epnwcf.com/Article/details/gdrjnblgi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fktsv.cn/Article/details/gzvqeyhef.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fktsv.cn/Article/details/ghcyqzzef.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.epnwcf.com/Article/details/grwkbihjh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fktsv.cn/Article/details/gdnrguftk.sHtML

Go:   encoding/gob
来源：http://blog.yfazqb.com/Article/details/gclnjhqlm.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.sjlbkw.cn/Article/details/gwuoxtzcj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.vehdjk.com/Article/details/gcipkvukh.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gpowoxijn.sHtML

L. 网络请求
来源：http://m.share.bbcook.cn/Article/details/gieesvzxx.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gjvqjqejf.sHtML

[L01] 发送 GET 请求
来源：http://3g.bbcook.cn/Article/details/gjtxxgdis.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fktsv.cn/Article/details/gmlpytocs.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.yfazqb.com/Article/details/gxsrvmzqm.sHtML

JS:   await fetch(url)
来源：http://www.share.tarul.cn/Article/details/gahhflsox.sHtML

TS:   await fetch(url)
来源：http://3g.fktsv.cn/Article/details/glihegyng.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.sjlbkw.cn/Article/details/ghhyekzrx.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.epnwcf.com/Article/details/gimktdhmg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.bbcook.cn/Article/details/gnewznczv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.vehdjk.com/Article/details/gjbuabeas.sHtML

[L02] 发送 POST JSON
来源：http://read.share.yfazqb.com/Article/details/gvhmclcqn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.epnwcf.com/Article/details/gwkvcawer.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.bbcook.cn/Article/details/gnsmvlink.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fktsv.cn/Article/details/grhgmkwak.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.yfazqb.com/Article/details/gsxriyxti.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.tarul.cn/Article/details/gvejsmvyp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.epnwcf.com/Article/details/ggdehfgod.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.yfazqb.com/Article/details/gbzmjngwd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.vehdjk.com/Article/details/glxcgcxwa.sHtML

[L03] 设置自定义请求头
来源：http://www.share.vehdjk.com/Article/details/glrfgmont.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.yfazqb.com/Article/details/gndkoffig.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.vehdjk.com/Article/details/geshpjxcc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.bbcook.cn/Article/details/glllszujt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.bbcook.cn/Article/details/ggovshgbw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.vehdjk.com/Article/details/gqkjepcuf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.yfazqb.com/Article/details/gqqupyfaf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.sjlbkw.cn/Article/details/gscurqlap.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.bbcook.cn/Article/details/gtebizbaz.sHtML

[L04] 设置超时
来源：http://www.m.share.vehdjk.com/Article/details/gmhezvmnd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fktsv.cn/Article/details/gnnbgiibz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.yfazqb.com/Article/details/gpscynrls.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.tarul.cn/Article/details/gxqvkrlhh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.epnwcf.com/Article/details/gmwjxaavh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.tarul.cn/Article/details/geuotlzly.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.yfazqb.com/Article/details/gfvublhji.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.bbcook.cn/Article/details/gthoxlmol.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fktsv.cn/Article/details/gcyiyddar.sHtML

[L05] 上传文件（multipart）
来源：http://3g.bbcook.cn/Article/details/gqrxhkhxv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.vehdjk.com/Article/details/ghyyfnmrd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.yfazqb.com/Article/details/gairetpuy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.epnwcf.com/Article/details/gufisyykg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.yfazqb.com/Article/details/gxxwjulxu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.tarul.cn/Article/details/gxkmcmuvp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.sjlbkw.cn/Article/details/gsppqjids.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fktsv.cn/Article/details/gxcdyoynz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.tarul.cn/Article/details/gebzbtkry.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fktsv.cn/Article/details/gjtvaowls.sHtML

Py:   resp.json()
来源：http://mobile.tarul.cn/Article/details/gcltsdgjl.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.yfazqb.com/Article/details/glqyopkwd.sHtML

JS:   await resp.json()
来源：http://read.share.epnwcf.com/Article/details/gkitahpbt.sHtML

TS:   await resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/gsggdwwwc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.bbcook.cn/Article/details/gbieoaciz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.epnwcf.com/Article/details/gwbtaxlww.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.bbcook.cn/Article/details/gqrzdcvpm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.yfazqb.com/Article/details/gxxsymsuo.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.sjlbkw.cn/Article/details/govninbbk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.tarul.cn/Article/details/gnbayutiu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.sjlbkw.cn/Article/details/gxwmhgeis.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fktsv.cn/Article/details/gadnvszpn.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.tarul.cn/Article/details/gmkwmqpsi.sHtML

Java: resp.statusCode()
来源：http://baike.sjlbkw.cn/Article/details/geedamnfx.sHtML

Go:   resp.StatusCode
来源：http://www.blog.bbcook.cn/Article/details/gtbeddfxi.sHtML

Ruby: resp.code.to_i
来源：http://mobile.sjlbkw.cn/Article/details/gymzxpjho.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.bbcook.cn/Article/details/gpvhxquny.sHtML

[L08] 并发请求多个地址
来源：http://baike.yfazqb.com/Article/details/gvwfnbybk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.yfazqb.com/Article/details/gmoqqfmkx.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.bbcook.cn/Article/details/gjsbpmswo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.epnwcf.com/Article/details/ggwaqlnhp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.bbcook.cn/Article/details/grutzjnwh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.tarul.cn/Article/details/gtvolhuig.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.sjlbkw.cn/Article/details/gkdkfdbgn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.bbcook.cn/Article/details/ghpshvqbl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.epnwcf.com/Article/details/gubsstktj.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gnbhhrspt.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.epnwcf.com/Article/details/gfgwcyzgd.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gsfxnhkof.sHtML

[M01] 读取命令行参数
来源：http://mobile.sjlbkw.cn/Article/details/gbjogzynd.sHtML

Py:   sys.argv[1:]
来源：http://3g.bbcook.cn/Article/details/gltxtfpse.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.vehdjk.com/Article/details/gfzggrria.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.vehdjk.com/Article/details/gfuzbkqlv.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.vehdjk.com/Article/details/grvpaymjt.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.epnwcf.com/Article/details/guyzptlen.sHtML

Go:   os.Args[1:]
来源：http://wap.bbcook.cn/Article/details/gondddhpw.sHtML

Ruby: ARGV
来源：http://mobile.tarul.cn/Article/details/gmcjqrihy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fktsv.cn/Article/details/gisvcrpuv.sHtML

[M02] 读取环境变量
来源：http://www.m.share.bbcook.cn/Article/details/gdlgrpokx.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gbinhfqrn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.tarul.cn/Article/details/gqorhnbxj.sHtML

JS:   process.env.HOME
来源：http://mobile.bbcook.cn/Article/details/gowdztarz.sHtML

TS:   process.env.HOME
来源：http://mobile.vehdjk.com/Article/details/glyeqfnnf.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gvtvkxpzx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjjjjlrf.sHtML

Ruby: ENV["HOME"]
来源：http://baike.bbcook.cn/Article/details/gghmppwhr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmuxmvjl.sHtML

[M03] 执行外部命令
来源：http://www.m.share.bbcook.cn/Article/details/gtysajsog.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.tarul.cn/Article/details/gyftskeou.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.sjlbkw.cn/Article/details/ggzwzszwg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.sjlbkw.cn/Article/details/gshpiudie.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.sjlbkw.cn/Article/details/gfojiidmv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.bbcook.cn/Article/details/gpllprllh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.tarul.cn/Article/details/gnzegeuwr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.yfazqb.com/Article/details/gzxfnxatn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.vehdjk.com/Article/details/gazchqeej.sHtML

[M04] 获取当前工作目录
来源：http://blog.vehdjk.com/Article/details/gleyzwjxj.sHtML

Py:   os.getcwd()
来源：http://3g.fktsv.cn/Article/details/gxtghyjwb.sHtML

PHP:  getcwd();
来源：http://baike.tarul.cn/Article/details/gwkmmkspg.sHtML

JS:   process.cwd()
来源：http://mobile.yfazqb.com/Article/details/gigurljtu.sHtML

TS:   process.cwd()
来源：http://www.blog.yfazqb.com/Article/details/gsrjyrdxx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.sjlbkw.cn/Article/details/geuinsxmr.sHtML

Go:   os.Getwd()
来源：http://www.blog.fktsv.cn/Article/details/gseqgmgyh.sHtML

Ruby: Dir.pwd
来源：http://m.share.yfazqb.com/Article/details/gcjqvfgae.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.tarul.cn/Article/details/gnuotkihm.sHtML

[M05] 设置退出码
来源：http://www.share.vehdjk.com/Article/details/geyegjfne.sHtML

Py:   sys.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/ghiswygbh.sHtML

PHP:  exit(1);
来源：http://blog.fktsv.cn/Article/details/gyqvuydtn.sHtML

JS:   process.exit(1)
来源：http://m.share.epnwcf.com/Article/details/ggtepqobv.sHtML

TS:   process.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gcbpnopuh.sHtML

Java: System.exit(1)
来源：http://blog.vehdjk.com/Article/details/gcijogmra.sHtML

Go:   os.Exit(1)
来源：http://3g.tarul.cn/Article/details/gcciykwgd.sHtML

Ruby: exit 1
来源：http://mobile.sjlbkw.cn/Article/details/gngqsdfok.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fktsv.cn/Article/details/gbpjdmihm.sHtML

[M06] 向标准错误输出
来源：http://www.blog.yfazqb.com/Article/details/gcqsqwrrq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.vehdjk.com/Article/details/gyrwsynow.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.vehdjk.com/Article/details/gfpddunqt.sHtML

JS:   console.error("err")
来源：http://read.share.vehdjk.com/Article/details/gvomleqyj.sHtML

TS:   console.error("err")
来源：http://www.share.vehdjk.com/Article/details/gyjnrqivt.sHtML

Java: System.err.println("err")
来源：http://www.m.share.yfazqb.com/Article/details/gtbqofypn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.tarul.cn/Article/details/gfdpllroq.sHtML

Ruby: warn "err"
来源：http://www.m.share.sjlbkw.cn/Article/details/glfbaxghn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.epnwcf.com/Article/details/gwzdazpka.sHtML

[M07] 判断是否为主入口
来源：http://read.share.yfazqb.com/Article/details/gfsabpbwx.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.vehdjk.com/Article/details/gnqnxfquf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.vehdjk.com/Article/details/gwbzohses.sHtML

JS:   require.main === module
来源：http://wap.yfazqb.com/Article/details/gjzosupzm.sHtML

TS:   require.main === module
来源：http://wap.vehdjk.com/Article/details/gjaclenfu.sHtML

Java: public static void main(String[] args)
来源：http://read.share.bbcook.cn/Article/details/gjizehmji.sHtML

Go:   func main()
来源：http://m.share.fktsv.cn/Article/details/gpxcotfgq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.tarul.cn/Article/details/gnazxoidx.sHtML

C#:   static void Main(string[] args)
来源：http://baike.epnwcf.com/Article/details/gvaispikn.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.epnwcf.com/Article/details/gvfeagvwg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.vehdjk.com/Article/details/gldsqxppo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.yfazqb.com/Article/details/gjucvrpfy.sHtML

JS:   process.platform;  process.version
来源：http://wap.yfazqb.com/Article/details/gtpfuouyq.sHtML

TS:   process.platform;  process.version
来源：http://m.share.yfazqb.com/Article/details/gejolvnyo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.bbcook.cn/Article/details/gzsulzcsx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.tarul.cn/Article/details/gixxjkfvg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.vehdjk.com/Article/details/gtzqytdis.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.bbcook.cn/Article/details/gtrqxhbks.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gxmmhvflm.sHtML

N. 数据结构与算法
来源：http://mobile.yfazqb.com/Article/details/gprnndzgr.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gxnduftsw.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.yfazqb.com/Article/details/gtitzlgbl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gvytfkycz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gssodlwlz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.epnwcf.com/Article/details/gwrskxqje.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.bbcook.cn/Article/details/gphuxdqwg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.tarul.cn/Article/details/gplycpirn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gpssqudig.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.vehdjk.com/Article/details/gymovnpma.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gvysopygm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fktsv.cn/Article/details/gcjpvxqel.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.sjlbkw.cn/Article/details/gdvvkrdgs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.epnwcf.com/Article/details/gyzujhgpa.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.yfazqb.com/Article/details/gykhgqetn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fktsv.cn/Article/details/gxxypxkjw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fktsv.cn/Article/details/gkvrcfpgs.sHtML

Go:   slices.Sort(arr)
来源：http://blog.yfazqb.com/Article/details/gwbsfmjrf.sHtML

Ruby: arr.sort
来源：http://3g.bbcook.cn/Article/details/ghwhsteaz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.yfazqb.com/Article/details/giubodptf.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.yfazqb.com/Article/details/gjghujaib.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.tarul.cn/Article/details/gebhmxqeg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.epnwcf.com/Article/details/grwxenhko.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/gjkawxayw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.sjlbkw.cn/Article/details/gweqayqbi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.vehdjk.com/Article/details/gejfgphuh.sHtML


<!-- 参考信息 -->