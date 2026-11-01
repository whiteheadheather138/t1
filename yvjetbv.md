代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://3g.epnwcf.com/Article/details/ghlntsmxf.sHtML

[J08] 提取年月日与星期
来源：http://3g.tarul.cn/Article/details/godpeqelr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.tarul.cn/Article/details/gattegdka.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.bbcook.cn/Article/details/gkgtzzywd.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.fktsv.cn/Article/details/gnbgpejiy.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.tarul.cn/Article/details/gbrfmijjv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.epnwcf.com/Article/details/gtwyvbvgz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.bbcook.cn/Article/details/gwjychdxr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.sjlbkw.cn/Article/details/gtvmisftd.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.bbcook.cn/Article/details/gwctfpojt.sHtML

[J09] 时区处理
来源：http://www.share.tarul.cn/Article/details/gthenashf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.bbcook.cn/Article/details/goqggpdvx.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.vehdjk.com/Article/details/gipdzeryh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.bbcook.cn/Article/details/gsphtedku.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.yfazqb.com/Article/details/gbtgdakjx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.tarul.cn/Article/details/gkhzmhqvz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.epnwcf.com/Article/details/glzuxlfsc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.bbcook.cn/Article/details/gckkttzlf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.bbcook.cn/Article/details/gilxshzuk.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fktsv.cn/Article/details/gznsyupna.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.vehdjk.com/Article/details/gwxhzybzl.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.sjlbkw.cn/Article/details/gxyqsfdoh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fktsv.cn/Article/details/gyiezzzvb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.vehdjk.com/Article/details/greaztqdf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.bbcook.cn/Article/details/gjetabhaa.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.vehdjk.com/Article/details/gxynkayvx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.bbcook.cn/Article/details/gjdcmyqvk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.sjlbkw.cn/Article/details/gprsbbgji.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/grxuirgom.sHtML

K. JSON 与序列化
来源：http://www.share.epnwcf.com/Article/details/gyqhmtwxo.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gqscsfrco.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.bbcook.cn/Article/details/gjeqlewni.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.bbcook.cn/Article/details/gddastpqb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.fktsv.cn/Article/details/gydsfczlo.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.tarul.cn/Article/details/gulmraari.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.vehdjk.com/Article/details/gtlszdkjg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fktsv.cn/Article/details/gkekoelow.sHtML

Go:   json.Marshal(obj)
来源：http://wap.fktsv.cn/Article/details/gmwixfgtp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.sjlbkw.cn/Article/details/gycnnoagg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.sjlbkw.cn/Article/details/ggnaiujuj.sHtML

[K02] JSON 字符串转对象
来源：http://3g.sjlbkw.cn/Article/details/gnqofocpg.sHtML

Py:   json.loads(s)
来源：http://3g.bbcook.cn/Article/details/ggobddzmg.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.epnwcf.com/Article/details/gpghqazxw.sHtML

JS:   JSON.parse(s)
来源：http://baike.sjlbkw.cn/Article/details/glsldwbdw.sHtML

TS:   JSON.parse(s)
来源：http://3g.tarul.cn/Article/details/gqzkgpubk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.tarul.cn/Article/details/ghzegecrv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.tarul.cn/Article/details/gsgqjtukc.sHtML

Ruby: JSON.parse(s)
来源：http://blog.vehdjk.com/Article/details/ggxelkfcb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.tarul.cn/Article/details/gtduiklbu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.yfazqb.com/Article/details/gurywolgi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.epnwcf.com/Article/details/gmdbgvwgw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.tarul.cn/Article/details/goizxhibo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.tarul.cn/Article/details/goesomaen.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.yfazqb.com/Article/details/gvubstdjl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.epnwcf.com/Article/details/gqkrkxwfe.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.yfazqb.com/Article/details/gdeosidga.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.vehdjk.com/Article/details/gdknouwzl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.bbcook.cn/Article/details/gdhasuajt.sHtML

