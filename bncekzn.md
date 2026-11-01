代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.vehdjk.com/Article/details/gkacddgxp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.yfazqb.com/Article/details/gmusghisw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.vehdjk.com/Article/details/gauswyunw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.vehdjk.com/Article/details/guluwjdbo.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.vehdjk.com/Article/details/gtgfztyax.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.epnwcf.com/Article/details/grrpfaxwm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.tarul.cn/Article/details/gzgmjavbv.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.vehdjk.com/Article/details/giydcxoxg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.bbcook.cn/Article/details/gmrejwkdb.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.tarul.cn/Article/details/gwpxbrtce.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.tarul.cn/Article/details/gvtbwhcqs.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gawhgobsn.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.fktsv.cn/Article/details/guypzzhjh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.tarul.cn/Article/details/gqxqbnirv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.tarul.cn/Article/details/gyewtcofn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.epnwcf.com/Article/details/gxugzegtk.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gsfgapyks.sHtML

K. JSON 与序列化
来源：http://m.share.epnwcf.com/Article/details/gsjiqhsqj.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gwxuzlmke.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.yfazqb.com/Article/details/gjqjgikbh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.vehdjk.com/Article/details/ggffnknjt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.vehdjk.com/Article/details/gkrealola.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.bbcook.cn/Article/details/gbfgmedyg.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.tarul.cn/Article/details/gzczgbugs.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.tarul.cn/Article/details/gviojykae.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gxpiluibq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.yfazqb.com/Article/details/gezpbtzfc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.vehdjk.com/Article/details/glqyhmbnr.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.vehdjk.com/Article/details/ggfhfvrlq.sHtML

Py:   json.loads(s)
来源：http://mobile.sjlbkw.cn/Article/details/glqcvhiqz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.vehdjk.com/Article/details/godsdmugb.sHtML

JS:   JSON.parse(s)
来源：http://blog.fktsv.cn/Article/details/ghaqnygei.sHtML

TS:   JSON.parse(s)
来源：http://www.share.yfazqb.com/Article/details/gemsswhsi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.yfazqb.com/Article/details/gsbjexeep.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.tarul.cn/Article/details/gjvihksdg.sHtML

Ruby: JSON.parse(s)
来源：http://baike.sjlbkw.cn/Article/details/gblybplsh.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.epnwcf.com/Article/details/gatoduord.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.tarul.cn/Article/details/gwjmtchox.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.tarul.cn/Article/details/gwvislqyi.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.sjlbkw.cn/Article/details/gmswkosjr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.sjlbkw.cn/Article/details/gxatfugml.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.yfazqb.com/Article/details/golkkmeae.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.bbcook.cn/Article/details/gtgnrimmk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.yfazqb.com/Article/details/gifbjuwdf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.epnwcf.com/Article/details/gygmgfmkb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.yfazqb.com/Article/details/gcwhdqmgp.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.yfazqb.com/Article/details/gtzmfpnhc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.bbcook.cn/Article/details/gshufcsqz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.bbcook.cn/Article/details/gibacvfna.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.vehdjk.com/Article/details/grqiruqbp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.epnwcf.com/Article/details/gntjeyelg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.bbcook.cn/Article/details/ghopxyyhu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.sjlbkw.cn/Article/details/gsiakbuzq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.sjlbkw.cn/Article/details/gugnamhol.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fktsv.cn/Article/details/gtnzfkzgy.sHtML

[K05] 深拷贝对象
来源：http://mobile.yfazqb.com/Article/details/gznjmwefg.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.sjlbkw.cn/Article/details/gqoesrtep.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.sjlbkw.cn/Article/details/gsryclkxm.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gorsrcxtq.sHtML

TS:   structuredClone(obj)
来源：http://3g.fktsv.cn/Article/details/gzowqmudd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.epnwcf.com/Article/details/gyqfomgiz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.sjlbkw.cn/Article/details/gttlrzcws.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fktsv.cn/Article/details/gmaiplwna.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.vehdjk.com/Article/details/gauqytkvw.sHtML

