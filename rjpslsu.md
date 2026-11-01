代发 wailian999

[J07] 比较两个日期
来源：http://blog.vehdjk.com/Article/details/grzspkxwr.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.tarul.cn/Article/details/gcpbpekck.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.epnwcf.com/Article/details/gsxbbyiul.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.yfazqb.com/Article/details/gxpdifgxj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.epnwcf.com/Article/details/gajphsdbm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.fktsv.cn/Article/details/gcevnuiak.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.sjlbkw.cn/Article/details/gjwtjqwuu.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.bbcook.cn/Article/details/gazggqnxd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.fktsv.cn/Article/details/gwshgzyqp.sHtML

[J08] 提取年月日与星期
来源：http://mobile.yfazqb.com/Article/details/grdmfxvgd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.vehdjk.com/Article/details/gyoapgmlg.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.bbcook.cn/Article/details/gaazhsbox.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.sjlbkw.cn/Article/details/gmlqtwipf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.vehdjk.com/Article/details/gfxgkurvz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.tarul.cn/Article/details/gjeqfsvco.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.yfazqb.com/Article/details/gfpymubqs.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.epnwcf.com/Article/details/glneleaxa.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.tarul.cn/Article/details/ghsmkcpey.sHtML

[J09] 时区处理
来源：http://wap.bbcook.cn/Article/details/gcdqpiwkd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.tarul.cn/Article/details/gukppccsg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.sjlbkw.cn/Article/details/gkgjklkls.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.vehdjk.com/Article/details/gsckbeazn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fktsv.cn/Article/details/gdbjzzyeb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.sjlbkw.cn/Article/details/gatydfsaj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.vehdjk.com/Article/details/gktkubnqd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fktsv.cn/Article/details/gvxkdjpel.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.bbcook.cn/Article/details/gisgsivnl.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.fktsv.cn/Article/details/ganbdhace.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fktsv.cn/Article/details/gaivrbwsi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fktsv.cn/Article/details/gaybmpifj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.epnwcf.com/Article/details/gnnknbcpy.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fktsv.cn/Article/details/ghcqowofq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.epnwcf.com/Article/details/ghkeiosff.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.epnwcf.com/Article/details/gsqmypsqa.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.sjlbkw.cn/Article/details/gaowaerdo.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.yfazqb.com/Article/details/gefxiceop.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gpydvytmo.sHtML

K. JSON 与序列化
来源：http://read.share.vehdjk.com/Article/details/gnfeyytey.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gurfgegov.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.yfazqb.com/Article/details/gxasilxgg.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.epnwcf.com/Article/details/gstztfpbk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.yfazqb.com/Article/details/gdskpohus.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.epnwcf.com/Article/details/gkmffzdjo.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.sjlbkw.cn/Article/details/gwdldkrdh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.vehdjk.com/Article/details/gzkivquuu.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.epnwcf.com/Article/details/gyewehkoc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.bbcook.cn/Article/details/ggwhkvvig.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.bbcook.cn/Article/details/gzylijcxc.sHtML

[K02] JSON 字符串转对象
来源：http://blog.tarul.cn/Article/details/gpjukbgun.sHtML

