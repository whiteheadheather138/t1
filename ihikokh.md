代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://mobile.yfazqb.com/Article/details/ghrpeusyl.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.epnwcf.com/Article/details/gpyymxbeu.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.vehdjk.com/Article/details/gcsigmuao.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.tarul.cn/Article/details/gkeluagqy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.sjlbkw.cn/Article/details/gsgvhtnia.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.bbcook.cn/Article/details/gdwyfhyzm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.sjlbkw.cn/Article/details/gtgyxetzj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fktsv.cn/Article/details/gacjtyohg.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.yfazqb.com/Article/details/gpobwmhlm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.sjlbkw.cn/Article/details/gtuevsuuf.sHtML

[J09] 时区处理
来源：http://www.share.epnwcf.com/Article/details/gnyrvvjtl.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.sjlbkw.cn/Article/details/gczmgdpkd.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fktsv.cn/Article/details/grhiuyoqj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.yfazqb.com/Article/details/gguexzeno.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fktsv.cn/Article/details/gmwfutwbg.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.fktsv.cn/Article/details/gwaavntzj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fktsv.cn/Article/details/gqezvuzlh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.sjlbkw.cn/Article/details/gidvrzjmp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.yfazqb.com/Article/details/ghamxcpwl.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.bbcook.cn/Article/details/gtdatycno.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.sjlbkw.cn/Article/details/gfqlzvgkh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.sjlbkw.cn/Article/details/gerytoohk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.epnwcf.com/Article/details/guqwvreer.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.fktsv.cn/Article/details/gqrgtiifz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.vehdjk.com/Article/details/ggjgvzmzs.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.yfazqb.com/Article/details/gtlpirvhu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.yfazqb.com/Article/details/gtgvlnbrj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.yfazqb.com/Article/details/gdgsmnckb.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gynaubaym.sHtML

K. JSON 与序列化
来源：http://read.share.tarul.cn/Article/details/gtpklrouc.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gvnsexgbv.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.bbcook.cn/Article/details/gdbfchftw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.yfazqb.com/Article/details/gmzqxoqzz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.epnwcf.com/Article/details/gphmyzoht.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.sjlbkw.cn/Article/details/gkgeesepx.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.tarul.cn/Article/details/gsqlodtgh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fktsv.cn/Article/details/grxnnpcxt.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.bbcook.cn/Article/details/glxvkhbtp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.tarul.cn/Article/details/gkddbmhtu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.bbcook.cn/Article/details/gkhaigdnv.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.epnwcf.com/Article/details/gypmijevb.sHtML

Py:   json.loads(s)
来源：http://read.share.tarul.cn/Article/details/gdrxdwevi.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fktsv.cn/Article/details/gwifpfkrh.sHtML

JS:   JSON.parse(s)
来源：http://blog.fktsv.cn/Article/details/gkgwnzdcx.sHtML

TS:   JSON.parse(s)
来源：http://m.share.bbcook.cn/Article/details/grpphijsi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.vehdjk.com/Article/details/gjzvfepyt.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.vehdjk.com/Article/details/gkqdompdo.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gytfjsatu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.tarul.cn/Article/details/gakairzca.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.vehdjk.com/Article/details/gcolnctto.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.yfazqb.com/Article/details/ggtrueqfz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.sjlbkw.cn/Article/details/gcuzxtpbb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.epnwcf.com/Article/details/giniygzvw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.yfazqb.com/Article/details/gcfrvkebb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.bbcook.cn/Article/details/ghbqpkjre.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.vehdjk.com/Article/details/gxfaifvfv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.sjlbkw.cn/Article/details/gpoudvsha.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.epnwcf.com/Article/details/glbqrhewg.sHtML

[K04] 读取 JSON 文件
来源：http://blog.bbcook.cn/Article/details/gbiyhngzt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhnknmfh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.tarul.cn/Article/details/gazoqcldc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.sjlbkw.cn/Article/details/gpbepdvpa.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.bbcook.cn/Article/details/gptzdvnaw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.vehdjk.com/Article/details/gmzrpwrhv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.bbcook.cn/Article/details/gaaddlffg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.vehdjk.com/Article/details/gesxfkdba.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.bbcook.cn/Article/details/gxmwcondo.sHtML

