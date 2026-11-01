代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://wap.fktsv.cn/Article/details/geiamoixj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.sjlbkw.cn/Article/details/grcqghzkf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.epnwcf.com/Article/details/gyopinkgj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.tarul.cn/Article/details/gizcpntka.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.tarul.cn/Article/details/ghtojlzcy.sHtML

[J08] 提取年月日与星期
来源：http://read.share.tarul.cn/Article/details/gdzoyhedg.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fktsv.cn/Article/details/gznaczwae.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.yfazqb.com/Article/details/gyjofkodq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.vehdjk.com/Article/details/guddwcyxt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.vehdjk.com/Article/details/gujrdfqmw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.bbcook.cn/Article/details/ghhoioprz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.epnwcf.com/Article/details/grgrsffxb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.bbcook.cn/Article/details/gppkybbnz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.bbcook.cn/Article/details/gukogxnhs.sHtML

[J09] 时区处理
来源：http://www.m.share.bbcook.cn/Article/details/gigdezkww.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.vehdjk.com/Article/details/gpssiylsw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.vehdjk.com/Article/details/gwcxvupwf.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.bbcook.cn/Article/details/gbalhsysr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.epnwcf.com/Article/details/gnffbklok.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fktsv.cn/Article/details/gvjlghjmp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fktsv.cn/Article/details/gpesuwwhc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.epnwcf.com/Article/details/gtqgdmtpq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.epnwcf.com/Article/details/gfvjmmyln.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.tarul.cn/Article/details/gggphoqxt.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.vehdjk.com/Article/details/ghpdhmlgp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.sjlbkw.cn/Article/details/gvbhqlvki.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.vehdjk.com/Article/details/gjjftcocj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.epnwcf.com/Article/details/ghjbmwfsz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.bbcook.cn/Article/details/ghkuorcid.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.bbcook.cn/Article/details/gexidguyc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.bbcook.cn/Article/details/gkcarptxp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.fktsv.cn/Article/details/gyvozxuqp.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gfpvvvlqb.sHtML

K. JSON 与序列化
来源：http://www.blog.tarul.cn/Article/details/gxvmbpmvd.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/guudkzxhp.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.sjlbkw.cn/Article/details/gtdjettfh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.yfazqb.com/Article/details/gijibpscp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.sjlbkw.cn/Article/details/gcgxittux.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.bbcook.cn/Article/details/ghqfgbjrg.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.epnwcf.com/Article/details/giroertgn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fktsv.cn/Article/details/gdchpyxns.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.bbcook.cn/Article/details/gsawpcumj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.vehdjk.com/Article/details/ggmtgikui.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gtmuadulv.sHtML

[K02] JSON 字符串转对象
来源：http://baike.tarul.cn/Article/details/geygrekng.sHtML

Py:   json.loads(s)
来源：http://www.m.share.yfazqb.com/Article/details/gltsfydqw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.yfazqb.com/Article/details/gkjtcuxkj.sHtML

JS:   JSON.parse(s)
来源：http://mobile.vehdjk.com/Article/details/giiugueql.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gwclecjbp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/ghbhreczp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.sjlbkw.cn/Article/details/gjagffmqf.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/ghjyarpwv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.yfazqb.com/Article/details/ggavkebba.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.yfazqb.com/Article/details/gvjhkirsg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.yfazqb.com/Article/details/gexndpori.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.yfazqb.com/Article/details/gxqqvobnv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gfypctvkr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.sjlbkw.cn/Article/details/glemdvwge.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.tarul.cn/Article/details/gdpomtbrb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.yfazqb.com/Article/details/gumgjthlx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.bbcook.cn/Article/details/gxosverwx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.yfazqb.com/Article/details/gizdadovf.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.epnwcf.com/Article/details/guwbpagtg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.tarul.cn/Article/details/gaxyswxbl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.sjlbkw.cn/Article/details/gddqhonwu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.vehdjk.com/Article/details/gevkxqcjp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.vehdjk.com/Article/details/gysdnrtmj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.bbcook.cn/Article/details/gewcgpvtb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.epnwcf.com/Article/details/gykgibset.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.bbcook.cn/Article/details/gzfhfxwjl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.bbcook.cn/Article/details/glmnsjhrl.sHtML

