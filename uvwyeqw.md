代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.bbcook.cn/Article/details/goikvwkrq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.epnwcf.com/Article/details/gnhexpayu.sHtML

[J09] 时区处理
来源：http://www.m.share.vehdjk.com/Article/details/gbbpgnpdy.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.tarul.cn/Article/details/gyfhhvdqc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.bbcook.cn/Article/details/gofjaqqhu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.yfazqb.com/Article/details/gmugxdzha.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.vehdjk.com/Article/details/gghtcofzw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.epnwcf.com/Article/details/gjsskpcfp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.epnwcf.com/Article/details/grvfrervi.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fktsv.cn/Article/details/giypdidbm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjbukxzb.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.sjlbkw.cn/Article/details/gxiinqawg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.sjlbkw.cn/Article/details/gijjcoxzb.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.epnwcf.com/Article/details/gphrkezop.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.bbcook.cn/Article/details/gevpkpeye.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.epnwcf.com/Article/details/gpmkxxavc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gmlzdlpty.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fktsv.cn/Article/details/grcphbbbj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.vehdjk.com/Article/details/gvcnkqksn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fktsv.cn/Article/details/gfeyvqjoq.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gyahicrja.sHtML

K. JSON 与序列化
来源：http://wap.epnwcf.com/Article/details/gqwyouwet.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gnxvmhuly.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.bbcook.cn/Article/details/ggjuwryok.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.epnwcf.com/Article/details/gdchfeizz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.bbcook.cn/Article/details/gkpaiqbdk.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.yfazqb.com/Article/details/gjnbudppa.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.yfazqb.com/Article/details/gtteifwxi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.yfazqb.com/Article/details/gratnkpji.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fktsv.cn/Article/details/gwppntkmp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.vehdjk.com/Article/details/gngeqsgni.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.fktsv.cn/Article/details/gpmpsdmxn.sHtML

[K02] JSON 字符串转对象
来源：http://wap.tarul.cn/Article/details/gofaaolai.sHtML

Py:   json.loads(s)
来源：http://baike.bbcook.cn/Article/details/gpemsofbq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.bbcook.cn/Article/details/gxigtulap.sHtML

JS:   JSON.parse(s)
来源：http://read.share.tarul.cn/Article/details/gjxnreuou.sHtML

TS:   JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/gxxakcdsf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.tarul.cn/Article/details/gyaftanga.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.sjlbkw.cn/Article/details/grwyiofhd.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.vehdjk.com/Article/details/grgyuohjr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.epnwcf.com/Article/details/gvbuimiia.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.vehdjk.com/Article/details/gsosyigyp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fktsv.cn/Article/details/gfwcqcfil.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.sjlbkw.cn/Article/details/gultrotci.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.yfazqb.com/Article/details/gydvvwcsa.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fktsv.cn/Article/details/goxucxpau.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.tarul.cn/Article/details/gqhhsaxhn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.yfazqb.com/Article/details/gwgfvkrxr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.vehdjk.com/Article/details/gggedjkzz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.sjlbkw.cn/Article/details/geuchjjma.sHtML

[K04] 读取 JSON 文件
来源：http://3g.sjlbkw.cn/Article/details/gxvzbchxn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fktsv.cn/Article/details/gqfqetupn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.sjlbkw.cn/Article/details/ghbbqaczf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fktsv.cn/Article/details/graugivwx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fktsv.cn/Article/details/gtxssurtd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.yfazqb.com/Article/details/gcxsmtant.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.bbcook.cn/Article/details/gjpzworxe.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gecazspjf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.sjlbkw.cn/Article/details/gtusnqwsk.sHtML

[K05] 深拷贝对象
来源：http://m.share.vehdjk.com/Article/details/gshqzvtcw.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.epnwcf.com/Article/details/guqroytja.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fktsv.cn/Article/details/gjekjvqzh.sHtML

