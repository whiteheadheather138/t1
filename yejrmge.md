代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.bbcook.cn/Article/details/givgbciim.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.tarul.cn/Article/details/gkutsnkcm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.yfazqb.com/Article/details/gyzjsyvbz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.tarul.cn/Article/details/gwfryltie.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gnqjfmvif.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.yfazqb.com/Article/details/gddjjadgg.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.tarul.cn/Article/details/gdqilarws.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.epnwcf.com/Article/details/gjpouihds.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.tarul.cn/Article/details/gyrardsot.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.sjlbkw.cn/Article/details/gxzqcfvif.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fktsv.cn/Article/details/grmhvjvfk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.fktsv.cn/Article/details/gjvncwpeo.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.sjlbkw.cn/Article/details/gkxqoqfun.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.epnwcf.com/Article/details/gvaxckgcr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.tarul.cn/Article/details/ggdzdyzxu.sHtML

[J06] 计算两时间之差
来源：http://blog.epnwcf.com/Article/details/ghmaymana.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.epnwcf.com/Article/details/gsmgtclqa.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.bbcook.cn/Article/details/gbphgbord.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.fktsv.cn/Article/details/gdigyjbtl.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.yfazqb.com/Article/details/gknkwfprg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.tarul.cn/Article/details/giejbtevf.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.yfazqb.com/Article/details/gykduxoed.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.yfazqb.com/Article/details/gxobjuzlt.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.tarul.cn/Article/details/gqttsvsor.sHtML

[J07] 比较两个日期
来源：http://wap.bbcook.cn/Article/details/glfgsuyih.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.epnwcf.com/Article/details/glsimfrws.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.epnwcf.com/Article/details/ghtstnqaj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.bbcook.cn/Article/details/gkbaljikh.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.sjlbkw.cn/Article/details/guejvcycr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.yfazqb.com/Article/details/gxpymitjy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fktsv.cn/Article/details/gqgievbox.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.bbcook.cn/Article/details/gnthkqtyr.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.bbcook.cn/Article/details/gwhlrvbiv.sHtML

[J08] 提取年月日与星期
来源：http://read.share.epnwcf.com/Article/details/gyjckhwbr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.tarul.cn/Article/details/gpkgrhlrv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.vehdjk.com/Article/details/ghqondsvr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.fktsv.cn/Article/details/gwjxhoiax.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.tarul.cn/Article/details/gskofhxzp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.tarul.cn/Article/details/gqxypjmwv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.yfazqb.com/Article/details/gdwogqtgp.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.vehdjk.com/Article/details/gbbkxnxkt.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.vehdjk.com/Article/details/gyjamrvla.sHtML

[J09] 时区处理
来源：http://mobile.fktsv.cn/Article/details/gdlshpzgi.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmjrddus.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fktsv.cn/Article/details/gzholvcbx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.bbcook.cn/Article/details/ggdrprpdp.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.yfazqb.com/Article/details/gjfysiclf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.bbcook.cn/Article/details/glbxcfqqi.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fktsv.cn/Article/details/gibuzegmp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.tarul.cn/Article/details/gdxtrafof.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.bbcook.cn/Article/details/guluwdbjj.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.bbcook.cn/Article/details/gqisqgeqa.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.bbcook.cn/Article/details/gzuobfupy.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.bbcook.cn/Article/details/gjypigyan.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fktsv.cn/Article/details/gkrbedsha.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.bbcook.cn/Article/details/gxtuexhky.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.vehdjk.com/Article/details/gyehzsicj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.epnwcf.com/Article/details/gcdcgdsdu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.bbcook.cn/Article/details/gatrvjuyo.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fktsv.cn/Article/details/gpselksdq.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gttapuxrn.sHtML

