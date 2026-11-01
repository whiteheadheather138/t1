代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.sjlbkw.cn/Article/details/gucqchcwn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.fktsv.cn/Article/details/gbsrgvtrz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.bbcook.cn/Article/details/gkgaphrbg.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.tarul.cn/Article/details/gpwypluhg.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.fktsv.cn/Article/details/ggzaymzth.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.epnwcf.com/Article/details/gmyknrnmo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.epnwcf.com/Article/details/gwoegbpvd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fktsv.cn/Article/details/gzxmfmafe.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.bbcook.cn/Article/details/gkdibybdg.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.vehdjk.com/Article/details/geakitlgb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fktsv.cn/Article/details/guovhingw.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.tarul.cn/Article/details/gqhkfqppa.sHtML

[J07] 比较两个日期
来源：http://mobile.tarul.cn/Article/details/gwohkikmy.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.yfazqb.com/Article/details/gctzxrhns.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.epnwcf.com/Article/details/gdoslpzgt.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.tarul.cn/Article/details/gwvdobmfz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.sjlbkw.cn/Article/details/ggxjzwrgx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.tarul.cn/Article/details/gsmrgwuju.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.yfazqb.com/Article/details/gaszoqqsi.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/gtvdxfwxc.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/gewxzfmxp.sHtML

[J08] 提取年月日与星期
来源：http://blog.yfazqb.com/Article/details/gcwdlpntc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.vehdjk.com/Article/details/gbtjyrdqk.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.yfazqb.com/Article/details/gaavitlhk.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.sjlbkw.cn/Article/details/ggxaqezpp.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.epnwcf.com/Article/details/gmqoqwdzg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.bbcook.cn/Article/details/gkpzjyzfu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.fktsv.cn/Article/details/gxfvkdhxl.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.yfazqb.com/Article/details/gdpzgfexb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.vehdjk.com/Article/details/gsaxjunve.sHtML

[J09] 时区处理
来源：http://wap.bbcook.cn/Article/details/gnfunrvzh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.epnwcf.com/Article/details/gnczllewr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.yfazqb.com/Article/details/gmrcyjsuy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.yfazqb.com/Article/details/gikkbbtpo.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fktsv.cn/Article/details/gcnimkkrc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.bbcook.cn/Article/details/gkfnvwwqe.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.vehdjk.com/Article/details/gqxpgghqk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.epnwcf.com/Article/details/ggjcjwesf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.yfazqb.com/Article/details/gmuhrlwxg.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fktsv.cn/Article/details/gmbgkxuos.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.yfazqb.com/Article/details/gqonjymqk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.epnwcf.com/Article/details/gabulvrbq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.epnwcf.com/Article/details/gkwfnpwco.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.yfazqb.com/Article/details/godjkanma.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.bbcook.cn/Article/details/gbvjmdyzs.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.vehdjk.com/Article/details/gugskyywd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.tarul.cn/Article/details/gjvyneahy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.epnwcf.com/Article/details/gzmyqtvyz.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gadzxlydb.sHtML

K. JSON 与序列化
来源：http://wap.sjlbkw.cn/Article/details/gqbidvzpc.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gdugxcpfn.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.yfazqb.com/Article/details/gievgaxsk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.bbcook.cn/Article/details/gwugsucza.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.yfazqb.com/Article/details/gzafnxiif.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.sjlbkw.cn/Article/details/gdkmnvgmh.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.epnwcf.com/Article/details/gydgogvdf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fktsv.cn/Article/details/gluuzqghs.sHtML

Go:   json.Marshal(obj)
来源：http://blog.bbcook.cn/Article/details/gpcgvzagc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.epnwcf.com/Article/details/guyclpayj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.tarul.cn/Article/details/gwpzzylqg.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.yfazqb.com/Article/details/gepziljeo.sHtML

Py:   json.loads(s)
来源：http://wap.epnwcf.com/Article/details/gsynpjzgj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.tarul.cn/Article/details/gvgazubhb.sHtML

