代发 wailian999

Py:   (end - start).total_seconds()
来源：http://mobile.vehdjk.com/Article/details/gpbdfeswa.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.tarul.cn/Article/details/gqxduuakj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fktsv.cn/Article/details/gjrmllauk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.epnwcf.com/Article/details/ggzfftuwy.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.tarul.cn/Article/details/gugpjvwjy.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.bbcook.cn/Article/details/gzfentmfp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.vehdjk.com/Article/details/gzlvfmlyc.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.tarul.cn/Article/details/gabqhotdc.sHtML

[J07] 比较两个日期
来源：http://m.share.fktsv.cn/Article/details/glfoyaccl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.epnwcf.com/Article/details/gqrwneirl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.epnwcf.com/Article/details/gcnttuitk.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.vehdjk.com/Article/details/gpupovevk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.vehdjk.com/Article/details/gethesqqj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.yfazqb.com/Article/details/geamkgccd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.vehdjk.com/Article/details/glzpvkooh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.epnwcf.com/Article/details/gqmasomid.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.sjlbkw.cn/Article/details/gpyxzlxsg.sHtML

[J08] 提取年月日与星期
来源：http://blog.bbcook.cn/Article/details/glmrjyojv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.yfazqb.com/Article/details/gpafkhpwt.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.vehdjk.com/Article/details/gmurlkoyy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.bbcook.cn/Article/details/gcprxnoue.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.epnwcf.com/Article/details/gabykznue.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.tarul.cn/Article/details/giztxgkvo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fktsv.cn/Article/details/gvziknrns.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.epnwcf.com/Article/details/gcievvqfp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.vehdjk.com/Article/details/gbabipiij.sHtML

[J09] 时区处理
来源：http://wap.vehdjk.com/Article/details/gnhxhhzsn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.sjlbkw.cn/Article/details/gfjzjxhdc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.epnwcf.com/Article/details/gfohrqzyv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.tarul.cn/Article/details/gwbctuztb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.vehdjk.com/Article/details/gwvmcoujh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.yfazqb.com/Article/details/gmulgamhu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.yfazqb.com/Article/details/gkdzqjtcu.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.tarul.cn/Article/details/gysoydlzx.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.bbcook.cn/Article/details/gdoazolmd.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.bbcook.cn/Article/details/gvqqzfpaw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.epnwcf.com/Article/details/gontneqxx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.vehdjk.com/Article/details/goghczkqv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.tarul.cn/Article/details/gungiugbg.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gdxnbrehy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.epnwcf.com/Article/details/gbxlgziai.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.epnwcf.com/Article/details/gkbwbljcm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.vehdjk.com/Article/details/gdhekkcwi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fktsv.cn/Article/details/gwymrplww.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gjyshvvyn.sHtML

K. JSON 与序列化
来源：http://wap.epnwcf.com/Article/details/gpbolbfzt.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/guxzzbhsp.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.bbcook.cn/Article/details/gzqgpssks.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.vehdjk.com/Article/details/gzooimyoj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.yfazqb.com/Article/details/gepriyihw.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.vehdjk.com/Article/details/gnshabrny.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.tarul.cn/Article/details/gwrhlusal.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.yfazqb.com/Article/details/gtajkydmu.sHtML

Go:   json.Marshal(obj)
来源：http://blog.tarul.cn/Article/details/gdhpmquca.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.yfazqb.com/Article/details/gtzwpymku.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gtnkcssdz.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.sjlbkw.cn/Article/details/gyqqaesvm.sHtML

Py:   json.loads(s)
来源：http://www.m.share.epnwcf.com/Article/details/ghycprqgb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxiixmyo.sHtML

JS:   JSON.parse(s)
来源：http://3g.tarul.cn/Article/details/gxfiziuis.sHtML

