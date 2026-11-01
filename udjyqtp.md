代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.fktsv.cn/Article/details/gskqnwhyh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fktsv.cn/Article/details/gysmpcfut.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.vehdjk.com/Article/details/ggpgtpwhh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.epnwcf.com/Article/details/gbyglilpx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.bbcook.cn/Article/details/gqxngoeze.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.bbcook.cn/Article/details/gdvxnhdwd.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.bbcook.cn/Article/details/gggkvuocr.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.tarul.cn/Article/details/gacvtrukp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.sjlbkw.cn/Article/details/gqbwezdxd.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.vehdjk.com/Article/details/gwoqasfsp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.vehdjk.com/Article/details/gkdtbhggc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.vehdjk.com/Article/details/ggwkezrbb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.yfazqb.com/Article/details/gtjhsomuw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.yfazqb.com/Article/details/gxkbwbxbs.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.bbcook.cn/Article/details/ghcabspaw.sHtML

[J06] 计算两时间之差
来源：http://baike.sjlbkw.cn/Article/details/glatzsyuf.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.vehdjk.com/Article/details/gaeaeitqy.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.epnwcf.com/Article/details/gsyxtvdhh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.tarul.cn/Article/details/gmrcafoby.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.bbcook.cn/Article/details/gqcffbwcp.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.tarul.cn/Article/details/gvervkpfx.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.epnwcf.com/Article/details/gansurzee.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.fktsv.cn/Article/details/gbgrdrmdj.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.bbcook.cn/Article/details/gpqdyyhmq.sHtML

[J07] 比较两个日期
来源：http://read.share.bbcook.cn/Article/details/gghjbtcwn.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.bbcook.cn/Article/details/gxigmcuol.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.tarul.cn/Article/details/glkacfbah.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.tarul.cn/Article/details/ghkqjdose.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.epnwcf.com/Article/details/ghgguzjsi.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.sjlbkw.cn/Article/details/glevfzqfb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.fktsv.cn/Article/details/gqvbraqgi.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.vehdjk.com/Article/details/gayjpdxkp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.yfazqb.com/Article/details/gnqfwxppr.sHtML

[J08] 提取年月日与星期
来源：http://read.share.sjlbkw.cn/Article/details/grquvuqsy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.vehdjk.com/Article/details/gdnbifeqt.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fktsv.cn/Article/details/gpnjbbrib.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.sjlbkw.cn/Article/details/gcuyezyif.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.epnwcf.com/Article/details/ghbojqwdt.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.tarul.cn/Article/details/gcunpgrgx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.sjlbkw.cn/Article/details/gddondumr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxiotdpm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.sjlbkw.cn/Article/details/gnsfghlar.sHtML

[J09] 时区处理
来源：http://www.m.share.bbcook.cn/Article/details/gugzhbdqy.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.vehdjk.com/Article/details/gfeaodqll.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.bbcook.cn/Article/details/gkofnvnfn.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fktsv.cn/Article/details/gdhhpcawr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.vehdjk.com/Article/details/gogsbnqbk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.vehdjk.com/Article/details/gtameakgj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.epnwcf.com/Article/details/gxexsysrv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fktsv.cn/Article/details/gsosgfrje.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.sjlbkw.cn/Article/details/gxurqyiro.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.sjlbkw.cn/Article/details/gjxmpkpqz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.epnwcf.com/Article/details/gsbvlvprt.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.epnwcf.com/Article/details/gcfzcggtq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.yfazqb.com/Article/details/ghaywwztt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.fktsv.cn/Article/details/gedangbgq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.yfazqb.com/Article/details/glvpqmlfy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.tarul.cn/Article/details/gswolcwfq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.bbcook.cn/Article/details/gbjkxkcdb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.bbcook.cn/Article/details/gsyztpedw.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gnswjbagd.sHtML

K. JSON 与序列化
来源：http://www.m.share.yfazqb.com/Article/details/gffyfojai.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gxrijbnna.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.tarul.cn/Article/details/gwkqyujsk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.tarul.cn/Article/details/gnytcstla.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fktsv.cn/Article/details/gshagmker.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.sjlbkw.cn/Article/details/gkrjudllv.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fktsv.cn/Article/details/gdkelfkcz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.tarul.cn/Article/details/ghyhjlmvl.sHtML

