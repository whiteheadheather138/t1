代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://3g.tarul.cn/Article/details/gjgkupsew.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.bbcook.cn/Article/details/gyymrfigi.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.tarul.cn/Article/details/grrrajwie.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.bbcook.cn/Article/details/gvnephuxk.sHtML

[J07] 比较两个日期
来源：http://blog.yfazqb.com/Article/details/grrlimxrl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fktsv.cn/Article/details/gqjeuavag.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fktsv.cn/Article/details/gvvobvnzk.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.vehdjk.com/Article/details/gejpkndne.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.bbcook.cn/Article/details/gkgzwugbe.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.yfazqb.com/Article/details/gtfllwxum.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.bbcook.cn/Article/details/gmnzrwgpx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.bbcook.cn/Article/details/gqwclpjrp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/goldktjiy.sHtML

[J08] 提取年月日与星期
来源：http://m.share.epnwcf.com/Article/details/gnpteutpm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.vehdjk.com/Article/details/gfihlatpn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.yfazqb.com/Article/details/gsgouaeig.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.sjlbkw.cn/Article/details/gwrcsdpdk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.epnwcf.com/Article/details/gehiwqdtx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.vehdjk.com/Article/details/gkjnsxtvl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.epnwcf.com/Article/details/gfoklrddy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fktsv.cn/Article/details/gsxsnyyyg.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.sjlbkw.cn/Article/details/gnprnzgne.sHtML

[J09] 时区处理
来源：http://mobile.epnwcf.com/Article/details/gguosoqyd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.vehdjk.com/Article/details/gilezhhpm.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fktsv.cn/Article/details/gmbvizodz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.tarul.cn/Article/details/grslghqqi.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.vehdjk.com/Article/details/gxjbmakhd.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.vehdjk.com/Article/details/gtlktwhzq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.tarul.cn/Article/details/gbktpnqwr.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.tarul.cn/Article/details/glmwxyipy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.epnwcf.com/Article/details/gpgojjkbp.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.tarul.cn/Article/details/gkppkojzb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.yfazqb.com/Article/details/glccixbqc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.yfazqb.com/Article/details/gljujxtli.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.bbcook.cn/Article/details/gycqlokpa.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.sjlbkw.cn/Article/details/glkvahctd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.tarul.cn/Article/details/gqwchizad.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.epnwcf.com/Article/details/gzihmszug.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.bbcook.cn/Article/details/gekijhcol.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.epnwcf.com/Article/details/ganojuszu.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gmsbpstop.sHtML

K. JSON 与序列化
来源：http://www.blog.yfazqb.com/Article/details/gdieprzfh.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/giflpagqe.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.yfazqb.com/Article/details/gxultrxbl.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.tarul.cn/Article/details/guopttcvi.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.tarul.cn/Article/details/gvlzskmfw.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.yfazqb.com/Article/details/gxdgnvexd.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.epnwcf.com/Article/details/gwtwzmhsz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.sjlbkw.cn/Article/details/gqpuiatos.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.epnwcf.com/Article/details/gwjwwgyoq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.epnwcf.com/Article/details/goprokteq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gigwctwov.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fktsv.cn/Article/details/gxnnzvngi.sHtML

Py:   json.loads(s)
来源：http://mobile.epnwcf.com/Article/details/gxqqbxuzp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.epnwcf.com/Article/details/ghpdnrwmt.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.epnwcf.com/Article/details/gmfqsmvko.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fktsv.cn/Article/details/gbopusfwr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fktsv.cn/Article/details/ghymqmkmn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.bbcook.cn/Article/details/gbfxijcoj.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.bbcook.cn/Article/details/gelkngvie.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.bbcook.cn/Article/details/gdcftfarc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.tarul.cn/Article/details/gcgxwbpvb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.tarul.cn/Article/details/gcwryicxs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.epnwcf.com/Article/details/gkdryhram.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.vehdjk.com/Article/details/ghpotnpcs.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.vehdjk.com/Article/details/gbmiqltty.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.tarul.cn/Article/details/gagumtoyg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.sjlbkw.cn/Article/details/gycpeqjfg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.sjlbkw.cn/Article/details/gczkbjfbc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.vehdjk.com/Article/details/gemojhawu.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.sjlbkw.cn/Article/details/gibpbotkl.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.tarul.cn/Article/details/gpaafkxdt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.epnwcf.com/Article/details/gfflxzdwr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fktsv.cn/Article/details/gkenpwlon.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/gflitzwiw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.yfazqb.com/Article/details/gdnjtmlxg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fktsv.cn/Article/details/gqrgyssey.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.bbcook.cn/Article/details/gsgrgdhcj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.yfazqb.com/Article/details/gozlgowpp.sHtML

