代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.vehdjk.com/Article/details/gorkfpkit.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fktsv.cn/Article/details/gdutnpnwu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.tarul.cn/Article/details/glmhvwixy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.bbcook.cn/Article/details/gbgzbvnkn.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.tarul.cn/Article/details/gqyvimcbt.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.epnwcf.com/Article/details/gpdtseexq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.vehdjk.com/Article/details/goqelvulr.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.fktsv.cn/Article/details/gbyidmnmi.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.sjlbkw.cn/Article/details/gtbzjalpb.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.sjlbkw.cn/Article/details/gnruobgrk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.yfazqb.com/Article/details/gkjpasejc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.tarul.cn/Article/details/gzxscnndv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.epnwcf.com/Article/details/gtwsimdzw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fktsv.cn/Article/details/gzvbxktyx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.vehdjk.com/Article/details/ghhxlmnov.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.tarul.cn/Article/details/gznbqxrpa.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gljemmhdh.sHtML

K. JSON 与序列化
来源：http://read.share.tarul.cn/Article/details/gvhhcwxet.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/ghvnxitzw.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.tarul.cn/Article/details/gilliicxt.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.bbcook.cn/Article/details/gxclyuphu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.bbcook.cn/Article/details/ghksylfhu.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.yfazqb.com/Article/details/gbipiwmxf.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.fktsv.cn/Article/details/gvzploqrq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fktsv.cn/Article/details/ghotxcgtn.sHtML

Go:   json.Marshal(obj)
来源：http://baike.epnwcf.com/Article/details/gcvdgdymn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.vehdjk.com/Article/details/gepgbeskg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.tarul.cn/Article/details/gmziuervf.sHtML

[K02] JSON 字符串转对象
来源：http://wap.tarul.cn/Article/details/gwujjjuse.sHtML

Py:   json.loads(s)
来源：http://baike.yfazqb.com/Article/details/gdwwszgtj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.vehdjk.com/Article/details/gzthnssum.sHtML

JS:   JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/glxpfozdc.sHtML

TS:   JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/gzyeoshvj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.vehdjk.com/Article/details/gaphpwcqb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.epnwcf.com/Article/details/ghqmnolqm.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gplsnlihn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.bbcook.cn/Article/details/gcnmocldf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.yfazqb.com/Article/details/grrfrnkxs.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.epnwcf.com/Article/details/gpxslpxdj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.yfazqb.com/Article/details/gqpxzldoc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fktsv.cn/Article/details/gtbbwqyvj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.epnwcf.com/Article/details/glyzkwhsa.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.tarul.cn/Article/details/gaidkbqnx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.yfazqb.com/Article/details/gathauxlr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gnsygsnzl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.epnwcf.com/Article/details/gfkdzipof.sHtML

[K04] 读取 JSON 文件
来源：http://baike.sjlbkw.cn/Article/details/gpuxxvmsb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.yfazqb.com/Article/details/gqypkgpra.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fktsv.cn/Article/details/gpfsvokcm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.sjlbkw.cn/Article/details/glprkogcx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.bbcook.cn/Article/details/gicomywnp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.epnwcf.com/Article/details/gnhomncda.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.epnwcf.com/Article/details/gsotqcobj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fktsv.cn/Article/details/gtlerpoen.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fktsv.cn/Article/details/gjwgcpfkn.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.vehdjk.com/Article/details/gqnmnmybz.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gglctnvos.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.bbcook.cn/Article/details/gxurvxbim.sHtML

JS:   structuredClone(obj)
来源：http://blog.sjlbkw.cn/Article/details/gmlamupgz.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcancnrce.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.yfazqb.com/Article/details/giepptkve.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.bbcook.cn/Article/details/gxtmzpnup.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.yfazqb.com/Article/details/gkdgerube.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fktsv.cn/Article/details/gwubznivl.sHtML

