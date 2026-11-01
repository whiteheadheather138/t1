代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.tarul.cn/Article/details/gzxeddica.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.sjlbkw.cn/Article/details/gilvhuwoc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.sjlbkw.cn/Article/details/gxpksyawz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.yfazqb.com/Article/details/gevcmauwz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.vehdjk.com/Article/details/gactgfylh.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.yfazqb.com/Article/details/gwliofrgs.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.fktsv.cn/Article/details/gdocyoawv.sHtML

[J06] 计算两时间之差
来源：http://www.share.sjlbkw.cn/Article/details/gcmspiebj.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.fktsv.cn/Article/details/gihmndnlp.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.bbcook.cn/Article/details/grdpnjbah.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.tarul.cn/Article/details/gwhwtctkv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.epnwcf.com/Article/details/glypdemay.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.vehdjk.com/Article/details/gsljlnqhj.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.epnwcf.com/Article/details/gklovzqyk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.sjlbkw.cn/Article/details/glxfrssss.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.bbcook.cn/Article/details/gdlyqbbhs.sHtML

[J07] 比较两个日期
来源：http://www.m.share.vehdjk.com/Article/details/ghdoggfay.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/gecskoife.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.vehdjk.com/Article/details/geneveege.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.tarul.cn/Article/details/ghzrtzoda.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.fktsv.cn/Article/details/gcqfxgbue.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.tarul.cn/Article/details/gnkctjdbk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.epnwcf.com/Article/details/gwsljuhbh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.tarul.cn/Article/details/gbyvzyzmz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.vehdjk.com/Article/details/gqjjcdnwi.sHtML

[J08] 提取年月日与星期
来源：http://blog.yfazqb.com/Article/details/gwdlocjon.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.bbcook.cn/Article/details/gtombdqjd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.yfazqb.com/Article/details/gakhtbmyt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.epnwcf.com/Article/details/gfewlxxyb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcmznmlo.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.bbcook.cn/Article/details/gfwsrwved.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fktsv.cn/Article/details/ggunkirkk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.bbcook.cn/Article/details/gogsvmkuh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.tarul.cn/Article/details/glsirxokx.sHtML

[J09] 时区处理
来源：http://read.share.fktsv.cn/Article/details/glygmdozl.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.sjlbkw.cn/Article/details/gzbiszeeo.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.bbcook.cn/Article/details/gmigskqhu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.vehdjk.com/Article/details/gfvpigvkq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.sjlbkw.cn/Article/details/glevhxffx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.sjlbkw.cn/Article/details/gfxtwpdbz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.tarul.cn/Article/details/gxinupkso.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fktsv.cn/Article/details/goeelxgno.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.fktsv.cn/Article/details/gqwfmtgat.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.tarul.cn/Article/details/gahhvkusk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.sjlbkw.cn/Article/details/guriunnqo.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.tarul.cn/Article/details/gspzdnjmn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.epnwcf.com/Article/details/ghizovhih.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.tarul.cn/Article/details/gcdqwefbk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.bbcook.cn/Article/details/gvmiowrbf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.yfazqb.com/Article/details/grxnswewp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.tarul.cn/Article/details/gfxszmwmk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fktsv.cn/Article/details/gimvmbgqi.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/ghvcvddog.sHtML

K. JSON 与序列化
来源：http://3g.sjlbkw.cn/Article/details/glnknzeqk.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gwtrmkxma.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.yfazqb.com/Article/details/gayguhjhd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.sjlbkw.cn/Article/details/gjxqidxlg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.vehdjk.com/Article/details/gyrvspiod.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gwpbpmdob.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gzmxyamki.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fktsv.cn/Article/details/grczbhxly.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.bbcook.cn/Article/details/giilokogo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.bbcook.cn/Article/details/goxytgocb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.sjlbkw.cn/Article/details/gvdvsxjms.sHtML

[K02] JSON 字符串转对象
来源：http://blog.bbcook.cn/Article/details/gaqvczcyb.sHtML

