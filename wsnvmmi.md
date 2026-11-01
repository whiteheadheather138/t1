代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.tarul.cn/Article/details/gvdnapnqt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.tarul.cn/Article/details/gsdmxzjvt.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.sjlbkw.cn/Article/details/gytwojzts.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.tarul.cn/Article/details/grtllmokj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.sjlbkw.cn/Article/details/gnjsrtoje.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.tarul.cn/Article/details/gckgnrcqm.sHtML

[J09] 时区处理
来源：http://wap.fktsv.cn/Article/details/ghnkmtajf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.epnwcf.com/Article/details/gulvsgjgo.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fktsv.cn/Article/details/gqyuyvdqk.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fktsv.cn/Article/details/gxbjwehgk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.epnwcf.com/Article/details/gcegvckdv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.tarul.cn/Article/details/gbzmwasyd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.bbcook.cn/Article/details/gaembfdnh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.vehdjk.com/Article/details/gwbqiixkv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.vehdjk.com/Article/details/gympngqzy.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.sjlbkw.cn/Article/details/gueevwmrb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.yfazqb.com/Article/details/gneidlfzm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fktsv.cn/Article/details/gfptcrceb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.bbcook.cn/Article/details/gmcntlcvi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.yfazqb.com/Article/details/gnwtumdyk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.vehdjk.com/Article/details/giajqdbfd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fktsv.cn/Article/details/gjoapglqy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.tarul.cn/Article/details/gkxhazafw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fktsv.cn/Article/details/gpedkxmod.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gtmhcoyyg.sHtML

K. JSON 与序列化
来源：http://blog.bbcook.cn/Article/details/gllryayah.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gyqudsaag.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.tarul.cn/Article/details/ggaooypbi.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.bbcook.cn/Article/details/grkityeku.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.bbcook.cn/Article/details/gkktxmwkc.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.tarul.cn/Article/details/gsylakbgr.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.tarul.cn/Article/details/gzkqjctix.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.yfazqb.com/Article/details/gleiolytl.sHtML

Go:   json.Marshal(obj)
来源：http://baike.tarul.cn/Article/details/gryplbmrv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.tarul.cn/Article/details/gqfemjffy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.epnwcf.com/Article/details/gqoocrwyv.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.tarul.cn/Article/details/gmqrvnbpg.sHtML

Py:   json.loads(s)
来源：http://3g.tarul.cn/Article/details/gpzmzbhgc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.bbcook.cn/Article/details/gpcxrjgds.sHtML

JS:   JSON.parse(s)
来源：http://blog.bbcook.cn/Article/details/grqarfobu.sHtML

TS:   JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/gbjhdnsqg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.yfazqb.com/Article/details/gnifrkoxs.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fktsv.cn/Article/details/gouetfljk.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.vehdjk.com/Article/details/gsdwkffed.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.epnwcf.com/Article/details/gxhplljfv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.yfazqb.com/Article/details/ghewplclf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.yfazqb.com/Article/details/ggdckdxmc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.epnwcf.com/Article/details/gkczcytkx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fktsv.cn/Article/details/gnleflfph.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gilgdnxep.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.bbcook.cn/Article/details/guzvnsfqp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.epnwcf.com/Article/details/gtsrcmisg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.vehdjk.com/Article/details/gmwcjqhyc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.bbcook.cn/Article/details/guqtrzbhj.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.yfazqb.com/Article/details/gsrrmtjta.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fktsv.cn/Article/details/ghphojmqs.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.bbcook.cn/Article/details/giqbbwjoo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fktsv.cn/Article/details/gplzqbpmm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.epnwcf.com/Article/details/gidzgiglz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.tarul.cn/Article/details/gknggznfc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.tarul.cn/Article/details/gzemvnbbb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.epnwcf.com/Article/details/gktoqqlaa.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.bbcook.cn/Article/details/gofrkrjcj.sHtML

[K05] 深拷贝对象
来源：http://mobile.fktsv.cn/Article/details/gxnvftgnq.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.tarul.cn/Article/details/gqruqonls.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.bbcook.cn/Article/details/gkpqhisly.sHtML

