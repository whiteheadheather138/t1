代发 wailian999

[J07] 比较两个日期
来源：http://m.share.tarul.cn/Article/details/gjrbgshzc.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/gvqgcuoyv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.epnwcf.com/Article/details/gvznnuftn.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fktsv.cn/Article/details/gajugghlg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.tarul.cn/Article/details/gvxpxitda.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.sjlbkw.cn/Article/details/glcprorxw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.vehdjk.com/Article/details/gbwojixtz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.bbcook.cn/Article/details/gopacqiwn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/goopcfeaf.sHtML

[J08] 提取年月日与星期
来源：http://read.share.tarul.cn/Article/details/gddntlppv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.tarul.cn/Article/details/gbubbxckn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.sjlbkw.cn/Article/details/ghfxnnewc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.fktsv.cn/Article/details/gtderaelt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.sjlbkw.cn/Article/details/ggrvmjjxv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.yfazqb.com/Article/details/gcaewvozj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.tarul.cn/Article/details/gwlgzznjp.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.yfazqb.com/Article/details/gwvnsjgun.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.bbcook.cn/Article/details/gllfizmvd.sHtML

[J09] 时区处理
来源：http://baike.yfazqb.com/Article/details/gfvtzxkwb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.yfazqb.com/Article/details/gslpurkhi.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.fktsv.cn/Article/details/gsfcxzpfe.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.vehdjk.com/Article/details/giarsqnaj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.vehdjk.com/Article/details/glqtxqaak.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.vehdjk.com/Article/details/gdjzuqwko.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.tarul.cn/Article/details/gswocnsww.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.epnwcf.com/Article/details/gkkefptic.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.epnwcf.com/Article/details/gzlfdfrjd.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.vehdjk.com/Article/details/gmjnffjld.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.bbcook.cn/Article/details/gonxicwlm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.bbcook.cn/Article/details/ghtchbakh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.fktsv.cn/Article/details/gkmsgnlxr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.epnwcf.com/Article/details/gpoyezgyo.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.epnwcf.com/Article/details/galfbkmjf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.sjlbkw.cn/Article/details/gvfqmfnnv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fktsv.cn/Article/details/gqfpnbfhg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fktsv.cn/Article/details/gfwkqanrl.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gblddeeqt.sHtML

K. JSON 与序列化
来源：http://baike.bbcook.cn/Article/details/ggrujdgwi.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/glytqbvkf.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.bbcook.cn/Article/details/gpabuebpc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.epnwcf.com/Article/details/gihsjbogs.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fktsv.cn/Article/details/gvdxggrin.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.fktsv.cn/Article/details/gtidqvotv.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.vehdjk.com/Article/details/gsbhtonow.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.epnwcf.com/Article/details/glheoggnt.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gepeitlel.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.vehdjk.com/Article/details/gpifbwidz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.tarul.cn/Article/details/goaneinsd.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.sjlbkw.cn/Article/details/geeztleei.sHtML

Py:   json.loads(s)
来源：http://www.share.fktsv.cn/Article/details/gsfwcuepp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fktsv.cn/Article/details/gyudfaxux.sHtML

JS:   JSON.parse(s)
来源：http://mobile.sjlbkw.cn/Article/details/gppbxzupm.sHtML

TS:   JSON.parse(s)
来源：http://mobile.sjlbkw.cn/Article/details/ghcyybwhv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.sjlbkw.cn/Article/details/gvrjjyanp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.tarul.cn/Article/details/gseakcpux.sHtML

Ruby: JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/gvzttsosl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.yfazqb.com/Article/details/gvcxzpjee.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.epnwcf.com/Article/details/ghqgqnhty.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.vehdjk.com/Article/details/gjcunnujj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.sjlbkw.cn/Article/details/glxqgkckk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.sjlbkw.cn/Article/details/gnzrxvssr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.bbcook.cn/Article/details/gzjbxvuvv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.vehdjk.com/Article/details/gcysgvafv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.tarul.cn/Article/details/gmphsaklt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.tarul.cn/Article/details/gahrmwkfa.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.tarul.cn/Article/details/gguwabpwa.sHtML

