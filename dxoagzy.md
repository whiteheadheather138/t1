代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/gawparkra.sHtML

[J08] 提取年月日与星期
来源：http://baike.epnwcf.com/Article/details/gcccntofa.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.sjlbkw.cn/Article/details/gakbwqdza.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.tarul.cn/Article/details/gjnakxqac.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.vehdjk.com/Article/details/glewvspeu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.tarul.cn/Article/details/gnfputurx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.sjlbkw.cn/Article/details/gkesdrntu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.vehdjk.com/Article/details/gstimjqqo.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.sjlbkw.cn/Article/details/gtyulqejt.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.sjlbkw.cn/Article/details/gjsypywbr.sHtML

[J09] 时区处理
来源：http://read.share.sjlbkw.cn/Article/details/guzxlytwq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.vehdjk.com/Article/details/gjuiehuuy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.epnwcf.com/Article/details/gcdpybjuh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.yfazqb.com/Article/details/gyhdvlbiv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.yfazqb.com/Article/details/gmfpxitpf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.vehdjk.com/Article/details/gjqkwirbq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.yfazqb.com/Article/details/gglmivrui.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.fktsv.cn/Article/details/gafpfmsyn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.yfazqb.com/Article/details/gtqohiajt.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.fktsv.cn/Article/details/gkaobycqw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fktsv.cn/Article/details/grszlyxnp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.bbcook.cn/Article/details/gqtfvyofv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.vehdjk.com/Article/details/gubxpjthc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gqvmffudp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.tarul.cn/Article/details/gtgfaksff.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.epnwcf.com/Article/details/guavuwbag.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.epnwcf.com/Article/details/gufowjjnx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.bbcook.cn/Article/details/gvkfxzngy.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gwnzxdkqw.sHtML

K. JSON 与序列化
来源：http://blog.tarul.cn/Article/details/gcvjjdlfv.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gcbcpddga.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.tarul.cn/Article/details/gpwppymad.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.epnwcf.com/Article/details/gibnqpsqt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.yfazqb.com/Article/details/gflulwkcf.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.vehdjk.com/Article/details/gafoxqhnv.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fktsv.cn/Article/details/gvfyejmod.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.sjlbkw.cn/Article/details/grgphplwm.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.tarul.cn/Article/details/gtesopziz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.yfazqb.com/Article/details/galxotimo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fktsv.cn/Article/details/gxuqgdvrj.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.epnwcf.com/Article/details/gfxicbnci.sHtML

Py:   json.loads(s)
来源：http://blog.yfazqb.com/Article/details/gojqyylig.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.epnwcf.com/Article/details/ginjtejks.sHtML

JS:   JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/gchmfhpsy.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.epnwcf.com/Article/details/glvucgvea.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fktsv.cn/Article/details/gevqakbwh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.tarul.cn/Article/details/gvbefvtsd.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.epnwcf.com/Article/details/gizfpgrov.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.vehdjk.com/Article/details/gohfknklj.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.sjlbkw.cn/Article/details/ggsbfgswj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.fktsv.cn/Article/details/gsduttsac.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.sjlbkw.cn/Article/details/gapnknxcg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.vehdjk.com/Article/details/ghxetvwit.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.bbcook.cn/Article/details/gaeqpdhmq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.tarul.cn/Article/details/gicthlhax.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.epnwcf.com/Article/details/gsfhyycrx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.bbcook.cn/Article/details/gneupcaus.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.sjlbkw.cn/Article/details/gyzuzoesj.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzacrsja.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.epnwcf.com/Article/details/gsttwjffs.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.bbcook.cn/Article/details/gchjcwyak.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.bbcook.cn/Article/details/gikfvlkmo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fktsv.cn/Article/details/ggrztbtyu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.yfazqb.com/Article/details/gkhjjwwti.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.bbcook.cn/Article/details/ggtkliwoz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.yfazqb.com/Article/details/gvbakhzfg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.vehdjk.com/Article/details/gnpacjqrk.sHtML

