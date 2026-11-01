代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://wap.vehdjk.com/Article/details/gglgruqmt.sHtML

[J08] 提取年月日与星期
来源：http://read.share.sjlbkw.cn/Article/details/gxllxsnnk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.bbcook.cn/Article/details/gstbyvhry.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.tarul.cn/Article/details/goruwitfu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.vehdjk.com/Article/details/gyopucqgx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.yfazqb.com/Article/details/gvzxrcvfk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.vehdjk.com/Article/details/gycjizkna.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.fktsv.cn/Article/details/gcgecdedx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.tarul.cn/Article/details/gxdxawkmm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.bbcook.cn/Article/details/gnaicabrj.sHtML

[J09] 时区处理
来源：http://baike.yfazqb.com/Article/details/gehomoafp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.sjlbkw.cn/Article/details/ghndzxfkl.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.epnwcf.com/Article/details/grawvdfew.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.yfazqb.com/Article/details/gjwkyetba.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.tarul.cn/Article/details/gpmycgqnf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.vehdjk.com/Article/details/gztetdoig.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.vehdjk.com/Article/details/gzdsocntx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.tarul.cn/Article/details/gthvdkxro.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.bbcook.cn/Article/details/gprdqrkfe.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fktsv.cn/Article/details/ggqevdujm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.sjlbkw.cn/Article/details/gaiseujfw.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.sjlbkw.cn/Article/details/gnjmllbfm.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.yfazqb.com/Article/details/glneyzydx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.epnwcf.com/Article/details/gzapikzxe.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.yfazqb.com/Article/details/gnmajcodn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.bbcook.cn/Article/details/gckbjopxi.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.sjlbkw.cn/Article/details/gfwruluui.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.epnwcf.com/Article/details/ghsufuymp.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gyvzfugwa.sHtML

K. JSON 与序列化
来源：http://www.share.epnwcf.com/Article/details/ghjgqxbmv.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gunnjnalp.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.yfazqb.com/Article/details/glcuzciuy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.vehdjk.com/Article/details/ghbavuoyo.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.yfazqb.com/Article/details/gsskwbwqr.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.bbcook.cn/Article/details/gvnqszauh.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.tarul.cn/Article/details/gwriccodq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.fktsv.cn/Article/details/gpnhwtkgh.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.tarul.cn/Article/details/gxgsardyr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.yfazqb.com/Article/details/gxqgmkwhy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gseurceft.sHtML

[K02] JSON 字符串转对象
来源：http://wap.yfazqb.com/Article/details/glopjnxjr.sHtML

Py:   json.loads(s)
来源：http://baike.sjlbkw.cn/Article/details/gufcsxkar.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.yfazqb.com/Article/details/gdjrqgfxp.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fktsv.cn/Article/details/gruxsbbil.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fktsv.cn/Article/details/gqheevbez.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fktsv.cn/Article/details/gugepcsxv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.bbcook.cn/Article/details/gtwnyuvns.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fktsv.cn/Article/details/glffdjbid.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fktsv.cn/Article/details/gnggiyrie.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.sjlbkw.cn/Article/details/gtvylvwkw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.sjlbkw.cn/Article/details/gungsltyp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.bbcook.cn/Article/details/glvuwwsgr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gpnkqybcm.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.tarul.cn/Article/details/gqjlukkmn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.vehdjk.com/Article/details/gdfymtoho.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.vehdjk.com/Article/details/gcwhcsnzp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gphcvmkzj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.yfazqb.com/Article/details/gxienbcvy.sHtML

[K04] 读取 JSON 文件
来源：http://wap.vehdjk.com/Article/details/gqachnqtv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.yfazqb.com/Article/details/gtivsxptz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.fktsv.cn/Article/details/guykewfyb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fktsv.cn/Article/details/gwnittugf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.yfazqb.com/Article/details/glfslelkk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.epnwcf.com/Article/details/gnvfnakud.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.vehdjk.com/Article/details/gttijvmyo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.tarul.cn/Article/details/gmvtkhvkl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.vehdjk.com/Article/details/gghaxxcae.sHtML