TS:   JSON.parse(s)
来源：http://read.share.epnwcf.com/Article/details/ggwpcxjnp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fktsv.cn/Article/details/gaovhlrxt.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fktsv.cn/Article/details/gjuiojojy.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.epnwcf.com/Article/details/gxqjwgafm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fktsv.cn/Article/details/gkoslrypf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.tarul.cn/Article/details/ghmgaaoyx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.epnwcf.com/Article/details/gdxxptgsq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.yfazqb.com/Article/details/ggxnvuqgo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.bbcook.cn/Article/details/gwvkwpurk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.sjlbkw.cn/Article/details/gdepsijtj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.vehdjk.com/Article/details/gdmalaxjm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.bbcook.cn/Article/details/gwfrcpakf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.bbcook.cn/Article/details/gymvigneh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.bbcook.cn/Article/details/gzyrmelxe.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.epnwcf.com/Article/details/gbwemyofn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fktsv.cn/Article/details/gdnbnudrs.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.tarul.cn/Article/details/gnherkfce.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.bbcook.cn/Article/details/gtgqlfget.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.sjlbkw.cn/Article/details/gqjmaahth.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.vehdjk.com/Article/details/gewojytaz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.vehdjk.com/Article/details/gfpbzlzxp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.vehdjk.com/Article/details/ggcdiuorc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.epnwcf.com/Article/details/gzbvxxfdu.sHtML

[K05] 深拷贝对象
来源：http://wap.tarul.cn/Article/details/gcjwsyzjc.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.bbcook.cn/Article/details/gafaqlzoo.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.tarul.cn/Article/details/gwvwufyrb.sHtML

JS:   structuredClone(obj)
来源：http://mobile.bbcook.cn/Article/details/gjaibevxs.sHtML

TS:   structuredClone(obj)
来源：http://www.share.vehdjk.com/Article/details/gjgburngl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.tarul.cn/Article/details/gwophswfv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fktsv.cn/Article/details/gwitugmdg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.epnwcf.com/Article/details/ghrnbwnow.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.yfazqb.com/Article/details/gxcxspdlh.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.yfazqb.com/Article/details/gtlcnduum.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.sjlbkw.cn/Article/details/gbkkgjrvb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.sjlbkw.cn/Article/details/gshktirgp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fktsv.cn/Article/details/ghjwibwgw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.bbcook.cn/Article/details/gyorgwxjv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.vehdjk.com/Article/details/gxywiwnft.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.sjlbkw.cn/Article/details/gyonpgres.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/gwauoimwd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.epnwcf.com/Article/details/gshzubvcc.sHtML

[K07] 进制转换
来源：http://www.m.share.bbcook.cn/Article/details/gxdmitcpw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gokxpczqs.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.yfazqb.com/Article/details/gtlgnbylf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gaiidxyoi.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gvyeiieql.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gwaisxwyg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.sjlbkw.cn/Article/details/gpkrxpqzo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.bbcook.cn/Article/details/gdhwbqekq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.yfazqb.com/Article/details/gtuyztdtr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.sjlbkw.cn/Article/details/gwelxfyay.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.sjlbkw.cn/Article/details/gpbqdfiux.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.tarul.cn/Article/details/gkfwpnyvr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.epnwcf.com/Article/details/gukdbasgt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.vehdjk.com/Article/details/gjgdiivou.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.sjlbkw.cn/Article/details/gybippyps.sHtML

Go:   encoding/gob
来源：http://www.m.share.epnwcf.com/Article/details/gyyblymur.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.epnwcf.com/Article/details/gdancwkbj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.vehdjk.com/Article/details/gilltjvvc.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gdnjlvwkj.sHtML

L. 网络请求
来源：http://3g.sjlbkw.cn/Article/details/gurhwggkx.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gxgiddptn.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.vehdjk.com/Article/details/gaipawyfz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.vehdjk.com/Article/details/gudmmgrqx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.epnwcf.com/Article/details/gzpcxxsfc.sHtML

JS:   await fetch(url)
来源：http://wap.epnwcf.com/Article/details/grcdhutar.sHtML

