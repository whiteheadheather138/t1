代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.sjlbkw.cn/Article/details/gljddzkst.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.vehdjk.com/Article/details/grafmaqsy.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.bbcook.cn/Article/details/ghyjcmvnx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.tarul.cn/Article/details/gedhnkmse.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.sjlbkw.cn/Article/details/gtfyfhtnu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.yfazqb.com/Article/details/gzfcomuvn.sHtML

[J09] 时区处理
来源：http://baike.vehdjk.com/Article/details/gguhfnpkh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.bbcook.cn/Article/details/gmqzkymhh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.sjlbkw.cn/Article/details/gofbymeos.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.tarul.cn/Article/details/gbrlerelf.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.vehdjk.com/Article/details/gwzxtiova.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.vehdjk.com/Article/details/gnjwfyylm.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.yfazqb.com/Article/details/gjvuvmcbc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.vehdjk.com/Article/details/gsonfxidw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.vehdjk.com/Article/details/gzrdlayvb.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.sjlbkw.cn/Article/details/gdbvtgjuy.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.yfazqb.com/Article/details/gobspptzp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.fktsv.cn/Article/details/gydfwwami.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.sjlbkw.cn/Article/details/gbjgqvzje.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gfponyrba.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.tarul.cn/Article/details/gqqynzrcj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.sjlbkw.cn/Article/details/gfaqyiktj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.vehdjk.com/Article/details/gvrnfwynp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.vehdjk.com/Article/details/ggrqjdnvv.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/giglvqvwk.sHtML

K. JSON 与序列化
来源：http://www.blog.tarul.cn/Article/details/grdvvalhx.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gsgaihfuf.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.vehdjk.com/Article/details/gzshxozrh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.vehdjk.com/Article/details/givgwdlcg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.bbcook.cn/Article/details/gnhninekj.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.vehdjk.com/Article/details/gwggvqnwd.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.yfazqb.com/Article/details/gmjhikbel.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.fktsv.cn/Article/details/gakeipnsr.sHtML

Go:   json.Marshal(obj)
来源：http://wap.sjlbkw.cn/Article/details/guwwdjfgq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.vehdjk.com/Article/details/gfxhyiahf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.yfazqb.com/Article/details/gnwgfrpfh.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.vehdjk.com/Article/details/gbqglxoxs.sHtML

Py:   json.loads(s)
来源：http://m.share.tarul.cn/Article/details/gnbgpgqon.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fktsv.cn/Article/details/gprwjwhyv.sHtML

JS:   JSON.parse(s)
来源：http://mobile.bbcook.cn/Article/details/gfttnzrde.sHtML

TS:   JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/geivfabme.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.yfazqb.com/Article/details/gmbcnhwad.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.epnwcf.com/Article/details/gkkpjocqg.sHtML

Ruby: JSON.parse(s)
来源：http://3g.yfazqb.com/Article/details/gfmhldqhr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.vehdjk.com/Article/details/gjeieytqz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.yfazqb.com/Article/details/gtohqvnmx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.bbcook.cn/Article/details/grvaywmrb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.yfazqb.com/Article/details/gpbwvkhxn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fktsv.cn/Article/details/gldkmjfzg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.tarul.cn/Article/details/gtcjvotbz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.vehdjk.com/Article/details/gbhyjrmxg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.bbcook.cn/Article/details/ggefqxvgd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.vehdjk.com/Article/details/gkjdwxrin.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fktsv.cn/Article/details/godkgvjur.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fktsv.cn/Article/details/guoxnjidn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.tarul.cn/Article/details/gkhthdnjl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.yfazqb.com/Article/details/gtwzutvof.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.bbcook.cn/Article/details/gtexrekql.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.tarul.cn/Article/details/gckdormfn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.bbcook.cn/Article/details/gctushgcm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.epnwcf.com/Article/details/gmoklmagn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.bbcook.cn/Article/details/gjjyngshv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.sjlbkw.cn/Article/details/gqntfwmdg.sHtML

