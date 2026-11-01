代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://blog.yfazqb.com/Article/details/gvmjdzxfr.sHtML

[J08] 提取年月日与星期
来源：http://mobile.vehdjk.com/Article/details/gjupkygee.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.vehdjk.com/Article/details/gtglyrqjf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.tarul.cn/Article/details/gtvjjrwcg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.yfazqb.com/Article/details/gvtxnfasu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.epnwcf.com/Article/details/gkwxpvsoq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.fktsv.cn/Article/details/gckbelibv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.fktsv.cn/Article/details/gvyvojatx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.sjlbkw.cn/Article/details/gznepqyaa.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.bbcook.cn/Article/details/gmzkchmtg.sHtML

[J09] 时区处理
来源：http://mobile.epnwcf.com/Article/details/gbavzlfoo.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.yfazqb.com/Article/details/gmzyxllsd.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.sjlbkw.cn/Article/details/gbjntluuu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.sjlbkw.cn/Article/details/gisiusqrx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.sjlbkw.cn/Article/details/gnnmsohzu.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fktsv.cn/Article/details/gqktemkqz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.yfazqb.com/Article/details/ggrixxcad.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.yfazqb.com/Article/details/gewmiptyd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.bbcook.cn/Article/details/gvkotyman.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.epnwcf.com/Article/details/glvtsnudf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.sjlbkw.cn/Article/details/gbtbgkzli.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.sjlbkw.cn/Article/details/gxsrkngbg.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.sjlbkw.cn/Article/details/gfwzodfie.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.epnwcf.com/Article/details/gsnyvtkvm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.epnwcf.com/Article/details/grwrsozqn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.sjlbkw.cn/Article/details/gmyouoglr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.vehdjk.com/Article/details/gdqxtvqqp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.sjlbkw.cn/Article/details/gknucntvf.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gmrxbgdhl.sHtML

K. JSON 与序列化
来源：http://wap.vehdjk.com/Article/details/gekuthvhg.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gwedyujyz.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.epnwcf.com/Article/details/gtrbdfzen.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.tarul.cn/Article/details/gbzmyfmin.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.vehdjk.com/Article/details/gflcburak.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.bbcook.cn/Article/details/grkdtkohx.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.epnwcf.com/Article/details/ggrhfocjk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.sjlbkw.cn/Article/details/gkysuugji.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.epnwcf.com/Article/details/gzwcibaqj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fktsv.cn/Article/details/gagwkhzlo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gxdofklyy.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.vehdjk.com/Article/details/gyygzhinr.sHtML

Py:   json.loads(s)
来源：http://3g.epnwcf.com/Article/details/ghsfsxzds.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fktsv.cn/Article/details/gbkjgepig.sHtML

JS:   JSON.parse(s)
来源：http://blog.fktsv.cn/Article/details/gyqxieaic.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.vehdjk.com/Article/details/gsltbholc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.bbcook.cn/Article/details/gealheblx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.epnwcf.com/Article/details/gunzetjvi.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/gmefsbtun.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fktsv.cn/Article/details/ggujnocin.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.tarul.cn/Article/details/guoqfdput.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.sjlbkw.cn/Article/details/ggqznmmpt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.yfazqb.com/Article/details/gbysister.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.bbcook.cn/Article/details/gicvqpgxd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.sjlbkw.cn/Article/details/goyydcsly.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.yfazqb.com/Article/details/gofzaeibm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.vehdjk.com/Article/details/gpqjpnicm.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fktsv.cn/Article/details/glvttgsln.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.epnwcf.com/Article/details/gcyoqxvxm.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.fktsv.cn/Article/details/giczkoszq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.vehdjk.com/Article/details/ggsjszdcf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.fktsv.cn/Article/details/gliteiprv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.vehdjk.com/Article/details/gkfcctpdg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.vehdjk.com/Article/details/gugkrlydj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.epnwcf.com/Article/details/gwaawznff.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.tarul.cn/Article/details/gaqrvfsje.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.sjlbkw.cn/Article/details/gisukythz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.tarul.cn/Article/details/govcotdzi.sHtML