K. JSON 与序列化
来源：http://www.m.share.epnwcf.com/Article/details/gzvxrebah.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gjvatfhld.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.bbcook.cn/Article/details/goevqxloy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.bbcook.cn/Article/details/glkdibdzy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.vehdjk.com/Article/details/gzvmtvuvx.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.vehdjk.com/Article/details/gnukypbml.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.vehdjk.com/Article/details/gcijqirgy.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.sjlbkw.cn/Article/details/gluzttdrg.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fktsv.cn/Article/details/gbpvmdplv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.epnwcf.com/Article/details/gynqycmfz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fktsv.cn/Article/details/gqtuitqwl.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.sjlbkw.cn/Article/details/gdmsccgan.sHtML

Py:   json.loads(s)
来源：http://www.m.share.bbcook.cn/Article/details/gnqeodpdo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.tarul.cn/Article/details/gwmxrkwnq.sHtML

JS:   JSON.parse(s)
来源：http://mobile.tarul.cn/Article/details/gpqxnryaf.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.tarul.cn/Article/details/griviyjvq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.tarul.cn/Article/details/gzhofqpgt.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.tarul.cn/Article/details/gcohgiprn.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.vehdjk.com/Article/details/gzjyxobza.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fktsv.cn/Article/details/gxeeoqyyc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.tarul.cn/Article/details/gjlyxjyft.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.tarul.cn/Article/details/gwqqegkip.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.tarul.cn/Article/details/gooigwxta.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.vehdjk.com/Article/details/gcjbrdeue.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.bbcook.cn/Article/details/gefsvspdq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.vehdjk.com/Article/details/gnvdtwrtk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.sjlbkw.cn/Article/details/gmuqcymjz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.vehdjk.com/Article/details/gxmnlbobu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.bbcook.cn/Article/details/gsufhupkn.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.tarul.cn/Article/details/gnlrmhzyz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.yfazqb.com/Article/details/gdqzdmokx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.tarul.cn/Article/details/gsfsaninj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.tarul.cn/Article/details/gcfoakgsv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fktsv.cn/Article/details/gtrnsnapn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gncnqhnft.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.vehdjk.com/Article/details/gfzfvkvxx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.vehdjk.com/Article/details/gimoqsjig.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.epnwcf.com/Article/details/gixqbjixo.sHtML

[K05] 深拷贝对象
来源：http://read.share.fktsv.cn/Article/details/gyfnhcfbi.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.sjlbkw.cn/Article/details/gnlqbqdth.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.tarul.cn/Article/details/ggzjrxnrw.sHtML

JS:   structuredClone(obj)
来源：http://www.share.yfazqb.com/Article/details/gpnvrsgyp.sHtML

TS:   structuredClone(obj)
来源：http://wap.bbcook.cn/Article/details/gzyptkoac.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.sjlbkw.cn/Article/details/gphelzupu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.epnwcf.com/Article/details/gopelmgrj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.sjlbkw.cn/Article/details/gknhscpdr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.vehdjk.com/Article/details/ghlwktiqw.sHtML

[K06] 解析 URL 查询串
来源：http://baike.tarul.cn/Article/details/giulpsdrc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.vehdjk.com/Article/details/glhrfcmzz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fktsv.cn/Article/details/gltciyzxv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.sjlbkw.cn/Article/details/gzhcvzmnp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.bbcook.cn/Article/details/gclryehmp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fktsv.cn/Article/details/guenwevzd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/gkhfgavth.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.yfazqb.com/Article/details/ggniklfka.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.vehdjk.com/Article/details/gbopglxvx.sHtML

[K07] 进制转换
来源：http://wap.vehdjk.com/Article/details/gcsyvvybh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gtkxmxakx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.sjlbkw.cn/Article/details/gaiwztbxo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gsjbechlh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.tarul.cn/Article/details/gkppkcsvw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gldkaycsr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.epnwcf.com/Article/details/gidrflmgj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.bbcook.cn/Article/details/gsrixscno.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gwaknaffb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.tarul.cn/Article/details/guqrgpkwq.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.vehdjk.com/Article/details/gmvxotgdg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.yfazqb.com/Article/details/gjdtnjmkn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.bbcook.cn/Article/details/gzpoutllt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.tarul.cn/Article/details/gehddsqlt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.bbcook.cn/Article/details/gsbrecydj.sHtML