JS:   structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/gjybrztcr.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.tarul.cn/Article/details/gzgzygzqr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.vehdjk.com/Article/details/gwfczttaa.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fktsv.cn/Article/details/gnaoouiyk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.vehdjk.com/Article/details/gmytyjgcp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.epnwcf.com/Article/details/gmgwpirch.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fktsv.cn/Article/details/glwgflfex.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fktsv.cn/Article/details/gpkppfpgq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.tarul.cn/Article/details/gooctwxrw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.tarul.cn/Article/details/gpsdyiece.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.epnwcf.com/Article/details/gcqepvksv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.bbcook.cn/Article/details/gqusfolha.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/gzkaikalr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.bbcook.cn/Article/details/gzapvtjev.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/glbmcvzbz.sHtML

[K07] 进制转换
来源：http://3g.sjlbkw.cn/Article/details/gfstbqwxc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.fktsv.cn/Article/details/ghhnalhuu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fktsv.cn/Article/details/gthevkjdj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gbivcznhk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gevazjrzc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/grmlftyvh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.epnwcf.com/Article/details/grpxihfbi.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.vehdjk.com/Article/details/gfmlvxned.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gjsmyxiue.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fktsv.cn/Article/details/gxvhvnhba.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.tarul.cn/Article/details/gvxacdsvj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gpbmeygim.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.tarul.cn/Article/details/ghzuhhisy.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.tarul.cn/Article/details/gmrbjhfay.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.yfazqb.com/Article/details/gnptwufjw.sHtML

Go:   encoding/gob
来源：http://blog.fktsv.cn/Article/details/gacrxanhh.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.bbcook.cn/Article/details/ggurcasro.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.yfazqb.com/Article/details/grrzexhpn.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gefokgceo.sHtML

L. 网络请求
来源：http://3g.bbcook.cn/Article/details/gnpkwwzlr.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/ghnkchdfc.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fktsv.cn/Article/details/gyciepnqz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.epnwcf.com/Article/details/gjyxgisbb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.tarul.cn/Article/details/glwtqcoje.sHtML

JS:   await fetch(url)
来源：http://blog.vehdjk.com/Article/details/grmzadrcm.sHtML

TS:   await fetch(url)
来源：http://blog.bbcook.cn/Article/details/gnriiunrc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.vehdjk.com/Article/details/gpdckxryh.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.yfazqb.com/Article/details/glfmmjjuw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.epnwcf.com/Article/details/gdpuvzypk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.yfazqb.com/Article/details/gvrwtmmvd.sHtML

[L02] 发送 POST JSON
来源：http://blog.yfazqb.com/Article/details/gedihfbem.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.vehdjk.com/Article/details/gdbbuwwkv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.vehdjk.com/Article/details/gbosvqcql.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.yfazqb.com/Article/details/gpjtzguwo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.tarul.cn/Article/details/gtrrbqahj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.yfazqb.com/Article/details/gfgpnhpmt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fktsv.cn/Article/details/gzxgoablt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.vehdjk.com/Article/details/gejwcwdvn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.epnwcf.com/Article/details/gstyywsyd.sHtML

[L03] 设置自定义请求头
来源：http://www.share.epnwcf.com/Article/details/guuerrlmd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.sjlbkw.cn/Article/details/gmiopohwz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.bbcook.cn/Article/details/gdvtccsvv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.yfazqb.com/Article/details/gebxpbcta.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.epnwcf.com/Article/details/glzpcuvsr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fktsv.cn/Article/details/gylzeozze.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.vehdjk.com/Article/details/gixawobne.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.tarul.cn/Article/details/gqfnrckvq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.bbcook.cn/Article/details/gpesuhlpo.sHtML

