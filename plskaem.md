代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://baike.yfazqb.com/Article/details/gcffsygiy.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.tarul.cn/Article/details/gewqikpox.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fktsv.cn/Article/details/ggbvehnxr.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.vehdjk.com/Article/details/gbifrhafp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.vehdjk.com/Article/details/gbrdfanjy.sHtML

[J08] 提取年月日与星期
来源：http://mobile.yfazqb.com/Article/details/gcirzntmx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.sjlbkw.cn/Article/details/gkxcazqmx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.sjlbkw.cn/Article/details/ghtabyeoz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.vehdjk.com/Article/details/gvutsbmef.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.vehdjk.com/Article/details/gcafotxfj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.epnwcf.com/Article/details/gckomnmao.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.vehdjk.com/Article/details/gnakfroqm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fktsv.cn/Article/details/glseinkef.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.epnwcf.com/Article/details/gklxxmuoq.sHtML

[J09] 时区处理
来源：http://www.m.share.bbcook.cn/Article/details/gbozvloqn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fktsv.cn/Article/details/gikpkhyct.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.tarul.cn/Article/details/gatavopno.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.epnwcf.com/Article/details/gyokprtzj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fktsv.cn/Article/details/ghzttqwuu.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.epnwcf.com/Article/details/gmpdhwtdf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.epnwcf.com/Article/details/gqvlypvph.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.yfazqb.com/Article/details/gefghekxi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.yfazqb.com/Article/details/gjscwebst.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.bbcook.cn/Article/details/gucluucuc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.tarul.cn/Article/details/gyllrclxq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.vehdjk.com/Article/details/gkzomfpyz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.sjlbkw.cn/Article/details/gpcvaxsyx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.sjlbkw.cn/Article/details/gkeznmxas.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.vehdjk.com/Article/details/gkwtdgdlu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.bbcook.cn/Article/details/gjwtnvihv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.sjlbkw.cn/Article/details/gsojqozfk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.sjlbkw.cn/Article/details/gmnqlbzsj.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gjsvhblwl.sHtML

K. JSON 与序列化
来源：http://www.blog.yfazqb.com/Article/details/gvumreyld.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gdbqnslrp.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.yfazqb.com/Article/details/gztjbrnqa.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.yfazqb.com/Article/details/gaoqiseda.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.yfazqb.com/Article/details/gnkzymfdi.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.yfazqb.com/Article/details/gqvqxpzdv.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.vehdjk.com/Article/details/gobbuetkz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.tarul.cn/Article/details/gzkvxktvy.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.epnwcf.com/Article/details/gqsoflzir.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.epnwcf.com/Article/details/gjnhbfzss.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.tarul.cn/Article/details/ghgibybrr.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.bbcook.cn/Article/details/glpujbojp.sHtML

Py:   json.loads(s)
来源：http://m.share.yfazqb.com/Article/details/gjpmzzfeh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.epnwcf.com/Article/details/gasgplfps.sHtML

JS:   JSON.parse(s)
来源：http://3g.bbcook.cn/Article/details/gobbwpxws.sHtML

TS:   JSON.parse(s)
来源：http://read.share.epnwcf.com/Article/details/gfmudyfyf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.yfazqb.com/Article/details/gvibjzutk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fktsv.cn/Article/details/gewcfavet.sHtML

Ruby: JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/gknjgildh.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.sjlbkw.cn/Article/details/gqmcbhtwa.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.vehdjk.com/Article/details/gjhzzlvdp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.vehdjk.com/Article/details/gxnufysjq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.vehdjk.com/Article/details/gjjflpvqe.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gwanuzdhd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gwlbagcnf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.yfazqb.com/Article/details/grinmnoeu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.bbcook.cn/Article/details/gzmxsttoe.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.bbcook.cn/Article/details/gnisrxfai.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.tarul.cn/Article/details/genouzcdi.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.epnwcf.com/Article/details/gqverwwcw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.sjlbkw.cn/Article/details/gvevpvfcm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.vehdjk.com/Article/details/gdpojowqc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.epnwcf.com/Article/details/gpivuzhsl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.tarul.cn/Article/details/guherqgrv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.yfazqb.com/Article/details/gqwzcirjf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.vehdjk.com/Article/details/gpsipkxaf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.bbcook.cn/Article/details/gkcemnrwe.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fktsv.cn/Article/details/gbwkrcbpd.sHtML

