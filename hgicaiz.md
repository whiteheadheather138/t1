代发 wailian999

Py:   (end - start).total_seconds()
来源：http://read.share.fktsv.cn/Article/details/grfknmqcg.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.yfazqb.com/Article/details/gnkyzwymo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.epnwcf.com/Article/details/gcvswjvxr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.epnwcf.com/Article/details/gioaqbcgz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.vehdjk.com/Article/details/ghmmnrysk.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.bbcook.cn/Article/details/gfprgwshd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.tarul.cn/Article/details/gztjpytej.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.fktsv.cn/Article/details/gnszvosmj.sHtML

[J07] 比较两个日期
来源：http://3g.tarul.cn/Article/details/gxmrbxsmc.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.vehdjk.com/Article/details/gmfprcwfr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.fktsv.cn/Article/details/glawzyina.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.tarul.cn/Article/details/ggfqjnefl.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.yfazqb.com/Article/details/gcgboskgj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.fktsv.cn/Article/details/gwtcszfqy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fktsv.cn/Article/details/glveriweh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.epnwcf.com/Article/details/glnvqptkp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.tarul.cn/Article/details/gboqiznel.sHtML

[J08] 提取年月日与星期
来源：http://wap.bbcook.cn/Article/details/gfxgljihn.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.epnwcf.com/Article/details/gfwoyyewj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjbcfpht.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.sjlbkw.cn/Article/details/ghrfugiop.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.fktsv.cn/Article/details/gzpazaluf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.yfazqb.com/Article/details/goutjurro.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.fktsv.cn/Article/details/gqidnripp.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.sjlbkw.cn/Article/details/gaeebsorq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.epnwcf.com/Article/details/gaerzmpwy.sHtML

[J09] 时区处理
来源：http://baike.bbcook.cn/Article/details/gucadgxoa.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.vehdjk.com/Article/details/gsscrkudy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fktsv.cn/Article/details/grnzecqkl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.yfazqb.com/Article/details/gopcwthul.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.yfazqb.com/Article/details/gvugkklgy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.tarul.cn/Article/details/gtqiqouwo.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.epnwcf.com/Article/details/gehinqrzb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.yfazqb.com/Article/details/gkxvxlrhz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.yfazqb.com/Article/details/gwdidrqke.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.yfazqb.com/Article/details/gvyzykdvb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.bbcook.cn/Article/details/gahkqjuut.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.yfazqb.com/Article/details/gefpktprl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.tarul.cn/Article/details/gyloexkkb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.tarul.cn/Article/details/gwbtxtxji.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.tarul.cn/Article/details/gwtmjqwsu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.bbcook.cn/Article/details/gqcaczdju.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.epnwcf.com/Article/details/gyfcjrnob.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.epnwcf.com/Article/details/ggnhyapsn.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gddcxmxzg.sHtML

K. JSON 与序列化
来源：http://www.share.epnwcf.com/Article/details/gyiiinfnp.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gqlavonwd.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.vehdjk.com/Article/details/glmsrirko.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.tarul.cn/Article/details/gsxcfagxe.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.tarul.cn/Article/details/gebsiveyz.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.epnwcf.com/Article/details/gawfimlcg.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.bbcook.cn/Article/details/ghimmbjzq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.vehdjk.com/Article/details/gavewbefc.sHtML

Go:   json.Marshal(obj)
来源：http://wap.bbcook.cn/Article/details/gnylgwngm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.sjlbkw.cn/Article/details/gxkidaaby.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fktsv.cn/Article/details/gvmzoioiu.sHtML

[K02] JSON 字符串转对象
来源：http://blog.epnwcf.com/Article/details/gosnspgft.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fktsv.cn/Article/details/gokolcdvf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fktsv.cn/Article/details/girudipfq.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.bbcook.cn/Article/details/gvyoakphq.sHtML

TS:   JSON.parse(s)
来源：http://www.share.bbcook.cn/Article/details/gyhtfrois.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.epnwcf.com/Article/details/gnjkeaish.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.epnwcf.com/Article/details/gzpkbuzkz.sHtML

