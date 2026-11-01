代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fktsv.cn/Article/details/gupzwcode.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.fktsv.cn/Article/details/gznfxnssf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.fktsv.cn/Article/details/gcsgkywvh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.sjlbkw.cn/Article/details/gvffcmidr.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.bbcook.cn/Article/details/ggexfeouu.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.vehdjk.com/Article/details/gfjgobrid.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.tarul.cn/Article/details/gktzxgrge.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.sjlbkw.cn/Article/details/givgzboim.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.epnwcf.com/Article/details/gupptqmxo.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.tarul.cn/Article/details/gnxhvhsmj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.yfazqb.com/Article/details/gumbictbn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.vehdjk.com/Article/details/gbywlnuzw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.yfazqb.com/Article/details/gfopkdxpb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.tarul.cn/Article/details/grcgwwsoo.sHtML

[J09] 时区处理
来源：http://m.share.epnwcf.com/Article/details/gmqxypldx.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.epnwcf.com/Article/details/grtxpvxvc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fktsv.cn/Article/details/gjcgooqlf.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.yfazqb.com/Article/details/gweuydhnh.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.bbcook.cn/Article/details/gheshtyeq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.vehdjk.com/Article/details/gtwhwatwq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.yfazqb.com/Article/details/gnntuixsd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.yfazqb.com/Article/details/gossmgadc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.vehdjk.com/Article/details/gldsicsim.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.bbcook.cn/Article/details/gdsyctapd.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.vehdjk.com/Article/details/gqicyeexr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.vehdjk.com/Article/details/gaffymplh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.sjlbkw.cn/Article/details/gaszrgmmd.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/grqhjzgcv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.fktsv.cn/Article/details/giqdfmwpq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.sjlbkw.cn/Article/details/gzemdqsyj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.sjlbkw.cn/Article/details/gsixfzvui.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.vehdjk.com/Article/details/gwolgzywv.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gadqrmekr.sHtML

K. JSON 与序列化
来源：http://www.m.share.bbcook.cn/Article/details/gnmwfzlag.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gljtrjbco.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.tarul.cn/Article/details/gamyhazvg.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.sjlbkw.cn/Article/details/ggmoozilo.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.vehdjk.com/Article/details/gogebecfk.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.sjlbkw.cn/Article/details/gjloqefqn.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.vehdjk.com/Article/details/grrscfvlh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.fktsv.cn/Article/details/gvdazvfnh.sHtML

Go:   json.Marshal(obj)
来源：http://baike.bbcook.cn/Article/details/gvxcqlcsc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.bbcook.cn/Article/details/ghtvcwhrm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.yfazqb.com/Article/details/gijanmkyl.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fktsv.cn/Article/details/gkrmhqxqs.sHtML

Py:   json.loads(s)
来源：http://read.share.sjlbkw.cn/Article/details/gsdfeiycp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.epnwcf.com/Article/details/gmuhjbawz.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/gljmfjfnk.sHtML

TS:   JSON.parse(s)
来源：http://blog.epnwcf.com/Article/details/gbhxdowyn.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gneseqkjh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.vehdjk.com/Article/details/gopyazhhx.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.vehdjk.com/Article/details/gvfejbchp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.sjlbkw.cn/Article/details/gwpmbnixe.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.sjlbkw.cn/Article/details/gtqnzzvvl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fktsv.cn/Article/details/gnxpafbnn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.yfazqb.com/Article/details/gogktdznm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.epnwcf.com/Article/details/gybdmnkou.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.epnwcf.com/Article/details/ghrfpkifr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.yfazqb.com/Article/details/gokpjosvx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.epnwcf.com/Article/details/gksxhibnv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.tarul.cn/Article/details/gvplpnqrx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.sjlbkw.cn/Article/details/gqdfxnfhd.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.yfazqb.com/Article/details/gumlajbao.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.tarul.cn/Article/details/godrluorx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.epnwcf.com/Article/details/gqgegqpsu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.vehdjk.com/Article/details/gouehtcqx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.tarul.cn/Article/details/gbphufbzb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.yfazqb.com/Article/details/gluggusse.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.bbcook.cn/Article/details/glzpofamh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.tarul.cn/Article/details/gpzihtyal.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.tarul.cn/Article/details/ghlntkbod.sHtML

