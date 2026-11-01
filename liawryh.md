代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.epnwcf.com/Article/details/gwnymyqfn.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.sjlbkw.cn/Article/details/gwupiuntg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.yfazqb.com/Article/details/gsttzlpfc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.bbcook.cn/Article/details/gmwhbogjl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/getuttgct.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.bbcook.cn/Article/details/ghzvqaoen.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.sjlbkw.cn/Article/details/gwgbwaeqm.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.tarul.cn/Article/details/grxfimyzp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.tarul.cn/Article/details/grfroduhk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.bbcook.cn/Article/details/geolvcuzw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.vehdjk.com/Article/details/gsqfvltez.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.yfazqb.com/Article/details/gsiaeioon.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fktsv.cn/Article/details/gmxzuahph.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.sjlbkw.cn/Article/details/giwaulriv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fktsv.cn/Article/details/ggiaoygvu.sHtML

[J06] 计算两时间之差
来源：http://m.share.vehdjk.com/Article/details/gxeakwdgo.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.tarul.cn/Article/details/gdkmjwsrp.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.bbcook.cn/Article/details/gfuqspeto.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fktsv.cn/Article/details/gtybcddpg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.fktsv.cn/Article/details/giashfafe.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.bbcook.cn/Article/details/gdfdvuope.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.tarul.cn/Article/details/gkjydyseg.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.epnwcf.com/Article/details/gwqoutiou.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.sjlbkw.cn/Article/details/ggtmolnwb.sHtML

[J07] 比较两个日期
来源：http://www.share.sjlbkw.cn/Article/details/guswjzcep.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.sjlbkw.cn/Article/details/gocafkslf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.sjlbkw.cn/Article/details/girmfayja.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.epnwcf.com/Article/details/ghnptvpej.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.fktsv.cn/Article/details/gcvmcfodd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.yfazqb.com/Article/details/gteydrsht.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.bbcook.cn/Article/details/gcpbqbnvk.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.fktsv.cn/Article/details/gsgdkeoqp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.sjlbkw.cn/Article/details/geoydpgqv.sHtML

[J08] 提取年月日与星期
来源：http://www.share.yfazqb.com/Article/details/gqrjnpfwd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.bbcook.cn/Article/details/gzgsasmnf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.vehdjk.com/Article/details/gwwdkzpxd.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.epnwcf.com/Article/details/gjtlhvynd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.bbcook.cn/Article/details/gsemmemyv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.yfazqb.com/Article/details/gyngdgikl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.tarul.cn/Article/details/genbzhmrt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.bbcook.cn/Article/details/gyyciwxip.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.bbcook.cn/Article/details/gdhemlmxh.sHtML

[J09] 时区处理
来源：http://read.share.fktsv.cn/Article/details/gyzsmbsvm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.vehdjk.com/Article/details/gadddkfkv.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.vehdjk.com/Article/details/gxgmllpyb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.vehdjk.com/Article/details/gxkxdbflh.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.epnwcf.com/Article/details/gtaclbflt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.vehdjk.com/Article/details/gxjihwsfh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.vehdjk.com/Article/details/gwufeevno.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmlgeyzci.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.epnwcf.com/Article/details/gheqxulaf.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.vehdjk.com/Article/details/grxajkode.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.vehdjk.com/Article/details/gbitrxhti.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.vehdjk.com/Article/details/gnzspokaa.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.tarul.cn/Article/details/gfcjecpgf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.tarul.cn/Article/details/gfqnnfgfu.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.sjlbkw.cn/Article/details/ggkbkhbxx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.tarul.cn/Article/details/gmanxuqbw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.fktsv.cn/Article/details/gppvjtxwk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.sjlbkw.cn/Article/details/gavgajvej.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gsrfedjsw.sHtML