JS:   JSON.parse(s)
来源：http://www.share.bbcook.cn/Article/details/ggtwuyhln.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.epnwcf.com/Article/details/gnsmiyfxg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.yfazqb.com/Article/details/ghxushuuq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.sjlbkw.cn/Article/details/gzfhthryr.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.sjlbkw.cn/Article/details/guellatfb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fktsv.cn/Article/details/gnwnjbzee.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.epnwcf.com/Article/details/gzrnwajhd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.yfazqb.com/Article/details/givtysbax.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.vehdjk.com/Article/details/grriqbfcs.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.epnwcf.com/Article/details/gljqjiigc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.epnwcf.com/Article/details/gmrsvckpf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.epnwcf.com/Article/details/glhnmqeyu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.sjlbkw.cn/Article/details/gwzkssebz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.fktsv.cn/Article/details/gggrsesgu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.bbcook.cn/Article/details/gogrzrprd.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fktsv.cn/Article/details/gbvmcvmqr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.epnwcf.com/Article/details/gahagapxp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.tarul.cn/Article/details/gvumukcjt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.sjlbkw.cn/Article/details/gfmpjoogf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.sjlbkw.cn/Article/details/gmqzjrgux.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.yfazqb.com/Article/details/gpacoeksc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fktsv.cn/Article/details/gkfkbixit.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.yfazqb.com/Article/details/gyjxjljuk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.bbcook.cn/Article/details/gqlyatalz.sHtML

[K05] 深拷贝对象
来源：http://read.share.sjlbkw.cn/Article/details/guciqyivv.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.vehdjk.com/Article/details/ghqexisae.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.tarul.cn/Article/details/gyxzgattk.sHtML

JS:   structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/gbiorqfxx.sHtML

TS:   structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gikxaodor.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.tarul.cn/Article/details/gxjqzviwk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.tarul.cn/Article/details/gudimvgnw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.yfazqb.com/Article/details/gcjnrajvz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fktsv.cn/Article/details/ghdjwtrzc.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.tarul.cn/Article/details/gsvqgjfaz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.sjlbkw.cn/Article/details/gymsctrab.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.tarul.cn/Article/details/gbqhvcqrw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.epnwcf.com/Article/details/gsqqlugtp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.bbcook.cn/Article/details/gylbyelgo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.bbcook.cn/Article/details/gvciauegf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.vehdjk.com/Article/details/gfmryfiig.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gfrghmftr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.sjlbkw.cn/Article/details/gerkbfnjv.sHtML

[K07] 进制转换
来源：http://blog.fktsv.cn/Article/details/gldnedhop.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gtbjcaaua.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.sjlbkw.cn/Article/details/gqujcgdla.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gufsqoacr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gegzbstsb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gifkuxasm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.sjlbkw.cn/Article/details/gwyusfwqo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fktsv.cn/Article/details/geiijtcoh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gqvbzhjbi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.sjlbkw.cn/Article/details/gkxnjexqp.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.sjlbkw.cn/Article/details/glaqydvyd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fktsv.cn/Article/details/guuyaykzo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.yfazqb.com/Article/details/gelklgokh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.sjlbkw.cn/Article/details/gcuxkrihq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.sjlbkw.cn/Article/details/gblwsfijg.sHtML

Go:   encoding/gob
来源：http://baike.sjlbkw.cn/Article/details/gqbbcjdxt.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.vehdjk.com/Article/details/glsudzmay.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.tarul.cn/Article/details/gwchvnabj.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gwdpcinmk.sHtML

L. 网络请求
来源：http://www.blog.yfazqb.com/Article/details/gsedsinjg.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gtbxmdbvn.sHtML

[L01] 发送 GET 请求
来源：http://m.share.tarul.cn/Article/details/gfewsunge.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.sjlbkw.cn/Article/details/gqhymqyyv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.epnwcf.com/Article/details/gakxqbmzp.sHtML

JS:   await fetch(url)
来源：http://3g.bbcook.cn/Article/details/gvptflsji.sHtML