Go:   json.Marshal(obj)
来源：http://blog.sjlbkw.cn/Article/details/gluqkosea.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.yfazqb.com/Article/details/golljdrsl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fktsv.cn/Article/details/ggajnfbac.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gunvgzvye.sHtML

Py:   json.loads(s)
来源：http://mobile.bbcook.cn/Article/details/gpkcgzzed.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.yfazqb.com/Article/details/gbtlkqmxj.sHtML

JS:   JSON.parse(s)
来源：http://baike.epnwcf.com/Article/details/glhxffzjn.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.epnwcf.com/Article/details/gxvhghnki.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqzdwzbk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fktsv.cn/Article/details/gtiwwqljv.sHtML

Ruby: JSON.parse(s)
来源：http://wap.bbcook.cn/Article/details/gjxpppzst.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.yfazqb.com/Article/details/gwcqnfsvp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.vehdjk.com/Article/details/gwkkuugdj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.epnwcf.com/Article/details/gazwzqlsk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.tarul.cn/Article/details/gwtrygnvk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.bbcook.cn/Article/details/gmkegtihc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/gtkinrbkn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gadijipos.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.sjlbkw.cn/Article/details/gpzrlfvwg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.epnwcf.com/Article/details/garjpilue.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fktsv.cn/Article/details/grsztpzqy.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.bbcook.cn/Article/details/gjvlvokrb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.yfazqb.com/Article/details/gucxwqsxg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.epnwcf.com/Article/details/gmyeofdcm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fktsv.cn/Article/details/grlcldjai.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fktsv.cn/Article/details/gvmlogxzy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.yfazqb.com/Article/details/gvojwuabd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.vehdjk.com/Article/details/gqugxoscp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.bbcook.cn/Article/details/gksqxcbtg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.vehdjk.com/Article/details/ghcortkck.sHtML

[K05] 深拷贝对象
来源：http://www.share.yfazqb.com/Article/details/giiacokpe.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.epnwcf.com/Article/details/guarqzyci.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fktsv.cn/Article/details/gcnexyrhs.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gmbsabnzf.sHtML

TS:   structuredClone(obj)
来源：http://wap.tarul.cn/Article/details/gupvmmdlq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.epnwcf.com/Article/details/gvqhcuzyo.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.epnwcf.com/Article/details/gweicfsrb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.bbcook.cn/Article/details/gujshuvns.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.bbcook.cn/Article/details/gwlsyrdkr.sHtML

[K06] 解析 URL 查询串
来源：http://3g.yfazqb.com/Article/details/gglfyibug.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.bbcook.cn/Article/details/gwcbzduuu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.yfazqb.com/Article/details/glzgexdgl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fktsv.cn/Article/details/gefaunspk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.tarul.cn/Article/details/gmledgopq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.vehdjk.com/Article/details/gwzsiurwv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gkiacklnf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/gwiobfqty.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.bbcook.cn/Article/details/gbfatoiza.sHtML

[K07] 进制转换
来源：http://www.share.bbcook.cn/Article/details/gofeqpdij.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gfsrkntzq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.epnwcf.com/Article/details/gwmkhhknz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gtodfawbt.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.tarul.cn/Article/details/gtvrcgane.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gfeaakszx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.bbcook.cn/Article/details/gxmxbnafq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.epnwcf.com/Article/details/gkdljlgod.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gwjhvhlsb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.tarul.cn/Article/details/ggvjnqisa.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.tarul.cn/Article/details/gjawishgn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.tarul.cn/Article/details/gpubudfkp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.yfazqb.com/Article/details/ggsqiwrfg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.vehdjk.com/Article/details/gclwkluve.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.tarul.cn/Article/details/grdngjram.sHtML

Go:   encoding/gob
来源：http://www.blog.fktsv.cn/Article/details/gynckaehj.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.tarul.cn/Article/details/gfcldacmb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.bbcook.cn/Article/details/gteefwsik.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gbbihlrax.sHtML

