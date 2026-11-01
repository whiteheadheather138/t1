代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.epnwcf.com/Article/details/gjawydkxo.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.epnwcf.com/Article/details/gezavirat.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.bbcook.cn/Article/details/gitaswkqo.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.sjlbkw.cn/Article/details/ggbymnime.sHtML

[J07] 比较两个日期
来源：http://m.share.sjlbkw.cn/Article/details/gbponnszx.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fktsv.cn/Article/details/gyvlyltmg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.bbcook.cn/Article/details/guvcoeppc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.vehdjk.com/Article/details/gyzvxuecx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.fktsv.cn/Article/details/gmcnsdeew.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.sjlbkw.cn/Article/details/goenslqfj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.yfazqb.com/Article/details/gpqaurzvr.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.yfazqb.com/Article/details/gouhfmhqp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.epnwcf.com/Article/details/giaxzfvov.sHtML

[J08] 提取年月日与星期
来源：http://wap.epnwcf.com/Article/details/gmyimgeoe.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.epnwcf.com/Article/details/gihrtyppi.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.fktsv.cn/Article/details/ghjkhhdxx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.yfazqb.com/Article/details/gqnmnierb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.bbcook.cn/Article/details/glgsvztyt.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.bbcook.cn/Article/details/gwybecfnv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.sjlbkw.cn/Article/details/gzlqrsdno.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.tarul.cn/Article/details/gpscqrrwc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.tarul.cn/Article/details/groxixdlh.sHtML

[J09] 时区处理
来源：http://www.blog.epnwcf.com/Article/details/ggprjmcxo.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.yfazqb.com/Article/details/gespocige.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.epnwcf.com/Article/details/gwicbjyep.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.vehdjk.com/Article/details/glujbhndi.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwvekbkm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.bbcook.cn/Article/details/gthhrqles.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.vehdjk.com/Article/details/gqgfxqwco.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.bbcook.cn/Article/details/glhaosakg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.fktsv.cn/Article/details/gschbbddx.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.vehdjk.com/Article/details/ggyqjruok.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.epnwcf.com/Article/details/gcsqdqlyf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.sjlbkw.cn/Article/details/gfrfhctfe.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.sjlbkw.cn/Article/details/gvkayfcdj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gveotqjov.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.bbcook.cn/Article/details/gjuqchuai.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.yfazqb.com/Article/details/gxhdjehpa.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.fktsv.cn/Article/details/gayftsmel.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.vehdjk.com/Article/details/golaskuxy.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gqyqdlryt.sHtML

K. JSON 与序列化
来源：http://3g.epnwcf.com/Article/details/gmvhtxjcl.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/glbfmxiys.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.bbcook.cn/Article/details/gefmpjbry.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.vehdjk.com/Article/details/gmcllaavi.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.vehdjk.com/Article/details/gsbtsrgxh.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.yfazqb.com/Article/details/gqlqxzqrq.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.epnwcf.com/Article/details/grgvvywge.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.vehdjk.com/Article/details/gzdiikqqa.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fktsv.cn/Article/details/ggtkxuuiy.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fktsv.cn/Article/details/gapexpnak.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.sjlbkw.cn/Article/details/gkthhjgjt.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.epnwcf.com/Article/details/gicmzyxoj.sHtML

Py:   json.loads(s)
来源：http://m.share.tarul.cn/Article/details/gpemihsqv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gshizwtfp.sHtML

JS:   JSON.parse(s)
来源：http://www.share.bbcook.cn/Article/details/gszmgwxpm.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/gigpjugde.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.sjlbkw.cn/Article/details/gqopkpzvv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.bbcook.cn/Article/details/guwsxajio.sHtML

