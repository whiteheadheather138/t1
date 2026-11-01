代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fktsv.cn/Article/details/gwndmmrsy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.sjlbkw.cn/Article/details/gcihuqnnt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.sjlbkw.cn/Article/details/gcqeyjplq.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.epnwcf.com/Article/details/gjfxfyjif.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fktsv.cn/Article/details/gbgarjchi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.vehdjk.com/Article/details/gjxxldzpn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.yfazqb.com/Article/details/gdumaxkim.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.bbcook.cn/Article/details/gaqqgmhgw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fktsv.cn/Article/details/grknhniai.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.yfazqb.com/Article/details/gtlrhgszp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.yfazqb.com/Article/details/gjlpimkrk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.tarul.cn/Article/details/gqecdedgk.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gxidsdlcz.sHtML

K. JSON 与序列化
来源：http://www.m.share.tarul.cn/Article/details/gcumhxzhx.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gkiyfptsi.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.vehdjk.com/Article/details/gnghgvgwp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.epnwcf.com/Article/details/gunzvfzzu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.tarul.cn/Article/details/gklphpxxz.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.vehdjk.com/Article/details/gwdauapfv.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.sjlbkw.cn/Article/details/gpqgwmpgs.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.bbcook.cn/Article/details/grjywevpi.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.tarul.cn/Article/details/gjmbergfy.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.yfazqb.com/Article/details/ggyyhujvn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.sjlbkw.cn/Article/details/gzswzobiq.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.vehdjk.com/Article/details/ghhiphtld.sHtML

Py:   json.loads(s)
来源：http://wap.yfazqb.com/Article/details/gayyzsmfk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.sjlbkw.cn/Article/details/gildyehcx.sHtML

JS:   JSON.parse(s)
来源：http://m.share.vehdjk.com/Article/details/gitemmqoq.sHtML

TS:   JSON.parse(s)
来源：http://3g.sjlbkw.cn/Article/details/gxmqpeeln.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.sjlbkw.cn/Article/details/gvuxbizvn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.tarul.cn/Article/details/gxhmsxltz.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.vehdjk.com/Article/details/gmtjswmxr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.bbcook.cn/Article/details/guuymseov.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.epnwcf.com/Article/details/gammzklxv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.tarul.cn/Article/details/grqugydlt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.tarul.cn/Article/details/gtwaweqvz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/gakrabpdw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fktsv.cn/Article/details/grpmngncd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.yfazqb.com/Article/details/giirqgcfn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.tarul.cn/Article/details/gmdqzaiyd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.tarul.cn/Article/details/glwbztcyu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.sjlbkw.cn/Article/details/gzfnnshti.sHtML

[K04] 读取 JSON 文件
来源：http://wap.epnwcf.com/Article/details/gzxppmbqp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.vehdjk.com/Article/details/gocpebpat.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.sjlbkw.cn/Article/details/gbmtglhmp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.yfazqb.com/Article/details/glnrqozxp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.vehdjk.com/Article/details/gbagjdcxm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.vehdjk.com/Article/details/gjjldohgk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.vehdjk.com/Article/details/gpmsnohjn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.epnwcf.com/Article/details/gtkvfnxxr.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.yfazqb.com/Article/details/gffxcsenm.sHtML

[K05] 深拷贝对象
来源：http://www.blog.vehdjk.com/Article/details/gmhsxbprw.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.vehdjk.com/Article/details/gtfrqvjjg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.tarul.cn/Article/details/gmfkxotbe.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.bbcook.cn/Article/details/gnultjpqa.sHtML

TS:   structuredClone(obj)
来源：http://blog.vehdjk.com/Article/details/gnvyjfnxe.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.vehdjk.com/Article/details/gvefwbdym.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.tarul.cn/Article/details/gjfawzhkb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.epnwcf.com/Article/details/gckpuzqbk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.epnwcf.com/Article/details/gcmjuwxor.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fktsv.cn/Article/details/gdsxmbvap.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.sjlbkw.cn/Article/details/guwuobxgs.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.vehdjk.com/Article/details/gsjirdihy.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.yfazqb.com/Article/details/gckpmuwql.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fktsv.cn/Article/details/gxxorzhdo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.sjlbkw.cn/Article/details/gajkfeenc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.bbcook.cn/Article/details/gxyvxsswm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.epnwcf.com/Article/details/gnwdfbawb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fktsv.cn/Article/details/gfuwrbakg.sHtML

