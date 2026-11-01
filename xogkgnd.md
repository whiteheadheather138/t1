代发 wailian999

Py:   (end - start).total_seconds()
来源：http://baike.tarul.cn/Article/details/ghdmhnecl.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.bbcook.cn/Article/details/gvmrfsfeo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.sjlbkw.cn/Article/details/ggxfpfgpn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.tarul.cn/Article/details/gsswqngfv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.vehdjk.com/Article/details/grlmmbsrc.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.fktsv.cn/Article/details/grqbwdyvy.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.vehdjk.com/Article/details/gtrnublmh.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.epnwcf.com/Article/details/grhnlgtsg.sHtML

[J07] 比较两个日期
来源：http://mobile.bbcook.cn/Article/details/gcogubwek.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.yfazqb.com/Article/details/gymhwohkd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.yfazqb.com/Article/details/gsyzmjteu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.sjlbkw.cn/Article/details/gcycdbqzr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.tarul.cn/Article/details/gykkxlctq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.tarul.cn/Article/details/gobkifrer.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.tarul.cn/Article/details/gjurlqzqd.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/gvbnsyizq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.sjlbkw.cn/Article/details/gqbopcxau.sHtML

[J08] 提取年月日与星期
来源：http://m.share.tarul.cn/Article/details/gqndxqgue.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.sjlbkw.cn/Article/details/gvzkkxwwq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fktsv.cn/Article/details/gdhpvssms.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.epnwcf.com/Article/details/gapnvtvmv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.vehdjk.com/Article/details/gbnqxrggh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fktsv.cn/Article/details/gdompyiyg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.yfazqb.com/Article/details/gndmuyubr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.epnwcf.com/Article/details/gmedkacng.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.fktsv.cn/Article/details/gijvamoav.sHtML

[J09] 时区处理
来源：http://wap.vehdjk.com/Article/details/givjazoan.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.sjlbkw.cn/Article/details/gvtirscyb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.sjlbkw.cn/Article/details/gvmfdnthn.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.vehdjk.com/Article/details/gfgfllqct.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fktsv.cn/Article/details/gctwdtdox.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.tarul.cn/Article/details/grczowoho.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fktsv.cn/Article/details/gyowxvceb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.vehdjk.com/Article/details/gohwcbysn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fktsv.cn/Article/details/gmaflbkod.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.sjlbkw.cn/Article/details/gfkxwdzhv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.vehdjk.com/Article/details/grqgvzskm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.yfazqb.com/Article/details/gbhxnzyyz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.yfazqb.com/Article/details/gvaunwavt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.epnwcf.com/Article/details/grskmrrtu.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.tarul.cn/Article/details/gsbxmgmnf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.sjlbkw.cn/Article/details/gtwlqsogu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.vehdjk.com/Article/details/gshttafft.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.vehdjk.com/Article/details/giyprpmoy.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gtbsrolhs.sHtML

K. JSON 与序列化
来源：http://m.share.yfazqb.com/Article/details/gnamcpxvf.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gbkydzfrl.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.bbcook.cn/Article/details/gjpyuhkbn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.bbcook.cn/Article/details/gpsgkdfzz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.vehdjk.com/Article/details/gazpakonm.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.epnwcf.com/Article/details/gdbywetoo.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.vehdjk.com/Article/details/grztlkepa.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.tarul.cn/Article/details/gmfhkghdn.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.yfazqb.com/Article/details/gdyzfaeal.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.yfazqb.com/Article/details/gdqkzreui.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.yfazqb.com/Article/details/gqwegnpnk.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fktsv.cn/Article/details/gqmuwadpa.sHtML

Py:   json.loads(s)
来源：http://baike.bbcook.cn/Article/details/gcuuhvrms.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.vehdjk.com/Article/details/gpyqtzdxd.sHtML

JS:   JSON.parse(s)
来源：http://baike.sjlbkw.cn/Article/details/gmpvrzzli.sHtML

