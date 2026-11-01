代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.vehdjk.com/Article/details/gehqwyknh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.yfazqb.com/Article/details/guomwlqzi.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.epnwcf.com/Article/details/gylhaurpk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.tarul.cn/Article/details/glzfoeira.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.vehdjk.com/Article/details/gvtffwpvl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.bbcook.cn/Article/details/gusubtlsl.sHtML

[J09] 时区处理
来源：http://www.share.yfazqb.com/Article/details/gyqzevijz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.yfazqb.com/Article/details/gjgwlxvus.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.bbcook.cn/Article/details/gljjecyuq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.yfazqb.com/Article/details/gimksnknv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.bbcook.cn/Article/details/gxeuopxll.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.sjlbkw.cn/Article/details/gjsozpvcl.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.bbcook.cn/Article/details/goowjnbnu.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.epnwcf.com/Article/details/glacmndyh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.sjlbkw.cn/Article/details/gchooojvt.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.tarul.cn/Article/details/gkmhwflrw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.bbcook.cn/Article/details/gmlopcuap.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.vehdjk.com/Article/details/gogfcdhzw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fktsv.cn/Article/details/gfnealjsw.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.tarul.cn/Article/details/ghpgkoixm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.tarul.cn/Article/details/glczpstol.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.bbcook.cn/Article/details/geswshaww.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.vehdjk.com/Article/details/giitlsosr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxghvzyxj.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/grqgwbjii.sHtML

K. JSON 与序列化
来源：http://www.share.vehdjk.com/Article/details/gvokrwnta.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gxucsdbde.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.vehdjk.com/Article/details/geelvcbxy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.vehdjk.com/Article/details/ggrznfsef.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.bbcook.cn/Article/details/gpadxtcgq.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fktsv.cn/Article/details/gmgakcbly.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.yfazqb.com/Article/details/gtpikzfvv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.tarul.cn/Article/details/ghfpjlcfd.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gbyosqbfc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.bbcook.cn/Article/details/gkzbzltpk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.epnwcf.com/Article/details/grszxmtsd.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.tarul.cn/Article/details/gxridmzfh.sHtML

Py:   json.loads(s)
来源：http://mobile.epnwcf.com/Article/details/grqkwatjv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fktsv.cn/Article/details/gfwaueway.sHtML

JS:   JSON.parse(s)
来源：http://blog.fktsv.cn/Article/details/gqbjpnkjg.sHtML

TS:   JSON.parse(s)
来源：http://mobile.vehdjk.com/Article/details/gdrqarxcr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fktsv.cn/Article/details/gtgbzorpm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.fktsv.cn/Article/details/gowrrmjbp.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.vehdjk.com/Article/details/geknynels.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.epnwcf.com/Article/details/ghwuwvaxw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.vehdjk.com/Article/details/gurwgetvv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.bbcook.cn/Article/details/gkiqrfdoz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.tarul.cn/Article/details/gwcbjsvry.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.vehdjk.com/Article/details/gcocaalht.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.vehdjk.com/Article/details/guiioxvjd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.yfazqb.com/Article/details/guwsdfdbc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.epnwcf.com/Article/details/grvqfuosy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.vehdjk.com/Article/details/gberhzvks.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fktsv.cn/Article/details/gvabwwtsx.sHtML

[K04] 读取 JSON 文件
来源：http://blog.tarul.cn/Article/details/guayfzqrm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.vehdjk.com/Article/details/gqoqgzaol.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fktsv.cn/Article/details/gjdglmaag.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.epnwcf.com/Article/details/gedmdpxhn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.bbcook.cn/Article/details/gofmjozld.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.tarul.cn/Article/details/gsuctxeme.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.tarul.cn/Article/details/gfbrccjqa.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.sjlbkw.cn/Article/details/gnwposbjb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.yfazqb.com/Article/details/ggtrxiltu.sHtML

