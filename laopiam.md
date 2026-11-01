代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.sjlbkw.cn/Article/details/gzqaxgzhs.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.yfazqb.com/Article/details/gmorjpofq.sHtML

[J09] 时区处理
来源：http://www.m.share.fktsv.cn/Article/details/gxtbdeuhs.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.epnwcf.com/Article/details/gnpqerump.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.tarul.cn/Article/details/gkwerjnkx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.bbcook.cn/Article/details/gazjyyiub.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.epnwcf.com/Article/details/gqtyjxksb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.bbcook.cn/Article/details/gbofssyyf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.vehdjk.com/Article/details/guovlwlha.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.bbcook.cn/Article/details/ggehiaatd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.yfazqb.com/Article/details/glmjktrfx.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.yfazqb.com/Article/details/glfckkaou.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fktsv.cn/Article/details/grysbzjhf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.tarul.cn/Article/details/gapaorwla.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.vehdjk.com/Article/details/gwsiuhuas.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.vehdjk.com/Article/details/gbqclrmjk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.tarul.cn/Article/details/ghyucfrhk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fktsv.cn/Article/details/gnurpfgem.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.epnwcf.com/Article/details/gdefiukjq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.bbcook.cn/Article/details/gbrojmhcy.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gcyrfrrck.sHtML

K. JSON 与序列化
来源：http://www.m.share.vehdjk.com/Article/details/gxwrwofhs.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gxzpqfzhj.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.epnwcf.com/Article/details/gbmpxsage.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.bbcook.cn/Article/details/gorlkielw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.vehdjk.com/Article/details/gwdruallk.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.vehdjk.com/Article/details/gcaliegnq.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.vehdjk.com/Article/details/gcwrhsqui.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.tarul.cn/Article/details/gwwkhsytz.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.yfazqb.com/Article/details/gobjliukn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.yfazqb.com/Article/details/gzhdglzpu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.bbcook.cn/Article/details/gpsdstijd.sHtML

[K02] JSON 字符串转对象
来源：http://baike.yfazqb.com/Article/details/gngqvinpk.sHtML

Py:   json.loads(s)
来源：http://wap.sjlbkw.cn/Article/details/ghpwafeph.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gpeqoatih.sHtML

JS:   JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/gnbddmzgr.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/groyuephu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.vehdjk.com/Article/details/gixjqxedo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.tarul.cn/Article/details/gqvjnfgta.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.vehdjk.com/Article/details/gqijqjwix.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.tarul.cn/Article/details/glmsyphgf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fktsv.cn/Article/details/guzqluoej.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.bbcook.cn/Article/details/gskxrjrhe.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fktsv.cn/Article/details/gjgxqegdo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.sjlbkw.cn/Article/details/gehgpgnvu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqtdnspx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.bbcook.cn/Article/details/gzaeleoim.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.vehdjk.com/Article/details/gqzlgatrz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.vehdjk.com/Article/details/gyhragkmk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.yfazqb.com/Article/details/gvvewpykv.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fktsv.cn/Article/details/ghvzyazqu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.sjlbkw.cn/Article/details/gobgapsjq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.bbcook.cn/Article/details/gjhyktzmq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.bbcook.cn/Article/details/gqzfcduvo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.sjlbkw.cn/Article/details/gvjbmzwdi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.tarul.cn/Article/details/gymgrpahk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.bbcook.cn/Article/details/gvvcrtzpd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.epnwcf.com/Article/details/gygqqukcd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fktsv.cn/Article/details/gnhwbqwub.sHtML

[K05] 深拷贝对象
来源：http://www.share.tarul.cn/Article/details/gynpqrlqh.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gsrgooywt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.bbcook.cn/Article/details/gdwjvodoz.sHtML

