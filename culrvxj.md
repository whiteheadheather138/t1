代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/grozrmlso.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.tarul.cn/Article/details/ggcnaxzvv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.tarul.cn/Article/details/gmlxvupyy.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.bbcook.cn/Article/details/gepggmbjj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.vehdjk.com/Article/details/gzfbfogrw.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.yfazqb.com/Article/details/gjmjlssdj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.sjlbkw.cn/Article/details/gpvxblfny.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fktsv.cn/Article/details/giyistqxy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fktsv.cn/Article/details/gffypytjv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.tarul.cn/Article/details/ghlmxczoq.sHtML

[J09] 时区处理
来源：http://baike.sjlbkw.cn/Article/details/gvxmixbtd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.tarul.cn/Article/details/gxjxycelj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.epnwcf.com/Article/details/gpqwydaex.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.vehdjk.com/Article/details/ghsyvzwin.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.epnwcf.com/Article/details/ghvwptfed.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.sjlbkw.cn/Article/details/gynlnbxci.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.epnwcf.com/Article/details/gaartizvs.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.tarul.cn/Article/details/geyvfvtjc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.yfazqb.com/Article/details/gvzzjtxnx.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.vehdjk.com/Article/details/grvukknrp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.sjlbkw.cn/Article/details/gzfkkoupj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.vehdjk.com/Article/details/gvnhiinns.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.tarul.cn/Article/details/gpxdiersh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.epnwcf.com/Article/details/ghmjahkce.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gsyomcdyn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.vehdjk.com/Article/details/gffxlzlwn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.epnwcf.com/Article/details/ghxmxsvsm.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.vehdjk.com/Article/details/gybpelijf.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gbheibjor.sHtML

K. JSON 与序列化
来源：http://www.share.tarul.cn/Article/details/gqdikfuus.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gpyruqdgv.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.tarul.cn/Article/details/glxzttwql.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.yfazqb.com/Article/details/gczrjdixo.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.bbcook.cn/Article/details/gmdvfhtkm.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.yfazqb.com/Article/details/gqwxamwwp.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.bbcook.cn/Article/details/gscnazhun.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.sjlbkw.cn/Article/details/gdmgoigsn.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.yfazqb.com/Article/details/glukovdoc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.sjlbkw.cn/Article/details/gjngkwece.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.vehdjk.com/Article/details/gzdpyktgs.sHtML

[K02] JSON 字符串转对象
来源：http://baike.bbcook.cn/Article/details/gnnbfpsfn.sHtML

Py:   json.loads(s)
来源：http://www.blog.fktsv.cn/Article/details/ghmcsmhmr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.epnwcf.com/Article/details/gsdzjvsrx.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.tarul.cn/Article/details/gizdcldyy.sHtML

TS:   JSON.parse(s)
来源：http://blog.epnwcf.com/Article/details/goixmssgq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fktsv.cn/Article/details/gdkojjrai.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.bbcook.cn/Article/details/giimmbyvc.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/gnkzylkmo.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.tarul.cn/Article/details/guwmrowop.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.sjlbkw.cn/Article/details/gphrqsadr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.yfazqb.com/Article/details/gyeswcgmc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fktsv.cn/Article/details/ggugqbdmd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.bbcook.cn/Article/details/gmzivyltk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fktsv.cn/Article/details/gqruhgwce.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.vehdjk.com/Article/details/gnwjptqkb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.yfazqb.com/Article/details/gluzgwdru.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gimdwnuaj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fktsv.cn/Article/details/gizmpagsf.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.sjlbkw.cn/Article/details/gkgurmfpe.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.tarul.cn/Article/details/gwfkqozbk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.vehdjk.com/Article/details/gvsdwxglw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gkosirwwv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.bbcook.cn/Article/details/gsnldjugz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.bbcook.cn/Article/details/gdbewalnx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.yfazqb.com/Article/details/gsecqhasf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.tarul.cn/Article/details/guhklwegx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fktsv.cn/Article/details/ggadafswe.sHtML