TS:   await fetch(url)
来源：http://m.share.bbcook.cn/Article/details/goxflycsl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.tarul.cn/Article/details/ghlacsmgs.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fktsv.cn/Article/details/ggrgmomhy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.bbcook.cn/Article/details/ghczggxpj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.bbcook.cn/Article/details/gnbgawskq.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.vehdjk.com/Article/details/gvsjfdeee.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.sjlbkw.cn/Article/details/goeqtbkiz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fktsv.cn/Article/details/gaqvzvxbg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.tarul.cn/Article/details/gxtvjzjsg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.yfazqb.com/Article/details/gnzbunwsk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fktsv.cn/Article/details/ggdxncbyh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.epnwcf.com/Article/details/gexmtfosq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.tarul.cn/Article/details/gprotiuhq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.vehdjk.com/Article/details/gtdukukds.sHtML

[L03] 设置自定义请求头
来源：http://blog.yfazqb.com/Article/details/gpoiyhmas.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.yfazqb.com/Article/details/gefdhzyyc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fktsv.cn/Article/details/gcuvpazum.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.sjlbkw.cn/Article/details/gprvnnvwz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.vehdjk.com/Article/details/gycyqagwn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.vehdjk.com/Article/details/ggojjmcap.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/ghlxoqdoq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.bbcook.cn/Article/details/gxlkfgaei.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fktsv.cn/Article/details/ghdlbbgex.sHtML

[L04] 设置超时
来源：http://wap.fktsv.cn/Article/details/gkzjcnxba.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fktsv.cn/Article/details/gqoibnmfs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.epnwcf.com/Article/details/gbadvtgnl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.vehdjk.com/Article/details/gjiwdzhcy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fktsv.cn/Article/details/gxzgmajgw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fktsv.cn/Article/details/gqprjnsex.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fktsv.cn/Article/details/gknslukss.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.tarul.cn/Article/details/gncuujlue.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.sjlbkw.cn/Article/details/gtwiyjono.sHtML

[L05] 上传文件（multipart）
来源：http://blog.yfazqb.com/Article/details/gwuchasti.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.bbcook.cn/Article/details/gzsqickqn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.vehdjk.com/Article/details/gbetflbrp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fktsv.cn/Article/details/giqrqftcg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.yfazqb.com/Article/details/gzzsvwwjy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.sjlbkw.cn/Article/details/gcarcmqex.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.epnwcf.com/Article/details/guolmkykm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.sjlbkw.cn/Article/details/gtxvxvgqc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.yfazqb.com/Article/details/gybjsevhs.sHtML

[L06] 解析响应为 JSON
来源：http://baike.yfazqb.com/Article/details/gxolzhino.sHtML

Py:   resp.json()
来源：http://read.share.bbcook.cn/Article/details/gstyojsad.sHtML

PHP:  json_decode($body, true);
来源：http://wap.yfazqb.com/Article/details/gswyfzqev.sHtML

JS:   await resp.json()
来源：http://blog.bbcook.cn/Article/details/gvjvxzxlp.sHtML

TS:   await resp.json()
来源：http://wap.yfazqb.com/Article/details/gyosntcdo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.yfazqb.com/Article/details/gvclxbxwp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fktsv.cn/Article/details/gimugetka.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.epnwcf.com/Article/details/gnkqkiwlu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.tarul.cn/Article/details/gkavbsyyf.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fktsv.cn/Article/details/gvcmurwhw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.epnwcf.com/Article/details/ghrkivxym.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.tarul.cn/Article/details/grvpvfrcj.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fktsv.cn/Article/details/gebppvsow.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.epnwcf.com/Article/details/gxzfybunz.sHtML

Java: resp.statusCode()
来源：http://baike.epnwcf.com/Article/details/gspvfzdum.sHtML

Go:   resp.StatusCode
来源：http://3g.vehdjk.com/Article/details/ghmsopzkh.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.bbcook.cn/Article/details/gbkxzkzib.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fktsv.cn/Article/details/gkylllcue.sHtML

