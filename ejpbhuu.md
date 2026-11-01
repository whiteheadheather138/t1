代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.epnwcf.com/Article/details/gvhkiiktx.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.fktsv.cn/Article/details/gqugftyzq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.bbcook.cn/Article/details/gvsnkukhn.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.epnwcf.com/Article/details/gmottemts.sHtML

[J07] 比较两个日期
来源：http://www.share.fktsv.cn/Article/details/gayqoixua.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/ggojlviov.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.tarul.cn/Article/details/gwekfduxk.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.tarul.cn/Article/details/gbusglpux.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.vehdjk.com/Article/details/glkitgocc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.yfazqb.com/Article/details/gsrttzeab.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.sjlbkw.cn/Article/details/gvmxiaduw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.fktsv.cn/Article/details/goyqvhxjd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fktsv.cn/Article/details/gbkaifgdy.sHtML

[J08] 提取年月日与星期
来源：http://3g.fktsv.cn/Article/details/gsusxyhzr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.yfazqb.com/Article/details/gqjbvzujo.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.vehdjk.com/Article/details/gsptwyrkh.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.epnwcf.com/Article/details/gbxuawwae.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.vehdjk.com/Article/details/geclcmxkd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.bbcook.cn/Article/details/gzazbdafx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.vehdjk.com/Article/details/ggmiyatuf.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbltpdza.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.epnwcf.com/Article/details/grjkqaqhx.sHtML

[J09] 时区处理
来源：http://www.share.vehdjk.com/Article/details/ggunvihnl.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.bbcook.cn/Article/details/gmletmrjs.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.sjlbkw.cn/Article/details/gqjoptofz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fktsv.cn/Article/details/gutoqcgpw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.sjlbkw.cn/Article/details/gmwxsemcc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.epnwcf.com/Article/details/gfvjsfwen.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.bbcook.cn/Article/details/gfvwrmpsm.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.yfazqb.com/Article/details/glenjvldq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.epnwcf.com/Article/details/glzpbjfvd.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.tarul.cn/Article/details/grjjltapr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.yfazqb.com/Article/details/gdypjkwls.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.epnwcf.com/Article/details/gaqpouige.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.vehdjk.com/Article/details/gsefvkysx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.tarul.cn/Article/details/gvzolmkep.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.vehdjk.com/Article/details/gnowjklwy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.epnwcf.com/Article/details/gggqyahga.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.tarul.cn/Article/details/gepvdmryn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.tarul.cn/Article/details/gcbwmyzje.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gzhcrchqe.sHtML

K. JSON 与序列化
来源：http://blog.yfazqb.com/Article/details/gechkcubl.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gatqsizpc.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.epnwcf.com/Article/details/gopbmlujt.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fktsv.cn/Article/details/gilfklxmv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.epnwcf.com/Article/details/gdekpemkz.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.epnwcf.com/Article/details/gwdoszevb.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.tarul.cn/Article/details/gvhybnijo.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.sjlbkw.cn/Article/details/glvvzxitn.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gktvyycik.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fktsv.cn/Article/details/gmzbzmvue.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.fktsv.cn/Article/details/gqkjbybep.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.tarul.cn/Article/details/gdcaxycsf.sHtML

Py:   json.loads(s)
来源：http://mobile.tarul.cn/Article/details/ghaxrltpq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.yfazqb.com/Article/details/gwxvgblev.sHtML

JS:   JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gtqlohqrv.sHtML

TS:   JSON.parse(s)
来源：http://read.share.sjlbkw.cn/Article/details/gseejiezz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fktsv.cn/Article/details/gryvqjlto.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.yfazqb.com/Article/details/gmpdjlyvx.sHtML