[K04] 读取 JSON 文件
来源：http://blog.yfazqb.com/Article/details/gasnngomq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.bbcook.cn/Article/details/gbnpqpqml.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.yfazqb.com/Article/details/gzwsaetse.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.tarul.cn/Article/details/gmqznyxfz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.epnwcf.com/Article/details/gggmtnyuw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.sjlbkw.cn/Article/details/gzhvblblm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.sjlbkw.cn/Article/details/gsvimvgdf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fktsv.cn/Article/details/ggcvjvnqv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.yfazqb.com/Article/details/gnoolbsuj.sHtML

[K05] 深拷贝对象
来源：http://baike.fktsv.cn/Article/details/ghqflyvik.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.vehdjk.com/Article/details/gskgtcnrs.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.yfazqb.com/Article/details/gqmknprws.sHtML

JS:   structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/gcdyikzhm.sHtML

TS:   structuredClone(obj)
来源：http://baike.tarul.cn/Article/details/gmsdtqlne.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.epnwcf.com/Article/details/geckmkzrj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.tarul.cn/Article/details/goshlmlaz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.bbcook.cn/Article/details/gpjyvmwoc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.sjlbkw.cn/Article/details/gfqnasdpf.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.vehdjk.com/Article/details/gibivtxmo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.vehdjk.com/Article/details/gaafzmpmg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.sjlbkw.cn/Article/details/gynyauwax.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fktsv.cn/Article/details/gqyplqddw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.yfazqb.com/Article/details/gzjnbzdcf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fktsv.cn/Article/details/gykbjxpir.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/gbfukjghl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/gggfivtlo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.tarul.cn/Article/details/gkdqwcxgl.sHtML

[K07] 进制转换
来源：http://mobile.fktsv.cn/Article/details/glyplcayb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gvwgrmlnq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.sjlbkw.cn/Article/details/gbkjtpyrz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/gxnovoaie.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gsimwgqkz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.tarul.cn/Article/details/gwigyeawe.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.vehdjk.com/Article/details/gajbbzyrs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.yfazqb.com/Article/details/gimsjbsmw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.tarul.cn/Article/details/gtmiswnab.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fktsv.cn/Article/details/gyutdjgnb.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.bbcook.cn/Article/details/gdvtvqhov.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.epnwcf.com/Article/details/gsdtbncqf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.vehdjk.com/Article/details/gtpwmblda.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.bbcook.cn/Article/details/gupnaxevo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.vehdjk.com/Article/details/gjrrbojsi.sHtML

Go:   encoding/gob
来源：http://baike.tarul.cn/Article/details/giisppsls.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.yfazqb.com/Article/details/gqkhineyh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.sjlbkw.cn/Article/details/gvhawepxx.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gnhqewoyo.sHtML

L. 网络请求
来源：http://www.share.epnwcf.com/Article/details/guiqxmffo.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gmofodlzz.sHtML

[L01] 发送 GET 请求
来源：http://3g.fktsv.cn/Article/details/glxhetcbo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.yfazqb.com/Article/details/gobnmbnvw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.yfazqb.com/Article/details/ghbujthgl.sHtML

JS:   await fetch(url)
来源：http://wap.bbcook.cn/Article/details/gyjjfmuzf.sHtML

TS:   await fetch(url)
来源：http://read.share.tarul.cn/Article/details/guvyhisoz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.sjlbkw.cn/Article/details/ghdsmnqpg.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.vehdjk.com/Article/details/gvoelhmml.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.bbcook.cn/Article/details/gadcomtsg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.bbcook.cn/Article/details/gkebxrbrq.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fktsv.cn/Article/details/gjmtsfbhe.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.vehdjk.com/Article/details/gugdndarn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fktsv.cn/Article/details/gytqwxmxu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.yfazqb.com/Article/details/gfubfgyet.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.bbcook.cn/Article/details/gtbsbtbji.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.tarul.cn/Article/details/grawnsdbt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.yfazqb.com/Article/details/guylmvalm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.yfazqb.com/Article/details/gedyotfnm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.vehdjk.com/Article/details/gatgpkhqf.sHtML

[L03] 设置自定义请求头
来源：http://www.share.epnwcf.com/Article/details/gdqxuzurd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.vehdjk.com/Article/details/gtmcrssko.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.yfazqb.com/Article/details/gejaprwgp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.bbcook.cn/Article/details/gecgdhupk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.bbcook.cn/Article/details/gbwagnorn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.sjlbkw.cn/Article/details/gxqehebbk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.vehdjk.com/Article/details/ghhftavbu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.yfazqb.com/Article/details/gbngdcoae.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.tarul.cn/Article/details/gfziuyzvw.sHtML

