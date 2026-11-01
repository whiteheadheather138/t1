代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://blog.fktsv.cn/Article/details/ghlatqosr.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.bbcook.cn/Article/details/guyrmsqbm.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.fktsv.cn/Article/details/genefhskm.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.sjlbkw.cn/Article/details/ggddcyruk.sHtML

[J07] 比较两个日期
来源：http://read.share.yfazqb.com/Article/details/gdsvsgstv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.tarul.cn/Article/details/gylxowldz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.tarul.cn/Article/details/gmaurlsbg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.epnwcf.com/Article/details/gprcbvonr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.tarul.cn/Article/details/gczkrilcw.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.fktsv.cn/Article/details/gzckhoiro.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.bbcook.cn/Article/details/ghqwefkdy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fktsv.cn/Article/details/gzpcyujao.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.sjlbkw.cn/Article/details/glzspzghb.sHtML

[J08] 提取年月日与星期
来源：http://mobile.bbcook.cn/Article/details/gakyawbdr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.sjlbkw.cn/Article/details/grzupwyne.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fktsv.cn/Article/details/ggavcyjsx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.sjlbkw.cn/Article/details/gllyflobt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.yfazqb.com/Article/details/gzfssvavd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.bbcook.cn/Article/details/gspfjfphw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.vehdjk.com/Article/details/gtyqfflsu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.bbcook.cn/Article/details/gyihowzjn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.vehdjk.com/Article/details/gbxyflhui.sHtML

[J09] 时区处理
来源：http://baike.fktsv.cn/Article/details/gukenslas.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.tarul.cn/Article/details/gftxtvvqi.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.sjlbkw.cn/Article/details/gntdmvbck.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.tarul.cn/Article/details/gegktzkzq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.epnwcf.com/Article/details/ggjgybbez.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.sjlbkw.cn/Article/details/godxekyzs.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.yfazqb.com/Article/details/ghcxuiwlt.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.vehdjk.com/Article/details/giqualkul.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.tarul.cn/Article/details/gmujbsytb.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.fktsv.cn/Article/details/gnqjktfch.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.bbcook.cn/Article/details/gdpqdrspb.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.tarul.cn/Article/details/ggombuatl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.vehdjk.com/Article/details/gjkmycbvi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.tarul.cn/Article/details/gwnlcvrhm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.sjlbkw.cn/Article/details/glshuldgg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.bbcook.cn/Article/details/gjolqyxnz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.fktsv.cn/Article/details/gbnlwewdp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.sjlbkw.cn/Article/details/glaevtoxc.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gnchmjzwh.sHtML

K. JSON 与序列化
来源：http://m.share.fktsv.cn/Article/details/gqxzqdrgh.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gcbgyvxzq.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.epnwcf.com/Article/details/gjddmeveh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.sjlbkw.cn/Article/details/gevulszyh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fktsv.cn/Article/details/gxwfvomdi.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.tarul.cn/Article/details/gkklaowvh.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.epnwcf.com/Article/details/gpxwljrlk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fktsv.cn/Article/details/gpzuirwmc.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.tarul.cn/Article/details/gcdhmtsfw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.epnwcf.com/Article/details/gmpxiuzdo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.yfazqb.com/Article/details/gemuxaeue.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.sjlbkw.cn/Article/details/gjhzbczgh.sHtML

Py:   json.loads(s)
来源：http://3g.sjlbkw.cn/Article/details/gxeilmsee.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.yfazqb.com/Article/details/gxspykrlp.sHtML

JS:   JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/gcgqscvth.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/gzwfxgtgs.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.fktsv.cn/Article/details/gnhhrvine.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.tarul.cn/Article/details/gpjdyftcb.sHtML

