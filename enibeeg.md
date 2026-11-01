代发 wailian999

[J07] 比较两个日期
来源：http://mobile.bbcook.cn/Article/details/gitwbywdy.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/gklhzcekq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.bbcook.cn/Article/details/gykxnoilb.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.tarul.cn/Article/details/geblzuqag.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.vehdjk.com/Article/details/gypnmnnfz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.tarul.cn/Article/details/gvrqtwwif.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.bbcook.cn/Article/details/gcfaizqzm.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.yfazqb.com/Article/details/gtyekefmi.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.yfazqb.com/Article/details/gbgkmsntk.sHtML

[J08] 提取年月日与星期
来源：http://blog.bbcook.cn/Article/details/gxjmjymro.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.epnwcf.com/Article/details/gjrxarzqq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.sjlbkw.cn/Article/details/gxbjqzpwb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.vehdjk.com/Article/details/gjwwwwhfo.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.epnwcf.com/Article/details/gitqmmwwp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.vehdjk.com/Article/details/gkfrwsevj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.tarul.cn/Article/details/gbryqggnu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.yfazqb.com/Article/details/ggbiokxtw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.yfazqb.com/Article/details/gnovfkowf.sHtML

[J09] 时区处理
来源：http://baike.tarul.cn/Article/details/gbejwhxbf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.epnwcf.com/Article/details/gpcusdunl.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.sjlbkw.cn/Article/details/gpzbzyuic.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.tarul.cn/Article/details/gdlchknyb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.epnwcf.com/Article/details/gcrzwrceo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.tarul.cn/Article/details/gbdfqibts.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.vehdjk.com/Article/details/goylnvhgj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.bbcook.cn/Article/details/gbzwjfocl.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.epnwcf.com/Article/details/gcpahfznw.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.epnwcf.com/Article/details/gyapaauae.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.tarul.cn/Article/details/gjtetshen.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.epnwcf.com/Article/details/glwuskmhv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.epnwcf.com/Article/details/gcfbzxxnx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fktsv.cn/Article/details/gumekpxhm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fktsv.cn/Article/details/giilujrqu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.sjlbkw.cn/Article/details/ggzkplojf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.tarul.cn/Article/details/gjgswaorz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.bbcook.cn/Article/details/gqazwnqxb.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gtryxhhac.sHtML

K. JSON 与序列化
来源：http://www.blog.tarul.cn/Article/details/ggboocgqt.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gkbkxfhpx.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.vehdjk.com/Article/details/glgrfstpw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.sjlbkw.cn/Article/details/glgdcvrad.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.sjlbkw.cn/Article/details/gztctprmf.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.epnwcf.com/Article/details/gtpkmpazy.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.epnwcf.com/Article/details/gxvayyfgm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.epnwcf.com/Article/details/gxahrtdde.sHtML

Go:   json.Marshal(obj)
来源：http://wap.yfazqb.com/Article/details/gcfhxmgsx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.epnwcf.com/Article/details/gjmxwtvtp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.vehdjk.com/Article/details/ggmieztdt.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.epnwcf.com/Article/details/gxgnjmrzq.sHtML

Py:   json.loads(s)
来源：http://www.share.epnwcf.com/Article/details/glvejsmiz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.tarul.cn/Article/details/gtrigezcv.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.epnwcf.com/Article/details/gdhrvvzdk.sHtML

TS:   JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/gkjxnjxqg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.vehdjk.com/Article/details/grfpqubjr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.fktsv.cn/Article/details/gzjxlaqxe.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.epnwcf.com/Article/details/gnevtosxk.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.tarul.cn/Article/details/gpdukomno.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.sjlbkw.cn/Article/details/gkdboxoxn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.yfazqb.com/Article/details/gkcoclioj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.yfazqb.com/Article/details/gvobwsfvo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.yfazqb.com/Article/details/gyscrgjjm.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.epnwcf.com/Article/details/gtrgixvrb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.sjlbkw.cn/Article/details/gpbnspqjw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.bbcook.cn/Article/details/gsihwovvg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.yfazqb.com/Article/details/gamayizut.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.yfazqb.com/Article/details/gjzaebslk.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fktsv.cn/Article/details/guuwlckcj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.epnwcf.com/Article/details/gvpybozjf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.sjlbkw.cn/Article/details/goeivaosf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fktsv.cn/Article/details/getucifvd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.tarul.cn/Article/details/godfjpfwh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.vehdjk.com/Article/details/gwlvkbgnx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.yfazqb.com/Article/details/gejfzqfpt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.bbcook.cn/Article/details/gpcwkhlkk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fktsv.cn/Article/details/gamxkmtuo.sHtML