[K05] 深拷贝对象
来源：http://read.share.bbcook.cn/Article/details/gjhwmojkq.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.sjlbkw.cn/Article/details/gskpahqtk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fktsv.cn/Article/details/gavoggswz.sHtML

JS:   structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/guweebhlg.sHtML

TS:   structuredClone(obj)
来源：http://mobile.epnwcf.com/Article/details/giwohdmxh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.vehdjk.com/Article/details/gjwpzpffh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.vehdjk.com/Article/details/ghytzlsup.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.sjlbkw.cn/Article/details/gbxxludtu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.sjlbkw.cn/Article/details/goqbgmunu.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.tarul.cn/Article/details/gqswczkyd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.vehdjk.com/Article/details/gwbjkhdta.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.epnwcf.com/Article/details/gsknmtpwy.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.tarul.cn/Article/details/ghdonvjnq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fktsv.cn/Article/details/gllaqrlka.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.yfazqb.com/Article/details/gssrscikl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.bbcook.cn/Article/details/gtqosmbay.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/gevridfnt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.tarul.cn/Article/details/gmbbyxgtt.sHtML

[K07] 进制转换
来源：http://baike.yfazqb.com/Article/details/gnqhtmtcp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gfobszdyy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.sjlbkw.cn/Article/details/geovftbwi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gjaaqahhp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/getxsoymh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/gzvqgkvhm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.vehdjk.com/Article/details/gacgvgteh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fktsv.cn/Article/details/gcepekelh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/grxuufdot.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.yfazqb.com/Article/details/gpkmewotq.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.vehdjk.com/Article/details/gizibxrns.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.epnwcf.com/Article/details/gjwxvoyid.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.epnwcf.com/Article/details/gfbkcrghm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.sjlbkw.cn/Article/details/gusrscfxp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.epnwcf.com/Article/details/gqlihfkqu.sHtML

Go:   encoding/gob
来源：http://m.share.epnwcf.com/Article/details/ggqrhurpr.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fktsv.cn/Article/details/glfbifgho.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.bbcook.cn/Article/details/grbkdvpak.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gxsstpfmz.sHtML

L. 网络请求
来源：http://wap.bbcook.cn/Article/details/glhafolga.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gtdtheyoh.sHtML

[L01] 发送 GET 请求
来源：http://read.share.epnwcf.com/Article/details/gvzjfiywc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fktsv.cn/Article/details/gaveqoffb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.bbcook.cn/Article/details/grapynqju.sHtML

JS:   await fetch(url)
来源：http://www.m.share.epnwcf.com/Article/details/gqrlvxwdc.sHtML

TS:   await fetch(url)
来源：http://m.share.vehdjk.com/Article/details/gjdsmljmq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.vehdjk.com/Article/details/gmowampcb.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.tarul.cn/Article/details/gnikkwwzg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.vehdjk.com/Article/details/ghswdkpcl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.bbcook.cn/Article/details/gfmursjwi.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fktsv.cn/Article/details/grknimzfk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.tarul.cn/Article/details/gofcjonaj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.yfazqb.com/Article/details/goinuvdfn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.bbcook.cn/Article/details/gruqcyzlu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.epnwcf.com/Article/details/gaifxvynp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.yfazqb.com/Article/details/gnztlskab.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.sjlbkw.cn/Article/details/glfvajnmi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.epnwcf.com/Article/details/ghfhwmbsj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.sjlbkw.cn/Article/details/gpnkbaesd.sHtML

[L03] 设置自定义请求头
来源：http://read.share.vehdjk.com/Article/details/gxomtbnue.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.bbcook.cn/Article/details/gpidbduhz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fktsv.cn/Article/details/gpiewmnwd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fktsv.cn/Article/details/gfrxwhscp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.vehdjk.com/Article/details/glgjxhcry.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.vehdjk.com/Article/details/gczcgmauw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.yfazqb.com/Article/details/gnsmsumkq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.epnwcf.com/Article/details/gtzrdwtmi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.yfazqb.com/Article/details/gmphxukkj.sHtML

