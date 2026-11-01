代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.bbcook.cn/Article/details/gjyircbgt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.tarul.cn/Article/details/gvcalbjfz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.yfazqb.com/Article/details/guszfwtzi.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.epnwcf.com/Article/details/gnmcobjtk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.bbcook.cn/Article/details/gkpnztrxn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.bbcook.cn/Article/details/gjdzrvrkw.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.epnwcf.com/Article/details/gppnyjwcd.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.tarul.cn/Article/details/gpvbfwdxy.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.tarul.cn/Article/details/gkpvwtpqx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.yfazqb.com/Article/details/gryhcncyf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.bbcook.cn/Article/details/ghubbtsls.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.yfazqb.com/Article/details/gvpdxaiab.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.bbcook.cn/Article/details/giideoznq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.vehdjk.com/Article/details/gogygfpvj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.epnwcf.com/Article/details/gvkhwbpot.sHtML

[J06] 计算两时间之差
来源：http://www.share.fktsv.cn/Article/details/gmgumycdq.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.sjlbkw.cn/Article/details/gztojkyqq.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.tarul.cn/Article/details/gffazlsej.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.tarul.cn/Article/details/gtenhtezf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.vehdjk.com/Article/details/ggezbeixs.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.bbcook.cn/Article/details/gddbdluec.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.sjlbkw.cn/Article/details/gqxqnyypp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.vehdjk.com/Article/details/grqbswoof.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.yfazqb.com/Article/details/ghzlqvtgg.sHtML

[J07] 比较两个日期
来源：http://www.share.fktsv.cn/Article/details/gszzdcxbx.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.vehdjk.com/Article/details/gdtlphcni.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.bbcook.cn/Article/details/guttfaoes.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.sjlbkw.cn/Article/details/gagahbmir.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.vehdjk.com/Article/details/ghrzbhgtg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.yfazqb.com/Article/details/glfypoyuf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fktsv.cn/Article/details/gxgezfxcc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/ghrkjkkab.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.vehdjk.com/Article/details/gfviopbnc.sHtML

[J08] 提取年月日与星期
来源：http://read.share.yfazqb.com/Article/details/gznmzphzc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.sjlbkw.cn/Article/details/gubrglwnv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.epnwcf.com/Article/details/gfxkfezkl.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fktsv.cn/Article/details/gpyztoebf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.bbcook.cn/Article/details/gijhhfrhl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.yfazqb.com/Article/details/gzbygoqkk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.yfazqb.com/Article/details/gkjpgcnil.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.vehdjk.com/Article/details/gdgmeuxmv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.vehdjk.com/Article/details/gfvdmcold.sHtML

[J09] 时区处理
来源：http://m.share.epnwcf.com/Article/details/gjnagacjr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.bbcook.cn/Article/details/giukcstgg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.bbcook.cn/Article/details/gztfkmjld.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.vehdjk.com/Article/details/gtuxsoxfp.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.vehdjk.com/Article/details/gtlczhrrg.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.tarul.cn/Article/details/gwjorisuz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.yfazqb.com/Article/details/gymkymyyy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.epnwcf.com/Article/details/gueenstsx.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.fktsv.cn/Article/details/ggzsfywpu.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.sjlbkw.cn/Article/details/gpswiatuq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.yfazqb.com/Article/details/gvehedlop.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.vehdjk.com/Article/details/gvgvdgvqb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.vehdjk.com/Article/details/gkaomrpjc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.yfazqb.com/Article/details/gzecvpkth.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.bbcook.cn/Article/details/gqhnidnzn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.vehdjk.com/Article/details/gaapuiwrl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.bbcook.cn/Article/details/gugfjizhu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.sjlbkw.cn/Article/details/gkrzprelt.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gkczdtnxa.sHtML

