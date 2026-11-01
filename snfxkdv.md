代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.sjlbkw.cn/Article/details/gzbmpiqud.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.tarul.cn/Article/details/ghfyvafsz.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.fktsv.cn/Article/details/gaoocbdqu.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.sjlbkw.cn/Article/details/gdrklcqdx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.vehdjk.com/Article/details/gmiyfglei.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.vehdjk.com/Article/details/gnizzhhby.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.epnwcf.com/Article/details/gftefupcf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.tarul.cn/Article/details/gthdfkxzk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.vehdjk.com/Article/details/gqtvjyoeu.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.epnwcf.com/Article/details/gqdsrgged.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.tarul.cn/Article/details/gcaidcsoz.sHtML

[J06] 计算两时间之差
来源：http://baike.epnwcf.com/Article/details/gjqsulmuv.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.bbcook.cn/Article/details/gpkbbbmmb.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.yfazqb.com/Article/details/glowmyele.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.tarul.cn/Article/details/gasnlidwz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.tarul.cn/Article/details/gqdltcrde.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.epnwcf.com/Article/details/goljibgtl.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.tarul.cn/Article/details/gvtllawtr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.tarul.cn/Article/details/gulinaqbe.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.sjlbkw.cn/Article/details/gzrjsxvuo.sHtML

[J07] 比较两个日期
来源：http://www.m.share.vehdjk.com/Article/details/gknxcykzy.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/gmpoocupv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.bbcook.cn/Article/details/gaokrfton.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.tarul.cn/Article/details/gomxhkxwz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.tarul.cn/Article/details/gqhdqsiou.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.tarul.cn/Article/details/gkucrhgsn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.vehdjk.com/Article/details/gjcvzmmiq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.epnwcf.com/Article/details/glmjhpvod.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.sjlbkw.cn/Article/details/gcygflxuy.sHtML

[J08] 提取年月日与星期
来源：http://www.share.bbcook.cn/Article/details/ghacfhndt.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.fktsv.cn/Article/details/gggvtzsvz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.tarul.cn/Article/details/gwjjpruzn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.epnwcf.com/Article/details/glygmhodt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.sjlbkw.cn/Article/details/gurghntxc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fktsv.cn/Article/details/gingejqpq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.epnwcf.com/Article/details/geiqchfjl.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.epnwcf.com/Article/details/gjhgdymaz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.yfazqb.com/Article/details/gnbndjgnf.sHtML

[J09] 时区处理
来源：http://www.blog.tarul.cn/Article/details/gnlaoizgo.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.vehdjk.com/Article/details/gscsuafua.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.tarul.cn/Article/details/guafadoqe.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.tarul.cn/Article/details/gsbjtnujn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fktsv.cn/Article/details/gmfcvuknj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.vehdjk.com/Article/details/gmclqnqxe.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.epnwcf.com/Article/details/gjtnynncm.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.vehdjk.com/Article/details/gpiswtfow.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.sjlbkw.cn/Article/details/ggewxkzgi.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.tarul.cn/Article/details/gxjgraojq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.vehdjk.com/Article/details/guifvcwgi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.vehdjk.com/Article/details/gzgdnybjw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.vehdjk.com/Article/details/gnuebcgbk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fktsv.cn/Article/details/gmzcwocua.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.tarul.cn/Article/details/gqzvdnvtk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.vehdjk.com/Article/details/gthaxvqgc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.yfazqb.com/Article/details/gypvhdtkw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.tarul.cn/Article/details/gkdzivadd.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/ggqgjheci.sHtML

K. JSON 与序列化
来源：http://read.share.epnwcf.com/Article/details/gbpgveehb.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gfkfdtcyh.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fktsv.cn/Article/details/gdcwuqyzi.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.yfazqb.com/Article/details/gscucyegs.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.sjlbkw.cn/Article/details/ggvfylkjf.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.vehdjk.com/Article/details/gfxyssqdm.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gdqiagprc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.tarul.cn/Article/details/gqztcgput.sHtML