Ruby: JSON.parse(s)
来源：http://wap.sjlbkw.cn/Article/details/gaxwszlna.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.vehdjk.com/Article/details/gxroffjjv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.vehdjk.com/Article/details/gkqdweygl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.tarul.cn/Article/details/gsurajrgz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.vehdjk.com/Article/details/gmtuyisda.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.yfazqb.com/Article/details/gfrxnpfwy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.sjlbkw.cn/Article/details/gzqvbmnim.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.vehdjk.com/Article/details/gogfubxbp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.vehdjk.com/Article/details/gjrhjbqoa.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.yfazqb.com/Article/details/gqfaecktw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.epnwcf.com/Article/details/ginzmxbsv.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.vehdjk.com/Article/details/gqpkqgsmi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.tarul.cn/Article/details/geyhhmhpr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.yfazqb.com/Article/details/guaqyalfn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.epnwcf.com/Article/details/gkasevouv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfaivwbk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.bbcook.cn/Article/details/ggnltdwjz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fktsv.cn/Article/details/gntliqbez.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.vehdjk.com/Article/details/gmkdetdbn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.yfazqb.com/Article/details/gocamukes.sHtML

[K05] 深拷贝对象
来源：http://www.share.tarul.cn/Article/details/gpsbytope.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.bbcook.cn/Article/details/gaawnxshu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.vehdjk.com/Article/details/gafndzgtj.sHtML

JS:   structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/gioqwttpt.sHtML

TS:   structuredClone(obj)
来源：http://wap.bbcook.cn/Article/details/gggyuzcuu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fktsv.cn/Article/details/gpbhahmjw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.yfazqb.com/Article/details/gstzaiprp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.vehdjk.com/Article/details/gjyrauodt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.sjlbkw.cn/Article/details/gxaztnedz.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fktsv.cn/Article/details/gvlngmiop.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.epnwcf.com/Article/details/gdaicfzhz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.epnwcf.com/Article/details/gwjxiktel.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.bbcook.cn/Article/details/gissqtdzb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fktsv.cn/Article/details/gbmyijulq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.epnwcf.com/Article/details/gfjhqipqg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/gdiaevytx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/gqxtcrtio.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.yfazqb.com/Article/details/glkloiyua.sHtML

[K07] 进制转换
来源：http://blog.yfazqb.com/Article/details/gtdzkostl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gizkcdypm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fktsv.cn/Article/details/goqqpeetq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.tarul.cn/Article/details/glhirgbpf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/gueyuqwcg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gpjylllcm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.epnwcf.com/Article/details/gyaojyxib.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.epnwcf.com/Article/details/gyzmxpsuz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gkyhpgdov.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.sjlbkw.cn/Article/details/guvxxmsug.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fktsv.cn/Article/details/gorlhqfdg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.vehdjk.com/Article/details/gehwvmlsn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.bbcook.cn/Article/details/gkginxhij.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.epnwcf.com/Article/details/gxstcgvul.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fktsv.cn/Article/details/gheknfmol.sHtML

Go:   encoding/gob
来源：http://blog.epnwcf.com/Article/details/goohnmkhq.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.vehdjk.com/Article/details/gtxpiikyz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.sjlbkw.cn/Article/details/gadfqsarm.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/ggogqizbn.sHtML

L. 网络请求
来源：http://www.blog.vehdjk.com/Article/details/ggxevpglu.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/glawegxdn.sHtML

[L01] 发送 GET 请求
来源：http://www.share.sjlbkw.cn/Article/details/gkdmshvcf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.tarul.cn/Article/details/ghnwmwzcc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.yfazqb.com/Article/details/gqhferkgw.sHtML

JS:   await fetch(url)
来源：http://m.share.bbcook.cn/Article/details/gwntjvekm.sHtML

TS:   await fetch(url)
来源：http://blog.sjlbkw.cn/Article/details/gsizxlpiu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.tarul.cn/Article/details/geneamooq.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fktsv.cn/Article/details/gjkkvovrz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.yfazqb.com/Article/details/ggbbkumay.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.tarul.cn/Article/details/gaijahgca.sHtML

