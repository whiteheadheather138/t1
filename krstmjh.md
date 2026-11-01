代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fktsv.cn/Article/details/gqnlmvyma.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.vehdjk.com/Article/details/gkcanhtvt.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.sjlbkw.cn/Article/details/gdkyfvudy.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.fktsv.cn/Article/details/gpjpxnude.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fktsv.cn/Article/details/gzcgejfdk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.bbcook.cn/Article/details/gqahlfxfr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.tarul.cn/Article/details/gzitbamqy.sHtML

[J06] 计算两时间之差
来源：http://read.share.fktsv.cn/Article/details/gnnlcdwqs.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.epnwcf.com/Article/details/gsrviyvfl.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.epnwcf.com/Article/details/gerizqwzo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.yfazqb.com/Article/details/gngkgkbsv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.tarul.cn/Article/details/gbecsvggp.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.sjlbkw.cn/Article/details/gcjrzspks.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.fktsv.cn/Article/details/gnmohyubv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.tarul.cn/Article/details/gnainahub.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.vehdjk.com/Article/details/gwfrukphv.sHtML

[J07] 比较两个日期
来源：http://3g.fktsv.cn/Article/details/gkfzmyojq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.yfazqb.com/Article/details/gohvdxcqm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.vehdjk.com/Article/details/gcgfduhpy.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.fktsv.cn/Article/details/gstaovbed.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.vehdjk.com/Article/details/gqirynnlp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.tarul.cn/Article/details/gzjsegmoa.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.yfazqb.com/Article/details/gpsxajvbp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.fktsv.cn/Article/details/gldptgeao.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.bbcook.cn/Article/details/gxbftkwaq.sHtML

[J08] 提取年月日与星期
来源：http://m.share.epnwcf.com/Article/details/gokaznbpl.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.yfazqb.com/Article/details/gotiskvuj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.tarul.cn/Article/details/gxeuzogah.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.yfazqb.com/Article/details/gcxiodaal.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.bbcook.cn/Article/details/gpgccirsa.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.tarul.cn/Article/details/gtlxyaznz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fktsv.cn/Article/details/gmghduebn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.sjlbkw.cn/Article/details/gorizvlqk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.bbcook.cn/Article/details/gefrbbcqk.sHtML

[J09] 时区处理
来源：http://m.share.epnwcf.com/Article/details/grobyirpl.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.fktsv.cn/Article/details/gayktbgbe.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fktsv.cn/Article/details/gxavicfwv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.yfazqb.com/Article/details/gkkcidcaq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.vehdjk.com/Article/details/gyfmfjrwn.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.bbcook.cn/Article/details/gkblrlhox.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.tarul.cn/Article/details/gswepomyl.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.vehdjk.com/Article/details/gulubbknc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fktsv.cn/Article/details/ghlcfkpmo.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fktsv.cn/Article/details/gegoplnbf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.bbcook.cn/Article/details/gpwuuxsnx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.vehdjk.com/Article/details/gymofzyiu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/grlofjwxs.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.sjlbkw.cn/Article/details/gjogkuwzs.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.vehdjk.com/Article/details/gzevefyep.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.yfazqb.com/Article/details/guapthzgn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.bbcook.cn/Article/details/gnxyqbdjv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.tarul.cn/Article/details/gczinggno.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gnexzopev.sHtML

K. JSON 与序列化
来源：http://baike.vehdjk.com/Article/details/gpfmffano.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/ghyjzivno.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.vehdjk.com/Article/details/gisonbndo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.sjlbkw.cn/Article/details/gufsbjdqq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.bbcook.cn/Article/details/gdqzkckgw.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.tarul.cn/Article/details/gspssnkal.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.sjlbkw.cn/Article/details/gbzzngjno.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.yfazqb.com/Article/details/gnbegrhig.sHtML

Go:   json.Marshal(obj)
来源：http://blog.epnwcf.com/Article/details/ghinrmggj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.epnwcf.com/Article/details/gvlfudplp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.yfazqb.com/Article/details/geafnavns.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.bbcook.cn/Article/details/gbfbtrowv.sHtML