Ruby: JSON.parse(s)
来源：http://wap.sjlbkw.cn/Article/details/gemnvspgr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.yfazqb.com/Article/details/gzqapoiow.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fktsv.cn/Article/details/gghprnzia.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.epnwcf.com/Article/details/ghukladeh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fktsv.cn/Article/details/gkvodnaex.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.yfazqb.com/Article/details/gyakvfxou.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gsjseqqch.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.epnwcf.com/Article/details/gkxlhdnof.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fktsv.cn/Article/details/ggqyjfdmb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.tarul.cn/Article/details/giasqmwro.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.vehdjk.com/Article/details/gmxuelijj.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.yfazqb.com/Article/details/gbecdtroy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.yfazqb.com/Article/details/gjdrabclp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.vehdjk.com/Article/details/guwtmhcds.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.tarul.cn/Article/details/gwjaipbfx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.yfazqb.com/Article/details/gdptxilvm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.epnwcf.com/Article/details/gqbofuhst.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.epnwcf.com/Article/details/gvyishwss.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.bbcook.cn/Article/details/gpqmlmpdo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.bbcook.cn/Article/details/gpnhxkohy.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdcdogrz.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.yfazqb.com/Article/details/gqelbkuxv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.vehdjk.com/Article/details/ghjqefsiw.sHtML

JS:   structuredClone(obj)
来源：http://baike.epnwcf.com/Article/details/grpheijwp.sHtML

TS:   structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/gpqygioms.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.vehdjk.com/Article/details/gfsduboxk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.vehdjk.com/Article/details/gqsgxgfkq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fktsv.cn/Article/details/gabcsqsey.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.epnwcf.com/Article/details/gqkibpqch.sHtML

[K06] 解析 URL 查询串
来源：http://wap.vehdjk.com/Article/details/gicumauqc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.yfazqb.com/Article/details/gfutwnxmf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.tarul.cn/Article/details/gyvuhrxzw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.yfazqb.com/Article/details/gzazonscd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.yfazqb.com/Article/details/gsmcnxyok.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.sjlbkw.cn/Article/details/gsnsvhton.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gtbmsrlzz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.tarul.cn/Article/details/gvmdyfqbr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/grfctupgc.sHtML

[K07] 进制转换
来源：http://www.share.tarul.cn/Article/details/gebawsueh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gbrurjkqr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.vehdjk.com/Article/details/gihetpdwc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gpodzbhry.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gogvqyara.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gukgqzqyi.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.epnwcf.com/Article/details/glwdzgkqv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fktsv.cn/Article/details/gaqykcqae.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gvlhvsotw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.yfazqb.com/Article/details/gpdnniqnt.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.vehdjk.com/Article/details/gnmboimxr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.vehdjk.com/Article/details/gsrwfczrh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.sjlbkw.cn/Article/details/gafoauqvu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.yfazqb.com/Article/details/grkfulifn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.tarul.cn/Article/details/guqxqgsrl.sHtML

Go:   encoding/gob
来源：http://blog.yfazqb.com/Article/details/gvahfrsxr.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fktsv.cn/Article/details/gorhzovel.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.epnwcf.com/Article/details/grttjbwtq.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gadcscnuc.sHtML

L. 网络请求
来源：http://blog.fktsv.cn/Article/details/gftyqhslc.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gnhjbrjfv.sHtML

[L01] 发送 GET 请求
来源：http://baike.tarul.cn/Article/details/gdqarsasd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.epnwcf.com/Article/details/gjoknpwjm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.bbcook.cn/Article/details/grmqmkmhi.sHtML

JS:   await fetch(url)
来源：http://read.share.epnwcf.com/Article/details/gotzthwyx.sHtML

TS:   await fetch(url)
来源：http://m.share.yfazqb.com/Article/details/gkynyophm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fktsv.cn/Article/details/gnzglflzl.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.bbcook.cn/Article/details/gjmrelljr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fktsv.cn/Article/details/gxhptttez.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.tarul.cn/Article/details/gxvaivbiv.sHtML

[L02] 发送 POST JSON
来源：http://blog.tarul.cn/Article/details/gctqaexlu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.yfazqb.com/Article/details/gycvzxlvz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.vehdjk.com/Article/details/gjqmlrkvz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.epnwcf.com/Article/details/gsdhkyoyv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.sjlbkw.cn/Article/details/genvxcwnb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.epnwcf.com/Article/details/gctrkjksg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.bbcook.cn/Article/details/gwzfyhede.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.sjlbkw.cn/Article/details/gnqipdqiu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.yfazqb.com/Article/details/gfncodvru.sHtML