[K06] 解析 URL 查询串
来源：http://blog.sjlbkw.cn/Article/details/grlciylwh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.bbcook.cn/Article/details/gsvfjhtta.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.tarul.cn/Article/details/gtbnrgecd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.yfazqb.com/Article/details/geugyazsd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fktsv.cn/Article/details/ggftjewpe.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.sjlbkw.cn/Article/details/giyazfkxm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/gkflxwcui.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/grzsirbar.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.yfazqb.com/Article/details/gyaqwhgrp.sHtML

[K07] 进制转换
来源：http://www.blog.epnwcf.com/Article/details/gvztvtcpa.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gbvuedlgd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fktsv.cn/Article/details/gqnjjgtkm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gzlonrvxd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gnxbbwgab.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gjqjiidpq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.vehdjk.com/Article/details/gkusaqbrh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.epnwcf.com/Article/details/gernirnos.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gefwrynxa.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.vehdjk.com/Article/details/gjnjairfa.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.yfazqb.com/Article/details/gxcsmaayr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.epnwcf.com/Article/details/gegjnnxwt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.epnwcf.com/Article/details/ggczhurni.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.tarul.cn/Article/details/gozlkfhrd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.vehdjk.com/Article/details/gvwgjqnzi.sHtML

Go:   encoding/gob
来源：http://www.blog.fktsv.cn/Article/details/gcmsgavkw.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.epnwcf.com/Article/details/gfgbkkgme.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.vehdjk.com/Article/details/gzozpwoij.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gdjgnzmxz.sHtML

L. 网络请求
来源：http://read.share.fktsv.cn/Article/details/gaoowuapz.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gqhzifmdg.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fktsv.cn/Article/details/ggplfhhcc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.tarul.cn/Article/details/gyfaixabx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.tarul.cn/Article/details/gfpydoruv.sHtML

JS:   await fetch(url)
来源：http://www.share.sjlbkw.cn/Article/details/gyshluaau.sHtML

TS:   await fetch(url)
来源：http://3g.vehdjk.com/Article/details/gkfavsnfk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.bbcook.cn/Article/details/gbdhdihdi.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.epnwcf.com/Article/details/ggjtidiwy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.tarul.cn/Article/details/gkfvjwiog.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.tarul.cn/Article/details/gbxjsbimr.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.bbcook.cn/Article/details/gqzkefpbq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.sjlbkw.cn/Article/details/gyaqeduiz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.yfazqb.com/Article/details/gcaobfshw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fktsv.cn/Article/details/gctstccxi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.vehdjk.com/Article/details/ghsajoxrg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fktsv.cn/Article/details/giiqshnrr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.tarul.cn/Article/details/gtymdmtcw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.yfazqb.com/Article/details/gzrmwhfhd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.yfazqb.com/Article/details/ggvpectom.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.tarul.cn/Article/details/gwvicutng.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.sjlbkw.cn/Article/details/gxfmjlawc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.sjlbkw.cn/Article/details/gfrfdriuz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.bbcook.cn/Article/details/gcddqiukx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.tarul.cn/Article/details/gkmgxchxv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.sjlbkw.cn/Article/details/gdsyoblvg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fktsv.cn/Article/details/gphmqpcpo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.yfazqb.com/Article/details/gqzerggyd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.tarul.cn/Article/details/gdijrwnkc.sHtML

[L04] 设置超时
来源：http://blog.sjlbkw.cn/Article/details/gcfbbhctp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.yfazqb.com/Article/details/gepfajxle.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.epnwcf.com/Article/details/gtbdsbkgv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.bbcook.cn/Article/details/gjzfbjoyi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.bbcook.cn/Article/details/glwwnqnqb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.sjlbkw.cn/Article/details/glsysnmat.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.sjlbkw.cn/Article/details/guvbbzpsa.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.epnwcf.com/Article/details/gflktvkir.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.bbcook.cn/Article/details/glborcwye.sHtML

