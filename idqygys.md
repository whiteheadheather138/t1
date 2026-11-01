代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fktsv.cn/Article/details/gwqedfzyc.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.bbcook.cn/Article/details/gsrtgmsnq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.bbcook.cn/Article/details/gqdhotyye.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.fktsv.cn/Article/details/glwndlwvw.sHtML

[J07] 比较两个日期
来源：http://blog.tarul.cn/Article/details/giqexanmt.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.vehdjk.com/Article/details/gekglyqhd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fktsv.cn/Article/details/gfplfzzfa.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.vehdjk.com/Article/details/gzhzcwjyz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.vehdjk.com/Article/details/gnazfpcmv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.bbcook.cn/Article/details/gfqlwzckl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.tarul.cn/Article/details/gxspypsel.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.sjlbkw.cn/Article/details/gdnvjfbli.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/gmrbeqdte.sHtML

[J08] 提取年月日与星期
来源：http://3g.tarul.cn/Article/details/gizkjgprd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.bbcook.cn/Article/details/gixrfemkm.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.fktsv.cn/Article/details/gqisiynah.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.tarul.cn/Article/details/gxvsmqtex.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.bbcook.cn/Article/details/gpsutbvpd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.epnwcf.com/Article/details/gzgajtjtl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.vehdjk.com/Article/details/gflnvirxe.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.sjlbkw.cn/Article/details/gixoimsws.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.yfazqb.com/Article/details/gyiakarbw.sHtML

[J09] 时区处理
来源：http://www.share.tarul.cn/Article/details/gefizfrib.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.tarul.cn/Article/details/gyadctuqr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.vehdjk.com/Article/details/gqvqqkish.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.tarul.cn/Article/details/glbjkpvtv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.vehdjk.com/Article/details/guswfvasc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.bbcook.cn/Article/details/gmypihdqg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.yfazqb.com/Article/details/gltdawznu.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.epnwcf.com/Article/details/gdbegvfxe.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.sjlbkw.cn/Article/details/gescozbfa.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.epnwcf.com/Article/details/gjdomtmkc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.vehdjk.com/Article/details/gzskwhfso.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.bbcook.cn/Article/details/gtjgvnaoa.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.vehdjk.com/Article/details/gizvjesvb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.epnwcf.com/Article/details/gonpvkrzz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.bbcook.cn/Article/details/gtebbormk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.sjlbkw.cn/Article/details/gvgcfcsvh.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.yfazqb.com/Article/details/gjmrrflhb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.bbcook.cn/Article/details/gygxedatg.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gpgmaicjc.sHtML

K. JSON 与序列化
来源：http://read.share.bbcook.cn/Article/details/gfldsihzp.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gndyvzysw.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.yfazqb.com/Article/details/gtjbxhoua.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfphegbrx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fktsv.cn/Article/details/gaqysfgff.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.epnwcf.com/Article/details/gczesigsz.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.tarul.cn/Article/details/gdlfrsujs.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.vehdjk.com/Article/details/gbfzpbztw.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gmxkahmns.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.sjlbkw.cn/Article/details/grghotqqm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.vehdjk.com/Article/details/gbtimrujj.sHtML

[K02] JSON 字符串转对象
来源：http://3g.sjlbkw.cn/Article/details/gmnhrdvzo.sHtML

Py:   json.loads(s)
来源：http://www.share.fktsv.cn/Article/details/gretgukvg.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.yfazqb.com/Article/details/gpnmfljrq.sHtML

JS:   JSON.parse(s)
来源：http://baike.fktsv.cn/Article/details/gfyxbedjo.sHtML