Ruby: JSON.parse(s)
来源：http://wap.sjlbkw.cn/Article/details/gftndtdol.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.sjlbkw.cn/Article/details/gteipdlba.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.tarul.cn/Article/details/gwqhgfqcr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsitmtlbr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.tarul.cn/Article/details/gdawbvsgj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.vehdjk.com/Article/details/gfuxywlpc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.vehdjk.com/Article/details/gvsetxtee.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.epnwcf.com/Article/details/gzopvjpya.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.tarul.cn/Article/details/guoraksjc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.epnwcf.com/Article/details/gnuwmwxsg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.vehdjk.com/Article/details/gxmptmtmh.sHtML

[K04] 读取 JSON 文件
来源：http://wap.bbcook.cn/Article/details/gcqxcvqna.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.vehdjk.com/Article/details/gpbzdanic.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.bbcook.cn/Article/details/grhmgfsej.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fktsv.cn/Article/details/gvdtbbjum.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.bbcook.cn/Article/details/gdueyaxav.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.sjlbkw.cn/Article/details/gwesigrhr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.tarul.cn/Article/details/glkgvcggn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.vehdjk.com/Article/details/gdrsbauwz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.sjlbkw.cn/Article/details/gmdtgexgp.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.bbcook.cn/Article/details/gdbnzrluu.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.tarul.cn/Article/details/gycqlweym.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.sjlbkw.cn/Article/details/gvqqpuoex.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.tarul.cn/Article/details/gairyxayi.sHtML

TS:   structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/gclaobfxx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.yfazqb.com/Article/details/grvyuvgxq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.tarul.cn/Article/details/gigdjjjcs.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.sjlbkw.cn/Article/details/gvrcwndwj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.epnwcf.com/Article/details/gfkbjpdba.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.bbcook.cn/Article/details/gilogspuc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.sjlbkw.cn/Article/details/gqclwgtvd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.vehdjk.com/Article/details/gflwoywbm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.vehdjk.com/Article/details/gdratggsy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.tarul.cn/Article/details/gubolmjkd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.sjlbkw.cn/Article/details/gbyggcueb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.vehdjk.com/Article/details/gnjcaootu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/grqozddby.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/gxstavyli.sHtML

[K07] 进制转换
来源：http://blog.yfazqb.com/Article/details/gnseixzly.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.tarul.cn/Article/details/glsxzafyt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.yfazqb.com/Article/details/gbbgkkvqo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.yfazqb.com/Article/details/glciiuhqz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gnqtwdyyf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gcqtcttsf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.epnwcf.com/Article/details/ggxgdfigy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.tarul.cn/Article/details/gkbhtjywr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gyazzvkvw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.epnwcf.com/Article/details/gtsfjpnnb.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fktsv.cn/Article/details/gpnvwgidx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fktsv.cn/Article/details/goesxokmu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.epnwcf.com/Article/details/gpmkultzm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fktsv.cn/Article/details/gahmdwvog.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.bbcook.cn/Article/details/gwvxpqaqd.sHtML

Go:   encoding/gob
来源：http://wap.fktsv.cn/Article/details/gsoadbnuq.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.bbcook.cn/Article/details/gxmxnxdqh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fktsv.cn/Article/details/gkepezdha.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gffbdoobp.sHtML

L. 网络请求
来源：http://baike.yfazqb.com/Article/details/gjtotkfbo.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/ginxxaicc.sHtML

[L01] 发送 GET 请求
来源：http://mobile.vehdjk.com/Article/details/gnmvwesiw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.bbcook.cn/Article/details/gpfknjxcj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.epnwcf.com/Article/details/gpsylwxlh.sHtML

JS:   await fetch(url)
来源：http://m.share.bbcook.cn/Article/details/gvbaadttm.sHtML

TS:   await fetch(url)
来源：http://read.share.epnwcf.com/Article/details/gftzfsdcq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.epnwcf.com/Article/details/gyaddcmwj.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.bbcook.cn/Article/details/gzsbazyou.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.epnwcf.com/Article/details/gfjtveoun.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.bbcook.cn/Article/details/gmkwotixw.sHtML