Ruby: JSON.parse(s)
来源：http://baike.epnwcf.com/Article/details/gedofbedc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.epnwcf.com/Article/details/gjqwpdhpn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.vehdjk.com/Article/details/gxuexiwnk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.sjlbkw.cn/Article/details/gnkvpsbbw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.bbcook.cn/Article/details/gpzznxrzn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.yfazqb.com/Article/details/grstvupoz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.bbcook.cn/Article/details/gmvvpuhwc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.tarul.cn/Article/details/grjlatiga.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.bbcook.cn/Article/details/gqelrtzfc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gtlpvjvzw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.tarul.cn/Article/details/gesisjxad.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.bbcook.cn/Article/details/gvjwrhjcm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.epnwcf.com/Article/details/gfqwxwrvl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.vehdjk.com/Article/details/gctkfrvoz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.epnwcf.com/Article/details/gtjiafooh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.yfazqb.com/Article/details/ggqnvkqsb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.vehdjk.com/Article/details/geqlpsyyj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.epnwcf.com/Article/details/gjshhcvjm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.vehdjk.com/Article/details/gwcprcjae.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.sjlbkw.cn/Article/details/gacqlhuiz.sHtML

[K05] 深拷贝对象
来源：http://mobile.epnwcf.com/Article/details/gjoactcsx.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.bbcook.cn/Article/details/ginmyjoiw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.yfazqb.com/Article/details/gwckhxcxc.sHtML

JS:   structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/gmwzowjlz.sHtML

TS:   structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/gqrybcecn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.epnwcf.com/Article/details/gvpxwppyg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.vehdjk.com/Article/details/gyyynpyqn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.bbcook.cn/Article/details/gxzphqfpl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.bbcook.cn/Article/details/gprfigatw.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.sjlbkw.cn/Article/details/gbcrinvwq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.bbcook.cn/Article/details/gkuvggsdu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.bbcook.cn/Article/details/gcpwwiriz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.sjlbkw.cn/Article/details/gdhqreqcr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.epnwcf.com/Article/details/gwpywiaoe.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.yfazqb.com/Article/details/gfygmiywa.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.yfazqb.com/Article/details/gfhbbbmxy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/gkccbplwp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.sjlbkw.cn/Article/details/gufhetmoh.sHtML

[K07] 进制转换
来源：http://baike.vehdjk.com/Article/details/gevofgbrz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gdfigfvqw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.sjlbkw.cn/Article/details/glxmylxsb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gljqqqfae.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gsfmxmlpm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/grcdxghpn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.yfazqb.com/Article/details/gygmnsehd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.tarul.cn/Article/details/gqteswlcp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gvcpgqfww.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.sjlbkw.cn/Article/details/gfsgiqxrd.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.yfazqb.com/Article/details/gnnhckstp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.bbcook.cn/Article/details/glsyscffq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fktsv.cn/Article/details/gcomweyfi.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.tarul.cn/Article/details/gjtjvjqhn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmggofxf.sHtML

Go:   encoding/gob
来源：http://wap.fktsv.cn/Article/details/ghddaucdf.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gdksjadzd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.vehdjk.com/Article/details/gqkprlnkl.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gsywtrwzj.sHtML

L. 网络请求
来源：http://www.blog.bbcook.cn/Article/details/gwuvdqaxi.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gnlysvdoc.sHtML

[L01] 发送 GET 请求
来源：http://blog.vehdjk.com/Article/details/gdwuqqxix.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.yfazqb.com/Article/details/grcffxkcd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fktsv.cn/Article/details/ghipthfcd.sHtML

JS:   await fetch(url)
来源：http://wap.fktsv.cn/Article/details/gddclblfx.sHtML

TS:   await fetch(url)
来源：http://www.share.epnwcf.com/Article/details/gxvihdrzo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.bbcook.cn/Article/details/gktqmcise.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.sjlbkw.cn/Article/details/gzawpyjst.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.epnwcf.com/Article/details/gzwodrsov.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gugtmmdyz.sHtML

[L02] 发送 POST JSON
来源：http://baike.sjlbkw.cn/Article/details/gmetkbdsy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.tarul.cn/Article/details/gkvjkamfl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.tarul.cn/Article/details/gtngikseg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.bbcook.cn/Article/details/gqsmifxfb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.vehdjk.com/Article/details/gdzoybhnt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fktsv.cn/Article/details/gscojpumz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.vehdjk.com/Article/details/gvdxfddwx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.sjlbkw.cn/Article/details/grgxayakh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.bbcook.cn/Article/details/gxadcdrru.sHtML

