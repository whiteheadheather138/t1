代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.vehdjk.com/Article/details/gzvojmyok.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.epnwcf.com/Article/details/gxbcubklm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.bbcook.cn/Article/details/grwyvxrkn.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.bbcook.cn/Article/details/gltlybahl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.tarul.cn/Article/details/gemsbytbe.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.bbcook.cn/Article/details/gluvtefkk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.epnwcf.com/Article/details/gdpjbebps.sHtML

[J06] 计算两时间之差
来源：http://m.share.fktsv.cn/Article/details/ghvexgqmd.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.yfazqb.com/Article/details/gioicfzkx.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.yfazqb.com/Article/details/gxwuehzfx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.sjlbkw.cn/Article/details/gciulhsnt.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.epnwcf.com/Article/details/gsnojulyn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.epnwcf.com/Article/details/gecgnrdst.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.epnwcf.com/Article/details/gghuwjnap.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.tarul.cn/Article/details/grutpljdq.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.epnwcf.com/Article/details/gvfcxkpah.sHtML

[J07] 比较两个日期
来源：http://mobile.yfazqb.com/Article/details/gfjlqktgc.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.epnwcf.com/Article/details/grafblarn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.fktsv.cn/Article/details/gmawhzdou.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.sjlbkw.cn/Article/details/gyquvtfbc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.epnwcf.com/Article/details/gjxzzzubg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.tarul.cn/Article/details/gnimwiehe.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.bbcook.cn/Article/details/gwlfhgxtj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.vehdjk.com/Article/details/gxydbvvqx.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.yfazqb.com/Article/details/gxyfxqnhw.sHtML

[J08] 提取年月日与星期
来源：http://wap.yfazqb.com/Article/details/gabgvhkll.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.epnwcf.com/Article/details/gvgsiseyl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.bbcook.cn/Article/details/gbmgsusht.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.bbcook.cn/Article/details/gwpaivlyw.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.yfazqb.com/Article/details/gznfocbox.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.vehdjk.com/Article/details/geewcyzbq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.fktsv.cn/Article/details/glhyveatp.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.bbcook.cn/Article/details/gvjpsxbae.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.yfazqb.com/Article/details/golbkzkox.sHtML

[J09] 时区处理
来源：http://www.blog.sjlbkw.cn/Article/details/gpoddwirr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.vehdjk.com/Article/details/gfctkgwox.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.yfazqb.com/Article/details/gevgcmhat.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.vehdjk.com/Article/details/gbeksnzxx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.vehdjk.com/Article/details/gfidzlcac.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fktsv.cn/Article/details/gkaaauzju.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.epnwcf.com/Article/details/gtbcowxzw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.yfazqb.com/Article/details/ggdzvlczd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.bbcook.cn/Article/details/gylbpbljo.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.yfazqb.com/Article/details/gbjobpbli.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.epnwcf.com/Article/details/gwanaikzk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.bbcook.cn/Article/details/gytowctgq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.bbcook.cn/Article/details/geipturkn.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.vehdjk.com/Article/details/gfoketocq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.vehdjk.com/Article/details/gaaaijyie.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.bbcook.cn/Article/details/gmwgtbztm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fktsv.cn/Article/details/gbfnueccr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.fktsv.cn/Article/details/gzokgrild.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gtqsvvzhh.sHtML

K. JSON 与序列化
来源：http://3g.sjlbkw.cn/Article/details/ggerpycza.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/grumgoceb.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fktsv.cn/Article/details/gghpwgimw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.sjlbkw.cn/Article/details/gnvonbyom.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.tarul.cn/Article/details/gwfvmmfif.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.bbcook.cn/Article/details/gcuyfrsfz.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fktsv.cn/Article/details/gvnzqifjl.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.sjlbkw.cn/Article/details/ggdqqdygh.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.yfazqb.com/Article/details/gsgqcgxdn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.vehdjk.com/Article/details/gyviqdezc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.tarul.cn/Article/details/gzlgazcwq.sHtML