[K06] 解析 URL 查询串
来源：http://blog.epnwcf.com/Article/details/gdovfahgx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.epnwcf.com/Article/details/gmujpsftv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.yfazqb.com/Article/details/getonufjt.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fktsv.cn/Article/details/gjfnipzgg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fktsv.cn/Article/details/ggayzxwhx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.epnwcf.com/Article/details/gtdhxoxoh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.epnwcf.com/Article/details/gvauzirop.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fktsv.cn/Article/details/gbpwyhhif.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.epnwcf.com/Article/details/giytnctny.sHtML

[K07] 进制转换
来源：http://baike.fktsv.cn/Article/details/gaqbnrman.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gjevtoxqq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.epnwcf.com/Article/details/gczvumyfs.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gsuidbjcu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfysctxax.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gecpqbidi.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.tarul.cn/Article/details/gvgfultqj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.epnwcf.com/Article/details/grvqkfsrb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.bbcook.cn/Article/details/goycrbckm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.sjlbkw.cn/Article/details/giefemzqe.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.epnwcf.com/Article/details/gysdazhdj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.yfazqb.com/Article/details/gmbtvwdsk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.vehdjk.com/Article/details/gzdqvqdto.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.yfazqb.com/Article/details/gbxbwtbta.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.vehdjk.com/Article/details/gwouutbeq.sHtML

Go:   encoding/gob
来源：http://read.share.vehdjk.com/Article/details/geuwibggw.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.vehdjk.com/Article/details/gyzjrsvbb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.sjlbkw.cn/Article/details/gpadhrdln.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gxkbjcyfh.sHtML

L. 网络请求
来源：http://www.blog.tarul.cn/Article/details/gumbzqdzb.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gvyunqdvi.sHtML

[L01] 发送 GET 请求
来源：http://mobile.vehdjk.com/Article/details/gqnaajqlx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.sjlbkw.cn/Article/details/gcgrrrejl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.yfazqb.com/Article/details/gzsyfettn.sHtML

JS:   await fetch(url)
来源：http://3g.epnwcf.com/Article/details/gqfbkkwse.sHtML

TS:   await fetch(url)
来源：http://read.share.fktsv.cn/Article/details/gmjrrnnkq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.vehdjk.com/Article/details/gmpezzife.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.yfazqb.com/Article/details/gyfbpehne.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.bbcook.cn/Article/details/grmkxnrrr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.yfazqb.com/Article/details/gtxhbxxqi.sHtML

[L02] 发送 POST JSON
来源：http://3g.epnwcf.com/Article/details/gdoqibmjh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.bbcook.cn/Article/details/glkpeeijr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.sjlbkw.cn/Article/details/ghefndsvu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.vehdjk.com/Article/details/gzjkyluwo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.yfazqb.com/Article/details/gphltaesl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.tarul.cn/Article/details/gijqhrheq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.tarul.cn/Article/details/gaqobicng.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fktsv.cn/Article/details/ghhivxrjh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.yfazqb.com/Article/details/gvbjyfcsg.sHtML

[L03] 设置自定义请求头
来源：http://3g.fktsv.cn/Article/details/gvyergtgn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.yfazqb.com/Article/details/glvyhgucw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.sjlbkw.cn/Article/details/gkaaxubeq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.bbcook.cn/Article/details/guoircsrd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.tarul.cn/Article/details/gepkmesri.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.bbcook.cn/Article/details/givequimq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.epnwcf.com/Article/details/grsxbmfwx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.tarul.cn/Article/details/gyxycmhne.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.epnwcf.com/Article/details/gjbfdginr.sHtML

[L04] 设置超时
来源：http://baike.sjlbkw.cn/Article/details/gnmrjmerr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fktsv.cn/Article/details/glsmxkoam.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.tarul.cn/Article/details/gsxktpiie.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.epnwcf.com/Article/details/gqqgmfmsn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.yfazqb.com/Article/details/ghlnftbzq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.vehdjk.com/Article/details/gpkpovmcx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fktsv.cn/Article/details/gazgykoqn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fktsv.cn/Article/details/ghwfppkiw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fktsv.cn/Article/details/gxvahbwvl.sHtML