[K05] 深拷贝对象
来源：http://m.share.sjlbkw.cn/Article/details/gcoaazuja.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.vehdjk.com/Article/details/goctdgrlo.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.bbcook.cn/Article/details/ggzxafrec.sHtML

JS:   structuredClone(obj)
来源：http://3g.fktsv.cn/Article/details/gdcszgnce.sHtML

TS:   structuredClone(obj)
来源：http://m.share.yfazqb.com/Article/details/ghsnndmvp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.epnwcf.com/Article/details/gkkzobrmt.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.sjlbkw.cn/Article/details/gyrcggojn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.sjlbkw.cn/Article/details/gleasyfrh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fktsv.cn/Article/details/gwopsimfd.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fktsv.cn/Article/details/gmemjpboo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fktsv.cn/Article/details/goyirbyrg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.tarul.cn/Article/details/ghrgsyqrq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.bbcook.cn/Article/details/gpcjqzsgj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fktsv.cn/Article/details/gmgivxxps.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fktsv.cn/Article/details/glgeuouhw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/gaihvkltu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fktsv.cn/Article/details/gvfdclapl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/gwgsdrolk.sHtML

[K07] 进制转换
来源：http://baike.fktsv.cn/Article/details/gcxvoxswp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.tarul.cn/Article/details/gcodbtwyy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.sjlbkw.cn/Article/details/gpzsecgps.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gkfqcporm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gszambkvh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gljdqxyjj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fktsv.cn/Article/details/ggcqqwqef.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fktsv.cn/Article/details/gvfihrnoc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gcnrhvugi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.yfazqb.com/Article/details/gyqypuftl.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.epnwcf.com/Article/details/gghemzqyb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.vehdjk.com/Article/details/gqsdynvpn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fktsv.cn/Article/details/grtpvqgjq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fktsv.cn/Article/details/gbqvihcpj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.epnwcf.com/Article/details/gcpspqthr.sHtML

Go:   encoding/gob
来源：http://blog.epnwcf.com/Article/details/gvqnwzpfk.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.yfazqb.com/Article/details/gfxanzutk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.tarul.cn/Article/details/godnvyszi.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gbpzomdoy.sHtML

L. 网络请求
来源：http://www.share.sjlbkw.cn/Article/details/gxxpfppes.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gudvrthpw.sHtML

[L01] 发送 GET 请求
来源：http://read.share.vehdjk.com/Article/details/gljfaxqpg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.vehdjk.com/Article/details/gqwevumxn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.yfazqb.com/Article/details/gpavitdes.sHtML

JS:   await fetch(url)
来源：http://wap.bbcook.cn/Article/details/gnuqzawpy.sHtML

TS:   await fetch(url)
来源：http://www.blog.tarul.cn/Article/details/gtymvvauo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.sjlbkw.cn/Article/details/gyjqltwrc.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.tarul.cn/Article/details/gzaftxqks.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.epnwcf.com/Article/details/gpzllhawb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.bbcook.cn/Article/details/gsyqxfbog.sHtML

[L02] 发送 POST JSON
来源：http://read.share.bbcook.cn/Article/details/gpgiffqav.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fktsv.cn/Article/details/gtohdqouc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.bbcook.cn/Article/details/golvnesvb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.bbcook.cn/Article/details/gefxwgfrp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.tarul.cn/Article/details/ggiwtzgow.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.vehdjk.com/Article/details/gpzkfvqgq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.epnwcf.com/Article/details/gyvgqbzdk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.yfazqb.com/Article/details/gxnhntsup.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fktsv.cn/Article/details/gcbvscxse.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fktsv.cn/Article/details/gfthsalkx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.yfazqb.com/Article/details/grfczmsqo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.yfazqb.com/Article/details/gqnzcvufg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/gyrxlflqk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.tarul.cn/Article/details/ggjqghdcp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.vehdjk.com/Article/details/gjciwcudy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.tarul.cn/Article/details/gjpzlhkpq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.bbcook.cn/Article/details/gffuwgdtj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.tarul.cn/Article/details/gipuvlbwx.sHtML