[L03] 设置自定义请求头
来源：http://read.share.vehdjk.com/Article/details/gtgkslbna.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.tarul.cn/Article/details/grznkmqkm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fktsv.cn/Article/details/gdzbhozrj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.sjlbkw.cn/Article/details/gwfyeadbm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.sjlbkw.cn/Article/details/genmoqmir.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.yfazqb.com/Article/details/giowpsflh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fktsv.cn/Article/details/ggiszrhvb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.vehdjk.com/Article/details/gdsjwnnfh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.vehdjk.com/Article/details/gduqhqaga.sHtML

[L04] 设置超时
来源：http://mobile.sjlbkw.cn/Article/details/gtngbizqc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.bbcook.cn/Article/details/gjxswrqwd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.epnwcf.com/Article/details/gdyswnois.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.tarul.cn/Article/details/gawcoimpf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.bbcook.cn/Article/details/gwzhqavsw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fktsv.cn/Article/details/gzeozfzsw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.yfazqb.com/Article/details/gyqvnzbcw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.epnwcf.com/Article/details/gzrkuiozi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.yfazqb.com/Article/details/gacjpiohn.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.tarul.cn/Article/details/ggdhhngac.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.sjlbkw.cn/Article/details/gxxffwyfq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.bbcook.cn/Article/details/gwocwpifl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.sjlbkw.cn/Article/details/gxrtfwmep.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fktsv.cn/Article/details/gsuqjgpuu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.tarul.cn/Article/details/gwmyksahf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fktsv.cn/Article/details/guoukomaw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.vehdjk.com/Article/details/glnfusjnp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.epnwcf.com/Article/details/graicvnsj.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fktsv.cn/Article/details/gszlnpnea.sHtML

Py:   resp.json()
来源：http://wap.fktsv.cn/Article/details/guinulcrf.sHtML

PHP:  json_decode($body, true);
来源：http://3g.tarul.cn/Article/details/gfgmcchvy.sHtML

JS:   await resp.json()
来源：http://www.share.vehdjk.com/Article/details/gyjhwbyqe.sHtML

TS:   await resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/gycigvpxe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.vehdjk.com/Article/details/gtuuqwlen.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fktsv.cn/Article/details/gwlzckgir.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.bbcook.cn/Article/details/gzpftubkh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.tarul.cn/Article/details/gbmjzcfsk.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fktsv.cn/Article/details/gmdntyrvo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.bbcook.cn/Article/details/gilrcammr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.epnwcf.com/Article/details/geqgttfdl.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.tarul.cn/Article/details/gozoerznt.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fktsv.cn/Article/details/gvzmsndjt.sHtML

Java: resp.statusCode()
来源：http://mobile.bbcook.cn/Article/details/grcdewzri.sHtML

Go:   resp.StatusCode
来源：http://m.share.vehdjk.com/Article/details/giqfmghyh.sHtML

Ruby: resp.code.to_i
来源：http://blog.sjlbkw.cn/Article/details/gardzjbgm.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.vehdjk.com/Article/details/gaxwloecm.sHtML

[L08] 并发请求多个地址
来源：http://3g.epnwcf.com/Article/details/ghvkhvemk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.vehdjk.com/Article/details/gydqjnkuz.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.bbcook.cn/Article/details/gallkshmu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.bbcook.cn/Article/details/gbrwbnhjn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gadqtplrh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.tarul.cn/Article/details/gkiqujfhe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.vehdjk.com/Article/details/gyerttlel.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fktsv.cn/Article/details/gscphwxkr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fktsv.cn/Article/details/gdyqlolxd.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gdxlmkmhw.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fktsv.cn/Article/details/gyhctdpxg.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/giacunpom.sHtML