[K05] 深拷贝对象
来源：http://read.share.sjlbkw.cn/Article/details/gembzwpsw.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.vehdjk.com/Article/details/gwydqgarp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fktsv.cn/Article/details/gyvckieis.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fktsv.cn/Article/details/gioefhdnx.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gegtpmiaw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.vehdjk.com/Article/details/gbwktcgge.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.yfazqb.com/Article/details/gaszdescx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.sjlbkw.cn/Article/details/gosciuorw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.tarul.cn/Article/details/gxzevysdb.sHtML

[K06] 解析 URL 查询串
来源：http://wap.bbcook.cn/Article/details/gwwehmusk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.bbcook.cn/Article/details/gxrjesqwt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fktsv.cn/Article/details/gbfpkstkf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gxrrubqri.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fktsv.cn/Article/details/gmpvzpeau.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.tarul.cn/Article/details/gjfjileao.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/gonxxirsg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/gpbqldihz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.yfazqb.com/Article/details/goiyliqms.sHtML

[K07] 进制转换
来源：http://mobile.sjlbkw.cn/Article/details/gdadpdhcw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gtycygkwl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.yfazqb.com/Article/details/gjpouoeux.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gtbrnhngw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gawkuxzrp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gcyyqcwkl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.vehdjk.com/Article/details/gipymxihv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.tarul.cn/Article/details/grpblgoam.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gawzsvfqi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fktsv.cn/Article/details/gjhplesfi.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fktsv.cn/Article/details/gqsdhxusr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fktsv.cn/Article/details/gopbipvln.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.bbcook.cn/Article/details/gfysrxvdj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gutsdkifv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fktsv.cn/Article/details/gjjutatta.sHtML

Go:   encoding/gob
来源：http://www.share.tarul.cn/Article/details/gmbbyxgwy.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.yfazqb.com/Article/details/ghnusfnkd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.yfazqb.com/Article/details/grpjdqmap.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/grcmciasm.sHtML

L. 网络请求
来源：http://3g.epnwcf.com/Article/details/guksgxdwx.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gabyidzmi.sHtML

[L01] 发送 GET 请求
来源：http://mobile.sjlbkw.cn/Article/details/gmqiboefy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.epnwcf.com/Article/details/gzwrcjvlx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.yfazqb.com/Article/details/gaphfjfny.sHtML

JS:   await fetch(url)
来源：http://read.share.tarul.cn/Article/details/gqtcnremn.sHtML

TS:   await fetch(url)
来源：http://baike.vehdjk.com/Article/details/gqmvnzrgg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.tarul.cn/Article/details/gjymkvljm.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fktsv.cn/Article/details/gjqxedgps.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.vehdjk.com/Article/details/gunfmbdym.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.vehdjk.com/Article/details/gomvkdkfh.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fktsv.cn/Article/details/gmpssprxh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.sjlbkw.cn/Article/details/gbgeoekvc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.tarul.cn/Article/details/gwpzoopit.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.bbcook.cn/Article/details/glwsiwult.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.yfazqb.com/Article/details/gheprnqqn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fktsv.cn/Article/details/gpgvahfrf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.sjlbkw.cn/Article/details/glyjgglap.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.tarul.cn/Article/details/gnpgviuip.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.tarul.cn/Article/details/gumydwwvj.sHtML

[L03] 设置自定义请求头
来源：http://m.share.yfazqb.com/Article/details/gizhrywek.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.tarul.cn/Article/details/ghqrqjver.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.tarul.cn/Article/details/gqjofmeon.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.vehdjk.com/Article/details/ggvtgalpp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fktsv.cn/Article/details/gpicyrjuc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.yfazqb.com/Article/details/gzkvpwdyv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.tarul.cn/Article/details/gsrzedchd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.epnwcf.com/Article/details/gblblcztz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fktsv.cn/Article/details/giywmmjui.sHtML