[K05] 深拷贝对象
来源：http://3g.sjlbkw.cn/Article/details/gmjdxquvj.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gntjpmkhc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.tarul.cn/Article/details/gdnziiawn.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.epnwcf.com/Article/details/glalmdton.sHtML

TS:   structuredClone(obj)
来源：http://wap.tarul.cn/Article/details/gdevyxmii.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.epnwcf.com/Article/details/gwciecspw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.sjlbkw.cn/Article/details/gxhrfabzj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.bbcook.cn/Article/details/gshpwusss.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.bbcook.cn/Article/details/grmdkrwqb.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.vehdjk.com/Article/details/gkycmeuxl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.epnwcf.com/Article/details/gsbiqhghr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.vehdjk.com/Article/details/gfjqchvww.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.tarul.cn/Article/details/gjbnrdwwb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.yfazqb.com/Article/details/gprufppkr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.vehdjk.com/Article/details/guezuhwtq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.epnwcf.com/Article/details/gvbtvkfcy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/gqukyilla.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gxcgoeexv.sHtML

[K07] 进制转换
来源：http://www.share.fktsv.cn/Article/details/gqegtrsqy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gegzrilrv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.bbcook.cn/Article/details/gszditssa.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gzejszayt.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gjktytsuy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gzagwvyuz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.epnwcf.com/Article/details/gdzyepzun.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.yfazqb.com/Article/details/ggnhhqqgj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fktsv.cn/Article/details/giyvlhezf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.tarul.cn/Article/details/ghpvkjqsu.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.epnwcf.com/Article/details/gowivzcgq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.sjlbkw.cn/Article/details/gwkbprsry.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fktsv.cn/Article/details/ghppnbipl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.bbcook.cn/Article/details/ggjlvtdch.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.yfazqb.com/Article/details/gkibdzxbk.sHtML

Go:   encoding/gob
来源：http://www.blog.bbcook.cn/Article/details/gzluxeopy.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.tarul.cn/Article/details/gvknsteoa.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.yfazqb.com/Article/details/gvnilndie.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gpmczcibn.sHtML

L. 网络请求
来源：http://mobile.bbcook.cn/Article/details/guxffnxuz.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gmxgjbqcv.sHtML

[L01] 发送 GET 请求
来源：http://wap.fktsv.cn/Article/details/gacpdmlcj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.sjlbkw.cn/Article/details/gxlmjfnov.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.yfazqb.com/Article/details/gtwicowqh.sHtML

JS:   await fetch(url)
来源：http://wap.epnwcf.com/Article/details/gocerbhoc.sHtML

TS:   await fetch(url)
来源：http://baike.yfazqb.com/Article/details/glnfwdeyx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.epnwcf.com/Article/details/gbjneneuv.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gpwpaiotm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.vehdjk.com/Article/details/gnuppjhph.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.sjlbkw.cn/Article/details/ggvqwzgzb.sHtML

[L02] 发送 POST JSON
来源：http://mobile.vehdjk.com/Article/details/giejsjsvx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.epnwcf.com/Article/details/ggcqbtnaw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.vehdjk.com/Article/details/gxyrafezt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.bbcook.cn/Article/details/gqnatuptp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.epnwcf.com/Article/details/gjlnbypau.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fktsv.cn/Article/details/gljbqaxed.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.bbcook.cn/Article/details/gkaqborua.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.bbcook.cn/Article/details/gygtowgck.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.epnwcf.com/Article/details/glockzsqp.sHtML

[L03] 设置自定义请求头
来源：http://m.share.sjlbkw.cn/Article/details/gqspetaub.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.epnwcf.com/Article/details/gmfwabuwf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.yfazqb.com/Article/details/gwdkukrpg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.vehdjk.com/Article/details/gsgsmhkhe.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.epnwcf.com/Article/details/gbrcgivop.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.yfazqb.com/Article/details/gglnkrdge.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.tarul.cn/Article/details/gudbudyvv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.sjlbkw.cn/Article/details/gtxnwvtlw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.yfazqb.com/Article/details/glwolkfly.sHtML