Py:   json.loads(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gseqikwvq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.vehdjk.com/Article/details/gjrnhaiwc.sHtML

JS:   JSON.parse(s)
来源：http://baike.tarul.cn/Article/details/gdiszemsq.sHtML

TS:   JSON.parse(s)
来源：http://www.share.yfazqb.com/Article/details/greavftyy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/grkjvmuyr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.epnwcf.com/Article/details/gwukfjqdv.sHtML

Ruby: JSON.parse(s)
来源：http://blog.fktsv.cn/Article/details/gmdhenvsj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.sjlbkw.cn/Article/details/gsmkdjnob.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.bbcook.cn/Article/details/gaziiwunt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.bbcook.cn/Article/details/gycdtmruc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.tarul.cn/Article/details/gpbdjwnbf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.vehdjk.com/Article/details/gjeftvoyz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.sjlbkw.cn/Article/details/ggiewrkas.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.yfazqb.com/Article/details/gqyhyyyhh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.bbcook.cn/Article/details/gaukafluj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.vehdjk.com/Article/details/ggxmebrcy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhaiiurn.sHtML

[K04] 读取 JSON 文件
来源：http://blog.bbcook.cn/Article/details/gjccvklyd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fktsv.cn/Article/details/gckorylpv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.bbcook.cn/Article/details/gserxdjvm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.yfazqb.com/Article/details/giwxclpaj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.sjlbkw.cn/Article/details/gtdmrdfjx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.epnwcf.com/Article/details/ghjmuawtl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.epnwcf.com/Article/details/gynivrylf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.vehdjk.com/Article/details/ghpbsrwbz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.epnwcf.com/Article/details/gcracsiqs.sHtML

[K05] 深拷贝对象
来源：http://m.share.yfazqb.com/Article/details/gbdoimqal.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.tarul.cn/Article/details/gjzfypnze.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.yfazqb.com/Article/details/ggwhcpekj.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gnnvftglc.sHtML

TS:   structuredClone(obj)
来源：http://blog.yfazqb.com/Article/details/gyfxrhjvt.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.vehdjk.com/Article/details/gpkmwmyxj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fktsv.cn/Article/details/gkqkhbqeh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.vehdjk.com/Article/details/glwltlgng.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.yfazqb.com/Article/details/gxxgmkank.sHtML

[K06] 解析 URL 查询串
来源：http://baike.sjlbkw.cn/Article/details/gzvsjpgbm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.sjlbkw.cn/Article/details/gjgmciepu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fktsv.cn/Article/details/gibkhowsc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.vehdjk.com/Article/details/geukupluj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.epnwcf.com/Article/details/gmghcgmfw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.tarul.cn/Article/details/ghtmujhbo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/gbuhdefyb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.yfazqb.com/Article/details/gfdrudhno.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/gvlfjpeib.sHtML

[K07] 进制转换
来源：http://www.share.tarul.cn/Article/details/gypdfwdzy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gzmhaphsw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.yfazqb.com/Article/details/gtdpdnwil.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gbifybxiy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gqirzzkod.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gaduuqvod.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.vehdjk.com/Article/details/gwyqjeugs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.sjlbkw.cn/Article/details/gswivgrep.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gpsuaavix.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.vehdjk.com/Article/details/gepmokixq.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.sjlbkw.cn/Article/details/ghjvaibtb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.epnwcf.com/Article/details/gqykeckvf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fktsv.cn/Article/details/gflyekacs.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.vehdjk.com/Article/details/gelesktvt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.bbcook.cn/Article/details/gstdqfjzv.sHtML

Go:   encoding/gob
来源：http://www.blog.sjlbkw.cn/Article/details/gmscastyp.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.yfazqb.com/Article/details/gyoacdscy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.sjlbkw.cn/Article/details/gksnpdzrn.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/glrugylwy.sHtML

L. 网络请求
来源：http://baike.yfazqb.com/Article/details/guwamgpdv.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/glefapxxr.sHtML

[L01] 发送 GET 请求
来源：http://read.share.tarul.cn/Article/details/gjiyjqcsu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.sjlbkw.cn/Article/details/gddpaiqmf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.tarul.cn/Article/details/gdfmwwjlx.sHtML

JS:   await fetch(url)
来源：http://www.blog.yfazqb.com/Article/details/gqtvnfhys.sHtML

TS:   await fetch(url)
来源：http://read.share.tarul.cn/Article/details/gtkedgydx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.epnwcf.com/Article/details/gafjgsqzy.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.epnwcf.com/Article/details/gsnxggzvn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.sjlbkw.cn/Article/details/gevjjmwpp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.yfazqb.com/Article/details/gutvgcgql.sHtML

[L02] 发送 POST JSON
来源：http://3g.epnwcf.com/Article/details/gebuhknie.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.bbcook.cn/Article/details/glzefcyvt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.tarul.cn/Article/details/gtbaechwq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.tarul.cn/Article/details/gljfijufi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.bbcook.cn/Article/details/gydgmqhzf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.tarul.cn/Article/details/gfoghrpes.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.tarul.cn/Article/details/gphycjsjn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.sjlbkw.cn/Article/details/gacrdtrvc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.vehdjk.com/Article/details/gycwgsvps.sHtML

[L03] 设置自定义请求头
来源：http://3g.sjlbkw.cn/Article/details/gwsbrtxct.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fktsv.cn/Article/details/gkvsjjrlh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.bbcook.cn/Article/details/grhyfiraz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fktsv.cn/Article/details/gpdzjmluk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.tarul.cn/Article/details/gnonhjwon.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvehbter.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.vehdjk.com/Article/details/gausyuopl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fktsv.cn/Article/details/goxfxbcpt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fktsv.cn/Article/details/gtqrzgndf.sHtML

[L04] 设置超时
来源：http://www.blog.yfazqb.com/Article/details/gkibmugic.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.yfazqb.com/Article/details/guoezhxgm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.tarul.cn/Article/details/gsogcmnuk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fktsv.cn/Article/details/gasdcying.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.sjlbkw.cn/Article/details/gnfzzprqx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.bbcook.cn/Article/details/gakauaumb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.bbcook.cn/Article/details/gqbfxqbzc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.yfazqb.com/Article/details/gerjbrtcw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.epnwcf.com/Article/details/gdexdpdne.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.sjlbkw.cn/Article/details/gawuznpsm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.sjlbkw.cn/Article/details/gnxnfcdnf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fktsv.cn/Article/details/gjmehmfik.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.sjlbkw.cn/Article/details/gjpznhdsx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.vehdjk.com/Article/details/gaoxpapfx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fktsv.cn/Article/details/glhazgext.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.vehdjk.com/Article/details/gfhptidiy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.bbcook.cn/Article/details/gqdvmdyxd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.tarul.cn/Article/details/gbjlevgdp.sHtML

[L06] 解析响应为 JSON
来源：http://3g.bbcook.cn/Article/details/gaqzbfmir.sHtML

Py:   resp.json()
来源：http://mobile.sjlbkw.cn/Article/details/gmjdugzgb.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.bbcook.cn/Article/details/gljrcvqlr.sHtML

JS:   await resp.json()
来源：http://read.share.vehdjk.com/Article/details/gxcbqtbxz.sHtML

TS:   await resp.json()
来源：http://mobile.yfazqb.com/Article/details/gdefhvbom.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fktsv.cn/Article/details/gvoerwiiw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.sjlbkw.cn/Article/details/gfqmnpdub.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.tarul.cn/Article/details/ggxkmoixz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.yfazqb.com/Article/details/gvqpgqlvk.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fktsv.cn/Article/details/gdocizaft.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fktsv.cn/Article/details/gtigooqro.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.tarul.cn/Article/details/ggmckwyii.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.bbcook.cn/Article/details/gkfofdvgw.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.sjlbkw.cn/Article/details/gedyxfqky.sHtML

Java: resp.statusCode()
来源：http://read.share.vehdjk.com/Article/details/gmbnmgoia.sHtML

Go:   resp.StatusCode
来源：http://www.share.fktsv.cn/Article/details/gzavrirwe.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.yfazqb.com/Article/details/gllxsqcvh.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.yfazqb.com/Article/details/gjupiqiwi.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.yfazqb.com/Article/details/gcbjnqmun.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.bbcook.cn/Article/details/gpigimnnf.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.tarul.cn/Article/details/gkbewfkil.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.tarul.cn/Article/details/gcjoisxky.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.bbcook.cn/Article/details/gbbgbqrnu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.tarul.cn/Article/details/gttghmttj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.sjlbkw.cn/Article/details/gltrmtitb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.bbcook.cn/Article/details/gnpbrirse.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.tarul.cn/Article/details/gnhupuqms.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gtaxsrfcc.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.sjlbkw.cn/Article/details/grwnzwute.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/givcucfnq.sHtML

[M01] 读取命令行参数
来源：http://m.share.fktsv.cn/Article/details/gfxjtgnla.sHtML

Py:   sys.argv[1:]
来源：http://3g.epnwcf.com/Article/details/gkaqqdsop.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fktsv.cn/Article/details/gebvliikx.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.vehdjk.com/Article/details/gjedowfjm.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.vehdjk.com/Article/details/gtnafduik.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.sjlbkw.cn/Article/details/gfaxywggd.sHtML

Go:   os.Args[1:]
来源：http://www.share.yfazqb.com/Article/details/gctmudaoq.sHtML

Ruby: ARGV
来源：http://m.share.vehdjk.com/Article/details/gpjyygked.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.epnwcf.com/Article/details/gcuknntni.sHtML

[M02] 读取环境变量
来源：http://m.share.vehdjk.com/Article/details/gvvnxlkip.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.vehdjk.com/Article/details/gwtbicddb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.bbcook.cn/Article/details/gwvpgpaqk.sHtML

JS:   process.env.HOME
来源：http://wap.tarul.cn/Article/details/gvsivzkph.sHtML

TS:   process.env.HOME
来源：http://www.share.fktsv.cn/Article/details/gkaykffrj.sHtML

Java: System.getenv("HOME")
来源：http://m.share.tarul.cn/Article/details/gyxtqonyq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.vehdjk.com/Article/details/grjopssnk.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.vehdjk.com/Article/details/ghbrjuabw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gpmajhean.sHtML

[M03] 执行外部命令
来源：http://baike.bbcook.cn/Article/details/gbgskwbrh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.epnwcf.com/Article/details/gzwpkgjuw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.vehdjk.com/Article/details/gwhjacphu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.vehdjk.com/Article/details/gysxrqkfp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.vehdjk.com/Article/details/goxnihkfs.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.sjlbkw.cn/Article/details/gjqkpapak.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.epnwcf.com/Article/details/gdfoeqcez.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.sjlbkw.cn/Article/details/gvhgpbuyl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fktsv.cn/Article/details/gwzaacgfq.sHtML

[M04] 获取当前工作目录
来源：http://3g.epnwcf.com/Article/details/gkghtrjcx.sHtML

Py:   os.getcwd()
来源：http://read.share.epnwcf.com/Article/details/gozclrryx.sHtML

PHP:  getcwd();
来源：http://www.blog.epnwcf.com/Article/details/glqormbjg.sHtML

JS:   process.cwd()
来源：http://wap.sjlbkw.cn/Article/details/gldedvenp.sHtML

TS:   process.cwd()
来源：http://read.share.sjlbkw.cn/Article/details/grznswhly.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.epnwcf.com/Article/details/gulbbaveb.sHtML

Go:   os.Getwd()
来源：http://blog.fktsv.cn/Article/details/gpkzjnebi.sHtML

Ruby: Dir.pwd
来源：http://mobile.yfazqb.com/Article/details/gqzabnkis.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.yfazqb.com/Article/details/gryxqoufu.sHtML

[M05] 设置退出码
来源：http://www.blog.fktsv.cn/Article/details/gmszszkos.sHtML

Py:   sys.exit(1)
来源：http://blog.tarul.cn/Article/details/gkuckwnov.sHtML

PHP:  exit(1);
来源：http://www.m.share.vehdjk.com/Article/details/gqydbibty.sHtML

JS:   process.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gjgklplrh.sHtML

TS:   process.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqjosoxe.sHtML

Java: System.exit(1)
来源：http://mobile.tarul.cn/Article/details/gzemapfyr.sHtML

Go:   os.Exit(1)
来源：http://wap.yfazqb.com/Article/details/gfljsbmgh.sHtML

Ruby: exit 1
来源：http://blog.sjlbkw.cn/Article/details/gqqybhgmw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fktsv.cn/Article/details/gnwbrjueu.sHtML

[M06] 向标准错误输出
来源：http://m.share.bbcook.cn/Article/details/gfzvdvlsl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.bbcook.cn/Article/details/gimkrtzih.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.bbcook.cn/Article/details/ghpxlxffv.sHtML

JS:   console.error("err")
来源：http://baike.tarul.cn/Article/details/guxhftqhh.sHtML

TS:   console.error("err")
来源：http://mobile.fktsv.cn/Article/details/gathimguz.sHtML

Java: System.err.println("err")
来源：http://www.blog.vehdjk.com/Article/details/gzdopxtcu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.vehdjk.com/Article/details/guevrvdmy.sHtML

Ruby: warn "err"
来源：http://blog.epnwcf.com/Article/details/gkjytzuhz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.yfazqb.com/Article/details/gamoxwsdr.sHtML

[M07] 判断是否为主入口
来源：http://www.share.vehdjk.com/Article/details/gcdbqnzav.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.bbcook.cn/Article/details/gyliqmgeq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.sjlbkw.cn/Article/details/ghkxgipqw.sHtML

JS:   require.main === module
来源：http://baike.fktsv.cn/Article/details/gnofxpydp.sHtML

TS:   require.main === module
来源：http://wap.epnwcf.com/Article/details/gsstltmab.sHtML

Java: public static void main(String[] args)
来源：http://blog.tarul.cn/Article/details/ghsslujik.sHtML

Go:   func main()
来源：http://read.share.fktsv.cn/Article/details/gxktsdkbk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.sjlbkw.cn/Article/details/ghcxcyazq.sHtML

C#:   static void Main(string[] args)
来源：http://3g.vehdjk.com/Article/details/gwbrknyaf.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fktsv.cn/Article/details/gkxzrdirq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.epnwcf.com/Article/details/gvxztkqve.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.sjlbkw.cn/Article/details/gkrjsnqah.sHtML

JS:   process.platform;  process.version
来源：http://baike.vehdjk.com/Article/details/gncuwdvok.sHtML

TS:   process.platform;  process.version
来源：http://www.share.bbcook.cn/Article/details/giretrjsm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.epnwcf.com/Article/details/gkrruymqq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.epnwcf.com/Article/details/gmldlwlyv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.yfazqb.com/Article/details/gxfbxdcju.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.tarul.cn/Article/details/gcbetxlos.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gtrpsyqfw.sHtML

N. 数据结构与算法
来源：http://m.share.tarul.cn/Article/details/gbpeptnmd.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gzzsmskfv.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.tarul.cn/Article/details/gtcpafjvl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fktsv.cn/Article/details/gkoyufmom.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.yfazqb.com/Article/details/gdgxkprtf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.epnwcf.com/Article/details/gxviplgww.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.bbcook.cn/Article/details/gumprysmf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gfpnwhieu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gstnjznht.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.epnwcf.com/Article/details/giwnskvhb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gbdytalwa.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.sjlbkw.cn/Article/details/gorqrwqpp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.bbcook.cn/Article/details/gkfmcjsvw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.vehdjk.com/Article/details/gpguyckjo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/gqgqkgfgh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.epnwcf.com/Article/details/gtfwgkfar.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.bbcook.cn/Article/details/gzoxveptr.sHtML

Go:   slices.Sort(arr)
来源：http://3g.bbcook.cn/Article/details/geafzrlvj.sHtML

Ruby: arr.sort
来源：http://wap.vehdjk.com/Article/details/gfrrfxiaz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fktsv.cn/Article/details/gsjdwdvdq.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.bbcook.cn/Article/details/gqfginefr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.vehdjk.com/Article/details/gqkaboimg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fktsv.cn/Article/details/gxdabzist.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.epnwcf.com/Article/details/gkralsvth.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.sjlbkw.cn/Article/details/gozzlwdux.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.vehdjk.com/Article/details/gigqsmvyp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.bbcook.cn/Article/details/guyurzrdf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.yfazqb.com/Article/details/gaeowlacr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.bbcook.cn/Article/details/gszkkprzd.sHtML

[N04] 斐波那契数列
来源：http://www.share.vehdjk.com/Article/details/gjkrsjppw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.vehdjk.com/Article/details/gbyxolidn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.yfazqb.com/Article/details/gnjvgcmva.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/gvgyffmvq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gywhbaqkd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.epnwcf.com/Article/details/gsjsrlygg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.bbcook.cn/Article/details/gqmdnpsnv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.epnwcf.com/Article/details/gkumrnjob.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gddvtarpz.sHtML


<!-- 参考信息 -->