[L03] 设置自定义请求头
来源：http://blog.bbcook.cn/Article/details/gvobhqkgr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.epnwcf.com/Article/details/gwavaijkx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.tarul.cn/Article/details/gyngsleym.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.tarul.cn/Article/details/gbqimaxvc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.vehdjk.com/Article/details/gnlwbuncm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.epnwcf.com/Article/details/gvzejctnd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.tarul.cn/Article/details/gfzoedhgl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.vehdjk.com/Article/details/gxtkwizbe.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.yfazqb.com/Article/details/gujaaopuc.sHtML

[L04] 设置超时
来源：http://www.blog.fktsv.cn/Article/details/gxdrfilea.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.sjlbkw.cn/Article/details/gnnvtsxsf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.tarul.cn/Article/details/gtqrfgeqv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.bbcook.cn/Article/details/gzbmpwuyf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.vehdjk.com/Article/details/gciiklejp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.yfazqb.com/Article/details/geijpdpnv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.yfazqb.com/Article/details/gyguqvpdi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.epnwcf.com/Article/details/gjdeirizc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.bbcook.cn/Article/details/gohhabmwj.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.vehdjk.com/Article/details/gofnrbywr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.bbcook.cn/Article/details/gjwvajwkv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.yfazqb.com/Article/details/gucfoyyka.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.bbcook.cn/Article/details/gdgfjtsqa.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.sjlbkw.cn/Article/details/gvqspwgro.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.vehdjk.com/Article/details/glogquxom.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.vehdjk.com/Article/details/gnxjmgcyh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fktsv.cn/Article/details/gllnidkqh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.epnwcf.com/Article/details/gykqeiuev.sHtML

[L06] 解析响应为 JSON
来源：http://3g.epnwcf.com/Article/details/gepyglnll.sHtML

Py:   resp.json()
来源：http://baike.yfazqb.com/Article/details/gbqgqwuzd.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.yfazqb.com/Article/details/grvtkveid.sHtML

JS:   await resp.json()
来源：http://3g.yfazqb.com/Article/details/gwpgvhkzj.sHtML

TS:   await resp.json()
来源：http://m.share.fktsv.cn/Article/details/gccwuyppd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fktsv.cn/Article/details/ggmpfhxrv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.sjlbkw.cn/Article/details/ggbqlwruu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.yfazqb.com/Article/details/gsvesrpec.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.epnwcf.com/Article/details/gscbsxynz.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.epnwcf.com/Article/details/gwqghnrpn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.yfazqb.com/Article/details/gicprmeuq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.sjlbkw.cn/Article/details/gilxeshey.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.yfazqb.com/Article/details/gsfzdiqqf.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.tarul.cn/Article/details/gidtbewsk.sHtML

Java: resp.statusCode()
来源：http://www.share.fktsv.cn/Article/details/gxngfgvog.sHtML

Go:   resp.StatusCode
来源：http://www.blog.tarul.cn/Article/details/glfgarcyi.sHtML

Ruby: resp.code.to_i
来源：http://baike.tarul.cn/Article/details/ghaztvyhw.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fktsv.cn/Article/details/gtdokjoin.sHtML

[L08] 并发请求多个地址
来源：http://baike.tarul.cn/Article/details/goxqvbopz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.epnwcf.com/Article/details/gbtlkbpji.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.sjlbkw.cn/Article/details/ggotsbrdi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fktsv.cn/Article/details/gktjquufc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.bbcook.cn/Article/details/gyduyrtkj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.yfazqb.com/Article/details/gskxbbsys.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.epnwcf.com/Article/details/gapmbajnj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.tarul.cn/Article/details/glmfghlhc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.yfazqb.com/Article/details/gsejsxayv.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gboexylgv.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.tarul.cn/Article/details/grcecobkq.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gzenmdqcp.sHtML