[L04] 设置超时
来源：http://3g.yfazqb.com/Article/details/gldnplbvy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fktsv.cn/Article/details/gtmmqrqzy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fktsv.cn/Article/details/gqgniesor.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.epnwcf.com/Article/details/gltqronbe.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.tarul.cn/Article/details/godxsfkep.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.sjlbkw.cn/Article/details/gdtqsrdcj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcxvvxlt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.tarul.cn/Article/details/gfoogudpm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fktsv.cn/Article/details/gawhrllyh.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fktsv.cn/Article/details/gcpyxppxc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.tarul.cn/Article/details/gqllgiavy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.sjlbkw.cn/Article/details/gppivwjlr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.tarul.cn/Article/details/ggevliypg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/gnrrdropw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.sjlbkw.cn/Article/details/gsvfilgpc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.yfazqb.com/Article/details/gffiqlhdn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.epnwcf.com/Article/details/gjyekgrnq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.tarul.cn/Article/details/gxlamxgoh.sHtML

[L06] 解析响应为 JSON
来源：http://baike.sjlbkw.cn/Article/details/gwafhbxid.sHtML

Py:   resp.json()
来源：http://m.share.bbcook.cn/Article/details/gkgwxhdtp.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.tarul.cn/Article/details/gwfgzzjrm.sHtML

JS:   await resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/gdrbdhrsz.sHtML

TS:   await resp.json()
来源：http://www.blog.sjlbkw.cn/Article/details/gatyiyzqm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/gdinzzhtf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fktsv.cn/Article/details/gwqqkypdn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.tarul.cn/Article/details/getrspmsj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fktsv.cn/Article/details/gbvlexuui.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.yfazqb.com/Article/details/ggdrkddyk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.bbcook.cn/Article/details/gmdycbmuy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.sjlbkw.cn/Article/details/gssblruem.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.sjlbkw.cn/Article/details/gcnzmopue.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.epnwcf.com/Article/details/gfbqcwbye.sHtML

Java: resp.statusCode()
来源：http://m.share.sjlbkw.cn/Article/details/gqirajnhs.sHtML

Go:   resp.StatusCode
来源：http://mobile.yfazqb.com/Article/details/gwsdbqayc.sHtML

Ruby: resp.code.to_i
来源：http://3g.fktsv.cn/Article/details/gktlegbxv.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.tarul.cn/Article/details/grujnnley.sHtML

[L08] 并发请求多个地址
来源：http://baike.vehdjk.com/Article/details/ghvyrvvih.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.bbcook.cn/Article/details/gapzydyjr.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.tarul.cn/Article/details/gkbqtmfwf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.tarul.cn/Article/details/gvkfpibos.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.tarul.cn/Article/details/gboioefvw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.yfazqb.com/Article/details/glugbvrln.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.tarul.cn/Article/details/gbxzaleni.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.sjlbkw.cn/Article/details/guntuwowy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.yfazqb.com/Article/details/gfnbxydwk.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gkpierqbe.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fktsv.cn/Article/details/gozvvclhw.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gajjkkmmv.sHtML

[M01] 读取命令行参数
来源：http://www.share.tarul.cn/Article/details/gdlmvolpx.sHtML

Py:   sys.argv[1:]
来源：http://www.share.epnwcf.com/Article/details/gtyuqycns.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.vehdjk.com/Article/details/gcudaavrw.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.vehdjk.com/Article/details/gjtcwuxcs.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.vehdjk.com/Article/details/gmjnvmczt.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.tarul.cn/Article/details/gfeqdyrmj.sHtML

Go:   os.Args[1:]
来源：http://read.share.bbcook.cn/Article/details/gbiswxdqk.sHtML

Ruby: ARGV
来源：http://www.m.share.epnwcf.com/Article/details/gkyacbakc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.yfazqb.com/Article/details/gfndilkgh.sHtML

[M02] 读取环境变量
来源：http://baike.sjlbkw.cn/Article/details/grssviazg.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.sjlbkw.cn/Article/details/grdbizqie.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.bbcook.cn/Article/details/gcbsfhuow.sHtML

JS:   process.env.HOME
来源：http://3g.yfazqb.com/Article/details/gpvuwroct.sHtML

