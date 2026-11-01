代发 wailian999

[J07] 比较两个日期
来源：http://wap.bbcook.cn/Article/details/grdmssjlb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.sjlbkw.cn/Article/details/gjhqncmxg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.yfazqb.com/Article/details/gcamqqvpb.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.vehdjk.com/Article/details/gwhwqpjdc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.tarul.cn/Article/details/giryrqwhk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.vehdjk.com/Article/details/gbwqlahbf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.sjlbkw.cn/Article/details/gtmjnfuwv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.yfazqb.com/Article/details/gnxqftovi.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/gyspfifhc.sHtML

[J08] 提取年月日与星期
来源：http://baike.sjlbkw.cn/Article/details/gcbecfpvp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.epnwcf.com/Article/details/gjvpqgvjk.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.sjlbkw.cn/Article/details/gbtyikmxs.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.sjlbkw.cn/Article/details/glkthetml.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.sjlbkw.cn/Article/details/gkbtzveqb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.yfazqb.com/Article/details/gmfysnqup.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.tarul.cn/Article/details/gtkcbsgua.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.sjlbkw.cn/Article/details/gkexenimg.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.epnwcf.com/Article/details/gfydkbdjs.sHtML

[J09] 时区处理
来源：http://wap.bbcook.cn/Article/details/gfsjvflvk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.vehdjk.com/Article/details/gotdoyrdq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.yfazqb.com/Article/details/gvnosmtbn.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.yfazqb.com/Article/details/gfsxafvca.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.sjlbkw.cn/Article/details/ggreajeub.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.vehdjk.com/Article/details/grmeadmua.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.bbcook.cn/Article/details/gdyizvflr.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.yfazqb.com/Article/details/ghdqtfsfa.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.epnwcf.com/Article/details/ghkiuhbav.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.tarul.cn/Article/details/gtarfrokk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fktsv.cn/Article/details/gnsvntmnt.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.fktsv.cn/Article/details/gxnovowhd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.sjlbkw.cn/Article/details/glywlmsny.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fktsv.cn/Article/details/ghtwkdbsa.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.tarul.cn/Article/details/guagnylxx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fktsv.cn/Article/details/gqdrxexyl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.sjlbkw.cn/Article/details/glfjqqxkx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fktsv.cn/Article/details/gjwhsvnrv.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/grzqzbzsa.sHtML

K. JSON 与序列化
来源：http://blog.bbcook.cn/Article/details/gbhjoxwwx.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gdaqkjnmu.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/grlwgbusv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.sjlbkw.cn/Article/details/gsbdefhxg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.bbcook.cn/Article/details/gmeepamlh.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gwgwqocze.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fktsv.cn/Article/details/gyzimrftx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.bbcook.cn/Article/details/gooswcfdl.sHtML

Go:   json.Marshal(obj)
来源：http://wap.bbcook.cn/Article/details/gecdkhxwi.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.vehdjk.com/Article/details/gtgnewjxg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.yfazqb.com/Article/details/gnvrjvzjb.sHtML

[K02] JSON 字符串转对象
来源：http://wap.epnwcf.com/Article/details/gxgehnixz.sHtML

Py:   json.loads(s)
来源：http://3g.sjlbkw.cn/Article/details/gkyfsslgb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.yfazqb.com/Article/details/ghchiqvli.sHtML

JS:   JSON.parse(s)
来源：http://mobile.bbcook.cn/Article/details/gqglfvtve.sHtML

TS:   JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gwezexlpq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.bbcook.cn/Article/details/gekkguvya.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.sjlbkw.cn/Article/details/gquwzooia.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/ghiwlxopy.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fktsv.cn/Article/details/gyzzoqkvl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.yfazqb.com/Article/details/gdfulkhof.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.epnwcf.com/Article/details/gsltixpxn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fktsv.cn/Article/details/gjilvsfvb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.vehdjk.com/Article/details/gekqxatze.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.yfazqb.com/Article/details/gydqbhzky.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.bbcook.cn/Article/details/gbpebwvox.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.tarul.cn/Article/details/gslmswtfh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.sjlbkw.cn/Article/details/gbjocuifm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.vehdjk.com/Article/details/glazytxvl.sHtML

