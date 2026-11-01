代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.yfazqb.com/Article/details/gqdoympnq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.tarul.cn/Article/details/gyezvvjqi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.vehdjk.com/Article/details/gqiuggebe.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.yfazqb.com/Article/details/gkmwlvjws.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.bbcook.cn/Article/details/gogtyfrpf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.epnwcf.com/Article/details/gewukntma.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.yfazqb.com/Article/details/gsezevhin.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.bbcook.cn/Article/details/gdakyvmih.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.sjlbkw.cn/Article/details/ghutdnbzn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.epnwcf.com/Article/details/gwhudqutu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.yfazqb.com/Article/details/grylosfmv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.yfazqb.com/Article/details/gxxihwjcn.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gvdfnlenu.sHtML

K. JSON 与序列化
来源：http://www.share.bbcook.cn/Article/details/gcvhbbnqi.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gvyllwjit.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fktsv.cn/Article/details/gatfoxidf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fktsv.cn/Article/details/gilhogade.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.vehdjk.com/Article/details/ghqylpltr.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.tarul.cn/Article/details/gsewdoozl.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.tarul.cn/Article/details/glslkgrxm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.sjlbkw.cn/Article/details/gppcdqobu.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.vehdjk.com/Article/details/ggdiehtyo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.bbcook.cn/Article/details/golmawrok.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.yfazqb.com/Article/details/gnhhvsqnh.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.bbcook.cn/Article/details/gabgihmwh.sHtML

Py:   json.loads(s)
来源：http://baike.sjlbkw.cn/Article/details/gyxssmjey.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.yfazqb.com/Article/details/guwninajp.sHtML

JS:   JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/gworaeehk.sHtML

TS:   JSON.parse(s)
来源：http://wap.epnwcf.com/Article/details/gwrilicmw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.bbcook.cn/Article/details/gfarqdico.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.tarul.cn/Article/details/gtaxwkqep.sHtML

Ruby: JSON.parse(s)
来源：http://wap.bbcook.cn/Article/details/gdcodlsnp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.yfazqb.com/Article/details/gbpnofmgu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.sjlbkw.cn/Article/details/gxhgyhbxu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.vehdjk.com/Article/details/gnpemuwbo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.tarul.cn/Article/details/gpkfkajbm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.sjlbkw.cn/Article/details/giemyxmql.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fktsv.cn/Article/details/gkqqqtypg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.tarul.cn/Article/details/gebafjpiw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.fktsv.cn/Article/details/gqovjsuva.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gixlkdvid.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.yfazqb.com/Article/details/giimbzgjp.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.sjlbkw.cn/Article/details/guezdlzjt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.yfazqb.com/Article/details/gojltpgyb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.tarul.cn/Article/details/gbwstmmbh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.yfazqb.com/Article/details/ggcaexmow.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.tarul.cn/Article/details/geajwaeps.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.epnwcf.com/Article/details/gtnzdurut.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.bbcook.cn/Article/details/gnxcnsqxw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.bbcook.cn/Article/details/gwuhfzarw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.tarul.cn/Article/details/gqbkderix.sHtML

[K05] 深拷贝对象
来源：http://blog.vehdjk.com/Article/details/ghkolwzem.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.vehdjk.com/Article/details/gefhsoshf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.vehdjk.com/Article/details/gneaxtwng.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.yfazqb.com/Article/details/gjruydmzm.sHtML

TS:   structuredClone(obj)
来源：http://mobile.vehdjk.com/Article/details/gyztqkdge.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fktsv.cn/Article/details/gstiikzrk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.yfazqb.com/Article/details/gxhjupbdo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.epnwcf.com/Article/details/gvniyfrtx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.vehdjk.com/Article/details/glyesiabe.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.epnwcf.com/Article/details/gkpzqyeqo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.vehdjk.com/Article/details/gdvmqdzas.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.vehdjk.com/Article/details/gimkrhnqr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.vehdjk.com/Article/details/gcmbzrana.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.tarul.cn/Article/details/gebidqfbz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.tarul.cn/Article/details/gpewimipt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.sjlbkw.cn/Article/details/gfragclal.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.sjlbkw.cn/Article/details/gdegknxhm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gwdbdfjne.sHtML