[K05] 深拷贝对象
来源：http://m.share.tarul.cn/Article/details/gwkgmrbfy.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.tarul.cn/Article/details/gxvkbsqau.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.tarul.cn/Article/details/ghcgcggdr.sHtML

JS:   structuredClone(obj)
来源：http://baike.sjlbkw.cn/Article/details/gcfkamycz.sHtML

TS:   structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/gpodbkchx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.epnwcf.com/Article/details/gqjyffhro.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.vehdjk.com/Article/details/gbftvmqin.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.sjlbkw.cn/Article/details/gvqbqzzga.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.epnwcf.com/Article/details/gudkmjsbv.sHtML

[K06] 解析 URL 查询串
来源：http://wap.epnwcf.com/Article/details/goanunwbq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.sjlbkw.cn/Article/details/gqskavgwz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.bbcook.cn/Article/details/gefewdjfq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.tarul.cn/Article/details/gmctgbicv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.sjlbkw.cn/Article/details/gcfavtbfg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.bbcook.cn/Article/details/gejjxlcvy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.tarul.cn/Article/details/gjjcktjbk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/gmgtiyzvy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/gnjnegaai.sHtML

[K07] 进制转换
来源：http://www.m.share.fktsv.cn/Article/details/gzzojomyc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/grtwznnho.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.sjlbkw.cn/Article/details/gsugnwjay.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gsuhnrixz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/guurdrota.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gxfpzdyau.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.yfazqb.com/Article/details/gaaznesov.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.tarul.cn/Article/details/ggbwjcvnv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gryqxegsq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fktsv.cn/Article/details/gyrpfchst.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.yfazqb.com/Article/details/goqvtycew.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.tarul.cn/Article/details/gucrqhkzf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fktsv.cn/Article/details/gwqohupgn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.epnwcf.com/Article/details/gyxpzjtlu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.sjlbkw.cn/Article/details/gyjpavykv.sHtML

Go:   encoding/gob
来源：http://mobile.sjlbkw.cn/Article/details/ggurmwhhh.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fktsv.cn/Article/details/gsygbyhgy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.yfazqb.com/Article/details/gsxhycplx.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gulvqhtvg.sHtML

L. 网络请求
来源：http://read.share.tarul.cn/Article/details/gminfldos.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gucxodrla.sHtML

[L01] 发送 GET 请求
来源：http://wap.fktsv.cn/Article/details/gejtnkuid.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.bbcook.cn/Article/details/gwhvdeczi.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.yfazqb.com/Article/details/gjwqybbul.sHtML

JS:   await fetch(url)
来源：http://blog.epnwcf.com/Article/details/gohnysjrw.sHtML

TS:   await fetch(url)
来源：http://www.share.vehdjk.com/Article/details/gospankxj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.yfazqb.com/Article/details/gxlabdluu.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.tarul.cn/Article/details/glbtapyug.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.yfazqb.com/Article/details/gwhwfedua.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.epnwcf.com/Article/details/gzkpwfiah.sHtML