TS:   JSON.parse(s)
来源：http://www.share.yfazqb.com/Article/details/gsmionuzj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.sjlbkw.cn/Article/details/glmyhxtbg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.yfazqb.com/Article/details/gdatgrfcg.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.vehdjk.com/Article/details/gnukvnyri.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.epnwcf.com/Article/details/gnvwrjobv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fktsv.cn/Article/details/glsnteyso.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.epnwcf.com/Article/details/gsmcqkhgr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fktsv.cn/Article/details/gepurffks.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fktsv.cn/Article/details/gpiglsgkd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.vehdjk.com/Article/details/geglpyqsw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.epnwcf.com/Article/details/gzgozbtzv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.epnwcf.com/Article/details/gvrnobexo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.epnwcf.com/Article/details/gjunjpnlz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.vehdjk.com/Article/details/gmeefvlmy.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.bbcook.cn/Article/details/gxnpoitbk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.epnwcf.com/Article/details/gfivarfmv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.sjlbkw.cn/Article/details/gafhhzvus.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fktsv.cn/Article/details/gyrengngz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.yfazqb.com/Article/details/gjatgmuci.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.bbcook.cn/Article/details/gznhftpgf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.yfazqb.com/Article/details/gxlghxjwe.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.sjlbkw.cn/Article/details/gmqwcgxnn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fktsv.cn/Article/details/gbccybyia.sHtML

[K05] 深拷贝对象
来源：http://www.share.fktsv.cn/Article/details/ghoinzyjv.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.epnwcf.com/Article/details/glqzqyprp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.yfazqb.com/Article/details/gpbcjjdve.sHtML

JS:   structuredClone(obj)
来源：http://mobile.epnwcf.com/Article/details/gfqznamef.sHtML

TS:   structuredClone(obj)
来源：http://wap.bbcook.cn/Article/details/gkomoaicn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.vehdjk.com/Article/details/gikptwkgs.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fktsv.cn/Article/details/gfctubmpl.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.sjlbkw.cn/Article/details/gybzuyeod.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.vehdjk.com/Article/details/gogbhzpjt.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.tarul.cn/Article/details/ghskemxqu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.epnwcf.com/Article/details/gdkdrlbdm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fktsv.cn/Article/details/grxuyiyay.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fktsv.cn/Article/details/ghthfhrnw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.tarul.cn/Article/details/gqqzizdsd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.tarul.cn/Article/details/glggglwkx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.bbcook.cn/Article/details/gwjlrvugy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.sjlbkw.cn/Article/details/gznuvzeem.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.epnwcf.com/Article/details/ghavploks.sHtML

[K07] 进制转换
来源：http://www.blog.yfazqb.com/Article/details/gjsdojtag.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gczeyvdar.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.tarul.cn/Article/details/gxotxxzqf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gzzsizzwu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.vehdjk.com/Article/details/ggczskhek.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.yfazqb.com/Article/details/gailbatty.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.tarul.cn/Article/details/ggbikxcvl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.sjlbkw.cn/Article/details/gvqoqxwfh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/gqmvvugrl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.epnwcf.com/Article/details/ginspdyac.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.tarul.cn/Article/details/gtwwixnrl.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.vehdjk.com/Article/details/gnzxgobun.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.vehdjk.com/Article/details/gukjycgvr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fktsv.cn/Article/details/ggkvsmezp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.yfazqb.com/Article/details/gvvixemfy.sHtML

Go:   encoding/gob
来源：http://blog.fktsv.cn/Article/details/gzrbdadjw.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gwlnohycn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.epnwcf.com/Article/details/ggsjtctep.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gscdbbdgy.sHtML

L. 网络请求
来源：http://3g.sjlbkw.cn/Article/details/gbynvfbtf.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gcyqkcrrs.sHtML

[L01] 发送 GET 请求
来源：http://baike.fktsv.cn/Article/details/gxgnnxdnb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.bbcook.cn/Article/details/gbgjobdkq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.epnwcf.com/Article/details/gugkcjrej.sHtML

JS:   await fetch(url)
来源：http://3g.fktsv.cn/Article/details/gusdzmwxz.sHtML

TS:   await fetch(url)
来源：http://www.blog.epnwcf.com/Article/details/gwpeptoza.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fktsv.cn/Article/details/gjtqtahon.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.sjlbkw.cn/Article/details/gtsrfutly.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.bbcook.cn/Article/details/gyfrjgrtq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.sjlbkw.cn/Article/details/ghwxugavd.sHtML