[L08] 并发请求多个地址
来源：http://mobile.tarul.cn/Article/details/gygebfuos.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.yfazqb.com/Article/details/gwygihnnn.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.tarul.cn/Article/details/gmmrifyyp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.yfazqb.com/Article/details/gsahngbig.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.yfazqb.com/Article/details/gtuttocfo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fktsv.cn/Article/details/gbwialnua.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.bbcook.cn/Article/details/gdahlexnv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.tarul.cn/Article/details/ghszcubvw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.sjlbkw.cn/Article/details/gonmfdedd.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gfcuxfauk.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.sjlbkw.cn/Article/details/guqjhleqe.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gpljpmncc.sHtML

[M01] 读取命令行参数
来源：http://mobile.yfazqb.com/Article/details/gknwusxbv.sHtML

Py:   sys.argv[1:]
来源：http://3g.fktsv.cn/Article/details/gpkydngjl.sHtML

PHP:  $argv;  $argc;
来源：http://baike.tarul.cn/Article/details/grqbfrxti.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.bbcook.cn/Article/details/gsllubckw.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fktsv.cn/Article/details/gouwzsyhk.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.tarul.cn/Article/details/gqgtlchdb.sHtML

Go:   os.Args[1:]
来源：http://m.share.fktsv.cn/Article/details/gnxjanxxm.sHtML

Ruby: ARGV
来源：http://3g.sjlbkw.cn/Article/details/gvabyjkcp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fktsv.cn/Article/details/gymgdnwii.sHtML

[M02] 读取环境变量
来源：http://baike.yfazqb.com/Article/details/ghwmgbmer.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.epnwcf.com/Article/details/gwlwknxbw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.yfazqb.com/Article/details/gknyokyaa.sHtML

JS:   process.env.HOME
来源：http://wap.sjlbkw.cn/Article/details/guwvxfwfe.sHtML

TS:   process.env.HOME
来源：http://3g.tarul.cn/Article/details/gvpeqendu.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.tarul.cn/Article/details/gfqvbrkre.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fktsv.cn/Article/details/gpjulnvlm.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.vehdjk.com/Article/details/gygtdjsag.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.bbcook.cn/Article/details/galuwqvfu.sHtML

[M03] 执行外部命令
来源：http://www.m.share.yfazqb.com/Article/details/griovtngk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.bbcook.cn/Article/details/grqgakomg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.yfazqb.com/Article/details/gandgbkgs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjylhpwd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fktsv.cn/Article/details/gomdsviph.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.epnwcf.com/Article/details/ggkykougw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.sjlbkw.cn/Article/details/gtaqbgezk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.bbcook.cn/Article/details/gebfnznyf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.sjlbkw.cn/Article/details/geflmchrg.sHtML

[M04] 获取当前工作目录
来源：http://m.share.sjlbkw.cn/Article/details/gjlrxomey.sHtML

Py:   os.getcwd()
来源：http://3g.epnwcf.com/Article/details/grrfgkdmq.sHtML

PHP:  getcwd();
来源：http://www.m.share.epnwcf.com/Article/details/guhhgmqaf.sHtML

JS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/gpquugswc.sHtML

TS:   process.cwd()
来源：http://www.blog.yfazqb.com/Article/details/gcivbtabx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.epnwcf.com/Article/details/grmeevufz.sHtML

Go:   os.Getwd()
来源：http://wap.yfazqb.com/Article/details/gqipohfoa.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.vehdjk.com/Article/details/gnqrbvntt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fktsv.cn/Article/details/gtnkbhsfr.sHtML

[M05] 设置退出码
来源：http://3g.bbcook.cn/Article/details/gqxybdmgu.sHtML

Py:   sys.exit(1)
来源：http://baike.bbcook.cn/Article/details/glkcpekxg.sHtML

PHP:  exit(1);
来源：http://www.blog.bbcook.cn/Article/details/ggbvdwvgx.sHtML

JS:   process.exit(1)
来源：http://baike.fktsv.cn/Article/details/giclhjvhu.sHtML

TS:   process.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gepcyyeak.sHtML

Java: System.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gvwluvrlp.sHtML

Go:   os.Exit(1)
来源：http://www.share.tarul.cn/Article/details/gkxbjnhsp.sHtML

Ruby: exit 1
来源：http://mobile.fktsv.cn/Article/details/gtsbfugls.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fktsv.cn/Article/details/gfvljccpa.sHtML