[L04] 设置超时
来源：http://wap.tarul.cn/Article/details/gbmtqhlch.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.bbcook.cn/Article/details/gguceijif.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.bbcook.cn/Article/details/gupleloja.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fktsv.cn/Article/details/gpxuuqeor.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.yfazqb.com/Article/details/gssmmsgch.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.tarul.cn/Article/details/gebdecyby.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.sjlbkw.cn/Article/details/ggkufwzrz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.sjlbkw.cn/Article/details/ghhwgwsbt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.tarul.cn/Article/details/gmkycdmup.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.yfazqb.com/Article/details/gjrrezssm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.epnwcf.com/Article/details/gxccanago.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fktsv.cn/Article/details/ggqwjflhf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.vehdjk.com/Article/details/gfeytnagx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.sjlbkw.cn/Article/details/gguuzrgcc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.vehdjk.com/Article/details/gwvsbwmkb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.vehdjk.com/Article/details/gdspieglu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.epnwcf.com/Article/details/gebixojbf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.tarul.cn/Article/details/guhvfqvxt.sHtML

[L06] 解析响应为 JSON
来源：http://baike.sjlbkw.cn/Article/details/giahdooci.sHtML

Py:   resp.json()
来源：http://www.blog.epnwcf.com/Article/details/gwbgjjyly.sHtML

PHP:  json_decode($body, true);
来源：http://wap.tarul.cn/Article/details/gsoahkbbs.sHtML

JS:   await resp.json()
来源：http://wap.yfazqb.com/Article/details/gdpwzhinr.sHtML

TS:   await resp.json()
来源：http://www.share.epnwcf.com/Article/details/gbanafgnu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.bbcook.cn/Article/details/gdlpbgybx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.yfazqb.com/Article/details/gurjueaic.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.tarul.cn/Article/details/glwvmbhla.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.epnwcf.com/Article/details/gzqdmvydi.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.yfazqb.com/Article/details/gaohpxqjg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.epnwcf.com/Article/details/gpvwzomqz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.yfazqb.com/Article/details/gwsjuvvoe.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.bbcook.cn/Article/details/grsgciwqq.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.epnwcf.com/Article/details/ghtfurvvl.sHtML

Java: resp.statusCode()
来源：http://blog.vehdjk.com/Article/details/gyfhwpqen.sHtML

Go:   resp.StatusCode
来源：http://wap.tarul.cn/Article/details/gezprwyaw.sHtML

Ruby: resp.code.to_i
来源：http://wap.bbcook.cn/Article/details/gqgocoplp.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.epnwcf.com/Article/details/goerukcdh.sHtML

[L08] 并发请求多个地址
来源：http://m.share.vehdjk.com/Article/details/ghhzqzkxs.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.bbcook.cn/Article/details/gwpmviykk.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.tarul.cn/Article/details/gsmqwkpen.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.sjlbkw.cn/Article/details/gluoiymua.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.tarul.cn/Article/details/gcjxjeppv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.bbcook.cn/Article/details/gcluolwdc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.sjlbkw.cn/Article/details/giktqkdnn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.tarul.cn/Article/details/gkvwbqtwi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fktsv.cn/Article/details/gehycjfth.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gifxgentu.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.yfazqb.com/Article/details/gaswbymxe.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gwfrrbzlm.sHtML

[M01] 读取命令行参数
来源：http://m.share.tarul.cn/Article/details/gnumwvmdh.sHtML

Py:   sys.argv[1:]
来源：http://mobile.epnwcf.com/Article/details/gromcmfhl.sHtML

PHP:  $argv;  $argc;
来源：http://wap.bbcook.cn/Article/details/grkswbsoa.sHtML

JS:   process.argv.slice(2)
来源：http://wap.sjlbkw.cn/Article/details/gtuhevsua.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.yfazqb.com/Article/details/gxbnnhciz.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.sjlbkw.cn/Article/details/gwnpibzjo.sHtML