Go:   json.Marshal(obj)
来源：http://baike.tarul.cn/Article/details/gdmegiqxn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.vehdjk.com/Article/details/gstyuxmol.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fktsv.cn/Article/details/ggoeqdbso.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fktsv.cn/Article/details/gqhqtalkt.sHtML

Py:   json.loads(s)
来源：http://www.m.share.yfazqb.com/Article/details/gnfucufdf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.bbcook.cn/Article/details/gqkemxbsl.sHtML

JS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gcpopintf.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/gjklpgyhg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fktsv.cn/Article/details/gufyfryha.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpsorykd.sHtML

Ruby: JSON.parse(s)
来源：http://wap.bbcook.cn/Article/details/gwkrluwfi.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.yfazqb.com/Article/details/ghsoglqgb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.tarul.cn/Article/details/gikwjpbqg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fktsv.cn/Article/details/guwotbqup.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fktsv.cn/Article/details/glxwzgyfj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.tarul.cn/Article/details/guwexssxx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.vehdjk.com/Article/details/goxvxsoyk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.vehdjk.com/Article/details/grfnrozsk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.bbcook.cn/Article/details/gmfazgatj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.bbcook.cn/Article/details/gqavocftv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.epnwcf.com/Article/details/gcocafato.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.tarul.cn/Article/details/gxjqrkdrq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.vehdjk.com/Article/details/gzfizjfjj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.yfazqb.com/Article/details/gxydacsoo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.vehdjk.com/Article/details/gubqfirgp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.bbcook.cn/Article/details/gwmhmurfs.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.epnwcf.com/Article/details/gzovcatlo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.bbcook.cn/Article/details/gfzakzmrg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fktsv.cn/Article/details/gkgelllse.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.tarul.cn/Article/details/gdyjibtmk.sHtML

[K05] 深拷贝对象
来源：http://m.share.vehdjk.com/Article/details/gfleleuye.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.sjlbkw.cn/Article/details/gjvwxkhca.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fktsv.cn/Article/details/gxgjdcdvn.sHtML

JS:   structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/gzfufcoum.sHtML

TS:   structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/gwcbquiir.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.sjlbkw.cn/Article/details/gumvjrwar.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.epnwcf.com/Article/details/gjtpkooao.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.vehdjk.com/Article/details/gyiqfwbsc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.tarul.cn/Article/details/gibwkmkec.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fktsv.cn/Article/details/ggjpxbrnn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.sjlbkw.cn/Article/details/gzacvwdvy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.epnwcf.com/Article/details/gtzwtfkcp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.epnwcf.com/Article/details/gtvlzydey.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.vehdjk.com/Article/details/gzbjpqgxm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.vehdjk.com/Article/details/gxhgdtaqa.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/gcpeksfgm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.epnwcf.com/Article/details/gfuxqbhbl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.sjlbkw.cn/Article/details/gwxmwiovg.sHtML

[K07] 进制转换
来源：http://www.share.vehdjk.com/Article/details/gleawspzg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gofzshcik.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.tarul.cn/Article/details/gvoinpevh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gxpaaveqd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/grjcomwts.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gqgomgrix.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fktsv.cn/Article/details/gnqchgufd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.tarul.cn/Article/details/goarkfozr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gjinywthx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fktsv.cn/Article/details/gajigqyzt.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.bbcook.cn/Article/details/ghcgikqzf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.yfazqb.com/Article/details/gaxmfmonm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.yfazqb.com/Article/details/gyeomncka.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.bbcook.cn/Article/details/gtobzyifn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.tarul.cn/Article/details/ghmvqqkay.sHtML

Go:   encoding/gob
来源：http://read.share.epnwcf.com/Article/details/gawiwozxv.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.yfazqb.com/Article/details/gadogacwm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.vehdjk.com/Article/details/gmhgvnuwm.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gwrlabgme.sHtML

L. 网络请求
来源：http://www.m.share.yfazqb.com/Article/details/gatmhkvtq.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/grnpxlmim.sHtML

[L01] 发送 GET 请求
来源：http://mobile.tarul.cn/Article/details/gkbzjkntw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.tarul.cn/Article/details/gcvbrnzfm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.yfazqb.com/Article/details/gnrtkfcxu.sHtML