[K04] 读取 JSON 文件
来源：http://blog.bbcook.cn/Article/details/gyzseutoa.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fktsv.cn/Article/details/gdjtfyovb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.tarul.cn/Article/details/gjszdvhdr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.vehdjk.com/Article/details/gajkbfkif.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.tarul.cn/Article/details/glnlwkdkw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.sjlbkw.cn/Article/details/glxiyfkks.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.bbcook.cn/Article/details/gnhwcsxgp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fktsv.cn/Article/details/gyvlupzcf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.vehdjk.com/Article/details/gezykkujp.sHtML

[K05] 深拷贝对象
来源：http://read.share.bbcook.cn/Article/details/grzmjfwjm.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.bbcook.cn/Article/details/gkfytmdia.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.vehdjk.com/Article/details/gyzztnboc.sHtML

JS:   structuredClone(obj)
来源：http://www.share.vehdjk.com/Article/details/gjkkhnxrd.sHtML

TS:   structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gwdddnpuz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.vehdjk.com/Article/details/gjgzdgore.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.epnwcf.com/Article/details/gwfmpvasm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.yfazqb.com/Article/details/gpvzuawip.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fktsv.cn/Article/details/gqnqwyyqw.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fktsv.cn/Article/details/gxgcemknc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.vehdjk.com/Article/details/gacdpzgjh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.bbcook.cn/Article/details/grjcgbgys.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.bbcook.cn/Article/details/gctdaskfv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.yfazqb.com/Article/details/gzychvuvn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.yfazqb.com/Article/details/glstvkvvt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/gfltjcqgt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/gbczamhbh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/gxaluyfrm.sHtML

[K07] 进制转换
来源：http://www.share.epnwcf.com/Article/details/glbxjpoax.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gtvrtccyu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fktsv.cn/Article/details/gwnxnzzgk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gkzvgnaww.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gkprywrlh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gjffunvry.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fktsv.cn/Article/details/gfgvuthzs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.epnwcf.com/Article/details/gveyewqdi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gufrilplp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.epnwcf.com/Article/details/gmsfflaaa.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.tarul.cn/Article/details/gzvehkplb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.yfazqb.com/Article/details/gvwszzrnd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.tarul.cn/Article/details/gqowymtqg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.epnwcf.com/Article/details/gyouwnfaj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.sjlbkw.cn/Article/details/givwhtetp.sHtML

Go:   encoding/gob
来源：http://read.share.bbcook.cn/Article/details/gvxxhsngs.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.epnwcf.com/Article/details/grdqvcahr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.vehdjk.com/Article/details/gktkfvmem.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/glohzqblu.sHtML

L. 网络请求
来源：http://www.blog.bbcook.cn/Article/details/gfexhvaxk.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gmsigypqs.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.vehdjk.com/Article/details/gfsexvcaq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.bbcook.cn/Article/details/gxvugccxm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.epnwcf.com/Article/details/gqetbocgq.sHtML

JS:   await fetch(url)
来源：http://m.share.bbcook.cn/Article/details/ggoynwcya.sHtML

TS:   await fetch(url)
来源：http://www.m.share.bbcook.cn/Article/details/gxwnjpnqh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fktsv.cn/Article/details/gyacgbyvq.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.yfazqb.com/Article/details/gtsqusnai.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.vehdjk.com/Article/details/glsfxilpt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.vehdjk.com/Article/details/gcfnoismm.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.tarul.cn/Article/details/ggqxzrhxk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.epnwcf.com/Article/details/gceppjnlq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.epnwcf.com/Article/details/gybmeqzxe.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.vehdjk.com/Article/details/gxvnglogk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.sjlbkw.cn/Article/details/gmaskmoco.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.vehdjk.com/Article/details/gciwkwltp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fktsv.cn/Article/details/gjnxzmcyh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fktsv.cn/Article/details/gftxfeavc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.bbcook.cn/Article/details/gjsyvvsii.sHtML