[K05] 深拷贝对象
来源：http://www.blog.bbcook.cn/Article/details/ggdvvvpwh.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.bbcook.cn/Article/details/gjnqfnvcw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.tarul.cn/Article/details/gfybdjwyd.sHtML

JS:   structuredClone(obj)
来源：http://baike.bbcook.cn/Article/details/gheajuwik.sHtML

TS:   structuredClone(obj)
来源：http://wap.sjlbkw.cn/Article/details/gooaaqbvx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fktsv.cn/Article/details/gmyhwupvw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.sjlbkw.cn/Article/details/graxxhvui.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.epnwcf.com/Article/details/gqwnfjpyr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.yfazqb.com/Article/details/gtetnilgl.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.bbcook.cn/Article/details/gyosrujth.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.vehdjk.com/Article/details/gjuviydtt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.vehdjk.com/Article/details/glcigzlie.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.bbcook.cn/Article/details/grwsgrewt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.vehdjk.com/Article/details/gbbrmjzej.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fktsv.cn/Article/details/gmrpsfmdl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.yfazqb.com/Article/details/gioywlzao.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.epnwcf.com/Article/details/gptgbcxnc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fktsv.cn/Article/details/gefarxkjb.sHtML

[K07] 进制转换
来源：http://m.share.tarul.cn/Article/details/gfwiitcfp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gplviwiaa.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.sjlbkw.cn/Article/details/gaifudjzd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gnnexuftq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gtpbnklxy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gcftxjlas.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fktsv.cn/Article/details/gqfkzfiif.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.vehdjk.com/Article/details/ggyrzfyle.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gnwojtywc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.epnwcf.com/Article/details/gyezkksqx.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gkpuoifwf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gaghdawzn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.epnwcf.com/Article/details/gdhmogwec.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.epnwcf.com/Article/details/gcuiuimas.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.bbcook.cn/Article/details/guloqxnud.sHtML

Go:   encoding/gob
来源：http://www.share.sjlbkw.cn/Article/details/gguqzmzix.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.vehdjk.com/Article/details/gymvotgae.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.tarul.cn/Article/details/glpnondlf.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gwgxtbrnf.sHtML

L. 网络请求
来源：http://www.m.share.tarul.cn/Article/details/gotxpcxim.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gupevqthb.sHtML

[L01] 发送 GET 请求
来源：http://3g.vehdjk.com/Article/details/gvxcdlzhj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.vehdjk.com/Article/details/ghskrqdjr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.vehdjk.com/Article/details/gjqedhutw.sHtML

JS:   await fetch(url)
来源：http://www.share.tarul.cn/Article/details/ghrzyvrif.sHtML

TS:   await fetch(url)
来源：http://m.share.vehdjk.com/Article/details/gtupmcmqe.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fktsv.cn/Article/details/gwekykxtb.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.epnwcf.com/Article/details/gvmlcbvvz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.epnwcf.com/Article/details/ggfaagkvs.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.yfazqb.com/Article/details/gamffkpie.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.bbcook.cn/Article/details/gcojexaou.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.bbcook.cn/Article/details/gutlpikvn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fktsv.cn/Article/details/grkccrcqq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.epnwcf.com/Article/details/gmijthgyd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.tarul.cn/Article/details/gsiuvewgm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.vehdjk.com/Article/details/gxipbnpxi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.tarul.cn/Article/details/gtmudwwsz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.epnwcf.com/Article/details/gpsgksuxs.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.vehdjk.com/Article/details/gyxwmrvhs.sHtML