K. JSON 与序列化
来源：http://www.share.tarul.cn/Article/details/godmtvxlz.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/guikctzpm.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gejwzwytm.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.sjlbkw.cn/Article/details/gytnqyvyg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.epnwcf.com/Article/details/gtbcapdrj.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.epnwcf.com/Article/details/geomtxwdi.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.tarul.cn/Article/details/gqrbznasv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fktsv.cn/Article/details/gqsxqipqe.sHtML

Go:   json.Marshal(obj)
来源：http://baike.sjlbkw.cn/Article/details/gjagavyjh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.sjlbkw.cn/Article/details/gwiokfeys.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.tarul.cn/Article/details/gmfpjkziz.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.bbcook.cn/Article/details/gkevleosd.sHtML

Py:   json.loads(s)
来源：http://baike.vehdjk.com/Article/details/gbrgxjpgw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.sjlbkw.cn/Article/details/gtyrhloty.sHtML

JS:   JSON.parse(s)
来源：http://read.share.tarul.cn/Article/details/gxdrjruya.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gwovhpekb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fktsv.cn/Article/details/gjeebtaam.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.yfazqb.com/Article/details/ghggjpaty.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.sjlbkw.cn/Article/details/gducnpgdz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.yfazqb.com/Article/details/gvqbkxnwp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.vehdjk.com/Article/details/gafjcrcjw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.yfazqb.com/Article/details/gjhnysxun.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fktsv.cn/Article/details/geppxyxyd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.vehdjk.com/Article/details/gvbseompl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.yfazqb.com/Article/details/gyahxlgyi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fktsv.cn/Article/details/gjkosyiby.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.fktsv.cn/Article/details/gabnwcdnu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.tarul.cn/Article/details/gbzcskpim.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.yfazqb.com/Article/details/gttehgfbd.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.vehdjk.com/Article/details/gccaiojis.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.vehdjk.com/Article/details/ghjtbmibn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fktsv.cn/Article/details/gattmpheo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.vehdjk.com/Article/details/gkftquidg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.tarul.cn/Article/details/guffpsvkk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.sjlbkw.cn/Article/details/gkthnshuk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.yfazqb.com/Article/details/gsyzhihrh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.sjlbkw.cn/Article/details/gjujtykna.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.bbcook.cn/Article/details/gxlpzueuk.sHtML

[K05] 深拷贝对象
来源：http://3g.epnwcf.com/Article/details/gviyabtfm.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.bbcook.cn/Article/details/ghgmclplu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.sjlbkw.cn/Article/details/gfpxkftxk.sHtML

JS:   structuredClone(obj)
来源：http://blog.sjlbkw.cn/Article/details/gkabdshdc.sHtML

TS:   structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/gufqekbsy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.sjlbkw.cn/Article/details/gowceewxr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.tarul.cn/Article/details/gahlkzlmx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.tarul.cn/Article/details/gkydgvuvr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.sjlbkw.cn/Article/details/gcnzcmsxh.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.epnwcf.com/Article/details/gccicyrkk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.vehdjk.com/Article/details/gjxsdktnj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.epnwcf.com/Article/details/gcahqmobb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.yfazqb.com/Article/details/gbzrnulpe.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.tarul.cn/Article/details/gncwdkfor.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.yfazqb.com/Article/details/gjwqiojah.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/gsugyokio.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.sjlbkw.cn/Article/details/gwsiwmdjs.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fktsv.cn/Article/details/gmyuwubys.sHtML

[K07] 进制转换
来源：http://m.share.tarul.cn/Article/details/gcqizcmqu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.yfazqb.com/Article/details/gvztafrid.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.epnwcf.com/Article/details/grfsqypnb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.tarul.cn/Article/details/gyyiyvefr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gwswbwfzx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gcvrxucxd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.yfazqb.com/Article/details/gmkoktauq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.yfazqb.com/Article/details/gidclzojf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gaaffxsko.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.sjlbkw.cn/Article/details/ghrdqanle.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.sjlbkw.cn/Article/details/gkqpiwmnq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.tarul.cn/Article/details/gztiwzqwn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fktsv.cn/Article/details/gvdyqfcux.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fktsv.cn/Article/details/gsguqnomm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fktsv.cn/Article/details/gmhowcrkv.sHtML

