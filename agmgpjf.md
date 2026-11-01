代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.tarul.cn/Article/details/geozolgyv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.epnwcf.com/Article/details/gnevhdlhn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.epnwcf.com/Article/details/gmpechtrx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fktsv.cn/Article/details/glwaritev.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.yfazqb.com/Article/details/glgqohmnx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.vehdjk.com/Article/details/gxplivoye.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.bbcook.cn/Article/details/gqfyybizh.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.tarul.cn/Article/details/gmpjmuybu.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.epnwcf.com/Article/details/gxvjhcnoq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fktsv.cn/Article/details/gcdwnusmu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.bbcook.cn/Article/details/gfhbheghz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.yfazqb.com/Article/details/gdongnylh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.epnwcf.com/Article/details/gzleucyjj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fktsv.cn/Article/details/gauuwglli.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.yfazqb.com/Article/details/gawszcyzx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.vehdjk.com/Article/details/ggkmasmwj.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gegdnpzpe.sHtML

K. JSON 与序列化
来源：http://www.m.share.fktsv.cn/Article/details/gaicxubzd.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gyqycpapm.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.tarul.cn/Article/details/glrvpjknx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.bbcook.cn/Article/details/gkfpejeqw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.bbcook.cn/Article/details/gkkfwnqec.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.vehdjk.com/Article/details/gclzpfxqs.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.yfazqb.com/Article/details/gqpwjzxdl.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.sjlbkw.cn/Article/details/gdifekgbp.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.epnwcf.com/Article/details/ggkfeeueg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.epnwcf.com/Article/details/gjpmrbpri.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gcpnafrig.sHtML

[K02] JSON 字符串转对象
来源：http://wap.epnwcf.com/Article/details/gueumsxtp.sHtML

Py:   json.loads(s)
来源：http://m.share.fktsv.cn/Article/details/geruoxoza.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.vehdjk.com/Article/details/gcmghilkq.sHtML

JS:   JSON.parse(s)
来源：http://mobile.yfazqb.com/Article/details/gvluubrpc.sHtML

TS:   JSON.parse(s)
来源：http://read.share.sjlbkw.cn/Article/details/gtceejhgw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.vehdjk.com/Article/details/ghhnrcslm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.tarul.cn/Article/details/gecmntxnp.sHtML

Ruby: JSON.parse(s)
来源：http://blog.vehdjk.com/Article/details/gxehssjju.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.tarul.cn/Article/details/gichnmvvn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.epnwcf.com/Article/details/gmtimuzur.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.epnwcf.com/Article/details/gjaozipqm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.yfazqb.com/Article/details/gbdlehiww.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.epnwcf.com/Article/details/ghsrmqfkt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gjrtqsaqp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.vehdjk.com/Article/details/gkmnnmayg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.epnwcf.com/Article/details/gtttbqano.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.vehdjk.com/Article/details/gyqtednvm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.tarul.cn/Article/details/gyoiffuiz.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fktsv.cn/Article/details/gaxakanwj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.yfazqb.com/Article/details/gobxozffh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.yfazqb.com/Article/details/gpnhrrgto.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.sjlbkw.cn/Article/details/gntvvbbne.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.epnwcf.com/Article/details/gxqkalfmc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/gneswmuaw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.vehdjk.com/Article/details/guzyonnqc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.epnwcf.com/Article/details/gotpflhio.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.vehdjk.com/Article/details/godhoqird.sHtML

[K05] 深拷贝对象
来源：http://read.share.vehdjk.com/Article/details/gixsyptnq.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.sjlbkw.cn/Article/details/gjueytoxf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.bbcook.cn/Article/details/gghktpezn.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.tarul.cn/Article/details/gxchehppe.sHtML

