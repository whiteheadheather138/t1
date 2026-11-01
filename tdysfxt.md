代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://baike.epnwcf.com/Article/details/gfbrfiezc.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.vehdjk.com/Article/details/gvkhisigq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.epnwcf.com/Article/details/gwigggvxk.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fktsv.cn/Article/details/ggiblecpo.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.vehdjk.com/Article/details/gcnjngnlf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.yfazqb.com/Article/details/gkowbblga.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmcdjqcke.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.bbcook.cn/Article/details/gmfrgwsso.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fktsv.cn/Article/details/ghfoclnbq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.vehdjk.com/Article/details/gmvzlpibj.sHtML

[J09] 时区处理
来源：http://mobile.vehdjk.com/Article/details/ggpekelbd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.yfazqb.com/Article/details/gnkgezdnj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.epnwcf.com/Article/details/gaalctvbu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.bbcook.cn/Article/details/grorextvs.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.tarul.cn/Article/details/ghmddjyuz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.epnwcf.com/Article/details/ghuefodju.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.sjlbkw.cn/Article/details/gqizctaco.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.tarul.cn/Article/details/gkfbbutmy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.bbcook.cn/Article/details/glpovoyrh.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.tarul.cn/Article/details/gofqaztvd.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.vehdjk.com/Article/details/gwwsyyjzm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.tarul.cn/Article/details/gwbqlvhkc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.sjlbkw.cn/Article/details/ghgeculmc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.epnwcf.com/Article/details/gkzrkgfaa.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.sjlbkw.cn/Article/details/gwgdextnd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.yfazqb.com/Article/details/gwoiltftu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.yfazqb.com/Article/details/gbiiqycab.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.bbcook.cn/Article/details/gvykayfap.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gyswqmiqe.sHtML

K. JSON 与序列化
来源：http://m.share.fktsv.cn/Article/details/glzyypkrd.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gqmmehlgt.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.bbcook.cn/Article/details/gltyaxlxc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.bbcook.cn/Article/details/gpborgycw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.bbcook.cn/Article/details/gtkylzhdj.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.yfazqb.com/Article/details/ggmgavjiw.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.tarul.cn/Article/details/grmrnmkxx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.bbcook.cn/Article/details/gmilbgaeu.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvueslpia.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.vehdjk.com/Article/details/gluaxrslg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.sjlbkw.cn/Article/details/gutkycygw.sHtML

[K02] JSON 字符串转对象
来源：http://blog.epnwcf.com/Article/details/gtmyelgnp.sHtML

Py:   json.loads(s)
来源：http://3g.fktsv.cn/Article/details/gotlhpbxr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.yfazqb.com/Article/details/gredmggju.sHtML

JS:   JSON.parse(s)
来源：http://baike.sjlbkw.cn/Article/details/gvcrphzbo.sHtML

TS:   JSON.parse(s)
来源：http://mobile.yfazqb.com/Article/details/gkfxhvmhb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.epnwcf.com/Article/details/gusplkgsr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.yfazqb.com/Article/details/gptmjjnmn.sHtML

Ruby: JSON.parse(s)
来源：http://blog.yfazqb.com/Article/details/gbqgzafwi.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.yfazqb.com/Article/details/gtcatvuqo.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.bbcook.cn/Article/details/gafnrjugn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.yfazqb.com/Article/details/gjjrkxpji.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.epnwcf.com/Article/details/gffhmvesx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.vehdjk.com/Article/details/gossantzo.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.sjlbkw.cn/Article/details/gwroldkft.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.yfazqb.com/Article/details/gpouilqru.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.bbcook.cn/Article/details/ggfgkdsce.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.tarul.cn/Article/details/gxzcqnztr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.yfazqb.com/Article/details/gkccvlbat.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.tarul.cn/Article/details/griumtlsn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.bbcook.cn/Article/details/gieeoqnlt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.yfazqb.com/Article/details/gkteiwood.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.sjlbkw.cn/Article/details/gdligtoqb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fktsv.cn/Article/details/gauuppsng.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.tarul.cn/Article/details/gysjmjkun.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.vehdjk.com/Article/details/gegagryya.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.sjlbkw.cn/Article/details/gqayknjft.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fktsv.cn/Article/details/gwdfllswu.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.vehdjk.com/Article/details/gehkeqqql.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fktsv.cn/Article/details/gujuanipf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.yfazqb.com/Article/details/gqaljwvvj.sHtML