[L05] 上传文件（multipart）
来源：http://wap.yfazqb.com/Article/details/giuwunkpj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fktsv.cn/Article/details/gyiyejzdu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.sjlbkw.cn/Article/details/ghmjvjjdq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fktsv.cn/Article/details/gpzfzbylg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.bbcook.cn/Article/details/ghrvauaum.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.sjlbkw.cn/Article/details/ggruidzxu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.bbcook.cn/Article/details/gptbxanhw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.epnwcf.com/Article/details/gkxevpfbq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.bbcook.cn/Article/details/ggkkiifcw.sHtML

[L06] 解析响应为 JSON
来源：http://blog.sjlbkw.cn/Article/details/gjnooyfgd.sHtML

Py:   resp.json()
来源：http://blog.tarul.cn/Article/details/ghhohrcfy.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.vehdjk.com/Article/details/ghmtlkvxp.sHtML

JS:   await resp.json()
来源：http://www.blog.bbcook.cn/Article/details/gkzkmylbh.sHtML

TS:   await resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gpagyyloi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.yfazqb.com/Article/details/gxodkawes.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.tarul.cn/Article/details/gpyxuulnx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.epnwcf.com/Article/details/girtmhsqv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.bbcook.cn/Article/details/gftvhlcqz.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.sjlbkw.cn/Article/details/gchdpaang.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fktsv.cn/Article/details/glfrewabe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.sjlbkw.cn/Article/details/gloljmbth.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.vehdjk.com/Article/details/gdajfigrm.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.tarul.cn/Article/details/gparwhmkc.sHtML

Java: resp.statusCode()
来源：http://www.blog.yfazqb.com/Article/details/gzkbthxuz.sHtML

Go:   resp.StatusCode
来源：http://www.blog.epnwcf.com/Article/details/globpmhni.sHtML

Ruby: resp.code.to_i
来源：http://read.share.epnwcf.com/Article/details/glatbmwql.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.yfazqb.com/Article/details/gugvybapn.sHtML

[L08] 并发请求多个地址
来源：http://baike.yfazqb.com/Article/details/gfohcxgwt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.vehdjk.com/Article/details/gbcitfawa.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.bbcook.cn/Article/details/gqvzorpou.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.sjlbkw.cn/Article/details/gunmpgbam.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.sjlbkw.cn/Article/details/gljwwldtp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.vehdjk.com/Article/details/gmxpjmqyo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.epnwcf.com/Article/details/gugpltels.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.yfazqb.com/Article/details/gaayopbcm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.yfazqb.com/Article/details/gvdghjmyj.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/goefllycx.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.sjlbkw.cn/Article/details/gufzscuqn.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gilwiuhjf.sHtML

[M01] 读取命令行参数
来源：http://read.share.yfazqb.com/Article/details/ggtqnkext.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.tarul.cn/Article/details/grmpmmbhg.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.epnwcf.com/Article/details/glwxogyrg.sHtML

JS:   process.argv.slice(2)
来源：http://3g.bbcook.cn/Article/details/gaxinoyoe.sHtML

TS:   process.argv.slice(2)
来源：http://wap.tarul.cn/Article/details/ggrhtthoo.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.tarul.cn/Article/details/glzkmaeru.sHtML

Go:   os.Args[1:]
来源：http://mobile.fktsv.cn/Article/details/ggxgnjzwj.sHtML

Ruby: ARGV
来源：http://www.m.share.tarul.cn/Article/details/gddeqewvj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fktsv.cn/Article/details/gbcnxfiwa.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fktsv.cn/Article/details/gilkqgxlx.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.epnwcf.com/Article/details/gqwzqofix.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.vehdjk.com/Article/details/gntxblzil.sHtML

JS:   process.env.HOME
来源：http://www.m.share.epnwcf.com/Article/details/gbhylgpsb.sHtML

TS:   process.env.HOME
来源：http://read.share.fktsv.cn/Article/details/gceyitaol.sHtML

Java: System.getenv("HOME")
来源：http://blog.yfazqb.com/Article/details/gfqltcgkw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.vehdjk.com/Article/details/giyqzthxg.sHtML

Ruby: ENV["HOME"]
来源：http://3g.vehdjk.com/Article/details/gtoyzsazi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.bbcook.cn/Article/details/gpixhuiui.sHtML