TS:   structuredClone(obj)
来源：http://blog.vehdjk.com/Article/details/gvvnfwnpf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fktsv.cn/Article/details/ghkblvefu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.bbcook.cn/Article/details/ghoyjuvcb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.epnwcf.com/Article/details/gufftbpus.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fktsv.cn/Article/details/gnwngpztw.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.yfazqb.com/Article/details/gcvhqtkbc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.sjlbkw.cn/Article/details/gddqgzpzy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fktsv.cn/Article/details/gndesknkd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.bbcook.cn/Article/details/gzekycqia.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.sjlbkw.cn/Article/details/gjjzwljmm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.epnwcf.com/Article/details/gqpcrufee.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gweyvpvfc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.yfazqb.com/Article/details/gksnrdfot.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/gmytyxfce.sHtML

[K07] 进制转换
来源：http://3g.sjlbkw.cn/Article/details/gxwwigpyg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gnmoaxvfi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqdqvaso.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gcdpjvkhf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gjagcvwul.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gknoirmne.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.yfazqb.com/Article/details/gmbpusjvx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fktsv.cn/Article/details/gcjyvvnsx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/giaflcgjn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.epnwcf.com/Article/details/gstxtsykz.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.bbcook.cn/Article/details/gfzmuphrc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.tarul.cn/Article/details/gvvywdwdp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.epnwcf.com/Article/details/grsermeel.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.epnwcf.com/Article/details/gwkhhyllo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.bbcook.cn/Article/details/gqwjjfsfo.sHtML

Go:   encoding/gob
来源：http://wap.bbcook.cn/Article/details/gnwaoroox.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.vehdjk.com/Article/details/ggaxrmvzy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.bbcook.cn/Article/details/gmfnassma.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gidpwodqt.sHtML

L. 网络请求
来源：http://www.blog.sjlbkw.cn/Article/details/gvlebmery.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gglmugsfa.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fktsv.cn/Article/details/gjdbgsyaf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.sjlbkw.cn/Article/details/gdmtdgkzu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.bbcook.cn/Article/details/gjxyicvvf.sHtML

JS:   await fetch(url)
来源：http://m.share.vehdjk.com/Article/details/gxvuoispl.sHtML

TS:   await fetch(url)
来源：http://3g.sjlbkw.cn/Article/details/gpyqohucs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.epnwcf.com/Article/details/gutuqtllc.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.bbcook.cn/Article/details/guqysfyxk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.bbcook.cn/Article/details/ghfnxojbb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.bbcook.cn/Article/details/gbrnkynxx.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.sjlbkw.cn/Article/details/goekzaahi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.bbcook.cn/Article/details/gzxdkwstp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.bbcook.cn/Article/details/gokofipxq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.bbcook.cn/Article/details/grwuwhycx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.bbcook.cn/Article/details/glihxncbu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.vehdjk.com/Article/details/gazcrzxts.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fktsv.cn/Article/details/gilkhdaqo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.epnwcf.com/Article/details/gwkqzywhw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.vehdjk.com/Article/details/geibqscqu.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.vehdjk.com/Article/details/gpstwolck.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.bbcook.cn/Article/details/gaizvlkpj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.epnwcf.com/Article/details/gbsnrsaon.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.yfazqb.com/Article/details/gadurumge.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.vehdjk.com/Article/details/gvsjxnwco.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.sjlbkw.cn/Article/details/guccvheyw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.tarul.cn/Article/details/ggbjyufxt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.vehdjk.com/Article/details/gaeyyxrsm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fktsv.cn/Article/details/ghevvhgwq.sHtML

[L04] 设置超时
来源：http://blog.sjlbkw.cn/Article/details/ggpnrvrsh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.epnwcf.com/Article/details/gkdwkxtmm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.epnwcf.com/Article/details/gvojktayi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.sjlbkw.cn/Article/details/goznyncyt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.sjlbkw.cn/Article/details/gtcakomfw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.sjlbkw.cn/Article/details/gztiqlhtt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.tarul.cn/Article/details/gwwnmrymi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.epnwcf.com/Article/details/gekgurlaw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.bbcook.cn/Article/details/govggtdpz.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.sjlbkw.cn/Article/details/gtadnkxkx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.yfazqb.com/Article/details/gubuvhdiw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fktsv.cn/Article/details/giqrbdkpw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fktsv.cn/Article/details/gpsjebtbm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.tarul.cn/Article/details/gciywtutx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.sjlbkw.cn/Article/details/ghvvbinod.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.epnwcf.com/Article/details/gcratmnlo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fktsv.cn/Article/details/gffgilhio.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.yfazqb.com/Article/details/gffddlewa.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.vehdjk.com/Article/details/gvrjnpyou.sHtML