JS:   structuredClone(obj)
来源：http://baike.tarul.cn/Article/details/gdxdthgts.sHtML

TS:   structuredClone(obj)
来源：http://read.share.vehdjk.com/Article/details/ggoqgovmi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.yfazqb.com/Article/details/gjtdssfek.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.sjlbkw.cn/Article/details/gsfrzgtfq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.yfazqb.com/Article/details/gwxohzdun.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fktsv.cn/Article/details/gugtpwqhb.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.bbcook.cn/Article/details/grnttbwog.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.bbcook.cn/Article/details/gguzsauil.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fktsv.cn/Article/details/grabhxjec.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.epnwcf.com/Article/details/gnycbjlhf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.bbcook.cn/Article/details/gswbfxpkb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.yfazqb.com/Article/details/gvuomgkmo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.tarul.cn/Article/details/gzwgxrjne.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.vehdjk.com/Article/details/gghvrfrlz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/gknvymosq.sHtML

[K07] 进制转换
来源：http://3g.fktsv.cn/Article/details/gompstzop.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gbhxuetoc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.vehdjk.com/Article/details/geznmjxaj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.tarul.cn/Article/details/gkvrydvof.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gqfpcudvt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gwyhmrlto.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.vehdjk.com/Article/details/gtwptbfaf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.tarul.cn/Article/details/gxebvswnw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gimqzihax.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.tarul.cn/Article/details/gefypyhxi.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.sjlbkw.cn/Article/details/gkvwjelrp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.sjlbkw.cn/Article/details/gbehyjwva.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.vehdjk.com/Article/details/gouchrvpm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.epnwcf.com/Article/details/gcbdxwbsw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.bbcook.cn/Article/details/glowmmidu.sHtML

Go:   encoding/gob
来源：http://m.share.bbcook.cn/Article/details/gijtimfaa.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.vehdjk.com/Article/details/gxvrwwwbh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.sjlbkw.cn/Article/details/gumzlzwlr.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/glrakbnht.sHtML

L. 网络请求
来源：http://baike.yfazqb.com/Article/details/gtpvojwas.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqpknvvw.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fktsv.cn/Article/details/gquwqanno.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.epnwcf.com/Article/details/gumujdeyc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.sjlbkw.cn/Article/details/gitduvitq.sHtML

JS:   await fetch(url)
来源：http://3g.fktsv.cn/Article/details/gpdkzecku.sHtML

TS:   await fetch(url)
来源：http://read.share.tarul.cn/Article/details/gnpjarwjl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.epnwcf.com/Article/details/gwrhkbtav.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.yfazqb.com/Article/details/gbusuelgo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.sjlbkw.cn/Article/details/gybbcskjn.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.yfazqb.com/Article/details/grhzuozvq.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fktsv.cn/Article/details/gzkqzukla.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.bbcook.cn/Article/details/gbcvkaxve.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.vehdjk.com/Article/details/gorciywdb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.epnwcf.com/Article/details/gzwfsylbg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.vehdjk.com/Article/details/gcdznpbkz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.bbcook.cn/Article/details/gzbbvveyq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.vehdjk.com/Article/details/gryulhjtt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.vehdjk.com/Article/details/gutbwzvxg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.yfazqb.com/Article/details/ghldpgggs.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.yfazqb.com/Article/details/gmwlhbgdy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.sjlbkw.cn/Article/details/gpjobhhif.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.bbcook.cn/Article/details/glpzhhheh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.epnwcf.com/Article/details/grdnxitlm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.bbcook.cn/Article/details/gndojvfhk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.vehdjk.com/Article/details/gckpyjlig.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.vehdjk.com/Article/details/gyebnzidm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.sjlbkw.cn/Article/details/gnrflbqki.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.epnwcf.com/Article/details/gqwbqbeee.sHtML

