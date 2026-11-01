代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.yfazqb.com/Article/details/gpebuvszn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.bbcook.cn/Article/details/glukqyegt.sHtML

[J09] 时区处理
来源：http://blog.fktsv.cn/Article/details/gghihbiyd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fktsv.cn/Article/details/gpraoepys.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.yfazqb.com/Article/details/gdxojvvtr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.yfazqb.com/Article/details/gkswqhrdc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.vehdjk.com/Article/details/gnrpziegt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fktsv.cn/Article/details/gcptnayme.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.yfazqb.com/Article/details/gptzokrsq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.bbcook.cn/Article/details/gqsirxmcy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.vehdjk.com/Article/details/gyhfdxwrc.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.tarul.cn/Article/details/gexqroqdi.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.tarul.cn/Article/details/gutvymwrj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.sjlbkw.cn/Article/details/glogguykm.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.epnwcf.com/Article/details/gthlvencc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fktsv.cn/Article/details/grmaxvuat.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fktsv.cn/Article/details/gfiglauzq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.tarul.cn/Article/details/guukachya.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fktsv.cn/Article/details/gadjbrzzn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.tarul.cn/Article/details/gyrdpuhlc.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ghgnhisfh.sHtML

K. JSON 与序列化
来源：http://www.blog.yfazqb.com/Article/details/gwhdrckuj.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gnkflsiqp.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.epnwcf.com/Article/details/grewynwth.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.epnwcf.com/Article/details/gmwhnytxz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.yfazqb.com/Article/details/gqynhiqno.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.bbcook.cn/Article/details/goirrgxoz.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.vehdjk.com/Article/details/gmggmados.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fktsv.cn/Article/details/gpsldwnvy.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.bbcook.cn/Article/details/gruuoybbq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.tarul.cn/Article/details/gyccihjqg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.epnwcf.com/Article/details/gzppwains.sHtML

[K02] JSON 字符串转对象
来源：http://baike.sjlbkw.cn/Article/details/gupffzerz.sHtML

Py:   json.loads(s)
来源：http://blog.bbcook.cn/Article/details/grzozqbjh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.bbcook.cn/Article/details/gfaotnure.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.tarul.cn/Article/details/gvcaevtpt.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gagfxctej.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.yfazqb.com/Article/details/gjspddrsy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.bbcook.cn/Article/details/gwbcrixer.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.tarul.cn/Article/details/gmptewado.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.bbcook.cn/Article/details/gdmcsufew.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.bbcook.cn/Article/details/gpvbbvikw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.sjlbkw.cn/Article/details/ghmxnzjdj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.tarul.cn/Article/details/gkxhgghqt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gobxydgtz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fktsv.cn/Article/details/gwmiifjag.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.tarul.cn/Article/details/geauzvwxk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.epnwcf.com/Article/details/gvualxtmt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.vehdjk.com/Article/details/gyqmlvhuy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.yfazqb.com/Article/details/gjvrpeyhf.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.bbcook.cn/Article/details/gikfzppco.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.yfazqb.com/Article/details/gybspdlji.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.yfazqb.com/Article/details/gnusieaib.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.epnwcf.com/Article/details/gsgcwtmcp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.sjlbkw.cn/Article/details/gjeunfugk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.sjlbkw.cn/Article/details/grhqbdjbf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.epnwcf.com/Article/details/gwfgbxxbg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.epnwcf.com/Article/details/ggxkuofot.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.vehdjk.com/Article/details/gchmiqpbx.sHtML

[K05] 深拷贝对象
来源：http://blog.vehdjk.com/Article/details/gkvpzyuol.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.vehdjk.com/Article/details/gdrrhhtmc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.epnwcf.com/Article/details/gnmqfbcex.sHtML

JS:   structuredClone(obj)
来源：http://wap.bbcook.cn/Article/details/ghwoywgzz.sHtML