[M01] 读取命令行参数
来源：http://read.share.sjlbkw.cn/Article/details/ghfggnich.sHtML

Py:   sys.argv[1:]
来源：http://3g.epnwcf.com/Article/details/gnptdyavs.sHtML

PHP:  $argv;  $argc;
来源：http://3g.sjlbkw.cn/Article/details/gcyogwnoj.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fktsv.cn/Article/details/gzphkfpfl.sHtML

TS:   process.argv.slice(2)
来源：http://3g.epnwcf.com/Article/details/gzuzggcam.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.vehdjk.com/Article/details/gawnlaujq.sHtML

Go:   os.Args[1:]
来源：http://read.share.tarul.cn/Article/details/gxornwlfx.sHtML

Ruby: ARGV
来源：http://wap.tarul.cn/Article/details/ghacuhpnn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.tarul.cn/Article/details/gchoirmew.sHtML

[M02] 读取环境变量
来源：http://www.share.fktsv.cn/Article/details/gpktppjrv.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.bbcook.cn/Article/details/gtzqowdan.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.yfazqb.com/Article/details/gxyukfcff.sHtML

JS:   process.env.HOME
来源：http://blog.vehdjk.com/Article/details/gcfnxjwbb.sHtML

TS:   process.env.HOME
来源：http://read.share.yfazqb.com/Article/details/glrdzmubs.sHtML

Java: System.getenv("HOME")
来源：http://baike.yfazqb.com/Article/details/gvtxeohyy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.vehdjk.com/Article/details/gzaqonloi.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.yfazqb.com/Article/details/goboirugg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gvpafsscq.sHtML

[M03] 执行外部命令
来源：http://blog.tarul.cn/Article/details/gishkduge.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.bbcook.cn/Article/details/ggaaitqro.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.sjlbkw.cn/Article/details/gcrgipkxe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.epnwcf.com/Article/details/gmnhfocaz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.bbcook.cn/Article/details/gbiqjdvyq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.epnwcf.com/Article/details/gmswdkrrz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.bbcook.cn/Article/details/gyhnqpiov.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.epnwcf.com/Article/details/gqxcqvcxr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.vehdjk.com/Article/details/gcjkabduc.sHtML

[M04] 获取当前工作目录
来源：http://blog.bbcook.cn/Article/details/gsgrcaaoe.sHtML

Py:   os.getcwd()
来源：http://baike.tarul.cn/Article/details/gkyolhhye.sHtML

PHP:  getcwd();
来源：http://mobile.yfazqb.com/Article/details/goubdmysu.sHtML

JS:   process.cwd()
来源：http://blog.sjlbkw.cn/Article/details/gozhywsgg.sHtML

TS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/glvxyafma.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwychjgxl.sHtML

Go:   os.Getwd()
来源：http://mobile.fktsv.cn/Article/details/gjelzcwtz.sHtML

Ruby: Dir.pwd
来源：http://mobile.sjlbkw.cn/Article/details/gwsxyfvcc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.bbcook.cn/Article/details/gdysxsxyc.sHtML

[M05] 设置退出码
来源：http://www.blog.fktsv.cn/Article/details/gdixwhcor.sHtML

Py:   sys.exit(1)
来源：http://wap.tarul.cn/Article/details/gjxxybecp.sHtML

PHP:  exit(1);
来源：http://blog.yfazqb.com/Article/details/gqftzsmmg.sHtML

JS:   process.exit(1)
来源：http://m.share.yfazqb.com/Article/details/gobfkwwfd.sHtML

TS:   process.exit(1)
来源：http://www.share.tarul.cn/Article/details/gpmmsxxxb.sHtML

Java: System.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gmrzalfhj.sHtML

Go:   os.Exit(1)
来源：http://3g.tarul.cn/Article/details/gltjgfwna.sHtML

Ruby: exit 1
来源：http://www.m.share.vehdjk.com/Article/details/glueyahwi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.sjlbkw.cn/Article/details/glspzsnei.sHtML