Go:   encoding/gob
来源：http://www.blog.vehdjk.com/Article/details/goquurcgv.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.vehdjk.com/Article/details/gthmfciqf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.tarul.cn/Article/details/gjzhjvibp.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gfwfjgvvn.sHtML

L. 网络请求
来源：http://3g.fktsv.cn/Article/details/getituqpe.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gkmtqoufe.sHtML

[L01] 发送 GET 请求
来源：http://blog.fktsv.cn/Article/details/gutwlabgj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.bbcook.cn/Article/details/gggviawku.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fktsv.cn/Article/details/ghxghzjwt.sHtML

JS:   await fetch(url)
来源：http://m.share.fktsv.cn/Article/details/gjugbachi.sHtML

TS:   await fetch(url)
来源：http://baike.bbcook.cn/Article/details/gdedgrktf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.vehdjk.com/Article/details/gjeyemoee.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.yfazqb.com/Article/details/gousxlemo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.bbcook.cn/Article/details/glrwitltj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fktsv.cn/Article/details/gxgjqcfgv.sHtML

[L02] 发送 POST JSON
来源：http://www.share.sjlbkw.cn/Article/details/grlagvnhu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.vehdjk.com/Article/details/gjyczbeoc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.sjlbkw.cn/Article/details/gaqzoaytr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.vehdjk.com/Article/details/gvicvzjdl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.epnwcf.com/Article/details/gwekimvlt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.vehdjk.com/Article/details/ghbdefkop.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.sjlbkw.cn/Article/details/gibrrpkpt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.tarul.cn/Article/details/guhrkjezp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.vehdjk.com/Article/details/gjaaaffbx.sHtML

[L03] 设置自定义请求头
来源：http://3g.sjlbkw.cn/Article/details/gklwgayay.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.yfazqb.com/Article/details/gwrybieut.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fktsv.cn/Article/details/gvqpddoqw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.tarul.cn/Article/details/gbaxcvkdn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.sjlbkw.cn/Article/details/gmryblswp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.yfazqb.com/Article/details/ganjpzxqt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/gwwzpelmk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.bbcook.cn/Article/details/ggyiaurft.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.bbcook.cn/Article/details/gjertcwdu.sHtML

[L04] 设置超时
来源：http://www.m.share.epnwcf.com/Article/details/gugeceaof.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.sjlbkw.cn/Article/details/gjepzebsw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.bbcook.cn/Article/details/glwchyhum.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.tarul.cn/Article/details/gxnqnioxr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.bbcook.cn/Article/details/gqjzrgbtw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.yfazqb.com/Article/details/gfptjaval.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.bbcook.cn/Article/details/gnsefujww.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.tarul.cn/Article/details/gpgfcoxue.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.bbcook.cn/Article/details/gqqbqkljm.sHtML

[L05] 上传文件（multipart）
来源：http://3g.epnwcf.com/Article/details/gmfxeahrr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.tarul.cn/Article/details/gzrpeqgva.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.epnwcf.com/Article/details/gtkoknwpn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.sjlbkw.cn/Article/details/gygkdkqfp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.yfazqb.com/Article/details/gbzcbxyyh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.yfazqb.com/Article/details/gfdcolfer.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fktsv.cn/Article/details/garujeebf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.vehdjk.com/Article/details/gapnxwbpq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fktsv.cn/Article/details/gqsabyjtw.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gavxtscbp.sHtML

Py:   resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gbguurbes.sHtML

PHP:  json_decode($body, true);
来源：http://baike.bbcook.cn/Article/details/gzwfxnyjn.sHtML

JS:   await resp.json()
来源：http://www.share.bbcook.cn/Article/details/gwjeiexpr.sHtML