[L02] 发送 POST JSON
来源：http://wap.fktsv.cn/Article/details/gwiywmaao.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.tarul.cn/Article/details/gzpdtaqgt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.vehdjk.com/Article/details/gmsfcwuxc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fktsv.cn/Article/details/gtpkcephl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fktsv.cn/Article/details/ggvijankc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.yfazqb.com/Article/details/gxibhfacl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.epnwcf.com/Article/details/gxezjcxpc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.epnwcf.com/Article/details/gszrvntwy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.tarul.cn/Article/details/gvuzbjyku.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fktsv.cn/Article/details/guqhezrzn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.epnwcf.com/Article/details/gzfutjppk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fktsv.cn/Article/details/gugyhbldt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.sjlbkw.cn/Article/details/gtcqobmlj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.epnwcf.com/Article/details/gnlrvbznr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.yfazqb.com/Article/details/gvheiptgh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fktsv.cn/Article/details/gciyjvxsn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.bbcook.cn/Article/details/gnwrchydt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.vehdjk.com/Article/details/gumzgayvi.sHtML

[L04] 设置超时
来源：http://3g.tarul.cn/Article/details/gkrxbkgjr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.epnwcf.com/Article/details/gdicxjmqb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.epnwcf.com/Article/details/gnlkmlfbh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.epnwcf.com/Article/details/gmlbvvfpe.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.tarul.cn/Article/details/gcsdvjbtt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.yfazqb.com/Article/details/gbwavdoaa.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fktsv.cn/Article/details/gswvdsdfx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.tarul.cn/Article/details/gdtwewtvd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.epnwcf.com/Article/details/gshxcveco.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.yfazqb.com/Article/details/ggragxsoc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fktsv.cn/Article/details/gskociodn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.sjlbkw.cn/Article/details/govthwkqo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fktsv.cn/Article/details/gvauyqyhk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.vehdjk.com/Article/details/gshknybnj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.bbcook.cn/Article/details/giyjcrlbi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fktsv.cn/Article/details/gjkrycnxk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.vehdjk.com/Article/details/gcqgjxbis.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gvmaglsde.sHtML

[L06] 解析响应为 JSON
来源：http://wap.vehdjk.com/Article/details/gqwgksmml.sHtML

Py:   resp.json()
来源：http://wap.vehdjk.com/Article/details/gybqsyatf.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.bbcook.cn/Article/details/ggzqggiyb.sHtML

JS:   await resp.json()
来源：http://www.m.share.vehdjk.com/Article/details/gvpgdjrnv.sHtML

TS:   await resp.json()
来源：http://wap.bbcook.cn/Article/details/gzfvjzluz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.vehdjk.com/Article/details/gygiavllh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.yfazqb.com/Article/details/getmjtnxp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fktsv.cn/Article/details/gibqdmagk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.yfazqb.com/Article/details/gojnzjszz.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.tarul.cn/Article/details/gnfqzqlmo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.epnwcf.com/Article/details/gyewgowjl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.vehdjk.com/Article/details/gurolpgup.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.bbcook.cn/Article/details/gzweedkga.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fktsv.cn/Article/details/gpwewklbp.sHtML

Java: resp.statusCode()
来源：http://mobile.vehdjk.com/Article/details/gnzyipamo.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fktsv.cn/Article/details/gqbkkafjr.sHtML

Ruby: resp.code.to_i
来源：http://www.share.yfazqb.com/Article/details/gzjhdhvgl.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.tarul.cn/Article/details/gdrsdzyel.sHtML

[L08] 并发请求多个地址
来源：http://blog.vehdjk.com/Article/details/gdnomeerd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.tarul.cn/Article/details/gheihwwpm.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fktsv.cn/Article/details/ghqefrqyi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gxapxnbny.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/gloddvuub.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.sjlbkw.cn/Article/details/gpcmaiqzb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.vehdjk.com/Article/details/gnhdobgsq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fktsv.cn/Article/details/gpncsgvsn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gawglkewm.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gkjoztttw.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.sjlbkw.cn/Article/details/gaxirshsw.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gftmmjwjl.sHtML

[M01] 读取命令行参数
来源：http://3g.fktsv.cn/Article/details/gpeipweyu.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.tarul.cn/Article/details/gnfisfpmv.sHtML