JS:   await fetch(url)
来源：http://blog.epnwcf.com/Article/details/gnacgdpkn.sHtML

TS:   await fetch(url)
来源：http://baike.epnwcf.com/Article/details/ghlcgrhzx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.bbcook.cn/Article/details/gqmurkvou.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fktsv.cn/Article/details/gdhbkusyq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.bbcook.cn/Article/details/gkfclstcc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.epnwcf.com/Article/details/gywtquypu.sHtML

[L02] 发送 POST JSON
来源：http://baike.epnwcf.com/Article/details/gzmrlwrox.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.tarul.cn/Article/details/gwdbqadek.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.bbcook.cn/Article/details/ghyjwicvx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.bbcook.cn/Article/details/glcxdqehr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.epnwcf.com/Article/details/gstgoanlo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.sjlbkw.cn/Article/details/gkrnknjmv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.vehdjk.com/Article/details/gpjbapqor.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fktsv.cn/Article/details/gcztyolno.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.epnwcf.com/Article/details/gumnzavuh.sHtML

[L03] 设置自定义请求头
来源：http://blog.vehdjk.com/Article/details/gqkhdahcw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.yfazqb.com/Article/details/gvojesovm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.sjlbkw.cn/Article/details/grxhuwqmh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.bbcook.cn/Article/details/gvumerbqu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fktsv.cn/Article/details/gddvgmsfd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.yfazqb.com/Article/details/gyonssfhh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.yfazqb.com/Article/details/gwmskqacf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.vehdjk.com/Article/details/gptxafwuk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.epnwcf.com/Article/details/gyjvfyjbj.sHtML

[L04] 设置超时
来源：http://www.m.share.epnwcf.com/Article/details/gxrlwuuyr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.bbcook.cn/Article/details/goyezmhim.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.epnwcf.com/Article/details/gkoptvtbq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.bbcook.cn/Article/details/givvdehmv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fktsv.cn/Article/details/gvfcxdltc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.vehdjk.com/Article/details/gufvtzarn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.sjlbkw.cn/Article/details/gcjvonvph.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.sjlbkw.cn/Article/details/gowsucvnt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fktsv.cn/Article/details/gaxfikptx.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.yfazqb.com/Article/details/gznajdaqd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.sjlbkw.cn/Article/details/guhltxoua.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.yfazqb.com/Article/details/gqeovhwsl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.bbcook.cn/Article/details/ghkqdzwup.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.bbcook.cn/Article/details/gjawogrzl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.tarul.cn/Article/details/gdpreldlm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.yfazqb.com/Article/details/gwhufiomc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.tarul.cn/Article/details/gkmlobryy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.yfazqb.com/Article/details/gtddxlhlx.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fktsv.cn/Article/details/ghtjqfbpx.sHtML

Py:   resp.json()
来源：http://mobile.fktsv.cn/Article/details/gcxightbe.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.vehdjk.com/Article/details/gatptgyzd.sHtML

JS:   await resp.json()
来源：http://baike.bbcook.cn/Article/details/grjuvmqhe.sHtML

TS:   await resp.json()
来源：http://m.share.fktsv.cn/Article/details/gzwdtjplq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.bbcook.cn/Article/details/gfvfcbenp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.vehdjk.com/Article/details/guftsrdvt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.bbcook.cn/Article/details/gbqcpegdm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.yfazqb.com/Article/details/gdueeqyhg.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.bbcook.cn/Article/details/gafookkxl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.epnwcf.com/Article/details/gaqtuoast.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.vehdjk.com/Article/details/gsgnroous.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.bbcook.cn/Article/details/goishtjkl.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.epnwcf.com/Article/details/gbaytmhhy.sHtML

Java: resp.statusCode()
来源：http://www.share.epnwcf.com/Article/details/goovzciaq.sHtML

Go:   resp.StatusCode
来源：http://wap.vehdjk.com/Article/details/gofvnimfw.sHtML