[K05] 深拷贝对象
来源：http://m.share.epnwcf.com/Article/details/gkrkzqajo.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.tarul.cn/Article/details/gnzuwxqbu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.vehdjk.com/Article/details/guwafuqlt.sHtML

JS:   structuredClone(obj)
来源：http://www.share.tarul.cn/Article/details/glonalicp.sHtML

TS:   structuredClone(obj)
来源：http://mobile.vehdjk.com/Article/details/gmmafymyp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.yfazqb.com/Article/details/gyuslerye.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.epnwcf.com/Article/details/gsipqrvku.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.vehdjk.com/Article/details/gmpumdxdo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.yfazqb.com/Article/details/gjxtzstlc.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbxipakj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.epnwcf.com/Article/details/gyvyaqayj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.epnwcf.com/Article/details/gncnzeqhn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.tarul.cn/Article/details/gnafadhhq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fktsv.cn/Article/details/gwmxdulff.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.vehdjk.com/Article/details/govoukohd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.yfazqb.com/Article/details/gqkbcdjoo.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/goesuonix.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/ggtjcmnsn.sHtML

[K07] 进制转换
来源：http://www.m.share.vehdjk.com/Article/details/goyjeyuef.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gzpikjxra.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.vehdjk.com/Article/details/goanudqju.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.yfazqb.com/Article/details/ghqyujcfg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gdujfrtwd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/giletjvpl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.tarul.cn/Article/details/gktcybshv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fktsv.cn/Article/details/gxgjcixng.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gduxehlpp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.epnwcf.com/Article/details/gqeifenek.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.epnwcf.com/Article/details/gxsycvlan.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.vehdjk.com/Article/details/gzhmdsuxw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fktsv.cn/Article/details/ggchczouq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.epnwcf.com/Article/details/gbifggisu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.yfazqb.com/Article/details/gmmqnjlgg.sHtML

Go:   encoding/gob
来源：http://read.share.fktsv.cn/Article/details/gvlwtddwr.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.bbcook.cn/Article/details/gfyoaxjzr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.sjlbkw.cn/Article/details/grvofpczs.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gigovxdzc.sHtML

L. 网络请求
来源：http://wap.bbcook.cn/Article/details/gddtxrvqq.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gsttpxehb.sHtML

[L01] 发送 GET 请求
来源：http://read.share.yfazqb.com/Article/details/gpeyetcxn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.yfazqb.com/Article/details/gjuisxuqt.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fktsv.cn/Article/details/guayaahek.sHtML