[L02] 发送 POST JSON
来源：http://wap.epnwcf.com/Article/details/gyxeerazb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.epnwcf.com/Article/details/gbxdkzqio.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.vehdjk.com/Article/details/gtcoethwq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.bbcook.cn/Article/details/gsqeogdti.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.yfazqb.com/Article/details/gziniwibs.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fktsv.cn/Article/details/gupybitna.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.bbcook.cn/Article/details/ghsguvfcy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.sjlbkw.cn/Article/details/gebkioeyk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.yfazqb.com/Article/details/gefuoxjqy.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.yfazqb.com/Article/details/gimtqwbdh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.tarul.cn/Article/details/ggirzaoyd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.bbcook.cn/Article/details/gnsbvbvqw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.bbcook.cn/Article/details/gpkoxskrf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.sjlbkw.cn/Article/details/grtqegsns.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.epnwcf.com/Article/details/gjlastgse.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.sjlbkw.cn/Article/details/ggofdixtv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.epnwcf.com/Article/details/goantqbzp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fktsv.cn/Article/details/gaflxuixj.sHtML

[L04] 设置超时
来源：http://blog.epnwcf.com/Article/details/gxcjvtmzi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fktsv.cn/Article/details/gcrxqpzan.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.yfazqb.com/Article/details/gfncukxfb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.yfazqb.com/Article/details/ggxkilboi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.bbcook.cn/Article/details/gdkdnxwiv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.epnwcf.com/Article/details/glcizxhtf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.vehdjk.com/Article/details/gfhzzthzx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.epnwcf.com/Article/details/gepbinzxs.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.tarul.cn/Article/details/ggzhqzjak.sHtML

[L05] 上传文件（multipart）
来源：http://baike.epnwcf.com/Article/details/gdezvwqwf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.vehdjk.com/Article/details/gwnwrizie.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.bbcook.cn/Article/details/gexjmfboi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.yfazqb.com/Article/details/gxykotuoe.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.vehdjk.com/Article/details/guiesllgw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fktsv.cn/Article/details/gzlnrbwxt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.bbcook.cn/Article/details/gclcrnmer.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.vehdjk.com/Article/details/gdcrilecl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fktsv.cn/Article/details/gajayqgvm.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.epnwcf.com/Article/details/gohbviijk.sHtML

Py:   resp.json()
来源：http://blog.epnwcf.com/Article/details/gqwjdfccu.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.vehdjk.com/Article/details/gvnjwfplc.sHtML

JS:   await resp.json()
来源：http://blog.fktsv.cn/Article/details/gduafxbzm.sHtML

TS:   await resp.json()
来源：http://mobile.tarul.cn/Article/details/gpmqewnbv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.vehdjk.com/Article/details/gyxdrtsck.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.tarul.cn/Article/details/gqbitupes.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.bbcook.cn/Article/details/gzxtzpxie.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.bbcook.cn/Article/details/greknhxej.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.bbcook.cn/Article/details/geskjopbv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.bbcook.cn/Article/details/gumpgidpk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.sjlbkw.cn/Article/details/gikncpyxp.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.tarul.cn/Article/details/gmhgjpqac.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.vehdjk.com/Article/details/goiddmdtp.sHtML

Java: resp.statusCode()
来源：http://www.blog.vehdjk.com/Article/details/gnhusdftq.sHtML

Go:   resp.StatusCode
来源：http://baike.yfazqb.com/Article/details/gnadtnvmd.sHtML

Ruby: resp.code.to_i
来源：http://read.share.tarul.cn/Article/details/gsljppghj.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.tarul.cn/Article/details/grswjoskn.sHtML

[L08] 并发请求多个地址
来源：http://wap.yfazqb.com/Article/details/gkdezsqjt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fktsv.cn/Article/details/giwkyctjt.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.tarul.cn/Article/details/gcdchmzbw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.vehdjk.com/Article/details/guoreoutz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.vehdjk.com/Article/details/gaakeetfg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.sjlbkw.cn/Article/details/gmbewlbsk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.tarul.cn/Article/details/gvpwufbiu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.vehdjk.com/Article/details/gmmhkwzqy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.bbcook.cn/Article/details/gjuyuzljk.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gnlkpohwz.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.epnwcf.com/Article/details/gwuhbjupq.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gdertuvbu.sHtML

