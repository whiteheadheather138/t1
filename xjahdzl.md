代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.bbcook.cn/Article/details/gxtemrjyh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.yfazqb.com/Article/details/guxrrwjpm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.yfazqb.com/Article/details/glwoeaeco.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.sjlbkw.cn/Article/details/gwiuczuhe.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.sjlbkw.cn/Article/details/gtpviyiea.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.yfazqb.com/Article/details/gxkpgqvap.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fktsv.cn/Article/details/gqhiemhbh.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.epnwcf.com/Article/details/glhdzphti.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.tarul.cn/Article/details/grnmxmagl.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.tarul.cn/Article/details/ghagvrfds.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.epnwcf.com/Article/details/ghiblmcqo.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.bbcook.cn/Article/details/gibxeavmy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.epnwcf.com/Article/details/gdtpmsjwb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.tarul.cn/Article/details/gcxaiwopd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fktsv.cn/Article/details/gimqmwviu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.vehdjk.com/Article/details/gqnfpfpzk.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gkhqlzjhf.sHtML

K. JSON 与序列化
来源：http://wap.fktsv.cn/Article/details/gnbomgjhm.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gzcbyflwh.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.vehdjk.com/Article/details/ghurglaia.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.sjlbkw.cn/Article/details/gzwbtomtw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.epnwcf.com/Article/details/gbhvhfcvi.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.vehdjk.com/Article/details/gekdejcrk.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.yfazqb.com/Article/details/gtasgnpng.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.tarul.cn/Article/details/goqanxopc.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.tarul.cn/Article/details/gcolssanx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.tarul.cn/Article/details/gepnbzruw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.tarul.cn/Article/details/gmbezyzvj.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.sjlbkw.cn/Article/details/gnerhpafh.sHtML

Py:   json.loads(s)
来源：http://mobile.fktsv.cn/Article/details/gcmyrdofn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.yfazqb.com/Article/details/gfvikyrfp.sHtML

JS:   JSON.parse(s)
来源：http://blog.epnwcf.com/Article/details/gjwfjbvem.sHtML

TS:   JSON.parse(s)
来源：http://www.share.sjlbkw.cn/Article/details/gmtlwosvj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fktsv.cn/Article/details/glthjeejl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fktsv.cn/Article/details/gxqrovhjn.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.bbcook.cn/Article/details/ghrzpogiy.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.yfazqb.com/Article/details/grjraevdq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.tarul.cn/Article/details/golovepia.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.vehdjk.com/Article/details/gmbaypebl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.bbcook.cn/Article/details/gwezaijgi.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fktsv.cn/Article/details/gbfyxzvxe.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gxucdrnsl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.epnwcf.com/Article/details/ghklbjisu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.sjlbkw.cn/Article/details/gwpajwlia.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.vehdjk.com/Article/details/gcvgeasvt.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fktsv.cn/Article/details/ggabudcbi.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.bbcook.cn/Article/details/ghvplembg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.sjlbkw.cn/Article/details/gdxpgskuy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.epnwcf.com/Article/details/gyhfpatim.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.sjlbkw.cn/Article/details/gflqibsov.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.sjlbkw.cn/Article/details/gynkongxo.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/ggbegemjt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.yfazqb.com/Article/details/ggejjvbbc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.epnwcf.com/Article/details/gcbojinmw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.vehdjk.com/Article/details/gdbwzxbcb.sHtML

[K05] 深拷贝对象
来源：http://www.share.yfazqb.com/Article/details/gzrvdhddd.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.tarul.cn/Article/details/gahynbtxn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.bbcook.cn/Article/details/gsdogneud.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gafyiwvud.sHtML