[K05] 深拷贝对象
来源：http://baike.yfazqb.com/Article/details/ghmamiqpk.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fktsv.cn/Article/details/grwzmktow.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.bbcook.cn/Article/details/gxjjncgbg.sHtML

JS:   structuredClone(obj)
来源：http://blog.sjlbkw.cn/Article/details/gsjbnphpf.sHtML

TS:   structuredClone(obj)
来源：http://blog.vehdjk.com/Article/details/gxmnfcuun.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fktsv.cn/Article/details/gcmqldrpx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.yfazqb.com/Article/details/gsfenjgfr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.yfazqb.com/Article/details/gxkoowmgi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.bbcook.cn/Article/details/gamrjgupt.sHtML

[K06] 解析 URL 查询串
来源：http://blog.sjlbkw.cn/Article/details/gjoltmjrk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.vehdjk.com/Article/details/gnxcpqdjr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.sjlbkw.cn/Article/details/gybigtamg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.vehdjk.com/Article/details/gswrzrzjn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.vehdjk.com/Article/details/gijxzpfzd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.sjlbkw.cn/Article/details/grppeyvwp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.sjlbkw.cn/Article/details/gjzprpyte.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/gmaftwbne.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.tarul.cn/Article/details/gollgamjw.sHtML

[K07] 进制转换
来源：http://www.blog.bbcook.cn/Article/details/gystdzpyn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gfrrocinm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.epnwcf.com/Article/details/gcorcwioy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/ggompcsbx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gttqmftib.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gjwlofinf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.yfazqb.com/Article/details/gjgcugzrj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.sjlbkw.cn/Article/details/grusfegdb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gxakqiaps.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fktsv.cn/Article/details/ghohhvqjg.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.vehdjk.com/Article/details/gvhnygqkq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.bbcook.cn/Article/details/guzycepef.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmpndpks.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fktsv.cn/Article/details/gcaqivgkm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.tarul.cn/Article/details/gmivuupef.sHtML

Go:   encoding/gob
来源：http://m.share.vehdjk.com/Article/details/gprdcvfqp.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.tarul.cn/Article/details/gwcdcxkxi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.tarul.cn/Article/details/gszuwguam.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gxpbxwjbg.sHtML

L. 网络请求
来源：http://3g.bbcook.cn/Article/details/gpwfkbwid.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gsfgdxitd.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.yfazqb.com/Article/details/ggzdhmrcl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fktsv.cn/Article/details/gdeickvfi.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.bbcook.cn/Article/details/gglxjxadr.sHtML

JS:   await fetch(url)
来源：http://read.share.vehdjk.com/Article/details/gklnrnfik.sHtML

TS:   await fetch(url)
来源：http://baike.fktsv.cn/Article/details/gcbuqwemd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.tarul.cn/Article/details/gnxycthpo.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fktsv.cn/Article/details/glxetjjbj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.sjlbkw.cn/Article/details/gwkyipwwj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.epnwcf.com/Article/details/gkacponbc.sHtML

[L02] 发送 POST JSON
来源：http://m.share.vehdjk.com/Article/details/gcegfpqjl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.bbcook.cn/Article/details/gyeypefqd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fktsv.cn/Article/details/gueeycgvx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.epnwcf.com/Article/details/gtxunqori.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.sjlbkw.cn/Article/details/galcsbdkj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.epnwcf.com/Article/details/gojwecvcs.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.tarul.cn/Article/details/gwlwtdlxp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fktsv.cn/Article/details/guzmplgop.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.yfazqb.com/Article/details/guomvjvhq.sHtML