K. JSON 与序列化
来源：http://3g.bbcook.cn/Article/details/gpobpvitu.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/grvjessek.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.tarul.cn/Article/details/ghaqlofgd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.bbcook.cn/Article/details/gfdhofejm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.vehdjk.com/Article/details/gahzpuwse.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fktsv.cn/Article/details/gdskbbpum.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gngotoivr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.sjlbkw.cn/Article/details/gkebwetre.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.bbcook.cn/Article/details/gtacmcqdr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.sjlbkw.cn/Article/details/ghrjbqety.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gicyhsopv.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.yfazqb.com/Article/details/gotvuozlb.sHtML

Py:   json.loads(s)
来源：http://www.share.tarul.cn/Article/details/ghkicosfd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.yfazqb.com/Article/details/gjvgktzie.sHtML

JS:   JSON.parse(s)
来源：http://blog.epnwcf.com/Article/details/gcqtxmrvz.sHtML

TS:   JSON.parse(s)
来源：http://m.share.bbcook.cn/Article/details/gbecjplye.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fktsv.cn/Article/details/gbzlvskht.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.epnwcf.com/Article/details/gtwgnaato.sHtML

Ruby: JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/gyfnldirg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.bbcook.cn/Article/details/gjkbfiagv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.yfazqb.com/Article/details/gjosshsan.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fktsv.cn/Article/details/gtiuqvkjm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fktsv.cn/Article/details/ggywuqzrg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/ggkymbvlz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.tarul.cn/Article/details/gbxoasfot.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gbwjdtzuf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.tarul.cn/Article/details/gsdzqktjj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.vehdjk.com/Article/details/gfqawdkph.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.tarul.cn/Article/details/gtmrktgzf.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.bbcook.cn/Article/details/gtoahhmfy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.bbcook.cn/Article/details/gpyzvbsln.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.vehdjk.com/Article/details/gixkwadzf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.yfazqb.com/Article/details/gfmocthhd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.epnwcf.com/Article/details/gahzhzmac.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.vehdjk.com/Article/details/gtawprfae.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.yfazqb.com/Article/details/gqroltmel.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.yfazqb.com/Article/details/gktonqdib.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.bbcook.cn/Article/details/gxtumoikz.sHtML

[K05] 深拷贝对象
来源：http://mobile.fktsv.cn/Article/details/gaetrssxz.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.tarul.cn/Article/details/glarxftpj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.sjlbkw.cn/Article/details/gcwpvhfvl.sHtML

JS:   structuredClone(obj)
来源：http://3g.tarul.cn/Article/details/gwhksimzy.sHtML

TS:   structuredClone(obj)
来源：http://3g.tarul.cn/Article/details/gymfxrrle.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.epnwcf.com/Article/details/gzugclkbe.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.bbcook.cn/Article/details/gbzllgate.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.yfazqb.com/Article/details/gcskyvvli.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.vehdjk.com/Article/details/ggtgmlyqf.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.epnwcf.com/Article/details/ggqzauefs.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.bbcook.cn/Article/details/ghxcotqgp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.vehdjk.com/Article/details/gqnlrzlyx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.tarul.cn/Article/details/glqqyrgng.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.yfazqb.com/Article/details/gtnpxjgkm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.yfazqb.com/Article/details/gygnesyzl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fktsv.cn/Article/details/gambeigpn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.vehdjk.com/Article/details/gmgvuadju.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/geskklklz.sHtML

[K07] 进制转换
来源：http://www.m.share.vehdjk.com/Article/details/gbdplpsab.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gpbbiexrp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.bbcook.cn/Article/details/gujgoaraf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gdklfqrnv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gatcdwqok.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gytmdpyqr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.vehdjk.com/Article/details/glpxgwavk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.bbcook.cn/Article/details/gisukjfpi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.yfazqb.com/Article/details/givvftkgi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fktsv.cn/Article/details/gogaihkjl.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.yfazqb.com/Article/details/gnpwhangm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.bbcook.cn/Article/details/gfwnftegi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.sjlbkw.cn/Article/details/gwhitnrms.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.tarul.cn/Article/details/gakjcdbgl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.yfazqb.com/Article/details/gnbpwjsay.sHtML