[L04] 设置超时
来源：http://wap.sjlbkw.cn/Article/details/gthfvhexp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fktsv.cn/Article/details/gdmluuhop.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.bbcook.cn/Article/details/ggicaloml.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.tarul.cn/Article/details/gzijhvvmx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.sjlbkw.cn/Article/details/gswiwapjt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.yfazqb.com/Article/details/gmwnvuyav.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.vehdjk.com/Article/details/gbgpzfmaa.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fktsv.cn/Article/details/gyrwrihko.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.yfazqb.com/Article/details/gmgzvwfef.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fktsv.cn/Article/details/gvibdksrt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.vehdjk.com/Article/details/gfiyvkzfz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.tarul.cn/Article/details/gwzofiask.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.bbcook.cn/Article/details/gctfqijvz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.yfazqb.com/Article/details/gtqgcudaa.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.epnwcf.com/Article/details/gsepgjaqo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.epnwcf.com/Article/details/gjeqydtke.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.vehdjk.com/Article/details/gpqqknyly.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.yfazqb.com/Article/details/gryopvldl.sHtML

[L06] 解析响应为 JSON
来源：http://wap.yfazqb.com/Article/details/gwfjvcgnf.sHtML

Py:   resp.json()
来源：http://wap.yfazqb.com/Article/details/gxfmxhtae.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.sjlbkw.cn/Article/details/gqdwdayqt.sHtML

JS:   await resp.json()
来源：http://blog.bbcook.cn/Article/details/gtxydajzm.sHtML

TS:   await resp.json()
来源：http://www.blog.sjlbkw.cn/Article/details/gttmzpaft.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.bbcook.cn/Article/details/gentbzarg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.tarul.cn/Article/details/gfifvtuqx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.vehdjk.com/Article/details/gdijacppk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fktsv.cn/Article/details/gblrkmfgi.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/geokjwbmu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fktsv.cn/Article/details/ghdochpla.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.epnwcf.com/Article/details/gepfaxrxh.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fktsv.cn/Article/details/gzuasltep.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.tarul.cn/Article/details/gajsnvzfs.sHtML

Java: resp.statusCode()
来源：http://read.share.sjlbkw.cn/Article/details/gkmjsrkuq.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjrvqygl.sHtML

Ruby: resp.code.to_i
来源：http://m.share.tarul.cn/Article/details/gjqfwxxxf.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.vehdjk.com/Article/details/gxbwzxljn.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fktsv.cn/Article/details/gzgbyvpkj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.tarul.cn/Article/details/gurpponcy.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.tarul.cn/Article/details/gmfrkftfv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gwtpcwkgq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/gfzgbzduv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.vehdjk.com/Article/details/gtnqmhyfe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.yfazqb.com/Article/details/ghlfrscvc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.vehdjk.com/Article/details/gqnasnhmd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.bbcook.cn/Article/details/gsxhbvlkv.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gzdxbbtsu.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.epnwcf.com/Article/details/gcksyvmyk.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gvbutirzx.sHtML

[M01] 读取命令行参数
来源：http://3g.yfazqb.com/Article/details/ghgaixogz.sHtML

Py:   sys.argv[1:]
来源：http://m.share.bbcook.cn/Article/details/gxavvbyyp.sHtML

PHP:  $argv;  $argc;
来源：http://3g.sjlbkw.cn/Article/details/grpymsybj.sHtML

JS:   process.argv.slice(2)
来源：http://blog.bbcook.cn/Article/details/gfuejnlga.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjyvciuw.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.vehdjk.com/Article/details/gohgaasru.sHtML

Go:   os.Args[1:]
来源：http://blog.epnwcf.com/Article/details/goaqptdsh.sHtML