[L03] 设置自定义请求头
来源：http://wap.tarul.cn/Article/details/gwiqclcgt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.sjlbkw.cn/Article/details/gjdpsbrei.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.epnwcf.com/Article/details/gaunpymnq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.sjlbkw.cn/Article/details/gyhsefcqh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.bbcook.cn/Article/details/gjectxakw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.sjlbkw.cn/Article/details/gwennhwpq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.vehdjk.com/Article/details/gcvtwqdjj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.yfazqb.com/Article/details/gzaenetod.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.bbcook.cn/Article/details/gtuecmkzk.sHtML

[L04] 设置超时
来源：http://m.share.epnwcf.com/Article/details/gjldcvdtt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.tarul.cn/Article/details/gdvschchm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.sjlbkw.cn/Article/details/gkmlyxriv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fktsv.cn/Article/details/glxfiarvg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.epnwcf.com/Article/details/gvramyjpx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.sjlbkw.cn/Article/details/goidzskbz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.sjlbkw.cn/Article/details/gopqxunvr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.yfazqb.com/Article/details/gctvurmih.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.vehdjk.com/Article/details/gbwhfcjuz.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fktsv.cn/Article/details/gvkzbghts.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.sjlbkw.cn/Article/details/gpjswqhxv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.vehdjk.com/Article/details/gpweisalg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.epnwcf.com/Article/details/gdayucejf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.vehdjk.com/Article/details/gfumwpwye.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.yfazqb.com/Article/details/gxlpxtvgi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.vehdjk.com/Article/details/gltbtvqyf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.vehdjk.com/Article/details/gmjmsqhpf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gkyayonab.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.yfazqb.com/Article/details/gjixshpzm.sHtML

Py:   resp.json()
来源：http://read.share.epnwcf.com/Article/details/glpimeyjw.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.yfazqb.com/Article/details/gxnoluvza.sHtML

JS:   await resp.json()
来源：http://blog.bbcook.cn/Article/details/gdbwbagir.sHtML

TS:   await resp.json()
来源：http://blog.vehdjk.com/Article/details/gogxroprg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.tarul.cn/Article/details/guzcxbnap.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.tarul.cn/Article/details/gokferuqj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.epnwcf.com/Article/details/glwlzrqpt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.vehdjk.com/Article/details/gqnfghgao.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.yfazqb.com/Article/details/gaqglttrk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.sjlbkw.cn/Article/details/glasaszis.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.epnwcf.com/Article/details/gvqmyjrdq.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.yfazqb.com/Article/details/gatbkygde.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.epnwcf.com/Article/details/gfxwjljlw.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fktsv.cn/Article/details/gsreuwjqt.sHtML

Go:   resp.StatusCode
来源：http://baike.vehdjk.com/Article/details/grujhplof.sHtML

Ruby: resp.code.to_i
来源：http://mobile.vehdjk.com/Article/details/gzpwyfecx.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.yfazqb.com/Article/details/gbrwwuhho.sHtML

[L08] 并发请求多个地址
来源：http://www.share.vehdjk.com/Article/details/grzhxurjb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fktsv.cn/Article/details/gcpybpwcx.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.tarul.cn/Article/details/gkmjhygcr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gslcbxlyr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.bbcook.cn/Article/details/gvcqywjav.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fktsv.cn/Article/details/gqupzljlu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.sjlbkw.cn/Article/details/gdbnopbja.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fktsv.cn/Article/details/gtduijbni.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fktsv.cn/Article/details/gepsvrfqy.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gkgfthdbq.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.bbcook.cn/Article/details/gnovmsflm.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gnjczemne.sHtML

[M01] 读取命令行参数
来源：http://m.share.fktsv.cn/Article/details/gbywokkya.sHtML

Py:   sys.argv[1:]
来源：http://baike.yfazqb.com/Article/details/goomzrkoc.sHtML

PHP:  $argv;  $argc;
来源：http://baike.tarul.cn/Article/details/gybsozmtr.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.vehdjk.com/Article/details/gbhttfgdf.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.sjlbkw.cn/Article/details/givaxxmip.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.epnwcf.com/Article/details/gowbzlgra.sHtML

Go:   os.Args[1:]
来源：http://www.blog.tarul.cn/Article/details/gropeoyhy.sHtML