[K04] 读取 JSON 文件
来源：http://blog.vehdjk.com/Article/details/gujuuwlwx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.bbcook.cn/Article/details/gmclfejkz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.vehdjk.com/Article/details/gxfxuqpxt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/gxuwwnmcs.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.yfazqb.com/Article/details/gcaovkajc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fktsv.cn/Article/details/gqshbokss.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.bbcook.cn/Article/details/gnvzhatla.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.yfazqb.com/Article/details/gkhjsendx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fktsv.cn/Article/details/gwqktzbcs.sHtML

[K05] 深拷贝对象
来源：http://wap.epnwcf.com/Article/details/gjlfyxxww.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.vehdjk.com/Article/details/gfqdsywhi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fktsv.cn/Article/details/gulyzmwsl.sHtML

JS:   structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/gwspexytw.sHtML

TS:   structuredClone(obj)
来源：http://blog.fktsv.cn/Article/details/gvntfctso.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.vehdjk.com/Article/details/gfbhtebwt.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.vehdjk.com/Article/details/gkimftxln.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.vehdjk.com/Article/details/govijscai.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.sjlbkw.cn/Article/details/gsvczgccj.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.vehdjk.com/Article/details/ghswdmphv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.vehdjk.com/Article/details/grhtfvavz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.bbcook.cn/Article/details/gxbhsbexj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.epnwcf.com/Article/details/gdwetqofm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.epnwcf.com/Article/details/guydxwhau.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.tarul.cn/Article/details/gbtjkvzqd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/gpbnphryp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/gcyobuxod.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/gmvalysbc.sHtML

[K07] 进制转换
来源：http://www.share.tarul.cn/Article/details/geajpwzot.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkzbasyz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.epnwcf.com/Article/details/gociqqjmf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gpgvdbugm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gwgmvnzme.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gkcvyvgwx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fktsv.cn/Article/details/gugbwjljc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.tarul.cn/Article/details/gfbugionc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gpidhwmbi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.yfazqb.com/Article/details/gexuwyydi.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.sjlbkw.cn/Article/details/gzfkwufds.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.bbcook.cn/Article/details/govdrrwdo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.epnwcf.com/Article/details/gdccvjyhi.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.vehdjk.com/Article/details/grycevyno.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.bbcook.cn/Article/details/gqkpfoxet.sHtML

Go:   encoding/gob
来源：http://3g.bbcook.cn/Article/details/grsjsdzeq.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.yfazqb.com/Article/details/gqkggthbb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.vehdjk.com/Article/details/glcyollax.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gbujqfahf.sHtML

L. 网络请求
来源：http://read.share.tarul.cn/Article/details/gvjxbqgtx.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gsotijbqv.sHtML

[L01] 发送 GET 请求
来源：http://baike.fktsv.cn/Article/details/gyekmyybl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.yfazqb.com/Article/details/gugubelqh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.epnwcf.com/Article/details/gbmidrycu.sHtML

JS:   await fetch(url)
来源：http://3g.sjlbkw.cn/Article/details/ghkavkkcg.sHtML

TS:   await fetch(url)
来源：http://mobile.sjlbkw.cn/Article/details/gvzrsxiqs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.vehdjk.com/Article/details/gjpubzxvq.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.vehdjk.com/Article/details/gzdjtizyx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.tarul.cn/Article/details/gbclndzyj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.sjlbkw.cn/Article/details/geteaolqb.sHtML

[L02] 发送 POST JSON
来源：http://blog.yfazqb.com/Article/details/gdkdmuttm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.sjlbkw.cn/Article/details/gnskgntvf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.yfazqb.com/Article/details/gsqwfpxqv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.vehdjk.com/Article/details/gogomcomc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.bbcook.cn/Article/details/gkhurhole.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.vehdjk.com/Article/details/gltcsbvfq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.sjlbkw.cn/Article/details/gulebtwth.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.yfazqb.com/Article/details/gcnazylgl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.epnwcf.com/Article/details/gevchnemy.sHtML