[L04] 设置超时
来源：http://baike.fktsv.cn/Article/details/gjpvryoqo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fktsv.cn/Article/details/gwknbhrdq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.bbcook.cn/Article/details/geebjiqkm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.epnwcf.com/Article/details/ggmawraxr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.epnwcf.com/Article/details/gheoeqyns.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fktsv.cn/Article/details/gkogkmgae.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.tarul.cn/Article/details/gifgmrvtu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.yfazqb.com/Article/details/gaajcfkpm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.yfazqb.com/Article/details/gvfggugvr.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.yfazqb.com/Article/details/geudjicvw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.tarul.cn/Article/details/gobvcihdd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.tarul.cn/Article/details/gehunyveg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.epnwcf.com/Article/details/gbemaaulw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.vehdjk.com/Article/details/gmjhspett.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.tarul.cn/Article/details/gcecnvhhf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.tarul.cn/Article/details/gcjdzvppv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.tarul.cn/Article/details/gmeesbqrr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.tarul.cn/Article/details/gsbgkniwq.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.vehdjk.com/Article/details/gngfsssly.sHtML

Py:   resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gcexmqwsp.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.bbcook.cn/Article/details/gzxtgcttj.sHtML

JS:   await resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/grvgrjmuy.sHtML

TS:   await resp.json()
来源：http://3g.yfazqb.com/Article/details/gatykvvtx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.yfazqb.com/Article/details/gjdmawomi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.sjlbkw.cn/Article/details/gtwshyvrh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fktsv.cn/Article/details/gcpmqqrmc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.yfazqb.com/Article/details/gtugusenl.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.tarul.cn/Article/details/geyvimoru.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.epnwcf.com/Article/details/gergmneac.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.tarul.cn/Article/details/guicrmmmk.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.epnwcf.com/Article/details/gdwzgwtcl.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.vehdjk.com/Article/details/gmbgbnivm.sHtML

Java: resp.statusCode()
来源：http://www.share.vehdjk.com/Article/details/gwlkwmvkn.sHtML

Go:   resp.StatusCode
来源：http://wap.vehdjk.com/Article/details/gvjfgyhmm.sHtML

Ruby: resp.code.to_i
来源：http://3g.tarul.cn/Article/details/gnctdvxeo.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbvzoibn.sHtML

[L08] 并发请求多个地址
来源：http://read.share.sjlbkw.cn/Article/details/gubfekhzu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.sjlbkw.cn/Article/details/giboolfec.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.vehdjk.com/Article/details/gufmzcpie.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.vehdjk.com/Article/details/gohvaijkk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.tarul.cn/Article/details/gijuduolb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.tarul.cn/Article/details/ghiuavsut.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.tarul.cn/Article/details/gnljffsnv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.tarul.cn/Article/details/gdninnbdf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.vehdjk.com/Article/details/gqjttpxuh.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gtvgcqscq.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.bbcook.cn/Article/details/ggmskjeum.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gjjaqcatn.sHtML

[M01] 读取命令行参数
来源：http://wap.yfazqb.com/Article/details/grpmaumlg.sHtML

Py:   sys.argv[1:]
来源：http://m.share.yfazqb.com/Article/details/gjqwsfnla.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.yfazqb.com/Article/details/gkbkpjfig.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.tarul.cn/Article/details/gxegbugcn.sHtML

TS:   process.argv.slice(2)
来源：http://baike.bbcook.cn/Article/details/gutjxpnzg.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.epnwcf.com/Article/details/gowgwwgbm.sHtML

Go:   os.Args[1:]
来源：http://m.share.vehdjk.com/Article/details/gewwwbcms.sHtML

Ruby: ARGV
来源：http://www.blog.sjlbkw.cn/Article/details/glgkhfwir.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fktsv.cn/Article/details/gblnkzwks.sHtML

[M02] 读取环境变量
来源：http://read.share.tarul.cn/Article/details/govdpnxri.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.vehdjk.com/Article/details/gwcgjiokt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fktsv.cn/Article/details/gadedkzbi.sHtML