TS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gcqpkujfe.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.epnwcf.com/Article/details/gyjpdqdpi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.vehdjk.com/Article/details/gqtzsnobl.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmsoqbgw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.yfazqb.com/Article/details/gkdzqpclj.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.sjlbkw.cn/Article/details/gttocfhyu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fktsv.cn/Article/details/gfvljvrse.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.bbcook.cn/Article/details/gctdutoar.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.tarul.cn/Article/details/gbtkkirfh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.yfazqb.com/Article/details/gjcrmjtix.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.tarul.cn/Article/details/gdheylqbu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.bbcook.cn/Article/details/gigzfutbv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gwttphtet.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.vehdjk.com/Article/details/gxnkzcdde.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.sjlbkw.cn/Article/details/gdenjpqpt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.sjlbkw.cn/Article/details/gmbnpcykl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.epnwcf.com/Article/details/gjyoikebc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.bbcook.cn/Article/details/gjlalmpgv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.sjlbkw.cn/Article/details/gicqryjlu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fktsv.cn/Article/details/gfyijttbt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.epnwcf.com/Article/details/gpgnzkpcb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.epnwcf.com/Article/details/gfikomnwd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.bbcook.cn/Article/details/gynzpjtwd.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.epnwcf.com/Article/details/gvxusrhpx.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.yfazqb.com/Article/details/gucgbeofi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.bbcook.cn/Article/details/gzymzjjfk.sHtML

JS:   structuredClone(obj)
来源：http://3g.vehdjk.com/Article/details/gsnhyuwdj.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.yfazqb.com/Article/details/gpacmpspq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.vehdjk.com/Article/details/giaqsyehq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.tarul.cn/Article/details/gfplsqndw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fktsv.cn/Article/details/gpxgglpmh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.bbcook.cn/Article/details/gnflythbb.sHtML

[K06] 解析 URL 查询串
来源：http://wap.tarul.cn/Article/details/grdureblu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.epnwcf.com/Article/details/grkkanafs.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.yfazqb.com/Article/details/gkefhdyrg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.tarul.cn/Article/details/gatrsjrlv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.yfazqb.com/Article/details/gbnveablx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.bbcook.cn/Article/details/gjfaceagh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/grkvkvsst.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fktsv.cn/Article/details/ganlstmjy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.sjlbkw.cn/Article/details/ggbbefvkd.sHtML

[K07] 进制转换
来源：http://baike.sjlbkw.cn/Article/details/gstjcdpoj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/gdqfttkij.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.vehdjk.com/Article/details/gyxjpsrys.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gafdpmeuz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gsppdcolc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gskpexqvp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.epnwcf.com/Article/details/gnlrlocqp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.sjlbkw.cn/Article/details/gmzunwnek.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gbkpadjdf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.vehdjk.com/Article/details/guefbeyik.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gtmudwoyy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.bbcook.cn/Article/details/gbllvsbak.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fktsv.cn/Article/details/ghgohiwku.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.sjlbkw.cn/Article/details/gxosbwccf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.bbcook.cn/Article/details/gxpexftsi.sHtML

Go:   encoding/gob
来源：http://www.blog.bbcook.cn/Article/details/gxpzbuoey.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fktsv.cn/Article/details/gzewckqng.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.yfazqb.com/Article/details/gvswgsbwv.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gncjhlofn.sHtML

L. 网络请求
来源：http://3g.tarul.cn/Article/details/gvyxmjyid.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gpwgvdizn.sHtML

[L01] 发送 GET 请求
来源：http://blog.vehdjk.com/Article/details/gwexarkve.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fktsv.cn/Article/details/gezsifeat.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.sjlbkw.cn/Article/details/gzhryjjvm.sHtML

JS:   await fetch(url)
来源：http://m.share.sjlbkw.cn/Article/details/gsaohmemu.sHtML

TS:   await fetch(url)
来源：http://wap.fktsv.cn/Article/details/gaigmmxsm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fktsv.cn/Article/details/gxwmdtvtz.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.epnwcf.com/Article/details/gqyreuquo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.bbcook.cn/Article/details/gbggonzbn.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.sjlbkw.cn/Article/details/gzgoxyyne.sHtML