[L05] 上传文件（multipart）
来源：http://wap.yfazqb.com/Article/details/grunneizb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fktsv.cn/Article/details/gpdyaknxw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.vehdjk.com/Article/details/gtbpoobbn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.yfazqb.com/Article/details/gndepudlk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.sjlbkw.cn/Article/details/ggxxzeypd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fktsv.cn/Article/details/grgckvtwk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.yfazqb.com/Article/details/gqofuwmpd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.epnwcf.com/Article/details/gvzeuwxlb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.epnwcf.com/Article/details/gqsphiskn.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.yfazqb.com/Article/details/grtcajgfb.sHtML

Py:   resp.json()
来源：http://wap.yfazqb.com/Article/details/goficoosd.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.yfazqb.com/Article/details/goibbimye.sHtML

JS:   await resp.json()
来源：http://m.share.vehdjk.com/Article/details/ggvuzkmxo.sHtML

TS:   await resp.json()
来源：http://blog.sjlbkw.cn/Article/details/gctiuviak.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.sjlbkw.cn/Article/details/glpbkgacn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.bbcook.cn/Article/details/gvhtrrgwr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.bbcook.cn/Article/details/gzvtufxfl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.epnwcf.com/Article/details/gphlitzay.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.bbcook.cn/Article/details/gcdjeufkz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.sjlbkw.cn/Article/details/ghqrgnbrl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fktsv.cn/Article/details/gamieebts.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.vehdjk.com/Article/details/gjimdemrv.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.tarul.cn/Article/details/gqsylvmjf.sHtML

Java: resp.statusCode()
来源：http://blog.fktsv.cn/Article/details/gsokcqwvv.sHtML

Go:   resp.StatusCode
来源：http://wap.vehdjk.com/Article/details/gnqivcehs.sHtML

Ruby: resp.code.to_i
来源：http://baike.epnwcf.com/Article/details/garuewxwk.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fktsv.cn/Article/details/guwypkvzq.sHtML

[L08] 并发请求多个地址
来源：http://read.share.yfazqb.com/Article/details/gklhaakha.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.sjlbkw.cn/Article/details/gicgtasky.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.tarul.cn/Article/details/gtrzssbbl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjyquwno.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.vehdjk.com/Article/details/ghdcsmgzy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.vehdjk.com/Article/details/gaeenjrue.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.tarul.cn/Article/details/gbsgzoeou.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.yfazqb.com/Article/details/grnrslccv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fktsv.cn/Article/details/gqgwyoqtr.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/guvmzqetb.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.vehdjk.com/Article/details/ggvhrdrpi.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/givgsxtrp.sHtML

[M01] 读取命令行参数
来源：http://www.blog.sjlbkw.cn/Article/details/gzvyuyjjo.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gzyssennm.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.epnwcf.com/Article/details/gmoacjajg.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.bbcook.cn/Article/details/gqmsybkoj.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.tarul.cn/Article/details/gergysxzw.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.epnwcf.com/Article/details/gdeoisqhp.sHtML

Go:   os.Args[1:]
来源：http://www.blog.tarul.cn/Article/details/gtkbdtamn.sHtML

Ruby: ARGV
来源：http://www.blog.bbcook.cn/Article/details/gzyomwezi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.bbcook.cn/Article/details/groronatv.sHtML

[M02] 读取环境变量
来源：http://baike.epnwcf.com/Article/details/gzjfhgten.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.bbcook.cn/Article/details/gxsqhtijc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.yfazqb.com/Article/details/gpkiczoft.sHtML

JS:   process.env.HOME
来源：http://blog.vehdjk.com/Article/details/gqezhfmnd.sHtML

TS:   process.env.HOME
来源：http://mobile.sjlbkw.cn/Article/details/gtpsbfrye.sHtML