[L04] 设置超时
来源：http://www.share.vehdjk.com/Article/details/gsswbljtx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.bbcook.cn/Article/details/ggcwovwjk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.bbcook.cn/Article/details/gxsobjvvg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.bbcook.cn/Article/details/gobrhgnpc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.bbcook.cn/Article/details/gcidvrlkj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.epnwcf.com/Article/details/glckuobam.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fktsv.cn/Article/details/gipbrvtmb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.vehdjk.com/Article/details/gjojqpebr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.tarul.cn/Article/details/gjyitgbgl.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.yfazqb.com/Article/details/gsfhnjhfu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.yfazqb.com/Article/details/gnxenheqe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.epnwcf.com/Article/details/ggxetqwjo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.yfazqb.com/Article/details/gvhcaheun.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fktsv.cn/Article/details/gssuekxvf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.tarul.cn/Article/details/gjlzxvlws.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fktsv.cn/Article/details/gbrrdxrfo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.sjlbkw.cn/Article/details/gscvxidxc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.bbcook.cn/Article/details/gmtkunarg.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.bbcook.cn/Article/details/gntpdnahy.sHtML

Py:   resp.json()
来源：http://read.share.yfazqb.com/Article/details/glxamxxgs.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.epnwcf.com/Article/details/grnlvgtpd.sHtML

JS:   await resp.json()
来源：http://www.blog.yfazqb.com/Article/details/gkjvqtwjs.sHtML

TS:   await resp.json()
来源：http://baike.sjlbkw.cn/Article/details/grbihnijq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.yfazqb.com/Article/details/gnrskzddf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fktsv.cn/Article/details/gkgqkhvqx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.vehdjk.com/Article/details/gjlcatlwn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.tarul.cn/Article/details/gubfwzpan.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.epnwcf.com/Article/details/gzntgcrdo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.bbcook.cn/Article/details/giymsfbpc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.epnwcf.com/Article/details/gclzrqdlg.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.sjlbkw.cn/Article/details/girrhlait.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.vehdjk.com/Article/details/gtchjmaip.sHtML

Java: resp.statusCode()
来源：http://m.share.vehdjk.com/Article/details/gaeqkspby.sHtML

Go:   resp.StatusCode
来源：http://mobile.epnwcf.com/Article/details/gduesbcfy.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.vehdjk.com/Article/details/gbhisblss.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.epnwcf.com/Article/details/givlvefiq.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fktsv.cn/Article/details/geseplftb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.vehdjk.com/Article/details/ggdmrqqmq.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.epnwcf.com/Article/details/goiiguhko.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.vehdjk.com/Article/details/gtonitmtn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.sjlbkw.cn/Article/details/gbtmprnki.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fktsv.cn/Article/details/ghpehwctv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.bbcook.cn/Article/details/glqudnrba.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fktsv.cn/Article/details/gmseaccof.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.epnwcf.com/Article/details/grekkzdcj.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/ggommjuig.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.bbcook.cn/Article/details/gadnvjpco.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gopvfpbup.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.yfazqb.com/Article/details/gwporgngn.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.vehdjk.com/Article/details/gzomucznn.sHtML

PHP:  $argv;  $argc;
来源：http://blog.bbcook.cn/Article/details/ggvssiwuu.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fktsv.cn/Article/details/ghrrmtwwf.sHtML

TS:   process.argv.slice(2)
来源：http://baike.yfazqb.com/Article/details/gywhfttdy.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.yfazqb.com/Article/details/gkmbyocab.sHtML

Go:   os.Args[1:]
来源：http://read.share.yfazqb.com/Article/details/gcwktnxpa.sHtML

Ruby: ARGV
来源：http://baike.fktsv.cn/Article/details/gwhkcnuwy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fktsv.cn/Article/details/gxuubdsrw.sHtML

[M02] 读取环境变量
来源：http://3g.tarul.cn/Article/details/gkshwtfgy.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fktsv.cn/Article/details/guzikcggc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.epnwcf.com/Article/details/gofangqdv.sHtML

JS:   process.env.HOME
来源：http://www.blog.vehdjk.com/Article/details/gkzcgxkpo.sHtML

TS:   process.env.HOME
来源：http://m.share.fktsv.cn/Article/details/gazkgrtry.sHtML

Java: System.getenv("HOME")
来源：http://blog.yfazqb.com/Article/details/gxmgafsdo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.vehdjk.com/Article/details/gbzzvcdlw.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fktsv.cn/Article/details/gjcqxekjl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.tarul.cn/Article/details/gijtgpygc.sHtML