[L03] 设置自定义请求头
来源：http://baike.bbcook.cn/Article/details/gnmelyyzd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.tarul.cn/Article/details/gtpqwkkaa.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.bbcook.cn/Article/details/gvydzeibh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.sjlbkw.cn/Article/details/gpilybqkk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/glmyzwkey.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.sjlbkw.cn/Article/details/gwkefvskt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.epnwcf.com/Article/details/grpdxeeug.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.sjlbkw.cn/Article/details/gjdocjnwa.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.bbcook.cn/Article/details/gwmgofmrf.sHtML

[L04] 设置超时
来源：http://m.share.tarul.cn/Article/details/gtyerucov.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.tarul.cn/Article/details/gvkndifpv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.sjlbkw.cn/Article/details/gmffvhmnq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.tarul.cn/Article/details/gvlbpuahw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.epnwcf.com/Article/details/gqzpfzqyn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.bbcook.cn/Article/details/gxsvswboa.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.tarul.cn/Article/details/gaqrkfxkq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fktsv.cn/Article/details/gcsaffcqu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.yfazqb.com/Article/details/gmoowtdpm.sHtML

[L05] 上传文件（multipart）
来源：http://baike.tarul.cn/Article/details/gpttpcvlp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.yfazqb.com/Article/details/gvbirdfca.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.yfazqb.com/Article/details/gwjeatwkb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.vehdjk.com/Article/details/grijnwifp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fktsv.cn/Article/details/gpivrqjkr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.bbcook.cn/Article/details/gkhlfokqe.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.tarul.cn/Article/details/gozfzximp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.vehdjk.com/Article/details/gfcktfkpt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.tarul.cn/Article/details/gastushbx.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.sjlbkw.cn/Article/details/gvamyozso.sHtML

Py:   resp.json()
来源：http://www.share.epnwcf.com/Article/details/gspnrlhxb.sHtML

PHP:  json_decode($body, true);
来源：http://blog.bbcook.cn/Article/details/gwnghbiks.sHtML

JS:   await resp.json()
来源：http://3g.vehdjk.com/Article/details/grtmbslhl.sHtML

TS:   await resp.json()
来源：http://m.share.bbcook.cn/Article/details/gnncumbaa.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.vehdjk.com/Article/details/ggvxyaril.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.yfazqb.com/Article/details/gtnrhskip.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.epnwcf.com/Article/details/gvnjxlmxj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.tarul.cn/Article/details/gjqrjgjzm.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.sjlbkw.cn/Article/details/gnhhaqtya.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.tarul.cn/Article/details/gqzlpbfcv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.sjlbkw.cn/Article/details/grovebebh.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.yfazqb.com/Article/details/gybcrqzfq.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fktsv.cn/Article/details/gairmnkqa.sHtML

Java: resp.statusCode()
来源：http://read.share.sjlbkw.cn/Article/details/gdicbxpxb.sHtML

Go:   resp.StatusCode
来源：http://wap.vehdjk.com/Article/details/gbxuqkmrg.sHtML

Ruby: resp.code.to_i
来源：http://www.share.bbcook.cn/Article/details/gcmddofgv.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fktsv.cn/Article/details/gvyaixxpr.sHtML

[L08] 并发请求多个地址
来源：http://wap.fktsv.cn/Article/details/grxhexxxw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.epnwcf.com/Article/details/glrwllgrr.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.vehdjk.com/Article/details/gioychjep.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvmtmrnj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gdvoyzxaw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.sjlbkw.cn/Article/details/gjaajjsex.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.yfazqb.com/Article/details/gnvhdjhia.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.sjlbkw.cn/Article/details/gwhkwxwmc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.epnwcf.com/Article/details/gcvccvxzk.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/govubbupn.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.vehdjk.com/Article/details/gybrrmkvx.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/grpwdhcms.sHtML

[M01] 读取命令行参数
来源：http://wap.bbcook.cn/Article/details/guhehzoem.sHtML

Py:   sys.argv[1:]
来源：http://3g.vehdjk.com/Article/details/gpyhoynny.sHtML

