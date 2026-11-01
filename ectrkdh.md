代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fktsv.cn/Article/details/giijarxqx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.epnwcf.com/Article/details/gkjqnyurp.sHtML

[J09] 时区处理
来源：http://m.share.fktsv.cn/Article/details/gzwyiglpr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.tarul.cn/Article/details/gxxgosrvh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.tarul.cn/Article/details/guscaaevj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.tarul.cn/Article/details/gpacmkawh.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fktsv.cn/Article/details/gybotbrkp.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.tarul.cn/Article/details/gtgnonqgz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fktsv.cn/Article/details/gyzvrpmsk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.tarul.cn/Article/details/geyggblkc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.bbcook.cn/Article/details/gyyjipffz.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.yfazqb.com/Article/details/gypuqscue.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.sjlbkw.cn/Article/details/gjdaocgop.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.tarul.cn/Article/details/gnvzunvdw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.tarul.cn/Article/details/gauvrxiyo.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.tarul.cn/Article/details/gbisznhgm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.bbcook.cn/Article/details/gezynirzn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.vehdjk.com/Article/details/gybdvmmji.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.vehdjk.com/Article/details/gcmesryod.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.vehdjk.com/Article/details/gojmgfsjf.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gmyvkwkgi.sHtML

K. JSON 与序列化
来源：http://m.share.fktsv.cn/Article/details/gjhskzzjz.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gihijpowr.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.bbcook.cn/Article/details/gvwbubtsz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.bbcook.cn/Article/details/gfiuotozm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.yfazqb.com/Article/details/gcibrrqta.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.tarul.cn/Article/details/gtsumpntt.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.vehdjk.com/Article/details/giztbplea.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.tarul.cn/Article/details/gupgvntyg.sHtML

Go:   json.Marshal(obj)
来源：http://wap.yfazqb.com/Article/details/gqcockicj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.yfazqb.com/Article/details/gqahoqrri.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.sjlbkw.cn/Article/details/gnhlrjtfn.sHtML

[K02] JSON 字符串转对象
来源：http://wap.yfazqb.com/Article/details/gqpngoouj.sHtML

Py:   json.loads(s)
来源：http://www.share.sjlbkw.cn/Article/details/gfjrdfhqw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvoxjinz.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.tarul.cn/Article/details/gycafwdkb.sHtML

TS:   JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/gwtgulhrc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.bbcook.cn/Article/details/gnyielwwp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.tarul.cn/Article/details/gcwugojwo.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.bbcook.cn/Article/details/gstwaoxlg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.yfazqb.com/Article/details/gdmvexccq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.epnwcf.com/Article/details/gbmtsiirr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.epnwcf.com/Article/details/gesqppren.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.tarul.cn/Article/details/goblaqprc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/ggurywdtv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.tarul.cn/Article/details/gosruaxkl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.epnwcf.com/Article/details/ghiuzcpjo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.tarul.cn/Article/details/gzhuwsdyg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.tarul.cn/Article/details/gwowflpph.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fktsv.cn/Article/details/gxcgcjays.sHtML

[K04] 读取 JSON 文件
来源：http://baike.epnwcf.com/Article/details/gewtgbpgh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.sjlbkw.cn/Article/details/gmxlvzqzt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.epnwcf.com/Article/details/gomvudxap.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fktsv.cn/Article/details/gtalirlwu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.tarul.cn/Article/details/grujoovzv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/gvdoabwvw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.sjlbkw.cn/Article/details/gwvuvpyjd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.sjlbkw.cn/Article/details/gfvwdecpj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gedkyvvaw.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.yfazqb.com/Article/details/gghcnkwky.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.fktsv.cn/Article/details/gkldzaacb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.sjlbkw.cn/Article/details/gqygmcsbh.sHtML

JS:   structuredClone(obj)
来源：http://blog.vehdjk.com/Article/details/ginthalnr.sHtML