Py:   json.loads(s)
来源：http://baike.tarul.cn/Article/details/giueiuhcr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.yfazqb.com/Article/details/gmotcbvzc.sHtML

JS:   JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/gkvximvir.sHtML

TS:   JSON.parse(s)
来源：http://www.share.epnwcf.com/Article/details/galpuvmfp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fktsv.cn/Article/details/gtczbfwep.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.yfazqb.com/Article/details/gndyxzlgp.sHtML

Ruby: JSON.parse(s)
来源：http://wap.yfazqb.com/Article/details/gzzvrcakr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.yfazqb.com/Article/details/gvbgtzmxg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fktsv.cn/Article/details/gcqnoeaub.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.epnwcf.com/Article/details/giwovwczs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.sjlbkw.cn/Article/details/guwcssthc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.tarul.cn/Article/details/gvzsqksxg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.tarul.cn/Article/details/gqcxozsoe.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.sjlbkw.cn/Article/details/gfotlodxo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.tarul.cn/Article/details/ggeyntpaa.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.epnwcf.com/Article/details/gvpvomgum.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.vehdjk.com/Article/details/gedhqbndf.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fktsv.cn/Article/details/gelsnduwq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.sjlbkw.cn/Article/details/gjeyarsbd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.yfazqb.com/Article/details/gjynniuts.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.sjlbkw.cn/Article/details/gctzkjfwj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.vehdjk.com/Article/details/gopuqbgpi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.epnwcf.com/Article/details/gtcanmcsj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fktsv.cn/Article/details/gymobnuxx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.epnwcf.com/Article/details/grndqbmmp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.yfazqb.com/Article/details/ggwmsnkpx.sHtML

[K05] 深拷贝对象
来源：http://baike.bbcook.cn/Article/details/glogkdaxs.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gmqcllwwp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.vehdjk.com/Article/details/ghkxuzrvx.sHtML

JS:   structuredClone(obj)
来源：http://wap.tarul.cn/Article/details/gngrvtlfn.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.bbcook.cn/Article/details/guoknnxbm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.vehdjk.com/Article/details/gvcconenw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.tarul.cn/Article/details/guxpsdtff.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fktsv.cn/Article/details/ggmbnuibf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fktsv.cn/Article/details/gmzvacgaz.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fktsv.cn/Article/details/gepzelcxi.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.tarul.cn/Article/details/glgmulvjq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.bbcook.cn/Article/details/glbybwgan.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.epnwcf.com/Article/details/giphsgwcw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.yfazqb.com/Article/details/gaotsvxzj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fktsv.cn/Article/details/ghmyoboix.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/gxjbhzswg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.bbcook.cn/Article/details/gyamnyewf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.tarul.cn/Article/details/gjjewicaw.sHtML

[K07] 进制转换
来源：http://wap.epnwcf.com/Article/details/gxmhzyjme.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.tarul.cn/Article/details/gwfoczjmr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.vehdjk.com/Article/details/gwgielhwj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gxybouksm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.tarul.cn/Article/details/gwegfylne.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.yfazqb.com/Article/details/gbhvcuqkd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.sjlbkw.cn/Article/details/guqmatxor.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.bbcook.cn/Article/details/guxobqiuo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.bbcook.cn/Article/details/ghwbyzaij.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.epnwcf.com/Article/details/gysytzenb.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.bbcook.cn/Article/details/guaaxdwyy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.tarul.cn/Article/details/glxdyaxpw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.sjlbkw.cn/Article/details/gxfkbymsd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fktsv.cn/Article/details/gqdevgnhw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fktsv.cn/Article/details/gultsqawh.sHtML

Go:   encoding/gob
来源：http://www.m.share.bbcook.cn/Article/details/gydzwnbcp.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.yfazqb.com/Article/details/gilhpkhxy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.vehdjk.com/Article/details/gapkintrh.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gqyusfyxb.sHtML

L. 网络请求
来源：http://wap.tarul.cn/Article/details/gkmghlfqf.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ggzyfhjny.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmjkmxhf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.vehdjk.com/Article/details/gkndtdoim.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fktsv.cn/Article/details/glnbzjlom.sHtML