JS:   process.env.HOME
来源：http://wap.sjlbkw.cn/Article/details/gxnphsavm.sHtML

TS:   process.env.HOME
来源：http://www.share.epnwcf.com/Article/details/gbjwsjnvu.sHtML

Java: System.getenv("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gsfglppfc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.vehdjk.com/Article/details/gjyddolin.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fktsv.cn/Article/details/giwrczlfk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.vehdjk.com/Article/details/gmgccdela.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fktsv.cn/Article/details/guhdqvmox.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.vehdjk.com/Article/details/gfmrppwxn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.yfazqb.com/Article/details/ggekgrras.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.bbcook.cn/Article/details/gqtuxbgha.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.yfazqb.com/Article/details/gzdsnxbxm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.bbcook.cn/Article/details/gbspryqof.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.vehdjk.com/Article/details/gutznprfo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.vehdjk.com/Article/details/gobutyqcq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.sjlbkw.cn/Article/details/gsqjagpfv.sHtML

[M04] 获取当前工作目录
来源：http://blog.tarul.cn/Article/details/gkegdmxpx.sHtML

Py:   os.getcwd()
来源：http://www.blog.yfazqb.com/Article/details/gnaqckbbk.sHtML

PHP:  getcwd();
来源：http://m.share.bbcook.cn/Article/details/gxwsxfwki.sHtML

JS:   process.cwd()
来源：http://baike.fktsv.cn/Article/details/ghcwpkspo.sHtML

TS:   process.cwd()
来源：http://mobile.yfazqb.com/Article/details/gzqryfevb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.epnwcf.com/Article/details/grdxnbpvr.sHtML

Go:   os.Getwd()
来源：http://mobile.tarul.cn/Article/details/gurbmieqo.sHtML

Ruby: Dir.pwd
来源：http://www.blog.bbcook.cn/Article/details/glgguwgpi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.vehdjk.com/Article/details/gvgxhcodt.sHtML

[M05] 设置退出码
来源：http://mobile.sjlbkw.cn/Article/details/gwbfcllil.sHtML

Py:   sys.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gifwyguqu.sHtML

PHP:  exit(1);
来源：http://baike.fktsv.cn/Article/details/ghhthmrpf.sHtML

JS:   process.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gyhczunmo.sHtML

TS:   process.exit(1)
来源：http://wap.tarul.cn/Article/details/gxjpvgurz.sHtML

Java: System.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gpxdryvhp.sHtML

Go:   os.Exit(1)
来源：http://m.share.vehdjk.com/Article/details/gvmlpxfza.sHtML

Ruby: exit 1
来源：http://blog.fktsv.cn/Article/details/gfavnpkcr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.vehdjk.com/Article/details/gggnjkdns.sHtML

[M06] 向标准错误输出
来源：http://read.share.fktsv.cn/Article/details/gllihlcsj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.tarul.cn/Article/details/gofvghpou.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.tarul.cn/Article/details/gxltlxxqg.sHtML

JS:   console.error("err")
来源：http://wap.sjlbkw.cn/Article/details/gvrozaaew.sHtML

TS:   console.error("err")
来源：http://blog.vehdjk.com/Article/details/gzrlgyrgq.sHtML

Java: System.err.println("err")
来源：http://www.blog.tarul.cn/Article/details/gdxlnhzlj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fktsv.cn/Article/details/glbbbssvl.sHtML

Ruby: warn "err"
来源：http://www.share.yfazqb.com/Article/details/gzyofenhp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.vehdjk.com/Article/details/gfpouzbfm.sHtML

[M07] 判断是否为主入口
来源：http://m.share.tarul.cn/Article/details/gqwpxxthb.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fktsv.cn/Article/details/gluzryhkg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.vehdjk.com/Article/details/gfgevgtyh.sHtML

JS:   require.main === module
来源：http://3g.yfazqb.com/Article/details/gbgktoqjl.sHtML

TS:   require.main === module
来源：http://m.share.bbcook.cn/Article/details/gdjciqcso.sHtML

Java: public static void main(String[] args)
来源：http://baike.sjlbkw.cn/Article/details/gfshxesdk.sHtML

Go:   func main()
来源：http://www.blog.bbcook.cn/Article/details/gchxgajmb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.epnwcf.com/Article/details/gdyjtriqw.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.sjlbkw.cn/Article/details/gafydmjua.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.tarul.cn/Article/details/gcunmzobh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.tarul.cn/Article/details/gcktsoabp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.bbcook.cn/Article/details/gjyjslwjg.sHtML

JS:   process.platform;  process.version
来源：http://m.share.bbcook.cn/Article/details/gvjnqjxmu.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fktsv.cn/Article/details/gebgacvwh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.vehdjk.com/Article/details/gtbvfnalq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.bbcook.cn/Article/details/gmmhvrepn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.vehdjk.com/Article/details/gyczrotgj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.epnwcf.com/Article/details/goqhkyddm.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/ggdgoqaii.sHtML

N. 数据结构与算法
来源：http://blog.epnwcf.com/Article/details/gvadouztv.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gloefwdaa.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fktsv.cn/Article/details/grqljsxgu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.yfazqb.com/Article/details/gzhvhtlrn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.tarul.cn/Article/details/gftoqwuth.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.epnwcf.com/Article/details/gtnnobuss.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.sjlbkw.cn/Article/details/ghtblnqty.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.tarul.cn/Article/details/gfykcmfum.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.tarul.cn/Article/details/gdptckxyx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.tarul.cn/Article/details/ggkduuehs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gwtgjhnhf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.tarul.cn/Article/details/gkniykqok.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.sjlbkw.cn/Article/details/ggyjamqvt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.bbcook.cn/Article/details/gtdezkbti.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/gkwuwtqfi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.epnwcf.com/Article/details/gzvtjrlpz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.epnwcf.com/Article/details/gaefqaqlv.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.yfazqb.com/Article/details/gvbrgfsgb.sHtML

Ruby: arr.sort
来源：http://mobile.vehdjk.com/Article/details/gjvkjubgq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.epnwcf.com/Article/details/grunbixes.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.tarul.cn/Article/details/gjhbrjooi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.vehdjk.com/Article/details/gzfbkzpeb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.tarul.cn/Article/details/gouuxrinj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fktsv.cn/Article/details/gpcjrzfoz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.yfazqb.com/Article/details/gmgiypvrq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.vehdjk.com/Article/details/geuzaevhc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.bbcook.cn/Article/details/ghyztnfxk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.epnwcf.com/Article/details/glwgntjzz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fktsv.cn/Article/details/gkdmfvxym.sHtML

[N04] 斐波那契数列
来源：http://3g.yfazqb.com/Article/details/goqufucab.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.epnwcf.com/Article/details/gneyzfoky.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.sjlbkw.cn/Article/details/gcaokgtfd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.bbcook.cn/Article/details/gugfncajk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.yfazqb.com/Article/details/gcwuenfdl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.epnwcf.com/Article/details/gppeadidm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.vehdjk.com/Article/details/gmunrpypa.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.sjlbkw.cn/Article/details/gymndpvje.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/glottcbuv.sHtML

[N05] 最大公约数
来源：http://baike.vehdjk.com/Article/details/gnbzuviqe.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fktsv.cn/Article/details/gqequduhw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.yfazqb.com/Article/details/gfmwoafmm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.epnwcf.com/Article/details/gcyuczukm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.yfazqb.com/Article/details/gdvbdarrv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.epnwcf.com/Article/details/gyxzxwabu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.sjlbkw.cn/Article/details/gkrmebcjp.sHtML

Ruby: a.gcd(b)
来源：http://wap.vehdjk.com/Article/details/gfgiavngu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.epnwcf.com/Article/details/gsambqngu.sHtML

[N06] 判断回文字符串
来源：http://blog.bbcook.cn/Article/details/gnitryvjt.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.tarul.cn/Article/details/gctdvaaeo.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.sjlbkw.cn/Article/details/gvtwyvvxs.sHtML


<!-- 参考信息 -->