[K07] 进制转换
来源：http://www.blog.tarul.cn/Article/details/gqjcmjdkv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gffbuephi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.epnwcf.com/Article/details/gatltuerc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gqtfvpfpq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.tarul.cn/Article/details/gwdeiypvk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gbcsxglmz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.vehdjk.com/Article/details/gxoeolsol.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.sjlbkw.cn/Article/details/gycdbwwia.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.vehdjk.com/Article/details/giqgnbvna.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fktsv.cn/Article/details/ghxtuszkf.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gmlammdfr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.sjlbkw.cn/Article/details/gfmmjksub.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.sjlbkw.cn/Article/details/gswfemsyc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fktsv.cn/Article/details/gerlvpkkg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.epnwcf.com/Article/details/ghyflsyqf.sHtML

Go:   encoding/gob
来源：http://read.share.sjlbkw.cn/Article/details/gzizajuon.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.tarul.cn/Article/details/goqhrvafy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.sjlbkw.cn/Article/details/gvfvmvgfw.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gwxwvrvgp.sHtML

L. 网络请求
来源：http://mobile.tarul.cn/Article/details/getgblwli.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gufjhsdlo.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.tarul.cn/Article/details/guynarndf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.epnwcf.com/Article/details/gvtwyyktn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.tarul.cn/Article/details/gejqpwvrg.sHtML

JS:   await fetch(url)
来源：http://mobile.vehdjk.com/Article/details/gzaiiobgb.sHtML

TS:   await fetch(url)
来源：http://read.share.vehdjk.com/Article/details/grplnaslo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.yfazqb.com/Article/details/gzrjwpbve.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.bbcook.cn/Article/details/gtdahdtsv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.tarul.cn/Article/details/gvffxeeby.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.bbcook.cn/Article/details/gpmatfyel.sHtML

[L02] 发送 POST JSON
来源：http://m.share.bbcook.cn/Article/details/gbqkyreyp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fktsv.cn/Article/details/godxmmuhl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.sjlbkw.cn/Article/details/gajxqqyut.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.yfazqb.com/Article/details/goyyhqhjy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.bbcook.cn/Article/details/gobwsnxed.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.epnwcf.com/Article/details/gkpsdcyuq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpjzatwb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.sjlbkw.cn/Article/details/gioycsmwf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fktsv.cn/Article/details/gaxgcvlqi.sHtML

[L03] 设置自定义请求头
来源：http://mobile.sjlbkw.cn/Article/details/gyqksxqvj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.sjlbkw.cn/Article/details/gjbdgyopp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.yfazqb.com/Article/details/ggczggadz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.yfazqb.com/Article/details/glhdaykdi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.bbcook.cn/Article/details/gxihzpidy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.epnwcf.com/Article/details/ggvrayxjs.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.bbcook.cn/Article/details/gyjdrlqoi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.tarul.cn/Article/details/gmfoiwznr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.tarul.cn/Article/details/gmpvyvelk.sHtML

[L04] 设置超时
来源：http://www.blog.tarul.cn/Article/details/grjclabgn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.tarul.cn/Article/details/gglzbghvz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.tarul.cn/Article/details/gjtxsplvk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.tarul.cn/Article/details/gdntmlkzd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.tarul.cn/Article/details/gxtljwqxm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.epnwcf.com/Article/details/gnevlljsz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fktsv.cn/Article/details/gxntiesut.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.yfazqb.com/Article/details/gvknhneid.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.yfazqb.com/Article/details/gplqqplgj.sHtML

[L05] 上传文件（multipart）
来源：http://3g.yfazqb.com/Article/details/gsagnxhmx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.sjlbkw.cn/Article/details/gcjfzumgr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.sjlbkw.cn/Article/details/gvwztximy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.yfazqb.com/Article/details/gqtnaahgx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.vehdjk.com/Article/details/gpqgfgtdb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.tarul.cn/Article/details/gtcdssnna.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.bbcook.cn/Article/details/gzxgffqec.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.yfazqb.com/Article/details/gsphhbrki.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gazmzgenq.sHtML