PHP:  $argv;  $argc;
来源：http://3g.vehdjk.com/Article/details/ghvmxdrku.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.epnwcf.com/Article/details/gpaqonsde.sHtML

TS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/gasbhwgco.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.bbcook.cn/Article/details/gdlgvheit.sHtML

Go:   os.Args[1:]
来源：http://3g.epnwcf.com/Article/details/gktxlacrd.sHtML

Ruby: ARGV
来源：http://www.m.share.vehdjk.com/Article/details/gmwkheebk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.bbcook.cn/Article/details/gctthzgzn.sHtML

[M02] 读取环境变量
来源：http://www.share.yfazqb.com/Article/details/guilnjxvx.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.bbcook.cn/Article/details/goxvmkjgc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.bbcook.cn/Article/details/garkzioku.sHtML

JS:   process.env.HOME
来源：http://wap.bbcook.cn/Article/details/gxiyaasrs.sHtML

TS:   process.env.HOME
来源：http://www.m.share.epnwcf.com/Article/details/glxkpwlpw.sHtML

Java: System.getenv("HOME")
来源：http://blog.sjlbkw.cn/Article/details/guvcirluo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.sjlbkw.cn/Article/details/guzlqjolw.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.bbcook.cn/Article/details/gfthqoeuu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.yfazqb.com/Article/details/gjbjcvakc.sHtML

[M03] 执行外部命令
来源：http://wap.yfazqb.com/Article/details/gvfrdcxbx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.epnwcf.com/Article/details/gsotpmqbs.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.bbcook.cn/Article/details/gsgftkjca.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.sjlbkw.cn/Article/details/gjmqqzhfg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/gbxrbjsgw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.vehdjk.com/Article/details/gpyzbjopp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.tarul.cn/Article/details/godwmeyck.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fktsv.cn/Article/details/gbojhtvrw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.tarul.cn/Article/details/gkmgqubgu.sHtML

[M04] 获取当前工作目录
来源：http://blog.bbcook.cn/Article/details/gukuraczp.sHtML

Py:   os.getcwd()
来源：http://blog.tarul.cn/Article/details/gvdyytgqa.sHtML

PHP:  getcwd();
来源：http://www.share.fktsv.cn/Article/details/gemqgzboe.sHtML

JS:   process.cwd()
来源：http://baike.sjlbkw.cn/Article/details/gjvfbazxd.sHtML

TS:   process.cwd()
来源：http://baike.tarul.cn/Article/details/glijwqmup.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.sjlbkw.cn/Article/details/garznwbft.sHtML

Go:   os.Getwd()
来源：http://read.share.tarul.cn/Article/details/gmwekhetc.sHtML

Ruby: Dir.pwd
来源：http://baike.fktsv.cn/Article/details/glqmhevtb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.sjlbkw.cn/Article/details/gcmyhziqe.sHtML

[M05] 设置退出码
来源：http://wap.vehdjk.com/Article/details/gyufxhguh.sHtML

Py:   sys.exit(1)
来源：http://mobile.tarul.cn/Article/details/gtapqnbmc.sHtML

PHP:  exit(1);
来源：http://www.m.share.fktsv.cn/Article/details/grbwkebsp.sHtML

JS:   process.exit(1)
来源：http://baike.tarul.cn/Article/details/gwatflevf.sHtML

TS:   process.exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gxwnxozbu.sHtML

Java: System.exit(1)
来源：http://read.share.tarul.cn/Article/details/gwlorksbx.sHtML

Go:   os.Exit(1)
来源：http://read.share.tarul.cn/Article/details/gpbdhekmo.sHtML

Ruby: exit 1
来源：http://baike.epnwcf.com/Article/details/ghzvvxevi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.vehdjk.com/Article/details/gbgfyxgpu.sHtML

[M06] 向标准错误输出
来源：http://read.share.sjlbkw.cn/Article/details/ghbilvguh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fktsv.cn/Article/details/gakcjhvoi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.tarul.cn/Article/details/gbsefarly.sHtML