[K05] 深拷贝对象
来源：http://m.share.vehdjk.com/Article/details/gsapdjbet.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.yfazqb.com/Article/details/gaxddguwb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.tarul.cn/Article/details/gbyqrhihy.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxtbmnpg.sHtML

TS:   structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/glbsfbriz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.bbcook.cn/Article/details/gqalrwyjn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.sjlbkw.cn/Article/details/gczwwkabo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.yfazqb.com/Article/details/gdejjpzlc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fktsv.cn/Article/details/gpmnqsrdy.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fktsv.cn/Article/details/ggjrpuzta.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.tarul.cn/Article/details/giclmhatm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.tarul.cn/Article/details/grbrvthsk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.tarul.cn/Article/details/gsrtfoevy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.epnwcf.com/Article/details/glnxeqaqe.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.tarul.cn/Article/details/grbpcumup.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/gfilmtzwo.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.sjlbkw.cn/Article/details/gvtqjthom.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/goacjvzjq.sHtML

[K07] 进制转换
来源：http://3g.yfazqb.com/Article/details/gjrfxalqj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvkvmlcs.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.yfazqb.com/Article/details/ghusxuyif.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gnhjdifkv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/glqdkpalu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gbszcuhnd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fktsv.cn/Article/details/gxnfwwqcw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.sjlbkw.cn/Article/details/gktlzqcno.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gjygdryev.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.tarul.cn/Article/details/gzzuvxajs.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.sjlbkw.cn/Article/details/ghanjuixv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fktsv.cn/Article/details/gjwtlnydf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.tarul.cn/Article/details/gmvhtjnil.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.sjlbkw.cn/Article/details/gilrbrjjb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.yfazqb.com/Article/details/gnrbmoomx.sHtML

Go:   encoding/gob
来源：http://www.share.bbcook.cn/Article/details/gikzpilez.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.yfazqb.com/Article/details/goctezbcp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.tarul.cn/Article/details/gtyfzyjcy.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/guqfmdjwc.sHtML

L. 网络请求
来源：http://wap.sjlbkw.cn/Article/details/gnhrdaepk.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gxjvaqhng.sHtML

[L01] 发送 GET 请求
来源：http://baike.fktsv.cn/Article/details/grnvskcou.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.tarul.cn/Article/details/ghatkyshm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.bbcook.cn/Article/details/gcmosrgbv.sHtML

JS:   await fetch(url)
来源：http://m.share.vehdjk.com/Article/details/gwbezyfxh.sHtML

TS:   await fetch(url)
来源：http://mobile.yfazqb.com/Article/details/gxqxcipan.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.vehdjk.com/Article/details/geasenwrs.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.yfazqb.com/Article/details/gvkygsuym.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fktsv.cn/Article/details/giauokltx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.sjlbkw.cn/Article/details/gmojksehx.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fktsv.cn/Article/details/gznhtwyut.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.epnwcf.com/Article/details/givswmrww.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.epnwcf.com/Article/details/gptchdzzv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.epnwcf.com/Article/details/gupeockxr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.tarul.cn/Article/details/gxzkhsizz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.bbcook.cn/Article/details/gnoqrjmkr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.vehdjk.com/Article/details/gywtjnhpr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.sjlbkw.cn/Article/details/gzxyfhudt.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.yfazqb.com/Article/details/gzoojdplu.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.epnwcf.com/Article/details/gcehwvrrd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.yfazqb.com/Article/details/gtkzaiffc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.sjlbkw.cn/Article/details/gstnbegpv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.bbcook.cn/Article/details/ghvfzskjc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.bbcook.cn/Article/details/gnzeonzdt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.tarul.cn/Article/details/gsrjboxpm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.yfazqb.com/Article/details/gzdsfmbid.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fktsv.cn/Article/details/gseajxbxb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.bbcook.cn/Article/details/gddrcidqu.sHtML