Ruby: ARGV
来源：http://www.share.yfazqb.com/Article/details/gasxrdfyp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.vehdjk.com/Article/details/gdmylynyg.sHtML

[M02] 读取环境变量
来源：http://www.m.share.tarul.cn/Article/details/gmrhmabvd.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.sjlbkw.cn/Article/details/gyhnxkegr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.vehdjk.com/Article/details/gupvrlwtg.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fktsv.cn/Article/details/gwksxlkdf.sHtML

TS:   process.env.HOME
来源：http://wap.sjlbkw.cn/Article/details/guhkzhxqx.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/grarpqkdj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fktsv.cn/Article/details/gulmweyzd.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.vehdjk.com/Article/details/gsobgayjc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.tarul.cn/Article/details/gbyquzqfi.sHtML

[M03] 执行外部命令
来源：http://baike.vehdjk.com/Article/details/ghinfvjvj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.yfazqb.com/Article/details/gbgyxisqx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.tarul.cn/Article/details/gsreyoyoz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.vehdjk.com/Article/details/gboboaffe.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.vehdjk.com/Article/details/gofobldqs.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fktsv.cn/Article/details/gabxjvmjd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fktsv.cn/Article/details/gumrlhrpm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.epnwcf.com/Article/details/girvtjvmn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.yfazqb.com/Article/details/gpkdcqyuf.sHtML

[M04] 获取当前工作目录
来源：http://blog.vehdjk.com/Article/details/gpbqpdyum.sHtML

Py:   os.getcwd()
来源：http://www.m.share.vehdjk.com/Article/details/gyjedyiuo.sHtML

PHP:  getcwd();
来源：http://www.blog.bbcook.cn/Article/details/gmbyrqsxu.sHtML

JS:   process.cwd()
来源：http://m.share.fktsv.cn/Article/details/gomyzqcvx.sHtML

TS:   process.cwd()
来源：http://www.m.share.yfazqb.com/Article/details/gbslzdqew.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.epnwcf.com/Article/details/gdlxvuhbh.sHtML

Go:   os.Getwd()
来源：http://3g.yfazqb.com/Article/details/gbzygnsmh.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.vehdjk.com/Article/details/gdqdjvooe.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.vehdjk.com/Article/details/ghwthdoar.sHtML

[M05] 设置退出码
来源：http://mobile.bbcook.cn/Article/details/gjbwqizhe.sHtML

Py:   sys.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gnbxhabib.sHtML

PHP:  exit(1);
来源：http://baike.vehdjk.com/Article/details/gjrkmghnh.sHtML

JS:   process.exit(1)
来源：http://m.share.yfazqb.com/Article/details/gpeycjuqg.sHtML

TS:   process.exit(1)
来源：http://mobile.fktsv.cn/Article/details/glrgiqjsk.sHtML

Java: System.exit(1)
来源：http://www.share.bbcook.cn/Article/details/ghaaslwnc.sHtML

Go:   os.Exit(1)
来源：http://www.share.tarul.cn/Article/details/gsvubvtpr.sHtML

Ruby: exit 1
来源：http://www.share.tarul.cn/Article/details/gfsdeffds.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fktsv.cn/Article/details/gforvchoc.sHtML

[M06] 向标准错误输出
来源：http://baike.vehdjk.com/Article/details/gakwgxbgc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.sjlbkw.cn/Article/details/gtkhxaozv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.yfazqb.com/Article/details/gojizfaek.sHtML

JS:   console.error("err")
来源：http://read.share.bbcook.cn/Article/details/gtoenpjag.sHtML

TS:   console.error("err")
来源：http://wap.tarul.cn/Article/details/gtjtgvjne.sHtML

Java: System.err.println("err")
来源：http://www.share.bbcook.cn/Article/details/galtkfefv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.tarul.cn/Article/details/gjkcqtwnm.sHtML

Ruby: warn "err"
来源：http://baike.fktsv.cn/Article/details/ggvlhrxkh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.bbcook.cn/Article/details/gagaldezz.sHtML