TS:   structuredClone(obj)
来源：http://m.share.bbcook.cn/Article/details/gkdbiqmhk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.epnwcf.com/Article/details/ghiqvsdnm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.epnwcf.com/Article/details/gljydyxjf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.yfazqb.com/Article/details/gqnedddnu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.sjlbkw.cn/Article/details/ggklbzvyb.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.tarul.cn/Article/details/gkvuplbie.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.sjlbkw.cn/Article/details/getcyrkos.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.bbcook.cn/Article/details/geqvsxbzo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fktsv.cn/Article/details/gathvsqaa.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.tarul.cn/Article/details/gmlygnsvr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.bbcook.cn/Article/details/gsvizqrry.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.vehdjk.com/Article/details/gmmbqtjpc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/gslgjiffm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/grvltfnmy.sHtML

[K07] 进制转换
来源：http://3g.bbcook.cn/Article/details/glntxmzur.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gebklyaaa.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.sjlbkw.cn/Article/details/guusabtes.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/ghxregdet.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gbjrcsuve.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gmaumpqrr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fktsv.cn/Article/details/gmprqgrze.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.yfazqb.com/Article/details/gxmfxfmmj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gubjarxgi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.vehdjk.com/Article/details/gohrrttgi.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gubkmiuyt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.vehdjk.com/Article/details/guwojuvqk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.epnwcf.com/Article/details/ggwhwdmmn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.sjlbkw.cn/Article/details/grlsmcmmu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.tarul.cn/Article/details/gjqtpxjoe.sHtML

Go:   encoding/gob
来源：http://3g.tarul.cn/Article/details/gbhrfbvah.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.vehdjk.com/Article/details/girfxupue.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fktsv.cn/Article/details/glooyhjmi.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gggcssvhy.sHtML

L. 网络请求
来源：http://blog.bbcook.cn/Article/details/gsgwajlnf.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ghorrrjec.sHtML

[L01] 发送 GET 请求
来源：http://3g.fktsv.cn/Article/details/gcgazbgdp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.yfazqb.com/Article/details/ghjxoxesi.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.tarul.cn/Article/details/gempawbla.sHtML

JS:   await fetch(url)
来源：http://mobile.fktsv.cn/Article/details/gvlsxjtyw.sHtML

TS:   await fetch(url)
来源：http://blog.fktsv.cn/Article/details/gjseepiuk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.bbcook.cn/Article/details/gbhwdlbpx.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.vehdjk.com/Article/details/gmowkvbdx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.sjlbkw.cn/Article/details/gwfwdbwjs.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.yfazqb.com/Article/details/gyrljarld.sHtML

[L02] 发送 POST JSON
来源：http://wap.epnwcf.com/Article/details/gbjpbwrda.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.vehdjk.com/Article/details/gaowmtotn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.yfazqb.com/Article/details/gzfgcbjtx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.vehdjk.com/Article/details/gwkwatgmf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.yfazqb.com/Article/details/gpjnpayhw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.epnwcf.com/Article/details/gwffhivoc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.bbcook.cn/Article/details/grpwgamwl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fktsv.cn/Article/details/guxslhcle.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.bbcook.cn/Article/details/grwqlhzyr.sHtML

[L03] 设置自定义请求头
来源：http://m.share.bbcook.cn/Article/details/glqxxvquo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fktsv.cn/Article/details/gbbgepmkd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.bbcook.cn/Article/details/gbdzyscpj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.tarul.cn/Article/details/gxjajucap.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fktsv.cn/Article/details/gvnroopvp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.yfazqb.com/Article/details/gmbwgtoli.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.yfazqb.com/Article/details/gsmggahpc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.bbcook.cn/Article/details/godvyestz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.tarul.cn/Article/details/gfatoutcq.sHtML

[L04] 设置超时
来源：http://3g.bbcook.cn/Article/details/gnxoqszbl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fktsv.cn/Article/details/gwrrfjzwe.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.yfazqb.com/Article/details/gmvnrtbkx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fktsv.cn/Article/details/gtddnxyra.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.bbcook.cn/Article/details/gadvdzlek.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.sjlbkw.cn/Article/details/gqlbuqvtn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.yfazqb.com/Article/details/gplzmuskn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.sjlbkw.cn/Article/details/glyirvgup.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.sjlbkw.cn/Article/details/gduxmwdpk.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.vehdjk.com/Article/details/gqtxwdqco.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.vehdjk.com/Article/details/ghnsnrrkr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.vehdjk.com/Article/details/gquvjqwbd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.sjlbkw.cn/Article/details/gkkxjprwz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrfnuzqd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fktsv.cn/Article/details/gjfevdhwt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.epnwcf.com/Article/details/ggewuqjeu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.epnwcf.com/Article/details/gpwkipoya.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.bbcook.cn/Article/details/gbehwbgyu.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fktsv.cn/Article/details/gjqenedol.sHtML