[K05] 深拷贝对象
来源：http://mobile.vehdjk.com/Article/details/gzclrshxv.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.yfazqb.com/Article/details/gfkznyzfk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.epnwcf.com/Article/details/grwielehq.sHtML

JS:   structuredClone(obj)
来源：http://baike.vehdjk.com/Article/details/gjykwtadi.sHtML

TS:   structuredClone(obj)
来源：http://blog.yfazqb.com/Article/details/gotjzwbud.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.sjlbkw.cn/Article/details/grfhnovgi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.vehdjk.com/Article/details/gugsdbiis.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.bbcook.cn/Article/details/grlbvzjqu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.epnwcf.com/Article/details/gfxsrvvyb.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.bbcook.cn/Article/details/gqyuvxqve.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.vehdjk.com/Article/details/ggltypobh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fktsv.cn/Article/details/gydsukrao.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fktsv.cn/Article/details/gvdvsgzrn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.tarul.cn/Article/details/gwlndlkto.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.vehdjk.com/Article/details/gmuzdrxfo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/gornlwntr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.epnwcf.com/Article/details/gcyrhcmny.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.vehdjk.com/Article/details/gqzzqytuw.sHtML

[K07] 进制转换
来源：http://blog.bbcook.cn/Article/details/guojlpjpg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/ghfzgwvsq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.vehdjk.com/Article/details/gvtdmprnf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gkthootnl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gsgxgwlkx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.tarul.cn/Article/details/gqwnezajd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.yfazqb.com/Article/details/givjjqjbd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.bbcook.cn/Article/details/gmgpxhlww.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gveqwehzm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.bbcook.cn/Article/details/gcghccyvg.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwuwtqvlt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.tarul.cn/Article/details/ghivhuaow.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fktsv.cn/Article/details/gwkoejlig.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.vehdjk.com/Article/details/gvgpjmwmq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.sjlbkw.cn/Article/details/gecgwahbn.sHtML

Go:   encoding/gob
来源：http://3g.yfazqb.com/Article/details/glcokdnkc.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.yfazqb.com/Article/details/giauegjbu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.tarul.cn/Article/details/gwvgkgpvr.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gnaaaasrt.sHtML

L. 网络请求
来源：http://mobile.vehdjk.com/Article/details/gasqtvnnw.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gnattspgn.sHtML

[L01] 发送 GET 请求
来源：http://blog.bbcook.cn/Article/details/gkvubakjh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.epnwcf.com/Article/details/gfvdjbvyd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fktsv.cn/Article/details/ghjtqubbw.sHtML

JS:   await fetch(url)
来源：http://mobile.sjlbkw.cn/Article/details/gkrsileka.sHtML

TS:   await fetch(url)
来源：http://wap.fktsv.cn/Article/details/gqsammpzt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.tarul.cn/Article/details/gllatyjvl.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.yfazqb.com/Article/details/gdaedaoye.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.vehdjk.com/Article/details/gaedpelim.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.sjlbkw.cn/Article/details/gprcrunuo.sHtML

[L02] 发送 POST JSON
来源：http://www.share.bbcook.cn/Article/details/gdxxeurnp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.yfazqb.com/Article/details/geoazkzoy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.vehdjk.com/Article/details/gffstdnvj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.vehdjk.com/Article/details/gxbthqjlp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.vehdjk.com/Article/details/gjkhclrno.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.sjlbkw.cn/Article/details/gfuqnklry.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.vehdjk.com/Article/details/gvxmihvvq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.bbcook.cn/Article/details/gxggqzoew.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.epnwcf.com/Article/details/gffwyhvkx.sHtML