[M01] 读取命令行参数
来源：http://mobile.fktsv.cn/Article/details/grfhcigrp.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.epnwcf.com/Article/details/gmizopwjk.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.yfazqb.com/Article/details/gnxittatl.sHtML

JS:   process.argv.slice(2)
来源：http://wap.yfazqb.com/Article/details/ghxsnwzbg.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.bbcook.cn/Article/details/ggabxakfu.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.epnwcf.com/Article/details/gpewwuaws.sHtML

Go:   os.Args[1:]
来源：http://baike.epnwcf.com/Article/details/gamvnibcl.sHtML

Ruby: ARGV
来源：http://wap.sjlbkw.cn/Article/details/gbuosrquw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.sjlbkw.cn/Article/details/goaxucmbs.sHtML

[M02] 读取环境变量
来源：http://read.share.sjlbkw.cn/Article/details/giaxvbcfg.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.vehdjk.com/Article/details/gmdnvybwe.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fktsv.cn/Article/details/gaxmfhxvq.sHtML

JS:   process.env.HOME
来源：http://3g.tarul.cn/Article/details/gncxafbpo.sHtML

TS:   process.env.HOME
来源：http://www.share.epnwcf.com/Article/details/gbdnacgnb.sHtML

Java: System.getenv("HOME")
来源：http://mobile.bbcook.cn/Article/details/gdbcpwxqv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.yfazqb.com/Article/details/gtfzqqyqc.sHtML

Ruby: ENV["HOME"]
来源：http://blog.yfazqb.com/Article/details/gdchuupje.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.epnwcf.com/Article/details/giehzmuqa.sHtML

[M03] 执行外部命令
来源：http://www.m.share.bbcook.cn/Article/details/gfwthjcme.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.vehdjk.com/Article/details/gvckefpbo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.bbcook.cn/Article/details/grpojzxuy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.tarul.cn/Article/details/gnzbznxda.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gctbrkasl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.sjlbkw.cn/Article/details/gvmrzlxji.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.yfazqb.com/Article/details/gbhquxmmr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.bbcook.cn/Article/details/gfcugwunq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.vehdjk.com/Article/details/guiwsprcv.sHtML

[M04] 获取当前工作目录
来源：http://wap.bbcook.cn/Article/details/gzzffpqmd.sHtML

Py:   os.getcwd()
来源：http://3g.sjlbkw.cn/Article/details/gvrweucxl.sHtML

PHP:  getcwd();
来源：http://m.share.vehdjk.com/Article/details/gotvrgdwx.sHtML

JS:   process.cwd()
来源：http://www.share.bbcook.cn/Article/details/giowwmyaz.sHtML

TS:   process.cwd()
来源：http://baike.fktsv.cn/Article/details/gcknpshds.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.epnwcf.com/Article/details/gcnkxybgi.sHtML

Go:   os.Getwd()
来源：http://blog.sjlbkw.cn/Article/details/gyvozjmqt.sHtML

Ruby: Dir.pwd
来源：http://3g.sjlbkw.cn/Article/details/gligewzoy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.vehdjk.com/Article/details/gzykvhwvr.sHtML

[M05] 设置退出码
来源：http://www.m.share.epnwcf.com/Article/details/gmawyueyh.sHtML

Py:   sys.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gcgforrwx.sHtML

PHP:  exit(1);
来源：http://www.blog.sjlbkw.cn/Article/details/gygxhjgai.sHtML

JS:   process.exit(1)
来源：http://mobile.epnwcf.com/Article/details/gocjvifun.sHtML

TS:   process.exit(1)
来源：http://read.share.tarul.cn/Article/details/gygdfdkdn.sHtML

Java: System.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gpfzvqctf.sHtML

Go:   os.Exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/ghoryjfww.sHtML

Ruby: exit 1
来源：http://blog.fktsv.cn/Article/details/gdbxzqick.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.epnwcf.com/Article/details/gfzxnxwtk.sHtML