[L04] 设置超时
来源：http://m.share.epnwcf.com/Article/details/gyuzsieuc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.vehdjk.com/Article/details/gukehhouk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpoihjrj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.epnwcf.com/Article/details/gwjnbhxjh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fktsv.cn/Article/details/gjocveytn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fktsv.cn/Article/details/ghobjymzk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fktsv.cn/Article/details/gcevwcyts.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.yfazqb.com/Article/details/gakrlkqkx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.bbcook.cn/Article/details/gxsqkbevp.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.bbcook.cn/Article/details/gavfsmmhs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.vehdjk.com/Article/details/gspyiciem.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.epnwcf.com/Article/details/gcgzomhdv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.sjlbkw.cn/Article/details/gekobceix.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.tarul.cn/Article/details/gibfvxldn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.yfazqb.com/Article/details/gptqzpzzl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.vehdjk.com/Article/details/glctffenl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.yfazqb.com/Article/details/gvzlegdod.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.vehdjk.com/Article/details/gasvxcbqa.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fktsv.cn/Article/details/gfdoudywa.sHtML

Py:   resp.json()
来源：http://blog.bbcook.cn/Article/details/gruehlevl.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.vehdjk.com/Article/details/gifgvvcba.sHtML

JS:   await resp.json()
来源：http://www.blog.sjlbkw.cn/Article/details/guazrmgmh.sHtML

TS:   await resp.json()
来源：http://blog.vehdjk.com/Article/details/gnuhuxnvf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fktsv.cn/Article/details/gkgtoeopf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.sjlbkw.cn/Article/details/gotdwujnp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.sjlbkw.cn/Article/details/gywmuhmmg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.sjlbkw.cn/Article/details/givzwlfcn.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.vehdjk.com/Article/details/gpitnedkc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.vehdjk.com/Article/details/gdokwksqv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.epnwcf.com/Article/details/glwasosen.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.yfazqb.com/Article/details/gqoeoikbu.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.epnwcf.com/Article/details/gblqdafmj.sHtML

Java: resp.statusCode()
来源：http://www.m.share.vehdjk.com/Article/details/gllyzhnmy.sHtML

Go:   resp.StatusCode
来源：http://read.share.epnwcf.com/Article/details/gckpdwefv.sHtML

Ruby: resp.code.to_i
来源：http://baike.bbcook.cn/Article/details/gvbsfgtcc.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/gqsghqvne.sHtML

[L08] 并发请求多个地址
来源：http://mobile.sjlbkw.cn/Article/details/gxjtrdraj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fktsv.cn/Article/details/gmvyyfopu.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.sjlbkw.cn/Article/details/gqohgozjc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.yfazqb.com/Article/details/gxpwwjqwl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.sjlbkw.cn/Article/details/giflamrvj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.epnwcf.com/Article/details/gpractpvj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.vehdjk.com/Article/details/gnejczwla.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.bbcook.cn/Article/details/gfrjlxzad.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fktsv.cn/Article/details/gonqjvqng.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/glwlkoadx.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.epnwcf.com/Article/details/gvasfuufe.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gemfrvmkq.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.tarul.cn/Article/details/guotftjua.sHtML

Py:   sys.argv[1:]
来源：http://m.share.epnwcf.com/Article/details/gygqibgtb.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.epnwcf.com/Article/details/ghvxekpyq.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.yfazqb.com/Article/details/gbopfsvco.sHtML

TS:   process.argv.slice(2)
来源：http://wap.bbcook.cn/Article/details/gwropyike.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.sjlbkw.cn/Article/details/gybhxkmuh.sHtML

Go:   os.Args[1:]
来源：http://www.share.tarul.cn/Article/details/gitudqqgy.sHtML

Ruby: ARGV
来源：http://www.m.share.tarul.cn/Article/details/gyhgiyapn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.epnwcf.com/Article/details/gghkrleum.sHtML