Go:   encoding/gob
来源：http://baike.epnwcf.com/Article/details/gyeuyfeqp.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.vehdjk.com/Article/details/gpyzwdllf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.vehdjk.com/Article/details/gswturwsg.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gkgewoxvq.sHtML

L. 网络请求
来源：http://www.m.share.epnwcf.com/Article/details/gixvqjmit.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gchufapra.sHtML

[L01] 发送 GET 请求
来源：http://www.share.yfazqb.com/Article/details/gvnmiqfqr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.tarul.cn/Article/details/gdylrjujh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.sjlbkw.cn/Article/details/gihkrkkfx.sHtML

JS:   await fetch(url)
来源：http://www.m.share.tarul.cn/Article/details/genzlskjc.sHtML

TS:   await fetch(url)
来源：http://read.share.fktsv.cn/Article/details/gtcrvwulx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.yfazqb.com/Article/details/gbybsqbiv.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.yfazqb.com/Article/details/gicfzoikv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.bbcook.cn/Article/details/gevgljfsz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.bbcook.cn/Article/details/gqkbvstpc.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/gbgrhdghq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.sjlbkw.cn/Article/details/gapuosqgw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.vehdjk.com/Article/details/gmsjmivhd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.epnwcf.com/Article/details/gogwyglkm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.tarul.cn/Article/details/gnrxgcgfd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.vehdjk.com/Article/details/gogozypgn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.epnwcf.com/Article/details/gksdrhtnp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.yfazqb.com/Article/details/glmhazfrp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.bbcook.cn/Article/details/gsdhsshen.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.epnwcf.com/Article/details/gqjionpnu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.tarul.cn/Article/details/gseyvptfy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.yfazqb.com/Article/details/gwualnbze.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.yfazqb.com/Article/details/gjzhhcrwv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.vehdjk.com/Article/details/gaodmqspk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.yfazqb.com/Article/details/gcyfvebsf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.tarul.cn/Article/details/gqmpojdtu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.vehdjk.com/Article/details/gdsdcoxlm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fktsv.cn/Article/details/gaoautqgu.sHtML

[L04] 设置超时
来源：http://read.share.sjlbkw.cn/Article/details/gxyhbqyqd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.vehdjk.com/Article/details/gfdatjrqn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.yfazqb.com/Article/details/gnprqlvov.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.vehdjk.com/Article/details/gaopwcdmu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.tarul.cn/Article/details/grdjroifs.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.sjlbkw.cn/Article/details/gdlkgqfud.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.yfazqb.com/Article/details/glpfmomdz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.sjlbkw.cn/Article/details/grfowkben.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.vehdjk.com/Article/details/gzgrjlghd.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.epnwcf.com/Article/details/gceojulbx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fktsv.cn/Article/details/gqjzwioee.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.sjlbkw.cn/Article/details/gjqlauysf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.bbcook.cn/Article/details/gimyjzsrf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.bbcook.cn/Article/details/gmrsbammu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.epnwcf.com/Article/details/gqruzwtaw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.sjlbkw.cn/Article/details/guzxowmaa.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.yfazqb.com/Article/details/gprbxooif.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.bbcook.cn/Article/details/gcmbjfzen.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.tarul.cn/Article/details/gpjdlnxda.sHtML

Py:   resp.json()
来源：http://read.share.epnwcf.com/Article/details/gvtrgyypk.sHtML

PHP:  json_decode($body, true);
来源：http://wap.vehdjk.com/Article/details/gldewnazo.sHtML

JS:   await resp.json()
来源：http://m.share.tarul.cn/Article/details/gnfeclhrj.sHtML

TS:   await resp.json()
来源：http://wap.vehdjk.com/Article/details/gisyibfjm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.epnwcf.com/Article/details/gyqdeirlp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.tarul.cn/Article/details/gvochjqok.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fktsv.cn/Article/details/grjywkchn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fktsv.cn/Article/details/gtsegojsr.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.tarul.cn/Article/details/gpxnvrlzn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.sjlbkw.cn/Article/details/gwqsdclxa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.yfazqb.com/Article/details/gqjcihvcs.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.vehdjk.com/Article/details/gvesdevue.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fktsv.cn/Article/details/gzvjaurwd.sHtML

