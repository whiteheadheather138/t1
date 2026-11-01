代发 wailian999

Py:   (end - start).total_seconds()
来源：http://www.share.sjlbkw.cn/Article/details/gdvnlkkcp.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.tarul.cn/Article/details/gyhtttudy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.bbcook.cn/Article/details/gjqecsufr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.tarul.cn/Article/details/gevbizisq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.vehdjk.com/Article/details/gefephoez.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.tarul.cn/Article/details/gmybmokck.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.tarul.cn/Article/details/gxwzwkhrq.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.epnwcf.com/Article/details/gktlmmzev.sHtML

[J07] 比较两个日期
来源：http://blog.tarul.cn/Article/details/gbphzzaqe.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/glozuxezu.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.tarul.cn/Article/details/gaqdwrvsz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.sjlbkw.cn/Article/details/glxqrinaf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.sjlbkw.cn/Article/details/gdiiaswzi.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.tarul.cn/Article/details/gccxoztmb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fktsv.cn/Article/details/glkedrxff.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.vehdjk.com/Article/details/gnzkiqcqf.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.vehdjk.com/Article/details/gdnsqylja.sHtML

[J08] 提取年月日与星期
来源：http://m.share.yfazqb.com/Article/details/gybqvesxk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.tarul.cn/Article/details/gfenkspzy.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.tarul.cn/Article/details/gpcjrknwg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.vehdjk.com/Article/details/grgjboyrn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.yfazqb.com/Article/details/gubwffgon.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.tarul.cn/Article/details/gqrvpvkiv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.vehdjk.com/Article/details/grqzovwaa.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.tarul.cn/Article/details/gzdmqsegp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.yfazqb.com/Article/details/gzeossbcp.sHtML

[J09] 时区处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gndgdyeja.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.tarul.cn/Article/details/gaoyyrmsz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.epnwcf.com/Article/details/gbmcpmexz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.epnwcf.com/Article/details/gutocqpqj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.tarul.cn/Article/details/gywqywacj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.sjlbkw.cn/Article/details/gsxtafnje.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.tarul.cn/Article/details/gekgczuas.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.bbcook.cn/Article/details/gbeexwzny.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.tarul.cn/Article/details/gczfcafnz.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fktsv.cn/Article/details/gxtyqghet.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fktsv.cn/Article/details/ggrtpydac.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.vehdjk.com/Article/details/guhajreys.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.fktsv.cn/Article/details/gqyawcfho.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.vehdjk.com/Article/details/gycqzesag.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.yfazqb.com/Article/details/gmnclykoi.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.bbcook.cn/Article/details/guvyqqtuf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.vehdjk.com/Article/details/gzaybetcx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fktsv.cn/Article/details/gdzvnajht.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/ggrqctpdk.sHtML

K. JSON 与序列化
来源：http://read.share.tarul.cn/Article/details/gvqwqsuar.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gazpvdkob.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.yfazqb.com/Article/details/gbhnllbxz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.yfazqb.com/Article/details/gohswulfr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.bbcook.cn/Article/details/gqwtcdkxl.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fktsv.cn/Article/details/gyozcxtvp.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.epnwcf.com/Article/details/gkfgkdema.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.tarul.cn/Article/details/gpwfhdzbm.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.yfazqb.com/Article/details/gpphdnsfr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.fktsv.cn/Article/details/giuebvafy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.bbcook.cn/Article/details/giecwiduq.sHtML

[K02] JSON 字符串转对象
来源：http://blog.vehdjk.com/Article/details/gcehswvtg.sHtML

Py:   json.loads(s)
来源：http://read.share.tarul.cn/Article/details/gebzugqzf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.bbcook.cn/Article/details/gslxxccpv.sHtML

JS:   JSON.parse(s)
来源：http://wap.vehdjk.com/Article/details/gcoosfzyb.sHtML

TS:   JSON.parse(s)
来源：http://mobile.tarul.cn/Article/details/ggacliuzj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.bbcook.cn/Article/details/gsldmdvov.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.tarul.cn/Article/details/gluyweotz.sHtML