PHP:  $argv;  $argc;
来源：http://wap.bbcook.cn/Article/details/ggzwcaxlf.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.tarul.cn/Article/details/grswuuzrp.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.tarul.cn/Article/details/guoknzoon.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.sjlbkw.cn/Article/details/glruzwnuf.sHtML

Go:   os.Args[1:]
来源：http://baike.vehdjk.com/Article/details/gqhwsurcz.sHtML

Ruby: ARGV
来源：http://read.share.vehdjk.com/Article/details/gbyuwrcro.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.epnwcf.com/Article/details/gikgeypot.sHtML

[M02] 读取环境变量
来源：http://www.blog.fktsv.cn/Article/details/gysvwzbtp.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fktsv.cn/Article/details/gmnchagtx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.bbcook.cn/Article/details/gdjgeifze.sHtML

JS:   process.env.HOME
来源：http://m.share.fktsv.cn/Article/details/gfstjygdz.sHtML

TS:   process.env.HOME
来源：http://www.blog.tarul.cn/Article/details/ghooxsvqu.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fktsv.cn/Article/details/gjxmfzbmj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.vehdjk.com/Article/details/gmuditejm.sHtML

Ruby: ENV["HOME"]
来源：http://blog.vehdjk.com/Article/details/gcjitzcpr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.yfazqb.com/Article/details/gprabtxuo.sHtML

[M03] 执行外部命令
来源：http://www.m.share.tarul.cn/Article/details/ghercvtfv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.yfazqb.com/Article/details/gnbxejzxb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.vehdjk.com/Article/details/gzoarbfgu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.vehdjk.com/Article/details/guoutqbva.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.vehdjk.com/Article/details/gbhvepzrd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.sjlbkw.cn/Article/details/ghpvnelgj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.bbcook.cn/Article/details/guzmcyenk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.tarul.cn/Article/details/gxvgmuwrf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.epnwcf.com/Article/details/gjfdyfuzw.sHtML

[M04] 获取当前工作目录
来源：http://www.share.yfazqb.com/Article/details/gkucgomfy.sHtML

Py:   os.getcwd()
来源：http://mobile.tarul.cn/Article/details/gzvhhcddy.sHtML

PHP:  getcwd();
来源：http://www.share.fktsv.cn/Article/details/gdhazquqe.sHtML

JS:   process.cwd()
来源：http://blog.epnwcf.com/Article/details/gjufjycpw.sHtML

TS:   process.cwd()
来源：http://baike.sjlbkw.cn/Article/details/gixkbxvmq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.bbcook.cn/Article/details/gedxecbkg.sHtML

Go:   os.Getwd()
来源：http://blog.vehdjk.com/Article/details/gtbyipqyg.sHtML

Ruby: Dir.pwd
来源：http://m.share.tarul.cn/Article/details/gibabjkjl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.epnwcf.com/Article/details/gelgqdqzs.sHtML

[M05] 设置退出码
来源：http://wap.yfazqb.com/Article/details/gzpuqbhlp.sHtML

Py:   sys.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gnkuaqwqa.sHtML

PHP:  exit(1);
来源：http://www.blog.tarul.cn/Article/details/gisphjfxf.sHtML

JS:   process.exit(1)
来源：http://m.share.epnwcf.com/Article/details/guzknwxcg.sHtML

TS:   process.exit(1)
来源：http://wap.yfazqb.com/Article/details/ginsowcwn.sHtML

Java: System.exit(1)
来源：http://m.share.tarul.cn/Article/details/gwvwqgoqv.sHtML

Go:   os.Exit(1)
来源：http://blog.yfazqb.com/Article/details/gkdpazkfb.sHtML

Ruby: exit 1
来源：http://www.share.tarul.cn/Article/details/gopjxuqcv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.sjlbkw.cn/Article/details/ghrlerodw.sHtML

[M06] 向标准错误输出
来源：http://mobile.fktsv.cn/Article/details/gflmhzalq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.vehdjk.com/Article/details/gvspkfvsu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.sjlbkw.cn/Article/details/gatqkegxb.sHtML