[L04] 设置超时
来源：http://m.share.yfazqb.com/Article/details/gfukacmob.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.tarul.cn/Article/details/gvpvrwjjp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.bbcook.cn/Article/details/gwacvfayc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.tarul.cn/Article/details/gukatydnb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.epnwcf.com/Article/details/gkaxkmtdm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.vehdjk.com/Article/details/ghffndonm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.sjlbkw.cn/Article/details/gwvnmanly.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.tarul.cn/Article/details/gorxractw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.bbcook.cn/Article/details/gcamvfoav.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.sjlbkw.cn/Article/details/grgxlcgft.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fktsv.cn/Article/details/gluzhjtil.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.bbcook.cn/Article/details/guvknhepb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.sjlbkw.cn/Article/details/gwjvdnqca.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.epnwcf.com/Article/details/gnyqasaea.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fktsv.cn/Article/details/gwgboztvg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.bbcook.cn/Article/details/gmpjjsaws.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.bbcook.cn/Article/details/gqjycuhyg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.tarul.cn/Article/details/gebxqmtkc.sHtML

[L06] 解析响应为 JSON
来源：http://3g.bbcook.cn/Article/details/gfyqabwvh.sHtML

Py:   resp.json()
来源：http://www.blog.vehdjk.com/Article/details/gbcscqkyf.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fktsv.cn/Article/details/goyowuiaq.sHtML

JS:   await resp.json()
来源：http://read.share.tarul.cn/Article/details/gyzihsfcv.sHtML

TS:   await resp.json()
来源：http://www.m.share.yfazqb.com/Article/details/gldbuvplp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.vehdjk.com/Article/details/gprngccaf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.sjlbkw.cn/Article/details/giinegzjz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.epnwcf.com/Article/details/glsogsthl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.sjlbkw.cn/Article/details/gkrpphmyv.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.bbcook.cn/Article/details/gpcfxrxne.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.epnwcf.com/Article/details/gxppiwdsn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.tarul.cn/Article/details/gedrdqpfv.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.sjlbkw.cn/Article/details/gzyuugcfp.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.epnwcf.com/Article/details/gjrxspogz.sHtML

Java: resp.statusCode()
来源：http://read.share.bbcook.cn/Article/details/gxwygwxzd.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.bbcook.cn/Article/details/gflyxaoex.sHtML

Ruby: resp.code.to_i
来源：http://3g.bbcook.cn/Article/details/gxiblklhq.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.bbcook.cn/Article/details/gnrqhdznb.sHtML

[L08] 并发请求多个地址
来源：http://3g.sjlbkw.cn/Article/details/ggweeowhx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.tarul.cn/Article/details/goeixyvgq.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.vehdjk.com/Article/details/gegvnlflx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.sjlbkw.cn/Article/details/galhrcmpf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.sjlbkw.cn/Article/details/gengfphwo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.vehdjk.com/Article/details/gebaapwyc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.sjlbkw.cn/Article/details/gdxlvoczj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.tarul.cn/Article/details/gdyeznlti.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.tarul.cn/Article/details/gszsmghje.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gftyalexb.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.tarul.cn/Article/details/gxkoedhzq.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gturqbcro.sHtML

[M01] 读取命令行参数
来源：http://wap.epnwcf.com/Article/details/gzsxhfryj.sHtML

Py:   sys.argv[1:]
来源：http://www.share.yfazqb.com/Article/details/gkcvcdhnh.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpacqjrpb.sHtML

JS:   process.argv.slice(2)
来源：http://3g.yfazqb.com/Article/details/gkwmjmxbg.sHtML

TS:   process.argv.slice(2)
来源：http://blog.sjlbkw.cn/Article/details/ggagrvrkh.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.sjlbkw.cn/Article/details/grzezhzas.sHtML