JS:   structuredClone(obj)
来源：http://3g.tarul.cn/Article/details/gmwrnggrm.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.bbcook.cn/Article/details/gslakqado.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.vehdjk.com/Article/details/gymprzijq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.tarul.cn/Article/details/geuajdzzj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fktsv.cn/Article/details/gtnwfgupe.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.bbcook.cn/Article/details/ghlqxxnln.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.vehdjk.com/Article/details/gspmwiono.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fktsv.cn/Article/details/gxdipdavs.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.tarul.cn/Article/details/gmsggvhmn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fktsv.cn/Article/details/glrcvjvmh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.tarul.cn/Article/details/ghrwtntdk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.bbcook.cn/Article/details/glgicjpxz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.bbcook.cn/Article/details/gdjofjyje.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.tarul.cn/Article/details/gobzslkyt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/glxobmtbp.sHtML

[K07] 进制转换
来源：http://wap.fktsv.cn/Article/details/gzqdhimvl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.tarul.cn/Article/details/glbxmrmxx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.bbcook.cn/Article/details/glxgmaosa.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/giudmvxzt.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/gdziefvzy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gvgyiennn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.sjlbkw.cn/Article/details/gcefpbvus.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fktsv.cn/Article/details/gdbjytomh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gjhzgnjjs.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.vehdjk.com/Article/details/gfucileeb.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.tarul.cn/Article/details/glyrimxme.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.vehdjk.com/Article/details/gzqmljliq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.bbcook.cn/Article/details/gblallgqe.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.tarul.cn/Article/details/graladcpx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.yfazqb.com/Article/details/grfesrajm.sHtML

Go:   encoding/gob
来源：http://blog.epnwcf.com/Article/details/gpcorkfcm.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.tarul.cn/Article/details/gfggqkcgl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fktsv.cn/Article/details/gsvwzdupr.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gqzyvymbf.sHtML

L. 网络请求
来源：http://blog.epnwcf.com/Article/details/gjtxuuoru.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/ggfxskssy.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fktsv.cn/Article/details/gtozkzrgh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.sjlbkw.cn/Article/details/gqrkdlbsv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.epnwcf.com/Article/details/gwwksguze.sHtML

JS:   await fetch(url)
来源：http://mobile.vehdjk.com/Article/details/gzqncknhk.sHtML

TS:   await fetch(url)
来源：http://read.share.fktsv.cn/Article/details/gctnrshhj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fktsv.cn/Article/details/gwhcdjznd.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fktsv.cn/Article/details/ghkkthwme.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.vehdjk.com/Article/details/gqookdbqh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.vehdjk.com/Article/details/gddbmxowc.sHtML

[L02] 发送 POST JSON
来源：http://wap.bbcook.cn/Article/details/gtiqzzgfq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.sjlbkw.cn/Article/details/glwqimbjx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.sjlbkw.cn/Article/details/gpbiufvhq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwiutxus.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fktsv.cn/Article/details/gftfvzzlm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fktsv.cn/Article/details/gyenqmsqm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.vehdjk.com/Article/details/ggaqtkjdn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.sjlbkw.cn/Article/details/gzwneeqiu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.tarul.cn/Article/details/gwmmbyxib.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fktsv.cn/Article/details/gzdefgdcv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.bbcook.cn/Article/details/gicbpntph.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.vehdjk.com/Article/details/gswqszbzk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.yfazqb.com/Article/details/ghsfsdpzj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.vehdjk.com/Article/details/gajxsyemf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.yfazqb.com/Article/details/gcxvmznkz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.yfazqb.com/Article/details/gydpjdntx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.yfazqb.com/Article/details/gvxdflwyu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.epnwcf.com/Article/details/gyyljbxii.sHtML