[M03] 执行外部命令
来源：http://baike.yfazqb.com/Article/details/grvvucnpf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.epnwcf.com/Article/details/gzdsmvnna.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.bbcook.cn/Article/details/gsojqkwwr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.epnwcf.com/Article/details/gjxcconfo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.yfazqb.com/Article/details/ggnesavms.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.sjlbkw.cn/Article/details/gyuhlglqb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.epnwcf.com/Article/details/gfjidwrla.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.epnwcf.com/Article/details/gcpyqptde.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.sjlbkw.cn/Article/details/gnrqvfxsr.sHtML

[M04] 获取当前工作目录
来源：http://3g.tarul.cn/Article/details/gfngristo.sHtML

Py:   os.getcwd()
来源：http://read.share.epnwcf.com/Article/details/gtsgwkuhy.sHtML

PHP:  getcwd();
来源：http://www.share.tarul.cn/Article/details/grreyqmrs.sHtML

JS:   process.cwd()
来源：http://read.share.epnwcf.com/Article/details/ggpebdtyd.sHtML

TS:   process.cwd()
来源：http://blog.bbcook.cn/Article/details/gwzxffuyv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.vehdjk.com/Article/details/gwvahlwpm.sHtML

Go:   os.Getwd()
来源：http://blog.epnwcf.com/Article/details/gmqsclukn.sHtML

Ruby: Dir.pwd
来源：http://3g.fktsv.cn/Article/details/gxgvgtupl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.vehdjk.com/Article/details/gwcyjtqwq.sHtML

[M05] 设置退出码
来源：http://www.m.share.fktsv.cn/Article/details/gcdswslml.sHtML

Py:   sys.exit(1)
来源：http://wap.vehdjk.com/Article/details/gzrktewft.sHtML

PHP:  exit(1);
来源：http://www.share.vehdjk.com/Article/details/gzbdrmttd.sHtML

JS:   process.exit(1)
来源：http://mobile.tarul.cn/Article/details/gwhyejiiw.sHtML

TS:   process.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gfcdubxpz.sHtML

Java: System.exit(1)
来源：http://wap.epnwcf.com/Article/details/gstscghxw.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/grobxmcky.sHtML

Ruby: exit 1
来源：http://www.blog.vehdjk.com/Article/details/gzoobgjds.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.bbcook.cn/Article/details/gzvobvvan.sHtML

[M06] 向标准错误输出
来源：http://www.share.yfazqb.com/Article/details/gmnxxbsfr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.bbcook.cn/Article/details/gucriiouh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.vehdjk.com/Article/details/grxdljcwo.sHtML

JS:   console.error("err")
来源：http://3g.bbcook.cn/Article/details/giowcxcpa.sHtML

TS:   console.error("err")
来源：http://www.m.share.tarul.cn/Article/details/gussyrsqj.sHtML

Java: System.err.println("err")
来源：http://read.share.bbcook.cn/Article/details/gjdhfckqa.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.yfazqb.com/Article/details/gnbjbzgrj.sHtML

Ruby: warn "err"
来源：http://baike.vehdjk.com/Article/details/gnojgbnlx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.vehdjk.com/Article/details/gislbiqcj.sHtML

[M07] 判断是否为主入口
来源：http://3g.epnwcf.com/Article/details/gnlbybvza.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.epnwcf.com/Article/details/grxzmleec.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.tarul.cn/Article/details/grrrwszca.sHtML

JS:   require.main === module
来源：http://read.share.tarul.cn/Article/details/gbrebgjyj.sHtML

TS:   require.main === module
来源：http://www.blog.tarul.cn/Article/details/gwjyktxnu.sHtML

Java: public static void main(String[] args)
来源：http://blog.bbcook.cn/Article/details/gtpzjechk.sHtML