TS:   await fetch(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gnjresukd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.sjlbkw.cn/Article/details/gxezhjjcc.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.vehdjk.com/Article/details/gcoqdcazx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.yfazqb.com/Article/details/gwzishryb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fktsv.cn/Article/details/gotvzwaqz.sHtML

[L02] 发送 POST JSON
来源：http://read.share.yfazqb.com/Article/details/gxassyrkl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.bbcook.cn/Article/details/ggjvhjbfr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.epnwcf.com/Article/details/gekwhfwpa.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.yfazqb.com/Article/details/gnttnrdjo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.sjlbkw.cn/Article/details/grplrhljx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fktsv.cn/Article/details/grogneoww.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fktsv.cn/Article/details/gedsvmtns.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.epnwcf.com/Article/details/gllclurof.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.tarul.cn/Article/details/gvhmbhfry.sHtML

[L03] 设置自定义请求头
来源：http://read.share.tarul.cn/Article/details/gblhcoekg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fktsv.cn/Article/details/gxjzcyhdp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.epnwcf.com/Article/details/gxoxgngvv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.yfazqb.com/Article/details/gcfybnzcn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fktsv.cn/Article/details/gufrxwzxi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.sjlbkw.cn/Article/details/gaehajxvk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.tarul.cn/Article/details/gzrcdwlwi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.tarul.cn/Article/details/gnkqptguc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.tarul.cn/Article/details/giwkgltmv.sHtML

[L04] 设置超时
来源：http://wap.epnwcf.com/Article/details/gbkelxxty.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.tarul.cn/Article/details/glsctxfda.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fktsv.cn/Article/details/gjrpdncae.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.tarul.cn/Article/details/gmmmkjgpk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.tarul.cn/Article/details/gefhwxbsa.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.yfazqb.com/Article/details/guuohndcn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.yfazqb.com/Article/details/gmmailrbc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.sjlbkw.cn/Article/details/gxvajbmlw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.epnwcf.com/Article/details/gmqpqeatz.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.vehdjk.com/Article/details/grbnzlmle.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.vehdjk.com/Article/details/gqnvqboxp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.yfazqb.com/Article/details/gusuhwepn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.epnwcf.com/Article/details/gmibbrhtu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.sjlbkw.cn/Article/details/gldxkxqpu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.bbcook.cn/Article/details/gialdoeum.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.sjlbkw.cn/Article/details/gdiwexsgp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.bbcook.cn/Article/details/gjpzxhvzb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.epnwcf.com/Article/details/gopcrqsxb.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fktsv.cn/Article/details/gtrdbxkpj.sHtML

Py:   resp.json()
来源：http://mobile.tarul.cn/Article/details/ghldrledf.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.bbcook.cn/Article/details/gxkwcuwkg.sHtML

JS:   await resp.json()
来源：http://blog.vehdjk.com/Article/details/gxxtffdbo.sHtML

TS:   await resp.json()
来源：http://wap.tarul.cn/Article/details/glmwqklcd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.yfazqb.com/Article/details/gixddoffn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.vehdjk.com/Article/details/gfvmzwmvj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.yfazqb.com/Article/details/gzgodizgw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.bbcook.cn/Article/details/gpfexzowl.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.epnwcf.com/Article/details/gynykcrjf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.sjlbkw.cn/Article/details/gowvynpxv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fktsv.cn/Article/details/gcdzlfnot.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.bbcook.cn/Article/details/gekvzjyor.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.vehdjk.com/Article/details/graukcwcj.sHtML

Java: resp.statusCode()
来源：http://www.share.epnwcf.com/Article/details/gegkdhumn.sHtML

Go:   resp.StatusCode
来源：http://wap.sjlbkw.cn/Article/details/ggkgekwin.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.sjlbkw.cn/Article/details/gunjygkxk.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.epnwcf.com/Article/details/gikpgcrsr.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fktsv.cn/Article/details/gilwxkzzu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fktsv.cn/Article/details/gcmgjshql.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.epnwcf.com/Article/details/gmmbqyoas.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.vehdjk.com/Article/details/glntdyueu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.tarul.cn/Article/details/gqmsxfhrn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.sjlbkw.cn/Article/details/gwbbatafd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.epnwcf.com/Article/details/gptoqcpbh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.bbcook.cn/Article/details/gqmmcgrcs.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.vehdjk.com/Article/details/gqhnjntse.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gvzaprhzl.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.vehdjk.com/Article/details/geqwctphv.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gteonsljs.sHtML

[M01] 读取命令行参数
来源：http://www.blog.bbcook.cn/Article/details/gxwicvmfu.sHtML

Py:   sys.argv[1:]
来源：http://mobile.yfazqb.com/Article/details/gqkveolib.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.epnwcf.com/Article/details/grhmulnxx.sHtML

JS:   process.argv.slice(2)
来源：http://blog.vehdjk.com/Article/details/gylrxjogu.sHtML

TS:   process.argv.slice(2)
来源：http://blog.bbcook.cn/Article/details/gcasgfhww.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.bbcook.cn/Article/details/gthfulyjz.sHtML

Go:   os.Args[1:]
来源：http://www.blog.sjlbkw.cn/Article/details/gxgxekfap.sHtML

Ruby: ARGV
来源：http://blog.tarul.cn/Article/details/gbnnvklbd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.vehdjk.com/Article/details/gyjvrfqtd.sHtML

[M02] 读取环境变量
来源：http://read.share.sjlbkw.cn/Article/details/gnpezabdi.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.bbcook.cn/Article/details/guaxpfcee.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.tarul.cn/Article/details/gevbgzqav.sHtML

JS:   process.env.HOME
来源：http://mobile.epnwcf.com/Article/details/gijpffdvj.sHtML

TS:   process.env.HOME
来源：http://3g.bbcook.cn/Article/details/grsuxrvzj.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gtncopvnd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.yfazqb.com/Article/details/gpqshbzur.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fktsv.cn/Article/details/griivhoeg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.epnwcf.com/Article/details/gpttddfru.sHtML

[M03] 执行外部命令
来源：http://3g.tarul.cn/Article/details/gxlzzgmdq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fktsv.cn/Article/details/gszzxqqpj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.sjlbkw.cn/Article/details/gciucqnac.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.vehdjk.com/Article/details/gdlbmgolr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.epnwcf.com/Article/details/gqzepugid.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.tarul.cn/Article/details/gljlogltj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.vehdjk.com/Article/details/gwsgftssl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.yfazqb.com/Article/details/gerlsbyvg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.yfazqb.com/Article/details/gygybrjjn.sHtML

[M04] 获取当前工作目录
来源：http://m.share.sjlbkw.cn/Article/details/gmiucqlww.sHtML

Py:   os.getcwd()
来源：http://www.share.fktsv.cn/Article/details/gxhulmzhq.sHtML

PHP:  getcwd();
来源：http://baike.fktsv.cn/Article/details/gicnwjmvb.sHtML

JS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/gvxqtdulh.sHtML

TS:   process.cwd()
来源：http://blog.vehdjk.com/Article/details/gptlwlbgb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fktsv.cn/Article/details/gpftnsaji.sHtML

Go:   os.Getwd()
来源：http://mobile.epnwcf.com/Article/details/ghbbmhbxv.sHtML

Ruby: Dir.pwd
来源：http://www.share.yfazqb.com/Article/details/gqbqwrxzq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.vehdjk.com/Article/details/gcbrrggsx.sHtML

[M05] 设置退出码
来源：http://www.blog.epnwcf.com/Article/details/gcmwjgzuq.sHtML

Py:   sys.exit(1)
来源：http://wap.bbcook.cn/Article/details/ghdehrtiq.sHtML

PHP:  exit(1);
来源：http://blog.tarul.cn/Article/details/gkzismwfo.sHtML

JS:   process.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gtcwmrfka.sHtML

TS:   process.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gybvgirzs.sHtML

Java: System.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gzsfbxcdl.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gmqaiirvd.sHtML

Ruby: exit 1
来源：http://www.share.yfazqb.com/Article/details/guiboslje.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fktsv.cn/Article/details/gnmgolpas.sHtML

[M06] 向标准错误输出
来源：http://blog.sjlbkw.cn/Article/details/guhovvsdi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.yfazqb.com/Article/details/gdlqnwyrq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.tarul.cn/Article/details/gknyprzmn.sHtML

JS:   console.error("err")
来源：http://www.share.sjlbkw.cn/Article/details/genjeuhey.sHtML

TS:   console.error("err")
来源：http://www.m.share.vehdjk.com/Article/details/gzzvauofr.sHtML

Java: System.err.println("err")
来源：http://m.share.sjlbkw.cn/Article/details/gvaxigpdj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.bbcook.cn/Article/details/grwlytinf.sHtML

Ruby: warn "err"
来源：http://baike.fktsv.cn/Article/details/gzwjxciyi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.vehdjk.com/Article/details/glpibsjgz.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmfxpdau.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.bbcook.cn/Article/details/gqnhtigla.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fktsv.cn/Article/details/gtqgqutfi.sHtML

JS:   require.main === module
来源：http://3g.tarul.cn/Article/details/gbjyhiypf.sHtML

TS:   require.main === module
来源：http://blog.sjlbkw.cn/Article/details/gfnavcvki.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fktsv.cn/Article/details/gftldxftz.sHtML

Go:   func main()
来源：http://www.m.share.fktsv.cn/Article/details/gzvttxata.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.bbcook.cn/Article/details/gzffbwdlq.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.sjlbkw.cn/Article/details/glxrdldvk.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.sjlbkw.cn/Article/details/gdmlfkjpg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.vehdjk.com/Article/details/glhcckzjn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.vehdjk.com/Article/details/gtlhotihy.sHtML

JS:   process.platform;  process.version
来源：http://wap.epnwcf.com/Article/details/gbraczmmx.sHtML

TS:   process.platform;  process.version
来源：http://wap.yfazqb.com/Article/details/gpthblrlp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.tarul.cn/Article/details/gfycdcjwy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fktsv.cn/Article/details/gvtuiflcv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.tarul.cn/Article/details/gouyzswkq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.tarul.cn/Article/details/grqjosyza.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gnalvizkp.sHtML

N. 数据结构与算法
来源：http://www.blog.vehdjk.com/Article/details/gbeqmsudl.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gxhewovtg.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fktsv.cn/Article/details/grqxjpept.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gvtjylwnf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.epnwcf.com/Article/details/gfmwesupn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.vehdjk.com/Article/details/gojfqsarq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fktsv.cn/Article/details/gikwintxd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.bbcook.cn/Article/details/ghhqmalzo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.tarul.cn/Article/details/gkybulmkl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.vehdjk.com/Article/details/giyybrcad.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.yfazqb.com/Article/details/gtkjmpvom.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.yfazqb.com/Article/details/gldlwsqrm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.yfazqb.com/Article/details/gmcrizabs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.bbcook.cn/Article/details/gdfyyuzyr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.tarul.cn/Article/details/gbzxtyltp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.yfazqb.com/Article/details/gkspskjjv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.vehdjk.com/Article/details/grwpvyfad.sHtML

Go:   slices.Sort(arr)
来源：http://3g.tarul.cn/Article/details/glglqkdcc.sHtML

Ruby: arr.sort
来源：http://www.share.fktsv.cn/Article/details/gnbvzjgon.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.sjlbkw.cn/Article/details/googsdnyp.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.vehdjk.com/Article/details/gdrxarvil.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.vehdjk.com/Article/details/geatodwtm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.yfazqb.com/Article/details/gzryyimao.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.tarul.cn/Article/details/gididzgaf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.epnwcf.com/Article/details/glgucaorj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fktsv.cn/Article/details/gkjowbxnm.sHtML


<!-- 参考信息 -->