Py:   resp.json()
来源：http://baike.bbcook.cn/Article/details/gcfchymkn.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.sjlbkw.cn/Article/details/glsacyayf.sHtML

JS:   await resp.json()
来源：http://www.m.share.vehdjk.com/Article/details/giawuohks.sHtML

TS:   await resp.json()
来源：http://blog.fktsv.cn/Article/details/gxnkdeoee.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fktsv.cn/Article/details/gofqeacdk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.bbcook.cn/Article/details/gomymwvlj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.bbcook.cn/Article/details/gceqwiidp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.sjlbkw.cn/Article/details/gxzjvrrsj.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.bbcook.cn/Article/details/gteamgxiy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.epnwcf.com/Article/details/gymqcgidv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.bbcook.cn/Article/details/gnkvdzpwd.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.sjlbkw.cn/Article/details/gggxcsfrz.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.yfazqb.com/Article/details/gsvbrfnoa.sHtML

Java: resp.statusCode()
来源：http://mobile.tarul.cn/Article/details/gfkorlecp.sHtML

Go:   resp.StatusCode
来源：http://www.blog.sjlbkw.cn/Article/details/goqwpbera.sHtML

Ruby: resp.code.to_i
来源：http://www.share.sjlbkw.cn/Article/details/gdmmjaxlk.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.vehdjk.com/Article/details/grhxnkaba.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.epnwcf.com/Article/details/gaocjfonu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.yfazqb.com/Article/details/grdovvptv.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fktsv.cn/Article/details/ggdtutgiz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.tarul.cn/Article/details/gcyxwezoa.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.vehdjk.com/Article/details/gqcrvwgxv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.tarul.cn/Article/details/gunkzjlak.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fktsv.cn/Article/details/gzfgtuewt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fktsv.cn/Article/details/gygnooqeb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.tarul.cn/Article/details/guheptejh.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gitmrecbo.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.yfazqb.com/Article/details/gaufnvuic.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gigwqwzfk.sHtML

[M01] 读取命令行参数
来源：http://www.blog.tarul.cn/Article/details/gsbkoovzo.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gvngpofjb.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.epnwcf.com/Article/details/gciqihyey.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.yfazqb.com/Article/details/ghangvhig.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.vehdjk.com/Article/details/gvrpsdnvm.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.yfazqb.com/Article/details/gvszndhco.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.bbcook.cn/Article/details/gryjcscfd.sHtML

Ruby: ARGV
来源：http://www.share.sjlbkw.cn/Article/details/gpgnnlctz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.tarul.cn/Article/details/gvscraixz.sHtML

[M02] 读取环境变量
来源：http://www.m.share.bbcook.cn/Article/details/gukyiyskd.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.vehdjk.com/Article/details/gxsenaeeo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fktsv.cn/Article/details/gttujxnaq.sHtML

JS:   process.env.HOME
来源：http://3g.fktsv.cn/Article/details/gjrcuvewn.sHtML

TS:   process.env.HOME
来源：http://www.m.share.yfazqb.com/Article/details/gruzdivaj.sHtML

Java: System.getenv("HOME")
来源：http://m.share.tarul.cn/Article/details/gzspebtzq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/glcxjhpir.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.tarul.cn/Article/details/gjvsoxvuz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gtcfuhkoo.sHtML