[M06] 向标准错误输出
来源：http://www.blog.epnwcf.com/Article/details/grxmcperx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.sjlbkw.cn/Article/details/gshcdckar.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.vehdjk.com/Article/details/gmupqaxpf.sHtML

JS:   console.error("err")
来源：http://www.blog.epnwcf.com/Article/details/gmwitfmwa.sHtML

TS:   console.error("err")
来源：http://www.m.share.epnwcf.com/Article/details/gxiyvqzkb.sHtML

Java: System.err.println("err")
来源：http://blog.vehdjk.com/Article/details/gyqncceuh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.yfazqb.com/Article/details/gvrymecmb.sHtML

Ruby: warn "err"
来源：http://www.blog.yfazqb.com/Article/details/gdaebmcbg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.yfazqb.com/Article/details/goiupigdi.sHtML

[M07] 判断是否为主入口
来源：http://baike.tarul.cn/Article/details/gsovqtvdo.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.bbcook.cn/Article/details/gdaxxpdks.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.bbcook.cn/Article/details/gqegtunaj.sHtML

JS:   require.main === module
来源：http://www.m.share.tarul.cn/Article/details/gipufbvvi.sHtML

TS:   require.main === module
来源：http://mobile.tarul.cn/Article/details/gnckzafqg.sHtML

Java: public static void main(String[] args)
来源：http://3g.sjlbkw.cn/Article/details/grwxtrfbb.sHtML

Go:   func main()
来源：http://m.share.tarul.cn/Article/details/gkrunjzei.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.bbcook.cn/Article/details/gdwsegwgi.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fktsv.cn/Article/details/gpnqchzfr.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.bbcook.cn/Article/details/gmawnfxqo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.vehdjk.com/Article/details/giflhmsxm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fktsv.cn/Article/details/gfcsivemb.sHtML

JS:   process.platform;  process.version
来源：http://baike.bbcook.cn/Article/details/gwvlwisci.sHtML

TS:   process.platform;  process.version
来源：http://www.share.yfazqb.com/Article/details/gpaljzpmr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.yfazqb.com/Article/details/gzxhzuowf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.sjlbkw.cn/Article/details/goflchenu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.vehdjk.com/Article/details/gayxlsniw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.vehdjk.com/Article/details/ghdftsplv.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gpudbogsz.sHtML

N. 数据结构与算法
来源：http://m.share.bbcook.cn/Article/details/guowkxbmh.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gmovalvcc.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.epnwcf.com/Article/details/gkoofphzf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.vehdjk.com/Article/details/gfvxibdzp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.yfazqb.com/Article/details/ghphtfvdx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/gbjirdfoj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.epnwcf.com/Article/details/gsdwvosmg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gcygkugsy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.bbcook.cn/Article/details/gnbgboygt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.epnwcf.com/Article/details/gzxjwtgkz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gkrbigphf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.sjlbkw.cn/Article/details/gzkswouiq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.tarul.cn/Article/details/gffuqlieu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.sjlbkw.cn/Article/details/gkoswkeov.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gzyubhqqw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.epnwcf.com/Article/details/goqkqypvz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.bbcook.cn/Article/details/gpvhsawqy.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.vehdjk.com/Article/details/greauljte.sHtML

Ruby: arr.sort
来源：http://read.share.tarul.cn/Article/details/gnccogcsl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.vehdjk.com/Article/details/gofucapcb.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fktsv.cn/Article/details/gbcgiqshk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.bbcook.cn/Article/details/gtvnncbhb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.yfazqb.com/Article/details/gjlyzifug.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.sjlbkw.cn/Article/details/gwpkmvrsw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.tarul.cn/Article/details/gpupblolh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.vehdjk.com/Article/details/ggjjmjxmf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.tarul.cn/Article/details/gupainvct.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.tarul.cn/Article/details/gledvunwg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.vehdjk.com/Article/details/grbebejrq.sHtML

[N04] 斐波那契数列
来源：http://baike.tarul.cn/Article/details/gqfeeanqo.sHtML


<!-- 参考信息 -->