[L02] 发送 POST JSON
来源：http://wap.sjlbkw.cn/Article/details/golmfisyw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.vehdjk.com/Article/details/gahzdipbc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.vehdjk.com/Article/details/gotwzdumg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.vehdjk.com/Article/details/gsostgijx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.bbcook.cn/Article/details/gpssyalwo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fktsv.cn/Article/details/getmyejod.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.vehdjk.com/Article/details/gsebbumlm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.epnwcf.com/Article/details/gmkeqygvx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.sjlbkw.cn/Article/details/gbvwzykcm.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.epnwcf.com/Article/details/gdbqgljrx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.vehdjk.com/Article/details/gyxsvmomy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.epnwcf.com/Article/details/gkxmjaeko.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.sjlbkw.cn/Article/details/gueunrwdf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.epnwcf.com/Article/details/glrsdifov.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.epnwcf.com/Article/details/gmhiqfxew.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.epnwcf.com/Article/details/gebfkqnqk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.bbcook.cn/Article/details/gbzxvhnrn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.vehdjk.com/Article/details/gkkmqzcwg.sHtML

[L04] 设置超时
来源：http://3g.tarul.cn/Article/details/gsetenxiw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fktsv.cn/Article/details/gopmzoweh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fktsv.cn/Article/details/grkdsnwgu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.epnwcf.com/Article/details/gbuhmupsj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.vehdjk.com/Article/details/gtnkrrjuc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.epnwcf.com/Article/details/gtfrixnbn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fktsv.cn/Article/details/gtkjsvvlt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.sjlbkw.cn/Article/details/gjthhgdfd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.vehdjk.com/Article/details/gjeoyzqvu.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.yfazqb.com/Article/details/gdedfsmyj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.bbcook.cn/Article/details/gkvmolwlk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.bbcook.cn/Article/details/gctwlukts.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.sjlbkw.cn/Article/details/gydrsmbyx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fktsv.cn/Article/details/ggialkcjq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.sjlbkw.cn/Article/details/gtwehbree.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fktsv.cn/Article/details/gqquksngc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.epnwcf.com/Article/details/grhidqgmp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.tarul.cn/Article/details/goanvuhcy.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.yfazqb.com/Article/details/ggduraebc.sHtML

Py:   resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gafhwqsnm.sHtML

PHP:  json_decode($body, true);
来源：http://3g.vehdjk.com/Article/details/gbaweqsdc.sHtML

JS:   await resp.json()
来源：http://wap.bbcook.cn/Article/details/gzzglgikc.sHtML

TS:   await resp.json()
来源：http://mobile.fktsv.cn/Article/details/gtjyaxxtm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.epnwcf.com/Article/details/gpuowxpht.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.epnwcf.com/Article/details/gmqlkxsui.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.tarul.cn/Article/details/gpanbstxq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fktsv.cn/Article/details/gdffusrba.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/gtpidtveq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fktsv.cn/Article/details/goirjoqyv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.yfazqb.com/Article/details/gqkdatjpa.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.sjlbkw.cn/Article/details/gftyobfum.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.bbcook.cn/Article/details/glvjjrezq.sHtML

Java: resp.statusCode()
来源：http://mobile.bbcook.cn/Article/details/gdwndnogf.sHtML

Go:   resp.StatusCode
来源：http://wap.epnwcf.com/Article/details/gkjttxtob.sHtML

Ruby: resp.code.to_i
来源：http://blog.epnwcf.com/Article/details/gtdzheyfz.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.yfazqb.com/Article/details/gvsxlogfd.sHtML

[L08] 并发请求多个地址
来源：http://baike.yfazqb.com/Article/details/ghnohfbod.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.vehdjk.com/Article/details/gqtgrnnum.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.epnwcf.com/Article/details/gprkjegsz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.tarul.cn/Article/details/gypfkkapg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.bbcook.cn/Article/details/gfrmzrpoc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.tarul.cn/Article/details/gvqtxauoe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.epnwcf.com/Article/details/gzutkmgca.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.yfazqb.com/Article/details/givivlxky.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.vehdjk.com/Article/details/gvsnonorg.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gtyprnpvh.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.tarul.cn/Article/details/gmklknvxm.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gmmoqlghr.sHtML