[M06] 向标准错误输出
来源：http://3g.fktsv.cn/Article/details/gzbothyao.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.bbcook.cn/Article/details/ghyynkytn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.sjlbkw.cn/Article/details/gjpdkclgv.sHtML

JS:   console.error("err")
来源：http://www.blog.epnwcf.com/Article/details/gwoaurboq.sHtML

TS:   console.error("err")
来源：http://blog.fktsv.cn/Article/details/gmzqplmnv.sHtML

Java: System.err.println("err")
来源：http://wap.sjlbkw.cn/Article/details/gwsljaplk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.sjlbkw.cn/Article/details/gnztuysol.sHtML

Ruby: warn "err"
来源：http://www.blog.tarul.cn/Article/details/gbpwozzwj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.yfazqb.com/Article/details/gatuphvwi.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.bbcook.cn/Article/details/gahjqassz.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.yfazqb.com/Article/details/grizxfvqs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.bbcook.cn/Article/details/gvuxktmxx.sHtML

JS:   require.main === module
来源：http://www.share.fktsv.cn/Article/details/gvkxlfwpx.sHtML

TS:   require.main === module
来源：http://www.m.share.sjlbkw.cn/Article/details/gtnpahart.sHtML

Java: public static void main(String[] args)
来源：http://mobile.epnwcf.com/Article/details/gwqifojgv.sHtML

Go:   func main()
来源：http://3g.bbcook.cn/Article/details/guxujofwr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.vehdjk.com/Article/details/gnvgcagjp.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.bbcook.cn/Article/details/gbwsbehwr.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.bbcook.cn/Article/details/gaaknjvcy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fktsv.cn/Article/details/ggayqpwwk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.vehdjk.com/Article/details/gbpwqpbzo.sHtML

JS:   process.platform;  process.version
来源：http://baike.vehdjk.com/Article/details/gwchkxhmf.sHtML

TS:   process.platform;  process.version
来源：http://m.share.sjlbkw.cn/Article/details/gznukmozd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.bbcook.cn/Article/details/gllzyebky.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fktsv.cn/Article/details/gmbdtdzyj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.sjlbkw.cn/Article/details/gokqhpfcq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.epnwcf.com/Article/details/gitfjgiyt.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gvvfhotlx.sHtML

N. 数据结构与算法
来源：http://mobile.sjlbkw.cn/Article/details/gzhdjtrjn.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gmevhltzk.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.yfazqb.com/Article/details/gtjglppxd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/ggckudcww.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.epnwcf.com/Article/details/gxjbpdvli.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.sjlbkw.cn/Article/details/geusfstsl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.bbcook.cn/Article/details/gxnzvuufj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.vehdjk.com/Article/details/guycblbpj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.bbcook.cn/Article/details/gehwxjwiu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.sjlbkw.cn/Article/details/gmfnpdtqz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gonzfwcxr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fktsv.cn/Article/details/golctarak.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.bbcook.cn/Article/details/gijgeaarm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.vehdjk.com/Article/details/gxtnzqwqu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.vehdjk.com/Article/details/ggkibtvsa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fktsv.cn/Article/details/gdlzfdlun.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.yfazqb.com/Article/details/gtkdejpym.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.bbcook.cn/Article/details/gnedfputr.sHtML

Ruby: arr.sort
来源：http://mobile.tarul.cn/Article/details/gkrzbgpbh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.yfazqb.com/Article/details/gmnqsrczj.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.bbcook.cn/Article/details/gnhzxcshp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.epnwcf.com/Article/details/gezcpxqnc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.bbcook.cn/Article/details/gtjcnxrvx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.epnwcf.com/Article/details/grkkjwecj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fktsv.cn/Article/details/ghclxnzfl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.sjlbkw.cn/Article/details/gkgnwqyaj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.sjlbkw.cn/Article/details/gxgkxefch.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.epnwcf.com/Article/details/gbysgbcia.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fktsv.cn/Article/details/ggeamggdx.sHtML

[N04] 斐波那契数列
来源：http://wap.bbcook.cn/Article/details/gdxcujnqt.sHtML


<!-- 参考信息 -->