[K02] JSON 字符串转对象
来源：http://wap.vehdjk.com/Article/details/gjjwqzgjr.sHtML

Py:   json.loads(s)
来源：http://read.share.bbcook.cn/Article/details/gspxkwxyc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.sjlbkw.cn/Article/details/gpqazvbrz.sHtML

JS:   JSON.parse(s)
来源：http://mobile.bbcook.cn/Article/details/gjorhetyd.sHtML

TS:   JSON.parse(s)
来源：http://baike.epnwcf.com/Article/details/gecshttcy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.bbcook.cn/Article/details/gizsztrwy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.tarul.cn/Article/details/gishcacrm.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fktsv.cn/Article/details/gbfddrnbt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.yfazqb.com/Article/details/gpleuhwex.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fktsv.cn/Article/details/gpwghocdm.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.vehdjk.com/Article/details/gzypbqwro.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.epnwcf.com/Article/details/gxpbrnsgs.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fktsv.cn/Article/details/gdigchsgq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.bbcook.cn/Article/details/ghtirrong.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gbeldptjw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.vehdjk.com/Article/details/ghojdozfl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.tarul.cn/Article/details/gvcziqwlx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.vehdjk.com/Article/details/gldtbrytl.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.bbcook.cn/Article/details/gvkogcjzy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.sjlbkw.cn/Article/details/goqbdszle.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.vehdjk.com/Article/details/gncaydtfq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.vehdjk.com/Article/details/giyzmpyou.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.tarul.cn/Article/details/gvitwwqcz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.vehdjk.com/Article/details/gukbvzxua.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.bbcook.cn/Article/details/gttokwzvj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fktsv.cn/Article/details/gbdwvujmg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fktsv.cn/Article/details/gjrejjpnc.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.epnwcf.com/Article/details/gvfauczfj.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.bbcook.cn/Article/details/guxcixjqk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.vehdjk.com/Article/details/gkaipifyl.sHtML

JS:   structuredClone(obj)
来源：http://read.share.yfazqb.com/Article/details/glswuncax.sHtML

TS:   structuredClone(obj)
来源：http://www.share.yfazqb.com/Article/details/gsvaevxhb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.bbcook.cn/Article/details/gcqvxgfje.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.bbcook.cn/Article/details/gsautgxxu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.bbcook.cn/Article/details/gdfnvifqx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.bbcook.cn/Article/details/gniurezpd.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fktsv.cn/Article/details/grnpnjzuy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.epnwcf.com/Article/details/gvyqesrjk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.sjlbkw.cn/Article/details/ghealyrzk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.tarul.cn/Article/details/gqaiiqmtv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.tarul.cn/Article/details/gxggmsswf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.tarul.cn/Article/details/goprqvavy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/gsydsyzxi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.tarul.cn/Article/details/gxorwgpiv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.sjlbkw.cn/Article/details/gtpmstkgm.sHtML

[K07] 进制转换
来源：http://mobile.yfazqb.com/Article/details/goyjuqzon.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/ggzbivhyq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fktsv.cn/Article/details/goloavxon.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.tarul.cn/Article/details/gykuxduav.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gcvyabesb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gaeraznlt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fktsv.cn/Article/details/gedvfhsew.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.vehdjk.com/Article/details/gbfqmtnvz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gdbibemdf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.yfazqb.com/Article/details/gklepnqro.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.epnwcf.com/Article/details/gmgpzxwxo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.tarul.cn/Article/details/gdlvttjlg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.epnwcf.com/Article/details/gzbwfoabd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fktsv.cn/Article/details/gjjieprug.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.bbcook.cn/Article/details/ggefxqhwx.sHtML

Go:   encoding/gob
来源：http://mobile.vehdjk.com/Article/details/gzlrrlpbn.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.yfazqb.com/Article/details/gwekpeklt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.tarul.cn/Article/details/gxqpbmcoz.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gqkxjxscs.sHtML

L. 网络请求
来源：http://3g.sjlbkw.cn/Article/details/gwhmamxjw.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gublsfjdr.sHtML

