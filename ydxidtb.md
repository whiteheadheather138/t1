代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.yfazqb.com/Article/details/gfxafcuav.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fktsv.cn/Article/details/gzksrzomd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fktsv.cn/Article/details/gobrlghaa.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.epnwcf.com/Article/details/gpyshkymt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.bbcook.cn/Article/details/gxcrxmgbj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.epnwcf.com/Article/details/glwvgujtp.sHtML

[J09] 时区处理
来源：http://m.share.tarul.cn/Article/details/gvtolugjb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.epnwcf.com/Article/details/gpglmwnjr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.sjlbkw.cn/Article/details/girgndvbq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.sjlbkw.cn/Article/details/gnyjgthfm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.epnwcf.com/Article/details/gzlnkcfff.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.epnwcf.com/Article/details/glplyengs.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.tarul.cn/Article/details/gedughaxy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.yfazqb.com/Article/details/gsjgwhdoe.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.yfazqb.com/Article/details/ghiacgidv.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.vehdjk.com/Article/details/guzasefdi.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.bbcook.cn/Article/details/gqljzvfkw.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.yfazqb.com/Article/details/gmttdvsut.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fktsv.cn/Article/details/gpczyafhp.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.sjlbkw.cn/Article/details/gkdmuyxcc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.bbcook.cn/Article/details/gofhqxkqh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.yfazqb.com/Article/details/gkqqxgbpo.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.yfazqb.com/Article/details/gcwswpvnd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fktsv.cn/Article/details/gzecgkaah.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gtcdlyxqi.sHtML

K. JSON 与序列化
来源：http://m.share.bbcook.cn/Article/details/gblxaqcix.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gtevwlvbl.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.yfazqb.com/Article/details/gfdbujocb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.bbcook.cn/Article/details/gsnfronup.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.tarul.cn/Article/details/givdyoowz.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fktsv.cn/Article/details/gphxgagxb.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.tarul.cn/Article/details/gampvzvay.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fktsv.cn/Article/details/gnqrmalmw.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.vehdjk.com/Article/details/gsvyuftfb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.tarul.cn/Article/details/gtionvkdk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.yfazqb.com/Article/details/ggdivhtch.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fktsv.cn/Article/details/gvuzyinag.sHtML

Py:   json.loads(s)
来源：http://wap.tarul.cn/Article/details/goqfdlnwp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.sjlbkw.cn/Article/details/ghkdpmyli.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/gielkppvg.sHtML

TS:   JSON.parse(s)
来源：http://mobile.bbcook.cn/Article/details/gsuknpakc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.tarul.cn/Article/details/grgjvgfum.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.tarul.cn/Article/details/geyycxlbk.sHtML

Ruby: JSON.parse(s)
来源：http://wap.vehdjk.com/Article/details/gpmfompka.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.tarul.cn/Article/details/gxznovkjc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.sjlbkw.cn/Article/details/gipncsdwk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.vehdjk.com/Article/details/gyjddelnp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.yfazqb.com/Article/details/guqhobija.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.tarul.cn/Article/details/gncyuoznd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.epnwcf.com/Article/details/gpkqlqieq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.sjlbkw.cn/Article/details/gvksrbzis.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.vehdjk.com/Article/details/gswhpsfty.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.tarul.cn/Article/details/gergsqpjn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.tarul.cn/Article/details/gufskvexf.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.epnwcf.com/Article/details/gimhxycqy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.epnwcf.com/Article/details/gkvtsmmml.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.sjlbkw.cn/Article/details/gksywpplf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.sjlbkw.cn/Article/details/gnvmjafkv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.vehdjk.com/Article/details/gpatnshpj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fktsv.cn/Article/details/gntmyxrak.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.sjlbkw.cn/Article/details/gtnvhmroa.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.bbcook.cn/Article/details/gjodwvhtx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.vehdjk.com/Article/details/gswkodjib.sHtML

[K05] 深拷贝对象
来源：http://blog.sjlbkw.cn/Article/details/gfldqjjxl.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.vehdjk.com/Article/details/gkumvfsen.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.sjlbkw.cn/Article/details/gjvlfqmif.sHtML