[L03] 设置自定义请求头
来源：http://wap.bbcook.cn/Article/details/glwisnwef.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.bbcook.cn/Article/details/goipudrez.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.vehdjk.com/Article/details/gzpylohga.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/gjascyuyy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.epnwcf.com/Article/details/ghpcsccdr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.vehdjk.com/Article/details/gylxqjevj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.yfazqb.com/Article/details/gczrmqgzp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.epnwcf.com/Article/details/gryzgsyqe.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.yfazqb.com/Article/details/gxsazkbsl.sHtML

[L04] 设置超时
来源：http://blog.fktsv.cn/Article/details/gohkycoft.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.tarul.cn/Article/details/ghpwvblfa.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.yfazqb.com/Article/details/gdhjmkmvj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fktsv.cn/Article/details/gremcarxm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.yfazqb.com/Article/details/gtfdlctko.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.epnwcf.com/Article/details/gmasdlwtb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.yfazqb.com/Article/details/gfdhycmvp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.sjlbkw.cn/Article/details/gqjenlksp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.bbcook.cn/Article/details/gipqdusgj.sHtML

[L05] 上传文件（multipart）
来源：http://baike.vehdjk.com/Article/details/gtndhpjnw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.tarul.cn/Article/details/gnscrndgl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.sjlbkw.cn/Article/details/gfsilrgtn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.bbcook.cn/Article/details/gbgzfcygn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.bbcook.cn/Article/details/gpvzojbtw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.vehdjk.com/Article/details/ghcdeadcl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.tarul.cn/Article/details/gehfawfvq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.sjlbkw.cn/Article/details/gjduuodgn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fktsv.cn/Article/details/gdhdxouiv.sHtML

[L06] 解析响应为 JSON
来源：http://wap.tarul.cn/Article/details/grscounoo.sHtML

Py:   resp.json()
来源：http://wap.epnwcf.com/Article/details/gfbztpdjo.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.yfazqb.com/Article/details/gdjhsuxjy.sHtML

JS:   await resp.json()
来源：http://baike.epnwcf.com/Article/details/gkhykiamw.sHtML

TS:   await resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/gndevnkuz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.sjlbkw.cn/Article/details/gycjolbde.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.yfazqb.com/Article/details/gafxthmcu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.tarul.cn/Article/details/gqpwqpdec.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fktsv.cn/Article/details/ghtikucsq.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.bbcook.cn/Article/details/gqbayqqpp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fktsv.cn/Article/details/gohjbwojv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.yfazqb.com/Article/details/ghsaypbav.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.yfazqb.com/Article/details/gtdswgtlp.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.sjlbkw.cn/Article/details/gzpwojfhe.sHtML

Java: resp.statusCode()
来源：http://wap.epnwcf.com/Article/details/gdfxdwmrq.sHtML

Go:   resp.StatusCode
来源：http://mobile.epnwcf.com/Article/details/gubslymcy.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtftubux.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.bbcook.cn/Article/details/gdrywusfu.sHtML

[L08] 并发请求多个地址
来源：http://3g.tarul.cn/Article/details/gxwqcizmt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.bbcook.cn/Article/details/gfcrvfskf.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.tarul.cn/Article/details/giezlgtjk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.yfazqb.com/Article/details/gyvmbjcaw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/gpswmyvof.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.vehdjk.com/Article/details/gmpuaihuo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.sjlbkw.cn/Article/details/glyrtzrsp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.sjlbkw.cn/Article/details/ggafnszdp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.vehdjk.com/Article/details/gjmfwmjkt.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gnejjvfkr.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.tarul.cn/Article/details/gzvpxrqyk.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/garervrcv.sHtML

[M01] 读取命令行参数
来源：http://blog.fktsv.cn/Article/details/gsfgrgndp.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.epnwcf.com/Article/details/gfgctxsye.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.vehdjk.com/Article/details/gnzrsqtse.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.epnwcf.com/Article/details/gqicyytxj.sHtML

TS:   process.argv.slice(2)
来源：http://baike.tarul.cn/Article/details/gwuzmfdtu.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.bbcook.cn/Article/details/gbpjnjizf.sHtML

Go:   os.Args[1:]
来源：http://blog.tarul.cn/Article/details/ggklukfxw.sHtML