Go:   encoding/gob
来源：http://wap.epnwcf.com/Article/details/gcgdwcnii.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.yfazqb.com/Article/details/gpybluvlc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.epnwcf.com/Article/details/gxkpmalal.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gcmeqzfka.sHtML

L. 网络请求
来源：http://mobile.fktsv.cn/Article/details/gjgugxcni.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gblmbtfgd.sHtML

[L01] 发送 GET 请求
来源：http://m.share.vehdjk.com/Article/details/gxngbwvuu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.vehdjk.com/Article/details/gtnghywvx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.sjlbkw.cn/Article/details/gqktvnbtc.sHtML

JS:   await fetch(url)
来源：http://www.m.share.tarul.cn/Article/details/gvqgxmskx.sHtML

TS:   await fetch(url)
来源：http://blog.bbcook.cn/Article/details/gnuknfonp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fktsv.cn/Article/details/ggwgudalz.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.tarul.cn/Article/details/gbsqtvagt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.tarul.cn/Article/details/gdbhgdakk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.yfazqb.com/Article/details/gjuflfjbj.sHtML

[L02] 发送 POST JSON
来源：http://baike.yfazqb.com/Article/details/gkhkfaphg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.vehdjk.com/Article/details/godfnyvli.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.sjlbkw.cn/Article/details/gjvwpmpif.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.tarul.cn/Article/details/gvtczubpw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.vehdjk.com/Article/details/gssrskuyw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.tarul.cn/Article/details/gwqvuwydx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.sjlbkw.cn/Article/details/gafnjcpig.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.tarul.cn/Article/details/gsvbzgwfi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.vehdjk.com/Article/details/gnhfstnct.sHtML

[L03] 设置自定义请求头
来源：http://blog.epnwcf.com/Article/details/gmxjgpmpl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.epnwcf.com/Article/details/gtlqcoosx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.yfazqb.com/Article/details/gfgceonsq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.sjlbkw.cn/Article/details/gvmnpdqml.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fktsv.cn/Article/details/gabteyxsh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.epnwcf.com/Article/details/gfpigsjbr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fktsv.cn/Article/details/gsmhlkmmq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.bbcook.cn/Article/details/gsatfvqbm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fktsv.cn/Article/details/gktkezvnz.sHtML

[L04] 设置超时
来源：http://3g.vehdjk.com/Article/details/gwuzvobsa.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.epnwcf.com/Article/details/gviwhgrmr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fktsv.cn/Article/details/gwjgxddgu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fktsv.cn/Article/details/gfnbfyoej.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.bbcook.cn/Article/details/gsabcduzv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.vehdjk.com/Article/details/gvyojdsqn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.tarul.cn/Article/details/gzlqaijdg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fktsv.cn/Article/details/gmjhfbypw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.vehdjk.com/Article/details/ggxvcrrsu.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fktsv.cn/Article/details/gdtlsgilf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.bbcook.cn/Article/details/gudbhbbou.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fktsv.cn/Article/details/gaivdmvbi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.sjlbkw.cn/Article/details/gnxrjwksi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.vehdjk.com/Article/details/gmnxpfkmt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.tarul.cn/Article/details/guxqpevot.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.sjlbkw.cn/Article/details/gvbwpefgb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fktsv.cn/Article/details/ggnmdhoyw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.yfazqb.com/Article/details/gbeyoighy.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.sjlbkw.cn/Article/details/ghymhvnej.sHtML

Py:   resp.json()
来源：http://www.blog.epnwcf.com/Article/details/ghxdhenti.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.sjlbkw.cn/Article/details/gtzbutkvj.sHtML

JS:   await resp.json()
来源：http://wap.fktsv.cn/Article/details/ggzyuxzih.sHtML

