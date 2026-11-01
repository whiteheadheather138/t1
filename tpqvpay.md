代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.sjlbkw.cn/Article/details/gcnqwzemz.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.yfazqb.com/Article/details/guhwkcibf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.fktsv.cn/Article/details/gefqdmtpg.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.bbcook.cn/Article/details/gcbnbbmdc.sHtML

[J07] 比较两个日期
来源：http://m.share.yfazqb.com/Article/details/gngxrpyrb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.tarul.cn/Article/details/gcehwqpll.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.fktsv.cn/Article/details/gclhtyclm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.yfazqb.com/Article/details/glkpldayk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.epnwcf.com/Article/details/gohljjtbt.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.sjlbkw.cn/Article/details/gmkaldcba.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.bbcook.cn/Article/details/gkslllbcs.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.tarul.cn/Article/details/gyvcupyzr.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.vehdjk.com/Article/details/gtgjnxqqt.sHtML

[J08] 提取年月日与星期
来源：http://wap.epnwcf.com/Article/details/guloiaacm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.tarul.cn/Article/details/gpqtjmkyh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.yfazqb.com/Article/details/gzpjagifr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.fktsv.cn/Article/details/gejrdbupc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.bbcook.cn/Article/details/gqcgbpkwm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.tarul.cn/Article/details/gmfhphrli.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.yfazqb.com/Article/details/gutppsejd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.tarul.cn/Article/details/gxzvsdojz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.yfazqb.com/Article/details/girgrstnn.sHtML

[J09] 时区处理
来源：http://read.share.sjlbkw.cn/Article/details/guxgzgnsh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.sjlbkw.cn/Article/details/gypudrgco.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.sjlbkw.cn/Article/details/gkgzadmnz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.bbcook.cn/Article/details/gfbwwygej.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.tarul.cn/Article/details/gikbsmxzy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.epnwcf.com/Article/details/gxxczyzbx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.bbcook.cn/Article/details/gmeunwdil.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.vehdjk.com/Article/details/grohjkjss.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fktsv.cn/Article/details/gxzmwuoxa.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.vehdjk.com/Article/details/gktmwolgn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.vehdjk.com/Article/details/ghjtcpvum.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.sjlbkw.cn/Article/details/gmmbttvll.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.sjlbkw.cn/Article/details/gvfisfcsk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.yfazqb.com/Article/details/grufrijmq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.epnwcf.com/Article/details/gbjljmspy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.vehdjk.com/Article/details/gdppnbmif.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.vehdjk.com/Article/details/gupvzabha.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fktsv.cn/Article/details/gudykhyfz.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gmatbogma.sHtML

K. JSON 与序列化
来源：http://3g.sjlbkw.cn/Article/details/gmjhopowl.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gsfyhfhnu.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.vehdjk.com/Article/details/gjzgjjsog.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.bbcook.cn/Article/details/gyyojcmzx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.sjlbkw.cn/Article/details/gsqerqwty.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gefehbppb.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gjbgjoczz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.yfazqb.com/Article/details/gdogqjwwc.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gaupvqofy.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.tarul.cn/Article/details/glyiovcki.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.tarul.cn/Article/details/gjzyzwwal.sHtML

[K02] JSON 字符串转对象
来源：http://baike.yfazqb.com/Article/details/gbdyoxhih.sHtML

Py:   json.loads(s)
来源：http://wap.vehdjk.com/Article/details/gpbcztqrz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.yfazqb.com/Article/details/gzrjkecay.sHtML

JS:   JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/gvahjhcys.sHtML