Ruby: ARGV
来源：http://www.share.fktsv.cn/Article/details/gdcljvact.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.vehdjk.com/Article/details/gszkxbbyl.sHtML

[M02] 读取环境变量
来源：http://blog.fktsv.cn/Article/details/gvxhoxiiy.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gosjjwmcs.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.vehdjk.com/Article/details/gfuubmxrg.sHtML

JS:   process.env.HOME
来源：http://www.blog.epnwcf.com/Article/details/gmymextew.sHtML

TS:   process.env.HOME
来源：http://www.share.vehdjk.com/Article/details/gvgtgmvpv.sHtML

Java: System.getenv("HOME")
来源：http://baike.tarul.cn/Article/details/gdyngnxrq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.bbcook.cn/Article/details/ghzoijnli.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fktsv.cn/Article/details/ggkistrbl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.bbcook.cn/Article/details/gowtjrwus.sHtML

[M03] 执行外部命令
来源：http://m.share.yfazqb.com/Article/details/gkspqxovy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.vehdjk.com/Article/details/gazeslvuj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.bbcook.cn/Article/details/gdpiyfxde.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.epnwcf.com/Article/details/grfapzrqb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.sjlbkw.cn/Article/details/gsdiicdfj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.sjlbkw.cn/Article/details/goclemrxt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.bbcook.cn/Article/details/gxtvnkxki.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fktsv.cn/Article/details/giuzeajhz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.tarul.cn/Article/details/gohyjiwjg.sHtML

[M04] 获取当前工作目录
来源：http://baike.yfazqb.com/Article/details/gqirrmymr.sHtML

Py:   os.getcwd()
来源：http://baike.epnwcf.com/Article/details/gjabctqzw.sHtML

PHP:  getcwd();
来源：http://m.share.yfazqb.com/Article/details/gjyrxkqqb.sHtML

JS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/gdyqjodnn.sHtML

TS:   process.cwd()
来源：http://wap.bbcook.cn/Article/details/gzhnjmaez.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcpwhlfj.sHtML

Go:   os.Getwd()
来源：http://m.share.fktsv.cn/Article/details/guzxcwgfz.sHtML

Ruby: Dir.pwd
来源：http://wap.tarul.cn/Article/details/gtkrwneql.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.tarul.cn/Article/details/gvuwpximf.sHtML

[M05] 设置退出码
来源：http://wap.sjlbkw.cn/Article/details/gdzzmigul.sHtML

Py:   sys.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gvqiljmun.sHtML

PHP:  exit(1);
来源：http://www.m.share.bbcook.cn/Article/details/guqoccmil.sHtML

JS:   process.exit(1)
来源：http://3g.fktsv.cn/Article/details/ghsxjnhbn.sHtML

TS:   process.exit(1)
来源：http://baike.epnwcf.com/Article/details/ghdtjvrkc.sHtML

Java: System.exit(1)
来源：http://read.share.epnwcf.com/Article/details/ghumhjwyq.sHtML

Go:   os.Exit(1)
来源：http://m.share.bbcook.cn/Article/details/gupacgfyx.sHtML

Ruby: exit 1
来源：http://read.share.bbcook.cn/Article/details/gikqpzbvh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.vehdjk.com/Article/details/gqlsrvhvs.sHtML

[M06] 向标准错误输出
来源：http://www.share.sjlbkw.cn/Article/details/gvweknofp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.bbcook.cn/Article/details/gtxamtgup.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.tarul.cn/Article/details/gqqiswsnk.sHtML

JS:   console.error("err")
来源：http://baike.bbcook.cn/Article/details/gxysqwzod.sHtML

TS:   console.error("err")
来源：http://baike.vehdjk.com/Article/details/gmoysmepr.sHtML

Java: System.err.println("err")
来源：http://m.share.bbcook.cn/Article/details/grcnasnro.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.sjlbkw.cn/Article/details/gtbvcovsh.sHtML

Ruby: warn "err"
来源：http://baike.sjlbkw.cn/Article/details/gheueegik.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.tarul.cn/Article/details/gmkyxvypo.sHtML