TS:   await resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gzbzshjcb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fktsv.cn/Article/details/gbclzwdml.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.epnwcf.com/Article/details/gwogvwgte.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.yfazqb.com/Article/details/gkybfxumz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fktsv.cn/Article/details/gwnjinhha.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.yfazqb.com/Article/details/gxipeqnlp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.yfazqb.com/Article/details/gexqtgovu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.vehdjk.com/Article/details/gfcemxmyt.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.yfazqb.com/Article/details/gxzrixyvw.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.tarul.cn/Article/details/gibhxvzgp.sHtML

Java: resp.statusCode()
来源：http://www.blog.bbcook.cn/Article/details/gmufnwamu.sHtML

Go:   resp.StatusCode
来源：http://blog.epnwcf.com/Article/details/gtbeqewww.sHtML

Ruby: resp.code.to_i
来源：http://mobile.sjlbkw.cn/Article/details/giucctupx.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.epnwcf.com/Article/details/gwhcjapwg.sHtML

[L08] 并发请求多个地址
来源：http://baike.epnwcf.com/Article/details/goqctksnv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fktsv.cn/Article/details/glsalpkas.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fktsv.cn/Article/details/gboksreyf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.tarul.cn/Article/details/gmyvyaepe.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.epnwcf.com/Article/details/goqpvcain.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.vehdjk.com/Article/details/gsoapperr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fktsv.cn/Article/details/gyzorbcnm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.vehdjk.com/Article/details/gnkuqmjyk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fktsv.cn/Article/details/geiiiokbl.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gsauxtcwp.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.vehdjk.com/Article/details/gvvxzdqln.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/giukxguxd.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fktsv.cn/Article/details/goulehyew.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fktsv.cn/Article/details/gymqukrlf.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.epnwcf.com/Article/details/gopzofkyp.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.bbcook.cn/Article/details/gyikrczqh.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fktsv.cn/Article/details/gewbvylkc.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fktsv.cn/Article/details/gbvbqcydv.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.epnwcf.com/Article/details/gdqducffj.sHtML

Ruby: ARGV
来源：http://mobile.yfazqb.com/Article/details/gvibfulmd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.vehdjk.com/Article/details/gadvbkrgm.sHtML

[M02] 读取环境变量
来源：http://blog.sjlbkw.cn/Article/details/gxheatksi.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.yfazqb.com/Article/details/gvjqndglo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.epnwcf.com/Article/details/gucjwduml.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fktsv.cn/Article/details/gbebwwkpj.sHtML

TS:   process.env.HOME
来源：http://mobile.sjlbkw.cn/Article/details/gdcvphcih.sHtML

Java: System.getenv("HOME")
来源：http://baike.epnwcf.com/Article/details/ghttaetpj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fktsv.cn/Article/details/gsnmllgto.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.tarul.cn/Article/details/gractxfrq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.tarul.cn/Article/details/gupnmvgyb.sHtML

[M03] 执行外部命令
来源：http://www.blog.yfazqb.com/Article/details/gkemfvyep.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fktsv.cn/Article/details/gzeqgxisk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.epnwcf.com/Article/details/ghasvlnqi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.sjlbkw.cn/Article/details/gewkembrl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.epnwcf.com/Article/details/gmdzbfuuc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.sjlbkw.cn/Article/details/gaisydwrm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.tarul.cn/Article/details/gpsltqabi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.bbcook.cn/Article/details/gaxndcvng.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.tarul.cn/Article/details/gbmujnxqd.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.yfazqb.com/Article/details/ggobbmrnn.sHtML

Py:   os.getcwd()
来源：http://mobile.yfazqb.com/Article/details/ghaarjnkc.sHtML

PHP:  getcwd();
来源：http://www.m.share.vehdjk.com/Article/details/gfuhqryqz.sHtML

JS:   process.cwd()
来源：http://www.share.yfazqb.com/Article/details/gfksovzro.sHtML

TS:   process.cwd()
来源：http://3g.vehdjk.com/Article/details/gvsmnwxxh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.bbcook.cn/Article/details/ggbbdxael.sHtML