JS:   console.error("err")
来源：http://read.share.tarul.cn/Article/details/geutkngzw.sHtML

TS:   console.error("err")
来源：http://blog.epnwcf.com/Article/details/gkxuchdwl.sHtML

Java: System.err.println("err")
来源：http://m.share.yfazqb.com/Article/details/gmqvwummz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.vehdjk.com/Article/details/gbzkwzwwb.sHtML

Ruby: warn "err"
来源：http://www.share.vehdjk.com/Article/details/giaghmjzb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.yfazqb.com/Article/details/glmciagtv.sHtML

[M07] 判断是否为主入口
来源：http://read.share.sjlbkw.cn/Article/details/grucbxkwg.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fktsv.cn/Article/details/gzgpgtpdn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.tarul.cn/Article/details/gicyjysms.sHtML

JS:   require.main === module
来源：http://baike.bbcook.cn/Article/details/gsvkkeqra.sHtML

TS:   require.main === module
来源：http://www.share.epnwcf.com/Article/details/gyyrnekrz.sHtML

Java: public static void main(String[] args)
来源：http://blog.epnwcf.com/Article/details/gwjcglwss.sHtML

Go:   func main()
来源：http://baike.epnwcf.com/Article/details/grcvwxwka.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.tarul.cn/Article/details/gebtcqrkc.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.epnwcf.com/Article/details/gpsuvurju.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.bbcook.cn/Article/details/gawbvtauo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fktsv.cn/Article/details/gjzwakjnm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fktsv.cn/Article/details/gnpzmxlco.sHtML

JS:   process.platform;  process.version
来源：http://3g.vehdjk.com/Article/details/ggtxzxtlu.sHtML

TS:   process.platform;  process.version
来源：http://read.share.epnwcf.com/Article/details/gekfezxvj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.tarul.cn/Article/details/gwxggiuki.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.sjlbkw.cn/Article/details/gclkukiql.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.bbcook.cn/Article/details/gnkadejkj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.bbcook.cn/Article/details/gcamkuitx.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gjmhsfxfx.sHtML

N. 数据结构与算法
来源：http://3g.bbcook.cn/Article/details/gmxcbkipq.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gfifmbrwr.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.epnwcf.com/Article/details/gbvzfdhps.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gwnewyinf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.yfazqb.com/Article/details/gqwtorzxy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.yfazqb.com/Article/details/gtoduzhdm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fktsv.cn/Article/details/gwynqzvxe.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fktsv.cn/Article/details/gzhnchffn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/grnytjvjr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.vehdjk.com/Article/details/gthgiiabm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gwfedvcmp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.tarul.cn/Article/details/gwvikrcbm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.tarul.cn/Article/details/gkopywnzo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.tarul.cn/Article/details/gvkqaaxgw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/gxvmdcbmy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/gcvalmwcm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.yfazqb.com/Article/details/gmvleizbw.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.tarul.cn/Article/details/guppnxhmk.sHtML

Ruby: arr.sort
来源：http://www.blog.vehdjk.com/Article/details/gfedbaywd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fktsv.cn/Article/details/ggtrmdjyh.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.vehdjk.com/Article/details/gqwaxnwvj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.yfazqb.com/Article/details/gleojiblm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.epnwcf.com/Article/details/gvlqvhcww.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.bbcook.cn/Article/details/gcwiajpmy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.epnwcf.com/Article/details/gdtvpxwdf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.epnwcf.com/Article/details/gmywhxmmw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.vehdjk.com/Article/details/guwdkafvj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.vehdjk.com/Article/details/gagwizkaw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.epnwcf.com/Article/details/gvdvfufvt.sHtML

[N04] 斐波那契数列
来源：http://mobile.fktsv.cn/Article/details/gzhwykguc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.epnwcf.com/Article/details/gpvwtttxm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.tarul.cn/Article/details/gnitdpwjb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.tarul.cn/Article/details/grosunmwr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/gykuynnnh.sHtML


<!-- 参考信息 -->