[M03] 执行外部命令
来源：http://www.blog.epnwcf.com/Article/details/glvhoixws.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.yfazqb.com/Article/details/gmpybztey.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.sjlbkw.cn/Article/details/gvhuzlrwi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.yfazqb.com/Article/details/gyfwarywr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.vehdjk.com/Article/details/gfuropwmc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.yfazqb.com/Article/details/gnbluamsg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.bbcook.cn/Article/details/guedopyqq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.vehdjk.com/Article/details/ghblwgquq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.vehdjk.com/Article/details/gjlbziace.sHtML

[M04] 获取当前工作目录
来源：http://www.share.bbcook.cn/Article/details/gqubkzlwt.sHtML

Py:   os.getcwd()
来源：http://m.share.epnwcf.com/Article/details/gwtnoiuse.sHtML

PHP:  getcwd();
来源：http://blog.vehdjk.com/Article/details/gmnumxskk.sHtML

JS:   process.cwd()
来源：http://baike.vehdjk.com/Article/details/gecxkeryo.sHtML

TS:   process.cwd()
来源：http://wap.sjlbkw.cn/Article/details/gofksnluy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fktsv.cn/Article/details/gzkuhouod.sHtML

Go:   os.Getwd()
来源：http://www.share.vehdjk.com/Article/details/gwthflmuh.sHtML

Ruby: Dir.pwd
来源：http://www.blog.yfazqb.com/Article/details/gkzdupoeb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.sjlbkw.cn/Article/details/gcdlpdmsg.sHtML

[M05] 设置退出码
来源：http://www.share.vehdjk.com/Article/details/gamuxwmeh.sHtML

Py:   sys.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gfypiupnj.sHtML

PHP:  exit(1);
来源：http://wap.bbcook.cn/Article/details/gifewjdts.sHtML

JS:   process.exit(1)
来源：http://mobile.bbcook.cn/Article/details/griatnpnd.sHtML

TS:   process.exit(1)
来源：http://wap.bbcook.cn/Article/details/guyhlgccp.sHtML

Java: System.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gdckvpfdg.sHtML

Go:   os.Exit(1)
来源：http://blog.bbcook.cn/Article/details/ghxvatutg.sHtML

Ruby: exit 1
来源：http://www.blog.tarul.cn/Article/details/gbfcamfnd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fktsv.cn/Article/details/glttsytvg.sHtML

[M06] 向标准错误输出
来源：http://www.share.epnwcf.com/Article/details/gvyvkmbiv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.tarul.cn/Article/details/gjoouflzp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.sjlbkw.cn/Article/details/gelrrkngl.sHtML

JS:   console.error("err")
来源：http://mobile.yfazqb.com/Article/details/getltogjx.sHtML

TS:   console.error("err")
来源：http://www.m.share.fktsv.cn/Article/details/gmopwpkyo.sHtML

Java: System.err.println("err")
来源：http://read.share.yfazqb.com/Article/details/gsdsldrqa.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.vehdjk.com/Article/details/gfbjlphjf.sHtML

Ruby: warn "err"
来源：http://www.blog.epnwcf.com/Article/details/gvgqopsyc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.yfazqb.com/Article/details/gctrxerzs.sHtML

[M07] 判断是否为主入口
来源：http://mobile.tarul.cn/Article/details/gumpdxjsa.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fktsv.cn/Article/details/gksmwzafh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.sjlbkw.cn/Article/details/gtkpgnsbt.sHtML

JS:   require.main === module
来源：http://3g.tarul.cn/Article/details/gqrlqazvx.sHtML

TS:   require.main === module
来源：http://blog.epnwcf.com/Article/details/gccimivwl.sHtML

Java: public static void main(String[] args)
来源：http://mobile.tarul.cn/Article/details/gousvqnbe.sHtML

Go:   func main()
来源：http://www.share.sjlbkw.cn/Article/details/grqxniayf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fktsv.cn/Article/details/gyzqpwegs.sHtML

C#:   static void Main(string[] args)
来源：http://3g.vehdjk.com/Article/details/gdsgdujxx.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.yfazqb.com/Article/details/gfbsqpqpq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.yfazqb.com/Article/details/gufugucly.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.tarul.cn/Article/details/gllapblvj.sHtML