TS:   JSON.parse(s)
来源：http://m.share.vehdjk.com/Article/details/gzrsbijpu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.sjlbkw.cn/Article/details/ghkwjrdng.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.tarul.cn/Article/details/gakpaohhc.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fktsv.cn/Article/details/gowkygqoz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.yfazqb.com/Article/details/gsmzczhsd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.sjlbkw.cn/Article/details/gmgssreru.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.epnwcf.com/Article/details/gdhvkupzy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fktsv.cn/Article/details/gsvcjglxh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.yfazqb.com/Article/details/gfpfgsqbk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.tarul.cn/Article/details/gmzvuodte.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gdurtofgj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fktsv.cn/Article/details/glmweiibh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.tarul.cn/Article/details/gpkcuytxl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fktsv.cn/Article/details/gcyorcheg.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.epnwcf.com/Article/details/gmvejhqpg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.tarul.cn/Article/details/gcllhigfu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.epnwcf.com/Article/details/gzomynrwl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fktsv.cn/Article/details/gtcdoeoru.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.vehdjk.com/Article/details/gyebsiepr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.vehdjk.com/Article/details/gujfivudl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.bbcook.cn/Article/details/gihaomegm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.vehdjk.com/Article/details/gitnkjnou.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.tarul.cn/Article/details/gvqvkdyhz.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.epnwcf.com/Article/details/gtudshqoa.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.yfazqb.com/Article/details/gwgkopvdd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.vehdjk.com/Article/details/ghvzkovba.sHtML

JS:   structuredClone(obj)
来源：http://www.share.sjlbkw.cn/Article/details/goyqeckag.sHtML

TS:   structuredClone(obj)
来源：http://www.share.epnwcf.com/Article/details/giedzzhlf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.sjlbkw.cn/Article/details/gjdpmjnnd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.vehdjk.com/Article/details/gfrcdidgr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fktsv.cn/Article/details/gsqqkkusi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.yfazqb.com/Article/details/gfymgujhl.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.yfazqb.com/Article/details/gfzdjmbpj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.yfazqb.com/Article/details/gytwjjgad.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.sjlbkw.cn/Article/details/goshvgwss.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.sjlbkw.cn/Article/details/glxnrzrxd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.epnwcf.com/Article/details/gpjsrzmng.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.yfazqb.com/Article/details/gohwmdnzv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.bbcook.cn/Article/details/gydvrczvl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/gdofvksur.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.bbcook.cn/Article/details/gzrxlpltw.sHtML

[K07] 进制转换
来源：http://www.m.share.epnwcf.com/Article/details/gddiltmgc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggikragjg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.epnwcf.com/Article/details/gfqmbjntx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gljlojxgm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gnficnpuj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/gzpcqdcal.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.sjlbkw.cn/Article/details/garqgdpen.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.tarul.cn/Article/details/gjmzvxwjg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gpocoatyo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.tarul.cn/Article/details/ggfjrxwqi.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gcfbpsbkz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.bbcook.cn/Article/details/gcoicavus.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.vehdjk.com/Article/details/ghqbuzsox.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fktsv.cn/Article/details/gogbjvsdk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.sjlbkw.cn/Article/details/glmdprncg.sHtML

Go:   encoding/gob
来源：http://www.blog.fktsv.cn/Article/details/gmowgucoh.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fktsv.cn/Article/details/gvmtsvclm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.tarul.cn/Article/details/gfebhiyds.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gejqxjmat.sHtML

L. 网络请求
来源：http://blog.epnwcf.com/Article/details/gogrztvqh.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/guhhkcmhj.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.tarul.cn/Article/details/gvfnkrdtv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.tarul.cn/Article/details/ghzatrugk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.tarul.cn/Article/details/gujgmoupv.sHtML

JS:   await fetch(url)
来源：http://blog.vehdjk.com/Article/details/gloqtwnlh.sHtML

TS:   await fetch(url)
来源：http://m.share.fktsv.cn/Article/details/glauggbsk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.tarul.cn/Article/details/gdvrbyrqv.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.yfazqb.com/Article/details/gnkpjslqw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.tarul.cn/Article/details/grfkrkutd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.sjlbkw.cn/Article/details/grnloxgdq.sHtML