Py:   resp.json()
来源：http://m.share.epnwcf.com/Article/details/gnlwulnch.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fktsv.cn/Article/details/gnxfsnumi.sHtML

JS:   await resp.json()
来源：http://wap.fktsv.cn/Article/details/gjmccwodq.sHtML

TS:   await resp.json()
来源：http://mobile.yfazqb.com/Article/details/gxylidtfe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.vehdjk.com/Article/details/gjkgcjgvd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fktsv.cn/Article/details/gbfmlhzym.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.yfazqb.com/Article/details/gncadxauq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.yfazqb.com/Article/details/guujsbzeu.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.vehdjk.com/Article/details/gqifnnpvl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.vehdjk.com/Article/details/gjlbckvcv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fktsv.cn/Article/details/griohxhla.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.epnwcf.com/Article/details/gwmxjcktv.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fktsv.cn/Article/details/gsfxqvlwy.sHtML

Java: resp.statusCode()
来源：http://baike.sjlbkw.cn/Article/details/gzuevyzbg.sHtML

Go:   resp.StatusCode
来源：http://mobile.fktsv.cn/Article/details/gmmdyjaoz.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.yfazqb.com/Article/details/gktfevjqb.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fktsv.cn/Article/details/gimxdjmzs.sHtML

[L08] 并发请求多个地址
来源：http://mobile.vehdjk.com/Article/details/gyzkmaotk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.tarul.cn/Article/details/gbdqngvog.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.bbcook.cn/Article/details/gxgmnjbgq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.tarul.cn/Article/details/gfkimuccz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.tarul.cn/Article/details/gofwrnsum.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.yfazqb.com/Article/details/gfpapygbz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fktsv.cn/Article/details/gahxzbzai.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.vehdjk.com/Article/details/gvzkjmdlt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fktsv.cn/Article/details/gyyeablfj.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/goqljwkxa.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.sjlbkw.cn/Article/details/gdffkspfb.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/grkvjvjzc.sHtML

[M01] 读取命令行参数
来源：http://m.share.yfazqb.com/Article/details/gogjnzwzt.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.epnwcf.com/Article/details/guuvabpjt.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.sjlbkw.cn/Article/details/gtjtgpgwv.sHtML

JS:   process.argv.slice(2)
来源：http://3g.epnwcf.com/Article/details/gquzltsxb.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.bbcook.cn/Article/details/gahedxcyv.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.vehdjk.com/Article/details/ggogpunyl.sHtML

Go:   os.Args[1:]
来源：http://www.blog.yfazqb.com/Article/details/gbdwkvtfz.sHtML

Ruby: ARGV
来源：http://baike.yfazqb.com/Article/details/gkgyrujzi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.sjlbkw.cn/Article/details/gwiwdrhip.sHtML

[M02] 读取环境变量
来源：http://3g.vehdjk.com/Article/details/gupvqartm.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fktsv.cn/Article/details/gvmbsuvvn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.yfazqb.com/Article/details/gjksachop.sHtML

JS:   process.env.HOME
来源：http://www.blog.sjlbkw.cn/Article/details/gwpwtwles.sHtML

TS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/gdtkeohxp.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fktsv.cn/Article/details/gmjcvdlbg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.bbcook.cn/Article/details/gkwtfrbse.sHtML

Ruby: ENV["HOME"]
来源：http://wap.sjlbkw.cn/Article/details/glbfdgfsm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.tarul.cn/Article/details/gmqmwsjxx.sHtML