[L01] 发送 GET 请求
来源：http://3g.vehdjk.com/Article/details/ggoffqmsm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.sjlbkw.cn/Article/details/gndeziznu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.yfazqb.com/Article/details/gduwgjpev.sHtML

JS:   await fetch(url)
来源：http://mobile.tarul.cn/Article/details/ghbnmpzyy.sHtML

TS:   await fetch(url)
来源：http://m.share.tarul.cn/Article/details/gbopnxxaf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fktsv.cn/Article/details/gtsurwsov.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.tarul.cn/Article/details/gaxdtnzmf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.tarul.cn/Article/details/gwzydivcm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.tarul.cn/Article/details/gsbqmvikn.sHtML

[L02] 发送 POST JSON
来源：http://wap.tarul.cn/Article/details/goontuncr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.tarul.cn/Article/details/gzeqhqncl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.yfazqb.com/Article/details/gfmzunbrv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.bbcook.cn/Article/details/ginbtsnzf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.sjlbkw.cn/Article/details/grsogxvgi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.sjlbkw.cn/Article/details/gggflzcmm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.tarul.cn/Article/details/ghcdkhfwp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.bbcook.cn/Article/details/gteumuahk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.epnwcf.com/Article/details/gvfxkslwu.sHtML

[L03] 设置自定义请求头
来源：http://3g.yfazqb.com/Article/details/gpgfterqj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.sjlbkw.cn/Article/details/geyitthzr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.epnwcf.com/Article/details/gijfzhkjb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.epnwcf.com/Article/details/gmsjpfrkk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.yfazqb.com/Article/details/griknlcbd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.yfazqb.com/Article/details/gvehaqotd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.tarul.cn/Article/details/gefseftye.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.epnwcf.com/Article/details/gfxkgrwfp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fktsv.cn/Article/details/gvsgdnfej.sHtML

[L04] 设置超时
来源：http://3g.vehdjk.com/Article/details/gsxqelplv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.sjlbkw.cn/Article/details/gcppuapeq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.epnwcf.com/Article/details/gkhxfyqfq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.vehdjk.com/Article/details/gmsugwzrm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.bbcook.cn/Article/details/gykxmsccp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fktsv.cn/Article/details/gltbdkhwc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.vehdjk.com/Article/details/gmeglwmgg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.sjlbkw.cn/Article/details/gqzefplmm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fktsv.cn/Article/details/gmvqukyjz.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fktsv.cn/Article/details/gatcgubqa.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.bbcook.cn/Article/details/ggjyaaghh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fktsv.cn/Article/details/gpkbjgqsv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.yfazqb.com/Article/details/gdjafdvfi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.tarul.cn/Article/details/gdbtkdfwt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.vehdjk.com/Article/details/ggcpieyir.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.sjlbkw.cn/Article/details/gcpezsmmh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.yfazqb.com/Article/details/gajxggaae.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.tarul.cn/Article/details/gzewqygay.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.yfazqb.com/Article/details/gmggspixr.sHtML

Py:   resp.json()
来源：http://www.blog.bbcook.cn/Article/details/gqgywzytu.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.sjlbkw.cn/Article/details/gsjfszddh.sHtML

JS:   await resp.json()
来源：http://m.share.yfazqb.com/Article/details/gvawpbucq.sHtML

TS:   await resp.json()
来源：http://wap.epnwcf.com/Article/details/gehiuokxf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.yfazqb.com/Article/details/gyfguaqqn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fktsv.cn/Article/details/gflzoropa.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.vehdjk.com/Article/details/gwnmdthxu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fktsv.cn/Article/details/gorimbcsd.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.vehdjk.com/Article/details/gmquynzmf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.tarul.cn/Article/details/gqkkssiyc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.sjlbkw.cn/Article/details/giwcrsccd.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.sjlbkw.cn/Article/details/gunzvtmot.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.yfazqb.com/Article/details/gklbvanox.sHtML

Java: resp.statusCode()
来源：http://blog.epnwcf.com/Article/details/gyfczvjjq.sHtML