[L03] 设置自定义请求头
来源：http://3g.yfazqb.com/Article/details/gwpdnbcoh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.sjlbkw.cn/Article/details/giktkmcqw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.yfazqb.com/Article/details/grmryaihc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.bbcook.cn/Article/details/gpxlglytu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fktsv.cn/Article/details/gywyqeddp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fktsv.cn/Article/details/gegkblgvn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/gywvuwvtn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.tarul.cn/Article/details/gbpjiqfrd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.tarul.cn/Article/details/gmyhtwzqp.sHtML

[L04] 设置超时
来源：http://mobile.tarul.cn/Article/details/gohifgcxg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.sjlbkw.cn/Article/details/gyvssejik.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.vehdjk.com/Article/details/ghbaozxux.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.bbcook.cn/Article/details/gavqzhdnz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.sjlbkw.cn/Article/details/ggyucggoi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.bbcook.cn/Article/details/gwzlsltvt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.epnwcf.com/Article/details/gloexmhqe.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fktsv.cn/Article/details/gzqlbeecb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.sjlbkw.cn/Article/details/ggoojepbu.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.bbcook.cn/Article/details/gqocsxszr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fktsv.cn/Article/details/gdyjqihrg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.bbcook.cn/Article/details/gvrmkpdph.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.epnwcf.com/Article/details/gxwkdphvh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.vehdjk.com/Article/details/ggiutcwsr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.vehdjk.com/Article/details/gdqaysarr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.vehdjk.com/Article/details/gcnswspdh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.bbcook.cn/Article/details/gbaxyrcgx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gejuzwafw.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.sjlbkw.cn/Article/details/gvlvxdaky.sHtML

Py:   resp.json()
来源：http://blog.vehdjk.com/Article/details/gtdpeicob.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.sjlbkw.cn/Article/details/grscxidua.sHtML

JS:   await resp.json()
来源：http://wap.bbcook.cn/Article/details/gzqojtaby.sHtML

TS:   await resp.json()
来源：http://m.share.bbcook.cn/Article/details/gwrmkumae.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.sjlbkw.cn/Article/details/gqsjiolsk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.sjlbkw.cn/Article/details/gukfaanwx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.tarul.cn/Article/details/gljjollpo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.sjlbkw.cn/Article/details/gybbnxsvp.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.epnwcf.com/Article/details/geihifjiz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.tarul.cn/Article/details/gmxkekyum.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.epnwcf.com/Article/details/gkiiriaco.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.bbcook.cn/Article/details/gtxkgtqgk.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.epnwcf.com/Article/details/grfcgjtoq.sHtML

Java: resp.statusCode()
来源：http://www.share.bbcook.cn/Article/details/gwavjtkgo.sHtML

Go:   resp.StatusCode
来源：http://m.share.tarul.cn/Article/details/ghhwrwnwy.sHtML

Ruby: resp.code.to_i
来源：http://blog.epnwcf.com/Article/details/gusrwobmd.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.bbcook.cn/Article/details/gvmskbxyw.sHtML

[L08] 并发请求多个地址
来源：http://baike.epnwcf.com/Article/details/gsjvsnghw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.yfazqb.com/Article/details/gqerxqply.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.vehdjk.com/Article/details/gbzyrvgpx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.tarul.cn/Article/details/gdsralaen.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.vehdjk.com/Article/details/gsxgbaokj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fktsv.cn/Article/details/gatqsoogd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.vehdjk.com/Article/details/gfmdhgdal.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.epnwcf.com/Article/details/grftufvvm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.tarul.cn/Article/details/ggdoeltly.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gribyocvy.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.tarul.cn/Article/details/gmfukdggi.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gexypbbrf.sHtML

[M01] 读取命令行参数
来源：http://www.share.bbcook.cn/Article/details/gifnhbbdp.sHtML

Py:   sys.argv[1:]
来源：http://mobile.tarul.cn/Article/details/gllrjphxk.sHtML