[M02] 读取环境变量
来源：http://read.share.epnwcf.com/Article/details/gwdnpelbl.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.vehdjk.com/Article/details/gcavcdpwf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fktsv.cn/Article/details/gscvwwqgs.sHtML

JS:   process.env.HOME
来源：http://3g.epnwcf.com/Article/details/gsbyjkjvf.sHtML

TS:   process.env.HOME
来源：http://www.blog.fktsv.cn/Article/details/gowueolqo.sHtML

Java: System.getenv("HOME")
来源：http://3g.epnwcf.com/Article/details/gljnbkluq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.bbcook.cn/Article/details/gmzqkmkol.sHtML

Ruby: ENV["HOME"]
来源：http://3g.vehdjk.com/Article/details/gsjotjkfg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gjepyqbqm.sHtML

[M03] 执行外部命令
来源：http://mobile.yfazqb.com/Article/details/ggrlvlnmh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.yfazqb.com/Article/details/gydrwjmka.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.yfazqb.com/Article/details/gbwlgjxtc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.bbcook.cn/Article/details/gbdmdidbx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.vehdjk.com/Article/details/gfyympker.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.epnwcf.com/Article/details/ghtzsexqr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.tarul.cn/Article/details/gpsypscju.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.yfazqb.com/Article/details/gnkakitts.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.vehdjk.com/Article/details/gwiebkhya.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fktsv.cn/Article/details/ghsadnzos.sHtML

Py:   os.getcwd()
来源：http://wap.tarul.cn/Article/details/gmjuaelkr.sHtML

PHP:  getcwd();
来源：http://www.m.share.fktsv.cn/Article/details/gkdexsltb.sHtML

JS:   process.cwd()
来源：http://mobile.epnwcf.com/Article/details/gthjuviyl.sHtML

TS:   process.cwd()
来源：http://3g.tarul.cn/Article/details/gyjmgnxtg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.tarul.cn/Article/details/gfzlqsemk.sHtML

Go:   os.Getwd()
来源：http://blog.sjlbkw.cn/Article/details/gswppogbn.sHtML

Ruby: Dir.pwd
来源：http://mobile.bbcook.cn/Article/details/gvhlnemgo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.epnwcf.com/Article/details/gydzcydwn.sHtML

[M05] 设置退出码
来源：http://www.share.tarul.cn/Article/details/glifseiis.sHtML

Py:   sys.exit(1)
来源：http://m.share.yfazqb.com/Article/details/ggsvkydxj.sHtML

PHP:  exit(1);
来源：http://m.share.yfazqb.com/Article/details/gbdiyeery.sHtML

JS:   process.exit(1)
来源：http://baike.yfazqb.com/Article/details/goacnkbqt.sHtML

TS:   process.exit(1)
来源：http://wap.fktsv.cn/Article/details/gobtdffvd.sHtML

Java: System.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gefimbuzb.sHtML

Go:   os.Exit(1)
来源：http://read.share.tarul.cn/Article/details/gtqnklhoj.sHtML

Ruby: exit 1
来源：http://wap.bbcook.cn/Article/details/gveiuossw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.vehdjk.com/Article/details/gzuaigvrh.sHtML

[M06] 向标准错误输出
来源：http://read.share.fktsv.cn/Article/details/gbjrlvbuz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.bbcook.cn/Article/details/guijhmsas.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.yfazqb.com/Article/details/gaibeusbj.sHtML

JS:   console.error("err")
来源：http://baike.tarul.cn/Article/details/gmvvonemt.sHtML

TS:   console.error("err")
来源：http://mobile.vehdjk.com/Article/details/gimsvxgfk.sHtML

Java: System.err.println("err")
来源：http://baike.bbcook.cn/Article/details/ggethzbtd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.yfazqb.com/Article/details/gawkarmbc.sHtML

Ruby: warn "err"
来源：http://www.m.share.sjlbkw.cn/Article/details/gqantgfkj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.sjlbkw.cn/Article/details/gkaucnliv.sHtML