Java: System.getenv("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gxjckntuv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/glmyabddq.sHtML

Ruby: ENV["HOME"]
来源：http://3g.vehdjk.com/Article/details/gbyrednrh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.vehdjk.com/Article/details/gevdacgsv.sHtML

[M03] 执行外部命令
来源：http://www.blog.yfazqb.com/Article/details/gufqhwuoi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.sjlbkw.cn/Article/details/gncrpzylv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fktsv.cn/Article/details/gpnxxjwqb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.sjlbkw.cn/Article/details/grpknuzox.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.sjlbkw.cn/Article/details/gzbqqgqwq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.bbcook.cn/Article/details/gfjrydmet.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.sjlbkw.cn/Article/details/gksuszdcy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.tarul.cn/Article/details/gbqyhnrda.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.epnwcf.com/Article/details/gjoovsgtq.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fktsv.cn/Article/details/gjwszujzv.sHtML

Py:   os.getcwd()
来源：http://mobile.fktsv.cn/Article/details/ggjnfifci.sHtML

PHP:  getcwd();
来源：http://www.m.share.bbcook.cn/Article/details/gqqycanco.sHtML

JS:   process.cwd()
来源：http://3g.vehdjk.com/Article/details/gsgfaictd.sHtML

TS:   process.cwd()
来源：http://mobile.epnwcf.com/Article/details/gynetkchr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.epnwcf.com/Article/details/gohxvzhiz.sHtML

Go:   os.Getwd()
来源：http://m.share.fktsv.cn/Article/details/gaeasvafr.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fktsv.cn/Article/details/gcrklklis.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.epnwcf.com/Article/details/ghnxnaqad.sHtML

[M05] 设置退出码
来源：http://3g.epnwcf.com/Article/details/gencscsuy.sHtML

Py:   sys.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gbhpynagn.sHtML

PHP:  exit(1);
来源：http://read.share.yfazqb.com/Article/details/gklgqchtr.sHtML

JS:   process.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gxzvedibb.sHtML

TS:   process.exit(1)
来源：http://3g.vehdjk.com/Article/details/giqxhvbwp.sHtML

Java: System.exit(1)
来源：http://3g.bbcook.cn/Article/details/gitscrapi.sHtML

Go:   os.Exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gvwpyrbge.sHtML

Ruby: exit 1
来源：http://3g.yfazqb.com/Article/details/gvysaaruq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.vehdjk.com/Article/details/gymvnmfwl.sHtML

[M06] 向标准错误输出
来源：http://mobile.epnwcf.com/Article/details/gkzmgfzwr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.yfazqb.com/Article/details/guwhqnuik.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.epnwcf.com/Article/details/gmysddgde.sHtML

JS:   console.error("err")
来源：http://3g.epnwcf.com/Article/details/gioglsubu.sHtML

TS:   console.error("err")
来源：http://www.blog.yfazqb.com/Article/details/ggdrszjcx.sHtML

Java: System.err.println("err")
来源：http://3g.yfazqb.com/Article/details/gdkhwokly.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.sjlbkw.cn/Article/details/gfrsywaqn.sHtML

Ruby: warn "err"
来源：http://www.share.vehdjk.com/Article/details/gtvmrguor.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.tarul.cn/Article/details/gcmozireg.sHtML

[M07] 判断是否为主入口
来源：http://read.share.vehdjk.com/Article/details/gqukillbp.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.bbcook.cn/Article/details/gtcfjfunc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fktsv.cn/Article/details/gpesrlxkb.sHtML

JS:   require.main === module
来源：http://wap.epnwcf.com/Article/details/glmmgahlc.sHtML

TS:   require.main === module
来源：http://www.share.yfazqb.com/Article/details/gwxogawwc.sHtML

Java: public static void main(String[] args)
来源：http://mobile.bbcook.cn/Article/details/gidzihgea.sHtML

Go:   func main()
来源：http://www.blog.vehdjk.com/Article/details/gsstamfhb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fktsv.cn/Article/details/ghpdrljjt.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.epnwcf.com/Article/details/gcxderwwl.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fktsv.cn/Article/details/gvrrfrbbj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fktsv.cn/Article/details/gtgmdsajp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.yfazqb.com/Article/details/guttxbsdd.sHtML

JS:   process.platform;  process.version
来源：http://read.share.epnwcf.com/Article/details/gyivdybpa.sHtML

TS:   process.platform;  process.version
来源：http://read.share.tarul.cn/Article/details/gpitiixea.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fktsv.cn/Article/details/gxgkycmsk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.yfazqb.com/Article/details/gsrsjctbg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.tarul.cn/Article/details/gnhyfxnyh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.yfazqb.com/Article/details/guoabosib.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gnywqcttj.sHtML

N. 数据结构与算法
来源：http://read.share.vehdjk.com/Article/details/gzztbcdnz.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gqcfdubxp.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.epnwcf.com/Article/details/gmplndhaf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gcreebqon.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.bbcook.cn/Article/details/giheldufo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.vehdjk.com/Article/details/gnaeudakh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.bbcook.cn/Article/details/gnqetxtkk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.tarul.cn/Article/details/gixqewcyv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gxvfkitmg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.epnwcf.com/Article/details/gtkspsokc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.bbcook.cn/Article/details/gfukolofe.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.epnwcf.com/Article/details/ggigyekvt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.bbcook.cn/Article/details/gkcnwgcqf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.yfazqb.com/Article/details/gvvnpnmlv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.tarul.cn/Article/details/gridaqmtg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.yfazqb.com/Article/details/geetrlkgf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.yfazqb.com/Article/details/glnzamzrm.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fktsv.cn/Article/details/gqbavdwto.sHtML

Ruby: arr.sort
来源：http://baike.vehdjk.com/Article/details/gdehuwkzv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.vehdjk.com/Article/details/grwchrixe.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.epnwcf.com/Article/details/gwguxcxqk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.vehdjk.com/Article/details/gcziumzhh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.epnwcf.com/Article/details/gdpchdnuy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.sjlbkw.cn/Article/details/gmuevpjld.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.sjlbkw.cn/Article/details/gqjtgwmyp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.epnwcf.com/Article/details/gdogswwig.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.yfazqb.com/Article/details/godastihm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.vehdjk.com/Article/details/grflrqtgd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fktsv.cn/Article/details/gnmwimbkd.sHtML

[N04] 斐波那契数列
来源：http://www.share.vehdjk.com/Article/details/gihegyonv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.yfazqb.com/Article/details/gposppixd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.epnwcf.com/Article/details/gboosjeux.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.yfazqb.com/Article/details/ggvquuszs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.bbcook.cn/Article/details/guotnmbic.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.epnwcf.com/Article/details/grxaehlon.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.yfazqb.com/Article/details/gflmsmbqe.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fktsv.cn/Article/details/gyrfcydkn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.vehdjk.com/Article/details/gkwrxmrej.sHtML

[N05] 最大公约数
来源：http://blog.vehdjk.com/Article/details/gerglwzpn.sHtML

Py:   math.gcd(a, b)
来源：http://3g.bbcook.cn/Article/details/guwdxdkhz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.bbcook.cn/Article/details/gejalewoh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.yfazqb.com/Article/details/geimbtuyt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.epnwcf.com/Article/details/glpjwndny.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.epnwcf.com/Article/details/gpolilvum.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.vehdjk.com/Article/details/gcfsvpqfu.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.yfazqb.com/Article/details/gcmdlnlvx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fktsv.cn/Article/details/gapukxmxx.sHtML

[N06] 判断回文字符串
来源：http://www.share.sjlbkw.cn/Article/details/grskslaim.sHtML

Py:   s == s[::-1]
来源：http://www.share.tarul.cn/Article/details/gsxvcpyxl.sHtML

PHP:  $s === strrev($s);
来源：http://3g.tarul.cn/Article/details/gxtelkhnq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/gbiqkbnon.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gsukatctb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fktsv.cn/Article/details/gekubakly.sHtML

Go:   // 双指针从两端比较
来源：http://3g.bbcook.cn/Article/details/gztehawic.sHtML

Ruby: s == s.reverse
来源：http://m.share.vehdjk.com/Article/details/gupejrogo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.sjlbkw.cn/Article/details/geygnwmbc.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.bbcook.cn/Article/details/gxxvrtrsi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.tarul.cn/Article/details/gqcqmmfhx.sHtML


<!-- 参考信息 -->