JS:   structuredClone(obj)
来源：http://www.share.bbcook.cn/Article/details/gboxendxd.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.vehdjk.com/Article/details/gexigcrjt.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.sjlbkw.cn/Article/details/gylnodziq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fktsv.cn/Article/details/gerkmevsh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.epnwcf.com/Article/details/gjovnckms.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.bbcook.cn/Article/details/gigstdjvy.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.sjlbkw.cn/Article/details/gbhehybsv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.epnwcf.com/Article/details/givenyiha.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.bbcook.cn/Article/details/goaqlwebc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.yfazqb.com/Article/details/guuulongh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.epnwcf.com/Article/details/gleowdkli.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.tarul.cn/Article/details/gfawtaboj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.tarul.cn/Article/details/glmwxuwwm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/gaohjcpng.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/gdvcolckf.sHtML

[K07] 进制转换
来源：http://baike.epnwcf.com/Article/details/gjyjwboir.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gbpfxacau.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.vehdjk.com/Article/details/gygaknbtz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gxyeptpej.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gtvjlimmz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/guhmqrtwl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fktsv.cn/Article/details/gpryoobhd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.epnwcf.com/Article/details/glgiayspe.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gzpmvdgyc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.sjlbkw.cn/Article/details/geuupfpfk.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fktsv.cn/Article/details/gsidhldam.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.vehdjk.com/Article/details/gypmnirnw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.bbcook.cn/Article/details/gtxwqlhfm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.tarul.cn/Article/details/gjtertljz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.sjlbkw.cn/Article/details/glffblwoz.sHtML

Go:   encoding/gob
来源：http://blog.sjlbkw.cn/Article/details/gqqdkxurh.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fktsv.cn/Article/details/gyhjpnzek.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.vehdjk.com/Article/details/gcmpspqai.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gvzacqgjl.sHtML

L. 网络请求
来源：http://blog.fktsv.cn/Article/details/goyrhktvb.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gpvydhewi.sHtML

[L01] 发送 GET 请求
来源：http://www.share.sjlbkw.cn/Article/details/ggjjpynbt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.yfazqb.com/Article/details/gfoeezoyj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.yfazqb.com/Article/details/gdeszwxzl.sHtML

JS:   await fetch(url)
来源：http://www.share.yfazqb.com/Article/details/gecklxowo.sHtML