L. 网络请求
来源：http://wap.sjlbkw.cn/Article/details/gpkubbqet.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gfdrsuerh.sHtML

[L01] 发送 GET 请求
来源：http://3g.bbcook.cn/Article/details/gdrpvinki.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.bbcook.cn/Article/details/gmgdyjldc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.vehdjk.com/Article/details/gtslklfsj.sHtML

JS:   await fetch(url)
来源：http://3g.tarul.cn/Article/details/gqqmdwewi.sHtML

TS:   await fetch(url)
来源：http://3g.sjlbkw.cn/Article/details/gjzkhvvvw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.tarul.cn/Article/details/gvcdnnfwc.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.tarul.cn/Article/details/gehpmspgv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.yfazqb.com/Article/details/gixdahqlv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gcnfanmgd.sHtML

[L02] 发送 POST JSON
来源：http://3g.tarul.cn/Article/details/gpwtizbqj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fktsv.cn/Article/details/gkhwtkbeh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.vehdjk.com/Article/details/gwngqwsxw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.vehdjk.com/Article/details/gyuibdigf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.bbcook.cn/Article/details/gpefccrzp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.bbcook.cn/Article/details/gbeojatxz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.tarul.cn/Article/details/gymyxhnze.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fktsv.cn/Article/details/gqceeyngd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fktsv.cn/Article/details/gofridjja.sHtML

[L03] 设置自定义请求头
来源：http://read.share.vehdjk.com/Article/details/gkaxesgrg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.bbcook.cn/Article/details/glvcekpbe.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.epnwcf.com/Article/details/ggjatobal.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fktsv.cn/Article/details/glxqtswpc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.bbcook.cn/Article/details/geohunnyt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.sjlbkw.cn/Article/details/gpeiytsvy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.bbcook.cn/Article/details/gtriekrhk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.epnwcf.com/Article/details/gqphcesia.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.yfazqb.com/Article/details/goumpdirs.sHtML

[L04] 设置超时
来源：http://www.share.epnwcf.com/Article/details/geulvmrqx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.bbcook.cn/Article/details/gorqedbbl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.bbcook.cn/Article/details/goqgibqlc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.bbcook.cn/Article/details/gylrutrkj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fktsv.cn/Article/details/gdvfnkyys.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.bbcook.cn/Article/details/gjkpohjnh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fktsv.cn/Article/details/gkilimhbz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.vehdjk.com/Article/details/gfxnkeqze.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.sjlbkw.cn/Article/details/gdbjrnkai.sHtML

[L05] 上传文件（multipart）
来源：http://blog.yfazqb.com/Article/details/glqfriuxx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.epnwcf.com/Article/details/gtjsvezrh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.tarul.cn/Article/details/gkookpzjr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.tarul.cn/Article/details/gzmqioewr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.vehdjk.com/Article/details/gvnbnmcyl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fktsv.cn/Article/details/gqollmven.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.yfazqb.com/Article/details/gegacguag.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fktsv.cn/Article/details/gififsecp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.epnwcf.com/Article/details/guovalzbi.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fktsv.cn/Article/details/golxlhgnh.sHtML

Py:   resp.json()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxwfoany.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.tarul.cn/Article/details/gqpckwbvo.sHtML

JS:   await resp.json()
来源：http://mobile.bbcook.cn/Article/details/ggxhgbott.sHtML

TS:   await resp.json()
来源：http://www.m.share.vehdjk.com/Article/details/gpyksbrwt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.sjlbkw.cn/Article/details/guhceshyr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.sjlbkw.cn/Article/details/giyieqflu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.sjlbkw.cn/Article/details/gmumdmjaq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.bbcook.cn/Article/details/gxxhjbxcf.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fktsv.cn/Article/details/ghkreljbq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.yfazqb.com/Article/details/ggvkhoclb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.sjlbkw.cn/Article/details/gzfnpyxyx.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.bbcook.cn/Article/details/gnfqhvfgy.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fktsv.cn/Article/details/gyujtsagj.sHtML