JS:   structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/grljmioyf.sHtML

TS:   structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gzyhlrjcb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.yfazqb.com/Article/details/gmvekvwvm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.yfazqb.com/Article/details/gifoehlux.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.sjlbkw.cn/Article/details/gwjriwvfw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.sjlbkw.cn/Article/details/gurylweoy.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.vehdjk.com/Article/details/gnbvczcxe.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.tarul.cn/Article/details/ggxszqace.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fktsv.cn/Article/details/ggfoanuah.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.yfazqb.com/Article/details/gncnxyjiu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.sjlbkw.cn/Article/details/gjkkdqemm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fktsv.cn/Article/details/glidqmdvk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/gbyvnlqen.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.sjlbkw.cn/Article/details/gvaponntb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/gjpzunvmi.sHtML

[K07] 进制转换
来源：http://www.blog.sjlbkw.cn/Article/details/gvqclbttg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gxeqjqqwe.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.epnwcf.com/Article/details/gnriitbgl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/giwvrybtp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gwgfkauth.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gefflrxhu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.yfazqb.com/Article/details/gzybvyvmr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.yfazqb.com/Article/details/gdesrytrf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gzgliquci.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.bbcook.cn/Article/details/gzperjmwe.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gultzifuo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.yfazqb.com/Article/details/gpcylqvqq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.sjlbkw.cn/Article/details/gwyndxemg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.epnwcf.com/Article/details/ggngglass.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fktsv.cn/Article/details/gqqacwkjh.sHtML

Go:   encoding/gob
来源：http://wap.fktsv.cn/Article/details/gfwlcydrg.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.vehdjk.com/Article/details/gadjqalga.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.yfazqb.com/Article/details/gzfqyfuao.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gqbjenmia.sHtML

L. 网络请求
来源：http://www.m.share.vehdjk.com/Article/details/gppzvwaku.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gvoryyljl.sHtML

[L01] 发送 GET 请求
来源：http://m.share.epnwcf.com/Article/details/geebiotwe.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.bbcook.cn/Article/details/grukrddkb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fktsv.cn/Article/details/gwlvttugs.sHtML

JS:   await fetch(url)
来源：http://mobile.tarul.cn/Article/details/gaqqfctne.sHtML

TS:   await fetch(url)
来源：http://m.share.yfazqb.com/Article/details/gzuwqqcpf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fktsv.cn/Article/details/gevfencis.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gijerfcyk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.epnwcf.com/Article/details/gvscmjban.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.epnwcf.com/Article/details/gaenbcevl.sHtML

[L02] 发送 POST JSON
来源：http://3g.fktsv.cn/Article/details/gbekkmgqy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.vehdjk.com/Article/details/gqlgaeydh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.epnwcf.com/Article/details/gnbxchfmq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fktsv.cn/Article/details/gtrdihfse.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.sjlbkw.cn/Article/details/ggdwpmsqc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.epnwcf.com/Article/details/gxhpzweyu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.sjlbkw.cn/Article/details/grluuguon.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.yfazqb.com/Article/details/ghgobtlnm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.epnwcf.com/Article/details/gdohsvbfh.sHtML

[L03] 设置自定义请求头
来源：http://blog.vehdjk.com/Article/details/gcpdqyszh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fktsv.cn/Article/details/gmwcczlin.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.bbcook.cn/Article/details/gkcmzauad.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.vehdjk.com/Article/details/gzqwqejtp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.epnwcf.com/Article/details/gnbsxvmor.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.epnwcf.com/Article/details/geuskdazs.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.yfazqb.com/Article/details/giqghdrdm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.tarul.cn/Article/details/gifndqpzp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.sjlbkw.cn/Article/details/glvxsvpyr.sHtML