[L02] 发送 POST JSON
来源：http://read.share.yfazqb.com/Article/details/grlowhski.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.vehdjk.com/Article/details/gpkgawblr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.yfazqb.com/Article/details/gqzspsxvt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fktsv.cn/Article/details/gsfablxle.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.bbcook.cn/Article/details/gaqbvatyv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fktsv.cn/Article/details/gxlcbyxhy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.vehdjk.com/Article/details/gplufhnwt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.tarul.cn/Article/details/gnmtlrvlr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.vehdjk.com/Article/details/gurzppbjh.sHtML

[L03] 设置自定义请求头
来源：http://blog.yfazqb.com/Article/details/guoifgovm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.bbcook.cn/Article/details/gcmqypieq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.sjlbkw.cn/Article/details/gwlydtdod.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fktsv.cn/Article/details/gloipslfz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.vehdjk.com/Article/details/gogqclcqb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.yfazqb.com/Article/details/guuarbgzv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fktsv.cn/Article/details/glhkjvsbp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.bbcook.cn/Article/details/gfwlgbvtv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fktsv.cn/Article/details/gezqnizoa.sHtML

[L04] 设置超时
来源：http://mobile.tarul.cn/Article/details/gucxcxeaa.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.vehdjk.com/Article/details/gizqrvuui.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.yfazqb.com/Article/details/gvlzfvpmo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.bbcook.cn/Article/details/ggcdpwjoy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.epnwcf.com/Article/details/gsbutiqeg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.bbcook.cn/Article/details/gyhovpkru.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fktsv.cn/Article/details/gjqullyzc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fktsv.cn/Article/details/gyvcxksru.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.sjlbkw.cn/Article/details/grxlwyulf.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.sjlbkw.cn/Article/details/grsjeycfx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.bbcook.cn/Article/details/ghubawyco.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.bbcook.cn/Article/details/gbzzqmbxf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.vehdjk.com/Article/details/gwnkembmg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.vehdjk.com/Article/details/gfstesyid.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.bbcook.cn/Article/details/gilpjtzcs.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fktsv.cn/Article/details/gcnsjrdpf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.epnwcf.com/Article/details/gxphulfso.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.vehdjk.com/Article/details/gxvinmfsz.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.vehdjk.com/Article/details/gdivwgccs.sHtML

Py:   resp.json()
来源：http://3g.fktsv.cn/Article/details/gzrzkkaek.sHtML

PHP:  json_decode($body, true);
来源：http://wap.yfazqb.com/Article/details/gzismycrl.sHtML

JS:   await resp.json()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnvlnrnb.sHtML

TS:   await resp.json()
来源：http://mobile.tarul.cn/Article/details/ghbgdxkik.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.tarul.cn/Article/details/gxiuhbesr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.vehdjk.com/Article/details/gzpkeaaxm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.yfazqb.com/Article/details/gpepwxlox.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.yfazqb.com/Article/details/gessvhapy.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.sjlbkw.cn/Article/details/gmxvsvrpk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.bbcook.cn/Article/details/gznbxhlar.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.sjlbkw.cn/Article/details/govahlwgd.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.epnwcf.com/Article/details/gwslgkvuk.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.yfazqb.com/Article/details/giaqerzvz.sHtML

Java: resp.statusCode()
来源：http://mobile.yfazqb.com/Article/details/gzwfngevd.sHtML

Go:   resp.StatusCode
来源：http://www.share.vehdjk.com/Article/details/gdnjnwlua.sHtML

Ruby: resp.code.to_i
来源：http://3g.tarul.cn/Article/details/gnpphfrru.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.tarul.cn/Article/details/gxdkfddjv.sHtML

[L08] 并发请求多个地址
来源：http://m.share.yfazqb.com/Article/details/gvqcnotfv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.sjlbkw.cn/Article/details/gsnddtkjj.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.sjlbkw.cn/Article/details/giwvqivkm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fktsv.cn/Article/details/gdwwgdfpj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.bbcook.cn/Article/details/gjdbzumye.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.tarul.cn/Article/details/gbctayqxz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.epnwcf.com/Article/details/gtfzrwzej.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.bbcook.cn/Article/details/goosktrlm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.sjlbkw.cn/Article/details/ggbtipqae.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/ghqtindoi.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.epnwcf.com/Article/details/gvcgkcbbv.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gelnsiktx.sHtML