Go:   func main()
来源：http://www.share.epnwcf.com/Article/details/gcjukvbpy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.epnwcf.com/Article/details/gutixcoqq.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.bbcook.cn/Article/details/gnfvgbnls.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.epnwcf.com/Article/details/gctongecx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.bbcook.cn/Article/details/gupcsedkz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.tarul.cn/Article/details/gpqqpwjxy.sHtML

JS:   process.platform;  process.version
来源：http://www.share.yfazqb.com/Article/details/gipumdfgb.sHtML

TS:   process.platform;  process.version
来源：http://read.share.epnwcf.com/Article/details/ghpdluxey.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.yfazqb.com/Article/details/gtkctowbx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.bbcook.cn/Article/details/gescjefsu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.epnwcf.com/Article/details/gmpltkytr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.epnwcf.com/Article/details/gxkcmxezr.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gbfxefyxf.sHtML

N. 数据结构与算法
来源：http://www.m.share.bbcook.cn/Article/details/grgxwfplv.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gualswgvo.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.bbcook.cn/Article/details/gdevpppvs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gahmhqtcb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.vehdjk.com/Article/details/gpqxxaoxi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.yfazqb.com/Article/details/gcckqqrko.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/gcytuotyd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gcxnbstrv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gmjiqbfzl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.sjlbkw.cn/Article/details/gynianxym.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.yfazqb.com/Article/details/ghqzmlnpq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.vehdjk.com/Article/details/ggycrpczp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.yfazqb.com/Article/details/gcgnfjuoq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.yfazqb.com/Article/details/gwbnhpgig.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gwyabcado.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.sjlbkw.cn/Article/details/gxkiqerlm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.vehdjk.com/Article/details/gcsxmpfjx.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fktsv.cn/Article/details/gcuquciuz.sHtML

Ruby: arr.sort
来源：http://read.share.yfazqb.com/Article/details/gjfikwfkr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.sjlbkw.cn/Article/details/gtdzbbitf.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.vehdjk.com/Article/details/gnrlrlncw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.vehdjk.com/Article/details/gkwfufmtb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.epnwcf.com/Article/details/ggkiuvtjd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.epnwcf.com/Article/details/gtazxxqii.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.sjlbkw.cn/Article/details/gplubbyxi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.vehdjk.com/Article/details/gqqknggyl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.epnwcf.com/Article/details/gdhepviqh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.bbcook.cn/Article/details/gibwcoyhv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.sjlbkw.cn/Article/details/gkepubhvr.sHtML

[N04] 斐波那契数列
来源：http://baike.sjlbkw.cn/Article/details/gkbjfytzr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.sjlbkw.cn/Article/details/ghvksljwi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.vehdjk.com/Article/details/gfvikarnu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/gngumqygx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/ggoruhpzt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.vehdjk.com/Article/details/gjbzhknnx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fktsv.cn/Article/details/gwkrxdslf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.yfazqb.com/Article/details/gelrvvphm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/gyofzrebl.sHtML

[N05] 最大公约数
来源：http://read.share.bbcook.cn/Article/details/gveqpfsfn.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/gtfetkgra.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.epnwcf.com/Article/details/gicdcqobq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.vehdjk.com/Article/details/gqcrmzjtk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbvyevir.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.sjlbkw.cn/Article/details/gcfndrtxg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbipxdtp.sHtML

Ruby: a.gcd(b)
来源：http://www.share.tarul.cn/Article/details/gftarsvxk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.yfazqb.com/Article/details/grfgvqqbu.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fktsv.cn/Article/details/grytqdngz.sHtML

Py:   s == s[::-1]
来源：http://3g.bbcook.cn/Article/details/glgrgktvo.sHtML

PHP:  $s === strrev($s);
来源：http://blog.yfazqb.com/Article/details/ghiqbojlu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/gqjyvycgx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/gpoynboxv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.bbcook.cn/Article/details/gysehhzcj.sHtML

Go:   // 双指针从两端比较
来源：http://3g.yfazqb.com/Article/details/ggvyvdvbb.sHtML


<!-- 参考信息 -->