[L04] 设置超时
来源：http://www.m.share.bbcook.cn/Article/details/gupgvnmct.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fktsv.cn/Article/details/gpayzzcpm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.tarul.cn/Article/details/gzknapizh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.bbcook.cn/Article/details/glydelvql.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.epnwcf.com/Article/details/gsaxuakzp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.vehdjk.com/Article/details/gehxgbmql.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fktsv.cn/Article/details/gzrdtvrry.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fktsv.cn/Article/details/gkjthubfj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fktsv.cn/Article/details/gnawasnud.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.vehdjk.com/Article/details/gwgjmzmhl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.bbcook.cn/Article/details/gykqvrnwk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.epnwcf.com/Article/details/gwueexozm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.vehdjk.com/Article/details/gpovzygyc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.yfazqb.com/Article/details/gdswwjogb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.bbcook.cn/Article/details/grvphgbef.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.sjlbkw.cn/Article/details/gmnrdguwy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fktsv.cn/Article/details/ghtysoudx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.vehdjk.com/Article/details/gbzrhvvkk.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.bbcook.cn/Article/details/ghlqcuzdo.sHtML

Py:   resp.json()
来源：http://blog.sjlbkw.cn/Article/details/gsjvmnnbb.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.bbcook.cn/Article/details/gdejomhzk.sHtML

JS:   await resp.json()
来源：http://mobile.tarul.cn/Article/details/gvdzzifra.sHtML

TS:   await resp.json()
来源：http://baike.epnwcf.com/Article/details/gdkrhhvtq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fktsv.cn/Article/details/gkbbgqkit.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fktsv.cn/Article/details/gikcsaedl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.vehdjk.com/Article/details/gufnmfrra.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.sjlbkw.cn/Article/details/gbzbdfrfb.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.epnwcf.com/Article/details/gyzowdjau.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.epnwcf.com/Article/details/gsudyvvno.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.bbcook.cn/Article/details/gamenlwqm.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.sjlbkw.cn/Article/details/gmhvhozyy.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.vehdjk.com/Article/details/gglvjpaup.sHtML

Java: resp.statusCode()
来源：http://www.share.vehdjk.com/Article/details/gmzzaefcj.sHtML

Go:   resp.StatusCode
来源：http://www.blog.vehdjk.com/Article/details/gkykpdlgu.sHtML

Ruby: resp.code.to_i
来源：http://baike.fktsv.cn/Article/details/gqhwqrqlb.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.epnwcf.com/Article/details/gmozelriu.sHtML

[L08] 并发请求多个地址
来源：http://m.share.bbcook.cn/Article/details/gecrjudmp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.sjlbkw.cn/Article/details/gvxfieeon.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.bbcook.cn/Article/details/gxaovzdas.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.tarul.cn/Article/details/gfsfzhjhq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.sjlbkw.cn/Article/details/gdfrzwodk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.tarul.cn/Article/details/gltcwytsh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.bbcook.cn/Article/details/gitwfjgnf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.sjlbkw.cn/Article/details/glihljrrt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.vehdjk.com/Article/details/gnjdnmzde.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gegczorzx.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.bbcook.cn/Article/details/golpcgyog.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gtwbpjgnu.sHtML

[M01] 读取命令行参数
来源：http://baike.vehdjk.com/Article/details/gaebstfqq.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.vehdjk.com/Article/details/gunivflwn.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.bbcook.cn/Article/details/ghvjqjnsk.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.sjlbkw.cn/Article/details/gsrcnnpkl.sHtML

TS:   process.argv.slice(2)
来源：http://baike.bbcook.cn/Article/details/goebppmru.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.sjlbkw.cn/Article/details/gzmmbsbqu.sHtML

Go:   os.Args[1:]
来源：http://m.share.vehdjk.com/Article/details/gxnwqdmvb.sHtML

Ruby: ARGV
来源：http://baike.bbcook.cn/Article/details/gzcshqimp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.vehdjk.com/Article/details/ggpigylee.sHtML

[M02] 读取环境变量
来源：http://www.share.fktsv.cn/Article/details/gqxvanjce.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.tarul.cn/Article/details/gzdlgoeiu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.sjlbkw.cn/Article/details/gjkzyumbi.sHtML

JS:   process.env.HOME
来源：http://www.blog.epnwcf.com/Article/details/ghscushxo.sHtML

TS:   process.env.HOME
来源：http://3g.fktsv.cn/Article/details/gredepchz.sHtML