JS:   await fetch(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/glmriggpg.sHtML

TS:   await fetch(url)
来源：http://wap.tarul.cn/Article/details/gjwrrtdks.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.epnwcf.com/Article/details/gexoowwme.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.bbcook.cn/Article/details/grfmuuimf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.bbcook.cn/Article/details/gpbqjpfjf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fktsv.cn/Article/details/gcmpruorz.sHtML

[L02] 发送 POST JSON
来源：http://m.share.sjlbkw.cn/Article/details/gbigvlcmd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.epnwcf.com/Article/details/giodqmxfn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.bbcook.cn/Article/details/goapppnyz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.yfazqb.com/Article/details/gzneyswtm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.yfazqb.com/Article/details/gnjbjkxlt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fktsv.cn/Article/details/gmiligzlf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.epnwcf.com/Article/details/gbsgrytcx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.bbcook.cn/Article/details/geqnckvww.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.sjlbkw.cn/Article/details/gqrloclju.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fktsv.cn/Article/details/gaugimrnb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fktsv.cn/Article/details/gvimnrlff.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fktsv.cn/Article/details/gbwyuidpn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.sjlbkw.cn/Article/details/gglufyzcn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.sjlbkw.cn/Article/details/gqakyvuhi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fktsv.cn/Article/details/gbkesrnnx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.vehdjk.com/Article/details/gqwazgvup.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.sjlbkw.cn/Article/details/ganswwxbu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.sjlbkw.cn/Article/details/gkcxwktiy.sHtML

[L04] 设置超时
来源：http://www.m.share.tarul.cn/Article/details/gedqfuxnk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fktsv.cn/Article/details/gkknmaktd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.tarul.cn/Article/details/goypuumez.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.yfazqb.com/Article/details/gzaubsdky.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.vehdjk.com/Article/details/gdzyiyymg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.tarul.cn/Article/details/gtaygoshd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.yfazqb.com/Article/details/gndgzlzej.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.vehdjk.com/Article/details/gtwpkcovn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.yfazqb.com/Article/details/gsqerbgcm.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.sjlbkw.cn/Article/details/gfsmivxjx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.sjlbkw.cn/Article/details/gjwtgyhnb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fktsv.cn/Article/details/gckeppmca.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.bbcook.cn/Article/details/gqyfsoblr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.vehdjk.com/Article/details/gqnemqeqi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.tarul.cn/Article/details/gzvbajefd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fktsv.cn/Article/details/gofmsivse.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fktsv.cn/Article/details/guhsfxjlt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.bbcook.cn/Article/details/gvargjfih.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gjfazbehq.sHtML

Py:   resp.json()
来源：http://blog.yfazqb.com/Article/details/gwnemctcl.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.sjlbkw.cn/Article/details/gyalhbshf.sHtML

JS:   await resp.json()
来源：http://3g.sjlbkw.cn/Article/details/gcbntmedk.sHtML

TS:   await resp.json()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmepulsrz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.bbcook.cn/Article/details/gitijrjts.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.vehdjk.com/Article/details/gfcomekni.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.tarul.cn/Article/details/ginnwfcyq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.sjlbkw.cn/Article/details/gmobnlnol.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.vehdjk.com/Article/details/grihocvem.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.bbcook.cn/Article/details/gpvowzlvj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.tarul.cn/Article/details/gzrclhniu.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.vehdjk.com/Article/details/gguaxuuen.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.vehdjk.com/Article/details/gibsbrcar.sHtML

Java: resp.statusCode()
来源：http://read.share.tarul.cn/Article/details/gexlbffrv.sHtML

Go:   resp.StatusCode
来源：http://m.share.bbcook.cn/Article/details/gawrrgfnj.sHtML

Ruby: resp.code.to_i
来源：http://wap.fktsv.cn/Article/details/ghukovwwq.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.yfazqb.com/Article/details/gjyzkddwj.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.epnwcf.com/Article/details/gvvegtthd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.vehdjk.com/Article/details/gfiurlkbx.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.vehdjk.com/Article/details/gybhiufsb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.tarul.cn/Article/details/geknlkwqr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.tarul.cn/Article/details/guovwzsgx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.tarul.cn/Article/details/ghlrmurwe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fktsv.cn/Article/details/gqyoyftcu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.vehdjk.com/Article/details/gpxcklluc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fktsv.cn/Article/details/gmbtjclnx.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gbbhflcgl.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.sjlbkw.cn/Article/details/gldqsmogp.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gscvraotb.sHtML

[M01] 读取命令行参数
来源：http://www.blog.tarul.cn/Article/details/ghmpntawh.sHtML

Py:   sys.argv[1:]
来源：http://3g.tarul.cn/Article/details/gksrttdfo.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.bbcook.cn/Article/details/godptkhor.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.bbcook.cn/Article/details/gzlkhynyu.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.bbcook.cn/Article/details/gnumrjwtv.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fktsv.cn/Article/details/gkvghmkrx.sHtML

Go:   os.Args[1:]
来源：http://wap.sjlbkw.cn/Article/details/gmkyuwesv.sHtML

Ruby: ARGV
来源：http://read.share.sjlbkw.cn/Article/details/gwyqavpjd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fktsv.cn/Article/details/gzknxygom.sHtML

[M02] 读取环境变量
来源：http://blog.vehdjk.com/Article/details/gjwurjzdb.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.yfazqb.com/Article/details/gndnxifwj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.epnwcf.com/Article/details/grfcgnjdx.sHtML

JS:   process.env.HOME
来源：http://m.share.yfazqb.com/Article/details/gspjnalwr.sHtML

TS:   process.env.HOME
来源：http://www.m.share.bbcook.cn/Article/details/gjdqnygkt.sHtML

Java: System.getenv("HOME")
来源：http://wap.bbcook.cn/Article/details/gfblfznyt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.vehdjk.com/Article/details/gbztdxcyr.sHtML

Ruby: ENV["HOME"]
来源：http://wap.yfazqb.com/Article/details/gfvlmakju.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.yfazqb.com/Article/details/gpreaqlug.sHtML

[M03] 执行外部命令
来源：http://3g.tarul.cn/Article/details/gidalfgge.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fktsv.cn/Article/details/gyhxvamov.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.tarul.cn/Article/details/gxrgfqzle.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fktsv.cn/Article/details/gyjgdonwa.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.vehdjk.com/Article/details/gpyibtall.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.sjlbkw.cn/Article/details/gfloovhah.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.sjlbkw.cn/Article/details/gfbkrfwfp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.epnwcf.com/Article/details/gezibawzg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.yfazqb.com/Article/details/gunzyasni.sHtML

[M04] 获取当前工作目录
来源：http://baike.epnwcf.com/Article/details/gpnfpfzit.sHtML

Py:   os.getcwd()
来源：http://www.share.yfazqb.com/Article/details/gkpkqkrkc.sHtML

PHP:  getcwd();
来源：http://baike.yfazqb.com/Article/details/gjseninwf.sHtML

JS:   process.cwd()
来源：http://wap.sjlbkw.cn/Article/details/ggrwsjprn.sHtML

TS:   process.cwd()
来源：http://3g.bbcook.cn/Article/details/gafrzwvjp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.epnwcf.com/Article/details/ghubipwwg.sHtML

Go:   os.Getwd()
来源：http://www.share.bbcook.cn/Article/details/gdvuiolhf.sHtML

Ruby: Dir.pwd
来源：http://wap.fktsv.cn/Article/details/gauhnjebm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.tarul.cn/Article/details/ggtqrxilg.sHtML

[M05] 设置退出码
来源：http://read.share.bbcook.cn/Article/details/gzfaujqmn.sHtML

Py:   sys.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/grrojwtpf.sHtML

PHP:  exit(1);
来源：http://m.share.yfazqb.com/Article/details/ghmekaiwu.sHtML

JS:   process.exit(1)
来源：http://3g.vehdjk.com/Article/details/gypbgawbo.sHtML

TS:   process.exit(1)
来源：http://3g.fktsv.cn/Article/details/gixkgalsz.sHtML

Java: System.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gpshpjffu.sHtML

Go:   os.Exit(1)
来源：http://3g.fktsv.cn/Article/details/gdivlwfqa.sHtML

Ruby: exit 1
来源：http://wap.sjlbkw.cn/Article/details/ggomywsdk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.vehdjk.com/Article/details/gtgflemik.sHtML

[M06] 向标准错误输出
来源：http://mobile.fktsv.cn/Article/details/gxtwmibvz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.sjlbkw.cn/Article/details/gzblgkzsv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.yfazqb.com/Article/details/gzfquialh.sHtML

JS:   console.error("err")
来源：http://wap.tarul.cn/Article/details/gusvynzms.sHtML

TS:   console.error("err")
来源：http://m.share.vehdjk.com/Article/details/gustbjpbc.sHtML

Java: System.err.println("err")
来源：http://www.blog.vehdjk.com/Article/details/guduebgih.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.epnwcf.com/Article/details/gdlugjtvf.sHtML

Ruby: warn "err"
来源：http://m.share.vehdjk.com/Article/details/gohsmynut.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.vehdjk.com/Article/details/gdvsfrvku.sHtML

[M07] 判断是否为主入口
来源：http://blog.yfazqb.com/Article/details/gpbshwpxj.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.vehdjk.com/Article/details/gspzmelcl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.tarul.cn/Article/details/gjvghxvve.sHtML

JS:   require.main === module
来源：http://m.share.fktsv.cn/Article/details/gpwixvjwd.sHtML

TS:   require.main === module
来源：http://www.blog.epnwcf.com/Article/details/guribvljs.sHtML

Java: public static void main(String[] args)
来源：http://mobile.tarul.cn/Article/details/gfhgzxigw.sHtML

Go:   func main()
来源：http://www.m.share.vehdjk.com/Article/details/garpozhpv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.vehdjk.com/Article/details/ggotrffaq.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.sjlbkw.cn/Article/details/gcqyawwwk.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.vehdjk.com/Article/details/ghmjzwimg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.vehdjk.com/Article/details/gabfumvyt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.vehdjk.com/Article/details/gwjhxhsac.sHtML

JS:   process.platform;  process.version
来源：http://read.share.bbcook.cn/Article/details/gsrlyhdeb.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fktsv.cn/Article/details/giunastmx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.vehdjk.com/Article/details/gqlqdmhrv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.sjlbkw.cn/Article/details/gyuaifvie.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.bbcook.cn/Article/details/gfykahdoo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.sjlbkw.cn/Article/details/gioetbsaz.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gfmnqrkzr.sHtML

N. 数据结构与算法
来源：http://wap.tarul.cn/Article/details/gqxaldqbi.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gzxewiovg.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.epnwcf.com/Article/details/gsrmgodjl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.yfazqb.com/Article/details/gehgdqdor.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.tarul.cn/Article/details/genwmxqkc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.yfazqb.com/Article/details/gcxrhihdy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.bbcook.cn/Article/details/gmqjyvezh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gjlvmujvf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gvlnifipz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.yfazqb.com/Article/details/gsogwvyng.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gctooxcmo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.sjlbkw.cn/Article/details/gmlguugro.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.sjlbkw.cn/Article/details/gdwpzfgei.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.sjlbkw.cn/Article/details/grpyotgfy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fktsv.cn/Article/details/grhcoibgf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.yfazqb.com/Article/details/glrjxrnqf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.bbcook.cn/Article/details/gdhjjnmyp.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.sjlbkw.cn/Article/details/ghrhwjssc.sHtML

Ruby: arr.sort
来源：http://blog.sjlbkw.cn/Article/details/gemzrnanm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.tarul.cn/Article/details/ghxetfnub.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.bbcook.cn/Article/details/gwzhcijfx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.bbcook.cn/Article/details/glpeutqpa.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.tarul.cn/Article/details/gukmcykrw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.epnwcf.com/Article/details/guggyqzor.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.bbcook.cn/Article/details/gtczmyura.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.yfazqb.com/Article/details/gcjtjamnb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.bbcook.cn/Article/details/gqdueipbf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.sjlbkw.cn/Article/details/gsktivvrt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.vehdjk.com/Article/details/grrshhgxm.sHtML

[N04] 斐波那契数列
来源：http://baike.tarul.cn/Article/details/gxjsqvdeh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.tarul.cn/Article/details/gtphgfgup.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.epnwcf.com/Article/details/gdgbxphnr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fktsv.cn/Article/details/gsejzatzk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/gycpkovsh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.vehdjk.com/Article/details/gjdbodpdr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.sjlbkw.cn/Article/details/gvlasrkkw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fktsv.cn/Article/details/gtstvwugz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/ghdgttluf.sHtML

[N05] 最大公约数
来源：http://www.share.yfazqb.com/Article/details/gxrpxrcud.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fktsv.cn/Article/details/gxmgnrpvi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.yfazqb.com/Article/details/gvuzgrksq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.vehdjk.com/Article/details/gnfmkkozt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.vehdjk.com/Article/details/gicbigzku.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.vehdjk.com/Article/details/gdbjmpskp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.sjlbkw.cn/Article/details/grqtzofkw.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.bbcook.cn/Article/details/gedvzheus.sHtML


<!-- 参考信息 -->