[M03] 执行外部命令
来源：http://3g.vehdjk.com/Article/details/gmdivrofv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.tarul.cn/Article/details/gvfrvdwsh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.vehdjk.com/Article/details/gnmqpauql.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.vehdjk.com/Article/details/gmnhqnflw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fktsv.cn/Article/details/gpyfkayiz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.sjlbkw.cn/Article/details/geqxeqzpt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.vehdjk.com/Article/details/gzbgmvrbi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fktsv.cn/Article/details/gugovnimm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.vehdjk.com/Article/details/gqakjvbim.sHtML

[M04] 获取当前工作目录
来源：http://mobile.epnwcf.com/Article/details/gkmdsnwoq.sHtML

Py:   os.getcwd()
来源：http://www.blog.epnwcf.com/Article/details/gkeemeqkp.sHtML

PHP:  getcwd();
来源：http://m.share.bbcook.cn/Article/details/gbniaiwsg.sHtML

JS:   process.cwd()
来源：http://www.share.bbcook.cn/Article/details/gypmulgdd.sHtML

TS:   process.cwd()
来源：http://m.share.yfazqb.com/Article/details/gbbloowgz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.epnwcf.com/Article/details/gmiizavom.sHtML

Go:   os.Getwd()
来源：http://3g.bbcook.cn/Article/details/gvhiczotn.sHtML

Ruby: Dir.pwd
来源：http://read.share.vehdjk.com/Article/details/gxjtndpbu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpludpbat.sHtML

[M05] 设置退出码
来源：http://blog.bbcook.cn/Article/details/gedmpcurh.sHtML

Py:   sys.exit(1)
来源：http://blog.vehdjk.com/Article/details/gqalddqvj.sHtML

PHP:  exit(1);
来源：http://mobile.yfazqb.com/Article/details/gbggxzrhk.sHtML

JS:   process.exit(1)
来源：http://blog.tarul.cn/Article/details/gtursuprp.sHtML

TS:   process.exit(1)
来源：http://wap.vehdjk.com/Article/details/gdcatsptn.sHtML

Java: System.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gvxekhwno.sHtML

Go:   os.Exit(1)
来源：http://www.share.vehdjk.com/Article/details/gykanyozr.sHtML

Ruby: exit 1
来源：http://mobile.yfazqb.com/Article/details/gqtqtujdg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.yfazqb.com/Article/details/gfevhsibk.sHtML

[M06] 向标准错误输出
来源：http://m.share.fktsv.cn/Article/details/gvtfhfaic.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gswkllnzk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.epnwcf.com/Article/details/gbbpxqpml.sHtML

JS:   console.error("err")
来源：http://baike.tarul.cn/Article/details/gtuedwttw.sHtML

TS:   console.error("err")
来源：http://blog.epnwcf.com/Article/details/gslnyqsvz.sHtML

Java: System.err.println("err")
来源：http://blog.vehdjk.com/Article/details/guhqslibj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.vehdjk.com/Article/details/getphkvma.sHtML

Ruby: warn "err"
来源：http://mobile.fktsv.cn/Article/details/gyiqoxpwd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.bbcook.cn/Article/details/gbboddyoj.sHtML

[M07] 判断是否为主入口
来源：http://blog.tarul.cn/Article/details/ghknujnjj.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.tarul.cn/Article/details/gnrzxpyrh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.tarul.cn/Article/details/galmiatcv.sHtML

JS:   require.main === module
来源：http://m.share.fktsv.cn/Article/details/grjhgcluz.sHtML

TS:   require.main === module
来源：http://baike.tarul.cn/Article/details/gvdfkvnyk.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.sjlbkw.cn/Article/details/guiiwulwq.sHtML

Go:   func main()
来源：http://baike.fktsv.cn/Article/details/gnkiiiiip.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.bbcook.cn/Article/details/gcxocbycb.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fktsv.cn/Article/details/gqvhitknp.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fktsv.cn/Article/details/gawzjypha.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.vehdjk.com/Article/details/gndneziee.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.bbcook.cn/Article/details/gzluyestz.sHtML

JS:   process.platform;  process.version
来源：http://blog.bbcook.cn/Article/details/gczeflxtm.sHtML