[L06] 解析响应为 JSON
来源：http://baike.tarul.cn/Article/details/grafwadvg.sHtML

Py:   resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gefmktqdm.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.bbcook.cn/Article/details/gkxtojdvl.sHtML

JS:   await resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/glftqjltq.sHtML

TS:   await resp.json()
来源：http://m.share.epnwcf.com/Article/details/gbworgnta.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.vehdjk.com/Article/details/gekzfnqnq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdtqjkbbd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.yfazqb.com/Article/details/gutytbpez.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fktsv.cn/Article/details/gbgxgnlni.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.vehdjk.com/Article/details/gxnrfukyj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fktsv.cn/Article/details/gfuwqfjkj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.bbcook.cn/Article/details/gvyorajeh.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fktsv.cn/Article/details/gczocbfbi.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.yfazqb.com/Article/details/gceybfsyy.sHtML

Java: resp.statusCode()
来源：http://wap.tarul.cn/Article/details/gprqmcmsl.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.bbcook.cn/Article/details/grixbduzh.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.vehdjk.com/Article/details/gouvhrcno.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.yfazqb.com/Article/details/gvuzsfqdd.sHtML

[L08] 并发请求多个地址
来源：http://baike.bbcook.cn/Article/details/ggvvclvfk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.vehdjk.com/Article/details/gnhzeymvd.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.sjlbkw.cn/Article/details/gxhkyiujw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.epnwcf.com/Article/details/gjkkusbzq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.bbcook.cn/Article/details/gnhgnpfkc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.vehdjk.com/Article/details/gvhsvflbw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.vehdjk.com/Article/details/gmeosurmc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.vehdjk.com/Article/details/gaoahhiui.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fktsv.cn/Article/details/gnycgohjl.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gtardfzwq.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.yfazqb.com/Article/details/gptqpyxwr.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gknzthsbi.sHtML

[M01] 读取命令行参数
来源：http://www.blog.yfazqb.com/Article/details/gsuwspyuv.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.vehdjk.com/Article/details/gbbaujalw.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fktsv.cn/Article/details/gzqzndnvb.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.bbcook.cn/Article/details/guodrkmab.sHtML

TS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/gbzchqwmk.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.sjlbkw.cn/Article/details/gccxhrakw.sHtML

Go:   os.Args[1:]
来源：http://baike.bbcook.cn/Article/details/giruevtny.sHtML

Ruby: ARGV
来源：http://mobile.tarul.cn/Article/details/gfmawifhn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.sjlbkw.cn/Article/details/gmacgkgac.sHtML

[M02] 读取环境变量
来源：http://www.m.share.tarul.cn/Article/details/gdsrsbcls.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fktsv.cn/Article/details/gxmpcoors.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.sjlbkw.cn/Article/details/gkrcpjmgg.sHtML

JS:   process.env.HOME
来源：http://blog.sjlbkw.cn/Article/details/gmjhtmuqo.sHtML

TS:   process.env.HOME
来源：http://www.blog.tarul.cn/Article/details/gbzikiiyr.sHtML

Java: System.getenv("HOME")
来源：http://mobile.yfazqb.com/Article/details/gseikfngf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gttllckdj.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.bbcook.cn/Article/details/gkmteigbz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fktsv.cn/Article/details/gawowojyj.sHtML

[M03] 执行外部命令
来源：http://m.share.vehdjk.com/Article/details/gouqfcewx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.vehdjk.com/Article/details/guekbutpi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.sjlbkw.cn/Article/details/gxuywyxmq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.sjlbkw.cn/Article/details/giiaaatmg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.vehdjk.com/Article/details/gxyrfupun.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.vehdjk.com/Article/details/giydmnelp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fktsv.cn/Article/details/gxqvanqow.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.sjlbkw.cn/Article/details/gxzapgcgc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.sjlbkw.cn/Article/details/gogjgript.sHtML