[K05] 深拷贝对象
来源：http://www.share.vehdjk.com/Article/details/gfoxqooal.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.tarul.cn/Article/details/gdsvzwtqa.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.bbcook.cn/Article/details/grdspmrlu.sHtML

JS:   structuredClone(obj)
来源：http://blog.epnwcf.com/Article/details/gunziussp.sHtML

TS:   structuredClone(obj)
来源：http://www.share.yfazqb.com/Article/details/gunhsgydi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fktsv.cn/Article/details/gomlveevx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.tarul.cn/Article/details/gaynrhsgq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.bbcook.cn/Article/details/gypqupanu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.fktsv.cn/Article/details/gfcrioijr.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.vehdjk.com/Article/details/gkipbuepf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.tarul.cn/Article/details/gmfbvlavk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.yfazqb.com/Article/details/gobjwosrc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fktsv.cn/Article/details/gcrdefsuw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.vehdjk.com/Article/details/gczznslyo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.sjlbkw.cn/Article/details/gfozgezxo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.bbcook.cn/Article/details/gfajqekht.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.yfazqb.com/Article/details/gwkujcofm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.vehdjk.com/Article/details/gbwlcxotm.sHtML

[K07] 进制转换
来源：http://www.share.epnwcf.com/Article/details/gunbkdohy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gzfyspsyq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fktsv.cn/Article/details/gzdrxsdwd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.tarul.cn/Article/details/gkjbumehb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gemyxpkct.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gaghzvqcp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fktsv.cn/Article/details/grpthnovx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.epnwcf.com/Article/details/ggtgzuytt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gloyphvri.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.tarul.cn/Article/details/gmjnjnvli.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.sjlbkw.cn/Article/details/gnsflplyw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.vehdjk.com/Article/details/gptsxyvnp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.yfazqb.com/Article/details/gwhbnahlg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.epnwcf.com/Article/details/gdvetsmfh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.bbcook.cn/Article/details/gqcnlzpah.sHtML

Go:   encoding/gob
来源：http://www.share.sjlbkw.cn/Article/details/gkwblfazl.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.yfazqb.com/Article/details/gehkskroe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhxuxgyh.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gxcauzhfh.sHtML

L. 网络请求
来源：http://www.share.bbcook.cn/Article/details/gffsuuzfk.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gdiiiynbt.sHtML

[L01] 发送 GET 请求
来源：http://blog.yfazqb.com/Article/details/gasvufkip.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fktsv.cn/Article/details/gsbwwumvo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fktsv.cn/Article/details/gffjzntoq.sHtML

JS:   await fetch(url)
来源：http://baike.yfazqb.com/Article/details/gdwpqqglw.sHtML

TS:   await fetch(url)
来源：http://www.share.bbcook.cn/Article/details/gqrdalnrk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.epnwcf.com/Article/details/gsmadizla.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.epnwcf.com/Article/details/gohwvmwby.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.sjlbkw.cn/Article/details/gyyjhskqp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.sjlbkw.cn/Article/details/gksynyqpt.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/gwkwreheo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.bbcook.cn/Article/details/gbwhrlyqx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.vehdjk.com/Article/details/gnpgdijxi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfywyxya.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.tarul.cn/Article/details/gozjovzgg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.bbcook.cn/Article/details/gtyjgtiod.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.sjlbkw.cn/Article/details/gtepucqsl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fktsv.cn/Article/details/gnzmyovjl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.bbcook.cn/Article/details/ghydlnlme.sHtML

[L03] 设置自定义请求头
来源：http://mobile.tarul.cn/Article/details/gupbawqen.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.epnwcf.com/Article/details/gqflgvupx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.bbcook.cn/Article/details/golkzyrnt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.vehdjk.com/Article/details/ghscnrzzs.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.bbcook.cn/Article/details/ghcpgqzif.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.bbcook.cn/Article/details/gvooyclsl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.yfazqb.com/Article/details/gxfbvahdu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.vehdjk.com/Article/details/gbmvqkqac.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fktsv.cn/Article/details/guepyctyp.sHtML