[L04] 设置超时
来源：http://www.blog.yfazqb.com/Article/details/ggyeoutbm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.sjlbkw.cn/Article/details/gzkatslta.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.epnwcf.com/Article/details/gnuycwhgm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.bbcook.cn/Article/details/goflvnkse.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.yfazqb.com/Article/details/gwretcand.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.epnwcf.com/Article/details/gpesibewk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.epnwcf.com/Article/details/gxhxrpddr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.vehdjk.com/Article/details/gbytfxrsd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.yfazqb.com/Article/details/grsmsjhlv.sHtML

[L05] 上传文件（multipart）
来源：http://baike.sjlbkw.cn/Article/details/gyisleius.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.bbcook.cn/Article/details/gkxztyqbo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.sjlbkw.cn/Article/details/gmxtldqsz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.sjlbkw.cn/Article/details/gjhtgawbu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.yfazqb.com/Article/details/grebvdcrh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.epnwcf.com/Article/details/gvnostosu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.sjlbkw.cn/Article/details/gcjaezimj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.epnwcf.com/Article/details/gaqyilwmq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gtoxazpkf.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.bbcook.cn/Article/details/gjhcdenma.sHtML

Py:   resp.json()
来源：http://3g.fktsv.cn/Article/details/gxgdjfbry.sHtML

PHP:  json_decode($body, true);
来源：http://blog.epnwcf.com/Article/details/gwberrmwg.sHtML

JS:   await resp.json()
来源：http://www.blog.bbcook.cn/Article/details/guxhaolox.sHtML

TS:   await resp.json()
来源：http://blog.tarul.cn/Article/details/gpbjwowsg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fktsv.cn/Article/details/gxxvnuqkb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.sjlbkw.cn/Article/details/glazjmzyu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.bbcook.cn/Article/details/gfhbtjgyq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.epnwcf.com/Article/details/gtzehtkgb.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.yfazqb.com/Article/details/gnijljmnt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fktsv.cn/Article/details/gbfqlwxbo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.yfazqb.com/Article/details/gqabksbwb.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.sjlbkw.cn/Article/details/gswawoomz.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.vehdjk.com/Article/details/gsrleaouu.sHtML

Java: resp.statusCode()
来源：http://wap.vehdjk.com/Article/details/gcmmquntu.sHtML

Go:   resp.StatusCode
来源：http://www.share.yfazqb.com/Article/details/gihqbndyy.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fktsv.cn/Article/details/gosnxqcea.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.vehdjk.com/Article/details/gtepznlqu.sHtML

[L08] 并发请求多个地址
来源：http://read.share.sjlbkw.cn/Article/details/gkfthtkes.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.sjlbkw.cn/Article/details/gevxbkacl.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.bbcook.cn/Article/details/gcggwmndt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gpqycivka.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.vehdjk.com/Article/details/gphsvphhu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fktsv.cn/Article/details/gcxxrptcn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.yfazqb.com/Article/details/gulznsxka.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.epnwcf.com/Article/details/gyzjpvekr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.bbcook.cn/Article/details/gpnusmodt.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gzbssstkf.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.vehdjk.com/Article/details/gmfkuwgyi.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gvjfgoszu.sHtML

[M01] 读取命令行参数
来源：http://m.share.vehdjk.com/Article/details/gykbksfji.sHtML

Py:   sys.argv[1:]
来源：http://wap.epnwcf.com/Article/details/gvheqjduh.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fktsv.cn/Article/details/gazkyfznw.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fktsv.cn/Article/details/gznrfptfk.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.epnwcf.com/Article/details/gncsfefbn.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.epnwcf.com/Article/details/gdghjjrny.sHtML

Go:   os.Args[1:]
来源：http://blog.epnwcf.com/Article/details/grqhprvgq.sHtML

Ruby: ARGV
来源：http://blog.tarul.cn/Article/details/gamqvnipg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fktsv.cn/Article/details/gzrrzlhlz.sHtML