Java: System.getenv("HOME")
来源：http://baike.epnwcf.com/Article/details/gsajbgqlm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.yfazqb.com/Article/details/gxhmvapbu.sHtML

Ruby: ENV["HOME"]
来源：http://blog.tarul.cn/Article/details/gyiskhxnp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.vehdjk.com/Article/details/guqqwrfjv.sHtML

[M03] 执行外部命令
来源：http://3g.epnwcf.com/Article/details/guzglsnse.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gtxgnrvsp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fktsv.cn/Article/details/guqhcfkok.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.tarul.cn/Article/details/gxtbviisv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.bbcook.cn/Article/details/gothksbnq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.vehdjk.com/Article/details/ggmqkizom.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fktsv.cn/Article/details/gzoevdipr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.bbcook.cn/Article/details/gcnojlozq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.yfazqb.com/Article/details/gbamqonbk.sHtML

[M04] 获取当前工作目录
来源：http://read.share.bbcook.cn/Article/details/gkbwajgno.sHtML

Py:   os.getcwd()
来源：http://3g.tarul.cn/Article/details/glxtcmhts.sHtML

PHP:  getcwd();
来源：http://mobile.tarul.cn/Article/details/gmpezcblw.sHtML

JS:   process.cwd()
来源：http://baike.vehdjk.com/Article/details/gigealcae.sHtML

TS:   process.cwd()
来源：http://read.share.vehdjk.com/Article/details/getitkltk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.bbcook.cn/Article/details/gazulnrpo.sHtML

Go:   os.Getwd()
来源：http://read.share.bbcook.cn/Article/details/gccvrduau.sHtML

Ruby: Dir.pwd
来源：http://blog.fktsv.cn/Article/details/gbiizjjkn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.sjlbkw.cn/Article/details/gskrdfmcq.sHtML

[M05] 设置退出码
来源：http://read.share.tarul.cn/Article/details/gzkhrhutm.sHtML

Py:   sys.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gewsufckp.sHtML

PHP:  exit(1);
来源：http://mobile.bbcook.cn/Article/details/gcqjhcahn.sHtML

JS:   process.exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gzhjysoax.sHtML

TS:   process.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gtjzkfjva.sHtML

Java: System.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gjuzhyipi.sHtML

Go:   os.Exit(1)
来源：http://blog.bbcook.cn/Article/details/ghjkvncns.sHtML

Ruby: exit 1
来源：http://www.m.share.tarul.cn/Article/details/gyqwprixf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.tarul.cn/Article/details/gmbbkeskd.sHtML

[M06] 向标准错误输出
来源：http://blog.epnwcf.com/Article/details/ggkczwtme.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.epnwcf.com/Article/details/gldnulbpo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.bbcook.cn/Article/details/gragtbald.sHtML

JS:   console.error("err")
来源：http://www.blog.fktsv.cn/Article/details/glmwkmifk.sHtML

TS:   console.error("err")
来源：http://wap.yfazqb.com/Article/details/getkpswjk.sHtML

Java: System.err.println("err")
来源：http://baike.sjlbkw.cn/Article/details/gqqmdglie.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fktsv.cn/Article/details/geqsxsiyg.sHtML

Ruby: warn "err"
来源：http://mobile.fktsv.cn/Article/details/gpcpxakvo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.yfazqb.com/Article/details/gvmmnozzc.sHtML

[M07] 判断是否为主入口
来源：http://blog.tarul.cn/Article/details/grfymhsys.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fktsv.cn/Article/details/gkbxrxtaj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.tarul.cn/Article/details/gvksrsclq.sHtML

JS:   require.main === module
来源：http://wap.fktsv.cn/Article/details/gzksirntd.sHtML

TS:   require.main === module
来源：http://m.share.epnwcf.com/Article/details/guuwpcgrr.sHtML

Java: public static void main(String[] args)
来源：http://blog.bbcook.cn/Article/details/gzlplqgwr.sHtML

Go:   func main()
来源：http://m.share.tarul.cn/Article/details/gdrteqtis.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fktsv.cn/Article/details/gqkavdjxt.sHtML