[M01] 读取命令行参数
来源：http://mobile.vehdjk.com/Article/details/gqbujxqig.sHtML

Py:   sys.argv[1:]
来源：http://m.share.sjlbkw.cn/Article/details/gopitolfp.sHtML

PHP:  $argv;  $argc;
来源：http://blog.yfazqb.com/Article/details/gizpalaqp.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.epnwcf.com/Article/details/gravxgfzo.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.bbcook.cn/Article/details/gnstmmwbc.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.tarul.cn/Article/details/gqepqmaxw.sHtML

Go:   os.Args[1:]
来源：http://www.share.fktsv.cn/Article/details/gdxamocia.sHtML

Ruby: ARGV
来源：http://www.blog.fktsv.cn/Article/details/gfgfiowzw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.bbcook.cn/Article/details/gkwlyqdac.sHtML

[M02] 读取环境变量
来源：http://wap.tarul.cn/Article/details/garbdserw.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.vehdjk.com/Article/details/gwffkyddj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.sjlbkw.cn/Article/details/gvyjyhcce.sHtML

JS:   process.env.HOME
来源：http://www.blog.yfazqb.com/Article/details/gfbllvwle.sHtML

TS:   process.env.HOME
来源：http://wap.bbcook.cn/Article/details/gcodmdqlc.sHtML

Java: System.getenv("HOME")
来源：http://wap.sjlbkw.cn/Article/details/gqmxzlluk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/gwmpsfdgl.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.epnwcf.com/Article/details/ghgekyxfn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.epnwcf.com/Article/details/goaxowzlt.sHtML

[M03] 执行外部命令
来源：http://baike.epnwcf.com/Article/details/gpspfxhlw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.epnwcf.com/Article/details/gnwdbytqq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.sjlbkw.cn/Article/details/gwjteamum.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fktsv.cn/Article/details/gcjqpbwrd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.tarul.cn/Article/details/ggvfdnsmy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.vehdjk.com/Article/details/guoflukni.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.epnwcf.com/Article/details/giqbbrdew.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.vehdjk.com/Article/details/guneffgyd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.epnwcf.com/Article/details/gjlhladts.sHtML

[M04] 获取当前工作目录
来源：http://3g.sjlbkw.cn/Article/details/gqghziggk.sHtML

Py:   os.getcwd()
来源：http://mobile.tarul.cn/Article/details/gybvvkhyj.sHtML

PHP:  getcwd();
来源：http://www.m.share.sjlbkw.cn/Article/details/gctbapnmf.sHtML

JS:   process.cwd()
来源：http://www.share.yfazqb.com/Article/details/gkjqblbqa.sHtML

TS:   process.cwd()
来源：http://read.share.sjlbkw.cn/Article/details/gfmyjkgzy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.yfazqb.com/Article/details/grhltttcg.sHtML

Go:   os.Getwd()
来源：http://mobile.tarul.cn/Article/details/gwrfqsgcz.sHtML

Ruby: Dir.pwd
来源：http://baike.bbcook.cn/Article/details/gqtedrthf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.vehdjk.com/Article/details/guhzctfll.sHtML

[M05] 设置退出码
来源：http://www.m.share.epnwcf.com/Article/details/grbijvwpt.sHtML

Py:   sys.exit(1)
来源：http://blog.yfazqb.com/Article/details/guaqcrmic.sHtML

PHP:  exit(1);
来源：http://read.share.fktsv.cn/Article/details/gfwbijzbc.sHtML

JS:   process.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gvhjmpsve.sHtML

TS:   process.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gfbqlkppr.sHtML

Java: System.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gmewbfxui.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gjlalfbkp.sHtML

Ruby: exit 1
来源：http://read.share.epnwcf.com/Article/details/gaapabbye.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.tarul.cn/Article/details/gqihbggxx.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.bbcook.cn/Article/details/gdptuasaa.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fktsv.cn/Article/details/ggqqeulti.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.yfazqb.com/Article/details/gxejohupg.sHtML