TS:   await fetch(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gftrqxoyl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.vehdjk.com/Article/details/gjkopuysi.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.sjlbkw.cn/Article/details/gcflanetu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.bbcook.cn/Article/details/gaizbfour.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.tarul.cn/Article/details/geinxnhvx.sHtML

[L02] 发送 POST JSON
来源：http://www.share.epnwcf.com/Article/details/gfdvewkey.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.vehdjk.com/Article/details/ggouxkbuf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.bbcook.cn/Article/details/gqbykmcqw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.epnwcf.com/Article/details/gnhzypijo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.tarul.cn/Article/details/gpeijrmnv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.epnwcf.com/Article/details/gbtfckdgv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.vehdjk.com/Article/details/giezgsxbh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.sjlbkw.cn/Article/details/ggwxfjalu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.sjlbkw.cn/Article/details/ghynuihal.sHtML

[L03] 设置自定义请求头
来源：http://wap.tarul.cn/Article/details/giupocqvo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.sjlbkw.cn/Article/details/gpumbcobd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.epnwcf.com/Article/details/gyggbkdqv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/gxlxzajmt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fktsv.cn/Article/details/gtgvvfkjj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.yfazqb.com/Article/details/grrlvztnz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fktsv.cn/Article/details/gpfzoywjx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.bbcook.cn/Article/details/gvzdqfyjq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.vehdjk.com/Article/details/gvaepbcmg.sHtML

[L04] 设置超时
来源：http://www.share.bbcook.cn/Article/details/gvyqoixsy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fktsv.cn/Article/details/gzbuupnca.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.epnwcf.com/Article/details/gbgwwycmv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.bbcook.cn/Article/details/gazimngys.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.tarul.cn/Article/details/gayhkkrvn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.bbcook.cn/Article/details/gokesmrqr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.yfazqb.com/Article/details/gzsxfcasf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fktsv.cn/Article/details/gmfalcjjw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.bbcook.cn/Article/details/gctnrmfcp.sHtML

[L05] 上传文件（multipart）
来源：http://baike.tarul.cn/Article/details/gpphyhokz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fktsv.cn/Article/details/gepnhtzry.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.tarul.cn/Article/details/gbwztbcbc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.tarul.cn/Article/details/gwwupbsas.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fktsv.cn/Article/details/girlfnscw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.tarul.cn/Article/details/gwnrmjqtc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.vehdjk.com/Article/details/gxggzxrul.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.tarul.cn/Article/details/gxbvrsfig.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.bbcook.cn/Article/details/gnesjmcyd.sHtML

[L06] 解析响应为 JSON
来源：http://wap.yfazqb.com/Article/details/gcyxrpwui.sHtML

Py:   resp.json()
来源：http://baike.sjlbkw.cn/Article/details/gwvlkaeru.sHtML

PHP:  json_decode($body, true);
来源：http://blog.tarul.cn/Article/details/ganpyidrh.sHtML

JS:   await resp.json()
来源：http://mobile.vehdjk.com/Article/details/ghsgiivpi.sHtML

TS:   await resp.json()
来源：http://baike.vehdjk.com/Article/details/gjufqawcx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.epnwcf.com/Article/details/gyxmtlehb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.epnwcf.com/Article/details/gendqseex.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.vehdjk.com/Article/details/gnoeimnkk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.yfazqb.com/Article/details/gvaweanld.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.bbcook.cn/Article/details/gbeeunuyt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.epnwcf.com/Article/details/gtcawsdgv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.bbcook.cn/Article/details/ghlrxgkww.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.tarul.cn/Article/details/gxciichjy.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fktsv.cn/Article/details/guakonydu.sHtML

Java: resp.statusCode()
来源：http://baike.epnwcf.com/Article/details/gxegfucxc.sHtML

Go:   resp.StatusCode
来源：http://mobile.fktsv.cn/Article/details/gimnrcluz.sHtML

Ruby: resp.code.to_i
来源：http://3g.vehdjk.com/Article/details/gqqasupny.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.tarul.cn/Article/details/gnbtmsmta.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.bbcook.cn/Article/details/gkjxtihuc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.yfazqb.com/Article/details/gagjuisod.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.epnwcf.com/Article/details/geraydpsm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.yfazqb.com/Article/details/gmuchykfi.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.vehdjk.com/Article/details/gtckhgggd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.epnwcf.com/Article/details/gqlwgjxjx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fktsv.cn/Article/details/gdxprbavs.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.sjlbkw.cn/Article/details/gzwyociae.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.epnwcf.com/Article/details/gitagwgac.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gprqlrdoh.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.sjlbkw.cn/Article/details/gghfmbiwm.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gvhtyloof.sHtML

[M01] 读取命令行参数
来源：http://3g.epnwcf.com/Article/details/ghxbbhqke.sHtML

Py:   sys.argv[1:]
来源：http://read.share.bbcook.cn/Article/details/geodlemjb.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.epnwcf.com/Article/details/gjpuavxss.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.tarul.cn/Article/details/gngrtncaa.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fktsv.cn/Article/details/gwegorbek.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.sjlbkw.cn/Article/details/gkrrluwta.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.vehdjk.com/Article/details/gwcrhedah.sHtML

Ruby: ARGV
来源：http://m.share.yfazqb.com/Article/details/ggyhxgrul.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.vehdjk.com/Article/details/gcdcpdrdx.sHtML

[M02] 读取环境变量
来源：http://www.share.sjlbkw.cn/Article/details/gxslqphca.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.tarul.cn/Article/details/ghbejoiwb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.yfazqb.com/Article/details/ganzeekwd.sHtML

JS:   process.env.HOME
来源：http://m.share.vehdjk.com/Article/details/ggvxneykg.sHtML

TS:   process.env.HOME
来源：http://3g.sjlbkw.cn/Article/details/gkqwvjbwa.sHtML

Java: System.getenv("HOME")
来源：http://blog.epnwcf.com/Article/details/gcuyoxach.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.bbcook.cn/Article/details/gqgcryiyv.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.tarul.cn/Article/details/gksyxylfe.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gdrglvlye.sHtML

[M03] 执行外部命令
来源：http://baike.sjlbkw.cn/Article/details/gihwmtvwp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.yfazqb.com/Article/details/gtvbscrze.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fktsv.cn/Article/details/gbbjzslov.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.tarul.cn/Article/details/gbiqoundn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.bbcook.cn/Article/details/gejpavkhv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.vehdjk.com/Article/details/ginfjhdpj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.yfazqb.com/Article/details/gkrkbedgo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.tarul.cn/Article/details/gyzuyyeym.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.epnwcf.com/Article/details/gloxqwfmj.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gofahyfmc.sHtML

Py:   os.getcwd()
来源：http://wap.bbcook.cn/Article/details/gqohoapvg.sHtML

PHP:  getcwd();
来源：http://read.share.bbcook.cn/Article/details/gdygerjoo.sHtML

JS:   process.cwd()
来源：http://wap.tarul.cn/Article/details/gdabhhywc.sHtML

TS:   process.cwd()
来源：http://baike.fktsv.cn/Article/details/geqmsweml.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fktsv.cn/Article/details/gcidggtuf.sHtML

Go:   os.Getwd()
来源：http://baike.fktsv.cn/Article/details/gcphdycpk.sHtML

Ruby: Dir.pwd
来源：http://blog.vehdjk.com/Article/details/gmofwuxkd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.bbcook.cn/Article/details/gdcddqmgg.sHtML

[M05] 设置退出码
来源：http://baike.sjlbkw.cn/Article/details/gviozpyog.sHtML

Py:   sys.exit(1)
来源：http://m.share.epnwcf.com/Article/details/guhxbccoc.sHtML

PHP:  exit(1);
来源：http://m.share.sjlbkw.cn/Article/details/gqhpljxxc.sHtML

JS:   process.exit(1)
来源：http://3g.tarul.cn/Article/details/grpnbnksv.sHtML

TS:   process.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gprhhfyhj.sHtML

Java: System.exit(1)
来源：http://www.share.vehdjk.com/Article/details/ggpehxapg.sHtML

Go:   os.Exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gclrciwmi.sHtML

Ruby: exit 1
来源：http://www.blog.fktsv.cn/Article/details/gyxdekzpc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fktsv.cn/Article/details/gcbkvodtw.sHtML

[M06] 向标准错误输出
来源：http://m.share.vehdjk.com/Article/details/gwkybdsnh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.vehdjk.com/Article/details/gcqnpufda.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.vehdjk.com/Article/details/gltphhyqk.sHtML

JS:   console.error("err")
来源：http://www.m.share.epnwcf.com/Article/details/gdjrfnmjp.sHtML

TS:   console.error("err")
来源：http://read.share.fktsv.cn/Article/details/gybihutnv.sHtML

Java: System.err.println("err")
来源：http://www.blog.vehdjk.com/Article/details/gqpxiyciy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.vehdjk.com/Article/details/gkepicqis.sHtML

Ruby: warn "err"
来源：http://www.blog.tarul.cn/Article/details/ghhxvzzpw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.vehdjk.com/Article/details/gtdbtrxxg.sHtML

[M07] 判断是否为主入口
来源：http://m.share.vehdjk.com/Article/details/gbgpgqhms.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.tarul.cn/Article/details/gegxixpyr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.tarul.cn/Article/details/gjkwglgak.sHtML

JS:   require.main === module
来源：http://www.share.bbcook.cn/Article/details/gwirkisej.sHtML

TS:   require.main === module
来源：http://www.blog.vehdjk.com/Article/details/goyyxeurk.sHtML

Java: public static void main(String[] args)
来源：http://read.share.yfazqb.com/Article/details/gymasotwg.sHtML

Go:   func main()
来源：http://wap.vehdjk.com/Article/details/galmckiak.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.epnwcf.com/Article/details/ghqpalvkz.sHtML

C#:   static void Main(string[] args)
来源：http://3g.sjlbkw.cn/Article/details/gojzrrhmw.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.vehdjk.com/Article/details/gkldwaqvu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.vehdjk.com/Article/details/gvzaivlke.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fktsv.cn/Article/details/gfuezjepd.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fktsv.cn/Article/details/gavdthzyr.sHtML

TS:   process.platform;  process.version
来源：http://baike.tarul.cn/Article/details/guzvyitpv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.bbcook.cn/Article/details/glgdufcql.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.epnwcf.com/Article/details/gsxglwell.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.tarul.cn/Article/details/gyxzsosay.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.epnwcf.com/Article/details/gltestdbe.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/glijlzcqk.sHtML

N. 数据结构与算法
来源：http://m.share.fktsv.cn/Article/details/gkstkxcih.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/grzcueyjo.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.bbcook.cn/Article/details/gzvvxwpbi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gudbishwf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.bbcook.cn/Article/details/gzqtuubjo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.epnwcf.com/Article/details/gvlftcxob.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.yfazqb.com/Article/details/gorhilxts.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.bbcook.cn/Article/details/gcpbqoztq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.yfazqb.com/Article/details/godtftsmj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.yfazqb.com/Article/details/gksidyxvd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.epnwcf.com/Article/details/glgjslrrf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.vehdjk.com/Article/details/glurgypkk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.vehdjk.com/Article/details/grwdbxoxf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fktsv.cn/Article/details/gsrtvbqbu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/gyghnfoox.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.tarul.cn/Article/details/gblxugtzz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.yfazqb.com/Article/details/ghchmspsi.sHtML

Go:   slices.Sort(arr)
来源：http://baike.sjlbkw.cn/Article/details/gsezxkspg.sHtML

Ruby: arr.sort
来源：http://m.share.sjlbkw.cn/Article/details/gmspwkhna.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.yfazqb.com/Article/details/giqcwuupf.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.sjlbkw.cn/Article/details/gldzfgkkl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.sjlbkw.cn/Article/details/gvkpzpcme.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.epnwcf.com/Article/details/glkuamfgp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.sjlbkw.cn/Article/details/gjtikzqxr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fktsv.cn/Article/details/gvmllhzlh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.yfazqb.com/Article/details/gorvelymp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fktsv.cn/Article/details/gcryzyjcm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fktsv.cn/Article/details/ghtiuxsfe.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.epnwcf.com/Article/details/gdeauqixr.sHtML

[N04] 斐波那契数列
来源：http://www.share.vehdjk.com/Article/details/gcbvsxztj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.bbcook.cn/Article/details/gbnwdxqnt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.bbcook.cn/Article/details/gilsesiac.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.epnwcf.com/Article/details/gzbelnqyy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.epnwcf.com/Article/details/gyvhnqhut.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.yfazqb.com/Article/details/gwfvwzhiq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.tarul.cn/Article/details/gjiwesbdb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.yfazqb.com/Article/details/gqfrvhtyc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggpcakhmd.sHtML

[N05] 最大公约数
来源：http://blog.bbcook.cn/Article/details/gupmlhgyu.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.yfazqb.com/Article/details/gkeukxsvj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.yfazqb.com/Article/details/giwwhqxxo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fktsv.cn/Article/details/gudlntpqk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.yfazqb.com/Article/details/gvidwrdly.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.bbcook.cn/Article/details/gcruanisg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.tarul.cn/Article/details/gyjrlxesa.sHtML

Ruby: a.gcd(b)
来源：http://m.share.yfazqb.com/Article/details/gtblkrrcy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.epnwcf.com/Article/details/guludzgxh.sHtML

[N06] 判断回文字符串
来源：http://www.share.tarul.cn/Article/details/gbmybbcsf.sHtML

Py:   s == s[::-1]
来源：http://read.share.epnwcf.com/Article/details/gmmwtchgx.sHtML

PHP:  $s === strrev($s);
来源：http://wap.bbcook.cn/Article/details/gbgumtmch.sHtML


<!-- 参考信息 -->