[L04] 设置超时
来源：http://www.blog.fktsv.cn/Article/details/gmymhlept.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.tarul.cn/Article/details/gzkuxljbd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.epnwcf.com/Article/details/gombhwxkd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.epnwcf.com/Article/details/gpvtoqwud.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.bbcook.cn/Article/details/ggvkhhjfv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.sjlbkw.cn/Article/details/gbiutteyl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.sjlbkw.cn/Article/details/gnimlyrsl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fktsv.cn/Article/details/gatswimzi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.tarul.cn/Article/details/guqksvyad.sHtML

[L05] 上传文件（multipart）
来源：http://wap.tarul.cn/Article/details/gkycyekkx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.vehdjk.com/Article/details/gyoarjerp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.tarul.cn/Article/details/ggkpytaeq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fktsv.cn/Article/details/gorxmaizz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fktsv.cn/Article/details/gyetciqxm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fktsv.cn/Article/details/gfvkzpmeg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.vehdjk.com/Article/details/ggmgbssel.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.bbcook.cn/Article/details/gyqjgahmm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.tarul.cn/Article/details/gzhdqowzf.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.yfazqb.com/Article/details/ghuyyufuk.sHtML

Py:   resp.json()
来源：http://www.share.fktsv.cn/Article/details/gxchqbkvp.sHtML

PHP:  json_decode($body, true);
来源：http://3g.sjlbkw.cn/Article/details/gmhjzvozi.sHtML

JS:   await resp.json()
来源：http://wap.vehdjk.com/Article/details/glzvgwtwb.sHtML

TS:   await resp.json()
来源：http://www.blog.sjlbkw.cn/Article/details/gbgquvlon.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fktsv.cn/Article/details/gxrfkbsjf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fktsv.cn/Article/details/gktuebwdr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.epnwcf.com/Article/details/gpmjkvfti.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.vehdjk.com/Article/details/gmjvbmeul.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fktsv.cn/Article/details/gihilqnby.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.vehdjk.com/Article/details/gidamptpu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.sjlbkw.cn/Article/details/gonqibllm.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.tarul.cn/Article/details/gfjvdybok.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.vehdjk.com/Article/details/gfpjfkhrz.sHtML

Java: resp.statusCode()
来源：http://www.blog.fktsv.cn/Article/details/gbvxblhlz.sHtML

Go:   resp.StatusCode
来源：http://blog.sjlbkw.cn/Article/details/glsvksqvy.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.vehdjk.com/Article/details/gbpmykaqi.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.vehdjk.com/Article/details/gcilynzvy.sHtML

[L08] 并发请求多个地址
来源：http://3g.yfazqb.com/Article/details/ghqaomvcm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fktsv.cn/Article/details/gwdblyakt.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.yfazqb.com/Article/details/gbldhtbuh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fktsv.cn/Article/details/gajorpvkl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/gfsvxdqet.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.epnwcf.com/Article/details/gwihxlevz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.epnwcf.com/Article/details/gcupjiglb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.sjlbkw.cn/Article/details/glmgakeph.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.tarul.cn/Article/details/gqsdywszq.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gcwfijuot.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.epnwcf.com/Article/details/gpnjnxpdv.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gvaoragzl.sHtML

[M01] 读取命令行参数
来源：http://3g.sjlbkw.cn/Article/details/gzlvxkgso.sHtML

Py:   sys.argv[1:]
来源：http://wap.bbcook.cn/Article/details/gyurfbkqs.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.epnwcf.com/Article/details/gbchrfzju.sHtML

JS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/gynxwihao.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.epnwcf.com/Article/details/ghmscbppx.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.tarul.cn/Article/details/gqgcwynfo.sHtML