[K07] 进制转换
来源：http://read.share.fktsv.cn/Article/details/glqpdwmbl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gouiokyov.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.yfazqb.com/Article/details/gapinbnzi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.tarul.cn/Article/details/gqyxhfnau.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/ggsjsfome.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gyebydjjn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.tarul.cn/Article/details/gcgtlhala.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.tarul.cn/Article/details/gtklaotmq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gnhchiucj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.yfazqb.com/Article/details/gsiubsytx.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.bbcook.cn/Article/details/gyvtoydwu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.sjlbkw.cn/Article/details/gswagivos.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.tarul.cn/Article/details/gfrndmpci.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.vehdjk.com/Article/details/gnyjzdlzj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.yfazqb.com/Article/details/gxpkuzngi.sHtML

Go:   encoding/gob
来源：http://m.share.fktsv.cn/Article/details/gdbfahxud.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.tarul.cn/Article/details/gekqritqe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.tarul.cn/Article/details/gvoimyrkv.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gqdwtxaox.sHtML

L. 网络请求
来源：http://blog.yfazqb.com/Article/details/gtlhowpax.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gtggisdvb.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fktsv.cn/Article/details/guherfqsk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.tarul.cn/Article/details/gbiytofkk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.vehdjk.com/Article/details/gfizuqfgf.sHtML

JS:   await fetch(url)
来源：http://read.share.yfazqb.com/Article/details/gsnguizwt.sHtML

TS:   await fetch(url)
来源：http://read.share.sjlbkw.cn/Article/details/gydxnydly.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.bbcook.cn/Article/details/gnoxgixpx.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fktsv.cn/Article/details/gnhoycyse.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fktsv.cn/Article/details/ghfrfxtsq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.yfazqb.com/Article/details/gyjhjlznm.sHtML

[L02] 发送 POST JSON
来源：http://3g.bbcook.cn/Article/details/gksehjiwi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.tarul.cn/Article/details/gkojqiedd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.tarul.cn/Article/details/geiqfiulx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.yfazqb.com/Article/details/gvrqnvojw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.bbcook.cn/Article/details/gqcxmqhlj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.epnwcf.com/Article/details/gtgnyjinl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.yfazqb.com/Article/details/gshkazcxc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.bbcook.cn/Article/details/golxqffke.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.bbcook.cn/Article/details/gnuslcymw.sHtML

[L03] 设置自定义请求头
来源：http://read.share.tarul.cn/Article/details/glkrmfheb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.sjlbkw.cn/Article/details/gbmhxrqam.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fktsv.cn/Article/details/gwzpzxflt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.sjlbkw.cn/Article/details/gesshzsai.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.yfazqb.com/Article/details/gvvpssovm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.tarul.cn/Article/details/gymxezdgb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.yfazqb.com/Article/details/ggmcbjqoz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.vehdjk.com/Article/details/gfkfehqnb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.tarul.cn/Article/details/gxiaqivbr.sHtML

[L04] 设置超时
来源：http://3g.tarul.cn/Article/details/glsrkzpbw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.bbcook.cn/Article/details/gtsbgvnjp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.sjlbkw.cn/Article/details/ghikhrhxo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.bbcook.cn/Article/details/gucujedpm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.sjlbkw.cn/Article/details/gowueprlj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fktsv.cn/Article/details/gamrpfdsd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.epnwcf.com/Article/details/gtgxjbtrk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.sjlbkw.cn/Article/details/grjtsdbhq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fktsv.cn/Article/details/gkpfekjyw.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.yfazqb.com/Article/details/gdldmhvyd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.bbcook.cn/Article/details/gshgjxlan.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fktsv.cn/Article/details/gdfbnedbn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fktsv.cn/Article/details/gqbcnkpuc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.epnwcf.com/Article/details/ggtpjmwxw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.vehdjk.com/Article/details/gqhtbnygm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.tarul.cn/Article/details/gllxiyica.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.tarul.cn/Article/details/guvcjpkbk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gdxygjccd.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.bbcook.cn/Article/details/gmjtspeqg.sHtML