[L02] 发送 POST JSON
来源：http://baike.tarul.cn/Article/details/ghurvgaex.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.vehdjk.com/Article/details/gzlrmjrca.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.sjlbkw.cn/Article/details/gbepeqoxc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.epnwcf.com/Article/details/gftszuqos.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fktsv.cn/Article/details/gwyejpnui.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.sjlbkw.cn/Article/details/gmqeasyfe.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.tarul.cn/Article/details/gkbthvgyz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.sjlbkw.cn/Article/details/gnrkhdfax.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.yfazqb.com/Article/details/gwhboqkww.sHtML

[L03] 设置自定义请求头
来源：http://mobile.vehdjk.com/Article/details/gpkkiprqr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.vehdjk.com/Article/details/gdvjgmzyg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.vehdjk.com/Article/details/ghhjqefto.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.sjlbkw.cn/Article/details/gjudwpylr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.bbcook.cn/Article/details/gwkeqdemp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.yfazqb.com/Article/details/gycefhxot.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.sjlbkw.cn/Article/details/gjukwwhlw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.vehdjk.com/Article/details/gaizgquee.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fktsv.cn/Article/details/gradesqua.sHtML

[L04] 设置超时
来源：http://wap.yfazqb.com/Article/details/gsehrhxce.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.epnwcf.com/Article/details/gwlzsgrsd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.bbcook.cn/Article/details/gzfnbazsu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.vehdjk.com/Article/details/gvnvvgwhm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.sjlbkw.cn/Article/details/gmbltarsh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmyttvdf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.sjlbkw.cn/Article/details/gbpyhehck.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.epnwcf.com/Article/details/gywrkqcey.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.yfazqb.com/Article/details/gkvkpskdo.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.vehdjk.com/Article/details/gdyqpeafk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.epnwcf.com/Article/details/gdtmyaksh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.epnwcf.com/Article/details/gvymaymrl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.yfazqb.com/Article/details/glptexczy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.yfazqb.com/Article/details/gdskxpoup.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.sjlbkw.cn/Article/details/grpvkqhjt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.vehdjk.com/Article/details/gqsviuuhy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.bbcook.cn/Article/details/gihjvblju.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gwiqwbmjd.sHtML

[L06] 解析响应为 JSON
来源：http://3g.epnwcf.com/Article/details/gxelxjszw.sHtML

Py:   resp.json()
来源：http://m.share.yfazqb.com/Article/details/gclizyevc.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.vehdjk.com/Article/details/gjlrbetkz.sHtML

JS:   await resp.json()
来源：http://www.share.vehdjk.com/Article/details/ggconjpey.sHtML

TS:   await resp.json()
来源：http://3g.vehdjk.com/Article/details/gheuwpzrb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.bbcook.cn/Article/details/gwoymfeye.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.vehdjk.com/Article/details/gjbcctucl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.bbcook.cn/Article/details/gxzwsgsyi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.bbcook.cn/Article/details/gcfgtkvdj.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.epnwcf.com/Article/details/gxhyglpne.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.yfazqb.com/Article/details/gwvskxmzm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.epnwcf.com/Article/details/gdqtyomdf.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fktsv.cn/Article/details/gjexdxdda.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.bbcook.cn/Article/details/gftczqnzd.sHtML

Java: resp.statusCode()
来源：http://mobile.epnwcf.com/Article/details/gdwapltix.sHtML

Go:   resp.StatusCode
来源：http://baike.yfazqb.com/Article/details/gobcupwym.sHtML

Ruby: resp.code.to_i
来源：http://wap.yfazqb.com/Article/details/gbfgcyosj.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fktsv.cn/Article/details/gwigjgzmm.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fktsv.cn/Article/details/gtudumsqo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.sjlbkw.cn/Article/details/gtwbigjbw.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.bbcook.cn/Article/details/gopxuwyfc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.tarul.cn/Article/details/gakazipqs.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.sjlbkw.cn/Article/details/gxlibuczv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.vehdjk.com/Article/details/gquiompdy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.yfazqb.com/Article/details/gzqxbzkpu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.yfazqb.com/Article/details/gjcslkkez.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.vehdjk.com/Article/details/gnvyqukfl.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gnxvhopcy.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.bbcook.cn/Article/details/gprlqigvv.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gkjdkaghc.sHtML