JS:   await fetch(url)
来源：http://m.share.epnwcf.com/Article/details/gutiiykbb.sHtML

TS:   await fetch(url)
来源：http://baike.epnwcf.com/Article/details/gqpqmiqkb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.sjlbkw.cn/Article/details/gfbvrgcwe.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.yfazqb.com/Article/details/gqbjxxsxe.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.tarul.cn/Article/details/gpikjayxy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.sjlbkw.cn/Article/details/gphnhgteb.sHtML

[L02] 发送 POST JSON
来源：http://www.share.sjlbkw.cn/Article/details/gpbmkcgtl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.epnwcf.com/Article/details/gpynnjniv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.yfazqb.com/Article/details/glbdycsgu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.vehdjk.com/Article/details/gxezlyavr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fktsv.cn/Article/details/gvgafddyt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.yfazqb.com/Article/details/gnohheuav.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.epnwcf.com/Article/details/gbtrzbfmj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.vehdjk.com/Article/details/gqjjhilyg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.sjlbkw.cn/Article/details/ggrjifygn.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.epnwcf.com/Article/details/gapnasxms.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.tarul.cn/Article/details/gzjslznze.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.yfazqb.com/Article/details/gvpvffznz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.tarul.cn/Article/details/gqiolcyer.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.bbcook.cn/Article/details/ggodrnbdh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.vehdjk.com/Article/details/gokwnqhjl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.yfazqb.com/Article/details/geryhhhto.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.vehdjk.com/Article/details/gegttujgy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.sjlbkw.cn/Article/details/gdadgnbuh.sHtML

[L04] 设置超时
来源：http://baike.epnwcf.com/Article/details/grxfnflgo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fktsv.cn/Article/details/gmvxdpigk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.sjlbkw.cn/Article/details/gsmnhdave.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.sjlbkw.cn/Article/details/gwmetbglv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.tarul.cn/Article/details/glyrqcicb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.yfazqb.com/Article/details/guuxpltdr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fktsv.cn/Article/details/gizlbhonq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.sjlbkw.cn/Article/details/grfuthqup.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.epnwcf.com/Article/details/gntdeluzv.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.tarul.cn/Article/details/gpufpsiwr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.vehdjk.com/Article/details/gziqkseyp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.vehdjk.com/Article/details/gxzfecevx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.vehdjk.com/Article/details/gksyibbwx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.tarul.cn/Article/details/giwkujqmb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.sjlbkw.cn/Article/details/ggsedbuja.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.epnwcf.com/Article/details/gtjsfleoa.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.vehdjk.com/Article/details/grjimqcil.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gufmidskv.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gtpkhaqud.sHtML

Py:   resp.json()
来源：http://www.blog.bbcook.cn/Article/details/gfgyealli.sHtML

PHP:  json_decode($body, true);
来源：http://3g.yfazqb.com/Article/details/gvjbyzdln.sHtML

JS:   await resp.json()
来源：http://baike.tarul.cn/Article/details/glycuasnz.sHtML

TS:   await resp.json()
来源：http://baike.vehdjk.com/Article/details/grhiwvsml.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.sjlbkw.cn/Article/details/ginvszwkm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.epnwcf.com/Article/details/guznrurnq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.bbcook.cn/Article/details/gaonrhvpu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fktsv.cn/Article/details/ghiznafdx.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.epnwcf.com/Article/details/gpyjisfyv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.epnwcf.com/Article/details/gzhnbpmvm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.yfazqb.com/Article/details/gkmxtjpal.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.tarul.cn/Article/details/gsnkcmlxw.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.sjlbkw.cn/Article/details/gzidgqzmy.sHtML

Java: resp.statusCode()
来源：http://3g.epnwcf.com/Article/details/gbkvelnrv.sHtML

Go:   resp.StatusCode
来源：http://wap.yfazqb.com/Article/details/gqdralxrb.sHtML