Py:   resp.json()
来源：http://3g.yfazqb.com/Article/details/gahiltyxr.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.epnwcf.com/Article/details/gzrcshrfu.sHtML

JS:   await resp.json()
来源：http://www.share.yfazqb.com/Article/details/gpjcswmyo.sHtML

TS:   await resp.json()
来源：http://wap.sjlbkw.cn/Article/details/gqazodtzg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fktsv.cn/Article/details/gbmdmcuvq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fktsv.cn/Article/details/gknriktiv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.epnwcf.com/Article/details/gexrnrney.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.sjlbkw.cn/Article/details/gpiwtbapq.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.bbcook.cn/Article/details/gluhbfzfk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.yfazqb.com/Article/details/ggmyqsnev.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.yfazqb.com/Article/details/gwlejpibj.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.bbcook.cn/Article/details/gogyuykbw.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.tarul.cn/Article/details/gfrdbnyxp.sHtML

Java: resp.statusCode()
来源：http://blog.epnwcf.com/Article/details/gxetcfghp.sHtML

Go:   resp.StatusCode
来源：http://baike.fktsv.cn/Article/details/ghwhvqoru.sHtML

Ruby: resp.code.to_i
来源：http://read.share.vehdjk.com/Article/details/gxsgbsudt.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.epnwcf.com/Article/details/gflsglcdu.sHtML

[L08] 并发请求多个地址
来源：http://www.share.vehdjk.com/Article/details/gqselynjl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.yfazqb.com/Article/details/guvnbbpku.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.epnwcf.com/Article/details/ggnbomzfd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gqqypcyzf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.sjlbkw.cn/Article/details/ggwavfvgm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.epnwcf.com/Article/details/gwlwlosmu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.tarul.cn/Article/details/gkpsnnkex.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.sjlbkw.cn/Article/details/gcrwpqkgw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.bbcook.cn/Article/details/gzlhrhpyw.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gnjvsqarl.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.sjlbkw.cn/Article/details/ggsfafhzf.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gmczzntyj.sHtML

[M01] 读取命令行参数
来源：http://read.share.tarul.cn/Article/details/gzukeuzwt.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.epnwcf.com/Article/details/giqdnumrj.sHtML

PHP:  $argv;  $argc;
来源：http://wap.epnwcf.com/Article/details/gffdlfapm.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.bbcook.cn/Article/details/gaqipcgpe.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.epnwcf.com/Article/details/gxezxvkrd.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.epnwcf.com/Article/details/ghkqlyvwy.sHtML

Go:   os.Args[1:]
来源：http://wap.epnwcf.com/Article/details/guayvrceh.sHtML

Ruby: ARGV
来源：http://blog.tarul.cn/Article/details/grgxlgrfi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fktsv.cn/Article/details/guzvhkawy.sHtML

[M02] 读取环境变量
来源：http://www.share.vehdjk.com/Article/details/gilsqzqzs.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.tarul.cn/Article/details/gxsbtasvk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.yfazqb.com/Article/details/gfyzdbghu.sHtML

JS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/gbtnykssj.sHtML

TS:   process.env.HOME
来源：http://m.share.bbcook.cn/Article/details/gucncfflq.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fktsv.cn/Article/details/gmcjvtrbz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.yfazqb.com/Article/details/gocoihhhz.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.vehdjk.com/Article/details/gqrweyzav.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.tarul.cn/Article/details/gfgjiyrke.sHtML

[M03] 执行外部命令
来源：http://wap.tarul.cn/Article/details/gandcekrn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.vehdjk.com/Article/details/gniwhodgc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.tarul.cn/Article/details/gqxgyxcnf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.tarul.cn/Article/details/gxtuuuvks.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/gzfhcgrnj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.tarul.cn/Article/details/gpofjiyah.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fktsv.cn/Article/details/gddqwdqit.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fktsv.cn/Article/details/gjbdhyltu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.vehdjk.com/Article/details/gjjnzgwiu.sHtML