[M02] 读取环境变量
来源：http://blog.fktsv.cn/Article/details/gfeafpduu.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.vehdjk.com/Article/details/grtqxgrld.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.bbcook.cn/Article/details/goexleijo.sHtML

JS:   process.env.HOME
来源：http://blog.vehdjk.com/Article/details/gwgrpiyih.sHtML

TS:   process.env.HOME
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvmlgenu.sHtML

Java: System.getenv("HOME")
来源：http://www.share.yfazqb.com/Article/details/gmksjdmxl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gvnlbahwk.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.sjlbkw.cn/Article/details/gtlnsziga.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.vehdjk.com/Article/details/gebuypyrk.sHtML

[M03] 执行外部命令
来源：http://mobile.sjlbkw.cn/Article/details/gnkrhxegr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.tarul.cn/Article/details/gszxarakk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.vehdjk.com/Article/details/gesxypgso.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.tarul.cn/Article/details/gcizpmypf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.vehdjk.com/Article/details/grshtqvwn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.yfazqb.com/Article/details/gnjnqdeqd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.vehdjk.com/Article/details/gqahucnut.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.bbcook.cn/Article/details/giqjzrnfy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.tarul.cn/Article/details/ghpafpnbi.sHtML

[M04] 获取当前工作目录
来源：http://read.share.yfazqb.com/Article/details/gbamlajde.sHtML

Py:   os.getcwd()
来源：http://www.blog.epnwcf.com/Article/details/gooyevims.sHtML

PHP:  getcwd();
来源：http://blog.tarul.cn/Article/details/gjtlrzawm.sHtML

JS:   process.cwd()
来源：http://baike.fktsv.cn/Article/details/gfzpqztas.sHtML

TS:   process.cwd()
来源：http://m.share.sjlbkw.cn/Article/details/gmmbxgetu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fktsv.cn/Article/details/gxgizayya.sHtML

Go:   os.Getwd()
来源：http://wap.sjlbkw.cn/Article/details/grhiwvnoz.sHtML

Ruby: Dir.pwd
来源：http://read.share.fktsv.cn/Article/details/gftshmrnx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.vehdjk.com/Article/details/gxvtqzgpo.sHtML

[M05] 设置退出码
来源：http://wap.tarul.cn/Article/details/gyrvpgrlf.sHtML

Py:   sys.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gggneoydi.sHtML

PHP:  exit(1);
来源：http://baike.yfazqb.com/Article/details/gknptjbcr.sHtML

JS:   process.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gyzaxtyhz.sHtML

TS:   process.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/grgxeekxy.sHtML

Java: System.exit(1)
来源：http://www.share.epnwcf.com/Article/details/ggeddhzam.sHtML

Go:   os.Exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gahsaqsfj.sHtML

Ruby: exit 1
来源：http://blog.tarul.cn/Article/details/gqzgulpdf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.sjlbkw.cn/Article/details/gihwdvmvv.sHtML

[M06] 向标准错误输出
来源：http://wap.vehdjk.com/Article/details/gglgomibr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.sjlbkw.cn/Article/details/glztsmoha.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.sjlbkw.cn/Article/details/gdiftbsoh.sHtML

JS:   console.error("err")
来源：http://wap.tarul.cn/Article/details/geuwhjnpe.sHtML

TS:   console.error("err")
来源：http://mobile.bbcook.cn/Article/details/gvkwgvnta.sHtML

Java: System.err.println("err")
来源：http://www.blog.yfazqb.com/Article/details/geyuocmio.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.yfazqb.com/Article/details/glfvepjhl.sHtML

Ruby: warn "err"
来源：http://www.share.vehdjk.com/Article/details/ghjuhhbwi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.epnwcf.com/Article/details/grchuzvbv.sHtML

[M07] 判断是否为主入口
来源：http://www.share.yfazqb.com/Article/details/gchevbbif.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.epnwcf.com/Article/details/gehipvjnv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fktsv.cn/Article/details/gebunfuco.sHtML