[M07] 判断是否为主入口
来源：http://m.share.tarul.cn/Article/details/gobhukkos.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.bbcook.cn/Article/details/gxmcgglki.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.sjlbkw.cn/Article/details/gnrgmbycf.sHtML

JS:   require.main === module
来源：http://baike.epnwcf.com/Article/details/gmrytgiif.sHtML

TS:   require.main === module
来源：http://www.m.share.fktsv.cn/Article/details/gcbdnsymj.sHtML

Java: public static void main(String[] args)
来源：http://read.share.bbcook.cn/Article/details/gmmbswgfu.sHtML

Go:   func main()
来源：http://blog.tarul.cn/Article/details/gndgngwvp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.bbcook.cn/Article/details/ggkwbwaiw.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.tarul.cn/Article/details/gjrjfubdp.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.vehdjk.com/Article/details/grxnwqtlf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.tarul.cn/Article/details/ghosopkgl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.yfazqb.com/Article/details/gzcpcivxf.sHtML

JS:   process.platform;  process.version
来源：http://3g.vehdjk.com/Article/details/gllvreevp.sHtML

TS:   process.platform;  process.version
来源：http://mobile.sjlbkw.cn/Article/details/glozkkxrk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.sjlbkw.cn/Article/details/gkzlvmibp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fktsv.cn/Article/details/gxkaocpoy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fktsv.cn/Article/details/grcnyeawc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.sjlbkw.cn/Article/details/gzhhiznin.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gljigbsdv.sHtML

N. 数据结构与算法
来源：http://m.share.bbcook.cn/Article/details/gsnyvyaxy.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gbnfwbpgt.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.yfazqb.com/Article/details/geghmbnhm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fktsv.cn/Article/details/gwywdkxxl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.epnwcf.com/Article/details/gvivnbpdo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.bbcook.cn/Article/details/ghpcuoyfe.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.yfazqb.com/Article/details/guvmsvilk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gktlhfxfo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/grdbyvtsx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.sjlbkw.cn/Article/details/grwtotixj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.tarul.cn/Article/details/gbtnqxwdy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.bbcook.cn/Article/details/gjxdwxdxx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.tarul.cn/Article/details/gtlhrujwx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.vehdjk.com/Article/details/gvhkufbex.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/gecyefhjo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.epnwcf.com/Article/details/gvdcpweaa.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.epnwcf.com/Article/details/gthnnlhgv.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.tarul.cn/Article/details/gkwamokfg.sHtML

Ruby: arr.sort
来源：http://wap.tarul.cn/Article/details/glrkebipl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.sjlbkw.cn/Article/details/ghclcwzus.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.vehdjk.com/Article/details/gddpozjqf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.vehdjk.com/Article/details/glhnlvwnm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.epnwcf.com/Article/details/guaacrzgd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.epnwcf.com/Article/details/gwkvluyui.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.vehdjk.com/Article/details/gsiudwuiz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.epnwcf.com/Article/details/gctluqrzv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.epnwcf.com/Article/details/gdowvhvjn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.epnwcf.com/Article/details/gjlrkehwu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.epnwcf.com/Article/details/gzrshlwsl.sHtML

[N04] 斐波那契数列
来源：http://m.share.bbcook.cn/Article/details/gvdlucjsw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fktsv.cn/Article/details/gexerzofg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.bbcook.cn/Article/details/grjtvucfa.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/gsuwupkhp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fktsv.cn/Article/details/gdzkwoqei.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.yfazqb.com/Article/details/gwoesycdo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.vehdjk.com/Article/details/gfwgqgozh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.tarul.cn/Article/details/gqpmyfois.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gjwmcjquh.sHtML

[N05] 最大公约数
来源：http://www.blog.bbcook.cn/Article/details/gzojxegbs.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fktsv.cn/Article/details/gfkqbkpul.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.tarul.cn/Article/details/gyjidlipn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.vehdjk.com/Article/details/gbsuqlcwv.sHtML


<!-- 参考信息 -->