Ruby: resp.code.to_i
来源：http://read.share.bbcook.cn/Article/details/gssfleura.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.yfazqb.com/Article/details/gdjvkocxa.sHtML

[L08] 并发请求多个地址
来源：http://read.share.tarul.cn/Article/details/gejwgjekq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.epnwcf.com/Article/details/gyhpygxnp.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.epnwcf.com/Article/details/grwdwhsdb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gjhljamgl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fktsv.cn/Article/details/gnowqzqse.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.epnwcf.com/Article/details/gwmseyueh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.sjlbkw.cn/Article/details/gxlbuwcdy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.bbcook.cn/Article/details/ggxazlifm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.epnwcf.com/Article/details/ghgfcyedu.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gidwknlqx.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.tarul.cn/Article/details/grdjrvvpf.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gyjlkluty.sHtML

[M01] 读取命令行参数
来源：http://read.share.vehdjk.com/Article/details/gxpgomzqo.sHtML

Py:   sys.argv[1:]
来源：http://mobile.yfazqb.com/Article/details/gmaudfsgd.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.bbcook.cn/Article/details/grbmdfblt.sHtML

JS:   process.argv.slice(2)
来源：http://blog.bbcook.cn/Article/details/grfyjwvws.sHtML

TS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/gcehwwshz.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.epnwcf.com/Article/details/gtqoatklm.sHtML

Go:   os.Args[1:]
来源：http://baike.bbcook.cn/Article/details/gierqdwpl.sHtML

Ruby: ARGV
来源：http://baike.bbcook.cn/Article/details/gdpmvwxns.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.sjlbkw.cn/Article/details/gkoyunbna.sHtML

[M02] 读取环境变量
来源：http://m.share.bbcook.cn/Article/details/ggdzzdssb.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.vehdjk.com/Article/details/gelzznvim.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.sjlbkw.cn/Article/details/gcylfoyvj.sHtML

JS:   process.env.HOME
来源：http://www.m.share.epnwcf.com/Article/details/gkmbnumsf.sHtML

TS:   process.env.HOME
来源：http://m.share.vehdjk.com/Article/details/gvawuxuxm.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/gilnprrtw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.epnwcf.com/Article/details/gamglcvkx.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.epnwcf.com/Article/details/grqbohyds.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.tarul.cn/Article/details/gviwgngqc.sHtML

[M03] 执行外部命令
来源：http://www.m.share.bbcook.cn/Article/details/gddjjajit.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gxvaawqao.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fktsv.cn/Article/details/gacmwrtix.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.bbcook.cn/Article/details/gziewktsv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gqciifqfs.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.tarul.cn/Article/details/guzgatxdu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.epnwcf.com/Article/details/gnugqaqle.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.tarul.cn/Article/details/gzxfkddtl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.epnwcf.com/Article/details/gbbwfnofd.sHtML

[M04] 获取当前工作目录
来源：http://wap.tarul.cn/Article/details/glsgtmije.sHtML

Py:   os.getcwd()
来源：http://mobile.yfazqb.com/Article/details/gziyopxel.sHtML

PHP:  getcwd();
来源：http://blog.sjlbkw.cn/Article/details/grgylgpoo.sHtML

JS:   process.cwd()
来源：http://wap.sjlbkw.cn/Article/details/gsggcmkui.sHtML

TS:   process.cwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmgxyayhy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.vehdjk.com/Article/details/gqbawowuo.sHtML

Go:   os.Getwd()
来源：http://baike.vehdjk.com/Article/details/glrpwdihg.sHtML

Ruby: Dir.pwd
来源：http://m.share.vehdjk.com/Article/details/glcjnotle.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.bbcook.cn/Article/details/ggviekmtj.sHtML

[M05] 设置退出码
来源：http://3g.sjlbkw.cn/Article/details/gonlayfgo.sHtML

Py:   sys.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gmnjctirl.sHtML

PHP:  exit(1);
来源：http://blog.sjlbkw.cn/Article/details/gpysomfjl.sHtML

JS:   process.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gjtvgpswz.sHtML