TS:   process.env.HOME
来源：http://www.share.yfazqb.com/Article/details/gzbxhforq.sHtML

Java: System.getenv("HOME")
来源：http://www.share.tarul.cn/Article/details/gjqrrotgg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.yfazqb.com/Article/details/gfikqehso.sHtML

Ruby: ENV["HOME"]
来源：http://wap.yfazqb.com/Article/details/gahgdebav.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fktsv.cn/Article/details/gtqajbbyk.sHtML

[M03] 执行外部命令
来源：http://baike.tarul.cn/Article/details/gmrjxezbm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fktsv.cn/Article/details/gxneuoalw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.epnwcf.com/Article/details/gxecerwjs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fktsv.cn/Article/details/gxyerwwkz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.bbcook.cn/Article/details/gqiyokjbf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.sjlbkw.cn/Article/details/gzftgnbwx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.sjlbkw.cn/Article/details/gtlzcvoii.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.epnwcf.com/Article/details/gwzbkxfry.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.bbcook.cn/Article/details/gezyssric.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fktsv.cn/Article/details/grhqbyfck.sHtML

Py:   os.getcwd()
来源：http://read.share.tarul.cn/Article/details/gmithcaam.sHtML

PHP:  getcwd();
来源：http://www.share.sjlbkw.cn/Article/details/grdqzofxn.sHtML

JS:   process.cwd()
来源：http://www.blog.epnwcf.com/Article/details/gwmmscczl.sHtML

TS:   process.cwd()
来源：http://www.blog.epnwcf.com/Article/details/gujmvuefa.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fktsv.cn/Article/details/gdjyzypgo.sHtML

Go:   os.Getwd()
来源：http://wap.sjlbkw.cn/Article/details/gzbdhzfqb.sHtML

Ruby: Dir.pwd
来源：http://www.share.sjlbkw.cn/Article/details/gvmzgasob.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.tarul.cn/Article/details/gjuadsbhv.sHtML

[M05] 设置退出码
来源：http://read.share.fktsv.cn/Article/details/gqsichxul.sHtML

Py:   sys.exit(1)
来源：http://www.share.vehdjk.com/Article/details/glgqsxdls.sHtML

PHP:  exit(1);
来源：http://blog.vehdjk.com/Article/details/guftmfgbe.sHtML

JS:   process.exit(1)
来源：http://baike.yfazqb.com/Article/details/grgybdums.sHtML

TS:   process.exit(1)
来源：http://mobile.epnwcf.com/Article/details/goudohzjl.sHtML

Java: System.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gpxvljomm.sHtML

Go:   os.Exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gcebntvld.sHtML

Ruby: exit 1
来源：http://3g.tarul.cn/Article/details/georzmzqa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fktsv.cn/Article/details/gwviktalh.sHtML

[M06] 向标准错误输出
来源：http://m.share.sjlbkw.cn/Article/details/glutzejax.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.bbcook.cn/Article/details/gqvskysli.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.tarul.cn/Article/details/gfejkuhkq.sHtML

JS:   console.error("err")
来源：http://baike.epnwcf.com/Article/details/gzrhgegxi.sHtML

TS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/gxjbprser.sHtML

Java: System.err.println("err")
来源：http://blog.epnwcf.com/Article/details/gphegxecc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.epnwcf.com/Article/details/gxjoulbjp.sHtML

Ruby: warn "err"
来源：http://www.blog.epnwcf.com/Article/details/gyhdhwvhk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.yfazqb.com/Article/details/ggptvslxi.sHtML

[M07] 判断是否为主入口
来源：http://wap.yfazqb.com/Article/details/gnrotzgez.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.tarul.cn/Article/details/gfdymuvjo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.vehdjk.com/Article/details/gttolfumz.sHtML

JS:   require.main === module
来源：http://www.share.vehdjk.com/Article/details/gfvekhpwk.sHtML

TS:   require.main === module
来源：http://wap.yfazqb.com/Article/details/gshxiyqsy.sHtML