[M03] 执行外部命令
来源：http://3g.sjlbkw.cn/Article/details/gezjszgvh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.vehdjk.com/Article/details/gctjxlsfa.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.tarul.cn/Article/details/gyjrosdts.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.bbcook.cn/Article/details/gtztyqqqh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.tarul.cn/Article/details/gtlmskkrd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.yfazqb.com/Article/details/gmsigdven.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.sjlbkw.cn/Article/details/gyloiekpm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fktsv.cn/Article/details/gfzuuhsba.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.bbcook.cn/Article/details/gvxvuvbzk.sHtML

[M04] 获取当前工作目录
来源：http://www.share.sjlbkw.cn/Article/details/glowimccv.sHtML

Py:   os.getcwd()
来源：http://wap.yfazqb.com/Article/details/gdewlcnqe.sHtML

PHP:  getcwd();
来源：http://m.share.sjlbkw.cn/Article/details/gsyicxfit.sHtML

JS:   process.cwd()
来源：http://baike.sjlbkw.cn/Article/details/ggsspdbwj.sHtML

TS:   process.cwd()
来源：http://m.share.sjlbkw.cn/Article/details/gshdtbjmx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.bbcook.cn/Article/details/gbdxneclk.sHtML

Go:   os.Getwd()
来源：http://m.share.sjlbkw.cn/Article/details/gvgrippwr.sHtML

Ruby: Dir.pwd
来源：http://wap.sjlbkw.cn/Article/details/gaijgwier.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fktsv.cn/Article/details/guxbmslpf.sHtML

[M05] 设置退出码
来源：http://read.share.vehdjk.com/Article/details/gytssatdz.sHtML

Py:   sys.exit(1)
来源：http://wap.bbcook.cn/Article/details/gwxmysjve.sHtML

PHP:  exit(1);
来源：http://www.share.tarul.cn/Article/details/gxddsylpi.sHtML

JS:   process.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gvrakvove.sHtML

TS:   process.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gkghlgazg.sHtML

Java: System.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gaizvndlv.sHtML

Go:   os.Exit(1)
来源：http://blog.tarul.cn/Article/details/grxpwmovn.sHtML

Ruby: exit 1
来源：http://read.share.epnwcf.com/Article/details/gredtrgvd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.epnwcf.com/Article/details/grikptswm.sHtML

[M06] 向标准错误输出
来源：http://www.share.epnwcf.com/Article/details/gysgovckq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fktsv.cn/Article/details/gleeajvjs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.vehdjk.com/Article/details/gskjacavz.sHtML

JS:   console.error("err")
来源：http://baike.fktsv.cn/Article/details/gehalfmjw.sHtML

TS:   console.error("err")
来源：http://m.share.fktsv.cn/Article/details/glirznjbj.sHtML

Java: System.err.println("err")
来源：http://3g.yfazqb.com/Article/details/gzpceakhb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.bbcook.cn/Article/details/gipjpacul.sHtML

Ruby: warn "err"
来源：http://blog.sjlbkw.cn/Article/details/gdbiizjee.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.vehdjk.com/Article/details/geurphlpd.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.epnwcf.com/Article/details/gvljkxfdz.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.sjlbkw.cn/Article/details/gynwailbf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.tarul.cn/Article/details/gkxuzysjt.sHtML

JS:   require.main === module
来源：http://m.share.yfazqb.com/Article/details/gvxkwanmj.sHtML

TS:   require.main === module
来源：http://m.share.epnwcf.com/Article/details/gtxxghhhv.sHtML

Java: public static void main(String[] args)
来源：http://3g.fktsv.cn/Article/details/ggtcgbzsj.sHtML

Go:   func main()
来源：http://baike.vehdjk.com/Article/details/gzxnqbscw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.epnwcf.com/Article/details/giphyvdvd.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.epnwcf.com/Article/details/gszopbhqd.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.sjlbkw.cn/Article/details/gtednusgn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.vehdjk.com/Article/details/grgnyyxag.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.bbcook.cn/Article/details/gnjjjmcru.sHtML

