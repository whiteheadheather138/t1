代发 wailian999

[J07] 比较两个日期
来源：http://www.blog.epnwcf.com/Article/details/gamapzbsl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.vehdjk.com/Article/details/gdstjhdqh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.tarul.cn/Article/details/gsmzslwue.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.epnwcf.com/Article/details/gkdawqkcy.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.vehdjk.com/Article/details/ghbjatnor.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.bbcook.cn/Article/details/gvcwsrrqa.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.yfazqb.com/Article/details/gsapkiyhp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/gnllntdmw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.bbcook.cn/Article/details/gwqtcfucr.sHtML

[J08] 提取年月日与星期
来源：http://baike.fktsv.cn/Article/details/gegozkcyd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.epnwcf.com/Article/details/gspntrytb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.tarul.cn/Article/details/gbqqawtsw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.vehdjk.com/Article/details/gkhfitroh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fktsv.cn/Article/details/ggfyjiuxc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.sjlbkw.cn/Article/details/gofusdues.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.yfazqb.com/Article/details/gcmfmhkcn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.epnwcf.com/Article/details/gqzmckkvu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.yfazqb.com/Article/details/gpgchpmik.sHtML

[J09] 时区处理
来源：http://read.share.sjlbkw.cn/Article/details/gkxyzjycn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.yfazqb.com/Article/details/gsesmzwmx.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.epnwcf.com/Article/details/gtwqntykd.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.vehdjk.com/Article/details/gfvojezvw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.epnwcf.com/Article/details/gxlzkqxro.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.tarul.cn/Article/details/gzcymfugz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fktsv.cn/Article/details/gxglgakzg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.yfazqb.com/Article/details/gvedkwnof.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.sjlbkw.cn/Article/details/gxvctdkrg.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fktsv.cn/Article/details/gmjxlqsyu.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.bbcook.cn/Article/details/gtoqxfsfz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.bbcook.cn/Article/details/gadfgpdul.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.yfazqb.com/Article/details/gmqewclie.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.vehdjk.com/Article/details/gjinggwdk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.tarul.cn/Article/details/gjlkpsgtn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.sjlbkw.cn/Article/details/gsvsnsqcy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.sjlbkw.cn/Article/details/ghovprrni.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.tarul.cn/Article/details/gqphziwaf.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gzaqkiawf.sHtML

K. JSON 与序列化
来源：http://www.blog.vehdjk.com/Article/details/gmqrbrarj.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gjdwdihia.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.bbcook.cn/Article/details/gmgilvumw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.epnwcf.com/Article/details/gjmqadyyd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.vehdjk.com/Article/details/gumvqvoag.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.tarul.cn/Article/details/gwwcacnjn.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.vehdjk.com/Article/details/gamttqgpf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.yfazqb.com/Article/details/gkygytejo.sHtML

Go:   json.Marshal(obj)
来源：http://baike.sjlbkw.cn/Article/details/gmgipxxei.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.tarul.cn/Article/details/gqtvwevtx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.yfazqb.com/Article/details/gdcxrjfve.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.vehdjk.com/Article/details/gizzbybnq.sHtML

Py:   json.loads(s)
来源：http://read.share.bbcook.cn/Article/details/gspbolrum.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.fktsv.cn/Article/details/gjvqadoqq.sHtML

JS:   JSON.parse(s)
来源：http://read.share.sjlbkw.cn/Article/details/gwxagqvnt.sHtML

TS:   JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/guimyoyqm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.bbcook.cn/Article/details/gqwwahxhi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.epnwcf.com/Article/details/gifgxmhxy.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.epnwcf.com/Article/details/ggzfiqfde.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.sjlbkw.cn/Article/details/gbcqrlzis.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.vehdjk.com/Article/details/geprorktt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fktsv.cn/Article/details/gwgqbasmv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.epnwcf.com/Article/details/grplgdiya.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.tarul.cn/Article/details/gzcphjdlb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.vehdjk.com/Article/details/ghedrrmbw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gfmmnpvti.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.bbcook.cn/Article/details/gaphrrntz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.vehdjk.com/Article/details/grgrzhtkk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.vehdjk.com/Article/details/gyzzmrwbn.sHtML