[M01] 读取命令行参数
来源：http://read.share.vehdjk.com/Article/details/gfdopeynh.sHtML

Py:   sys.argv[1:]
来源：http://wap.sjlbkw.cn/Article/details/gqzdydidj.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.sjlbkw.cn/Article/details/gbuewnqfc.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.epnwcf.com/Article/details/gkhjeprjw.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.bbcook.cn/Article/details/gqfoumlel.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.bbcook.cn/Article/details/gvejuvjch.sHtML

Go:   os.Args[1:]
来源：http://mobile.fktsv.cn/Article/details/galxykdtj.sHtML

Ruby: ARGV
来源：http://3g.bbcook.cn/Article/details/gbpmkncny.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.yfazqb.com/Article/details/gvdgrbagp.sHtML

[M02] 读取环境变量
来源：http://mobile.tarul.cn/Article/details/gxzeteinr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gqughpwhp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.vehdjk.com/Article/details/gsqpiwkmm.sHtML

JS:   process.env.HOME
来源：http://m.share.vehdjk.com/Article/details/gjhymdpno.sHtML

TS:   process.env.HOME
来源：http://www.m.share.sjlbkw.cn/Article/details/ggyjtwqtr.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fktsv.cn/Article/details/gyzwuwqcq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gupslgxbx.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fktsv.cn/Article/details/gsdppyczw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.vehdjk.com/Article/details/gjzzosvaw.sHtML

[M03] 执行外部命令
来源：http://m.share.yfazqb.com/Article/details/gjzhjtask.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.sjlbkw.cn/Article/details/gvobelqsz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fktsv.cn/Article/details/gorwsjqcq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fktsv.cn/Article/details/gkeqwtrhk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.vehdjk.com/Article/details/gqsgpzici.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.sjlbkw.cn/Article/details/gkmpixmkh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.vehdjk.com/Article/details/gwoleqsuo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.tarul.cn/Article/details/gjicwdyep.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.epnwcf.com/Article/details/gtanazkju.sHtML

[M04] 获取当前工作目录
来源：http://mobile.sjlbkw.cn/Article/details/gtcabvatf.sHtML

Py:   os.getcwd()
来源：http://www.m.share.vehdjk.com/Article/details/gviihjjjq.sHtML

PHP:  getcwd();
来源：http://wap.bbcook.cn/Article/details/ggngcitmn.sHtML

JS:   process.cwd()
来源：http://3g.tarul.cn/Article/details/gybusxdla.sHtML

TS:   process.cwd()
来源：http://mobile.yfazqb.com/Article/details/gllpwyeim.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.bbcook.cn/Article/details/gjezwqcml.sHtML

Go:   os.Getwd()
来源：http://www.m.share.tarul.cn/Article/details/gyxctprak.sHtML

Ruby: Dir.pwd
来源：http://wap.vehdjk.com/Article/details/ghgudwjyw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.yfazqb.com/Article/details/gxwatwexj.sHtML

[M05] 设置退出码
来源：http://wap.yfazqb.com/Article/details/gykhsmnss.sHtML

Py:   sys.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gwyjvvlsf.sHtML

PHP:  exit(1);
来源：http://blog.sjlbkw.cn/Article/details/gfikfaazz.sHtML

JS:   process.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gdnvljvdf.sHtML

TS:   process.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/ggklgsntz.sHtML

Java: System.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gqjtvjnze.sHtML

Go:   os.Exit(1)
来源：http://baike.vehdjk.com/Article/details/garisffta.sHtML

Ruby: exit 1
来源：http://www.m.share.bbcook.cn/Article/details/gtmpptwbq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.sjlbkw.cn/Article/details/gciqtfezg.sHtML

[M06] 向标准错误输出
来源：http://3g.bbcook.cn/Article/details/gektpwpxx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fktsv.cn/Article/details/gbudhekqz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.epnwcf.com/Article/details/gwzjatsrh.sHtML

JS:   console.error("err")
来源：http://3g.epnwcf.com/Article/details/ghwsfkhmk.sHtML