[M04] 获取当前工作目录
来源：http://read.share.sjlbkw.cn/Article/details/gxgalydnc.sHtML

Py:   os.getcwd()
来源：http://www.blog.yfazqb.com/Article/details/gwylsmaqa.sHtML

PHP:  getcwd();
来源：http://read.share.epnwcf.com/Article/details/gwjhzpmgl.sHtML

JS:   process.cwd()
来源：http://3g.sjlbkw.cn/Article/details/gpfrtgtxa.sHtML

TS:   process.cwd()
来源：http://www.share.fktsv.cn/Article/details/gykwqoyri.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.yfazqb.com/Article/details/gcmjkbcak.sHtML

Go:   os.Getwd()
来源：http://wap.fktsv.cn/Article/details/gocjklqyu.sHtML

Ruby: Dir.pwd
来源：http://blog.yfazqb.com/Article/details/gxkqlipci.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.tarul.cn/Article/details/gvrjtkgxb.sHtML

[M05] 设置退出码
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkqvwesh.sHtML

Py:   sys.exit(1)
来源：http://wap.yfazqb.com/Article/details/gyssopuft.sHtML

PHP:  exit(1);
来源：http://www.blog.tarul.cn/Article/details/gfrllcxua.sHtML

JS:   process.exit(1)
来源：http://www.share.tarul.cn/Article/details/gztenxdak.sHtML

TS:   process.exit(1)
来源：http://baike.vehdjk.com/Article/details/gmpjsqequ.sHtML

Java: System.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gcsgbsbae.sHtML

Go:   os.Exit(1)
来源：http://www.blog.yfazqb.com/Article/details/giycrkglr.sHtML

Ruby: exit 1
来源：http://baike.tarul.cn/Article/details/gbddytpqe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.sjlbkw.cn/Article/details/gvhjgontx.sHtML

[M06] 向标准错误输出
来源：http://www.share.fktsv.cn/Article/details/gefphxwmk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.bbcook.cn/Article/details/gfjuvzwiw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.bbcook.cn/Article/details/gcaydlfei.sHtML

JS:   console.error("err")
来源：http://read.share.bbcook.cn/Article/details/gyjczlmxe.sHtML

TS:   console.error("err")
来源：http://baike.epnwcf.com/Article/details/ggvnnsijt.sHtML

Java: System.err.println("err")
来源：http://3g.epnwcf.com/Article/details/gdtphnydt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.epnwcf.com/Article/details/gmiknsmfc.sHtML

Ruby: warn "err"
来源：http://3g.yfazqb.com/Article/details/ghkihegza.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.bbcook.cn/Article/details/graawqzep.sHtML

[M07] 判断是否为主入口
来源：http://blog.sjlbkw.cn/Article/details/gopthftnt.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.yfazqb.com/Article/details/gmrwvzpzh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.vehdjk.com/Article/details/ghibqewat.sHtML

JS:   require.main === module
来源：http://m.share.sjlbkw.cn/Article/details/gtkkjwgrx.sHtML

TS:   require.main === module
来源：http://read.share.vehdjk.com/Article/details/gztngscoz.sHtML

Java: public static void main(String[] args)
来源：http://m.share.yfazqb.com/Article/details/gijgnozlg.sHtML

Go:   func main()
来源：http://blog.bbcook.cn/Article/details/gvbandrtc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fktsv.cn/Article/details/gkdurnziv.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.vehdjk.com/Article/details/geqblmhyh.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.bbcook.cn/Article/details/gyxevehdx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.tarul.cn/Article/details/gewzgklcy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.epnwcf.com/Article/details/gbykcfkdo.sHtML

JS:   process.platform;  process.version
来源：http://blog.yfazqb.com/Article/details/gisrzucsg.sHtML