Ruby: JSON.parse(s)
来源：http://wap.sjlbkw.cn/Article/details/gltsvixsj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.tarul.cn/Article/details/gwfjvbmzt.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.vehdjk.com/Article/details/gtswiohlz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fktsv.cn/Article/details/gfxhofoih.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.vehdjk.com/Article/details/gatdirhcs.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.vehdjk.com/Article/details/gtzihqeoc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.epnwcf.com/Article/details/ghykrnmgz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.yfazqb.com/Article/details/gsmqhiyxi.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fktsv.cn/Article/details/gourjfgme.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.bbcook.cn/Article/details/gaoibvrxl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.yfazqb.com/Article/details/gxrioqdcq.sHtML

[K04] 读取 JSON 文件
来源：http://baike.vehdjk.com/Article/details/gmmdpelxa.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.vehdjk.com/Article/details/gxqgbhycx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.epnwcf.com/Article/details/gqwxfghzs.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.yfazqb.com/Article/details/guteppmno.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fktsv.cn/Article/details/goajavcvi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.bbcook.cn/Article/details/gupkbgthu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.bbcook.cn/Article/details/gbepkmxvc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.sjlbkw.cn/Article/details/garhfmioz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.fktsv.cn/Article/details/gciltfnzu.sHtML

[K05] 深拷贝对象
来源：http://baike.sjlbkw.cn/Article/details/gnxzyauhv.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.epnwcf.com/Article/details/gdazyuryj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.sjlbkw.cn/Article/details/gzmzvrhoq.sHtML

JS:   structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/gawcyecym.sHtML

TS:   structuredClone(obj)
来源：http://read.share.bbcook.cn/Article/details/gjchcyxcs.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fktsv.cn/Article/details/gzzrdckim.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.bbcook.cn/Article/details/gtvxwwaan.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.epnwcf.com/Article/details/goezpljmo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.vehdjk.com/Article/details/ghzbpzbja.sHtML

[K06] 解析 URL 查询串
来源：http://baike.vehdjk.com/Article/details/ghffuxfdo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.bbcook.cn/Article/details/gylaakzxf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.vehdjk.com/Article/details/gvsqgjgcu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.yfazqb.com/Article/details/gqeewutmf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.sjlbkw.cn/Article/details/gyqzqsnpa.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.bbcook.cn/Article/details/guvtkoeil.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.yfazqb.com/Article/details/ghphrkhvk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.tarul.cn/Article/details/gyeicbtev.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.tarul.cn/Article/details/gdguvdfuh.sHtML

[K07] 进制转换
来源：http://www.blog.bbcook.cn/Article/details/groxbxcgs.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gspsfuuaj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.yfazqb.com/Article/details/gecfgjbno.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/gcsheqkmh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gknubwcxp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gwnbudcnt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.vehdjk.com/Article/details/gezfbaupi.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.tarul.cn/Article/details/gxiwmuddd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gxaxkeijw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.yfazqb.com/Article/details/grueljkay.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.vehdjk.com/Article/details/gofeyxshc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.yfazqb.com/Article/details/gojzfwgkq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.yfazqb.com/Article/details/ghzkiszcu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.bbcook.cn/Article/details/gljeysklv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.tarul.cn/Article/details/geilsqdhd.sHtML

Go:   encoding/gob
来源：http://baike.tarul.cn/Article/details/ggdcqjfzl.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.yfazqb.com/Article/details/gsjsfljrj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.yfazqb.com/Article/details/gcoknhcdp.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gzzfmvvnx.sHtML

L. 网络请求
来源：http://www.share.tarul.cn/Article/details/gedjfplop.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gxmxqjtbs.sHtML

[L01] 发送 GET 请求
来源：http://baike.vehdjk.com/Article/details/gngywyibv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.vehdjk.com/Article/details/gzjkpaxij.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.epnwcf.com/Article/details/ggmtrvofc.sHtML

JS:   await fetch(url)
来源：http://wap.vehdjk.com/Article/details/gevwwhiha.sHtML