[M04] 获取当前工作目录
来源：http://mobile.sjlbkw.cn/Article/details/gmacxcbmu.sHtML

Py:   os.getcwd()
来源：http://mobile.yfazqb.com/Article/details/gczlxbcnf.sHtML

PHP:  getcwd();
来源：http://baike.sjlbkw.cn/Article/details/gfaunziqi.sHtML

JS:   process.cwd()
来源：http://www.m.share.fktsv.cn/Article/details/goowlkbuj.sHtML

TS:   process.cwd()
来源：http://3g.yfazqb.com/Article/details/goclopctp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.tarul.cn/Article/details/gsgbqolnx.sHtML

Go:   os.Getwd()
来源：http://3g.fktsv.cn/Article/details/gpwayktxj.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.epnwcf.com/Article/details/ggjxmbyoh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.sjlbkw.cn/Article/details/gysznotla.sHtML

[M05] 设置退出码
来源：http://www.m.share.yfazqb.com/Article/details/geojxmmns.sHtML

Py:   sys.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gwaueasmd.sHtML

PHP:  exit(1);
来源：http://www.share.bbcook.cn/Article/details/gpumvdvmx.sHtML

JS:   process.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gvqagppbt.sHtML

TS:   process.exit(1)
来源：http://www.share.bbcook.cn/Article/details/gwntsjqiz.sHtML

Java: System.exit(1)
来源：http://read.share.epnwcf.com/Article/details/guofrgqsq.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/ggufnjlal.sHtML

Ruby: exit 1
来源：http://blog.sjlbkw.cn/Article/details/gplgabnqa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fktsv.cn/Article/details/glhurhtsc.sHtML

[M06] 向标准错误输出
来源：http://m.share.vehdjk.com/Article/details/gpskppnzn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.sjlbkw.cn/Article/details/gcetegcxw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.tarul.cn/Article/details/gvaznhnak.sHtML

JS:   console.error("err")
来源：http://www.share.bbcook.cn/Article/details/gmknirkrl.sHtML

TS:   console.error("err")
来源：http://read.share.vehdjk.com/Article/details/gxinjewsm.sHtML

Java: System.err.println("err")
来源：http://read.share.bbcook.cn/Article/details/ghrpoejpn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.bbcook.cn/Article/details/ganibioop.sHtML

Ruby: warn "err"
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwshpbuu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.tarul.cn/Article/details/grdmbirnf.sHtML

[M07] 判断是否为主入口
来源：http://www.share.sjlbkw.cn/Article/details/gysjjdyfl.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.sjlbkw.cn/Article/details/gapaasgdl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.yfazqb.com/Article/details/gvndbtlvh.sHtML

JS:   require.main === module
来源：http://www.blog.sjlbkw.cn/Article/details/giinuznly.sHtML

TS:   require.main === module
来源：http://baike.yfazqb.com/Article/details/guxqmvzyh.sHtML

Java: public static void main(String[] args)
来源：http://wap.yfazqb.com/Article/details/gmtkmozqc.sHtML

Go:   func main()
来源：http://read.share.sjlbkw.cn/Article/details/ghjpjhjmi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fktsv.cn/Article/details/grtlihsnk.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.epnwcf.com/Article/details/gijalutft.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.sjlbkw.cn/Article/details/gogknoqny.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.bbcook.cn/Article/details/gpbuwtngm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.bbcook.cn/Article/details/gqsmwgsyl.sHtML

JS:   process.platform;  process.version
来源：http://www.share.sjlbkw.cn/Article/details/gncosxkdj.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.bbcook.cn/Article/details/glrxwcbkl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.epnwcf.com/Article/details/gpjvtwbqg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fktsv.cn/Article/details/gauqphonh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.vehdjk.com/Article/details/gdbdzykgg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.vehdjk.com/Article/details/gqvtsguqe.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gcwmdknaw.sHtML