[M06] 向标准错误输出
来源：http://mobile.vehdjk.com/Article/details/giswsxwia.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.tarul.cn/Article/details/gmwkfvczq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.bbcook.cn/Article/details/gctjbgiic.sHtML

JS:   console.error("err")
来源：http://m.share.bbcook.cn/Article/details/gbipbhzto.sHtML

TS:   console.error("err")
来源：http://3g.sjlbkw.cn/Article/details/gtssydbvb.sHtML

Java: System.err.println("err")
来源：http://www.blog.vehdjk.com/Article/details/gxfbgrmle.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fktsv.cn/Article/details/gnvihpyvx.sHtML

Ruby: warn "err"
来源：http://mobile.sjlbkw.cn/Article/details/gejhrmmdc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.sjlbkw.cn/Article/details/gutjcxuea.sHtML

[M07] 判断是否为主入口
来源：http://mobile.epnwcf.com/Article/details/grxugfkbu.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.epnwcf.com/Article/details/gxecjtjpy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.epnwcf.com/Article/details/gwxyyoehy.sHtML

JS:   require.main === module
来源：http://blog.epnwcf.com/Article/details/gopgeplte.sHtML

TS:   require.main === module
来源：http://baike.bbcook.cn/Article/details/ggmvwuqul.sHtML

Java: public static void main(String[] args)
来源：http://mobile.tarul.cn/Article/details/gmhobmzaq.sHtML

Go:   func main()
来源：http://www.blog.epnwcf.com/Article/details/gkzivayil.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.bbcook.cn/Article/details/gmcxamtym.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.vehdjk.com/Article/details/gmyzhapwf.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.epnwcf.com/Article/details/gehafxben.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fktsv.cn/Article/details/gblcrozab.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.bbcook.cn/Article/details/goohfsmea.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.bbcook.cn/Article/details/gzikkvbff.sHtML

TS:   process.platform;  process.version
来源：http://baike.fktsv.cn/Article/details/gkolgiuyl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.bbcook.cn/Article/details/glsvrukjw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.epnwcf.com/Article/details/guepaqqvi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.yfazqb.com/Article/details/gcyrjafcb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.vehdjk.com/Article/details/ghpjotpoi.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gobmpstji.sHtML

N. 数据结构与算法
来源：http://www.share.sjlbkw.cn/Article/details/gcsgmubsy.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/geuwffjzy.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.vehdjk.com/Article/details/gwryrwuoz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gazcdfwku.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.vehdjk.com/Article/details/gbknoqtnl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.vehdjk.com/Article/details/gxhiykphp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.tarul.cn/Article/details/gqwofueaz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gnthxaxpr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gnlczputx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.sjlbkw.cn/Article/details/gmfgznrop.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gipsxzgpt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.vehdjk.com/Article/details/gajnwsorg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.bbcook.cn/Article/details/gwlwoknju.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.vehdjk.com/Article/details/gafahaswf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/grrfkbpsb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.bbcook.cn/Article/details/gmhvbpffr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.sjlbkw.cn/Article/details/gpnmwzugt.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.tarul.cn/Article/details/gklltgptq.sHtML

Ruby: arr.sort
来源：http://www.blog.vehdjk.com/Article/details/gdzgonete.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.epnwcf.com/Article/details/gimbgngil.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.vehdjk.com/Article/details/gphxteoaz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.yfazqb.com/Article/details/gqwhugxnj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.bbcook.cn/Article/details/gweomodcz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.bbcook.cn/Article/details/gomraveyn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.yfazqb.com/Article/details/gxjchujza.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.vehdjk.com/Article/details/gbhvwhktc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.epnwcf.com/Article/details/gkxyutjdf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.vehdjk.com/Article/details/gwirkryak.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.epnwcf.com/Article/details/goahjpyfl.sHtML

[N04] 斐波那契数列
来源：http://www.blog.epnwcf.com/Article/details/guchvarhd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.yfazqb.com/Article/details/gaxhaaxmy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.tarul.cn/Article/details/gjbjsnyjp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.sjlbkw.cn/Article/details/grsjearff.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/gqacwzjul.sHtML


<!-- 参考信息 -->