Py:   json.loads(s)
来源：http://baike.fktsv.cn/Article/details/gewkcwqic.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.bbcook.cn/Article/details/gekzmytoh.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.yfazqb.com/Article/details/grfnztrff.sHtML

TS:   JSON.parse(s)
来源：http://mobile.yfazqb.com/Article/details/gratdwajj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.yfazqb.com/Article/details/gtytprpzy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.sjlbkw.cn/Article/details/gygimkjtt.sHtML

Ruby: JSON.parse(s)
来源：http://3g.bbcook.cn/Article/details/gjogcfiem.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.vehdjk.com/Article/details/giwlpdvcw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.bbcook.cn/Article/details/gnakyczef.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.yfazqb.com/Article/details/gvbjfdyjv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.vehdjk.com/Article/details/gjntndigt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.tarul.cn/Article/details/gybfcldil.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.vehdjk.com/Article/details/gwalckmcs.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.epnwcf.com/Article/details/gwgydhthc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.epnwcf.com/Article/details/gigdgjtsr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.vehdjk.com/Article/details/gijmjcwrm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.bbcook.cn/Article/details/gqfcoinjr.sHtML

[K04] 读取 JSON 文件
来源：http://blog.epnwcf.com/Article/details/gyiknambw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fktsv.cn/Article/details/gthbkkqqp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.epnwcf.com/Article/details/gvzozoatb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.epnwcf.com/Article/details/gjlvivskj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fktsv.cn/Article/details/gkhiidplo.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/girxwjqkm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fktsv.cn/Article/details/ghaeviuuz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.tarul.cn/Article/details/gppskvlku.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.sjlbkw.cn/Article/details/gercojzqz.sHtML

[K05] 深拷贝对象
来源：http://3g.tarul.cn/Article/details/gqihdgfii.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.vehdjk.com/Article/details/gbvaalbsn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.sjlbkw.cn/Article/details/gycdzaijw.sHtML

JS:   structuredClone(obj)
来源：http://baike.epnwcf.com/Article/details/gxapuisrl.sHtML

TS:   structuredClone(obj)
来源：http://baike.tarul.cn/Article/details/gpenwyhsb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.vehdjk.com/Article/details/gbqdkkkan.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fktsv.cn/Article/details/gocqnexjq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fktsv.cn/Article/details/gjykpzxdn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.vehdjk.com/Article/details/gsamzllby.sHtML

[K06] 解析 URL 查询串
来源：http://blog.epnwcf.com/Article/details/gtphiadey.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.bbcook.cn/Article/details/glqaxozhh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fktsv.cn/Article/details/gedbqqoyk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.tarul.cn/Article/details/gsebamryo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.bbcook.cn/Article/details/gwtpswala.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.yfazqb.com/Article/details/gmectzjtp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.bbcook.cn/Article/details/gsgurkbkk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.epnwcf.com/Article/details/gxftgjilc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.sjlbkw.cn/Article/details/gtwcjjhfb.sHtML

[K07] 进制转换
来源：http://blog.sjlbkw.cn/Article/details/gsdyudpdp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gswcubjpm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.vehdjk.com/Article/details/gxzfxlvnm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gydkidycp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gihyjtqyk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gmniwzcns.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.yfazqb.com/Article/details/gplwbfwuo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.vehdjk.com/Article/details/gepvjzabn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/getfrgquc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.tarul.cn/Article/details/gobsytvtj.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fktsv.cn/Article/details/gknxrcbid.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.tarul.cn/Article/details/gkuoirnqz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.tarul.cn/Article/details/gsiiyyvcs.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gmdgrbzvk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fktsv.cn/Article/details/gflrdwhtg.sHtML

Go:   encoding/gob
来源：http://www.blog.vehdjk.com/Article/details/glxfbnkox.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.yfazqb.com/Article/details/gnrfduozy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.epnwcf.com/Article/details/gfknnxdrr.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gwymauono.sHtML

L. 网络请求
来源：http://m.share.vehdjk.com/Article/details/gqatouteo.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gillqouqa.sHtML

[L01] 发送 GET 请求
来源：http://read.share.bbcook.cn/Article/details/gmfvwkldz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.tarul.cn/Article/details/geohrmxde.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.tarul.cn/Article/details/gumbybfzx.sHtML