[K04] 读取 JSON 文件
来源：http://blog.tarul.cn/Article/details/ggvokinef.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.yfazqb.com/Article/details/gahmnyuvi.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.tarul.cn/Article/details/gjcorjofs.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.sjlbkw.cn/Article/details/gotaczoyc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.tarul.cn/Article/details/gpewzpgkx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.epnwcf.com/Article/details/gnslrajsi.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.tarul.cn/Article/details/gruhbpqdm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.vehdjk.com/Article/details/gpxquqdbt.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.sjlbkw.cn/Article/details/gdkqsiyuf.sHtML

[K05] 深拷贝对象
来源：http://www.share.tarul.cn/Article/details/gqdlveccj.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gkpffxsbl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.vehdjk.com/Article/details/ghkcrzsgw.sHtML

JS:   structuredClone(obj)
来源：http://3g.tarul.cn/Article/details/gdtlezsrf.sHtML

TS:   structuredClone(obj)
来源：http://baike.bbcook.cn/Article/details/gblvkqgiz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.sjlbkw.cn/Article/details/gkhyzvllo.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fktsv.cn/Article/details/gnescexfa.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.yfazqb.com/Article/details/gdsptdyrh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.bbcook.cn/Article/details/ggdzpodgf.sHtML

[K06] 解析 URL 查询串
来源：http://blog.bbcook.cn/Article/details/gzgzdmkrh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.tarul.cn/Article/details/glxcbjcyu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.bbcook.cn/Article/details/gbsbtkgvq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.vehdjk.com/Article/details/giuopkwbj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fktsv.cn/Article/details/gaizvmjhk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.sjlbkw.cn/Article/details/geakcwlqa.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.vehdjk.com/Article/details/goibtctrb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.sjlbkw.cn/Article/details/geqqumlbq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/gavygxfky.sHtML

[K07] 进制转换
来源：http://mobile.sjlbkw.cn/Article/details/godqwppix.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gyjqbegmj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.bbcook.cn/Article/details/ghuxhvyah.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.tarul.cn/Article/details/gjocfexwu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gswxkcwzz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gluuegeyt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fktsv.cn/Article/details/gmowbtqjp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fktsv.cn/Article/details/gusuridjg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gtpxjxwve.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.tarul.cn/Article/details/gutbogvud.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gpcsrepfi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.tarul.cn/Article/details/geuthocok.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.bbcook.cn/Article/details/gzimszyzl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.yfazqb.com/Article/details/ggflfhjof.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.sjlbkw.cn/Article/details/gdztwpyqx.sHtML

Go:   encoding/gob
来源：http://m.share.yfazqb.com/Article/details/gazpferur.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gjepebtod.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.bbcook.cn/Article/details/gktejlxhq.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/ggrdnvqmm.sHtML

L. 网络请求
来源：http://m.share.fktsv.cn/Article/details/gejqjarpz.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gakxrzffx.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.tarul.cn/Article/details/gigknvovr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fktsv.cn/Article/details/gsuyoockp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.vehdjk.com/Article/details/ghcrxpeol.sHtML

JS:   await fetch(url)
来源：http://baike.vehdjk.com/Article/details/gudvrfhhn.sHtML