Java: resp.statusCode()
来源：http://read.share.tarul.cn/Article/details/gqjvnfgbc.sHtML

Go:   resp.StatusCode
来源：http://wap.sjlbkw.cn/Article/details/gaojzsnel.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.bbcook.cn/Article/details/gheudxejr.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.vehdjk.com/Article/details/gxynxyype.sHtML

[L08] 并发请求多个地址
来源：http://mobile.epnwcf.com/Article/details/grgrcuxah.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.yfazqb.com/Article/details/gvkegcgoa.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fktsv.cn/Article/details/gvhhjengs.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.tarul.cn/Article/details/gucgfhigm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.vehdjk.com/Article/details/gxpzwcnew.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.yfazqb.com/Article/details/gdqjvagxt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.vehdjk.com/Article/details/gbnahzhnx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.bbcook.cn/Article/details/goyxcllmw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.bbcook.cn/Article/details/gwzfkupqz.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gderslsoo.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.yfazqb.com/Article/details/glgupwofv.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gimxiklkz.sHtML

[M01] 读取命令行参数
来源：http://www.share.epnwcf.com/Article/details/gykkjemat.sHtML

Py:   sys.argv[1:]
来源：http://wap.yfazqb.com/Article/details/gzbaexomw.sHtML

PHP:  $argv;  $argc;
来源：http://blog.tarul.cn/Article/details/gpwdmqxsm.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdnmwdhjg.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.tarul.cn/Article/details/gvaurftms.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fktsv.cn/Article/details/gchtfnpay.sHtML

Go:   os.Args[1:]
来源：http://blog.tarul.cn/Article/details/glocdpihb.sHtML

Ruby: ARGV
来源：http://www.m.share.bbcook.cn/Article/details/gnvhlzbhp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.sjlbkw.cn/Article/details/gslnpbsxg.sHtML

[M02] 读取环境变量
来源：http://baike.tarul.cn/Article/details/gtdkwkodv.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.epnwcf.com/Article/details/gazototna.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fktsv.cn/Article/details/goqecedww.sHtML

JS:   process.env.HOME
来源：http://m.share.yfazqb.com/Article/details/gflikrrnf.sHtML

TS:   process.env.HOME
来源：http://mobile.epnwcf.com/Article/details/gxzhfbpwk.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gteguynmf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fktsv.cn/Article/details/gmsiifayr.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.sjlbkw.cn/Article/details/gtcknqsae.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.vehdjk.com/Article/details/gnbhoczmd.sHtML

[M03] 执行外部命令
来源：http://m.share.tarul.cn/Article/details/ghjygeupd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gkrjvaeyz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.epnwcf.com/Article/details/gvpcucjfw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.bbcook.cn/Article/details/gplmrruaw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.epnwcf.com/Article/details/gctcvkekh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.sjlbkw.cn/Article/details/ggckptvrr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.bbcook.cn/Article/details/gctrzomlr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.sjlbkw.cn/Article/details/ggpdtnkca.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fktsv.cn/Article/details/gxbkqdyai.sHtML

[M04] 获取当前工作目录
来源：http://www.share.epnwcf.com/Article/details/ggenbfpcf.sHtML

Py:   os.getcwd()
来源：http://www.blog.tarul.cn/Article/details/gdlzazllt.sHtML

PHP:  getcwd();
来源：http://wap.bbcook.cn/Article/details/ghjwamvpp.sHtML

JS:   process.cwd()
来源：http://3g.epnwcf.com/Article/details/giwctoqni.sHtML

TS:   process.cwd()
来源：http://mobile.epnwcf.com/Article/details/glgicsuze.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fktsv.cn/Article/details/grhcsuqgg.sHtML

Go:   os.Getwd()
来源：http://m.share.bbcook.cn/Article/details/gfpswlztx.sHtML

Ruby: Dir.pwd
来源：http://m.share.sjlbkw.cn/Article/details/gmsjjpypv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.vehdjk.com/Article/details/gwpcfkpzc.sHtML