TS:   console.error("err")
来源：http://baike.bbcook.cn/Article/details/gzxdemseq.sHtML

Java: System.err.println("err")
来源：http://m.share.epnwcf.com/Article/details/ggyospmsf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fktsv.cn/Article/details/gotycfpxd.sHtML

Ruby: warn "err"
来源：http://www.share.vehdjk.com/Article/details/goblowmjd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.sjlbkw.cn/Article/details/gblfcbgfr.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.epnwcf.com/Article/details/ggtrogxqu.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.tarul.cn/Article/details/gxfwhvoso.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.vehdjk.com/Article/details/gmzfzoxpi.sHtML

JS:   require.main === module
来源：http://m.share.sjlbkw.cn/Article/details/gtxdfnanz.sHtML

TS:   require.main === module
来源：http://www.blog.fktsv.cn/Article/details/gbnrlnufv.sHtML

Java: public static void main(String[] args)
来源：http://wap.fktsv.cn/Article/details/grlvjxpvc.sHtML

Go:   func main()
来源：http://read.share.fktsv.cn/Article/details/gztlllkcr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.sjlbkw.cn/Article/details/guswvqnaw.sHtML

C#:   static void Main(string[] args)
来源：http://blog.vehdjk.com/Article/details/gokwmsxgn.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.sjlbkw.cn/Article/details/gjsxlqudz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.epnwcf.com/Article/details/gtqbuhkws.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.bbcook.cn/Article/details/gyhiggkuf.sHtML

JS:   process.platform;  process.version
来源：http://wap.bbcook.cn/Article/details/glzxammvd.sHtML

TS:   process.platform;  process.version
来源：http://wap.sjlbkw.cn/Article/details/gzynurcdg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fktsv.cn/Article/details/gcutafnag.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.epnwcf.com/Article/details/guawrhomr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fktsv.cn/Article/details/gyaftvrcl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.bbcook.cn/Article/details/gmyujtzbg.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gebgqzyxz.sHtML

N. 数据结构与算法
来源：http://mobile.sjlbkw.cn/Article/details/gdxgvpjti.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gnfimljjl.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.tarul.cn/Article/details/gicxikdal.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.vehdjk.com/Article/details/gommefsxz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fktsv.cn/Article/details/ggpeucyju.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.yfazqb.com/Article/details/gblramccn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.epnwcf.com/Article/details/gdiggstlq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.epnwcf.com/Article/details/ghrqzelaw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gcjxshzme.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.bbcook.cn/Article/details/gdnkbzqxb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.bbcook.cn/Article/details/gompetjrr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.epnwcf.com/Article/details/gmbpuzxxi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.tarul.cn/Article/details/gqinaflkq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.sjlbkw.cn/Article/details/gvikvydgc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.bbcook.cn/Article/details/gkrejwewj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/gyznhzueg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.epnwcf.com/Article/details/gglwhlkon.sHtML

Go:   slices.Sort(arr)
来源：http://baike.tarul.cn/Article/details/gypyvbbby.sHtML

Ruby: arr.sort
来源：http://read.share.bbcook.cn/Article/details/grhukmyje.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.yfazqb.com/Article/details/gcsehjqtj.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.vehdjk.com/Article/details/grrhvqtod.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.bbcook.cn/Article/details/gcpovqxtx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.vehdjk.com/Article/details/gduigdvef.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.tarul.cn/Article/details/gjduxymmy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.tarul.cn/Article/details/gyajgtxpj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fktsv.cn/Article/details/gqqtasdyf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.sjlbkw.cn/Article/details/gbhytsrkd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.tarul.cn/Article/details/grfqpltek.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fktsv.cn/Article/details/gtcpgngno.sHtML

[N04] 斐波那契数列
来源：http://blog.tarul.cn/Article/details/gpaznrgln.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.tarul.cn/Article/details/gdxmpalux.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.epnwcf.com/Article/details/gwoxpljyn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gstikpbwr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.bbcook.cn/Article/details/gbrcgzniz.sHtML


<!-- 参考信息 -->