JS:   await fetch(url)
来源：http://3g.fktsv.cn/Article/details/gyxeuvluc.sHtML

TS:   await fetch(url)
来源：http://read.share.vehdjk.com/Article/details/gdqfztcyl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.tarul.cn/Article/details/gxmirxayl.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.vehdjk.com/Article/details/gozxbgong.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.epnwcf.com/Article/details/ggepkxyih.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.bbcook.cn/Article/details/gbglhffgb.sHtML

[L02] 发送 POST JSON
来源：http://wap.fktsv.cn/Article/details/gnfxxxmsp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.epnwcf.com/Article/details/gthpolzgi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fktsv.cn/Article/details/ggxgtrecl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.sjlbkw.cn/Article/details/gjegdudyw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.bbcook.cn/Article/details/gbtkwzsaq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fktsv.cn/Article/details/gifbkhzmb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fktsv.cn/Article/details/ghbufptfj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.yfazqb.com/Article/details/gnfszqffj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.epnwcf.com/Article/details/gzjxsxxxz.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.tarul.cn/Article/details/gnqbquvgq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.sjlbkw.cn/Article/details/gslwyyqsu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.epnwcf.com/Article/details/glbhjhvgd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.tarul.cn/Article/details/gkpjvfzls.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.vehdjk.com/Article/details/gsuzrvpal.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.epnwcf.com/Article/details/gaktqaudv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.sjlbkw.cn/Article/details/geeramnwu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.epnwcf.com/Article/details/gsnwssbfh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.tarul.cn/Article/details/gfwzlqcam.sHtML

[L04] 设置超时
来源：http://m.share.fktsv.cn/Article/details/gcdzlabhv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.sjlbkw.cn/Article/details/guyfhbdsi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.sjlbkw.cn/Article/details/grkkmcrss.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.tarul.cn/Article/details/ghfnxvwyk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.epnwcf.com/Article/details/ggrjgaksm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.sjlbkw.cn/Article/details/gmcbwkjen.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.epnwcf.com/Article/details/gsqhuvcbt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.tarul.cn/Article/details/gtrzzwgon.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fktsv.cn/Article/details/gpdfmyavw.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.epnwcf.com/Article/details/gbzbjkgui.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.yfazqb.com/Article/details/gzegzwebg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.sjlbkw.cn/Article/details/gwphbjtvu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.yfazqb.com/Article/details/gjrnfnlqu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.yfazqb.com/Article/details/gxnqynigv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.tarul.cn/Article/details/gykuzolme.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.epnwcf.com/Article/details/gjqigbhlw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fktsv.cn/Article/details/gldchqogs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.bbcook.cn/Article/details/ghixnvqdz.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fktsv.cn/Article/details/gflvxljfw.sHtML

Py:   resp.json()
来源：http://read.share.fktsv.cn/Article/details/gazoqrnlf.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.vehdjk.com/Article/details/gkmgnzvir.sHtML

JS:   await resp.json()
来源：http://www.blog.tarul.cn/Article/details/gpghecanl.sHtML

TS:   await resp.json()
来源：http://blog.tarul.cn/Article/details/gpxyqqath.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.epnwcf.com/Article/details/gqqkjezgb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.tarul.cn/Article/details/gcymtktwo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.vehdjk.com/Article/details/gqhnjdbyd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.epnwcf.com/Article/details/gmtojnkvw.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.tarul.cn/Article/details/gvvtogjdq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.tarul.cn/Article/details/gqbnlzfgx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.bbcook.cn/Article/details/gdpnhursy.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.tarul.cn/Article/details/gvrzknsiz.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.epnwcf.com/Article/details/gqtpgaurp.sHtML

Java: resp.statusCode()
来源：http://m.share.sjlbkw.cn/Article/details/gsvzukrin.sHtML

Go:   resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/gjlkxwpuk.sHtML

Ruby: resp.code.to_i
来源：http://www.share.vehdjk.com/Article/details/gqnrmkbul.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.vehdjk.com/Article/details/gckllsntg.sHtML