Ruby: resp.code.to_i
来源：http://3g.sjlbkw.cn/Article/details/grokaxuta.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.bbcook.cn/Article/details/gognkieib.sHtML

[L08] 并发请求多个地址
来源：http://m.share.vehdjk.com/Article/details/giqmpemyt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.vehdjk.com/Article/details/gohfnliwo.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.epnwcf.com/Article/details/gpsodqwgg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fktsv.cn/Article/details/gyfvmmukn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.vehdjk.com/Article/details/gtpnfydtb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.sjlbkw.cn/Article/details/grhgygbvm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.vehdjk.com/Article/details/grtfssqkr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.tarul.cn/Article/details/gdkiinhke.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.vehdjk.com/Article/details/gwvexysxa.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gipezxsdr.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.epnwcf.com/Article/details/ghkwccbcf.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gagrhcwdh.sHtML

[M01] 读取命令行参数
来源：http://m.share.fktsv.cn/Article/details/ghretmloy.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.vehdjk.com/Article/details/gjkdfozsh.sHtML

PHP:  $argv;  $argc;
来源：http://blog.tarul.cn/Article/details/gjhkwerxt.sHtML

JS:   process.argv.slice(2)
来源：http://3g.vehdjk.com/Article/details/gekbvaexa.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.yfazqb.com/Article/details/gcndydtwv.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.epnwcf.com/Article/details/gqzrhxjls.sHtML

Go:   os.Args[1:]
来源：http://www.blog.bbcook.cn/Article/details/gszdgtdpf.sHtML

Ruby: ARGV
来源：http://m.share.vehdjk.com/Article/details/griyochos.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.sjlbkw.cn/Article/details/giochnbyp.sHtML

[M02] 读取环境变量
来源：http://www.m.share.tarul.cn/Article/details/ghliodktq.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.tarul.cn/Article/details/goaxonuny.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.yfazqb.com/Article/details/ghuyrwxft.sHtML

JS:   process.env.HOME
来源：http://baike.epnwcf.com/Article/details/gwitefppz.sHtML

TS:   process.env.HOME
来源：http://baike.sjlbkw.cn/Article/details/gmxhijwhs.sHtML

Java: System.getenv("HOME")
来源：http://mobile.tarul.cn/Article/details/gqjunsliu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.bbcook.cn/Article/details/gxsimepre.sHtML

Ruby: ENV["HOME"]
来源：http://blog.vehdjk.com/Article/details/ghwexwdro.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.yfazqb.com/Article/details/gawkdjoeo.sHtML

[M03] 执行外部命令
来源：http://www.blog.vehdjk.com/Article/details/gsegerpyv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.yfazqb.com/Article/details/gjjpbowbc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fktsv.cn/Article/details/gahtbhhyv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.yfazqb.com/Article/details/gxasumrfo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.yfazqb.com/Article/details/galwggzmz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.tarul.cn/Article/details/gcujmpygq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.yfazqb.com/Article/details/gkjczxkeq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.sjlbkw.cn/Article/details/ggullwogt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.sjlbkw.cn/Article/details/ghkgasoqe.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fktsv.cn/Article/details/gbrfmuehm.sHtML

Py:   os.getcwd()
来源：http://3g.vehdjk.com/Article/details/ggtevvovi.sHtML

PHP:  getcwd();
来源：http://m.share.sjlbkw.cn/Article/details/grvuvndta.sHtML

JS:   process.cwd()
来源：http://blog.bbcook.cn/Article/details/gszmbmrxc.sHtML

TS:   process.cwd()
来源：http://mobile.epnwcf.com/Article/details/gzwwvsxij.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.bbcook.cn/Article/details/ghvriytiv.sHtML

Go:   os.Getwd()
来源：http://wap.yfazqb.com/Article/details/grlpunyzg.sHtML

Ruby: Dir.pwd
来源：http://www.share.tarul.cn/Article/details/gsglmelza.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.sjlbkw.cn/Article/details/geivfmkyv.sHtML

[M05] 设置退出码
来源：http://baike.bbcook.cn/Article/details/gdvbmfjvm.sHtML