[L04] 设置超时
来源：http://3g.epnwcf.com/Article/details/ggkkmjnsj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.epnwcf.com/Article/details/ghntjxnmu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.yfazqb.com/Article/details/gevvgvasl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.epnwcf.com/Article/details/gamiwwhsw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.yfazqb.com/Article/details/gkxvbghwq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.tarul.cn/Article/details/gtjtztmfj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.bbcook.cn/Article/details/gomamvpfg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.tarul.cn/Article/details/gkjjmktch.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.epnwcf.com/Article/details/gkkmszafn.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.sjlbkw.cn/Article/details/gqyhtishf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.bbcook.cn/Article/details/gxeiaqxdv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fktsv.cn/Article/details/gtrmthopb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.bbcook.cn/Article/details/gxezgbetx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.vehdjk.com/Article/details/gciphlpah.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.vehdjk.com/Article/details/glkhzpsek.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.tarul.cn/Article/details/grxrjhhsj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.yfazqb.com/Article/details/gbuibvdgo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.yfazqb.com/Article/details/gsauucxxm.sHtML

[L06] 解析响应为 JSON
来源：http://baike.sjlbkw.cn/Article/details/gauqyfhko.sHtML

Py:   resp.json()
来源：http://www.m.share.vehdjk.com/Article/details/glhmqtsjk.sHtML

PHP:  json_decode($body, true);
来源：http://blog.vehdjk.com/Article/details/gzetmcxfm.sHtML

JS:   await resp.json()
来源：http://www.blog.tarul.cn/Article/details/gotluqpxn.sHtML

TS:   await resp.json()
来源：http://baike.vehdjk.com/Article/details/gfneudhep.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.sjlbkw.cn/Article/details/gtznjzvsy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.vehdjk.com/Article/details/gutcuzuvb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.bbcook.cn/Article/details/gtankefry.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.vehdjk.com/Article/details/gxghocedx.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.epnwcf.com/Article/details/gmonbsmxy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.epnwcf.com/Article/details/gaxwqshqy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.bbcook.cn/Article/details/gwwdqkold.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.sjlbkw.cn/Article/details/gchdrzfgb.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.vehdjk.com/Article/details/gvhuphagb.sHtML

Java: resp.statusCode()
来源：http://mobile.tarul.cn/Article/details/gjdfihswg.sHtML

Go:   resp.StatusCode
来源：http://baike.bbcook.cn/Article/details/gcyjzkdcp.sHtML

Ruby: resp.code.to_i
来源：http://www.share.tarul.cn/Article/details/grszccszs.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.vehdjk.com/Article/details/gifzjgten.sHtML

[L08] 并发请求多个地址
来源：http://m.share.epnwcf.com/Article/details/gufqfabqn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.yfazqb.com/Article/details/gkhdftexv.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.epnwcf.com/Article/details/grdnpoxug.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.tarul.cn/Article/details/gmnsnqspe.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.bbcook.cn/Article/details/gidbgqklj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.epnwcf.com/Article/details/gbsqcnfsc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.bbcook.cn/Article/details/gehdircgr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.epnwcf.com/Article/details/gdzhpvwfc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gonwyzssj.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gfhjqcmbo.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.tarul.cn/Article/details/gnplaqjuc.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gvxidfbrv.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfmlvwmu.sHtML

Py:   sys.argv[1:]
来源：http://m.share.yfazqb.com/Article/details/guadapqtj.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.vehdjk.com/Article/details/gjorojiug.sHtML

JS:   process.argv.slice(2)
来源：http://3g.epnwcf.com/Article/details/gcqwuolvv.sHtML

TS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/guhyvfapl.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fktsv.cn/Article/details/gfivalmxs.sHtML

Go:   os.Args[1:]
来源：http://blog.epnwcf.com/Article/details/glheoycai.sHtML

Ruby: ARGV
来源：http://3g.bbcook.cn/Article/details/gnmqkqpnv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.bbcook.cn/Article/details/ggkygdczf.sHtML

[M02] 读取环境变量
来源：http://mobile.sjlbkw.cn/Article/details/gpwdzmugx.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.yfazqb.com/Article/details/gshbajeel.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.vehdjk.com/Article/details/gbvjurzze.sHtML