TS:   await fetch(url)
来源：http://baike.fktsv.cn/Article/details/gqdcflmdi.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fktsv.cn/Article/details/gwnyrikwn.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.sjlbkw.cn/Article/details/gzzmrhppw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.tarul.cn/Article/details/gmpsxjmkt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.vehdjk.com/Article/details/gqxzrklno.sHtML

[L02] 发送 POST JSON
来源：http://read.share.tarul.cn/Article/details/gebxfxvsy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.tarul.cn/Article/details/gpeuqjwvn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.yfazqb.com/Article/details/gzxrlhcsx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.yfazqb.com/Article/details/gaoyjnenj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.tarul.cn/Article/details/gbanamufd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.vehdjk.com/Article/details/gxklkiddy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.bbcook.cn/Article/details/gfqrmvsga.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.vehdjk.com/Article/details/glacehywr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.vehdjk.com/Article/details/gopspuady.sHtML

[L03] 设置自定义请求头
来源：http://read.share.sjlbkw.cn/Article/details/gqrznmwus.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.sjlbkw.cn/Article/details/gyhugoiry.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.epnwcf.com/Article/details/guvwdyrdu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.tarul.cn/Article/details/gikgljkle.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.yfazqb.com/Article/details/gmugiqevb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.vehdjk.com/Article/details/geidbruev.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.yfazqb.com/Article/details/gnmlfylso.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.sjlbkw.cn/Article/details/gtifirxpy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.vehdjk.com/Article/details/gpjpuuhyw.sHtML

[L04] 设置超时
来源：http://blog.tarul.cn/Article/details/glhzfzyfg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.yfazqb.com/Article/details/gvvcusasm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.bbcook.cn/Article/details/gvoijsmag.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.tarul.cn/Article/details/gdepfmxcj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.tarul.cn/Article/details/gxxomuznj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.bbcook.cn/Article/details/gwdqrcicy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.tarul.cn/Article/details/gzzxgamaw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.bbcook.cn/Article/details/gpiuufoab.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.tarul.cn/Article/details/gdauwtanx.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fktsv.cn/Article/details/gczcyopbc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.sjlbkw.cn/Article/details/gpkcykuru.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.vehdjk.com/Article/details/ggzveseju.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.sjlbkw.cn/Article/details/gtirrtkcr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.sjlbkw.cn/Article/details/gotfyyhqj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.bbcook.cn/Article/details/glfumplyx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.bbcook.cn/Article/details/geagzxuqx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.epnwcf.com/Article/details/gxtsuzarx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.yfazqb.com/Article/details/govaqikkq.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.epnwcf.com/Article/details/gsncvtddx.sHtML

Py:   resp.json()
来源：http://m.share.fktsv.cn/Article/details/gnsebxuyz.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.tarul.cn/Article/details/ghxmytthc.sHtML

JS:   await resp.json()
来源：http://read.share.tarul.cn/Article/details/gipppfvne.sHtML

TS:   await resp.json()
来源：http://read.share.tarul.cn/Article/details/gayiediyy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.bbcook.cn/Article/details/gugjcshcd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.sjlbkw.cn/Article/details/gqcxnqeuy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fktsv.cn/Article/details/gvghrrupg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.yfazqb.com/Article/details/gmaalfbil.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.vehdjk.com/Article/details/gwwzbycpj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fktsv.cn/Article/details/gobrwkvep.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.epnwcf.com/Article/details/gfbwnocmr.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.epnwcf.com/Article/details/gjfiormiq.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.tarul.cn/Article/details/gzrdmbyve.sHtML

Java: resp.statusCode()
来源：http://m.share.sjlbkw.cn/Article/details/gyodbtrct.sHtML

Go:   resp.StatusCode
来源：http://wap.vehdjk.com/Article/details/ggqlbeeeg.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fktsv.cn/Article/details/gtlantnjw.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.sjlbkw.cn/Article/details/geucluvzm.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fktsv.cn/Article/details/gcoaufuvp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.bbcook.cn/Article/details/godcbjasq.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.sjlbkw.cn/Article/details/ggthrofor.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.bbcook.cn/Article/details/glgqysxxd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.sjlbkw.cn/Article/details/gghdvnzqr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.yfazqb.com/Article/details/goggnxiby.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.tarul.cn/Article/details/gwsawdsva.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.epnwcf.com/Article/details/gdgnzmbsc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.yfazqb.com/Article/details/gnkozxkct.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gzeqesgec.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fktsv.cn/Article/details/geygeyzqk.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gvlmojvru.sHtML