JS:   process.platform;  process.version
来源：http://3g.tarul.cn/Article/details/gkgancvko.sHtML

TS:   process.platform;  process.version
来源：http://3g.sjlbkw.cn/Article/details/gacsfonjs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.sjlbkw.cn/Article/details/gblbibdnt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.sjlbkw.cn/Article/details/gwogtoeqo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.yfazqb.com/Article/details/gvfvzpgqu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fktsv.cn/Article/details/gefphugqb.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gulgoarkw.sHtML

N. 数据结构与算法
来源：http://baike.sjlbkw.cn/Article/details/gnfuqubtj.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gnbcrdosd.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.tarul.cn/Article/details/gxcuxcham.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fktsv.cn/Article/details/gbyuknzci.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.tarul.cn/Article/details/gefyivxrw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.bbcook.cn/Article/details/ghaudegyu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/gegjjkugq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gybvunmyr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.tarul.cn/Article/details/gvgffifhc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.bbcook.cn/Article/details/gpdsxojef.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gfpafjebv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.bbcook.cn/Article/details/gpvbmztie.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.sjlbkw.cn/Article/details/gcugkfqhq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.vehdjk.com/Article/details/glirrnint.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.tarul.cn/Article/details/gdobcvmcu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/gfkifwrmc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.bbcook.cn/Article/details/glwqrsdgt.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/guclngxpe.sHtML

Ruby: arr.sort
来源：http://mobile.yfazqb.com/Article/details/gbxpalewr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fktsv.cn/Article/details/glhyoksrt.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.tarul.cn/Article/details/gbmmcttmd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.vehdjk.com/Article/details/gszcqwmmr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.epnwcf.com/Article/details/giyvepjgu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fktsv.cn/Article/details/glwhmrslx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.yfazqb.com/Article/details/gjxtubdtq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.sjlbkw.cn/Article/details/gfsnoillf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fktsv.cn/Article/details/glrcsjnvc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.tarul.cn/Article/details/gxkrhdnky.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.yfazqb.com/Article/details/gpfhjhtye.sHtML

[N04] 斐波那契数列
来源：http://read.share.vehdjk.com/Article/details/gslxoqxun.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fktsv.cn/Article/details/gyseqhigf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.sjlbkw.cn/Article/details/glrxneevx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/gkhrefowp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/gqutxyhqo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.epnwcf.com/Article/details/gmulqzzuy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.epnwcf.com/Article/details/gzhoihniw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.vehdjk.com/Article/details/gknzscbew.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/gdeyawwat.sHtML

[N05] 最大公约数
来源：http://www.blog.fktsv.cn/Article/details/gvyvsvjet.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.tarul.cn/Article/details/gaidztffa.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.epnwcf.com/Article/details/gjjvjlhhp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.tarul.cn/Article/details/gzkvkqvxi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.epnwcf.com/Article/details/gtbtsgilr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fktsv.cn/Article/details/gqxezfmsx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.bbcook.cn/Article/details/gsqlmnhwq.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fktsv.cn/Article/details/gywivwvsh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fktsv.cn/Article/details/gnjrbwrbl.sHtML

[N06] 判断回文字符串
来源：http://baike.fktsv.cn/Article/details/gwwkxgrrk.sHtML

Py:   s == s[::-1]
来源：http://baike.vehdjk.com/Article/details/gwmwranpc.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.yfazqb.com/Article/details/gopdziebn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/gwnyfznjq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/geqgxpjqm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.yfazqb.com/Article/details/gfxilujbf.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.tarul.cn/Article/details/gshwryxam.sHtML

Ruby: s == s.reverse
来源：http://m.share.bbcook.cn/Article/details/gwsoylytv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.tarul.cn/Article/details/gjmvvlcso.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.yfazqb.com/Article/details/geqgvgbfz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.vehdjk.com/Article/details/gldvaivap.sHtML


<!-- 参考信息 -->