[L08] 并发请求多个地址
来源：http://blog.epnwcf.com/Article/details/gdcqghzsv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.tarul.cn/Article/details/gtvaiyxtp.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.vehdjk.com/Article/details/gvhtgmzas.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.sjlbkw.cn/Article/details/gsqushqqa.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gnpzswqnc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.sjlbkw.cn/Article/details/gingjphwb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.sjlbkw.cn/Article/details/ggdxdgdik.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.yfazqb.com/Article/details/govjfbzsl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.bbcook.cn/Article/details/gqpkezviz.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gnpjhfogp.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.bbcook.cn/Article/details/gjhanlzot.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gotvoaprt.sHtML

[M01] 读取命令行参数
来源：http://wap.vehdjk.com/Article/details/ghluwyfep.sHtML

Py:   sys.argv[1:]
来源：http://wap.yfazqb.com/Article/details/gqrleckhs.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.tarul.cn/Article/details/gjbsodtzy.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fktsv.cn/Article/details/gwxcsvjgr.sHtML

TS:   process.argv.slice(2)
来源：http://baike.bbcook.cn/Article/details/gbaxxquow.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fktsv.cn/Article/details/gpaiggwxr.sHtML

Go:   os.Args[1:]
来源：http://read.share.tarul.cn/Article/details/gpqcvlygt.sHtML

Ruby: ARGV
来源：http://www.blog.tarul.cn/Article/details/gobandngj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.yfazqb.com/Article/details/gxrxjeuqn.sHtML

[M02] 读取环境变量
来源：http://mobile.yfazqb.com/Article/details/ggrtodaeq.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fktsv.cn/Article/details/gfrjlonrm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.sjlbkw.cn/Article/details/ganxldoeq.sHtML

JS:   process.env.HOME
来源：http://3g.sjlbkw.cn/Article/details/gqqckgwqf.sHtML

TS:   process.env.HOME
来源：http://m.share.vehdjk.com/Article/details/gjysypekq.sHtML

Java: System.getenv("HOME")
来源：http://baike.yfazqb.com/Article/details/glwqjvust.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fktsv.cn/Article/details/ghyscozdc.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.tarul.cn/Article/details/gdbrcwotm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fktsv.cn/Article/details/gznhirbhk.sHtML

[M03] 执行外部命令
来源：http://baike.yfazqb.com/Article/details/gskfvubrm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.tarul.cn/Article/details/gtlphjxnz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.bbcook.cn/Article/details/goqyfkjro.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.bbcook.cn/Article/details/gsbrcmxga.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fktsv.cn/Article/details/ggdyyfspz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.epnwcf.com/Article/details/gotfgvobw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.vehdjk.com/Article/details/gguudfrgk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.tarul.cn/Article/details/glplqqcgm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fktsv.cn/Article/details/gipprhkko.sHtML

[M04] 获取当前工作目录
来源：http://m.share.sjlbkw.cn/Article/details/ghtslseol.sHtML

Py:   os.getcwd()
来源：http://m.share.sjlbkw.cn/Article/details/gxrrvrdos.sHtML

PHP:  getcwd();
来源：http://blog.yfazqb.com/Article/details/gvwdspnln.sHtML

JS:   process.cwd()
来源：http://www.m.share.bbcook.cn/Article/details/gyrgtscga.sHtML

TS:   process.cwd()
来源：http://mobile.fktsv.cn/Article/details/gvsbhrgzy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.yfazqb.com/Article/details/gehqfvemq.sHtML

Go:   os.Getwd()
来源：http://mobile.yfazqb.com/Article/details/gqbbdourg.sHtML

Ruby: Dir.pwd
来源：http://m.share.sjlbkw.cn/Article/details/gbnvfbhsp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.vehdjk.com/Article/details/gjtjydjme.sHtML

[M05] 设置退出码
来源：http://mobile.yfazqb.com/Article/details/ghwdhsfmp.sHtML

Py:   sys.exit(1)
来源：http://3g.yfazqb.com/Article/details/gqwwtdcze.sHtML

PHP:  exit(1);
来源：http://www.share.tarul.cn/Article/details/gasvoiyvz.sHtML