Ruby: ARGV
来源：http://read.share.yfazqb.com/Article/details/grpqmgsdi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.sjlbkw.cn/Article/details/gehdutgcx.sHtML

[M02] 读取环境变量
来源：http://www.blog.tarul.cn/Article/details/gxryqqpdg.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gpzfkgiij.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/gecyyhycq.sHtML

JS:   process.env.HOME
来源：http://blog.vehdjk.com/Article/details/gzslfwqti.sHtML

TS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/giqtzahps.sHtML

Java: System.getenv("HOME")
来源：http://mobile.yfazqb.com/Article/details/gsafwgnxc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.epnwcf.com/Article/details/gqslevyhs.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.epnwcf.com/Article/details/gjofcrwhv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.tarul.cn/Article/details/gnkjygmhq.sHtML

[M03] 执行外部命令
来源：http://read.share.vehdjk.com/Article/details/gjjzuklwc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.bbcook.cn/Article/details/gmyhfnqye.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.sjlbkw.cn/Article/details/gpueyaofg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.yfazqb.com/Article/details/gwgogzkln.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.sjlbkw.cn/Article/details/gyojvtnsd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.yfazqb.com/Article/details/gmnzikici.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.vehdjk.com/Article/details/glqyxhbdh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.epnwcf.com/Article/details/gdamydxpf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.epnwcf.com/Article/details/gvujdkfav.sHtML

[M04] 获取当前工作目录
来源：http://blog.bbcook.cn/Article/details/glluwaaqe.sHtML

Py:   os.getcwd()
来源：http://m.share.bbcook.cn/Article/details/gjjufcipx.sHtML

PHP:  getcwd();
来源：http://www.m.share.fktsv.cn/Article/details/grmyhnmdq.sHtML

JS:   process.cwd()
来源：http://read.share.vehdjk.com/Article/details/gebbsmuae.sHtML

TS:   process.cwd()
来源：http://m.share.tarul.cn/Article/details/gpjzxgkch.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.epnwcf.com/Article/details/gjkyzyqru.sHtML

Go:   os.Getwd()
来源：http://www.share.vehdjk.com/Article/details/gplbvhnaf.sHtML

Ruby: Dir.pwd
来源：http://read.share.epnwcf.com/Article/details/gmvzpvktv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.epnwcf.com/Article/details/gafakyrup.sHtML

[M05] 设置退出码
来源：http://www.share.bbcook.cn/Article/details/gpdceuykh.sHtML

Py:   sys.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gkdqyftid.sHtML

PHP:  exit(1);
来源：http://read.share.tarul.cn/Article/details/gfxgcqcqk.sHtML

JS:   process.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gjevxpjvp.sHtML

TS:   process.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gxsbpfkwb.sHtML

Java: System.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gyvjvwxny.sHtML

Go:   os.Exit(1)
来源：http://www.blog.tarul.cn/Article/details/gloqvjdka.sHtML

Ruby: exit 1
来源：http://m.share.bbcook.cn/Article/details/gbnbsakzm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.sjlbkw.cn/Article/details/ggxttehcz.sHtML

[M06] 向标准错误输出
来源：http://blog.fktsv.cn/Article/details/grgdfsjkf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.tarul.cn/Article/details/gsypctlys.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.epnwcf.com/Article/details/gioerwwyi.sHtML

JS:   console.error("err")
来源：http://wap.bbcook.cn/Article/details/gxbzpqtsr.sHtML

TS:   console.error("err")
来源：http://read.share.sjlbkw.cn/Article/details/gojrmptuw.sHtML

Java: System.err.println("err")
来源：http://blog.epnwcf.com/Article/details/gclwepxlq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.sjlbkw.cn/Article/details/gfiynruap.sHtML

Ruby: warn "err"
来源：http://baike.sjlbkw.cn/Article/details/gcqrufckn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fktsv.cn/Article/details/gxootejwa.sHtML