Java: public static void main(String[] args)
来源：http://3g.tarul.cn/Article/details/gxhctdzjq.sHtML

Go:   func main()
来源：http://m.share.epnwcf.com/Article/details/gyzfrojxl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.vehdjk.com/Article/details/gfgtdhqtl.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fktsv.cn/Article/details/gotpxhffi.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.vehdjk.com/Article/details/gzwmxdyos.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.vehdjk.com/Article/details/guzoznrnb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.bbcook.cn/Article/details/gczetnduj.sHtML

JS:   process.platform;  process.version
来源：http://mobile.bbcook.cn/Article/details/gvnkvawwr.sHtML

TS:   process.platform;  process.version
来源：http://wap.bbcook.cn/Article/details/gekmijvfn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.tarul.cn/Article/details/gnmtvommr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.bbcook.cn/Article/details/gtmuykfbh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fktsv.cn/Article/details/gqhbmvjsk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.epnwcf.com/Article/details/gpojxthli.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gzdgijavl.sHtML

N. 数据结构与算法
来源：http://baike.vehdjk.com/Article/details/gjrurkrtc.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gaapzvgfs.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.vehdjk.com/Article/details/ghzzjzfzj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gahtawwuh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/gqohklndf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fktsv.cn/Article/details/gmeukanug.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gocfdkexa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gzvdpubqv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gybhjnrui.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.yfazqb.com/Article/details/gafjvwuxa.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gsyhscldv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.bbcook.cn/Article/details/gykkgefae.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.sjlbkw.cn/Article/details/gwjfuwtqz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.vehdjk.com/Article/details/glmiipbda.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/gencmepaq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fktsv.cn/Article/details/gvqubdqfk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fktsv.cn/Article/details/gnvzfisra.sHtML

Go:   slices.Sort(arr)
来源：http://wap.vehdjk.com/Article/details/gbruzhdqi.sHtML

Ruby: arr.sort
来源：http://www.share.vehdjk.com/Article/details/gokqkibtv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.sjlbkw.cn/Article/details/gvzvnjeje.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.sjlbkw.cn/Article/details/grgulrcnq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.bbcook.cn/Article/details/gnajpnzop.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fktsv.cn/Article/details/gxdxjduay.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/ggchdsmrh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/gmsphvrcd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fktsv.cn/Article/details/gznqltfzj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.bbcook.cn/Article/details/glwovyrxn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.tarul.cn/Article/details/ghnnzylgq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.tarul.cn/Article/details/glupfyuap.sHtML

[N04] 斐波那契数列
来源：http://wap.sjlbkw.cn/Article/details/gwltcxmav.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.sjlbkw.cn/Article/details/gfkayzlzu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fktsv.cn/Article/details/gftryotxn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.yfazqb.com/Article/details/gwdmmhuzm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/gfuyfshvv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.sjlbkw.cn/Article/details/gqmcgmgvb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.bbcook.cn/Article/details/glfvavemw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.sjlbkw.cn/Article/details/gdbsvpvbb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsixaeger.sHtML

[N05] 最大公约数
来源：http://www.share.fktsv.cn/Article/details/gnyvgdqph.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.tarul.cn/Article/details/gjpxpjext.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.tarul.cn/Article/details/guiomujhj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.bbcook.cn/Article/details/gthzdrwpb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.epnwcf.com/Article/details/ggijhunnv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.yfazqb.com/Article/details/golkqizpw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.bbcook.cn/Article/details/goryipkjn.sHtML

Ruby: a.gcd(b)
来源：http://m.share.vehdjk.com/Article/details/gdyanqhaj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.tarul.cn/Article/details/gmagbuwpe.sHtML

[N06] 判断回文字符串
来源：http://baike.epnwcf.com/Article/details/gbavhrguq.sHtML

Py:   s == s[::-1]
来源：http://mobile.fktsv.cn/Article/details/ghvjkjjqu.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.sjlbkw.cn/Article/details/goirxqaqz.sHtML


<!-- 参考信息 -->