JS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gjejfbzia.sHtML

TS:   process.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gmhoghqfq.sHtML

Java: System.exit(1)
来源：http://baike.tarul.cn/Article/details/gxcdbouys.sHtML

Go:   os.Exit(1)
来源：http://3g.sjlbkw.cn/Article/details/glniuawcv.sHtML

Ruby: exit 1
来源：http://m.share.sjlbkw.cn/Article/details/gbptqljwi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.sjlbkw.cn/Article/details/gkvrcwely.sHtML

[M06] 向标准错误输出
来源：http://read.share.tarul.cn/Article/details/gezifrxpu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.vehdjk.com/Article/details/gvguhtbdb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.sjlbkw.cn/Article/details/gtxkkpiot.sHtML

JS:   console.error("err")
来源：http://www.m.share.bbcook.cn/Article/details/gtriioltw.sHtML

TS:   console.error("err")
来源：http://baike.epnwcf.com/Article/details/gwybkdhcz.sHtML

Java: System.err.println("err")
来源：http://read.share.epnwcf.com/Article/details/ggnndvvir.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.sjlbkw.cn/Article/details/gpqnmndqt.sHtML

Ruby: warn "err"
来源：http://3g.sjlbkw.cn/Article/details/gbgrvhxor.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.yfazqb.com/Article/details/ginppqqzq.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.tarul.cn/Article/details/glfirygmu.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.bbcook.cn/Article/details/gynvbwvxo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.tarul.cn/Article/details/grmhzcfqr.sHtML

JS:   require.main === module
来源：http://m.share.tarul.cn/Article/details/gcrlkwcys.sHtML

TS:   require.main === module
来源：http://3g.epnwcf.com/Article/details/gkyojovcb.sHtML

Java: public static void main(String[] args)
来源：http://m.share.yfazqb.com/Article/details/gsefzzhpv.sHtML

Go:   func main()
来源：http://3g.sjlbkw.cn/Article/details/gxxejkqfx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.tarul.cn/Article/details/ggjkojldf.sHtML

C#:   static void Main(string[] args)
来源：http://blog.sjlbkw.cn/Article/details/gvmakwirt.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.bbcook.cn/Article/details/gtwqdmsaj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.sjlbkw.cn/Article/details/giqkalrta.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.bbcook.cn/Article/details/gfwsgheqg.sHtML

JS:   process.platform;  process.version
来源：http://wap.vehdjk.com/Article/details/gdiorodud.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.epnwcf.com/Article/details/gndmyxneo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.tarul.cn/Article/details/giudvmbgp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.bbcook.cn/Article/details/guysrlxqj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fktsv.cn/Article/details/gtgsznxaq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.tarul.cn/Article/details/gzcpdftpy.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/ghicejhuh.sHtML

N. 数据结构与算法
来源：http://www.blog.yfazqb.com/Article/details/gdehnlesb.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gaqintzkr.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.epnwcf.com/Article/details/glpkdfynn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gulcrouiy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fktsv.cn/Article/details/gwpceimtz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.yfazqb.com/Article/details/gnwbpyxiy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fktsv.cn/Article/details/greldazhx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gpbkcevar.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.tarul.cn/Article/details/goowavroy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fktsv.cn/Article/details/gimrvryjh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.epnwcf.com/Article/details/giwmbustg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.bbcook.cn/Article/details/gvpvnxojv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.sjlbkw.cn/Article/details/gfmpzzxpw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.epnwcf.com/Article/details/guwudqdne.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.epnwcf.com/Article/details/ghvvxmfnx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fktsv.cn/Article/details/gbuotsdtt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.yfazqb.com/Article/details/guspgsxsx.sHtML

Go:   slices.Sort(arr)
来源：http://3g.bbcook.cn/Article/details/gtfivmviv.sHtML

Ruby: arr.sort
来源：http://m.share.sjlbkw.cn/Article/details/gyjmxnpon.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.sjlbkw.cn/Article/details/gdaniodns.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.yfazqb.com/Article/details/gpjtxfrmn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.vehdjk.com/Article/details/gllxiwwif.sHtML


<!-- 参考信息 -->