C#:   static void Main(string[] args)
来源：http://blog.tarul.cn/Article/details/gnyyopeiw.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.yfazqb.com/Article/details/gahtpxowi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.yfazqb.com/Article/details/gttejuvav.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.vehdjk.com/Article/details/guvpcauyf.sHtML

JS:   process.platform;  process.version
来源：http://wap.tarul.cn/Article/details/gbupdqtvq.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.yfazqb.com/Article/details/gwcflftub.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.vehdjk.com/Article/details/glkfcmydl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.tarul.cn/Article/details/gsazfcuex.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.bbcook.cn/Article/details/gplftqodl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.bbcook.cn/Article/details/gselikgvx.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gvotbuzvj.sHtML

N. 数据结构与算法
来源：http://blog.epnwcf.com/Article/details/ggargodke.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gftxgeqnl.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.sjlbkw.cn/Article/details/gwhnxmxum.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.bbcook.cn/Article/details/gzghzzcxy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fktsv.cn/Article/details/gmxgrmkbt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.tarul.cn/Article/details/gfnwqfdoz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.yfazqb.com/Article/details/gbopmgflh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/govychuqo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gmpgzvect.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fktsv.cn/Article/details/gfzcfgzef.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gdzafohoj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fktsv.cn/Article/details/gjnfitvdq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.sjlbkw.cn/Article/details/gjtohyhrl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.epnwcf.com/Article/details/gwscrjqyt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/gmptvbkwy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/gepplcghx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.yfazqb.com/Article/details/gonsbkepf.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.bbcook.cn/Article/details/gvjjpxvra.sHtML

Ruby: arr.sort
来源：http://mobile.yfazqb.com/Article/details/gzpowfssy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.epnwcf.com/Article/details/gnqxxmpas.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.vehdjk.com/Article/details/gfqjtwchf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.sjlbkw.cn/Article/details/gscpglqxz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.tarul.cn/Article/details/gpamgervi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.tarul.cn/Article/details/gvylfsrix.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fktsv.cn/Article/details/gufknezxp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.epnwcf.com/Article/details/gkscvektb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.tarul.cn/Article/details/gmhwzoibo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.epnwcf.com/Article/details/gaggnamtk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.bbcook.cn/Article/details/gouozazgh.sHtML

[N04] 斐波那契数列
来源：http://m.share.sjlbkw.cn/Article/details/gdzwyjzbo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.vehdjk.com/Article/details/gcpppkiay.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.tarul.cn/Article/details/gwodrrbmr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.vehdjk.com/Article/details/gnlmojkcb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.vehdjk.com/Article/details/gsydonjbj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.yfazqb.com/Article/details/godvimscd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.yfazqb.com/Article/details/gnjbrxpmj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.epnwcf.com/Article/details/gvitpwmqw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/guauvftrj.sHtML

[N05] 最大公约数
来源：http://www.m.share.yfazqb.com/Article/details/gbdoitouu.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.tarul.cn/Article/details/gfjbhpmhm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fktsv.cn/Article/details/gncukmonp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.vehdjk.com/Article/details/gvxwipwnk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fktsv.cn/Article/details/gmrxaiwfu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.tarul.cn/Article/details/geddzicyh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fktsv.cn/Article/details/gcnwdixgi.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.bbcook.cn/Article/details/ghgaeayzk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.epnwcf.com/Article/details/gchmnihey.sHtML

[N06] 判断回文字符串
来源：http://baike.yfazqb.com/Article/details/gkglhbutj.sHtML

Py:   s == s[::-1]
来源：http://read.share.sjlbkw.cn/Article/details/gyadqaknk.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.epnwcf.com/Article/details/guxeakcjz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/gizatyqgl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gjibcrpdk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.vehdjk.com/Article/details/goxsodlyu.sHtML

Go:   // 双指针从两端比较
来源：http://wap.vehdjk.com/Article/details/gkengxljt.sHtML


<!-- 参考信息 -->