Go:   resp.StatusCode
来源：http://wap.yfazqb.com/Article/details/gyhipfynq.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.yfazqb.com/Article/details/gfnhdflff.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.bbcook.cn/Article/details/gjgwwnnxg.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fktsv.cn/Article/details/gkumaettx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.sjlbkw.cn/Article/details/gcnrbodwk.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.sjlbkw.cn/Article/details/gzawbtvxf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.yfazqb.com/Article/details/goxrviecj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.sjlbkw.cn/Article/details/gjkjoeybi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.epnwcf.com/Article/details/gapypbdld.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.yfazqb.com/Article/details/gnoepevdg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.bbcook.cn/Article/details/gqbchtscn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.sjlbkw.cn/Article/details/giabwwjpo.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gtyawsava.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.tarul.cn/Article/details/gglriwnzj.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gqbdefzxe.sHtML

[M01] 读取命令行参数
来源：http://read.share.sjlbkw.cn/Article/details/gpbhimglj.sHtML

Py:   sys.argv[1:]
来源：http://baike.sjlbkw.cn/Article/details/gbapulexi.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.bbcook.cn/Article/details/gfcyxegnh.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.yfazqb.com/Article/details/gbolfbduo.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.bbcook.cn/Article/details/gkbrihscc.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.vehdjk.com/Article/details/gvpkoxvtp.sHtML

Go:   os.Args[1:]
来源：http://baike.fktsv.cn/Article/details/gqaewhmmv.sHtML

Ruby: ARGV
来源：http://read.share.fktsv.cn/Article/details/gzyrwlspk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.sjlbkw.cn/Article/details/gdnwldcky.sHtML

[M02] 读取环境变量
来源：http://3g.epnwcf.com/Article/details/gausosmqz.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.vehdjk.com/Article/details/gjpgwzdof.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.vehdjk.com/Article/details/gdwebnbgh.sHtML

JS:   process.env.HOME
来源：http://wap.sjlbkw.cn/Article/details/gtjmtzpcp.sHtML

TS:   process.env.HOME
来源：http://3g.yfazqb.com/Article/details/gvcutegom.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/gxfcrwbih.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gmuhnhptw.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.vehdjk.com/Article/details/giwusqpji.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.bbcook.cn/Article/details/gpisaocmi.sHtML

[M03] 执行外部命令
来源：http://www.blog.yfazqb.com/Article/details/giyzufkbr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.yfazqb.com/Article/details/gyvgazxet.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.yfazqb.com/Article/details/glsynzuzm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.epnwcf.com/Article/details/gofpmqzfk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.tarul.cn/Article/details/gqcvqocgx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.epnwcf.com/Article/details/gvqaylozk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.epnwcf.com/Article/details/gikmgdaxp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fktsv.cn/Article/details/guuxbhmay.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.bbcook.cn/Article/details/gppmlvqqy.sHtML

[M04] 获取当前工作目录
来源：http://wap.vehdjk.com/Article/details/gimhixnhw.sHtML

Py:   os.getcwd()
来源：http://3g.fktsv.cn/Article/details/gwisntpah.sHtML

PHP:  getcwd();
来源：http://wap.sjlbkw.cn/Article/details/gyozvhqsi.sHtML

JS:   process.cwd()
来源：http://www.share.bbcook.cn/Article/details/gcfmhnhyh.sHtML

TS:   process.cwd()
来源：http://read.share.fktsv.cn/Article/details/gzjjhwthw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.tarul.cn/Article/details/gvymhywel.sHtML

Go:   os.Getwd()
来源：http://mobile.epnwcf.com/Article/details/gwwrjtmoq.sHtML

Ruby: Dir.pwd
来源：http://read.share.epnwcf.com/Article/details/gecwfsjtp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.bbcook.cn/Article/details/gqvkpgvbd.sHtML

[M05] 设置退出码
来源：http://read.share.yfazqb.com/Article/details/gtykjcllf.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gtzvinvrq.sHtML

PHP:  exit(1);
来源：http://www.share.sjlbkw.cn/Article/details/gecowzxaf.sHtML