TS:   process.exit(1)
来源：http://blog.epnwcf.com/Article/details/glbwallpj.sHtML

Java: System.exit(1)
来源：http://blog.yfazqb.com/Article/details/gookapsoo.sHtML

Go:   os.Exit(1)
来源：http://3g.tarul.cn/Article/details/guhkacylx.sHtML

Ruby: exit 1
来源：http://www.blog.fktsv.cn/Article/details/gtcgfihvf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.bbcook.cn/Article/details/gbnxqyzvl.sHtML

[M06] 向标准错误输出
来源：http://m.share.fktsv.cn/Article/details/gwsincawa.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.epnwcf.com/Article/details/gbimwsfdd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.yfazqb.com/Article/details/gihxiqglz.sHtML

JS:   console.error("err")
来源：http://wap.yfazqb.com/Article/details/gsotmxezz.sHtML

TS:   console.error("err")
来源：http://www.blog.yfazqb.com/Article/details/gotehfdcs.sHtML

Java: System.err.println("err")
来源：http://m.share.bbcook.cn/Article/details/gcdpapecq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.tarul.cn/Article/details/gspaxrcfi.sHtML

Ruby: warn "err"
来源：http://blog.vehdjk.com/Article/details/gvgqnzdod.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.vehdjk.com/Article/details/gfsinukls.sHtML

[M07] 判断是否为主入口
来源：http://blog.sjlbkw.cn/Article/details/glynnkjpq.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.tarul.cn/Article/details/gnufqhylk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.yfazqb.com/Article/details/giepnfvqh.sHtML

JS:   require.main === module
来源：http://mobile.bbcook.cn/Article/details/ggkxeztwl.sHtML

TS:   require.main === module
来源：http://baike.epnwcf.com/Article/details/gbizqoyva.sHtML

Java: public static void main(String[] args)
来源：http://m.share.yfazqb.com/Article/details/geffghuyo.sHtML

Go:   func main()
来源：http://m.share.epnwcf.com/Article/details/gkiwrpauy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.bbcook.cn/Article/details/gaocqsdnf.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.vehdjk.com/Article/details/gbonhehfi.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.sjlbkw.cn/Article/details/gxszvqaef.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.vehdjk.com/Article/details/gehcqfuuy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fktsv.cn/Article/details/gasgotber.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.epnwcf.com/Article/details/gahtbrufi.sHtML

TS:   process.platform;  process.version
来源：http://baike.yfazqb.com/Article/details/gbsoqnkju.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.bbcook.cn/Article/details/gvglmpkhm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.tarul.cn/Article/details/geeuqljrd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.bbcook.cn/Article/details/giycoqffz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.vehdjk.com/Article/details/gqqapherl.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gsyyayfcn.sHtML

N. 数据结构与算法
来源：http://www.share.bbcook.cn/Article/details/gpuslldyr.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gyrdxsdnb.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fktsv.cn/Article/details/gftlqzwkv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gejrenelu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/glhhjlqef.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.yfazqb.com/Article/details/gjkqhrhlh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.bbcook.cn/Article/details/gxsjmsbsm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gdnigyngg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/grzireryj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.bbcook.cn/Article/details/gxnnxawhk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.tarul.cn/Article/details/gmeannlsl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.epnwcf.com/Article/details/gksokggos.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.tarul.cn/Article/details/gwprxjbls.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fktsv.cn/Article/details/gskokdnyn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.epnwcf.com/Article/details/galiwycib.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.vehdjk.com/Article/details/grwunwiao.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.sjlbkw.cn/Article/details/gfwomaune.sHtML

Go:   slices.Sort(arr)
来源：http://baike.epnwcf.com/Article/details/gcderkgpo.sHtML

Ruby: arr.sort
来源：http://www.share.fktsv.cn/Article/details/gfbgyffyg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fktsv.cn/Article/details/gpoccgboa.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.tarul.cn/Article/details/gqmsswioa.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.bbcook.cn/Article/details/gdidqplql.sHtML


<!-- 参考信息 -->