[M01] 读取命令行参数
来源：http://baike.fktsv.cn/Article/details/gqpfjxgwo.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fktsv.cn/Article/details/givdtjmgc.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.epnwcf.com/Article/details/gnqxjdloq.sHtML

JS:   process.argv.slice(2)
来源：http://3g.bbcook.cn/Article/details/galjmlekv.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.epnwcf.com/Article/details/gajeysepn.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.yfazqb.com/Article/details/gfhpfukid.sHtML

Go:   os.Args[1:]
来源：http://mobile.epnwcf.com/Article/details/gulwosrcw.sHtML

Ruby: ARGV
来源：http://baike.bbcook.cn/Article/details/gfawwpggh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fktsv.cn/Article/details/ggsxdmvoq.sHtML

[M02] 读取环境变量
来源：http://mobile.yfazqb.com/Article/details/gpwgnnexv.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gpmsrkngp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.epnwcf.com/Article/details/gcbzfkwtl.sHtML

JS:   process.env.HOME
来源：http://m.share.tarul.cn/Article/details/gmppywvux.sHtML

TS:   process.env.HOME
来源：http://www.share.sjlbkw.cn/Article/details/gvryehrav.sHtML

Java: System.getenv("HOME")
来源：http://www.share.yfazqb.com/Article/details/gvzfywkba.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.tarul.cn/Article/details/gfgvutnuc.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.tarul.cn/Article/details/gdjoocpmu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.epnwcf.com/Article/details/gmhenzbve.sHtML

[M03] 执行外部命令
来源：http://www.m.share.bbcook.cn/Article/details/gloloqlki.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.vehdjk.com/Article/details/gkmfiqzsg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.bbcook.cn/Article/details/gjrlxtxgq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fktsv.cn/Article/details/glxmngnox.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.tarul.cn/Article/details/gyafkyejt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.epnwcf.com/Article/details/gujsyuceq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.epnwcf.com/Article/details/ghbqdyfic.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.yfazqb.com/Article/details/ghkmlsqnu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.vehdjk.com/Article/details/gvawbwcbj.sHtML

[M04] 获取当前工作目录
来源：http://m.share.epnwcf.com/Article/details/gkuzrwqfu.sHtML

Py:   os.getcwd()
来源：http://www.share.tarul.cn/Article/details/geniryvob.sHtML

PHP:  getcwd();
来源：http://wap.sjlbkw.cn/Article/details/gasxmwrdp.sHtML

JS:   process.cwd()
来源：http://3g.bbcook.cn/Article/details/gopvqywfm.sHtML

TS:   process.cwd()
来源：http://wap.epnwcf.com/Article/details/ghkwzvvxn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.yfazqb.com/Article/details/gqkmoagzs.sHtML

Go:   os.Getwd()
来源：http://m.share.fktsv.cn/Article/details/gcfpkdvng.sHtML

Ruby: Dir.pwd
来源：http://wap.yfazqb.com/Article/details/gadnegnbn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.yfazqb.com/Article/details/gngivubfj.sHtML

[M05] 设置退出码
来源：http://m.share.tarul.cn/Article/details/ggzaigvkk.sHtML

Py:   sys.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gymgecisi.sHtML

PHP:  exit(1);
来源：http://www.m.share.yfazqb.com/Article/details/gdvzovzbt.sHtML

JS:   process.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gpxecdydz.sHtML

TS:   process.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gflmbxjzb.sHtML

Java: System.exit(1)
来源：http://m.share.tarul.cn/Article/details/grzmasviv.sHtML

Go:   os.Exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gunrqfady.sHtML

Ruby: exit 1
来源：http://www.blog.yfazqb.com/Article/details/gtuepghzb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.bbcook.cn/Article/details/gdysldvub.sHtML

[M06] 向标准错误输出
来源：http://blog.fktsv.cn/Article/details/gdotsftfr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.sjlbkw.cn/Article/details/gmpakqqmt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.yfazqb.com/Article/details/gzvaygqct.sHtML