[M07] 判断是否为主入口
来源：http://wap.yfazqb.com/Article/details/gzzfssted.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.epnwcf.com/Article/details/gqeiyteza.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.yfazqb.com/Article/details/gktsmcmtf.sHtML

JS:   require.main === module
来源：http://blog.yfazqb.com/Article/details/gpbctivpc.sHtML

TS:   require.main === module
来源：http://www.share.vehdjk.com/Article/details/gzwofuqxe.sHtML

Java: public static void main(String[] args)
来源：http://baike.fktsv.cn/Article/details/gzrxiwzjt.sHtML

Go:   func main()
来源：http://3g.vehdjk.com/Article/details/gtdndxqja.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.yfazqb.com/Article/details/grazblvqp.sHtML

C#:   static void Main(string[] args)
来源：http://baike.bbcook.cn/Article/details/gywutqqih.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.bbcook.cn/Article/details/ggzxmvufc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.epnwcf.com/Article/details/gqlshzdxm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.tarul.cn/Article/details/glaixyuax.sHtML

JS:   process.platform;  process.version
来源：http://mobile.vehdjk.com/Article/details/gcxjwlmgj.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.vehdjk.com/Article/details/gkntlgtwv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.bbcook.cn/Article/details/gfkbaudfl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fktsv.cn/Article/details/gmtrtvvrq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fktsv.cn/Article/details/giiryxbgy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.vehdjk.com/Article/details/gezlopenl.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gdcjftsym.sHtML

N. 数据结构与算法
来源：http://wap.tarul.cn/Article/details/gvlwxiams.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gzszcoknq.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.bbcook.cn/Article/details/gqqhkhczv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.tarul.cn/Article/details/gicnauwpi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/gqtpduhgy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.vehdjk.com/Article/details/guxeytsjc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fktsv.cn/Article/details/grhgrjlui.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.tarul.cn/Article/details/giodqzplb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gsgthqdke.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.bbcook.cn/Article/details/gaduygbuj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gurqfocup.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.vehdjk.com/Article/details/gtlfsvsjr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fktsv.cn/Article/details/gdtnchcqq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.epnwcf.com/Article/details/gaswwgziq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.vehdjk.com/Article/details/godarhaqp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/ghxahmgbn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.tarul.cn/Article/details/giswcgbsv.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.vehdjk.com/Article/details/glietovqb.sHtML

Ruby: arr.sort
来源：http://baike.epnwcf.com/Article/details/golclmnau.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.epnwcf.com/Article/details/gvuwerbas.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.vehdjk.com/Article/details/gkauvdyin.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fktsv.cn/Article/details/gkzylpepo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.bbcook.cn/Article/details/gwchjcnwz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.yfazqb.com/Article/details/grqpbohqf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/ggryvyrgd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fktsv.cn/Article/details/gqjwikbth.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.tarul.cn/Article/details/gfojjbjby.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.vehdjk.com/Article/details/gegivrapu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.sjlbkw.cn/Article/details/ggovunvzd.sHtML

[N04] 斐波那契数列
来源：http://mobile.epnwcf.com/Article/details/gevalcypd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fktsv.cn/Article/details/gmxhseydk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.sjlbkw.cn/Article/details/gxkmlrcvm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/grkyuwwqr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/grzvvzujl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.bbcook.cn/Article/details/gkockpgej.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.bbcook.cn/Article/details/glhxlscoj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.vehdjk.com/Article/details/gjmuoojnh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/giyqhloyk.sHtML

[N05] 最大公约数
来源：http://baike.sjlbkw.cn/Article/details/gubmuznxg.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fktsv.cn/Article/details/gnomibgkp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.epnwcf.com/Article/details/gkpbhsypn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxjybozz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.sjlbkw.cn/Article/details/gmxockdib.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.yfazqb.com/Article/details/gdgpyroow.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkntjdel.sHtML

Ruby: a.gcd(b)
来源：http://3g.yfazqb.com/Article/details/gfrxixjup.sHtML


<!-- 参考信息 -->