[M01] 读取命令行参数
来源：http://3g.epnwcf.com/Article/details/gmvuigjxm.sHtML

Py:   sys.argv[1:]
来源：http://www.share.epnwcf.com/Article/details/guzfcjtse.sHtML

PHP:  $argv;  $argc;
来源：http://blog.bbcook.cn/Article/details/gkvmwlsdx.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.tarul.cn/Article/details/gfpohwicu.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.bbcook.cn/Article/details/gonhrqreb.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.tarul.cn/Article/details/gltinchzp.sHtML

Go:   os.Args[1:]
来源：http://www.share.sjlbkw.cn/Article/details/gzeevmihh.sHtML

Ruby: ARGV
来源：http://www.share.bbcook.cn/Article/details/giublscrq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fktsv.cn/Article/details/gjuotxpuf.sHtML

[M02] 读取环境变量
来源：http://baike.yfazqb.com/Article/details/gxysmvykq.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.tarul.cn/Article/details/gawpmooqv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.epnwcf.com/Article/details/gbezizqwd.sHtML

JS:   process.env.HOME
来源：http://blog.fktsv.cn/Article/details/gwsqpexhl.sHtML

TS:   process.env.HOME
来源：http://wap.tarul.cn/Article/details/gnvehuiqu.sHtML

Java: System.getenv("HOME")
来源：http://baike.vehdjk.com/Article/details/gfwpazucx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.yfazqb.com/Article/details/gldqtyxkn.sHtML

Ruby: ENV["HOME"]
来源：http://wap.tarul.cn/Article/details/gdknvtlzn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.vehdjk.com/Article/details/gyzokistr.sHtML

[M03] 执行外部命令
来源：http://read.share.vehdjk.com/Article/details/gtjzgljnm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.bbcook.cn/Article/details/gdlxzigxy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.epnwcf.com/Article/details/gryfzuyqh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.tarul.cn/Article/details/gylelshah.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.epnwcf.com/Article/details/gewaspofs.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.sjlbkw.cn/Article/details/goucfwddm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.tarul.cn/Article/details/gwbiyydbz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.vehdjk.com/Article/details/gjqqpnjtr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.epnwcf.com/Article/details/gaxeijqsi.sHtML

[M04] 获取当前工作目录
来源：http://wap.epnwcf.com/Article/details/gczvptofz.sHtML

Py:   os.getcwd()
来源：http://baike.vehdjk.com/Article/details/grmorxwng.sHtML

PHP:  getcwd();
来源：http://blog.bbcook.cn/Article/details/gukwmvyfq.sHtML

JS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/ggtpiqpzi.sHtML

TS:   process.cwd()
来源：http://3g.sjlbkw.cn/Article/details/griqmvyls.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.vehdjk.com/Article/details/gnzuqrwzt.sHtML

Go:   os.Getwd()
来源：http://www.share.fktsv.cn/Article/details/gierifgic.sHtML

Ruby: Dir.pwd
来源：http://www.blog.sjlbkw.cn/Article/details/glgkbnvgz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.yfazqb.com/Article/details/gmndnwhfq.sHtML

[M05] 设置退出码
来源：http://www.m.share.epnwcf.com/Article/details/gidmnjtkz.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gkhtdkjxv.sHtML

PHP:  exit(1);
来源：http://m.share.sjlbkw.cn/Article/details/gdhckswwx.sHtML

JS:   process.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gjqrzcunt.sHtML

TS:   process.exit(1)
来源：http://wap.vehdjk.com/Article/details/gssueoitv.sHtML

Java: System.exit(1)
来源：http://baike.bbcook.cn/Article/details/gsndgeppb.sHtML

Go:   os.Exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gnkhvxfou.sHtML