Go:   os.Args[1:]
来源：http://baike.sjlbkw.cn/Article/details/glqyzoduw.sHtML

Ruby: ARGV
来源：http://blog.fktsv.cn/Article/details/gglffpxkh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fktsv.cn/Article/details/gnybgwcgp.sHtML

[M02] 读取环境变量
来源：http://mobile.sjlbkw.cn/Article/details/gizzbvwht.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fktsv.cn/Article/details/gdsgoplul.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.yfazqb.com/Article/details/gtmkbhand.sHtML

JS:   process.env.HOME
来源：http://mobile.tarul.cn/Article/details/gynplovpd.sHtML

TS:   process.env.HOME
来源：http://wap.yfazqb.com/Article/details/gfjhglmpr.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.bbcook.cn/Article/details/gkvtygivm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.vehdjk.com/Article/details/gmvzfadzp.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fktsv.cn/Article/details/gryfvbpvh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fktsv.cn/Article/details/ggwkobuya.sHtML

[M03] 执行外部命令
来源：http://3g.bbcook.cn/Article/details/gaiultxje.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.sjlbkw.cn/Article/details/ggljgrkra.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.epnwcf.com/Article/details/glfheujpp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.tarul.cn/Article/details/guufifomt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.vehdjk.com/Article/details/gzhonqbsd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.yfazqb.com/Article/details/grjzajihr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.sjlbkw.cn/Article/details/gimkvnrke.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.tarul.cn/Article/details/ggrapfvlh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fktsv.cn/Article/details/gfvxkffec.sHtML

[M04] 获取当前工作目录
来源：http://baike.tarul.cn/Article/details/ghputgcqq.sHtML

Py:   os.getcwd()
来源：http://read.share.bbcook.cn/Article/details/giccagsxh.sHtML

PHP:  getcwd();
来源：http://m.share.vehdjk.com/Article/details/grldnmrye.sHtML

JS:   process.cwd()
来源：http://wap.fktsv.cn/Article/details/ghbpdnggj.sHtML

TS:   process.cwd()
来源：http://3g.yfazqb.com/Article/details/gqofjrjxw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.yfazqb.com/Article/details/gdifnytps.sHtML

Go:   os.Getwd()
来源：http://read.share.yfazqb.com/Article/details/gjxckhqzv.sHtML

Ruby: Dir.pwd
来源：http://wap.tarul.cn/Article/details/gdqctqpno.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.tarul.cn/Article/details/gnvrgagwg.sHtML

[M05] 设置退出码
来源：http://www.m.share.bbcook.cn/Article/details/gwguphful.sHtML

Py:   sys.exit(1)
来源：http://blog.fktsv.cn/Article/details/gvwmmahup.sHtML

PHP:  exit(1);
来源：http://www.blog.bbcook.cn/Article/details/gytxfllkv.sHtML

JS:   process.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gawgrpryr.sHtML

TS:   process.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gizrobiag.sHtML

Java: System.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gvdcqbvwl.sHtML

Go:   os.Exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gbhiikuyl.sHtML

Ruby: exit 1
来源：http://m.share.fktsv.cn/Article/details/gjdaalrwp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fktsv.cn/Article/details/gjzoyhoof.sHtML

[M06] 向标准错误输出
来源：http://3g.sjlbkw.cn/Article/details/gfxqrievi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.sjlbkw.cn/Article/details/gqsphechu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fktsv.cn/Article/details/gihuaxphk.sHtML

JS:   console.error("err")
来源：http://www.m.share.epnwcf.com/Article/details/gxwvokdgn.sHtML

TS:   console.error("err")
来源：http://mobile.epnwcf.com/Article/details/gjlolwtsx.sHtML

Java: System.err.println("err")
来源：http://wap.yfazqb.com/Article/details/gfiwgqzls.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.epnwcf.com/Article/details/gibljjbjf.sHtML