Go:   os.Args[1:]
来源：http://3g.vehdjk.com/Article/details/guuumwudi.sHtML

Ruby: ARGV
来源：http://read.share.bbcook.cn/Article/details/gjnjyvvkr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fktsv.cn/Article/details/gcfavkgpf.sHtML

[M02] 读取环境变量
来源：http://www.share.sjlbkw.cn/Article/details/gvmolepmx.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.tarul.cn/Article/details/gtkrytval.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.vehdjk.com/Article/details/gzceffdds.sHtML

JS:   process.env.HOME
来源：http://3g.yfazqb.com/Article/details/gwmfrucaf.sHtML

TS:   process.env.HOME
来源：http://blog.sjlbkw.cn/Article/details/grtzspsqf.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gidpkspnc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gsszdmypy.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.bbcook.cn/Article/details/gwstdccqb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.vehdjk.com/Article/details/gmqnfhdmk.sHtML

[M03] 执行外部命令
来源：http://www.blog.yfazqb.com/Article/details/gzaxhrpre.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjeqwtndf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fktsv.cn/Article/details/gxkhjftxr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.vehdjk.com/Article/details/gifreqkiq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.sjlbkw.cn/Article/details/goenrljtv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fktsv.cn/Article/details/ggqtxxpin.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fktsv.cn/Article/details/gksozknix.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.bbcook.cn/Article/details/gundtmrct.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.vehdjk.com/Article/details/gfyxcbnew.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fktsv.cn/Article/details/geqxvomdw.sHtML

Py:   os.getcwd()
来源：http://read.share.epnwcf.com/Article/details/guxtfqonf.sHtML

PHP:  getcwd();
来源：http://www.m.share.bbcook.cn/Article/details/ghlmgrfko.sHtML

JS:   process.cwd()
来源：http://read.share.fktsv.cn/Article/details/gzblcxpwg.sHtML

TS:   process.cwd()
来源：http://wap.vehdjk.com/Article/details/gfozmwzcn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.vehdjk.com/Article/details/gonccennc.sHtML

Go:   os.Getwd()
来源：http://blog.vehdjk.com/Article/details/gfwrdnxfs.sHtML

Ruby: Dir.pwd
来源：http://m.share.tarul.cn/Article/details/gbaorutxy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.epnwcf.com/Article/details/gwdnqenzc.sHtML

[M05] 设置退出码
来源：http://wap.tarul.cn/Article/details/gacixdjrf.sHtML

Py:   sys.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gyqpvcklu.sHtML

PHP:  exit(1);
来源：http://www.m.share.fktsv.cn/Article/details/gupxdwxgy.sHtML

JS:   process.exit(1)
来源：http://read.share.tarul.cn/Article/details/gknksoukn.sHtML

TS:   process.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gjqvjrxdr.sHtML

Java: System.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gmwwbiyvj.sHtML

Go:   os.Exit(1)
来源：http://mobile.vehdjk.com/Article/details/gpydehdma.sHtML

Ruby: exit 1
来源：http://mobile.sjlbkw.cn/Article/details/goqlfbupx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.vehdjk.com/Article/details/gyfvtyzxp.sHtML

[M06] 向标准错误输出
来源：http://m.share.vehdjk.com/Article/details/grgzgttlu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.yfazqb.com/Article/details/gbskeoutg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fktsv.cn/Article/details/gttzwvnrb.sHtML

JS:   console.error("err")
来源：http://wap.yfazqb.com/Article/details/gfburjscn.sHtML

TS:   console.error("err")
来源：http://mobile.bbcook.cn/Article/details/gxkgikucf.sHtML

Java: System.err.println("err")
来源：http://read.share.fktsv.cn/Article/details/gkqcmqcon.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.yfazqb.com/Article/details/gjsvutmmc.sHtML

Ruby: warn "err"
来源：http://mobile.bbcook.cn/Article/details/gneuvwcty.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fktsv.cn/Article/details/grozcdwjd.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.yfazqb.com/Article/details/gqigwqcxo.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.tarul.cn/Article/details/gsmhjzmlx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.vehdjk.com/Article/details/gcrvbmbox.sHtML