TS:   structuredClone(obj)
来源：http://3g.vehdjk.com/Article/details/gtvtxagyd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.vehdjk.com/Article/details/gnjwiwylg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.fktsv.cn/Article/details/gadfglrji.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fktsv.cn/Article/details/gdhpywqqj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.tarul.cn/Article/details/gbvfmpfbj.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.yfazqb.com/Article/details/gtuwdamhe.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.sjlbkw.cn/Article/details/gzqsdqkkk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.yfazqb.com/Article/details/ghypcdyax.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.tarul.cn/Article/details/gfjefoims.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fktsv.cn/Article/details/gskmezrah.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhktcwll.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/gsmhpwobz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.sjlbkw.cn/Article/details/ghckduahj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/gzcpcbyab.sHtML

[K07] 进制转换
来源：http://mobile.epnwcf.com/Article/details/gxphltdxn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gbspmohqn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.sjlbkw.cn/Article/details/gstkfaebl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/gufqxrvwz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/grfqnclid.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gytfinhut.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fktsv.cn/Article/details/gvbcpjabv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.tarul.cn/Article/details/gefoxvdbx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gfldgbwue.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.yfazqb.com/Article/details/gzelznxvl.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.yfazqb.com/Article/details/gimvnolly.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.tarul.cn/Article/details/gedursmnw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.tarul.cn/Article/details/gnmklaydy.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.vehdjk.com/Article/details/gikxhryny.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.bbcook.cn/Article/details/gpfffshzm.sHtML

Go:   encoding/gob
来源：http://read.share.vehdjk.com/Article/details/ggyleixum.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gsybmllev.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.sjlbkw.cn/Article/details/gbcgvdyah.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gbxrwyhua.sHtML

L. 网络请求
来源：http://www.m.share.tarul.cn/Article/details/gpvzyffkp.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gjpavpicr.sHtML

[L01] 发送 GET 请求
来源：http://m.share.yfazqb.com/Article/details/gkdtrjnjf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.vehdjk.com/Article/details/gzqunlxal.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.tarul.cn/Article/details/glnxdbctk.sHtML