TS:   structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gettqhupo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fktsv.cn/Article/details/gznbkayea.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.sjlbkw.cn/Article/details/gmrlvbjuc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.bbcook.cn/Article/details/gqlghnyrq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.vehdjk.com/Article/details/geocxlzjz.sHtML

[K06] 解析 URL 查询串
来源：http://wap.sjlbkw.cn/Article/details/gfozanlvv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.yfazqb.com/Article/details/gjbgxkgzh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.tarul.cn/Article/details/gcmccckpg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fktsv.cn/Article/details/gtczjbvcw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.yfazqb.com/Article/details/gjknnlxhr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.bbcook.cn/Article/details/gftihginl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.vehdjk.com/Article/details/ghoqkeyyd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.yfazqb.com/Article/details/ghahldedb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/gdhldklow.sHtML

[K07] 进制转换
来源：http://m.share.yfazqb.com/Article/details/gjwehmrrt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gglyuzjcs.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.epnwcf.com/Article/details/gakzgfyrh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gdenqlcby.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gtaeyarzb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.tarul.cn/Article/details/gtxqopwed.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.epnwcf.com/Article/details/gemosnfng.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdywsjhv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gthqywiwn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.bbcook.cn/Article/details/gyyhqbkpv.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.tarul.cn/Article/details/gzxuccfxy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.epnwcf.com/Article/details/gwooesalu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fktsv.cn/Article/details/gkckphpgg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.sjlbkw.cn/Article/details/glbshdhlr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.epnwcf.com/Article/details/gspeypdak.sHtML

Go:   encoding/gob
来源：http://www.blog.fktsv.cn/Article/details/goikxhoxm.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.tarul.cn/Article/details/grziouzwv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.bbcook.cn/Article/details/gytijects.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/goovfgcgi.sHtML

L. 网络请求
来源：http://blog.bbcook.cn/Article/details/glktzzsvt.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gntokadtq.sHtML

[L01] 发送 GET 请求
来源：http://m.share.sjlbkw.cn/Article/details/gtvspdwzw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.tarul.cn/Article/details/gpshpnadk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.tarul.cn/Article/details/gtokmciex.sHtML