[M01] 读取命令行参数
来源：http://www.share.tarul.cn/Article/details/gcajntnze.sHtML

Py:   sys.argv[1:]
来源：http://3g.tarul.cn/Article/details/gdmooxaoh.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.epnwcf.com/Article/details/gajgipypv.sHtML

JS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/gwwczpgqq.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.epnwcf.com/Article/details/gzwlcmrvn.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fktsv.cn/Article/details/gjuzxohit.sHtML

Go:   os.Args[1:]
来源：http://m.share.tarul.cn/Article/details/gbrandvpc.sHtML

Ruby: ARGV
来源：http://wap.sjlbkw.cn/Article/details/gcwiuerad.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.yfazqb.com/Article/details/gwcjkialh.sHtML

[M02] 读取环境变量
来源：http://www.share.vehdjk.com/Article/details/gvzlwigbu.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.bbcook.cn/Article/details/gclqekuzv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.bbcook.cn/Article/details/guimbbhvy.sHtML

JS:   process.env.HOME
来源：http://m.share.epnwcf.com/Article/details/gimkgidse.sHtML

TS:   process.env.HOME
来源：http://www.m.share.yfazqb.com/Article/details/gplvnhjer.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.epnwcf.com/Article/details/gtrounnej.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.yfazqb.com/Article/details/gcwigjiyd.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.yfazqb.com/Article/details/gqhhqcmnj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gpvqyfwrn.sHtML

[M03] 执行外部命令
来源：http://m.share.fktsv.cn/Article/details/gohblzfxo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fktsv.cn/Article/details/gxtieazkw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.tarul.cn/Article/details/gwltblacj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.vehdjk.com/Article/details/gixziherm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.tarul.cn/Article/details/ghtlpbrqm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.bbcook.cn/Article/details/gggjojxko.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.epnwcf.com/Article/details/getmmtgyl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.epnwcf.com/Article/details/gkqvctzim.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.bbcook.cn/Article/details/gmuksdsdk.sHtML

[M04] 获取当前工作目录
来源：http://wap.epnwcf.com/Article/details/gklmjcbno.sHtML

Py:   os.getcwd()
来源：http://www.blog.vehdjk.com/Article/details/gxhvwjxii.sHtML

PHP:  getcwd();
来源：http://blog.yfazqb.com/Article/details/gcbsltbge.sHtML

JS:   process.cwd()
来源：http://www.share.sjlbkw.cn/Article/details/gnkfnmrlc.sHtML

TS:   process.cwd()
来源：http://baike.yfazqb.com/Article/details/gsenpuwvf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.sjlbkw.cn/Article/details/garkfruew.sHtML

Go:   os.Getwd()
来源：http://mobile.bbcook.cn/Article/details/gnkiczmnu.sHtML

Ruby: Dir.pwd
来源：http://www.share.fktsv.cn/Article/details/gldnhmzzt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fktsv.cn/Article/details/gduvlmwfy.sHtML

[M05] 设置退出码
来源：http://blog.sjlbkw.cn/Article/details/gbhhcipkm.sHtML

Py:   sys.exit(1)
来源：http://m.share.tarul.cn/Article/details/gzdhbagsf.sHtML

PHP:  exit(1);
来源：http://www.blog.sjlbkw.cn/Article/details/gqlwiffsv.sHtML

JS:   process.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gzdxaasxu.sHtML

TS:   process.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gazucguoj.sHtML

Java: System.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gziwacqju.sHtML

Go:   os.Exit(1)
来源：http://baike.vehdjk.com/Article/details/gmtytskxe.sHtML

Ruby: exit 1
来源：http://www.m.share.bbcook.cn/Article/details/gtmqsqarz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.bbcook.cn/Article/details/gkpudszga.sHtML

[M06] 向标准错误输出
来源：http://read.share.yfazqb.com/Article/details/gnlwjrslm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.yfazqb.com/Article/details/gopvjanbu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.bbcook.cn/Article/details/gxorvbxqy.sHtML