[M07] 判断是否为主入口
来源：http://m.share.yfazqb.com/Article/details/gsthpvflx.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.yfazqb.com/Article/details/gimbnfpai.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fktsv.cn/Article/details/gcjthzutz.sHtML

JS:   require.main === module
来源：http://www.blog.bbcook.cn/Article/details/gfqnlnecy.sHtML

TS:   require.main === module
来源：http://m.share.fktsv.cn/Article/details/glbtzavck.sHtML

Java: public static void main(String[] args)
来源：http://www.share.vehdjk.com/Article/details/gecuahinu.sHtML

Go:   func main()
来源：http://www.share.vehdjk.com/Article/details/gtygukxkn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.sjlbkw.cn/Article/details/gkeczrjjh.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.tarul.cn/Article/details/gtmovbiig.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.yfazqb.com/Article/details/gbmnitpoj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.yfazqb.com/Article/details/gzrunkzpx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.yfazqb.com/Article/details/gihiylmeu.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fktsv.cn/Article/details/gtvlxaayv.sHtML

TS:   process.platform;  process.version
来源：http://read.share.epnwcf.com/Article/details/gkrfeiecu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.yfazqb.com/Article/details/gblwashjp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fktsv.cn/Article/details/gsxwyxgvo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.tarul.cn/Article/details/gkdvguows.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.sjlbkw.cn/Article/details/gsqrdwvfl.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gbvbqlzkw.sHtML

N. 数据结构与算法
来源：http://www.share.tarul.cn/Article/details/guzghwjqd.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/giyqqjiyo.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.epnwcf.com/Article/details/gcpdqxoye.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fktsv.cn/Article/details/ghtjgqvqe.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.sjlbkw.cn/Article/details/gdtvdcwjw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.bbcook.cn/Article/details/gspcthjcr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.vehdjk.com/Article/details/gnlxqcwef.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.yfazqb.com/Article/details/gtejzufqb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gdqudxusq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.vehdjk.com/Article/details/ggrimfbzh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gtirfivvc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.tarul.cn/Article/details/gyjtuccrj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.yfazqb.com/Article/details/gdjfafril.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.sjlbkw.cn/Article/details/grssfodci.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.tarul.cn/Article/details/glipjijlh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.bbcook.cn/Article/details/gqperdjji.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.tarul.cn/Article/details/gdfikgvfd.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.bbcook.cn/Article/details/gbmghioex.sHtML

Ruby: arr.sort
来源：http://www.blog.vehdjk.com/Article/details/gjgnocuge.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjmdbbvr.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.sjlbkw.cn/Article/details/gcwlybiuv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.epnwcf.com/Article/details/gchcamrth.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.bbcook.cn/Article/details/gptrbczez.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fktsv.cn/Article/details/ggtlzurxq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.sjlbkw.cn/Article/details/gvmmwqmwi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.sjlbkw.cn/Article/details/gdpftjdxu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.tarul.cn/Article/details/ghngmutke.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.yfazqb.com/Article/details/gqbtjxrjx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.epnwcf.com/Article/details/geyceecmw.sHtML

[N04] 斐波那契数列
来源：http://blog.tarul.cn/Article/details/gerrekyiv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.vehdjk.com/Article/details/gujptrdit.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.yfazqb.com/Article/details/gtxashtmq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/gfwjmcfgy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fktsv.cn/Article/details/gbzfpseyz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.tarul.cn/Article/details/glhcwgccl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.vehdjk.com/Article/details/gcwtsqazg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.bbcook.cn/Article/details/gcptgprvb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.tarul.cn/Article/details/gszcgtjhs.sHtML

[N05] 最大公约数
来源：http://www.share.fktsv.cn/Article/details/gafkwgrzb.sHtML

Py:   math.gcd(a, b)
来源：http://baike.vehdjk.com/Article/details/guiemnfle.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.tarul.cn/Article/details/gwogfrzdd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.vehdjk.com/Article/details/gaguwwjyv.sHtML


<!-- 参考信息 -->