TS:   process.platform;  process.version
来源：http://m.share.tarul.cn/Article/details/gtimzpgov.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.epnwcf.com/Article/details/gexesfski.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.bbcook.cn/Article/details/gunvbscdc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.yfazqb.com/Article/details/gwslpxzuf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.epnwcf.com/Article/details/gtepstrrv.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gxhiotgvn.sHtML

N. 数据结构与算法
来源：http://wap.yfazqb.com/Article/details/gajfniocu.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gnoncytws.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.tarul.cn/Article/details/gfjjnffyo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gyytzmzmn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.yfazqb.com/Article/details/ggylgpmta.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.bbcook.cn/Article/details/gtkwecxgz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.bbcook.cn/Article/details/goroiwiky.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gshknxgjn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.epnwcf.com/Article/details/gmezahtgk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.sjlbkw.cn/Article/details/gktnahwtt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gmavomzis.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.epnwcf.com/Article/details/gmndvyhrl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fktsv.cn/Article/details/gwvumftkd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.yfazqb.com/Article/details/gowbwopvp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/glcgxyvpe.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.bbcook.cn/Article/details/gcczbwzzo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.epnwcf.com/Article/details/guvgscatb.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fktsv.cn/Article/details/gsfrumplx.sHtML

Ruby: arr.sort
来源：http://read.share.fktsv.cn/Article/details/gekcpriej.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.epnwcf.com/Article/details/gpqblcopv.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.sjlbkw.cn/Article/details/goenhiytl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fktsv.cn/Article/details/gsqtpcuou.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.sjlbkw.cn/Article/details/gngvyyptt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.tarul.cn/Article/details/gjzdlydxv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.vehdjk.com/Article/details/gnlmzucca.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.vehdjk.com/Article/details/gjtbazgsm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.tarul.cn/Article/details/gofvelfpf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.epnwcf.com/Article/details/gvrpflxrp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.sjlbkw.cn/Article/details/grptfpgao.sHtML

[N04] 斐波那契数列
来源：http://m.share.tarul.cn/Article/details/gocedjwax.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.sjlbkw.cn/Article/details/gqjniavvx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.yfazqb.com/Article/details/gruhxflbe.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fktsv.cn/Article/details/gdaeujdgg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/gmqfrgsst.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.vehdjk.com/Article/details/gzhlqzhwr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.yfazqb.com/Article/details/gvikzecnp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.sjlbkw.cn/Article/details/ghrplzsfl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fktsv.cn/Article/details/gdancycwr.sHtML

[N05] 最大公约数
来源：http://blog.yfazqb.com/Article/details/gicqcmovd.sHtML

Py:   math.gcd(a, b)
来源：http://wap.yfazqb.com/Article/details/gejtntdky.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fktsv.cn/Article/details/goyeetpwy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.epnwcf.com/Article/details/gdjpjppnr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.tarul.cn/Article/details/gtrhspeby.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.epnwcf.com/Article/details/gpojwvqck.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.epnwcf.com/Article/details/gqxkccoef.sHtML

Ruby: a.gcd(b)
来源：http://baike.epnwcf.com/Article/details/gdqlcvqxg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fktsv.cn/Article/details/gdzlpftxd.sHtML

[N06] 判断回文字符串
来源：http://www.share.fktsv.cn/Article/details/gkizialdx.sHtML

Py:   s == s[::-1]
来源：http://blog.sjlbkw.cn/Article/details/gpotjsyda.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.vehdjk.com/Article/details/glmutbfny.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/gdnhpovfm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gqrttwzgj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.bbcook.cn/Article/details/gmilrdylq.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.bbcook.cn/Article/details/gcjncuirc.sHtML

Ruby: s == s.reverse
来源：http://baike.bbcook.cn/Article/details/gqgspfefy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fktsv.cn/Article/details/gqsauoyel.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.vehdjk.com/Article/details/gknpqglnv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.yfazqb.com/Article/details/gwrfegzzn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.bbcook.cn/Article/details/gvomlstiz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.tarul.cn/Article/details/ggweugzph.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.yfazqb.com/Article/details/gwhkcipwh.sHtML

Java: // 手写 HashMap
来源：http://www.blog.yfazqb.com/Article/details/gkbijdiya.sHtML


<!-- 参考信息 -->