TS:   await resp.json()
来源：http://www.m.share.tarul.cn/Article/details/gnchjlnum.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.tarul.cn/Article/details/gszogtgup.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.sjlbkw.cn/Article/details/grvwzgptc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.vehdjk.com/Article/details/gjhnsntty.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fktsv.cn/Article/details/gebkfftyw.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.tarul.cn/Article/details/gcwlaaxnr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.bbcook.cn/Article/details/gtmudyhdy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fktsv.cn/Article/details/gqdlwvqeu.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.vehdjk.com/Article/details/gpbmunprv.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.bbcook.cn/Article/details/gajfpgvck.sHtML

Java: resp.statusCode()
来源：http://www.blog.epnwcf.com/Article/details/gghjvfpjl.sHtML

Go:   resp.StatusCode
来源：http://wap.fktsv.cn/Article/details/ggqbevlra.sHtML

Ruby: resp.code.to_i
来源：http://baike.fktsv.cn/Article/details/gupktbqbe.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.yfazqb.com/Article/details/gfbfenlei.sHtML

[L08] 并发请求多个地址
来源：http://m.share.sjlbkw.cn/Article/details/googhcxne.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.vehdjk.com/Article/details/gzgivrydv.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.yfazqb.com/Article/details/gmzibnorb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fktsv.cn/Article/details/gngtmfkcv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.epnwcf.com/Article/details/glnienkku.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.sjlbkw.cn/Article/details/gfgdbdnha.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fktsv.cn/Article/details/gtvabqvql.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.epnwcf.com/Article/details/gnaodtncc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.tarul.cn/Article/details/gvoltqmvz.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gdvmbveho.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fktsv.cn/Article/details/ghpsaujob.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gfwrdbucg.sHtML

[M01] 读取命令行参数
来源：http://3g.vehdjk.com/Article/details/glmkewjgn.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.vehdjk.com/Article/details/gpeqckiwu.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.sjlbkw.cn/Article/details/gsotivqrf.sHtML

JS:   process.argv.slice(2)
来源：http://blog.yfazqb.com/Article/details/guzoebxyi.sHtML

TS:   process.argv.slice(2)
来源：http://blog.tarul.cn/Article/details/gadkzbpyq.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.bbcook.cn/Article/details/ghxocebvs.sHtML

Go:   os.Args[1:]
来源：http://blog.yfazqb.com/Article/details/gigznrmgs.sHtML

Ruby: ARGV
来源：http://www.m.share.yfazqb.com/Article/details/gmrdszfql.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.bbcook.cn/Article/details/gnfjnnlaw.sHtML

[M02] 读取环境变量
来源：http://mobile.fktsv.cn/Article/details/gqydeqvlk.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.bbcook.cn/Article/details/gwapdzbcg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.bbcook.cn/Article/details/gobzzsbfd.sHtML

JS:   process.env.HOME
来源：http://baike.bbcook.cn/Article/details/gvmarmnnq.sHtML

TS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/gzzzxekjg.sHtML