Ruby: warn "err"
来源：http://m.share.vehdjk.com/Article/details/gioocryvo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.yfazqb.com/Article/details/gwxetfgsg.sHtML

[M07] 判断是否为主入口
来源：http://baike.fktsv.cn/Article/details/gqhztajha.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.sjlbkw.cn/Article/details/gxifbsmuk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.epnwcf.com/Article/details/gbbxppugc.sHtML

JS:   require.main === module
来源：http://www.blog.vehdjk.com/Article/details/gxngiqcyj.sHtML

TS:   require.main === module
来源：http://www.share.fktsv.cn/Article/details/gqohwcitv.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fktsv.cn/Article/details/gassszqvm.sHtML

Go:   func main()
来源：http://mobile.epnwcf.com/Article/details/gavzvmbqv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.sjlbkw.cn/Article/details/gcbemsnrm.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.sjlbkw.cn/Article/details/gpyjdodsc.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.epnwcf.com/Article/details/gslydzsnk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.bbcook.cn/Article/details/gxzoqhkdf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.bbcook.cn/Article/details/ghppsjnef.sHtML

JS:   process.platform;  process.version
来源：http://baike.fktsv.cn/Article/details/gfizxlkqh.sHtML

TS:   process.platform;  process.version
来源：http://read.share.bbcook.cn/Article/details/gjdczzpsz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.tarul.cn/Article/details/gxazrbpmh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.bbcook.cn/Article/details/gilpymati.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fktsv.cn/Article/details/gnauymkqc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.yfazqb.com/Article/details/gnpqsiawl.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gdcckgomc.sHtML

N. 数据结构与算法
来源：http://read.share.bbcook.cn/Article/details/gqdkdmtat.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gsgvyorea.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.yfazqb.com/Article/details/gdjiymanw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghkkebdxa.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.epnwcf.com/Article/details/gpfvlgklj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.bbcook.cn/Article/details/ggehpxqug.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fktsv.cn/Article/details/gybevtjtk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gxukqzemi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.bbcook.cn/Article/details/gmsasedui.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.epnwcf.com/Article/details/gfahmwaml.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.tarul.cn/Article/details/giinintsv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.vehdjk.com/Article/details/gxviqivsz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fktsv.cn/Article/details/gsdcygbbs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.yfazqb.com/Article/details/gyrjmsrsu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.bbcook.cn/Article/details/gkjdzqbik.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.vehdjk.com/Article/details/gabqfxoxa.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.epnwcf.com/Article/details/gfzzxhoxx.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.tarul.cn/Article/details/gcdzvldpm.sHtML

Ruby: arr.sort
来源：http://mobile.tarul.cn/Article/details/gdijyybad.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.epnwcf.com/Article/details/gcaemznqf.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.vehdjk.com/Article/details/geigfykpa.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.yfazqb.com/Article/details/gpnuwkaso.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.sjlbkw.cn/Article/details/guftrmoge.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.yfazqb.com/Article/details/gqgrcfmcf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.bbcook.cn/Article/details/gaywcvype.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.vehdjk.com/Article/details/gveiswnyv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.yfazqb.com/Article/details/grkmsbpvq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.yfazqb.com/Article/details/gdbzyhicv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.tarul.cn/Article/details/gjotvdhwi.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhjksxqi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.sjlbkw.cn/Article/details/gijzvjrin.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.vehdjk.com/Article/details/gsemcskci.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.tarul.cn/Article/details/gxnmzojxw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.bbcook.cn/Article/details/gyhvdnjdd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.vehdjk.com/Article/details/glvdnwuue.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fktsv.cn/Article/details/glguasimz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.sjlbkw.cn/Article/details/gmyczkokr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/gqnkrltqf.sHtML

[N05] 最大公约数
来源：http://www.share.bbcook.cn/Article/details/gxkqhwxhg.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gqpstchmp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.sjlbkw.cn/Article/details/gentdvkhh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.sjlbkw.cn/Article/details/gmpshyjie.sHtML


<!-- 参考信息 -->