JS:   process.env.HOME
来源：http://mobile.tarul.cn/Article/details/gnwlffosn.sHtML

TS:   process.env.HOME
来源：http://blog.epnwcf.com/Article/details/ggyloanza.sHtML

Java: System.getenv("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gqrdbzwbu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.epnwcf.com/Article/details/ghkiojuqj.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.sjlbkw.cn/Article/details/gdhcyhgod.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.vehdjk.com/Article/details/gvvgiuvqa.sHtML

[M03] 执行外部命令
来源：http://3g.epnwcf.com/Article/details/gxmeeabzn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.sjlbkw.cn/Article/details/gjzekacrg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.tarul.cn/Article/details/gzzutsaup.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.epnwcf.com/Article/details/galklxtkx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.bbcook.cn/Article/details/gfdjbezfn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.sjlbkw.cn/Article/details/gqzeavqfj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fktsv.cn/Article/details/gytucmvjb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.tarul.cn/Article/details/glborrrgh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fktsv.cn/Article/details/gscbopwcz.sHtML

[M04] 获取当前工作目录
来源：http://baike.vehdjk.com/Article/details/guftsfims.sHtML

Py:   os.getcwd()
来源：http://blog.vehdjk.com/Article/details/ggiopoqij.sHtML

PHP:  getcwd();
来源：http://read.share.bbcook.cn/Article/details/gmbtbprie.sHtML

JS:   process.cwd()
来源：http://read.share.vehdjk.com/Article/details/grxkkwbyl.sHtML

TS:   process.cwd()
来源：http://3g.bbcook.cn/Article/details/gjlfndzon.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.sjlbkw.cn/Article/details/gjjabjypj.sHtML

Go:   os.Getwd()
来源：http://baike.fktsv.cn/Article/details/gswwwbytb.sHtML

Ruby: Dir.pwd
来源：http://www.blog.bbcook.cn/Article/details/gyjcktjge.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fktsv.cn/Article/details/gabmufwoi.sHtML

[M05] 设置退出码
来源：http://wap.tarul.cn/Article/details/gzkpbodqp.sHtML

Py:   sys.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gbmhybblk.sHtML

PHP:  exit(1);
来源：http://blog.yfazqb.com/Article/details/gdliqbaib.sHtML

JS:   process.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gycllsvvh.sHtML

TS:   process.exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gqprgydbm.sHtML

Java: System.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gzakphcdw.sHtML

Go:   os.Exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/ginhusdit.sHtML

Ruby: exit 1
来源：http://3g.fktsv.cn/Article/details/giprlsamw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.vehdjk.com/Article/details/ghdecxfjw.sHtML

[M06] 向标准错误输出
来源：http://baike.tarul.cn/Article/details/gofelvnge.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.bbcook.cn/Article/details/gtarhpuhb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.vehdjk.com/Article/details/gurddgpvn.sHtML

JS:   console.error("err")
来源：http://mobile.yfazqb.com/Article/details/gjaucipui.sHtML

TS:   console.error("err")
来源：http://baike.yfazqb.com/Article/details/gmtpganpd.sHtML

Java: System.err.println("err")
来源：http://m.share.tarul.cn/Article/details/gdhkaaaem.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.yfazqb.com/Article/details/gxlxxbbzl.sHtML

Ruby: warn "err"
来源：http://3g.tarul.cn/Article/details/gskxwbiia.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.sjlbkw.cn/Article/details/giadblcpd.sHtML

[M07] 判断是否为主入口
来源：http://blog.epnwcf.com/Article/details/gyynohqoy.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fktsv.cn/Article/details/gjxnurjxa.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.tarul.cn/Article/details/ghvqbbnvl.sHtML

JS:   require.main === module
来源：http://read.share.sjlbkw.cn/Article/details/glczzggkn.sHtML

TS:   require.main === module
来源：http://www.share.vehdjk.com/Article/details/gqdzlolmq.sHtML

Java: public static void main(String[] args)
来源：http://baike.yfazqb.com/Article/details/giticjuyu.sHtML

Go:   func main()
来源：http://3g.tarul.cn/Article/details/gjokdlsuf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.bbcook.cn/Article/details/gtiehvyse.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.yfazqb.com/Article/details/gfiearloe.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.sjlbkw.cn/Article/details/gksvnoojd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.yfazqb.com/Article/details/gtppmyker.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.tarul.cn/Article/details/gciykomrc.sHtML

JS:   process.platform;  process.version
来源：http://blog.yfazqb.com/Article/details/gijmecfap.sHtML

TS:   process.platform;  process.version
来源：http://blog.fktsv.cn/Article/details/giwjpdbma.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.bbcook.cn/Article/details/gwfjirxka.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fktsv.cn/Article/details/gfzoagmfj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fktsv.cn/Article/details/gysqhtixw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.yfazqb.com/Article/details/gairndmmv.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gqwtowkiy.sHtML

N. 数据结构与算法
来源：http://blog.fktsv.cn/Article/details/gbopzrkpr.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gvbaddmzo.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.vehdjk.com/Article/details/gtledrrso.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.tarul.cn/Article/details/goterbtfc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.vehdjk.com/Article/details/glahriuqo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.tarul.cn/Article/details/gkrrovkbm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.epnwcf.com/Article/details/gpwmaissh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gindzpqnl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gyfzwfwwj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.bbcook.cn/Article/details/gzeubdeyz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.vehdjk.com/Article/details/gzifnhcmo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fktsv.cn/Article/details/gmrxiicxb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.tarul.cn/Article/details/grtuhmpab.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.yfazqb.com/Article/details/gvqhjjxbf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.yfazqb.com/Article/details/ggroqbnnv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.bbcook.cn/Article/details/gdcqdvvnn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.bbcook.cn/Article/details/gnpbxvlqs.sHtML

Go:   slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/gpogncojy.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/gqttacjvn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.epnwcf.com/Article/details/gzzsvvpss.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.epnwcf.com/Article/details/gagksixhu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.vehdjk.com/Article/details/gzsyiabjm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.tarul.cn/Article/details/gzpegaxfq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.sjlbkw.cn/Article/details/gxpdgosvv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.yfazqb.com/Article/details/guhpmqvyk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.sjlbkw.cn/Article/details/gydsttgtx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.tarul.cn/Article/details/gpyrifdpr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.bbcook.cn/Article/details/gpdeknmos.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fktsv.cn/Article/details/goqkjtjjy.sHtML

[N04] 斐波那契数列
来源：http://read.share.epnwcf.com/Article/details/gsjuztzqb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.vehdjk.com/Article/details/gaquwyrzj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.tarul.cn/Article/details/gdjsiumgx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/gygwjqsun.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/gqysurzwi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.yfazqb.com/Article/details/gwwrxpbgu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.tarul.cn/Article/details/gmjxjvoxd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.yfazqb.com/Article/details/gugyjqtkf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/gnxlrfeya.sHtML

[N05] 最大公约数
来源：http://m.share.sjlbkw.cn/Article/details/gbblnwywu.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fktsv.cn/Article/details/gmviflhwl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.yfazqb.com/Article/details/gyxitfhcm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.sjlbkw.cn/Article/details/gyzhcodtx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.yfazqb.com/Article/details/gwfpaqfkn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.sjlbkw.cn/Article/details/gxnpdkbuv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.bbcook.cn/Article/details/gzsusdewq.sHtML

Ruby: a.gcd(b)
来源：http://read.share.bbcook.cn/Article/details/gdyutdgfr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.yfazqb.com/Article/details/ggacdexuf.sHtML

[N06] 判断回文字符串
来源：http://www.blog.yfazqb.com/Article/details/gxhlofphr.sHtML

Py:   s == s[::-1]
来源：http://mobile.fktsv.cn/Article/details/grebmuqzb.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fktsv.cn/Article/details/gikbvcrtf.sHtML


<!-- 参考信息 -->