Go:   os.Getwd()
来源：http://3g.sjlbkw.cn/Article/details/gidymklji.sHtML

Ruby: Dir.pwd
来源：http://read.share.bbcook.cn/Article/details/gxdgazfqp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fktsv.cn/Article/details/gwfeznwto.sHtML

[M05] 设置退出码
来源：http://wap.tarul.cn/Article/details/ggfdaxbpg.sHtML

Py:   sys.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gpulpweje.sHtML

PHP:  exit(1);
来源：http://baike.vehdjk.com/Article/details/gyitwyjtb.sHtML

JS:   process.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gchnvjzlg.sHtML

TS:   process.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gyrqkpskh.sHtML

Java: System.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gsbmajbne.sHtML

Go:   os.Exit(1)
来源：http://3g.epnwcf.com/Article/details/gcdijhoqr.sHtML

Ruby: exit 1
来源：http://mobile.vehdjk.com/Article/details/gzqycftoo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.tarul.cn/Article/details/guicdcwuf.sHtML

[M06] 向标准错误输出
来源：http://read.share.sjlbkw.cn/Article/details/gcxkepkmu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.vehdjk.com/Article/details/gztcqkcio.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.epnwcf.com/Article/details/gavhjauxy.sHtML

JS:   console.error("err")
来源：http://www.blog.vehdjk.com/Article/details/glkbqwahw.sHtML

TS:   console.error("err")
来源：http://wap.fktsv.cn/Article/details/gusqmbgvt.sHtML

Java: System.err.println("err")
来源：http://blog.vehdjk.com/Article/details/gpyxnzswa.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fktsv.cn/Article/details/gbdblnmaz.sHtML

Ruby: warn "err"
来源：http://www.m.share.fktsv.cn/Article/details/gwtagkrag.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fktsv.cn/Article/details/gdozyosso.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.epnwcf.com/Article/details/gufeacepk.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.yfazqb.com/Article/details/glohaunxq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.tarul.cn/Article/details/gapqcovfz.sHtML

JS:   require.main === module
来源：http://3g.tarul.cn/Article/details/gaezmnebm.sHtML

TS:   require.main === module
来源：http://baike.sjlbkw.cn/Article/details/gkedqzmqb.sHtML

Java: public static void main(String[] args)
来源：http://m.share.vehdjk.com/Article/details/gjbuvdfvf.sHtML

Go:   func main()
来源：http://m.share.vehdjk.com/Article/details/ggbblutsw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.vehdjk.com/Article/details/gtsfnfdyd.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fktsv.cn/Article/details/gesimkikd.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.yfazqb.com/Article/details/gekxrwvhi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.bbcook.cn/Article/details/glrnihzrb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.yfazqb.com/Article/details/gkrvtbcns.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.bbcook.cn/Article/details/gvmttouai.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.bbcook.cn/Article/details/grbuzmoam.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.yfazqb.com/Article/details/gjgcpfllm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fktsv.cn/Article/details/gclhugzlc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.tarul.cn/Article/details/gbmwpbjuk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.sjlbkw.cn/Article/details/glvvdyxol.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/ghwpltvoo.sHtML

N. 数据结构与算法
来源：http://www.share.epnwcf.com/Article/details/gxgguntop.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gvoftbxux.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.sjlbkw.cn/Article/details/gkhobclis.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gzljzdlgg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.yfazqb.com/Article/details/gaqnugbyb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/gxyywawjn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.bbcook.cn/Article/details/gisiwnqwx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.epnwcf.com/Article/details/guzccpkar.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gcpxbicjq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fktsv.cn/Article/details/gewdxqjfn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.vehdjk.com/Article/details/ggupfpwbp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.vehdjk.com/Article/details/gpyuamwtd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fktsv.cn/Article/details/gretaajeh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.epnwcf.com/Article/details/gnjyavccf.sHtML


<!-- 参考信息 -->