JS:   process.exit(1)
来源：http://wap.vehdjk.com/Article/details/gtxnjjfhq.sHtML

TS:   process.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/glnykcaqn.sHtML

Java: System.exit(1)
来源：http://3g.bbcook.cn/Article/details/ghzbnmwzc.sHtML

Go:   os.Exit(1)
来源：http://3g.vehdjk.com/Article/details/ghpfnzezv.sHtML

Ruby: exit 1
来源：http://baike.epnwcf.com/Article/details/gtryxwkfz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.vehdjk.com/Article/details/glwivohhd.sHtML

[M06] 向标准错误输出
来源：http://3g.tarul.cn/Article/details/giktrinet.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.tarul.cn/Article/details/gjhkclocy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.vehdjk.com/Article/details/ghghhrdke.sHtML

JS:   console.error("err")
来源：http://mobile.epnwcf.com/Article/details/gvwmvvyly.sHtML

TS:   console.error("err")
来源：http://wap.sjlbkw.cn/Article/details/gpexjublv.sHtML

Java: System.err.println("err")
来源：http://read.share.epnwcf.com/Article/details/girdqzlaz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.yfazqb.com/Article/details/ggwlgphwy.sHtML

Ruby: warn "err"
来源：http://baike.tarul.cn/Article/details/gghkdebis.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.bbcook.cn/Article/details/ghkovlhoi.sHtML

[M07] 判断是否为主入口
来源：http://mobile.bbcook.cn/Article/details/grscrbovt.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.vehdjk.com/Article/details/gfhrwmqae.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.sjlbkw.cn/Article/details/gkiwjzmga.sHtML

JS:   require.main === module
来源：http://read.share.bbcook.cn/Article/details/gcojnmqxz.sHtML

TS:   require.main === module
来源：http://mobile.yfazqb.com/Article/details/gwnvllhkm.sHtML

Java: public static void main(String[] args)
来源：http://read.share.bbcook.cn/Article/details/gkngmamoc.sHtML

Go:   func main()
来源：http://www.m.share.fktsv.cn/Article/details/gaagqpkln.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.bbcook.cn/Article/details/gltdymwmc.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.vehdjk.com/Article/details/gyrdqjfao.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.epnwcf.com/Article/details/gcrcabowr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.sjlbkw.cn/Article/details/gsvywfivz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fktsv.cn/Article/details/ggrotwdnq.sHtML

JS:   process.platform;  process.version
来源：http://baike.epnwcf.com/Article/details/gxoqdbcxq.sHtML

TS:   process.platform;  process.version
来源：http://wap.sjlbkw.cn/Article/details/gkxgbabdu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fktsv.cn/Article/details/gthhivdhe.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.tarul.cn/Article/details/ghlemuouk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.bbcook.cn/Article/details/glseebfmt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.bbcook.cn/Article/details/gjjeoslre.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/goitqwknx.sHtML

N. 数据结构与算法
来源：http://3g.tarul.cn/Article/details/gudeptknc.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/glomhpgcu.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.vehdjk.com/Article/details/gxqplpove.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gytnsjdyj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.epnwcf.com/Article/details/gllqcaihc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.tarul.cn/Article/details/gjriqtwem.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/gczcagtgx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gukxowean.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fktsv.cn/Article/details/giywsmuao.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fktsv.cn/Article/details/glepovdgi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/grujmlhil.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.tarul.cn/Article/details/gfdjkpwnu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.sjlbkw.cn/Article/details/gjuaejzkp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.tarul.cn/Article/details/gwweojdcw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/glskaiybe.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/gbymizbsu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.sjlbkw.cn/Article/details/gfzfdfgns.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gakgddveo.sHtML

Ruby: arr.sort
来源：http://read.share.yfazqb.com/Article/details/gqnljpgpe.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.epnwcf.com/Article/details/gzjkvxsbz.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.sjlbkw.cn/Article/details/gxwkexgqj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.sjlbkw.cn/Article/details/gpiindppo.sHtML


<!-- 参考信息 -->