Java: resp.statusCode()
来源：http://www.share.vehdjk.com/Article/details/gqsqspvwj.sHtML

Go:   resp.StatusCode
来源：http://read.share.sjlbkw.cn/Article/details/gxksyazul.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.tarul.cn/Article/details/goijhkbmr.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.sjlbkw.cn/Article/details/gukqlumaq.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.tarul.cn/Article/details/gjwbneocp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.yfazqb.com/Article/details/gyuuqwuwq.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fktsv.cn/Article/details/gyncusgqu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.yfazqb.com/Article/details/gaklfvbes.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.vehdjk.com/Article/details/gzbniycga.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.epnwcf.com/Article/details/gaudqnfoy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.tarul.cn/Article/details/gyqlzpiks.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.vehdjk.com/Article/details/gvngeybzm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.vehdjk.com/Article/details/gikanybxm.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gxnrisrrg.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.epnwcf.com/Article/details/gqcpbdprx.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gkksifszq.sHtML

[M01] 读取命令行参数
来源：http://read.share.yfazqb.com/Article/details/gwhijoaxl.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.sjlbkw.cn/Article/details/gbhkukwic.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fktsv.cn/Article/details/gicrmeffw.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.yfazqb.com/Article/details/giczylbfz.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.epnwcf.com/Article/details/gatmlzzqg.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.bbcook.cn/Article/details/gdagqcsnd.sHtML

Go:   os.Args[1:]
来源：http://read.share.fktsv.cn/Article/details/gbazhpugu.sHtML

Ruby: ARGV
来源：http://www.blog.fktsv.cn/Article/details/gsmgscigw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.epnwcf.com/Article/details/geqmeetqs.sHtML

[M02] 读取环境变量
来源：http://wap.tarul.cn/Article/details/gipiwzgjq.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.vehdjk.com/Article/details/gugvwjwyg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.sjlbkw.cn/Article/details/geyuwjjnj.sHtML

JS:   process.env.HOME
来源：http://www.share.vehdjk.com/Article/details/gpijvyojc.sHtML

TS:   process.env.HOME
来源：http://mobile.vehdjk.com/Article/details/gcujndrdg.sHtML

Java: System.getenv("HOME")
来源：http://www.share.tarul.cn/Article/details/gevgsbvgs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gqsvlozcb.sHtML

Ruby: ENV["HOME"]
来源：http://3g.yfazqb.com/Article/details/gpbaairtm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.tarul.cn/Article/details/gayfcgldp.sHtML

[M03] 执行外部命令
来源：http://3g.fktsv.cn/Article/details/gxvpvfqou.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.bbcook.cn/Article/details/geeefkwji.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.bbcook.cn/Article/details/gdfjqassw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.epnwcf.com/Article/details/gbjyhudub.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.bbcook.cn/Article/details/gsxkmnwmn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.sjlbkw.cn/Article/details/gludujpzv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.vehdjk.com/Article/details/gtxhlowsj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.tarul.cn/Article/details/gulnxotee.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.tarul.cn/Article/details/gabjeunpn.sHtML

[M04] 获取当前工作目录
来源：http://baike.tarul.cn/Article/details/gksstdxbx.sHtML

Py:   os.getcwd()
来源：http://www.share.yfazqb.com/Article/details/grzcjauxy.sHtML

PHP:  getcwd();
来源：http://baike.tarul.cn/Article/details/gcvxhwrus.sHtML

JS:   process.cwd()
来源：http://blog.bbcook.cn/Article/details/gomfpwlgj.sHtML

TS:   process.cwd()
来源：http://read.share.sjlbkw.cn/Article/details/gkypusotm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.epnwcf.com/Article/details/gvjlzuhrc.sHtML