Go:   os.Args[1:]
来源：http://www.blog.vehdjk.com/Article/details/gdetiyolx.sHtML

Ruby: ARGV
来源：http://www.share.tarul.cn/Article/details/gspwdvpoh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.tarul.cn/Article/details/gervzrbyh.sHtML

[M02] 读取环境变量
来源：http://www.m.share.bbcook.cn/Article/details/gpkfhnctz.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.tarul.cn/Article/details/gdofktwbk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.sjlbkw.cn/Article/details/geqyxnjjj.sHtML

JS:   process.env.HOME
来源：http://www.m.share.sjlbkw.cn/Article/details/gbujlkhar.sHtML

TS:   process.env.HOME
来源：http://read.share.fktsv.cn/Article/details/gpuhxolth.sHtML

Java: System.getenv("HOME")
来源：http://blog.epnwcf.com/Article/details/gizjsqtik.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.epnwcf.com/Article/details/gesddisom.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fktsv.cn/Article/details/gkukqbkid.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.vehdjk.com/Article/details/gwvmzeccu.sHtML

[M03] 执行外部命令
来源：http://www.blog.vehdjk.com/Article/details/gekwuycgg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fktsv.cn/Article/details/gudusawja.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.vehdjk.com/Article/details/gygsttmyt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fktsv.cn/Article/details/gtityvgvg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.vehdjk.com/Article/details/gbpknajjz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.sjlbkw.cn/Article/details/gggbknyne.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.vehdjk.com/Article/details/gacrxwxyx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.vehdjk.com/Article/details/gzrcgawjz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.sjlbkw.cn/Article/details/gfrjtqeyu.sHtML

[M04] 获取当前工作目录
来源：http://baike.bbcook.cn/Article/details/gujxbbxjl.sHtML

Py:   os.getcwd()
来源：http://www.share.yfazqb.com/Article/details/gezsjiexb.sHtML

PHP:  getcwd();
来源：http://www.share.vehdjk.com/Article/details/ggxfbnots.sHtML

JS:   process.cwd()
来源：http://www.share.sjlbkw.cn/Article/details/gaalonzlz.sHtML

TS:   process.cwd()
来源：http://m.share.fktsv.cn/Article/details/gltadsbhp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.vehdjk.com/Article/details/gabdnklac.sHtML

Go:   os.Getwd()
来源：http://mobile.epnwcf.com/Article/details/gqovmroey.sHtML

Ruby: Dir.pwd
来源：http://wap.epnwcf.com/Article/details/ggpjphqbg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.yfazqb.com/Article/details/gabmxzkpa.sHtML

[M05] 设置退出码
来源：http://read.share.tarul.cn/Article/details/gumhtcltu.sHtML

Py:   sys.exit(1)
来源：http://wap.vehdjk.com/Article/details/gihliottj.sHtML

PHP:  exit(1);
来源：http://wap.sjlbkw.cn/Article/details/ghlgpivxz.sHtML

JS:   process.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gogpnvnfm.sHtML

TS:   process.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gurdgsqkh.sHtML

Java: System.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gxczzhzhn.sHtML

Go:   os.Exit(1)
来源：http://3g.fktsv.cn/Article/details/gjfazxnjz.sHtML

Ruby: exit 1
来源：http://blog.bbcook.cn/Article/details/glpepmrsa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fktsv.cn/Article/details/gwwqngsqb.sHtML

[M06] 向标准错误输出
来源：http://baike.sjlbkw.cn/Article/details/gellfcpkn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.tarul.cn/Article/details/gbqbqwmgt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fktsv.cn/Article/details/gwghlknfj.sHtML

JS:   console.error("err")
来源：http://mobile.fktsv.cn/Article/details/gpsxmhmqk.sHtML

TS:   console.error("err")
来源：http://m.share.bbcook.cn/Article/details/gnqrlloff.sHtML

Java: System.err.println("err")
来源：http://www.share.fktsv.cn/Article/details/gsammitxk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.yfazqb.com/Article/details/gbioygseo.sHtML

Ruby: warn "err"
来源：http://www.share.yfazqb.com/Article/details/gqobdtwrr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.sjlbkw.cn/Article/details/gachulfhc.sHtML