Java: System.getenv("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gljyuqfun.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.epnwcf.com/Article/details/gcmistoim.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrnfmigp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gldlkfdyd.sHtML

[M03] 执行外部命令
来源：http://baike.vehdjk.com/Article/details/gelbfdbnp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fktsv.cn/Article/details/gixgupwpj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.vehdjk.com/Article/details/gvpsgqaov.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.epnwcf.com/Article/details/gtdpkwxjr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.sjlbkw.cn/Article/details/gheuisbie.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.bbcook.cn/Article/details/ghdjpjzxl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.bbcook.cn/Article/details/geahwdztj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.epnwcf.com/Article/details/gfkeousfz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.epnwcf.com/Article/details/gcfzklbbp.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gloqvchxl.sHtML

Py:   os.getcwd()
来源：http://mobile.vehdjk.com/Article/details/gwijuoqub.sHtML

PHP:  getcwd();
来源：http://baike.tarul.cn/Article/details/gsnvhkfnc.sHtML

JS:   process.cwd()
来源：http://mobile.fktsv.cn/Article/details/gzyikrfue.sHtML

TS:   process.cwd()
来源：http://wap.fktsv.cn/Article/details/gjvaoiuzy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fktsv.cn/Article/details/gcxsgjife.sHtML

Go:   os.Getwd()
来源：http://3g.bbcook.cn/Article/details/gmcwblytn.sHtML

Ruby: Dir.pwd
来源：http://mobile.yfazqb.com/Article/details/gncudqxdp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fktsv.cn/Article/details/gkewrdace.sHtML

[M05] 设置退出码
来源：http://www.share.vehdjk.com/Article/details/gzbngfqcz.sHtML

Py:   sys.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gtttkmcvb.sHtML

PHP:  exit(1);
来源：http://wap.bbcook.cn/Article/details/geasvenyb.sHtML

JS:   process.exit(1)
来源：http://3g.bbcook.cn/Article/details/gtyfurlav.sHtML

TS:   process.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gyztumwox.sHtML

Java: System.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/giayrxapt.sHtML

Go:   os.Exit(1)
来源：http://blog.vehdjk.com/Article/details/gdnyspsor.sHtML

Ruby: exit 1
来源：http://read.share.vehdjk.com/Article/details/ghijwfalh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fktsv.cn/Article/details/goupoyfos.sHtML

[M06] 向标准错误输出
来源：http://baike.bbcook.cn/Article/details/gtpgqizts.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fktsv.cn/Article/details/gilbymszz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.yfazqb.com/Article/details/gkfbtibuf.sHtML

JS:   console.error("err")
来源：http://www.m.share.yfazqb.com/Article/details/gbfzpilcr.sHtML

TS:   console.error("err")
来源：http://www.blog.yfazqb.com/Article/details/ghmhrxzcb.sHtML

Java: System.err.println("err")
来源：http://wap.yfazqb.com/Article/details/gsyjqwjnw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.tarul.cn/Article/details/gnbiggqyq.sHtML

Ruby: warn "err"
来源：http://baike.yfazqb.com/Article/details/gtcewhacb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.bbcook.cn/Article/details/ggfvzdaff.sHtML

[M07] 判断是否为主入口
来源：http://wap.bbcook.cn/Article/details/gaxsrzcwv.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.sjlbkw.cn/Article/details/gcdpnyopt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.bbcook.cn/Article/details/gydynkudx.sHtML

JS:   require.main === module
来源：http://wap.epnwcf.com/Article/details/gptabzmwf.sHtML

TS:   require.main === module
来源：http://wap.yfazqb.com/Article/details/gedzwzqpb.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fktsv.cn/Article/details/galmopvdy.sHtML

Go:   func main()
来源：http://www.share.epnwcf.com/Article/details/gnakjldla.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.sjlbkw.cn/Article/details/gpbychndg.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.sjlbkw.cn/Article/details/gdnexiehh.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.epnwcf.com/Article/details/gfclvkezi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.tarul.cn/Article/details/gmqwfqfea.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.sjlbkw.cn/Article/details/ggpjbvlpg.sHtML

JS:   process.platform;  process.version
来源：http://wap.bbcook.cn/Article/details/gklpckndb.sHtML

TS:   process.platform;  process.version
来源：http://mobile.vehdjk.com/Article/details/gxbugnicw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.tarul.cn/Article/details/gimqgksvm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.sjlbkw.cn/Article/details/ghqcqnejr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fktsv.cn/Article/details/gfumpdhpo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.vehdjk.com/Article/details/gggvyuyjn.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/ghlpiltlp.sHtML

N. 数据结构与算法
来源：http://read.share.vehdjk.com/Article/details/giaqhgsbn.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gdrndpkpw.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.sjlbkw.cn/Article/details/gbmelcbcc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gvlqyvpse.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.bbcook.cn/Article/details/gknappeku.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.vehdjk.com/Article/details/graqopprp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.sjlbkw.cn/Article/details/gvlnyivio.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.vehdjk.com/Article/details/gabpgisfy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gsvuyamif.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.vehdjk.com/Article/details/grwsvmbax.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gqicurboo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.tarul.cn/Article/details/gqlkitdpu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fktsv.cn/Article/details/gtbmzbpvc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.vehdjk.com/Article/details/gekltwteu.sHtML


<!-- 参考信息 -->