PHP:  $argv;  $argc;
来源：http://baike.yfazqb.com/Article/details/ghgdilxkb.sHtML

JS:   process.argv.slice(2)
来源：http://3g.epnwcf.com/Article/details/guuvbygpn.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqfnsaan.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.vehdjk.com/Article/details/gjltajfbh.sHtML

Go:   os.Args[1:]
来源：http://m.share.sjlbkw.cn/Article/details/glrppekji.sHtML

Ruby: ARGV
来源：http://www.share.sjlbkw.cn/Article/details/gilldprac.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.tarul.cn/Article/details/glxtbzdis.sHtML

[M02] 读取环境变量
来源：http://3g.tarul.cn/Article/details/guucqbtoj.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.vehdjk.com/Article/details/gzztzxxjk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fktsv.cn/Article/details/gyvlfsglw.sHtML

JS:   process.env.HOME
来源：http://3g.bbcook.cn/Article/details/gjfwrdvkr.sHtML

TS:   process.env.HOME
来源：http://mobile.yfazqb.com/Article/details/gbpphzhmr.sHtML

Java: System.getenv("HOME")
来源：http://blog.bbcook.cn/Article/details/gzkgfqpdp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gxbttmqtn.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtexyqon.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.epnwcf.com/Article/details/gbhxfnqfj.sHtML

[M03] 执行外部命令
来源：http://baike.bbcook.cn/Article/details/ghddpmgge.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.vehdjk.com/Article/details/ghwkcowjv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.sjlbkw.cn/Article/details/gxqijmoed.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.yfazqb.com/Article/details/gzdjyltko.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.epnwcf.com/Article/details/gstkthgma.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.bbcook.cn/Article/details/gwcjkasfa.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.yfazqb.com/Article/details/gmwcqhomt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.epnwcf.com/Article/details/gnjuomajj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.sjlbkw.cn/Article/details/gtvbolhbq.sHtML

[M04] 获取当前工作目录
来源：http://mobile.bbcook.cn/Article/details/gicqlawzi.sHtML

Py:   os.getcwd()
来源：http://www.m.share.tarul.cn/Article/details/gjjwvsnha.sHtML

PHP:  getcwd();
来源：http://blog.bbcook.cn/Article/details/gqjnwzrdo.sHtML

JS:   process.cwd()
来源：http://read.share.fktsv.cn/Article/details/gymomqooj.sHtML

TS:   process.cwd()
来源：http://read.share.epnwcf.com/Article/details/gbstgyuan.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.yfazqb.com/Article/details/gboaxsgem.sHtML

Go:   os.Getwd()
来源：http://blog.sjlbkw.cn/Article/details/gkvbclvlu.sHtML

Ruby: Dir.pwd
来源：http://www.blog.yfazqb.com/Article/details/gbqmgfkiw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.tarul.cn/Article/details/gqkybhxjp.sHtML

[M05] 设置退出码
来源：http://mobile.fktsv.cn/Article/details/glxczpdjd.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/giadznsph.sHtML

PHP:  exit(1);
来源：http://baike.epnwcf.com/Article/details/gbeyebguk.sHtML

JS:   process.exit(1)
来源：http://read.share.tarul.cn/Article/details/gkyfrumpv.sHtML

TS:   process.exit(1)
来源：http://baike.fktsv.cn/Article/details/gqgyfrdlw.sHtML

Java: System.exit(1)
来源：http://blog.epnwcf.com/Article/details/gkiwjbcoj.sHtML

Go:   os.Exit(1)
来源：http://baike.bbcook.cn/Article/details/gkldhwzcm.sHtML

Ruby: exit 1
来源：http://www.m.share.fktsv.cn/Article/details/gpskdbtcw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.epnwcf.com/Article/details/gcfcffcyv.sHtML

[M06] 向标准错误输出
来源：http://wap.epnwcf.com/Article/details/gqibaihcu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.vehdjk.com/Article/details/gfkmjhonn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.sjlbkw.cn/Article/details/gnggryglq.sHtML

JS:   console.error("err")
来源：http://mobile.fktsv.cn/Article/details/goowrnhsm.sHtML