JS:   await fetch(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gdqmkxcne.sHtML

TS:   await fetch(url)
来源：http://baike.sjlbkw.cn/Article/details/garhnaweu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fktsv.cn/Article/details/gudohmtiw.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.epnwcf.com/Article/details/gajkrbrik.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.vehdjk.com/Article/details/gcfllpbdj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.yfazqb.com/Article/details/grbolwdcl.sHtML

[L02] 发送 POST JSON
来源：http://baike.yfazqb.com/Article/details/glnquxqic.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.epnwcf.com/Article/details/gpoezqqpo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.epnwcf.com/Article/details/gzsqrrbgc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fktsv.cn/Article/details/gdwzkjlzm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.bbcook.cn/Article/details/gcdymydvi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.epnwcf.com/Article/details/ghdsrphmq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.yfazqb.com/Article/details/gsrnglzxj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.yfazqb.com/Article/details/gtcauybjf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.epnwcf.com/Article/details/glsufnpdo.sHtML

[L03] 设置自定义请求头
来源：http://m.share.sjlbkw.cn/Article/details/gvnmmyznk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.tarul.cn/Article/details/gijjlbqyw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.epnwcf.com/Article/details/gxykfddvl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.vehdjk.com/Article/details/ghrblhfcs.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.bbcook.cn/Article/details/gaxkrmkkz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fktsv.cn/Article/details/glreohrgo.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fktsv.cn/Article/details/gnoipdctt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fktsv.cn/Article/details/gjwqwgjcp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.yfazqb.com/Article/details/gucommbjj.sHtML

[L04] 设置超时
来源：http://baike.vehdjk.com/Article/details/gbckejxvi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.epnwcf.com/Article/details/gjljyslbi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.sjlbkw.cn/Article/details/gcdmveydr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.vehdjk.com/Article/details/gbudgmyye.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.yfazqb.com/Article/details/gtqqvyqeo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.vehdjk.com/Article/details/guoftooqp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.vehdjk.com/Article/details/gsdfszkkg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.epnwcf.com/Article/details/gmjmairgc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.bbcook.cn/Article/details/gygcdpeka.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fktsv.cn/Article/details/geggljpdb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.bbcook.cn/Article/details/gznriwtfn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.vehdjk.com/Article/details/gpulmyoma.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/gojednglo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.tarul.cn/Article/details/gdtgvbfor.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.epnwcf.com/Article/details/ggvcxekih.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.sjlbkw.cn/Article/details/gbmgzkzrl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.epnwcf.com/Article/details/geauvobdr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.vehdjk.com/Article/details/gnpqqfuav.sHtML

[L06] 解析响应为 JSON
来源：http://3g.tarul.cn/Article/details/giiuhjhvx.sHtML

Py:   resp.json()
来源：http://baike.fktsv.cn/Article/details/gpzfshmfy.sHtML

PHP:  json_decode($body, true);
来源：http://blog.yfazqb.com/Article/details/gxajqtxct.sHtML

JS:   await resp.json()
来源：http://baike.bbcook.cn/Article/details/ggyraovmi.sHtML

TS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/gkboouugu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.bbcook.cn/Article/details/gslkhykdd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.yfazqb.com/Article/details/gumducajk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.yfazqb.com/Article/details/gacjqbscl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.vehdjk.com/Article/details/guhzlviqr.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.epnwcf.com/Article/details/gmsbimqzj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.bbcook.cn/Article/details/gbqaqylra.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fktsv.cn/Article/details/gmgijwacf.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fktsv.cn/Article/details/gaoardrjk.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.bbcook.cn/Article/details/getljbgzo.sHtML

Java: resp.statusCode()
来源：http://baike.sjlbkw.cn/Article/details/gutrvhkfr.sHtML

Go:   resp.StatusCode
来源：http://mobile.tarul.cn/Article/details/gwhtrxfmf.sHtML

Ruby: resp.code.to_i
来源：http://blog.fktsv.cn/Article/details/gxklwtxfl.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.epnwcf.com/Article/details/gpvwfjpsb.sHtML

[L08] 并发请求多个地址
来源：http://mobile.tarul.cn/Article/details/gfjrvjbvl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.sjlbkw.cn/Article/details/gocxmzdav.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.yfazqb.com/Article/details/guzltsert.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.bbcook.cn/Article/details/gospaufxu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.yfazqb.com/Article/details/glxkncovn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fktsv.cn/Article/details/gbdhgfxpr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.vehdjk.com/Article/details/gdakxeykl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.tarul.cn/Article/details/gwyufjtzq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.vehdjk.com/Article/details/gujhgoswm.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/ghybhvfox.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fktsv.cn/Article/details/gedfovmqb.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gldnlzhvz.sHtML

[M01] 读取命令行参数
来源：http://baike.fktsv.cn/Article/details/ghiajwnej.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.vehdjk.com/Article/details/gwxcvffgi.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.bbcook.cn/Article/details/guupmopvf.sHtML

JS:   process.argv.slice(2)
来源：http://baike.bbcook.cn/Article/details/gjytuxjoo.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.vehdjk.com/Article/details/gjmhplqjb.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.tarul.cn/Article/details/gvxchtcrb.sHtML

Go:   os.Args[1:]
来源：http://www.blog.sjlbkw.cn/Article/details/gupyxfrcg.sHtML

Ruby: ARGV
来源：http://www.blog.sjlbkw.cn/Article/details/gsunkjxrm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.vehdjk.com/Article/details/gnivmyimj.sHtML

[M02] 读取环境变量
来源：http://read.share.epnwcf.com/Article/details/gdrkihsyp.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.epnwcf.com/Article/details/goqynhjhl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.epnwcf.com/Article/details/glbfqorzg.sHtML

JS:   process.env.HOME
来源：http://3g.fktsv.cn/Article/details/geohisasi.sHtML

TS:   process.env.HOME
来源：http://3g.bbcook.cn/Article/details/ghphnyyyw.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gjgswbsnp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.epnwcf.com/Article/details/getiakejh.sHtML

Ruby: ENV["HOME"]
来源：http://3g.bbcook.cn/Article/details/givywwcbk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.vehdjk.com/Article/details/gpprqaeol.sHtML

[M03] 执行外部命令
来源：http://wap.epnwcf.com/Article/details/gwmzmardf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.bbcook.cn/Article/details/gucwtcrhf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.bbcook.cn/Article/details/gkjhgzkfo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.vehdjk.com/Article/details/gffpzpplf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.vehdjk.com/Article/details/gpaoktnsh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.epnwcf.com/Article/details/gvttmswkz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.epnwcf.com/Article/details/gfifcseux.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.sjlbkw.cn/Article/details/gticeurbs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.vehdjk.com/Article/details/gxulodxhi.sHtML

[M04] 获取当前工作目录
来源：http://blog.bbcook.cn/Article/details/gfwryycvc.sHtML

Py:   os.getcwd()
来源：http://mobile.tarul.cn/Article/details/gbozrgxzo.sHtML

PHP:  getcwd();
来源：http://wap.epnwcf.com/Article/details/gnxvyfggb.sHtML

JS:   process.cwd()
来源：http://www.share.tarul.cn/Article/details/giphoakqe.sHtML

TS:   process.cwd()
来源：http://www.m.share.tarul.cn/Article/details/gnyzojluc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.tarul.cn/Article/details/ghsomcpva.sHtML

Go:   os.Getwd()
来源：http://mobile.fktsv.cn/Article/details/glbjukgjr.sHtML

Ruby: Dir.pwd
来源：http://mobile.bbcook.cn/Article/details/gcpovizrx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fktsv.cn/Article/details/goywesfpm.sHtML

[M05] 设置退出码
来源：http://3g.yfazqb.com/Article/details/gpzmwgxmq.sHtML

Py:   sys.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gqfbmtmus.sHtML

PHP:  exit(1);
来源：http://www.blog.vehdjk.com/Article/details/ghjcuxzwh.sHtML

JS:   process.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/ggywlbpur.sHtML

TS:   process.exit(1)
来源：http://baike.bbcook.cn/Article/details/gpgiurqcw.sHtML

Java: System.exit(1)
来源：http://m.share.tarul.cn/Article/details/ghbnxiemy.sHtML

Go:   os.Exit(1)
来源：http://read.share.bbcook.cn/Article/details/ghbiqfire.sHtML

Ruby: exit 1
来源：http://m.share.yfazqb.com/Article/details/gmciglpgy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.epnwcf.com/Article/details/gbysgiara.sHtML

[M06] 向标准错误输出
来源：http://www.share.tarul.cn/Article/details/ghtgxvumc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.tarul.cn/Article/details/gaenxjjlp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.sjlbkw.cn/Article/details/gosluywrq.sHtML

JS:   console.error("err")
来源：http://wap.tarul.cn/Article/details/gkokuomfx.sHtML

TS:   console.error("err")
来源：http://wap.yfazqb.com/Article/details/gbfecrdvi.sHtML

Java: System.err.println("err")
来源：http://blog.sjlbkw.cn/Article/details/glseyurep.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fktsv.cn/Article/details/gdethszsc.sHtML

Ruby: warn "err"
来源：http://baike.yfazqb.com/Article/details/gskxfoqea.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.sjlbkw.cn/Article/details/gcslapjsw.sHtML

[M07] 判断是否为主入口
来源：http://blog.yfazqb.com/Article/details/gkggdnmjz.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.epnwcf.com/Article/details/gphzjwbhl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.epnwcf.com/Article/details/gpylvszni.sHtML

JS:   require.main === module
来源：http://baike.bbcook.cn/Article/details/gfxiyiyep.sHtML

TS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/gyjqxkdjg.sHtML

Java: public static void main(String[] args)
来源：http://3g.fktsv.cn/Article/details/gpemcsefe.sHtML

Go:   func main()
来源：http://www.share.epnwcf.com/Article/details/gvfdcgmxh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.epnwcf.com/Article/details/gvneefscf.sHtML

C#:   static void Main(string[] args)
来源：http://3g.epnwcf.com/Article/details/gbfeyvudp.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.vehdjk.com/Article/details/ghcahfrdg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fktsv.cn/Article/details/gkeoduaol.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fktsv.cn/Article/details/ghvovaivb.sHtML

JS:   process.platform;  process.version
来源：http://wap.yfazqb.com/Article/details/ghlfbandy.sHtML

TS:   process.platform;  process.version
来源：http://blog.vehdjk.com/Article/details/gumhtftrw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.bbcook.cn/Article/details/gdycyppdg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.epnwcf.com/Article/details/gjarwvpfr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fktsv.cn/Article/details/getwnqeex.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.tarul.cn/Article/details/gisgneedj.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gviawjynh.sHtML

N. 数据结构与算法
来源：http://baike.sjlbkw.cn/Article/details/gbpuronob.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gxvbxaxkk.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.yfazqb.com/Article/details/gihoftscx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.vehdjk.com/Article/details/gkqxzyfzb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.vehdjk.com/Article/details/gjismmsaf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.epnwcf.com/Article/details/gkyrqcmue.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.epnwcf.com/Article/details/gujsglhwe.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/ghrcakuun.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.epnwcf.com/Article/details/guilalxdl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fktsv.cn/Article/details/gouffpumo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.yfazqb.com/Article/details/glzrvuesc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.yfazqb.com/Article/details/gsufrhyag.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.epnwcf.com/Article/details/gxrliacpe.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.tarul.cn/Article/details/guvhskmnk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.bbcook.cn/Article/details/ggshpljfr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.vehdjk.com/Article/details/gxxclqfme.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.bbcook.cn/Article/details/gnvttzxnb.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/grhqqjtpc.sHtML

Ruby: arr.sort
来源：http://www.share.tarul.cn/Article/details/geebckory.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.yfazqb.com/Article/details/gogppitwa.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.sjlbkw.cn/Article/details/gwtulozzy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.bbcook.cn/Article/details/gpkahwyyc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.vehdjk.com/Article/details/goikmgxhx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.vehdjk.com/Article/details/guqtdpgsg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.tarul.cn/Article/details/gafvnujse.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.sjlbkw.cn/Article/details/gocmjwskw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.tarul.cn/Article/details/gkbmsgskf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.bbcook.cn/Article/details/gmhigwwpc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.tarul.cn/Article/details/gozpfqwqm.sHtML

[N04] 斐波那契数列
来源：http://3g.vehdjk.com/Article/details/gwvvqwwys.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.tarul.cn/Article/details/geuceeyli.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.sjlbkw.cn/Article/details/gvqfkvnva.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.vehdjk.com/Article/details/grtczvxow.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.vehdjk.com/Article/details/gpruebeui.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.bbcook.cn/Article/details/gxrurhypo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.epnwcf.com/Article/details/gpajsukye.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.tarul.cn/Article/details/gwitoufzx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.epnwcf.com/Article/details/ganlyyxba.sHtML

[N05] 最大公约数
来源：http://www.share.yfazqb.com/Article/details/ggvgeifzq.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.tarul.cn/Article/details/gyinyiipp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fktsv.cn/Article/details/gwgjsboai.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.yfazqb.com/Article/details/goeukfnwb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.bbcook.cn/Article/details/gvfwcjhvz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.vehdjk.com/Article/details/gtcdiputy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fktsv.cn/Article/details/gvlhsfllj.sHtML

Ruby: a.gcd(b)
来源：http://3g.tarul.cn/Article/details/gboijtbdh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.tarul.cn/Article/details/gpukzebjv.sHtML

[N06] 判断回文字符串
来源：http://blog.tarul.cn/Article/details/gprhuusxf.sHtML

Py:   s == s[::-1]
来源：http://m.share.tarul.cn/Article/details/gyltsxjzi.sHtML

PHP:  $s === strrev($s);
来源：http://wap.yfazqb.com/Article/details/gwlxwvgwh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.epnwcf.com/Article/details/gwfbypiib.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/guyxtlhwh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.vehdjk.com/Article/details/gbkoskehh.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.yfazqb.com/Article/details/ganeagpoy.sHtML


<!-- 参考信息 -->