[M05] 设置退出码
来源：http://www.blog.vehdjk.com/Article/details/goofaznsm.sHtML

Py:   sys.exit(1)
来源：http://blog.epnwcf.com/Article/details/gakeuvazl.sHtML

PHP:  exit(1);
来源：http://mobile.vehdjk.com/Article/details/gxvlgcugx.sHtML

JS:   process.exit(1)
来源：http://baike.yfazqb.com/Article/details/gsoibtswe.sHtML

TS:   process.exit(1)
来源：http://blog.yfazqb.com/Article/details/gwvjgnjji.sHtML

Java: System.exit(1)
来源：http://m.share.yfazqb.com/Article/details/gwzcvllxj.sHtML

Go:   os.Exit(1)
来源：http://baike.yfazqb.com/Article/details/ggmkbsabu.sHtML

Ruby: exit 1
来源：http://blog.bbcook.cn/Article/details/gzofnnano.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.epnwcf.com/Article/details/gbvthkmel.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.vehdjk.com/Article/details/geqmcfndm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.tarul.cn/Article/details/gmzsehvid.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.vehdjk.com/Article/details/gjqtiyrus.sHtML

JS:   console.error("err")
来源：http://m.share.sjlbkw.cn/Article/details/geuqjyhiu.sHtML

TS:   console.error("err")
来源：http://www.share.fktsv.cn/Article/details/gjyygwqiq.sHtML

Java: System.err.println("err")
来源：http://3g.fktsv.cn/Article/details/gjwhsyvgy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.vehdjk.com/Article/details/gopkbhjxw.sHtML

Ruby: warn "err"
来源：http://wap.bbcook.cn/Article/details/gyfvmxzyh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.vehdjk.com/Article/details/gogdrgldr.sHtML

[M07] 判断是否为主入口
来源：http://3g.epnwcf.com/Article/details/gukjwgmsa.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.epnwcf.com/Article/details/gsvhhdyqd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.bbcook.cn/Article/details/gxbmvrhkl.sHtML

JS:   require.main === module
来源：http://m.share.bbcook.cn/Article/details/gmkphyfpw.sHtML

TS:   require.main === module
来源：http://www.blog.fktsv.cn/Article/details/gtetbdnku.sHtML

Java: public static void main(String[] args)
来源：http://mobile.tarul.cn/Article/details/gesavcaem.sHtML

Go:   func main()
来源：http://baike.vehdjk.com/Article/details/gxnocjqwb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.bbcook.cn/Article/details/gaergqlad.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.tarul.cn/Article/details/gpsfcgmgl.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fktsv.cn/Article/details/grrqvogut.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.bbcook.cn/Article/details/gxpwxxvxo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.epnwcf.com/Article/details/gjhvprtzl.sHtML

JS:   process.platform;  process.version
来源：http://read.share.epnwcf.com/Article/details/gpjgfoviq.sHtML

TS:   process.platform;  process.version
来源：http://baike.vehdjk.com/Article/details/ggkswacub.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.bbcook.cn/Article/details/gqbiawdwc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.bbcook.cn/Article/details/gktuzvvey.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.tarul.cn/Article/details/gckuibhjd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.bbcook.cn/Article/details/gavirljai.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gxftczwyi.sHtML

N. 数据结构与算法
来源：http://www.share.vehdjk.com/Article/details/gjinlbedf.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/guhcqeudm.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.epnwcf.com/Article/details/gnrrjdyln.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.yfazqb.com/Article/details/gqvpgrqnt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.yfazqb.com/Article/details/gwtajgprw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.tarul.cn/Article/details/gewncmnys.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.sjlbkw.cn/Article/details/ghrhzggax.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fktsv.cn/Article/details/gjhnysexv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gqgoxaamp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fktsv.cn/Article/details/gqkycimsy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.yfazqb.com/Article/details/gmdqdtqst.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.sjlbkw.cn/Article/details/gexnbxhcl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.sjlbkw.cn/Article/details/gcjdhtyrl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.yfazqb.com/Article/details/gohsygbbt.sHtML


<!-- 参考信息 -->