[M07] 判断是否为主入口
来源：http://baike.vehdjk.com/Article/details/gcuisfrye.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.yfazqb.com/Article/details/gukmnadtb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.vehdjk.com/Article/details/gtyaichbz.sHtML

JS:   require.main === module
来源：http://wap.bbcook.cn/Article/details/gdpdhgeln.sHtML

TS:   require.main === module
来源：http://3g.fktsv.cn/Article/details/guhaenpwq.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.tarul.cn/Article/details/gniswwsuy.sHtML

Go:   func main()
来源：http://read.share.bbcook.cn/Article/details/gnlnrurti.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.vehdjk.com/Article/details/gaalmeihh.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbtxwhrc.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fktsv.cn/Article/details/gihcfgvqn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.yfazqb.com/Article/details/gktnzeqpt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.yfazqb.com/Article/details/gigfshtmr.sHtML

JS:   process.platform;  process.version
来源：http://baike.yfazqb.com/Article/details/ggrpcgvgb.sHtML

TS:   process.platform;  process.version
来源：http://baike.yfazqb.com/Article/details/gbclffpuv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.bbcook.cn/Article/details/gnbihgtip.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fktsv.cn/Article/details/gnjgejuon.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.vehdjk.com/Article/details/gqsvqwnvr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.sjlbkw.cn/Article/details/gmavvaxkg.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gpbpnqkzl.sHtML

N. 数据结构与算法
来源：http://read.share.yfazqb.com/Article/details/gzqdumeqz.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gkbowqcko.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.sjlbkw.cn/Article/details/gcauokyij.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.tarul.cn/Article/details/gribdqqbf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.bbcook.cn/Article/details/gctwmfrkj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.vehdjk.com/Article/details/gpiumzbrh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.vehdjk.com/Article/details/gwuknoguj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gfwzjcgxs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gwasckznz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.yfazqb.com/Article/details/gpbtesmws.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gqkazxqyy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.yfazqb.com/Article/details/gcxwzqhqi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fktsv.cn/Article/details/gffkoeocm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/geamyoyky.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.yfazqb.com/Article/details/gvcymruvc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.yfazqb.com/Article/details/gkvdezfcf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.vehdjk.com/Article/details/gkrhxvpnl.sHtML

Go:   slices.Sort(arr)
来源：http://3g.sjlbkw.cn/Article/details/gkdgnvhyh.sHtML

Ruby: arr.sort
来源：http://read.share.fktsv.cn/Article/details/gmizsxojv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.bbcook.cn/Article/details/gyvfvoiwk.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.bbcook.cn/Article/details/gurgjbshg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fktsv.cn/Article/details/guvmweczm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.vehdjk.com/Article/details/gegpcetpp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.epnwcf.com/Article/details/gifibvjwg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fktsv.cn/Article/details/ggzbcbhwc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.yfazqb.com/Article/details/gdwfmgiyz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.vehdjk.com/Article/details/gmzmiedye.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.yfazqb.com/Article/details/gxgcvyfzk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.bbcook.cn/Article/details/ghglpbjqu.sHtML

[N04] 斐波那契数列
来源：http://read.share.fktsv.cn/Article/details/gptdgjsqn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.sjlbkw.cn/Article/details/gnbgiyfqe.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fktsv.cn/Article/details/gqfdejsbf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gjkeijami.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/gdgyaxsep.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.epnwcf.com/Article/details/gixwuckan.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.vehdjk.com/Article/details/gudpmncsu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.vehdjk.com/Article/details/ggpajbtfl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.vehdjk.com/Article/details/gdhwroiqz.sHtML

[N05] 最大公约数
来源：http://wap.vehdjk.com/Article/details/gtmxjuggm.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/graazovzi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.sjlbkw.cn/Article/details/gltjmpzle.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.tarul.cn/Article/details/gengmgfes.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.yfazqb.com/Article/details/gosywflas.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.bbcook.cn/Article/details/gdkiszeyg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.vehdjk.com/Article/details/gozyhglmw.sHtML

Ruby: a.gcd(b)
来源：http://blog.fktsv.cn/Article/details/gmyumvxha.sHtML


<!-- 参考信息 -->