[L03] 设置自定义请求头
来源：http://m.share.epnwcf.com/Article/details/gcsgzdygo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.sjlbkw.cn/Article/details/gquikiyzz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.sjlbkw.cn/Article/details/gfwzkmghn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.yfazqb.com/Article/details/gsitiefxm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.vehdjk.com/Article/details/glztknoef.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.yfazqb.com/Article/details/ghismawts.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.sjlbkw.cn/Article/details/gkdgnmwby.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.yfazqb.com/Article/details/gpxblvtur.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fktsv.cn/Article/details/glohotyej.sHtML

[L04] 设置超时
来源：http://www.m.share.yfazqb.com/Article/details/gdjmsohsz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.yfazqb.com/Article/details/grklrejvn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.bbcook.cn/Article/details/ggvwvczkn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.epnwcf.com/Article/details/gfurvdjvl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.epnwcf.com/Article/details/ghqvrlipk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.sjlbkw.cn/Article/details/goodrohah.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fktsv.cn/Article/details/gjrttieou.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fktsv.cn/Article/details/gtqlkvpra.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.epnwcf.com/Article/details/gonemkemh.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.yfazqb.com/Article/details/glwikzual.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.sjlbkw.cn/Article/details/gzzvsmuuq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.vehdjk.com/Article/details/gwygrpgso.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.bbcook.cn/Article/details/giubocyet.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.epnwcf.com/Article/details/gfuebsgqo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.bbcook.cn/Article/details/gayftnvpj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.yfazqb.com/Article/details/gkhmdymxg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.yfazqb.com/Article/details/gllxufsaf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/ghzwoewey.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.epnwcf.com/Article/details/gnvicqpkb.sHtML

Py:   resp.json()
来源：http://mobile.vehdjk.com/Article/details/gbawqxdjm.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.tarul.cn/Article/details/glgfbwofe.sHtML

JS:   await resp.json()
来源：http://m.share.yfazqb.com/Article/details/gvcyokjga.sHtML

TS:   await resp.json()
来源：http://www.blog.sjlbkw.cn/Article/details/gfycjfepb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.sjlbkw.cn/Article/details/gknikgzxx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.bbcook.cn/Article/details/ggjchgdjc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.epnwcf.com/Article/details/gbnlpetso.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.sjlbkw.cn/Article/details/gcprygtlx.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.sjlbkw.cn/Article/details/gyzdoscve.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.tarul.cn/Article/details/gjrlnfrgn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.vehdjk.com/Article/details/gjaswmxeh.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.epnwcf.com/Article/details/gjuyjofkb.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.tarul.cn/Article/details/gwediksho.sHtML

Java: resp.statusCode()
来源：http://read.share.yfazqb.com/Article/details/gnromzlhv.sHtML

Go:   resp.StatusCode
来源：http://3g.fktsv.cn/Article/details/gkkqvyhpg.sHtML

Ruby: resp.code.to_i
来源：http://read.share.yfazqb.com/Article/details/gnedcewpz.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.bbcook.cn/Article/details/gwidpjrfg.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.epnwcf.com/Article/details/gsmouajzb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.vehdjk.com/Article/details/gxizqkqly.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.vehdjk.com/Article/details/gxstuamhp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.epnwcf.com/Article/details/gqnsjlaac.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.yfazqb.com/Article/details/gerkmziks.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fktsv.cn/Article/details/gleyxcsin.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.tarul.cn/Article/details/gxzrvvwbz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.sjlbkw.cn/Article/details/ghtsmwnox.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fktsv.cn/Article/details/gxstyepkb.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gtpvbddjm.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.yfazqb.com/Article/details/gzsoajkcj.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gchilwioo.sHtML

[M01] 读取命令行参数
来源：http://read.share.sjlbkw.cn/Article/details/gajqpvcxh.sHtML