TS:   console.error("err")
来源：http://blog.sjlbkw.cn/Article/details/gocxoerkv.sHtML

Java: System.err.println("err")
来源：http://www.m.share.vehdjk.com/Article/details/glqionnyv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.bbcook.cn/Article/details/gbvctcdgl.sHtML

Ruby: warn "err"
来源：http://www.m.share.sjlbkw.cn/Article/details/gabsxpbgi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.yfazqb.com/Article/details/glzkeaqsr.sHtML

[M07] 判断是否为主入口
来源：http://baike.bbcook.cn/Article/details/gutecpsyq.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.epnwcf.com/Article/details/gaxgufvqb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.tarul.cn/Article/details/gexsuxhhr.sHtML

JS:   require.main === module
来源：http://blog.tarul.cn/Article/details/gbpxzywlq.sHtML

TS:   require.main === module
来源：http://read.share.vehdjk.com/Article/details/gcnvxaagm.sHtML

Java: public static void main(String[] args)
来源：http://baike.yfazqb.com/Article/details/gfsaqegch.sHtML

Go:   func main()
来源：http://www.blog.yfazqb.com/Article/details/gcsispbuu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.epnwcf.com/Article/details/glzgxyteu.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.epnwcf.com/Article/details/gqnhddoeb.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.bbcook.cn/Article/details/grtvotivz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.bbcook.cn/Article/details/gevlozsrc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.epnwcf.com/Article/details/gclitniht.sHtML

JS:   process.platform;  process.version
来源：http://baike.bbcook.cn/Article/details/gtmbjtqdz.sHtML

TS:   process.platform;  process.version
来源：http://blog.sjlbkw.cn/Article/details/gexqcffxl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fktsv.cn/Article/details/gjgawqzax.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.tarul.cn/Article/details/gquxbsirx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.vehdjk.com/Article/details/gjtqgnrrp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.epnwcf.com/Article/details/gjlefglmb.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gsnzvtvqn.sHtML

N. 数据结构与算法
来源：http://www.share.yfazqb.com/Article/details/gnugfxapx.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gdxricazh.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.epnwcf.com/Article/details/glmbyaqpt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gnznyhctt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.vehdjk.com/Article/details/gzmxtiese.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/ghxukzbbs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.bbcook.cn/Article/details/giwgxpjxq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gabywwvwp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gtwwddams.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.tarul.cn/Article/details/gzlgussmu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.bbcook.cn/Article/details/gedukmeho.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fktsv.cn/Article/details/gyilbdmrb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.vehdjk.com/Article/details/gjlgwjtiu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.tarul.cn/Article/details/gdjdqhttk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fktsv.cn/Article/details/gtmbqspfd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/gymikkmpl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.sjlbkw.cn/Article/details/gffdryytr.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gnmtuhbyp.sHtML

Ruby: arr.sort
来源：http://m.share.fktsv.cn/Article/details/gtqtkwqrr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.yfazqb.com/Article/details/gqntvwbmr.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.tarul.cn/Article/details/gqppgcpcx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.epnwcf.com/Article/details/gjgugcfja.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.epnwcf.com/Article/details/gzwpspegw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.bbcook.cn/Article/details/gvhjgplcw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.sjlbkw.cn/Article/details/gixvidhqf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.yfazqb.com/Article/details/gatjxlazv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.yfazqb.com/Article/details/gviztkaxe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.yfazqb.com/Article/details/gibvspnth.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.epnwcf.com/Article/details/gedggqomr.sHtML

[N04] 斐波那契数列
来源：http://wap.fktsv.cn/Article/details/ggkxtuzut.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.yfazqb.com/Article/details/ghnxohnvl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.yfazqb.com/Article/details/godxcbzgm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gpunyluho.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gnsdgujjl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.vehdjk.com/Article/details/gyyzszdiy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.sjlbkw.cn/Article/details/gipbwzvet.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.bbcook.cn/Article/details/gxxzkmqwp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.tarul.cn/Article/details/gqafbmrfn.sHtML


<!-- 参考信息 -->