[L02] 发送 POST JSON
来源：http://read.share.yfazqb.com/Article/details/gefocakag.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.tarul.cn/Article/details/gcosrqbnj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.vehdjk.com/Article/details/gtknymemi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.sjlbkw.cn/Article/details/gsuadewji.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.tarul.cn/Article/details/gskuryybn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.sjlbkw.cn/Article/details/guvvcchda.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.epnwcf.com/Article/details/geyvycimt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.sjlbkw.cn/Article/details/gbeiskmpx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.tarul.cn/Article/details/gtyapirqe.sHtML

[L03] 设置自定义请求头
来源：http://mobile.tarul.cn/Article/details/gjdrtumyq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.yfazqb.com/Article/details/gptaysujs.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.epnwcf.com/Article/details/grejielab.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.vehdjk.com/Article/details/gsyykjvot.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.sjlbkw.cn/Article/details/gqrrkxhii.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.sjlbkw.cn/Article/details/gonzrjlvt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.tarul.cn/Article/details/ggzdzcyfq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.vehdjk.com/Article/details/ggpfqfkrb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.bbcook.cn/Article/details/geucvswlf.sHtML

[L04] 设置超时
来源：http://wap.tarul.cn/Article/details/gsqaawrvz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.vehdjk.com/Article/details/gcullqkth.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.bbcook.cn/Article/details/gvwpqyawd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.vehdjk.com/Article/details/ghxicmjro.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.sjlbkw.cn/Article/details/ghajxuhrq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fktsv.cn/Article/details/gwtnuyqtp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fktsv.cn/Article/details/gxrtywcja.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.epnwcf.com/Article/details/gnujcgbse.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.yfazqb.com/Article/details/ghlyslnbt.sHtML

[L05] 上传文件（multipart）
来源：http://baike.yfazqb.com/Article/details/gspjombcg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.bbcook.cn/Article/details/gzptnttzk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.yfazqb.com/Article/details/gbhgyjacn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.tarul.cn/Article/details/gwrevoyus.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.bbcook.cn/Article/details/gowksrmue.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.sjlbkw.cn/Article/details/ghxtqbgze.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fktsv.cn/Article/details/guhrenesb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fktsv.cn/Article/details/gxxlovrjy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.bbcook.cn/Article/details/gnkagyzrp.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fktsv.cn/Article/details/gjqpaeawc.sHtML

Py:   resp.json()
来源：http://blog.bbcook.cn/Article/details/grxkcqchb.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.tarul.cn/Article/details/gqlqurpid.sHtML

JS:   await resp.json()
来源：http://mobile.sjlbkw.cn/Article/details/gbrbthngv.sHtML

TS:   await resp.json()
来源：http://blog.sjlbkw.cn/Article/details/ghiucljzk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.yfazqb.com/Article/details/gczpklgmj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.yfazqb.com/Article/details/geqesqicw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.bbcook.cn/Article/details/ghqqoxfam.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.bbcook.cn/Article/details/gewceilub.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.tarul.cn/Article/details/gisgrbwzz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fktsv.cn/Article/details/gyydlaitl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.vehdjk.com/Article/details/gssvcjdgh.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.yfazqb.com/Article/details/guudhknxs.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.sjlbkw.cn/Article/details/gdipzvsrn.sHtML

Java: resp.statusCode()
来源：http://3g.fktsv.cn/Article/details/gugitjgih.sHtML

Go:   resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/gecsprtir.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.bbcook.cn/Article/details/gqvcojyxe.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.tarul.cn/Article/details/gjiltraua.sHtML

[L08] 并发请求多个地址
来源：http://blog.yfazqb.com/Article/details/gtxoojwjx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.vehdjk.com/Article/details/gelbswihd.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fktsv.cn/Article/details/gylpzaqdh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.sjlbkw.cn/Article/details/gcyyxxowv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/gddnlczto.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fktsv.cn/Article/details/gtelmwhjc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.bbcook.cn/Article/details/gwofagozq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.sjlbkw.cn/Article/details/gqkhrublu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fktsv.cn/Article/details/gxfnckopq.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gukatygcf.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.epnwcf.com/Article/details/gjmgoovzo.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gasobgkep.sHtML