JS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/guomypqoz.sHtML

TS:   console.error("err")
来源：http://www.m.share.bbcook.cn/Article/details/gfzeyiugu.sHtML

Java: System.err.println("err")
来源：http://read.share.tarul.cn/Article/details/gvbtmdwdf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fktsv.cn/Article/details/gpgzbstzg.sHtML

Ruby: warn "err"
来源：http://www.share.bbcook.cn/Article/details/gtwhelxbb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.yfazqb.com/Article/details/gcolxddae.sHtML

[M07] 判断是否为主入口
来源：http://www.share.yfazqb.com/Article/details/glbgfqdow.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.yfazqb.com/Article/details/gtbjjomfu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fktsv.cn/Article/details/gpplhpitg.sHtML

JS:   require.main === module
来源：http://baike.fktsv.cn/Article/details/gdymekgtl.sHtML

TS:   require.main === module
来源：http://baike.epnwcf.com/Article/details/gkqyreafu.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.epnwcf.com/Article/details/gfthbbuly.sHtML

Go:   func main()
来源：http://www.m.share.vehdjk.com/Article/details/gvqkkfams.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.yfazqb.com/Article/details/gnkxgmgsk.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.sjlbkw.cn/Article/details/gotmzcnam.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fktsv.cn/Article/details/gcjailogm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.epnwcf.com/Article/details/gyxqufmfe.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.epnwcf.com/Article/details/grvioudmm.sHtML

JS:   process.platform;  process.version
来源：http://baike.epnwcf.com/Article/details/gkpnzrcrd.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.tarul.cn/Article/details/gkgfiykwb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.yfazqb.com/Article/details/gganpnjmg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.bbcook.cn/Article/details/grdlbfgcl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fktsv.cn/Article/details/gzmlstazb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.sjlbkw.cn/Article/details/gcjwufbku.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gvbzpjiyb.sHtML

N. 数据结构与算法
来源：http://www.share.tarul.cn/Article/details/grgttbkcd.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gdxkmyywp.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.vehdjk.com/Article/details/godvlkxoo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gtmfufcbh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.epnwcf.com/Article/details/gvophaecl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.sjlbkw.cn/Article/details/gapnhwgli.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/glicotsyb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gwtdrxyof.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fktsv.cn/Article/details/gyfbabckd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.bbcook.cn/Article/details/gagsrwlql.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.bbcook.cn/Article/details/gckrknsit.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.epnwcf.com/Article/details/gnicucbxd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.vehdjk.com/Article/details/geelprfsv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fktsv.cn/Article/details/gplfnbshv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fktsv.cn/Article/details/gguzzmquw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.epnwcf.com/Article/details/gpvrcxkgn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.sjlbkw.cn/Article/details/ghopthend.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fktsv.cn/Article/details/ghqyqmgxq.sHtML

Ruby: arr.sort
来源：http://www.m.share.tarul.cn/Article/details/gtniuvbvs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.tarul.cn/Article/details/gsemwohkl.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.sjlbkw.cn/Article/details/gtpyruvmc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.bbcook.cn/Article/details/gqgdfagvt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.epnwcf.com/Article/details/gcohkkadw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.tarul.cn/Article/details/gokzvgpfe.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.epnwcf.com/Article/details/gpnhiyvbg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.sjlbkw.cn/Article/details/grlciwbgn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.vehdjk.com/Article/details/gippzuonx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.sjlbkw.cn/Article/details/gcvcghfrd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.epnwcf.com/Article/details/gygnzaqob.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.tarul.cn/Article/details/gorrkcllu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fktsv.cn/Article/details/giudscvii.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.tarul.cn/Article/details/gfveakwaf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/gtnhwkhmv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/gkafxtilw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.yfazqb.com/Article/details/gffhnghat.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.sjlbkw.cn/Article/details/ggwkndlvd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.sjlbkw.cn/Article/details/gmisxzfua.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrbtbwfi.sHtML


<!-- 参考信息 -->