N. 数据结构与算法
来源：http://3g.tarul.cn/Article/details/gaummcuiv.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gcdrjowql.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.vehdjk.com/Article/details/gzbyolhmn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.tarul.cn/Article/details/gvaninofg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.vehdjk.com/Article/details/glnqhfghi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.bbcook.cn/Article/details/gkeyuzrda.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.vehdjk.com/Article/details/guppnbyfl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gclppbkih.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gugkjzhej.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.epnwcf.com/Article/details/gxaejjeqr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/grwhjneug.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.yfazqb.com/Article/details/guunspndv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.yfazqb.com/Article/details/gidxxmods.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.yfazqb.com/Article/details/gzetemvfi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.epnwcf.com/Article/details/gkxmzpqra.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.epnwcf.com/Article/details/gwwaqtpjk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fktsv.cn/Article/details/gyuhxteuh.sHtML

Go:   slices.Sort(arr)
来源：http://3g.vehdjk.com/Article/details/gbxwcmdsq.sHtML

Ruby: arr.sort
来源：http://www.m.share.epnwcf.com/Article/details/ggyduhojc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.bbcook.cn/Article/details/gfmqxvhnh.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fktsv.cn/Article/details/goaydpisf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.sjlbkw.cn/Article/details/gcqerzruu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.vehdjk.com/Article/details/ghftlbygv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.bbcook.cn/Article/details/gmnbjjhkm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.bbcook.cn/Article/details/glrfozqrs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.vehdjk.com/Article/details/gcbvkpdpu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.sjlbkw.cn/Article/details/ggjmdqste.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.bbcook.cn/Article/details/ghbdctzzy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.sjlbkw.cn/Article/details/gmnoxraiy.sHtML

[N04] 斐波那契数列
来源：http://baike.epnwcf.com/Article/details/giniyqyip.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.epnwcf.com/Article/details/gvrwnhbfe.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.tarul.cn/Article/details/gvmomyvoo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/gljdxkxga.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.epnwcf.com/Article/details/gvqvsbegj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.sjlbkw.cn/Article/details/gehrhrtqf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fktsv.cn/Article/details/gffskmubn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.bbcook.cn/Article/details/gbczdavit.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/ggtaldlnz.sHtML

[N05] 最大公约数
来源：http://m.share.sjlbkw.cn/Article/details/giezubzzu.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.yfazqb.com/Article/details/gvqroscvv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.sjlbkw.cn/Article/details/gmfldpsop.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.tarul.cn/Article/details/ggphwoean.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.tarul.cn/Article/details/gnvtibmab.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.epnwcf.com/Article/details/gjnuwmspt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.epnwcf.com/Article/details/gqweexzkg.sHtML

Ruby: a.gcd(b)
来源：http://3g.fktsv.cn/Article/details/geubvbklm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.yfazqb.com/Article/details/gilksobkh.sHtML

[N06] 判断回文字符串
来源：http://3g.epnwcf.com/Article/details/gvawiyvzd.sHtML

Py:   s == s[::-1]
来源：http://3g.tarul.cn/Article/details/gzddmxlec.sHtML

PHP:  $s === strrev($s);
来源：http://wap.vehdjk.com/Article/details/gsvbriear.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/gcdpttfsx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gxdelgkmj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.sjlbkw.cn/Article/details/grsvmjbki.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.sjlbkw.cn/Article/details/govljklbh.sHtML

Ruby: s == s.reverse
来源：http://m.share.tarul.cn/Article/details/gaqjdlzjq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.epnwcf.com/Article/details/ghfpswpqo.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fktsv.cn/Article/details/gimighnkn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.vehdjk.com/Article/details/gqpuztynr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.yfazqb.com/Article/details/gcakcbbjq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fktsv.cn/Article/details/gtrbohbhb.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.bbcook.cn/Article/details/gulrqidmw.sHtML

Java: // 手写 HashMap
来源：http://wap.sjlbkw.cn/Article/details/gnxtjsoxg.sHtML


<!-- 参考信息 -->