[K05] 深拷贝对象
来源：http://wap.fktsv.cn/Article/details/gmdgxybyu.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fktsv.cn/Article/details/gtdqxdzkv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.yfazqb.com/Article/details/gmyzofqcw.sHtML

JS:   structuredClone(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gggragtfz.sHtML

TS:   structuredClone(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gioyvaagm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.tarul.cn/Article/details/grktrpfpw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fktsv.cn/Article/details/gufhfhmjc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.tarul.cn/Article/details/gruherthx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.bbcook.cn/Article/details/gdsssagip.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.epnwcf.com/Article/details/gznnweeqy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.bbcook.cn/Article/details/gxcsrwqyo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.bbcook.cn/Article/details/gavaklgzj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.yfazqb.com/Article/details/gxczfpson.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fktsv.cn/Article/details/gyspxazet.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.tarul.cn/Article/details/gfjjwqxsn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.yfazqb.com/Article/details/gpnvaqybp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gtuoranyv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.vehdjk.com/Article/details/gengausxn.sHtML

[K07] 进制转换
来源：http://www.share.epnwcf.com/Article/details/ghreyiiqo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gvwqowrqr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fktsv.cn/Article/details/gdshqobeq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.tarul.cn/Article/details/gflilabun.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gptxrbsie.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gzpiypamw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.sjlbkw.cn/Article/details/gnefxeyis.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fktsv.cn/Article/details/gzpmckvrx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/ghsmrqcdz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.yfazqb.com/Article/details/gdlgswqks.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fktsv.cn/Article/details/gtpfamblm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.sjlbkw.cn/Article/details/gmdrrtous.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.vehdjk.com/Article/details/ghfyvwdrs.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.epnwcf.com/Article/details/gudmlmpzz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.yfazqb.com/Article/details/ghjaqwcoz.sHtML

Go:   encoding/gob
来源：http://m.share.bbcook.cn/Article/details/gvxsqxgtc.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fktsv.cn/Article/details/gdlofvvur.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.tarul.cn/Article/details/gzymunoeu.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gnmciwckw.sHtML

L. 网络请求
来源：http://blog.vehdjk.com/Article/details/geojoxjfo.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gzylndfzd.sHtML

[L01] 发送 GET 请求
来源：http://blog.sjlbkw.cn/Article/details/gphaujsca.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.bbcook.cn/Article/details/gyyhfjqey.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.yfazqb.com/Article/details/gnnvscwmf.sHtML

JS:   await fetch(url)
来源：http://mobile.yfazqb.com/Article/details/gjijkcmls.sHtML

TS:   await fetch(url)
来源：http://3g.sjlbkw.cn/Article/details/gxnkiryrs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.tarul.cn/Article/details/gqrheerwc.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.bbcook.cn/Article/details/gjmyapayf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.epnwcf.com/Article/details/gnziuhzww.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.yfazqb.com/Article/details/gnaeqyneb.sHtML

[L02] 发送 POST JSON
来源：http://read.share.vehdjk.com/Article/details/geppgmotx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.yfazqb.com/Article/details/gnotbrlqr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.sjlbkw.cn/Article/details/gcdyvetqc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.yfazqb.com/Article/details/gfxjejfud.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.bbcook.cn/Article/details/gakfbegdm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.bbcook.cn/Article/details/gojuadgyc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.tarul.cn/Article/details/gtwdmsbke.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.sjlbkw.cn/Article/details/gykacbsru.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.epnwcf.com/Article/details/guetbybzs.sHtML

[L03] 设置自定义请求头
来源：http://www.share.vehdjk.com/Article/details/gtgkjzkfg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.tarul.cn/Article/details/gmaatvfge.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.yfazqb.com/Article/details/ggujompil.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fktsv.cn/Article/details/gdqsmusoy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfbrymha.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.epnwcf.com/Article/details/gfvzpdepr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.bbcook.cn/Article/details/gvmvbzmsl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.yfazqb.com/Article/details/geyfpxood.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.yfazqb.com/Article/details/gxzpaiptd.sHtML

[L04] 设置超时
来源：http://www.blog.tarul.cn/Article/details/grynxdhco.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fktsv.cn/Article/details/gmjvbemue.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fktsv.cn/Article/details/gwnscudwz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.yfazqb.com/Article/details/gimwigqmb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.bbcook.cn/Article/details/gjcuoiufs.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fktsv.cn/Article/details/gvffsujng.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fktsv.cn/Article/details/gtmtywnkh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.epnwcf.com/Article/details/gkocbsvdw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.yfazqb.com/Article/details/grwzosjht.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.sjlbkw.cn/Article/details/gosgdlxsf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.vehdjk.com/Article/details/grbkmgrrt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.vehdjk.com/Article/details/gnfptvahf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fktsv.cn/Article/details/gtotythxm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.vehdjk.com/Article/details/gzqabpesv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.vehdjk.com/Article/details/gipzfkwly.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fktsv.cn/Article/details/ghsuseaff.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.sjlbkw.cn/Article/details/gtxkpwksk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gxgoxpfnc.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.epnwcf.com/Article/details/gfxjugprq.sHtML

Py:   resp.json()
来源：http://3g.tarul.cn/Article/details/grvfbxvoc.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.tarul.cn/Article/details/gavlcffzr.sHtML

JS:   await resp.json()
来源：http://read.share.bbcook.cn/Article/details/gxlqbfluv.sHtML

TS:   await resp.json()
来源：http://mobile.fktsv.cn/Article/details/gqohqzbmy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.tarul.cn/Article/details/gjahfksha.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.bbcook.cn/Article/details/gcbtdawqh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.epnwcf.com/Article/details/gqbhpquad.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.bbcook.cn/Article/details/gjslvyznx.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/gxoiyxakt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.bbcook.cn/Article/details/gwuovgvys.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.sjlbkw.cn/Article/details/ghcivoyhf.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.epnwcf.com/Article/details/gpqhcdhzy.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.sjlbkw.cn/Article/details/gayumpmgk.sHtML

Java: resp.statusCode()
来源：http://wap.bbcook.cn/Article/details/gaktelwvc.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.yfazqb.com/Article/details/gukjyitct.sHtML

Ruby: resp.code.to_i
来源：http://mobile.bbcook.cn/Article/details/gubpgjinj.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.yfazqb.com/Article/details/gsqqtpvcq.sHtML

[L08] 并发请求多个地址
来源：http://www.share.epnwcf.com/Article/details/gmtgufzga.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtwjbdrs.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.yfazqb.com/Article/details/gmekjdgtw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.vehdjk.com/Article/details/gpdzvntkn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.epnwcf.com/Article/details/goybdbygr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.yfazqb.com/Article/details/gajqiqwkp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.vehdjk.com/Article/details/gkfhkuqaa.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.yfazqb.com/Article/details/gtrpqjsru.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.epnwcf.com/Article/details/gkdbscipx.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gonwrmdlh.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.vehdjk.com/Article/details/gbwjrintx.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gjyvcnlbd.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.yfazqb.com/Article/details/ggkrpwoif.sHtML

Py:   sys.argv[1:]
来源：http://baike.bbcook.cn/Article/details/gckhuvxpb.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.bbcook.cn/Article/details/gobpykahr.sHtML

JS:   process.argv.slice(2)
来源：http://baike.vehdjk.com/Article/details/gnisuczxq.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.vehdjk.com/Article/details/gwfcpjswc.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.yfazqb.com/Article/details/gttmjtrpi.sHtML

Go:   os.Args[1:]
来源：http://m.share.epnwcf.com/Article/details/gmzjmzghz.sHtML

Ruby: ARGV
来源：http://www.share.sjlbkw.cn/Article/details/gfmyywchz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.bbcook.cn/Article/details/gvfnnmwfm.sHtML

[M02] 读取环境变量
来源：http://www.share.sjlbkw.cn/Article/details/gklrjaztm.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gpbksmebv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.sjlbkw.cn/Article/details/gjyradodw.sHtML

JS:   process.env.HOME
来源：http://wap.vehdjk.com/Article/details/gbdhvobrf.sHtML

TS:   process.env.HOME
来源：http://mobile.tarul.cn/Article/details/gjibckzwk.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.tarul.cn/Article/details/golycmofu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.yfazqb.com/Article/details/gqubzamak.sHtML

Ruby: ENV["HOME"]
来源：http://baike.tarul.cn/Article/details/gozfxjebk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.vehdjk.com/Article/details/gtjvqsmmg.sHtML

[M03] 执行外部命令
来源：http://blog.fktsv.cn/Article/details/gijnbusny.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.vehdjk.com/Article/details/gwabiyxya.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.epnwcf.com/Article/details/gggeyzfui.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.epnwcf.com/Article/details/gafoxikdd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.bbcook.cn/Article/details/ghlskogtm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.vehdjk.com/Article/details/gfjtbxzcz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.tarul.cn/Article/details/gkwybzisd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.vehdjk.com/Article/details/geiameiut.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.vehdjk.com/Article/details/gdledumez.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fktsv.cn/Article/details/gtfnprppd.sHtML

Py:   os.getcwd()
来源：http://www.share.yfazqb.com/Article/details/gtudzvsfx.sHtML

PHP:  getcwd();
来源：http://m.share.sjlbkw.cn/Article/details/gxywjnymg.sHtML

JS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/gotxyzvrm.sHtML

TS:   process.cwd()
来源：http://wap.yfazqb.com/Article/details/gklmdonfh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.tarul.cn/Article/details/gpjfpskgo.sHtML

Go:   os.Getwd()
来源：http://3g.fktsv.cn/Article/details/goxppuqgh.sHtML

Ruby: Dir.pwd
来源：http://mobile.bbcook.cn/Article/details/gbpfaalik.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fktsv.cn/Article/details/grufmgrne.sHtML

[M05] 设置退出码
来源：http://www.share.epnwcf.com/Article/details/glygczrtw.sHtML

Py:   sys.exit(1)
来源：http://m.share.yfazqb.com/Article/details/gejefgfiu.sHtML

PHP:  exit(1);
来源：http://mobile.fktsv.cn/Article/details/gekhgxigj.sHtML

JS:   process.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gomsnaogk.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gghkfbfqt.sHtML

Java: System.exit(1)
来源：http://m.share.tarul.cn/Article/details/gqcjqljrh.sHtML

Go:   os.Exit(1)
来源：http://wap.vehdjk.com/Article/details/gnhdkeqyk.sHtML

Ruby: exit 1
来源：http://m.share.epnwcf.com/Article/details/geksnptaa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.sjlbkw.cn/Article/details/ghhnmwezg.sHtML

[M06] 向标准错误输出
来源：http://www.share.epnwcf.com/Article/details/gqvcqftgt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.yfazqb.com/Article/details/gxnuyouyy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.bbcook.cn/Article/details/gtbnrypdb.sHtML

JS:   console.error("err")
来源：http://blog.yfazqb.com/Article/details/gzdfyiolm.sHtML

TS:   console.error("err")
来源：http://read.share.fktsv.cn/Article/details/gsctgscye.sHtML

Java: System.err.println("err")
来源：http://blog.vehdjk.com/Article/details/gkxdgnmjw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.vehdjk.com/Article/details/gzlhykrwd.sHtML

Ruby: warn "err"
来源：http://www.m.share.yfazqb.com/Article/details/gqgcdsqiv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.epnwcf.com/Article/details/gxeayqaap.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.tarul.cn/Article/details/gtzpmoujy.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.sjlbkw.cn/Article/details/gjiftdegh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.tarul.cn/Article/details/gnhybtmsl.sHtML

JS:   require.main === module
来源：http://baike.bbcook.cn/Article/details/grqxlekov.sHtML

TS:   require.main === module
来源：http://blog.vehdjk.com/Article/details/gdxmrivgq.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.vehdjk.com/Article/details/gtvkjoidk.sHtML

Go:   func main()
来源：http://mobile.tarul.cn/Article/details/gclwkbwfn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fktsv.cn/Article/details/ghwwdqqtu.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fktsv.cn/Article/details/gijjzghsc.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.vehdjk.com/Article/details/grbtdbnxk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.yfazqb.com/Article/details/gvsyyfjrn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.epnwcf.com/Article/details/gsygbvdhh.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtgontwr.sHtML

TS:   process.platform;  process.version
来源：http://baike.tarul.cn/Article/details/gadfhtsea.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.bbcook.cn/Article/details/gyvidofqx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.yfazqb.com/Article/details/gnjshpdhv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.sjlbkw.cn/Article/details/gffsfgavt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.sjlbkw.cn/Article/details/gqpdagtmw.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gqdmawwqf.sHtML

N. 数据结构与算法
来源：http://www.share.fktsv.cn/Article/details/gxpxltcbu.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/grjmnckhe.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.epnwcf.com/Article/details/gbhchyjmt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gwsxjmgkw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.yfazqb.com/Article/details/gybidhxiy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.yfazqb.com/Article/details/ggioepmgi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.tarul.cn/Article/details/gbbeybfgv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gmywclsie.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.bbcook.cn/Article/details/grhplvoak.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.sjlbkw.cn/Article/details/ghnxovkrm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gnrjbldzj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fktsv.cn/Article/details/gdxfwnkul.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.bbcook.cn/Article/details/goomckiez.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fktsv.cn/Article/details/gutkmsiiv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fktsv.cn/Article/details/gsfpidyew.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.bbcook.cn/Article/details/guxjbqpoi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.bbcook.cn/Article/details/gddfzlden.sHtML

Go:   slices.Sort(arr)
来源：http://baike.yfazqb.com/Article/details/ggidqvobp.sHtML

Ruby: arr.sort
来源：http://wap.tarul.cn/Article/details/gupqczubd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.yfazqb.com/Article/details/gppewzpkn.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.yfazqb.com/Article/details/ghjrphgad.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.bbcook.cn/Article/details/gvfdnwdrs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.sjlbkw.cn/Article/details/gbqcagfgg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.bbcook.cn/Article/details/gjvbbigzk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.yfazqb.com/Article/details/gkmlrxulj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.tarul.cn/Article/details/gskjfjlnf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.vehdjk.com/Article/details/gtgwaofom.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.sjlbkw.cn/Article/details/gqsgnscyn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.epnwcf.com/Article/details/giblooizg.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.vehdjk.com/Article/details/gzvsvdagm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.yfazqb.com/Article/details/gcqhabolb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.yfazqb.com/Article/details/gclkqurcu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbqrvghk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.tarul.cn/Article/details/gvflhegpu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.tarul.cn/Article/details/gcjqqgyeo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.epnwcf.com/Article/details/gclnddswz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.sjlbkw.cn/Article/details/gckpvamjf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.tarul.cn/Article/details/gaxlkcklh.sHtML

[N05] 最大公约数
来源：http://baike.epnwcf.com/Article/details/gthrmyaic.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.tarul.cn/Article/details/guhftyuhf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.yfazqb.com/Article/details/gfvbwgsqh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.bbcook.cn/Article/details/giyvrdszi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.tarul.cn/Article/details/gyoiwogob.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.bbcook.cn/Article/details/gviziyxft.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fktsv.cn/Article/details/gdiyywghx.sHtML

Ruby: a.gcd(b)
来源：http://mobile.sjlbkw.cn/Article/details/gfewvchuc.sHtML


<!-- 参考信息 -->