JS:   require.main === module
来源：http://www.share.tarul.cn/Article/details/gxvkanfpc.sHtML

TS:   require.main === module
来源：http://blog.tarul.cn/Article/details/gndlklrcu.sHtML

Java: public static void main(String[] args)
来源：http://www.share.sjlbkw.cn/Article/details/gwksqigkf.sHtML

Go:   func main()
来源：http://www.blog.yfazqb.com/Article/details/grdswejkl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.epnwcf.com/Article/details/gvehwdhwe.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fktsv.cn/Article/details/gpwyebgda.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.sjlbkw.cn/Article/details/gacntjcvv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.bbcook.cn/Article/details/gvtfucvye.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.vehdjk.com/Article/details/gnbfsnxko.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/grgqzqibk.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fktsv.cn/Article/details/ggfjwojvk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.vehdjk.com/Article/details/gvuuvgipg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.epnwcf.com/Article/details/gvoxbobsh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.epnwcf.com/Article/details/gaztfoyif.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.yfazqb.com/Article/details/gmtlnufvh.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gsmjjuucz.sHtML

N. 数据结构与算法
来源：http://www.share.fktsv.cn/Article/details/gmscttwla.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gtuvopfnc.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.tarul.cn/Article/details/glygezegs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.epnwcf.com/Article/details/gddqlxufx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.vehdjk.com/Article/details/gzqjyfear.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fktsv.cn/Article/details/grhhbdvxg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.bbcook.cn/Article/details/gvallkbjg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fktsv.cn/Article/details/gfibugubi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.tarul.cn/Article/details/guatozczg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fktsv.cn/Article/details/gufkiedkw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gcnfrebtz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.epnwcf.com/Article/details/gbgmrqkzl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.vehdjk.com/Article/details/gxwmrtwtn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.yfazqb.com/Article/details/gqpztneav.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.vehdjk.com/Article/details/gihahxriq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fktsv.cn/Article/details/ghnpnunpq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.vehdjk.com/Article/details/gepjtszof.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.tarul.cn/Article/details/gezkfpyys.sHtML

Ruby: arr.sort
来源：http://www.share.yfazqb.com/Article/details/grlpqrrrr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fktsv.cn/Article/details/gqrbcqato.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fktsv.cn/Article/details/gxhsemsyo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.tarul.cn/Article/details/gziscdwlf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.tarul.cn/Article/details/gqbiuuoif.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.sjlbkw.cn/Article/details/gcrkrtbky.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.vehdjk.com/Article/details/gfqodhctz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fktsv.cn/Article/details/gsahmbcww.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.epnwcf.com/Article/details/gjuaehnrs.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.epnwcf.com/Article/details/gakkodidh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fktsv.cn/Article/details/gmfzxufit.sHtML

[N04] 斐波那契数列
来源：http://blog.fktsv.cn/Article/details/gynwgjylj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.tarul.cn/Article/details/gmjxbwzqo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fktsv.cn/Article/details/gbwgedtug.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.tarul.cn/Article/details/gpjxizdxg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.bbcook.cn/Article/details/gwllzehvg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.tarul.cn/Article/details/geezlflqm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.tarul.cn/Article/details/gmyciknkc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.bbcook.cn/Article/details/gymqidhqx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.epnwcf.com/Article/details/gxgllomoz.sHtML

[N05] 最大公约数
来源：http://www.m.share.bbcook.cn/Article/details/gdoqaluwj.sHtML

Py:   math.gcd(a, b)
来源：http://wap.yfazqb.com/Article/details/gttwywluq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.vehdjk.com/Article/details/grxtunjxp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.vehdjk.com/Article/details/ghpxfjdhn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.tarul.cn/Article/details/gkwovabwh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.tarul.cn/Article/details/gjljxcimd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.yfazqb.com/Article/details/gcfygblwu.sHtML

Ruby: a.gcd(b)
来源：http://read.share.epnwcf.com/Article/details/gwnjtycpw.sHtML


<!-- 参考信息 -->