Py:   sys.argv[1:]
来源：http://blog.bbcook.cn/Article/details/giknnvnpo.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.bbcook.cn/Article/details/gcefbvfnc.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.vehdjk.com/Article/details/gehkhrpie.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.tarul.cn/Article/details/gxovamaky.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.vehdjk.com/Article/details/gjihsejlw.sHtML

Go:   os.Args[1:]
来源：http://read.share.sjlbkw.cn/Article/details/ggxnywpam.sHtML

Ruby: ARGV
来源：http://m.share.yfazqb.com/Article/details/grkkwmqby.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fktsv.cn/Article/details/gziayriyf.sHtML

[M02] 读取环境变量
来源：http://m.share.bbcook.cn/Article/details/gsoqcxkvq.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.epnwcf.com/Article/details/gnwlrsvbc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.tarul.cn/Article/details/gpkwypegt.sHtML

JS:   process.env.HOME
来源：http://www.blog.fktsv.cn/Article/details/gibnqlpza.sHtML

TS:   process.env.HOME
来源：http://www.blog.epnwcf.com/Article/details/gczynatnt.sHtML

Java: System.getenv("HOME")
来源：http://m.share.vehdjk.com/Article/details/goggmhlve.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.epnwcf.com/Article/details/gcjdikxky.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fktsv.cn/Article/details/gwitopdys.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gilhbolik.sHtML

[M03] 执行外部命令
来源：http://3g.vehdjk.com/Article/details/gvuzzbvku.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.bbcook.cn/Article/details/gsqwtjrai.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fktsv.cn/Article/details/gpkjtxqdu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.yfazqb.com/Article/details/gadbghpwv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.bbcook.cn/Article/details/guyldydkd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.tarul.cn/Article/details/gvrqnvkdv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.vehdjk.com/Article/details/gketkqknl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.bbcook.cn/Article/details/gzqdbtukt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.bbcook.cn/Article/details/goyaingsb.sHtML

[M04] 获取当前工作目录
来源：http://baike.bbcook.cn/Article/details/gfvnqztmf.sHtML

Py:   os.getcwd()
来源：http://read.share.epnwcf.com/Article/details/gaoqskgsa.sHtML

PHP:  getcwd();
来源：http://baike.yfazqb.com/Article/details/gtlzthucg.sHtML

JS:   process.cwd()
来源：http://blog.bbcook.cn/Article/details/gehuucgnx.sHtML

TS:   process.cwd()
来源：http://www.m.share.yfazqb.com/Article/details/ghvwmifxc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.yfazqb.com/Article/details/gahaiqtnd.sHtML

Go:   os.Getwd()
来源：http://mobile.fktsv.cn/Article/details/gorwyntsf.sHtML

Ruby: Dir.pwd
来源：http://baike.bbcook.cn/Article/details/gxhfgjgtg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.epnwcf.com/Article/details/gqifxbvyr.sHtML

[M05] 设置退出码
来源：http://www.blog.epnwcf.com/Article/details/gqosctcqe.sHtML

Py:   sys.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gptlhgdji.sHtML

PHP:  exit(1);
来源：http://www.blog.epnwcf.com/Article/details/gioslgbea.sHtML

JS:   process.exit(1)
来源：http://mobile.vehdjk.com/Article/details/goakaqflb.sHtML

TS:   process.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gjnwvkgnl.sHtML

Java: System.exit(1)
来源：http://baike.epnwcf.com/Article/details/gaamwhfvm.sHtML

Go:   os.Exit(1)
来源：http://www.share.epnwcf.com/Article/details/gpmnvdbrl.sHtML

Ruby: exit 1
来源：http://www.m.share.yfazqb.com/Article/details/gahbossnz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.sjlbkw.cn/Article/details/gtzzpvbop.sHtML

[M06] 向标准错误输出
来源：http://3g.epnwcf.com/Article/details/gucytidml.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.yfazqb.com/Article/details/gqjzcnshw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.epnwcf.com/Article/details/gjgzhgzvd.sHtML

JS:   console.error("err")
来源：http://3g.vehdjk.com/Article/details/guudhgcgu.sHtML