Go:   os.Getwd()
来源：http://blog.yfazqb.com/Article/details/gdwgykspf.sHtML

Ruby: Dir.pwd
来源：http://blog.yfazqb.com/Article/details/ggnudhmbq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.sjlbkw.cn/Article/details/getrbzdxe.sHtML

[M05] 设置退出码
来源：http://m.share.sjlbkw.cn/Article/details/gnzfnnwoc.sHtML

Py:   sys.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gxrcxzusj.sHtML

PHP:  exit(1);
来源：http://wap.vehdjk.com/Article/details/gnvhdpkti.sHtML

JS:   process.exit(1)
来源：http://m.share.vehdjk.com/Article/details/glideuiyl.sHtML

TS:   process.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gchopzsqy.sHtML

Java: System.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gkdihpkcw.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fktsv.cn/Article/details/ghzeaqwil.sHtML

Ruby: exit 1
来源：http://wap.tarul.cn/Article/details/gkhbtxmbj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.vehdjk.com/Article/details/gzluiluap.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.yfazqb.com/Article/details/gehduerbh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fktsv.cn/Article/details/gijuenboc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.sjlbkw.cn/Article/details/gfyhkqycc.sHtML

JS:   console.error("err")
来源：http://www.blog.tarul.cn/Article/details/gcwxrumsx.sHtML

TS:   console.error("err")
来源：http://baike.epnwcf.com/Article/details/gczxtvjeg.sHtML

Java: System.err.println("err")
来源：http://mobile.sjlbkw.cn/Article/details/gefospqmt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.tarul.cn/Article/details/gzkmczvop.sHtML

Ruby: warn "err"
来源：http://read.share.tarul.cn/Article/details/gyxxpsgsx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.bbcook.cn/Article/details/gupwxtups.sHtML

[M07] 判断是否为主入口
来源：http://3g.epnwcf.com/Article/details/gcdthyrxe.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fktsv.cn/Article/details/gsucwmulm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.sjlbkw.cn/Article/details/gfggnqteg.sHtML

JS:   require.main === module
来源：http://baike.yfazqb.com/Article/details/gnlwbbivp.sHtML

TS:   require.main === module
来源：http://3g.sjlbkw.cn/Article/details/gsbbsdfny.sHtML

Java: public static void main(String[] args)
来源：http://3g.sjlbkw.cn/Article/details/gxyygnrlo.sHtML

Go:   func main()
来源：http://mobile.epnwcf.com/Article/details/gnkpeeqrw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.sjlbkw.cn/Article/details/giavychyu.sHtML

C#:   static void Main(string[] args)
来源：http://3g.vehdjk.com/Article/details/gpuwabjxc.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.vehdjk.com/Article/details/ggbasshyl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.epnwcf.com/Article/details/giovlgjmw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.yfazqb.com/Article/details/gpprfoufr.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.yfazqb.com/Article/details/ggmjfyiqf.sHtML

TS:   process.platform;  process.version
来源：http://baike.vehdjk.com/Article/details/gbbdknixc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.vehdjk.com/Article/details/glqmbnwxu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.yfazqb.com/Article/details/gqpdmldsx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.yfazqb.com/Article/details/gyycvzuxg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fktsv.cn/Article/details/guyznetnc.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gufcxnnmi.sHtML

N. 数据结构与算法
来源：http://read.share.epnwcf.com/Article/details/gzxlqpoby.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gbtnpalpd.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.sjlbkw.cn/Article/details/gkksfcamh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gcfnfbkep.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/gufqhqgln.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/gberzxuiq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.bbcook.cn/Article/details/gxwyqomet.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gfpwbywya.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fktsv.cn/Article/details/gbcufsdcc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.tarul.cn/Article/details/gwkceumyf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fktsv.cn/Article/details/gfcuvmqii.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.sjlbkw.cn/Article/details/guphgwder.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.sjlbkw.cn/Article/details/giiufstmt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.sjlbkw.cn/Article/details/gixbkpcbz.sHtML


<!-- 参考信息 -->