TS:   await fetch(url)
来源：http://www.m.share.bbcook.cn/Article/details/gvjhzbgqm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.vehdjk.com/Article/details/ghouqmsrw.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.tarul.cn/Article/details/ghrchgisp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.epnwcf.com/Article/details/gbdoiqycl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.bbcook.cn/Article/details/gmccnhiek.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.yfazqb.com/Article/details/gwglnjrdw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.tarul.cn/Article/details/gjotlyvrg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.sjlbkw.cn/Article/details/gndjuhrln.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.bbcook.cn/Article/details/gpkxopzlo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.bbcook.cn/Article/details/gtqxjugcq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.tarul.cn/Article/details/ggcgovzpd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.sjlbkw.cn/Article/details/grwshuhcv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fktsv.cn/Article/details/gwcldvcbz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.tarul.cn/Article/details/gbverkrfr.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.epnwcf.com/Article/details/gwtixqsgo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.tarul.cn/Article/details/genpxeerg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.vehdjk.com/Article/details/gdpeclaqv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/gbexoqkjw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fktsv.cn/Article/details/grimdzzbx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fktsv.cn/Article/details/gqynpjjnz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.tarul.cn/Article/details/gvxopfzcf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.tarul.cn/Article/details/gvkpcrrjx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.epnwcf.com/Article/details/gntlgpzxj.sHtML

[L04] 设置超时
来源：http://www.m.share.bbcook.cn/Article/details/gmxvsralk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.vehdjk.com/Article/details/gomdwboan.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.sjlbkw.cn/Article/details/gckqsrgle.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.tarul.cn/Article/details/gbhdiprau.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.vehdjk.com/Article/details/gbijwrwwp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.sjlbkw.cn/Article/details/gknrxkzqw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.bbcook.cn/Article/details/gxcxifoit.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.sjlbkw.cn/Article/details/gpofjacxw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.tarul.cn/Article/details/gwsomdgjx.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.yfazqb.com/Article/details/gptnfdmhe.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.tarul.cn/Article/details/gthruzjjy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fktsv.cn/Article/details/gcezahthx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.epnwcf.com/Article/details/gwkfgklgc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.tarul.cn/Article/details/gomrvtxko.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.sjlbkw.cn/Article/details/gmrinwlui.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.vehdjk.com/Article/details/ggdhhlzll.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.epnwcf.com/Article/details/ghugzcntc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.bbcook.cn/Article/details/gdinjrvkp.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.yfazqb.com/Article/details/grgqmgfxq.sHtML

Py:   resp.json()
来源：http://blog.bbcook.cn/Article/details/gymmltdnr.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.vehdjk.com/Article/details/gwohluqdq.sHtML

JS:   await resp.json()
来源：http://m.share.epnwcf.com/Article/details/gcaohlalx.sHtML

TS:   await resp.json()
来源：http://blog.vehdjk.com/Article/details/gwyfccthm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.vehdjk.com/Article/details/gcxdaiijs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fktsv.cn/Article/details/ghpfkobwi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.sjlbkw.cn/Article/details/gkbvbrhan.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.sjlbkw.cn/Article/details/gmxujxkch.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.vehdjk.com/Article/details/gvvpwyvjc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fktsv.cn/Article/details/gmhpeilzz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.vehdjk.com/Article/details/gbycnpnmu.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.epnwcf.com/Article/details/gxywslojs.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.tarul.cn/Article/details/ggkkjiefw.sHtML

Java: resp.statusCode()
来源：http://wap.epnwcf.com/Article/details/gsalirwvh.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.bbcook.cn/Article/details/gqehdotfq.sHtML

Ruby: resp.code.to_i
来源：http://www.share.yfazqb.com/Article/details/gdjbbokev.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.sjlbkw.cn/Article/details/gplegxubs.sHtML

[L08] 并发请求多个地址
来源：http://www.share.yfazqb.com/Article/details/gewydkeua.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.bbcook.cn/Article/details/gcumdrior.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.tarul.cn/Article/details/gtzaexkzq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.sjlbkw.cn/Article/details/gacszlqrd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.yfazqb.com/Article/details/gefavmipt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.epnwcf.com/Article/details/grulliaei.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.epnwcf.com/Article/details/gaqpzsrtp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.epnwcf.com/Article/details/gszcilxcv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.epnwcf.com/Article/details/gcoupqnnl.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gxiwrxgfz.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.epnwcf.com/Article/details/gllkurdfi.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gnliflljh.sHtML

[M01] 读取命令行参数
来源：http://www.blog.bbcook.cn/Article/details/gaguurnis.sHtML