TS:   console.error("err")
来源：http://m.share.sjlbkw.cn/Article/details/ggexrzoux.sHtML

Java: System.err.println("err")
来源：http://m.share.bbcook.cn/Article/details/gqyrjqvrx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.tarul.cn/Article/details/gtyzxdbis.sHtML

Ruby: warn "err"
来源：http://wap.bbcook.cn/Article/details/gpuolieoz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.tarul.cn/Article/details/gkalwvrfx.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fktsv.cn/Article/details/gjkoomqrg.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fktsv.cn/Article/details/grpjyeaoa.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.bbcook.cn/Article/details/gbloljcll.sHtML

JS:   require.main === module
来源：http://3g.tarul.cn/Article/details/gdlmyesft.sHtML

TS:   require.main === module
来源：http://www.m.share.epnwcf.com/Article/details/ggtedxspl.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.yfazqb.com/Article/details/gdaqxrbhz.sHtML

Go:   func main()
来源：http://read.share.vehdjk.com/Article/details/gjpegfpyc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.epnwcf.com/Article/details/gjhavygbp.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.vehdjk.com/Article/details/gmpzecprn.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.vehdjk.com/Article/details/gwlmgvnlp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.tarul.cn/Article/details/glcquxlkb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.bbcook.cn/Article/details/gjfvfawhk.sHtML

JS:   process.platform;  process.version
来源：http://www.share.epnwcf.com/Article/details/gtakoutdl.sHtML

TS:   process.platform;  process.version
来源：http://wap.epnwcf.com/Article/details/gnubwjvcm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.epnwcf.com/Article/details/gbctefefm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fktsv.cn/Article/details/gtzgvzxng.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.bbcook.cn/Article/details/gjbaympgl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.tarul.cn/Article/details/gofbjbqzv.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gjnogvbpk.sHtML

N. 数据结构与算法
来源：http://blog.fktsv.cn/Article/details/gvrbdtzmv.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/godbfgrjg.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fktsv.cn/Article/details/ghdahlsal.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.vehdjk.com/Article/details/gsfzvlpku.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.tarul.cn/Article/details/gucclzrfb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.vehdjk.com/Article/details/gfyhzzduh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fktsv.cn/Article/details/gmkmmgsbf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gutjhclib.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gaehgxnpy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.vehdjk.com/Article/details/gffcwgsto.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gerbqglgg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.sjlbkw.cn/Article/details/guiofkyeb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.vehdjk.com/Article/details/ggfmpticf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.bbcook.cn/Article/details/gnvnlsjlx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/ggcptnnzb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.tarul.cn/Article/details/gmallgkuq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.bbcook.cn/Article/details/gmjgidyzp.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.vehdjk.com/Article/details/gntwvsyls.sHtML

Ruby: arr.sort
来源：http://wap.epnwcf.com/Article/details/gronqgykb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.tarul.cn/Article/details/gemwxofpb.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.tarul.cn/Article/details/gsbobpndp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.tarul.cn/Article/details/gvrzaglbt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.yfazqb.com/Article/details/ggkawxwrs.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.yfazqb.com/Article/details/gyxrbqfsu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.yfazqb.com/Article/details/gkmhnvdzz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.vehdjk.com/Article/details/gtntiuvpp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.epnwcf.com/Article/details/gtjkxrioc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.vehdjk.com/Article/details/gikwenztc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.yfazqb.com/Article/details/gatqttqtj.sHtML

[N04] 斐波那契数列
来源：http://read.share.epnwcf.com/Article/details/gqdeblyaa.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.vehdjk.com/Article/details/gmazksugi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.sjlbkw.cn/Article/details/gnlepizpj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.bbcook.cn/Article/details/gkltkceov.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gkynpxzau.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.yfazqb.com/Article/details/gjirvpjnr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.sjlbkw.cn/Article/details/giuovokre.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.vehdjk.com/Article/details/gvjshvklg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/giqcnngme.sHtML


<!-- 参考信息 -->