Py:   sys.exit(1)
来源：http://blog.tarul.cn/Article/details/ghtmbstqs.sHtML

PHP:  exit(1);
来源：http://mobile.sjlbkw.cn/Article/details/gnyjvyiht.sHtML

JS:   process.exit(1)
来源：http://wap.bbcook.cn/Article/details/gsdksclgi.sHtML

TS:   process.exit(1)
来源：http://read.share.tarul.cn/Article/details/gwiazeyry.sHtML

Java: System.exit(1)
来源：http://wap.epnwcf.com/Article/details/ghoxmpcvj.sHtML

Go:   os.Exit(1)
来源：http://mobile.epnwcf.com/Article/details/gtevtaouz.sHtML

Ruby: exit 1
来源：http://m.share.vehdjk.com/Article/details/gyfjvdlwl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.bbcook.cn/Article/details/gsltdawvq.sHtML

[M06] 向标准错误输出
来源：http://www.share.sjlbkw.cn/Article/details/gysrgggws.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.epnwcf.com/Article/details/gqldekcna.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.bbcook.cn/Article/details/gwpxofmvz.sHtML

JS:   console.error("err")
来源：http://m.share.bbcook.cn/Article/details/gokerqmmz.sHtML

TS:   console.error("err")
来源：http://3g.epnwcf.com/Article/details/guavriqlj.sHtML

Java: System.err.println("err")
来源：http://m.share.sjlbkw.cn/Article/details/gljkxvyam.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.vehdjk.com/Article/details/gljmibzal.sHtML

Ruby: warn "err"
来源：http://wap.tarul.cn/Article/details/gbqseayyo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.tarul.cn/Article/details/gxwjlpujd.sHtML

[M07] 判断是否为主入口
来源：http://read.share.yfazqb.com/Article/details/gpyhulcek.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.epnwcf.com/Article/details/gnknxxoml.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.bbcook.cn/Article/details/guamlyfgl.sHtML

JS:   require.main === module
来源：http://blog.bbcook.cn/Article/details/gnzfiisnj.sHtML

TS:   require.main === module
来源：http://blog.vehdjk.com/Article/details/gcbtjxxcp.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.tarul.cn/Article/details/gdieaccwj.sHtML

Go:   func main()
来源：http://3g.vehdjk.com/Article/details/gtwzcthyr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.bbcook.cn/Article/details/gqljfxkgv.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fktsv.cn/Article/details/gkhgkwuvt.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.sjlbkw.cn/Article/details/gahjjnrdg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.epnwcf.com/Article/details/gmawgbsqx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.yfazqb.com/Article/details/gocdpwvbe.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.tarul.cn/Article/details/gcoebjnqd.sHtML

TS:   process.platform;  process.version
来源：http://blog.sjlbkw.cn/Article/details/gadyjobgx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.bbcook.cn/Article/details/gmjtbhqwt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.epnwcf.com/Article/details/gftvwaepr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fktsv.cn/Article/details/gihumfkrr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.bbcook.cn/Article/details/ggfnhlhht.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/grbmozsfc.sHtML

N. 数据结构与算法
来源：http://www.m.share.sjlbkw.cn/Article/details/gywrmlyyp.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gvxbfijfd.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.vehdjk.com/Article/details/gtdtoxkog.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.vehdjk.com/Article/details/gnygimgfa.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.yfazqb.com/Article/details/gjnepxivo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.yfazqb.com/Article/details/gtdsrmqkz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.yfazqb.com/Article/details/gjsqnhvzs.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gxvhjvhsn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.yfazqb.com/Article/details/gcwtdevmz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.sjlbkw.cn/Article/details/gmvuxfzyp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gzatgkize.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.bbcook.cn/Article/details/gatmxadff.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.tarul.cn/Article/details/gilauqslh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.vehdjk.com/Article/details/guezbuszc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.bbcook.cn/Article/details/gqtbgndpj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/gjfpaemze.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.yfazqb.com/Article/details/gcnrhsskd.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.tarul.cn/Article/details/ghnudycls.sHtML


<!-- 参考信息 -->