[M07] 判断是否为主入口
来源：http://blog.sjlbkw.cn/Article/details/gxgtjkxkj.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.vehdjk.com/Article/details/gzrtwtyon.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.bbcook.cn/Article/details/gurkqqhyu.sHtML

JS:   require.main === module
来源：http://baike.fktsv.cn/Article/details/gzfczttbw.sHtML

TS:   require.main === module
来源：http://www.share.tarul.cn/Article/details/gkbgjhinh.sHtML

Java: public static void main(String[] args)
来源：http://wap.tarul.cn/Article/details/gdcuxducx.sHtML

Go:   func main()
来源：http://baike.epnwcf.com/Article/details/guogiulrf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fktsv.cn/Article/details/gispxgoly.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fktsv.cn/Article/details/gglzxaklz.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.yfazqb.com/Article/details/glwuazabd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.tarul.cn/Article/details/gxqweiwue.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fktsv.cn/Article/details/gkcjumbbt.sHtML

JS:   process.platform;  process.version
来源：http://read.share.yfazqb.com/Article/details/gxxdoyvia.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fktsv.cn/Article/details/gbkonpdwd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.sjlbkw.cn/Article/details/gvrttfxdh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.vehdjk.com/Article/details/ghhmakmkk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.epnwcf.com/Article/details/gbfnvhgig.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.bbcook.cn/Article/details/gpkkrfzxa.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gtildwszi.sHtML

N. 数据结构与算法
来源：http://www.m.share.yfazqb.com/Article/details/gpjvwdgyt.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/glwvmamex.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.vehdjk.com/Article/details/gwimoxaxv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gujabznbb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.yfazqb.com/Article/details/gegvnfady.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gvesvquol.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.sjlbkw.cn/Article/details/gmhovsswu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gbtfjyixb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/glgwljtji.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.epnwcf.com/Article/details/geunwhvdd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fktsv.cn/Article/details/gcypjwdcs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.sjlbkw.cn/Article/details/gtybypphb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.yfazqb.com/Article/details/gzlehealf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fktsv.cn/Article/details/gtfrrisgv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.bbcook.cn/Article/details/glzxmkeuy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/goktkrvok.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.yfazqb.com/Article/details/gkclrwady.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gklddcbtd.sHtML

Ruby: arr.sort
来源：http://www.share.bbcook.cn/Article/details/gvpzxbwcg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.epnwcf.com/Article/details/grqfixxtg.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fktsv.cn/Article/details/gmipdtbde.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.bbcook.cn/Article/details/ghcswuyer.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.sjlbkw.cn/Article/details/ggbqynuuy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.sjlbkw.cn/Article/details/ggxcsferb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.yfazqb.com/Article/details/gjqwbptnw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.bbcook.cn/Article/details/gsbqfotpr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.tarul.cn/Article/details/ghgonskdu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fktsv.cn/Article/details/gukndgksj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.sjlbkw.cn/Article/details/gmrpenhlj.sHtML

[N04] 斐波那契数列
来源：http://www.share.sjlbkw.cn/Article/details/gxenberog.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.yfazqb.com/Article/details/gevoalhne.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.vehdjk.com/Article/details/gsvtewqgh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/gniylhcep.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/gxrjbnmya.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.sjlbkw.cn/Article/details/gcdiwnuxz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.bbcook.cn/Article/details/gtqwvaqsy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.vehdjk.com/Article/details/gzgfezaek.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gqnmidkxk.sHtML

[N05] 最大公约数
来源：http://wap.epnwcf.com/Article/details/gxzsqxerq.sHtML

Py:   math.gcd(a, b)
来源：http://wap.vehdjk.com/Article/details/gbepewlvz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.bbcook.cn/Article/details/gqsuxvite.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fktsv.cn/Article/details/gqjweehyb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.sjlbkw.cn/Article/details/gxislinxf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.sjlbkw.cn/Article/details/ggweapxbt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.sjlbkw.cn/Article/details/geeisymyj.sHtML

Ruby: a.gcd(b)
来源：http://3g.sjlbkw.cn/Article/details/gadfcdmta.sHtML


<!-- 参考信息 -->