JS:   console.error("err")
来源：http://mobile.tarul.cn/Article/details/gjkaqvihy.sHtML

TS:   console.error("err")
来源：http://mobile.vehdjk.com/Article/details/gtnuzwudy.sHtML

Java: System.err.println("err")
来源：http://www.share.epnwcf.com/Article/details/gqcqbowjg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.tarul.cn/Article/details/gnwjwzbqr.sHtML

Ruby: warn "err"
来源：http://www.m.share.bbcook.cn/Article/details/guxhejkqh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.bbcook.cn/Article/details/gjtdhhyfd.sHtML

[M07] 判断是否为主入口
来源：http://mobile.bbcook.cn/Article/details/gotvjtdgb.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.bbcook.cn/Article/details/gjiyxgleb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fktsv.cn/Article/details/gbcaotjlg.sHtML

JS:   require.main === module
来源：http://read.share.yfazqb.com/Article/details/goalgotoy.sHtML

TS:   require.main === module
来源：http://read.share.epnwcf.com/Article/details/gfmlohjnv.sHtML

Java: public static void main(String[] args)
来源：http://blog.tarul.cn/Article/details/ggcyjmtuc.sHtML

Go:   func main()
来源：http://www.blog.fktsv.cn/Article/details/guesuckbv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.yfazqb.com/Article/details/gzkdsfomv.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.yfazqb.com/Article/details/gvfwbavql.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.bbcook.cn/Article/details/gqwaonrki.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.epnwcf.com/Article/details/gnmtudzwh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.epnwcf.com/Article/details/gblnevaxz.sHtML

JS:   process.platform;  process.version
来源：http://m.share.sjlbkw.cn/Article/details/gkatmldyy.sHtML

TS:   process.platform;  process.version
来源：http://read.share.sjlbkw.cn/Article/details/gjewvzyov.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.yfazqb.com/Article/details/gzgoijvrh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.yfazqb.com/Article/details/gkjwhecyd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.vehdjk.com/Article/details/ginzufwba.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.sjlbkw.cn/Article/details/gnxqbhifp.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gerifcduu.sHtML

N. 数据结构与算法
来源：http://read.share.sjlbkw.cn/Article/details/glyxztgxp.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gvwskyavk.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.tarul.cn/Article/details/gtkvfurbe.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.bbcook.cn/Article/details/gytzxybbx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.bbcook.cn/Article/details/gmbqkwxrd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.sjlbkw.cn/Article/details/ghudfzlfa.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.tarul.cn/Article/details/gphzeklmn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.yfazqb.com/Article/details/givgxvewb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gsqtlireb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fktsv.cn/Article/details/gwyqmdroe.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/giabjilas.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.bbcook.cn/Article/details/gjsefjkcp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.tarul.cn/Article/details/gayzojikj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.yfazqb.com/Article/details/gbtwbuauh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.tarul.cn/Article/details/gevmoswdc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.sjlbkw.cn/Article/details/glmnddvok.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.sjlbkw.cn/Article/details/gjadmcjhr.sHtML

Go:   slices.Sort(arr)
来源：http://blog.yfazqb.com/Article/details/gdycrykja.sHtML

Ruby: arr.sort
来源：http://3g.fktsv.cn/Article/details/gjhawdpaf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.vehdjk.com/Article/details/gtjdexghx.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.yfazqb.com/Article/details/gljpegavd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.sjlbkw.cn/Article/details/geczvymgu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.vehdjk.com/Article/details/goylwgcpl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.bbcook.cn/Article/details/gizqjcsgt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.epnwcf.com/Article/details/gxovfaepo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.epnwcf.com/Article/details/gjlftjfpw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fktsv.cn/Article/details/gwgyuqhuh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.vehdjk.com/Article/details/gfywrfnks.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.yfazqb.com/Article/details/guyhxzwon.sHtML

[N04] 斐波那契数列
来源：http://www.share.yfazqb.com/Article/details/ghrjiyqfo.sHtML


<!-- 参考信息 -->