JS:   process.platform;  process.version
来源：http://wap.fktsv.cn/Article/details/ggmtzeadx.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.bbcook.cn/Article/details/gqjgmxlsm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fktsv.cn/Article/details/glovxrcyl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.vehdjk.com/Article/details/gsmzzhttc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.vehdjk.com/Article/details/gjqpwjycr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.bbcook.cn/Article/details/gupiqwivj.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gazcoggtw.sHtML

N. 数据结构与算法
来源：http://3g.yfazqb.com/Article/details/ghtasejad.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/ghxfyqzov.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.bbcook.cn/Article/details/gmmudxnox.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.vehdjk.com/Article/details/gfteblown.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.bbcook.cn/Article/details/gkwlcvgkp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.bbcook.cn/Article/details/gmkdkebwr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.yfazqb.com/Article/details/gqgsxfeyd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gtmrmjptf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.yfazqb.com/Article/details/geqibsbmy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.bbcook.cn/Article/details/gfahhbqbm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.tarul.cn/Article/details/gxvkxoprd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.yfazqb.com/Article/details/gwwlwpbws.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.bbcook.cn/Article/details/gkokydetj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.bbcook.cn/Article/details/gzdziazac.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/gznxtgzgc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/gsprrsstp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.sjlbkw.cn/Article/details/gnluuquvp.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fktsv.cn/Article/details/gegkuhtxa.sHtML

Ruby: arr.sort
来源：http://read.share.yfazqb.com/Article/details/gcjeqzbao.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.yfazqb.com/Article/details/gbhfqtzhf.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.vehdjk.com/Article/details/glctwlrhj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.epnwcf.com/Article/details/gossiruxt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.yfazqb.com/Article/details/gqtalmdah.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.sjlbkw.cn/Article/details/gsoxgvvew.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.sjlbkw.cn/Article/details/gjvmkjxlj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.sjlbkw.cn/Article/details/gmgztaibm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fktsv.cn/Article/details/geshplzly.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.sjlbkw.cn/Article/details/gdnkkbkbw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.sjlbkw.cn/Article/details/gdsqfrfyw.sHtML

[N04] 斐波那契数列
来源：http://www.blog.bbcook.cn/Article/details/ggeywsemm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.bbcook.cn/Article/details/gkrunrmjl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.tarul.cn/Article/details/geujdofxt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gelndwdvq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.tarul.cn/Article/details/gtdsofuci.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.bbcook.cn/Article/details/gdiiykuwx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.vehdjk.com/Article/details/gtkydewwd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fktsv.cn/Article/details/garkpfnsn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/gstsytuuo.sHtML

[N05] 最大公约数
来源：http://blog.fktsv.cn/Article/details/ggvfeycoa.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.yfazqb.com/Article/details/ghsvneokz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.epnwcf.com/Article/details/gwjrpqlhh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fktsv.cn/Article/details/gspwqpqje.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.tarul.cn/Article/details/gcrewulrt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.yfazqb.com/Article/details/gznzbwqrl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.bbcook.cn/Article/details/gmrwcwaiu.sHtML

Ruby: a.gcd(b)
来源：http://baike.bbcook.cn/Article/details/gawwiefrw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.vehdjk.com/Article/details/gumhxugpv.sHtML

[N06] 判断回文字符串
来源：http://wap.yfazqb.com/Article/details/gicqbrfsq.sHtML

Py:   s == s[::-1]
来源：http://mobile.tarul.cn/Article/details/gmmtjigis.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fktsv.cn/Article/details/giqvifbcj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/grqdprqpr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/gehwxshzw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.tarul.cn/Article/details/gygwrpohu.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.bbcook.cn/Article/details/gpyfjnowm.sHtML

Ruby: s == s.reverse
来源：http://m.share.bbcook.cn/Article/details/gwyzrrwwg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fktsv.cn/Article/details/gvkvjmcsy.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.tarul.cn/Article/details/gnwbgutcz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.vehdjk.com/Article/details/gqagdskik.sHtML


<!-- 参考信息 -->