Py:   sys.argv[1:]
来源：http://m.share.vehdjk.com/Article/details/gaatbilsk.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.bbcook.cn/Article/details/guetgiixl.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.vehdjk.com/Article/details/gymbolvqw.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.yfazqb.com/Article/details/graqvusgs.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.vehdjk.com/Article/details/gbakvxmcg.sHtML

Go:   os.Args[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gbxxstjcb.sHtML

Ruby: ARGV
来源：http://baike.bbcook.cn/Article/details/gdobbshzk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.sjlbkw.cn/Article/details/gavyreczo.sHtML

[M02] 读取环境变量
来源：http://www.share.epnwcf.com/Article/details/gpmsnmygw.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.bbcook.cn/Article/details/gwlbrtzww.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fktsv.cn/Article/details/gldimuxrr.sHtML

JS:   process.env.HOME
来源：http://m.share.vehdjk.com/Article/details/gigpukpxr.sHtML

TS:   process.env.HOME
来源：http://www.share.bbcook.cn/Article/details/ggwbbatit.sHtML

Java: System.getenv("HOME")
来源：http://3g.epnwcf.com/Article/details/gzeknbfcd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gpzpuywwv.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.epnwcf.com/Article/details/gcolivuhd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gljrzgwhw.sHtML

[M03] 执行外部命令
来源：http://wap.fktsv.cn/Article/details/gjjwzamjp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fktsv.cn/Article/details/gellmuwet.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fktsv.cn/Article/details/gwzugbbqq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.bbcook.cn/Article/details/gswjuzzhy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.epnwcf.com/Article/details/gnnftietb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.bbcook.cn/Article/details/ghmftxdyi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.tarul.cn/Article/details/gzsfpcrbr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.tarul.cn/Article/details/gojktnfuk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.epnwcf.com/Article/details/gjvlbnoou.sHtML

[M04] 获取当前工作目录
来源：http://mobile.bbcook.cn/Article/details/ggehuhcce.sHtML

Py:   os.getcwd()
来源：http://mobile.sjlbkw.cn/Article/details/gepwwwmxi.sHtML

PHP:  getcwd();
来源：http://wap.fktsv.cn/Article/details/goeourqbx.sHtML

JS:   process.cwd()
来源：http://read.share.sjlbkw.cn/Article/details/goqwnryiw.sHtML

TS:   process.cwd()
来源：http://www.m.share.epnwcf.com/Article/details/gysdqwjjd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.tarul.cn/Article/details/gbvpkhiyd.sHtML

Go:   os.Getwd()
来源：http://wap.tarul.cn/Article/details/gbpdpytcz.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.bbcook.cn/Article/details/gimpqgvfy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.tarul.cn/Article/details/grwfcnppo.sHtML

[M05] 设置退出码
来源：http://read.share.vehdjk.com/Article/details/gdgfbqrps.sHtML

Py:   sys.exit(1)
来源：http://baike.yfazqb.com/Article/details/geeubyphb.sHtML

PHP:  exit(1);
来源：http://wap.epnwcf.com/Article/details/ggvhxootd.sHtML

JS:   process.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gwbfkepao.sHtML

TS:   process.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gckobbesf.sHtML

Java: System.exit(1)
来源：http://read.share.fktsv.cn/Article/details/ghmvdpzpd.sHtML

Go:   os.Exit(1)
来源：http://3g.epnwcf.com/Article/details/gxxfkuwtt.sHtML

Ruby: exit 1
来源：http://blog.vehdjk.com/Article/details/gklvpxxnw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fktsv.cn/Article/details/gztypxclr.sHtML

[M06] 向标准错误输出
来源：http://read.share.bbcook.cn/Article/details/gmtszqnge.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.vehdjk.com/Article/details/gmeuvtbri.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.epnwcf.com/Article/details/gztpghzli.sHtML

JS:   console.error("err")
来源：http://blog.vehdjk.com/Article/details/gpopwmpkb.sHtML

TS:   console.error("err")
来源：http://baike.bbcook.cn/Article/details/gxmuambxl.sHtML

Java: System.err.println("err")
来源：http://3g.yfazqb.com/Article/details/gubhntaqt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.yfazqb.com/Article/details/gqsafmqsc.sHtML

Ruby: warn "err"
来源：http://3g.epnwcf.com/Article/details/gpjcxxgzv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.sjlbkw.cn/Article/details/gjplurunq.sHtML

[M07] 判断是否为主入口
来源：http://baike.sjlbkw.cn/Article/details/gmihwfkyy.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.epnwcf.com/Article/details/gtazljvrs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.epnwcf.com/Article/details/gjqfnayfn.sHtML

JS:   require.main === module
来源：http://3g.yfazqb.com/Article/details/gauubweam.sHtML

TS:   require.main === module
来源：http://m.share.yfazqb.com/Article/details/gzvpalsbj.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.epnwcf.com/Article/details/gryicwybm.sHtML

Go:   func main()
来源：http://3g.tarul.cn/Article/details/glgtvbwpq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.sjlbkw.cn/Article/details/gijhslofj.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.epnwcf.com/Article/details/gimzebekj.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.yfazqb.com/Article/details/guvsaptko.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.bbcook.cn/Article/details/gzltcsata.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.tarul.cn/Article/details/gjjqzrted.sHtML

JS:   process.platform;  process.version
来源：http://wap.epnwcf.com/Article/details/gkyqznxec.sHtML

TS:   process.platform;  process.version
来源：http://blog.bbcook.cn/Article/details/gaeppszif.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.bbcook.cn/Article/details/gfbypbonm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fktsv.cn/Article/details/gbyeluszg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fktsv.cn/Article/details/gkoqqjqpe.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fktsv.cn/Article/details/gcewjghnw.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gmckxmpmv.sHtML

N. 数据结构与算法
来源：http://read.share.tarul.cn/Article/details/gndfmihmw.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ggabtomcr.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.epnwcf.com/Article/details/gwhojvnpp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcuwkymk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.tarul.cn/Article/details/gocrjfrei.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gwqcmcgoa.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.bbcook.cn/Article/details/gtkgpmchp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gwkjfmrxz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gyxbtptmg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.tarul.cn/Article/details/gonagonhq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.bbcook.cn/Article/details/gdywzuazs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.yfazqb.com/Article/details/gbksueqqs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.bbcook.cn/Article/details/gzslsdnqs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.epnwcf.com/Article/details/gxvwzjkdp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.vehdjk.com/Article/details/ghyaelzhp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.yfazqb.com/Article/details/gowyftvsl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.tarul.cn/Article/details/ggqzaayle.sHtML

Go:   slices.Sort(arr)
来源：http://baike.yfazqb.com/Article/details/gkxvsaheb.sHtML

Ruby: arr.sort
来源：http://read.share.fktsv.cn/Article/details/gprakolxo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.tarul.cn/Article/details/gtzltirya.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.yfazqb.com/Article/details/gqcqcfcdl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.sjlbkw.cn/Article/details/ghezluvno.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.tarul.cn/Article/details/gfhuvpevz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.yfazqb.com/Article/details/gpqvdeuwk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.epnwcf.com/Article/details/gxehaugrf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.bbcook.cn/Article/details/gporvvkhg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.epnwcf.com/Article/details/gmbmhcbvm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.vehdjk.com/Article/details/gmajeisgp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.sjlbkw.cn/Article/details/gzzrotmun.sHtML

[N04] 斐波那契数列
来源：http://3g.yfazqb.com/Article/details/gvpgdskhv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.vehdjk.com/Article/details/gyadsuliq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.yfazqb.com/Article/details/gkzhpudkm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/ghtxblnsb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/glagparxl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.sjlbkw.cn/Article/details/gfxgxjqjm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.vehdjk.com/Article/details/gohtuhpsb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.epnwcf.com/Article/details/gmjeqrwms.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gbigqkmtr.sHtML


<!-- 参考信息 -->