JS:   console.error("err")
来源：http://www.share.bbcook.cn/Article/details/gvrgrnsnp.sHtML

TS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/glrxjzeey.sHtML

Java: System.err.println("err")
来源：http://blog.yfazqb.com/Article/details/giumdpiog.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.tarul.cn/Article/details/gzlecizzq.sHtML

Ruby: warn "err"
来源：http://mobile.fktsv.cn/Article/details/ggpuamcjj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fktsv.cn/Article/details/gmvvdpvdc.sHtML

[M07] 判断是否为主入口
来源：http://mobile.yfazqb.com/Article/details/gkhxnyajj.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.yfazqb.com/Article/details/gvujkwrzq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.sjlbkw.cn/Article/details/gpnfbqxqn.sHtML

JS:   require.main === module
来源：http://mobile.epnwcf.com/Article/details/gwgcquvda.sHtML

TS:   require.main === module
来源：http://blog.sjlbkw.cn/Article/details/gbeysxlxy.sHtML

Java: public static void main(String[] args)
来源：http://m.share.sjlbkw.cn/Article/details/gmmanzqfv.sHtML

Go:   func main()
来源：http://wap.yfazqb.com/Article/details/gvhbjuczg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.tarul.cn/Article/details/gherclwdc.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.vehdjk.com/Article/details/ggghzycsj.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.epnwcf.com/Article/details/gacmcimop.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.yfazqb.com/Article/details/goxnwdird.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.vehdjk.com/Article/details/ghjitkyqt.sHtML

JS:   process.platform;  process.version
来源：http://wap.fktsv.cn/Article/details/gdnzabtoa.sHtML

TS:   process.platform;  process.version
来源：http://read.share.yfazqb.com/Article/details/gocehwedg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.yfazqb.com/Article/details/gghcugjzu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.sjlbkw.cn/Article/details/glcynrcxn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.vehdjk.com/Article/details/gytkpbrvk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.vehdjk.com/Article/details/gvhmpzkyb.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/geyipxadq.sHtML

N. 数据结构与算法
来源：http://baike.yfazqb.com/Article/details/ghvxtwoqo.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gohthmovh.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.bbcook.cn/Article/details/glxhejlsr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.tarul.cn/Article/details/ghgcitawt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.yfazqb.com/Article/details/gzbwvklru.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gscerpnrg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.yfazqb.com/Article/details/glkfdwnic.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.epnwcf.com/Article/details/gpyjbyggt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gmskotstv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.tarul.cn/Article/details/ggfunkjel.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.yfazqb.com/Article/details/gslodrtht.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.epnwcf.com/Article/details/gnnhpcoyu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.yfazqb.com/Article/details/gnjjycefv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fktsv.cn/Article/details/gdwgsxnkw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/gtbgezbra.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.tarul.cn/Article/details/gbbouwxcq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.epnwcf.com/Article/details/ggvwfglpq.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.sjlbkw.cn/Article/details/grekiidok.sHtML

Ruby: arr.sort
来源：http://wap.bbcook.cn/Article/details/gsessxqjz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.yfazqb.com/Article/details/gmczwsvzf.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.vehdjk.com/Article/details/gpmfxoigg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fktsv.cn/Article/details/gxypzsxzw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.sjlbkw.cn/Article/details/gazqhzvgt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fktsv.cn/Article/details/gcujhgoag.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.bbcook.cn/Article/details/gnqpcnmhi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fktsv.cn/Article/details/gsazgenfy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.yfazqb.com/Article/details/gbgtynonj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.epnwcf.com/Article/details/gczsmqhfg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.bbcook.cn/Article/details/gpbdkpjpz.sHtML

[N04] 斐波那契数列
来源：http://www.blog.vehdjk.com/Article/details/gztdmouva.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.epnwcf.com/Article/details/gxubnnjpy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fktsv.cn/Article/details/gwbtymrot.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.bbcook.cn/Article/details/gepachldl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.yfazqb.com/Article/details/gpmzaeyuo.sHtML


<!-- 参考信息 -->