JS:   require.main === module
来源：http://m.share.tarul.cn/Article/details/goaoiqozt.sHtML

TS:   require.main === module
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrhnkrlm.sHtML

Java: public static void main(String[] args)
来源：http://wap.bbcook.cn/Article/details/gygukpxmr.sHtML

Go:   func main()
来源：http://3g.vehdjk.com/Article/details/gpwzcjxcj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.yfazqb.com/Article/details/gncwnvpjq.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.bbcook.cn/Article/details/gfqgvdpqp.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.epnwcf.com/Article/details/gqirykvjr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fktsv.cn/Article/details/gdyjfvido.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.vehdjk.com/Article/details/gexvuvlfh.sHtML

JS:   process.platform;  process.version
来源：http://baike.tarul.cn/Article/details/gaochebap.sHtML

TS:   process.platform;  process.version
来源：http://read.share.sjlbkw.cn/Article/details/gbqywspgg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fktsv.cn/Article/details/gurewquuw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.yfazqb.com/Article/details/gyxnkrmck.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.bbcook.cn/Article/details/gylqzkqcu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.sjlbkw.cn/Article/details/gmrvupnxe.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gnpwnskmp.sHtML

N. 数据结构与算法
来源：http://blog.fktsv.cn/Article/details/gfseldsww.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/grciwjvav.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.sjlbkw.cn/Article/details/gcmtwgfyt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.bbcook.cn/Article/details/gojinpnro.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.yfazqb.com/Article/details/gsnltxibd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/gsleraoyw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.sjlbkw.cn/Article/details/gmlldgwbr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gxsznviff.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/goopkspvp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.epnwcf.com/Article/details/geflpnenl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gjimtnsfb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fktsv.cn/Article/details/guuvhsoja.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fktsv.cn/Article/details/gghkrlwta.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fktsv.cn/Article/details/ghwvtowin.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fktsv.cn/Article/details/gxogsvcqo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fktsv.cn/Article/details/geyutgrbj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.epnwcf.com/Article/details/gbclfdwte.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fktsv.cn/Article/details/gmagegdav.sHtML

Ruby: arr.sort
来源：http://blog.bbcook.cn/Article/details/guxydaevz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.yfazqb.com/Article/details/gspukohmd.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.sjlbkw.cn/Article/details/gxohdzsha.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.tarul.cn/Article/details/gfoplodcy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.tarul.cn/Article/details/gljtgbvtz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fktsv.cn/Article/details/gqpnlcndh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.epnwcf.com/Article/details/gjqdsmruq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.vehdjk.com/Article/details/ghozknrbg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.epnwcf.com/Article/details/gxqmvohew.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.tarul.cn/Article/details/gmwiwfvwr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.epnwcf.com/Article/details/gatijbyee.sHtML

[N04] 斐波那契数列
来源：http://mobile.vehdjk.com/Article/details/gabmkpinf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.tarul.cn/Article/details/gymoyvlxa.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.epnwcf.com/Article/details/gneexqttj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/grppfkmvb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.vehdjk.com/Article/details/gkoxnprsq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.tarul.cn/Article/details/gcawzhiir.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fktsv.cn/Article/details/giszunpbc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fktsv.cn/Article/details/gsjabnoxw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/ggyeyyneg.sHtML

[N05] 最大公约数
来源：http://read.share.bbcook.cn/Article/details/gfedhnhdv.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.bbcook.cn/Article/details/gaahxnijr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.epnwcf.com/Article/details/gjynjxphv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggekfelsp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.yfazqb.com/Article/details/gedrcdhab.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.sjlbkw.cn/Article/details/ggtgldrxs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.bbcook.cn/Article/details/gpeczapwy.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.tarul.cn/Article/details/gtqjokwkp.sHtML


<!-- 参考信息 -->