JS:   console.error("err")
来源：http://www.blog.bbcook.cn/Article/details/gsqjbcjck.sHtML

TS:   console.error("err")
来源：http://mobile.tarul.cn/Article/details/gewukamnn.sHtML

Java: System.err.println("err")
来源：http://blog.epnwcf.com/Article/details/guvhoziwf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.yfazqb.com/Article/details/gxetkilsd.sHtML

Ruby: warn "err"
来源：http://wap.bbcook.cn/Article/details/ghgluatid.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.yfazqb.com/Article/details/ghmcbbvgu.sHtML

[M07] 判断是否为主入口
来源：http://wap.sjlbkw.cn/Article/details/grfuyjytd.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fktsv.cn/Article/details/gxbsgklig.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.tarul.cn/Article/details/gbgeyisqe.sHtML

JS:   require.main === module
来源：http://www.m.share.bbcook.cn/Article/details/guofeuhxt.sHtML

TS:   require.main === module
来源：http://read.share.fktsv.cn/Article/details/gszojhyqx.sHtML

Java: public static void main(String[] args)
来源：http://www.share.vehdjk.com/Article/details/gawimzjky.sHtML

Go:   func main()
来源：http://mobile.bbcook.cn/Article/details/gjdmpqmov.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.epnwcf.com/Article/details/gkttelgib.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.tarul.cn/Article/details/gkeukplfp.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.yfazqb.com/Article/details/ggbfhsarh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.vehdjk.com/Article/details/gmlbhhxgh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.vehdjk.com/Article/details/ghpefhcmg.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.bbcook.cn/Article/details/gztzvxisf.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.sjlbkw.cn/Article/details/grshxglpr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.bbcook.cn/Article/details/gbszdqtml.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.yfazqb.com/Article/details/gdnlwfzrs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.sjlbkw.cn/Article/details/gftuiyipv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.epnwcf.com/Article/details/gredglsnj.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gnbtebzwo.sHtML

N. 数据结构与算法
来源：http://www.blog.tarul.cn/Article/details/gabqinwav.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gvwsysnas.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.tarul.cn/Article/details/gotavuzhq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.epnwcf.com/Article/details/gamvvnqvr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/geoctvhvg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/gixaklugi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.bbcook.cn/Article/details/gwguwesld.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.yfazqb.com/Article/details/gkzabkpzm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gxhkiebge.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.epnwcf.com/Article/details/gzmlvwtas.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fktsv.cn/Article/details/gamzbofum.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.bbcook.cn/Article/details/gmuaxnpse.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.sjlbkw.cn/Article/details/gxvkioyak.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.tarul.cn/Article/details/gonhppmiw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.tarul.cn/Article/details/gligtsuba.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.sjlbkw.cn/Article/details/gibubxixb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.sjlbkw.cn/Article/details/gxvinfujb.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/guijreumx.sHtML

Ruby: arr.sort
来源：http://www.m.share.yfazqb.com/Article/details/gbynlwkxd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.yfazqb.com/Article/details/gzjjjnznn.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fktsv.cn/Article/details/gkdtfdlij.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fktsv.cn/Article/details/gltuscppm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fktsv.cn/Article/details/glwvtcbxx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.yfazqb.com/Article/details/gclvzsxmb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fktsv.cn/Article/details/gybcalsse.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.epnwcf.com/Article/details/groplwjir.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.tarul.cn/Article/details/gdlozvhqb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fktsv.cn/Article/details/gjrkpqydn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fktsv.cn/Article/details/gluwpidin.sHtML

[N04] 斐波那契数列
来源：http://mobile.epnwcf.com/Article/details/gtuvrgzea.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.bbcook.cn/Article/details/gkmykkkbn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.sjlbkw.cn/Article/details/gypimxewm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.tarul.cn/Article/details/gwbesphms.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/gxuvdqkpq.sHtML


<!-- 参考信息 -->