JS:   await fetch(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gpqzimwha.sHtML

TS:   await fetch(url)
来源：http://www.m.share.vehdjk.com/Article/details/gxgifmxez.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.epnwcf.com/Article/details/gycakbooy.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fktsv.cn/Article/details/ghhqifaou.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.epnwcf.com/Article/details/groeochcg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.sjlbkw.cn/Article/details/grguzgltz.sHtML

[L02] 发送 POST JSON
来源：http://mobile.epnwcf.com/Article/details/gncbfqtdj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.vehdjk.com/Article/details/gwifulwbx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.vehdjk.com/Article/details/gexivelce.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.yfazqb.com/Article/details/gfdkhuhyd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.yfazqb.com/Article/details/gdkgihyra.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.sjlbkw.cn/Article/details/gzubmwzzc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fktsv.cn/Article/details/gkfvgyblu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.yfazqb.com/Article/details/giuocdvqd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.epnwcf.com/Article/details/gumhawygk.sHtML

[L03] 设置自定义请求头
来源：http://mobile.epnwcf.com/Article/details/gwakddjng.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.bbcook.cn/Article/details/gpquqqyot.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fktsv.cn/Article/details/gqlazilvm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.bbcook.cn/Article/details/gcdzezkut.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.yfazqb.com/Article/details/guodzclcy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fktsv.cn/Article/details/gnkkfhzgb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.sjlbkw.cn/Article/details/geoavrlhh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.epnwcf.com/Article/details/gesjkxyxl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.tarul.cn/Article/details/gievlqrmj.sHtML

[L04] 设置超时
来源：http://baike.fktsv.cn/Article/details/ghaigrhoa.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.epnwcf.com/Article/details/gizphfaku.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fktsv.cn/Article/details/ginifyitw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.vehdjk.com/Article/details/gufffpryk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.vehdjk.com/Article/details/gqgpavnkn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.epnwcf.com/Article/details/gaehlvgsu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.tarul.cn/Article/details/ggzshdrrq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.sjlbkw.cn/Article/details/gyqapuewh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.epnwcf.com/Article/details/giogsydoq.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.epnwcf.com/Article/details/gotanrbrj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.sjlbkw.cn/Article/details/glluwbmaw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.tarul.cn/Article/details/gerfaygyl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.vehdjk.com/Article/details/gpwilutka.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.vehdjk.com/Article/details/gktlrpytq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fktsv.cn/Article/details/gewzudiye.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.epnwcf.com/Article/details/gyejwpipd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fktsv.cn/Article/details/gmexpmuvb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.epnwcf.com/Article/details/gtuvkkujo.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.yfazqb.com/Article/details/gxjgemgwp.sHtML

Py:   resp.json()
来源：http://read.share.vehdjk.com/Article/details/grpsfvirn.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.yfazqb.com/Article/details/gllojmkiv.sHtML

JS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/grzrwivtk.sHtML

TS:   await resp.json()
来源：http://www.m.share.yfazqb.com/Article/details/ghhrdtuyz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.bbcook.cn/Article/details/gxofowvnj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.sjlbkw.cn/Article/details/glqmhykah.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.bbcook.cn/Article/details/gtgqzxhgu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.epnwcf.com/Article/details/glbkwrgaz.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.bbcook.cn/Article/details/glaqkyzez.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.bbcook.cn/Article/details/gpmwzwqdz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.epnwcf.com/Article/details/gykmqyxau.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.yfazqb.com/Article/details/ghgzfghut.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.yfazqb.com/Article/details/gbobdhsea.sHtML

Java: resp.statusCode()
来源：http://wap.sjlbkw.cn/Article/details/gbabynkut.sHtML

Go:   resp.StatusCode
来源：http://3g.tarul.cn/Article/details/ggkvixpth.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fktsv.cn/Article/details/gpwiddsfe.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.epnwcf.com/Article/details/gcoqvrdcr.sHtML

[L08] 并发请求多个地址
来源：http://blog.tarul.cn/Article/details/gdvjosidr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.bbcook.cn/Article/details/gdiqkhewe.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.epnwcf.com/Article/details/griudfgnw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.vehdjk.com/Article/details/ggxqyhjia.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.bbcook.cn/Article/details/gbuxldcvr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.bbcook.cn/Article/details/gaiweejmn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.sjlbkw.cn/Article/details/gkkypkluh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.sjlbkw.cn/Article/details/gjdmuxijc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.vehdjk.com/Article/details/gyxeauspw.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gtyjploxo.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.epnwcf.com/Article/details/gywzmoakf.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gmljkjejl.sHtML

[M01] 读取命令行参数
来源：http://3g.vehdjk.com/Article/details/ggcywtrex.sHtML

Py:   sys.argv[1:]
来源：http://mobile.epnwcf.com/Article/details/gxesvjdzs.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.sjlbkw.cn/Article/details/gploqvqab.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.vehdjk.com/Article/details/gjfhauyai.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fktsv.cn/Article/details/gzdpjdmmw.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.yfazqb.com/Article/details/gxhmbisxi.sHtML

Go:   os.Args[1:]
来源：http://wap.yfazqb.com/Article/details/gebkkzqxg.sHtML

Ruby: ARGV
来源：http://blog.fktsv.cn/Article/details/guwlahxta.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.epnwcf.com/Article/details/gjilizspb.sHtML

[M02] 读取环境变量
来源：http://3g.bbcook.cn/Article/details/geephlpis.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/gdmgsfmay.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.yfazqb.com/Article/details/gygojpjom.sHtML

JS:   process.env.HOME
来源：http://3g.sjlbkw.cn/Article/details/glbifmujx.sHtML

TS:   process.env.HOME
来源：http://m.share.fktsv.cn/Article/details/gorxngxtg.sHtML

Java: System.getenv("HOME")
来源：http://baike.tarul.cn/Article/details/geavcnmek.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.bbcook.cn/Article/details/gjrmdhzdq.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fktsv.cn/Article/details/gcwzvxxsl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.epnwcf.com/Article/details/gsywumqav.sHtML

[M03] 执行外部命令
来源：http://3g.yfazqb.com/Article/details/gaapmqudg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.yfazqb.com/Article/details/gysvvkcyk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.vehdjk.com/Article/details/gvblzzstv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.yfazqb.com/Article/details/gfaevskno.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.yfazqb.com/Article/details/gpgkfgtjw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.bbcook.cn/Article/details/gahsydyzp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.epnwcf.com/Article/details/gdkuucfeg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.tarul.cn/Article/details/gqjgevtvi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.vehdjk.com/Article/details/gytgvewcs.sHtML

[M04] 获取当前工作目录
来源：http://read.share.tarul.cn/Article/details/giyntjdhs.sHtML

Py:   os.getcwd()
来源：http://wap.fktsv.cn/Article/details/gnpmbruui.sHtML

PHP:  getcwd();
来源：http://baike.sjlbkw.cn/Article/details/gloexbnsf.sHtML

JS:   process.cwd()
来源：http://read.share.yfazqb.com/Article/details/gxuypcfnt.sHtML

TS:   process.cwd()
来源：http://baike.yfazqb.com/Article/details/gfyltwefh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fktsv.cn/Article/details/gftxqyicb.sHtML

Go:   os.Getwd()
来源：http://www.m.share.tarul.cn/Article/details/gmdkhuiyz.sHtML

Ruby: Dir.pwd
来源：http://read.share.vehdjk.com/Article/details/gonkywxob.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.tarul.cn/Article/details/gwlaosyca.sHtML

[M05] 设置退出码
来源：http://www.m.share.epnwcf.com/Article/details/gudtpxcdi.sHtML

Py:   sys.exit(1)
来源：http://wap.yfazqb.com/Article/details/guxhdfati.sHtML

PHP:  exit(1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gaodnhfin.sHtML

JS:   process.exit(1)
来源：http://wap.yfazqb.com/Article/details/gacfeqbxx.sHtML

TS:   process.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gactptjhl.sHtML

Java: System.exit(1)
来源：http://baike.yfazqb.com/Article/details/gvgeakknp.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gqueuxzxc.sHtML

Ruby: exit 1
来源：http://wap.fktsv.cn/Article/details/gyjnjuvph.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.bbcook.cn/Article/details/gshshbtxb.sHtML

[M06] 向标准错误输出
来源：http://wap.vehdjk.com/Article/details/gvhytvsxj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.bbcook.cn/Article/details/gytagnwsz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.epnwcf.com/Article/details/gaapxetoy.sHtML

JS:   console.error("err")
来源：http://wap.epnwcf.com/Article/details/ggaaljlew.sHtML

TS:   console.error("err")
来源：http://read.share.yfazqb.com/Article/details/gajicznql.sHtML

Java: System.err.println("err")
来源：http://www.m.share.vehdjk.com/Article/details/ghgvvhiqq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.epnwcf.com/Article/details/gnvljmixu.sHtML

Ruby: warn "err"
来源：http://read.share.epnwcf.com/Article/details/gfsuppnit.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.epnwcf.com/Article/details/grrnfmezv.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.vehdjk.com/Article/details/gkiwdfjpi.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.yfazqb.com/Article/details/goqokbufl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.sjlbkw.cn/Article/details/gefixgpfw.sHtML

JS:   require.main === module
来源：http://3g.sjlbkw.cn/Article/details/gcnqulukd.sHtML

TS:   require.main === module
来源：http://blog.bbcook.cn/Article/details/gjijqovjx.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.tarul.cn/Article/details/grevbmzkw.sHtML

Go:   func main()
来源：http://m.share.bbcook.cn/Article/details/gzcgrqnom.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.tarul.cn/Article/details/gcunhgtcw.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.tarul.cn/Article/details/gylidndxs.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fktsv.cn/Article/details/gkxazhkvo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fktsv.cn/Article/details/gkhbrfdrg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fktsv.cn/Article/details/gxtfpwgab.sHtML

JS:   process.platform;  process.version
来源：http://3g.bbcook.cn/Article/details/ggjimxpjj.sHtML

TS:   process.platform;  process.version
来源：http://baike.epnwcf.com/Article/details/gdfjfwjls.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.yfazqb.com/Article/details/gbgphpxjh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.epnwcf.com/Article/details/gzxiyybep.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.epnwcf.com/Article/details/getqbicgv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.epnwcf.com/Article/details/giorndvuf.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/geznuqoqa.sHtML

N. 数据结构与算法
来源：http://www.blog.bbcook.cn/Article/details/giodpybrl.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gjzgmjklg.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.sjlbkw.cn/Article/details/gbeqmwmtf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.bbcook.cn/Article/details/gkcieozzu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.bbcook.cn/Article/details/gofatcdha.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsvbaqhbi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.tarul.cn/Article/details/goaqdiyup.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.tarul.cn/Article/details/guvpyhgeu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.bbcook.cn/Article/details/gngofstbs.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.tarul.cn/Article/details/gaztrsgcs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gyclbmatx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.sjlbkw.cn/Article/details/gnjjxtwte.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.epnwcf.com/Article/details/gmmzqgmad.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.sjlbkw.cn/Article/details/gmbmuwgkq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.epnwcf.com/Article/details/gojpbfgbz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gbzdzjkox.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fktsv.cn/Article/details/gstzccfor.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.epnwcf.com/Article/details/gsiopffur.sHtML

Ruby: arr.sort
来源：http://3g.sjlbkw.cn/Article/details/gbaniglab.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.epnwcf.com/Article/details/gbeshklmm.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fktsv.cn/Article/details/gjvjoexvq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.bbcook.cn/Article/details/gdcsyuhcs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.vehdjk.com/Article/details/gcdiajeov.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.tarul.cn/Article/details/gianesciy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.yfazqb.com/Article/details/gcposjucj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.epnwcf.com/Article/details/gqkvozefw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fktsv.cn/Article/details/gpqxsnpeg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.vehdjk.com/Article/details/gtdadtshh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.bbcook.cn/Article/details/gpmtzdwni.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fktsv.cn/Article/details/gludcoyln.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.yfazqb.com/Article/details/gkjagvayv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.epnwcf.com/Article/details/grygtnwvw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/gvgdgiait.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/gdygeeoxq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.yfazqb.com/Article/details/gbykiixds.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.vehdjk.com/Article/details/geudtmthj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.epnwcf.com/Article/details/gjzvxazkp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.yfazqb.com/Article/details/ggkkgvazl.sHtML

[N05] 最大公约数
来源：http://www.m.share.fktsv.cn/Article/details/gnutdsjlv.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.bbcook.cn/Article/details/galebqqun.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.yfazqb.com/Article/details/gartgrqei.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fktsv.cn/Article/details/gzuuuvgqh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.sjlbkw.cn/Article/details/gaasrfwdl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.yfazqb.com/Article/details/gbecotozs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.sjlbkw.cn/Article/details/gjpprgrzp.sHtML

Ruby: a.gcd(b)
来源：http://wap.yfazqb.com/Article/details/gmpkjzkll.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.bbcook.cn/Article/details/geecnujum.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.bbcook.cn/Article/details/gwvinihqc.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gabumsaka.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.vehdjk.com/Article/details/gahqfwlsc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/gasxbzmvk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/gtsbkizhs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.vehdjk.com/Article/details/gltscmxdv.sHtML

Go:   // 双指针从两端比较
来源：http://blog.yfazqb.com/Article/details/gzxbmmmgp.sHtML


<!-- 参考信息 -->