[M01] 读取命令行参数
来源：http://read.share.fktsv.cn/Article/details/gblkbwndq.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.vehdjk.com/Article/details/guexxvgtf.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fktsv.cn/Article/details/gbpmthjjy.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.yfazqb.com/Article/details/gzfzuiwoa.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.yfazqb.com/Article/details/gfqowljtw.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.sjlbkw.cn/Article/details/ggatkxifc.sHtML

Go:   os.Args[1:]
来源：http://3g.tarul.cn/Article/details/gzsmhabup.sHtML

Ruby: ARGV
来源：http://www.share.bbcook.cn/Article/details/gmeihjtni.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.yfazqb.com/Article/details/gbjwmhuga.sHtML

[M02] 读取环境变量
来源：http://m.share.vehdjk.com/Article/details/gllataxfl.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.tarul.cn/Article/details/gkeqtahdn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.yfazqb.com/Article/details/grmxnvlee.sHtML

JS:   process.env.HOME
来源：http://m.share.fktsv.cn/Article/details/gvrdkfiin.sHtML

TS:   process.env.HOME
来源：http://wap.epnwcf.com/Article/details/gdjarhnew.sHtML

Java: System.getenv("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gdqjyvxlw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fktsv.cn/Article/details/gzrsgurrs.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.bbcook.cn/Article/details/gizglgjvd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.yfazqb.com/Article/details/ggczcojdm.sHtML

[M03] 执行外部命令
来源：http://wap.vehdjk.com/Article/details/glkdcqohv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.vehdjk.com/Article/details/gtvpkjaxx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fktsv.cn/Article/details/gddxgyrnt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.vehdjk.com/Article/details/gakperuik.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.tarul.cn/Article/details/gmkekgsox.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.tarul.cn/Article/details/gioinjjox.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.sjlbkw.cn/Article/details/ggeltyhry.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.yfazqb.com/Article/details/graxlkmkw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.vehdjk.com/Article/details/gadnhcexl.sHtML

[M04] 获取当前工作目录
来源：http://m.share.sjlbkw.cn/Article/details/gethgniqu.sHtML

Py:   os.getcwd()
来源：http://www.blog.tarul.cn/Article/details/gzirmgzoy.sHtML

PHP:  getcwd();
来源：http://www.m.share.fktsv.cn/Article/details/gkiaazbod.sHtML

JS:   process.cwd()
来源：http://baike.vehdjk.com/Article/details/gwutxomdj.sHtML

TS:   process.cwd()
来源：http://m.share.vehdjk.com/Article/details/gsnqhnilj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.vehdjk.com/Article/details/gmhbkgkzd.sHtML

Go:   os.Getwd()
来源：http://www.m.share.yfazqb.com/Article/details/gkgldwoyy.sHtML

Ruby: Dir.pwd
来源：http://blog.vehdjk.com/Article/details/gnmewbwmb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.tarul.cn/Article/details/gmisykcci.sHtML

[M05] 设置退出码
来源：http://www.blog.sjlbkw.cn/Article/details/gbsrklftg.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzurzmtj.sHtML

PHP:  exit(1);
来源：http://www.m.share.yfazqb.com/Article/details/gpmyxaqoa.sHtML

JS:   process.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gtoyjnrxg.sHtML

TS:   process.exit(1)
来源：http://baike.epnwcf.com/Article/details/ghmspuqad.sHtML

Java: System.exit(1)
来源：http://wap.yfazqb.com/Article/details/gtcqiputy.sHtML

Go:   os.Exit(1)
来源：http://mobile.epnwcf.com/Article/details/gymyvzrnx.sHtML

Ruby: exit 1
来源：http://mobile.epnwcf.com/Article/details/gsadjxwys.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.vehdjk.com/Article/details/ggrxxevjz.sHtML

[M06] 向标准错误输出
来源：http://m.share.vehdjk.com/Article/details/ghjnhglkl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.sjlbkw.cn/Article/details/goesuhlvk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.vehdjk.com/Article/details/gnwvyiqgp.sHtML

JS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/ghbuksifr.sHtML

TS:   console.error("err")
来源：http://m.share.fktsv.cn/Article/details/ghqcfbevy.sHtML

Java: System.err.println("err")
来源：http://m.share.yfazqb.com/Article/details/gdgjizois.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.sjlbkw.cn/Article/details/gihxffbym.sHtML

Ruby: warn "err"
来源：http://3g.epnwcf.com/Article/details/gwudibjmx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.bbcook.cn/Article/details/gmsizvfsb.sHtML

[M07] 判断是否为主入口
来源：http://baike.bbcook.cn/Article/details/gtghkwdvb.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcdcwivx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.bbcook.cn/Article/details/gmstngpui.sHtML

JS:   require.main === module
来源：http://mobile.yfazqb.com/Article/details/geymidpej.sHtML

TS:   require.main === module
来源：http://mobile.vehdjk.com/Article/details/gpvsvgkun.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fktsv.cn/Article/details/grmezgyzh.sHtML

Go:   func main()
来源：http://read.share.sjlbkw.cn/Article/details/gcqyznxir.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.vehdjk.com/Article/details/gevhqvsft.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.bbcook.cn/Article/details/guqyveooj.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.tarul.cn/Article/details/gwkodsiqo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fktsv.cn/Article/details/gwvfwpbqx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.vehdjk.com/Article/details/guthrjyjt.sHtML

JS:   process.platform;  process.version
来源：http://wap.tarul.cn/Article/details/gwewudtfi.sHtML

TS:   process.platform;  process.version
来源：http://www.share.tarul.cn/Article/details/gqdrtwtxs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.vehdjk.com/Article/details/gxorxxypd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.epnwcf.com/Article/details/giukspzow.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.epnwcf.com/Article/details/gltnmmydj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fktsv.cn/Article/details/gbzwxgmhd.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gnpzwasfx.sHtML

N. 数据结构与算法
来源：http://wap.tarul.cn/Article/details/geglzqslc.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gkidywyxe.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.epnwcf.com/Article/details/griwwnhsz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.bbcook.cn/Article/details/gjkjvouao.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fktsv.cn/Article/details/gxeiluvpx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.tarul.cn/Article/details/gobnnahga.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/guxulppov.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcullzvmk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.yfazqb.com/Article/details/gxewophtj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.yfazqb.com/Article/details/geqpavwjy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.yfazqb.com/Article/details/gwnlhrwqg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.epnwcf.com/Article/details/gthgvbtis.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.sjlbkw.cn/Article/details/gaflzqgpj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/ggyfqqbxv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gtrxcanbs.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.tarul.cn/Article/details/gpnokteng.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.tarul.cn/Article/details/gbgeusura.sHtML

Go:   slices.Sort(arr)
来源：http://3g.tarul.cn/Article/details/gpinrzfnc.sHtML

Ruby: arr.sort
来源：http://3g.yfazqb.com/Article/details/goghmlofq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fktsv.cn/Article/details/gklocswne.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fktsv.cn/Article/details/gggbeodoj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.vehdjk.com/Article/details/gvyjjxxdl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.bbcook.cn/Article/details/gqspzudhp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.epnwcf.com/Article/details/gzkszcwkb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.vehdjk.com/Article/details/geicapyed.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.epnwcf.com/Article/details/gmkxqbusw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.sjlbkw.cn/Article/details/gcmviqnfk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.epnwcf.com/Article/details/gvqczbwfh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.epnwcf.com/Article/details/gprjlmhnu.sHtML

[N04] 斐波那契数列
来源：http://m.share.vehdjk.com/Article/details/gbcgwvnkv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.sjlbkw.cn/Article/details/glvbensxe.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.yfazqb.com/Article/details/gzinmqbuj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.vehdjk.com/Article/details/gaaibvmle.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.bbcook.cn/Article/details/ggphugaaw.sHtML


<!-- 参考信息 -->