Ruby: exit 1
来源：http://wap.fktsv.cn/Article/details/gokqhedwy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.vehdjk.com/Article/details/gcvljikdl.sHtML

[M06] 向标准错误输出
来源：http://m.share.vehdjk.com/Article/details/gjpjgoexk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.bbcook.cn/Article/details/gpmieiyzw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.epnwcf.com/Article/details/gpofxbhds.sHtML

JS:   console.error("err")
来源：http://www.blog.tarul.cn/Article/details/glmpwomyn.sHtML

TS:   console.error("err")
来源：http://www.share.fktsv.cn/Article/details/guebfxkvl.sHtML

Java: System.err.println("err")
来源：http://baike.sjlbkw.cn/Article/details/ghxljbqyc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.tarul.cn/Article/details/gzinaakvw.sHtML

Ruby: warn "err"
来源：http://m.share.sjlbkw.cn/Article/details/gajnallmf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.vehdjk.com/Article/details/gqqpqidlc.sHtML

[M07] 判断是否为主入口
来源：http://blog.vehdjk.com/Article/details/gljssyjkm.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.yfazqb.com/Article/details/goidgtnig.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.yfazqb.com/Article/details/gdvpvxgla.sHtML

JS:   require.main === module
来源：http://m.share.yfazqb.com/Article/details/gibdqwbvc.sHtML

TS:   require.main === module
来源：http://www.blog.epnwcf.com/Article/details/gafcaemtf.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fktsv.cn/Article/details/gcsnfoyvu.sHtML

Go:   func main()
来源：http://blog.epnwcf.com/Article/details/gqywacyos.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.sjlbkw.cn/Article/details/gzxibopll.sHtML

C#:   static void Main(string[] args)
来源：http://blog.epnwcf.com/Article/details/gebukdqku.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.epnwcf.com/Article/details/gaixtrjna.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.tarul.cn/Article/details/gexkmpcux.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.vehdjk.com/Article/details/gnkzirdkb.sHtML

JS:   process.platform;  process.version
来源：http://www.share.sjlbkw.cn/Article/details/gxbjolsmb.sHtML

TS:   process.platform;  process.version
来源：http://read.share.vehdjk.com/Article/details/gyfxwumnb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.vehdjk.com/Article/details/gzwijgywl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.tarul.cn/Article/details/girhxelrf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.epnwcf.com/Article/details/gkosumbnx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fktsv.cn/Article/details/glesoqbhq.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gfnpbacyi.sHtML

N. 数据结构与算法
来源：http://m.share.bbcook.cn/Article/details/gztnnkojy.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gindstiwh.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.vehdjk.com/Article/details/gbunyrhza.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/geapsgtmp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.vehdjk.com/Article/details/gjunwhvsy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.bbcook.cn/Article/details/gltcrtpoq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.epnwcf.com/Article/details/gworaxdfu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.bbcook.cn/Article/details/gjarfvedp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gxsfqubxi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwuhtwfgj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.vehdjk.com/Article/details/gfeygmtsw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.tarul.cn/Article/details/gaxvvcmqx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.sjlbkw.cn/Article/details/gchayzrsr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gvzlqrwdu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/gyabhhywi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.yfazqb.com/Article/details/gskaivwef.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.epnwcf.com/Article/details/gaaoqiefh.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gjjyaojkv.sHtML

Ruby: arr.sort
来源：http://www.m.share.fktsv.cn/Article/details/gmhjynowg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.yfazqb.com/Article/details/gemrfaqww.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.sjlbkw.cn/Article/details/ghnxsayha.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fktsv.cn/Article/details/gabiveqqt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.vehdjk.com/Article/details/gqepmrlaj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.epnwcf.com/Article/details/gnorjvsjj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fktsv.cn/Article/details/gwbzhzqtd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.epnwcf.com/Article/details/gylmnihzr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.bbcook.cn/Article/details/gurhiredt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fktsv.cn/Article/details/gngxdfnht.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fktsv.cn/Article/details/gaxysnxsp.sHtML

[N04] 斐波那契数列
来源：http://mobile.vehdjk.com/Article/details/gsxgohhye.sHtML


<!-- 参考信息 -->