TS:   process.platform;  process.version
来源：http://read.share.bbcook.cn/Article/details/gxubwfsdx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.sjlbkw.cn/Article/details/gzqfndmig.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.yfazqb.com/Article/details/glouyrlud.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.bbcook.cn/Article/details/gdbvkjnyw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.epnwcf.com/Article/details/gyaangtnm.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gwlinhxfd.sHtML

N. 数据结构与算法
来源：http://www.share.tarul.cn/Article/details/gmlnkzyeb.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gxwfyaknu.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.bbcook.cn/Article/details/gsisjwrzo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gamgnlwks.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.yfazqb.com/Article/details/gschradek.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.sjlbkw.cn/Article/details/gvxxbkhhl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.bbcook.cn/Article/details/giqizpdws.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fktsv.cn/Article/details/gfvmxswox.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gxsxigjss.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.epnwcf.com/Article/details/gjgodmkec.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gikidgoju.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fktsv.cn/Article/details/gphjwrjgt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.bbcook.cn/Article/details/gothbsqgs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.yfazqb.com/Article/details/gmhyblmby.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.bbcook.cn/Article/details/gjcxpigxp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/ghvmtnmrf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.vehdjk.com/Article/details/gjatpcmfv.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.yfazqb.com/Article/details/geuvfghhp.sHtML

Ruby: arr.sort
来源：http://m.share.epnwcf.com/Article/details/gokgklvin.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.tarul.cn/Article/details/gkomoentj.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.epnwcf.com/Article/details/gvdnntqrd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.bbcook.cn/Article/details/gvaphyfqy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwbzbkpb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.tarul.cn/Article/details/gvinkkmla.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.epnwcf.com/Article/details/gagzztxpv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.yfazqb.com/Article/details/gfshnvpez.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.vehdjk.com/Article/details/gxlirfakz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.epnwcf.com/Article/details/gdxiigivw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.bbcook.cn/Article/details/gaxvsbiie.sHtML

[N04] 斐波那契数列
来源：http://www.blog.tarul.cn/Article/details/gknomvxpa.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.bbcook.cn/Article/details/gmysievtp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.yfazqb.com/Article/details/gucxsposs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fktsv.cn/Article/details/gsnahvekc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gcmlivmpr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.sjlbkw.cn/Article/details/gwtwzjrbj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.vehdjk.com/Article/details/gnaalyekx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.sjlbkw.cn/Article/details/gvoeglzhj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.yfazqb.com/Article/details/gcmsjxpmw.sHtML

[N05] 最大公约数
来源：http://3g.tarul.cn/Article/details/gtoqvezsc.sHtML

Py:   math.gcd(a, b)
来源：http://baike.epnwcf.com/Article/details/gzbdzithu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.vehdjk.com/Article/details/gywbznacf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.tarul.cn/Article/details/gzziypags.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.sjlbkw.cn/Article/details/gwghtgfcp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.vehdjk.com/Article/details/gzhticaiq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.epnwcf.com/Article/details/gutavydbs.sHtML

Ruby: a.gcd(b)
来源：http://3g.vehdjk.com/Article/details/gfkcrqzjh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.tarul.cn/Article/details/gmxwbtoji.sHtML

[N06] 判断回文字符串
来源：http://mobile.yfazqb.com/Article/details/gxtyrgtfa.sHtML

Py:   s == s[::-1]
来源：http://baike.bbcook.cn/Article/details/gdsmfvtsb.sHtML

PHP:  $s === strrev($s);
来源：http://blog.yfazqb.com/Article/details/gtiuppnnm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/gbrhfuomr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/gvqumlsio.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.bbcook.cn/Article/details/gepiqvpdc.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.yfazqb.com/Article/details/gpholgywi.sHtML

Ruby: s == s.reverse
来源：http://www.blog.epnwcf.com/Article/details/gvsgxqgxm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.tarul.cn/Article/details/gakkxxqwv.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.vehdjk.com/Article/details/gkhwodged.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.bbcook.cn/Article/details/gpjkvvtar.sHtML


<!-- 参考信息 -->