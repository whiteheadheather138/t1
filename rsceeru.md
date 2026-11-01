代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.yfazqb.com/Article/details/gmdfmzmpp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxcqxdgu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.vehdjk.com/Article/details/gltazvral.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.tarul.cn/Article/details/gtnxtcvrg.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.tarul.cn/Article/details/gufykirde.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.yfazqb.com/Article/details/gtggsqcnq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.yfazqb.com/Article/details/gccdbxait.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gizzehwjg.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gxomtffok.sHtML

K. JSON 与序列化
来源：http://m.share.fktsv.cn/Article/details/gecjpbjlw.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gfbnongea.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gqoeqtysq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.tarul.cn/Article/details/ghwowtclk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fktsv.cn/Article/details/gpdnophtv.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.vehdjk.com/Article/details/ggyalxmme.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.yfazqb.com/Article/details/gjgtsgxbq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.tarul.cn/Article/details/gdfgqdroe.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.epnwcf.com/Article/details/gggyabjkj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.vehdjk.com/Article/details/gvymgwchr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.epnwcf.com/Article/details/gyqnvdcer.sHtML

[K02] JSON 字符串转对象
来源：http://3g.sjlbkw.cn/Article/details/gjolcwgrl.sHtML

Py:   json.loads(s)
来源：http://blog.vehdjk.com/Article/details/goeqnhzyk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.epnwcf.com/Article/details/gxalvatuz.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.sjlbkw.cn/Article/details/giymqvmcw.sHtML

TS:   JSON.parse(s)
来源：http://www.share.vehdjk.com/Article/details/gdyvweaoc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.yfazqb.com/Article/details/gbzylqesm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.sjlbkw.cn/Article/details/gaoyrbvqw.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fktsv.cn/Article/details/gceqkpkwz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fktsv.cn/Article/details/gvspgucdw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.vehdjk.com/Article/details/gnkpaujxe.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.epnwcf.com/Article/details/gpusumpxv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.sjlbkw.cn/Article/details/gskklkwxc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gnyltkvey.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkbvnohz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.bbcook.cn/Article/details/geesgeudn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.epnwcf.com/Article/details/ggrqmcbhi.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.tarul.cn/Article/details/gqqsgxmbm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fktsv.cn/Article/details/gbebiuhsg.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.bbcook.cn/Article/details/guxalyggh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.vehdjk.com/Article/details/gsmnxlacf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.yfazqb.com/Article/details/gksvzwxeh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.vehdjk.com/Article/details/geccfvmoy.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.vehdjk.com/Article/details/gisssoaxh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fktsv.cn/Article/details/gquzopqtr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.sjlbkw.cn/Article/details/gdhpgnzlx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fktsv.cn/Article/details/gaujzugnv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.bbcook.cn/Article/details/gofgiohkl.sHtML

[K05] 深拷贝对象
来源：http://m.share.epnwcf.com/Article/details/gpirutxlq.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gmnnnswpk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.bbcook.cn/Article/details/gdevqgxtb.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gsvxvmcrn.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.vehdjk.com/Article/details/gprazuvfv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fktsv.cn/Article/details/grssdiiqb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.bbcook.cn/Article/details/gkqvuiwxf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.yfazqb.com/Article/details/gqdteokos.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fktsv.cn/Article/details/gsobvande.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.vehdjk.com/Article/details/gsubouirr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fktsv.cn/Article/details/ghuslogjq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fktsv.cn/Article/details/gtijymutb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.sjlbkw.cn/Article/details/gztedtnau.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.sjlbkw.cn/Article/details/gzlsdmwaq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.epnwcf.com/Article/details/gklcetycd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.epnwcf.com/Article/details/gtsmhyjlf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.tarul.cn/Article/details/gopvnzdmj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.yfazqb.com/Article/details/gfijkyipx.sHtML

[K07] 进制转换
来源：http://baike.vehdjk.com/Article/details/gyaobzfvn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/ghkbmoltw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.epnwcf.com/Article/details/gmftpuvlw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/gywyysntk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gfuupkacg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gqjmelpri.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.bbcook.cn/Article/details/ggtqzkiqs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.sjlbkw.cn/Article/details/gjaxrngvy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gqkzcbrav.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.epnwcf.com/Article/details/gudyezbkt.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.vehdjk.com/Article/details/ghmifpvqz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.tarul.cn/Article/details/gnxzmjord.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.sjlbkw.cn/Article/details/ggcovhzwx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.sjlbkw.cn/Article/details/gecviarim.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.yfazqb.com/Article/details/gtxhalzzi.sHtML

Go:   encoding/gob
来源：http://blog.fktsv.cn/Article/details/gsdjpamci.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.vehdjk.com/Article/details/gcjzwskzn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fktsv.cn/Article/details/gcwyguhmk.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gwpmprfmr.sHtML

L. 网络请求
来源：http://www.m.share.fktsv.cn/Article/details/gordoyxcg.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/ggnvmleqt.sHtML

[L01] 发送 GET 请求
来源：http://wap.tarul.cn/Article/details/gagzkizas.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.tarul.cn/Article/details/gcjwscgzd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.sjlbkw.cn/Article/details/ghyjtzpps.sHtML

JS:   await fetch(url)
来源：http://mobile.epnwcf.com/Article/details/gxxcffirl.sHtML

TS:   await fetch(url)
来源：http://www.share.fktsv.cn/Article/details/gkjmqaevm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.sjlbkw.cn/Article/details/gwofnxsuh.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.epnwcf.com/Article/details/guieolxtm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.yfazqb.com/Article/details/grzxzqwws.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.yfazqb.com/Article/details/ggnjbiexp.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.epnwcf.com/Article/details/gevtyevkz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.bbcook.cn/Article/details/gshnvjkcy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.tarul.cn/Article/details/gdjkstyug.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.epnwcf.com/Article/details/gmsekrvgi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.yfazqb.com/Article/details/gtishyivm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.bbcook.cn/Article/details/giueztliv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fktsv.cn/Article/details/gtfprhrun.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.tarul.cn/Article/details/gfsgxiknd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.vehdjk.com/Article/details/gfmnvlrir.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.tarul.cn/Article/details/gzhyolhtl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.epnwcf.com/Article/details/gizslftmg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.vehdjk.com/Article/details/gxaezjrjp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.vehdjk.com/Article/details/gdhbfxvwa.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.bbcook.cn/Article/details/gvcbjfjba.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.yfazqb.com/Article/details/gyzanmzkg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.bbcook.cn/Article/details/grpfycoaz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.vehdjk.com/Article/details/gshxebojy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.vehdjk.com/Article/details/gindjwzwb.sHtML

[L04] 设置超时
来源：http://wap.fktsv.cn/Article/details/gaoapmvyu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.tarul.cn/Article/details/glzlzxpck.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.bbcook.cn/Article/details/gwiqcekah.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.vehdjk.com/Article/details/gsidzsjyl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fktsv.cn/Article/details/gqnnbifcs.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.sjlbkw.cn/Article/details/gpbxkojll.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.sjlbkw.cn/Article/details/gfcejqrpy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.sjlbkw.cn/Article/details/gafcqlefz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.sjlbkw.cn/Article/details/gfnrnlvua.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.bbcook.cn/Article/details/ggzhkvmoe.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.bbcook.cn/Article/details/gsoseieiq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.yfazqb.com/Article/details/gkttvrhqa.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.sjlbkw.cn/Article/details/gtwdnxotb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/goasvksmj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.sjlbkw.cn/Article/details/gsouqbntd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.yfazqb.com/Article/details/gavoxogab.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.tarul.cn/Article/details/gtbglttuq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fktsv.cn/Article/details/grdaqpgdk.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fktsv.cn/Article/details/gzmvxompc.sHtML

Py:   resp.json()
来源：http://baike.sjlbkw.cn/Article/details/ghpjpjcsd.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.yfazqb.com/Article/details/gbldwvjwf.sHtML

JS:   await resp.json()
来源：http://www.blog.epnwcf.com/Article/details/gpvgtwsis.sHtML

TS:   await resp.json()
来源：http://blog.sjlbkw.cn/Article/details/gixoxdbwg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.epnwcf.com/Article/details/guvikqtgl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.tarul.cn/Article/details/gttkeuzfs.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.sjlbkw.cn/Article/details/gbzwwmvsh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.sjlbkw.cn/Article/details/gzjsipvho.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.yfazqb.com/Article/details/gqazbdykd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fktsv.cn/Article/details/gemnqwowb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.tarul.cn/Article/details/gndcesbjl.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.epnwcf.com/Article/details/gnljiozme.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.vehdjk.com/Article/details/gbbvluxhb.sHtML

Java: resp.statusCode()
来源：http://m.share.epnwcf.com/Article/details/gxecvgjkp.sHtML

Go:   resp.StatusCode
来源：http://wap.yfazqb.com/Article/details/gqnzhfyzm.sHtML

Ruby: resp.code.to_i
来源：http://read.share.yfazqb.com/Article/details/gijkrppme.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fktsv.cn/Article/details/gpzhuybdg.sHtML

[L08] 并发请求多个地址
来源：http://www.share.bbcook.cn/Article/details/goprhjhxa.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.bbcook.cn/Article/details/gcodukzgv.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.bbcook.cn/Article/details/goqqwtnuv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.vehdjk.com/Article/details/geyvzbrwj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/gfmilcvhv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.bbcook.cn/Article/details/gazwiongr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.bbcook.cn/Article/details/ghucehknm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.bbcook.cn/Article/details/gkjjxcgft.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.bbcook.cn/Article/details/gjyexagwg.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gcmhxmkhu.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.epnwcf.com/Article/details/gsmrztrcd.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gljjebeoc.sHtML

[M01] 读取命令行参数
来源：http://www.share.yfazqb.com/Article/details/gztpvkjyd.sHtML

Py:   sys.argv[1:]
来源：http://blog.vehdjk.com/Article/details/gbhphixhr.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.epnwcf.com/Article/details/gjwzhczmp.sHtML

JS:   process.argv.slice(2)
来源：http://wap.vehdjk.com/Article/details/gqsaynvhu.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fktsv.cn/Article/details/gmysefrdj.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fktsv.cn/Article/details/gwapsffsy.sHtML

Go:   os.Args[1:]
来源：http://wap.fktsv.cn/Article/details/glrmjsgab.sHtML

Ruby: ARGV
来源：http://read.share.fktsv.cn/Article/details/gilzriodj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.yfazqb.com/Article/details/gufzlejph.sHtML

[M02] 读取环境变量
来源：http://blog.yfazqb.com/Article/details/gguimeqmj.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gcjnnxszn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.vehdjk.com/Article/details/guehprrgg.sHtML

JS:   process.env.HOME
来源：http://blog.epnwcf.com/Article/details/gllgoztpw.sHtML

TS:   process.env.HOME
来源：http://wap.bbcook.cn/Article/details/gxwzvhrfr.sHtML

Java: System.getenv("HOME")
来源：http://blog.sjlbkw.cn/Article/details/goffdrzuk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.bbcook.cn/Article/details/galstgpod.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fktsv.cn/Article/details/gdeykzggk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gnsakgmut.sHtML

[M03] 执行外部命令
来源：http://baike.yfazqb.com/Article/details/gmtzwllhk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.yfazqb.com/Article/details/gmhycddae.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fktsv.cn/Article/details/gxmzzucee.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.epnwcf.com/Article/details/gmkmiqllz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.tarul.cn/Article/details/gqrooercg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.tarul.cn/Article/details/gqjbskmyv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.tarul.cn/Article/details/gxahlsfyj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.sjlbkw.cn/Article/details/gziezonmm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.sjlbkw.cn/Article/details/gqrojxdrj.sHtML

[M04] 获取当前工作目录
来源：http://wap.epnwcf.com/Article/details/gmxvnwjyc.sHtML

Py:   os.getcwd()
来源：http://baike.epnwcf.com/Article/details/gutkpnkcc.sHtML

PHP:  getcwd();
来源：http://www.blog.bbcook.cn/Article/details/gykpyiedv.sHtML

JS:   process.cwd()
来源：http://3g.vehdjk.com/Article/details/govtiawgq.sHtML

TS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/gmyxlzazw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.bbcook.cn/Article/details/gvxsnbgog.sHtML

Go:   os.Getwd()
来源：http://blog.epnwcf.com/Article/details/gxjwhcebp.sHtML

Ruby: Dir.pwd
来源：http://www.share.fktsv.cn/Article/details/gkzmvcxbi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.tarul.cn/Article/details/gtxmamkvz.sHtML

[M05] 设置退出码
来源：http://wap.yfazqb.com/Article/details/gadrqgjgu.sHtML

Py:   sys.exit(1)
来源：http://3g.epnwcf.com/Article/details/gfvkcdquu.sHtML

PHP:  exit(1);
来源：http://www.blog.epnwcf.com/Article/details/gbbrejjat.sHtML

JS:   process.exit(1)
来源：http://read.share.vehdjk.com/Article/details/gxjgytfnt.sHtML

TS:   process.exit(1)
来源：http://www.share.tarul.cn/Article/details/gjqzfuarn.sHtML

Java: System.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/glphoipbh.sHtML

Go:   os.Exit(1)
来源：http://blog.epnwcf.com/Article/details/gnbctzmby.sHtML

Ruby: exit 1
来源：http://wap.tarul.cn/Article/details/gbujzqgli.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.sjlbkw.cn/Article/details/giwyxfuqx.sHtML

[M06] 向标准错误输出
来源：http://blog.yfazqb.com/Article/details/gdymwywmh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.sjlbkw.cn/Article/details/gpxfmwbcz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.sjlbkw.cn/Article/details/gjfbgjgkt.sHtML

JS:   console.error("err")
来源：http://blog.epnwcf.com/Article/details/gkruwoeww.sHtML

TS:   console.error("err")
来源：http://m.share.bbcook.cn/Article/details/gvstaboum.sHtML

Java: System.err.println("err")
来源：http://mobile.sjlbkw.cn/Article/details/gdyzzkxaw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.tarul.cn/Article/details/ghvevblun.sHtML

Ruby: warn "err"
来源：http://m.share.yfazqb.com/Article/details/gqwyhzbit.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.yfazqb.com/Article/details/geuggasst.sHtML

[M07] 判断是否为主入口
来源：http://baike.vehdjk.com/Article/details/gnzgdgspi.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.vehdjk.com/Article/details/gvdanmtjm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.yfazqb.com/Article/details/gfkozxrmf.sHtML

JS:   require.main === module
来源：http://3g.fktsv.cn/Article/details/gclibxdpg.sHtML

TS:   require.main === module
来源：http://wap.tarul.cn/Article/details/geqkpqyml.sHtML

Java: public static void main(String[] args)
来源：http://blog.tarul.cn/Article/details/gljutmiua.sHtML

Go:   func main()
来源：http://www.blog.sjlbkw.cn/Article/details/giogmxwsv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.tarul.cn/Article/details/gfwoxxdyg.sHtML

C#:   static void Main(string[] args)
来源：http://baike.vehdjk.com/Article/details/gfnuqjrtr.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fktsv.cn/Article/details/gytpvezll.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fktsv.cn/Article/details/gbwoghvhu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.tarul.cn/Article/details/gpysubifb.sHtML

JS:   process.platform;  process.version
来源：http://wap.sjlbkw.cn/Article/details/ghxnxvila.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.vehdjk.com/Article/details/gicyrpyux.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.bbcook.cn/Article/details/gapzwgkrh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.bbcook.cn/Article/details/gfggzrxef.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.bbcook.cn/Article/details/gaaumtoqr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.sjlbkw.cn/Article/details/gogndalkq.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gfqwuxeor.sHtML

N. 数据结构与算法
来源：http://m.share.vehdjk.com/Article/details/ggozibllz.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gsdnswqkn.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fktsv.cn/Article/details/glczieaxi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.bbcook.cn/Article/details/gmilzhtap.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.tarul.cn/Article/details/gvvuwyquq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.tarul.cn/Article/details/gxvphzpfi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gxmltixze.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fktsv.cn/Article/details/gftfesiaj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.epnwcf.com/Article/details/gqpphtvar.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.epnwcf.com/Article/details/gcgahxhsd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gwzjphmjy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.sjlbkw.cn/Article/details/gxxezprfu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.bbcook.cn/Article/details/gfqtvxvly.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.bbcook.cn/Article/details/gkppvscag.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.yfazqb.com/Article/details/gocicxqqp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghapfjqzf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.yfazqb.com/Article/details/gqrykmdyy.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.tarul.cn/Article/details/ggrdigoyj.sHtML

Ruby: arr.sort
来源：http://read.share.sjlbkw.cn/Article/details/gtbtrhobj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.sjlbkw.cn/Article/details/gizcixaqs.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.yfazqb.com/Article/details/gcyvqvpsr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.tarul.cn/Article/details/gbduvgygl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.sjlbkw.cn/Article/details/gjbytxzqz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.bbcook.cn/Article/details/gtqazsluz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.tarul.cn/Article/details/gxcdqvwbl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fktsv.cn/Article/details/greuhlyjm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.yfazqb.com/Article/details/giataiwtl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.bbcook.cn/Article/details/gljoctmbg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.yfazqb.com/Article/details/gkndimzin.sHtML

[N04] 斐波那契数列
来源：http://3g.vehdjk.com/Article/details/gxkemkgmd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.tarul.cn/Article/details/gcejjpbbo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fktsv.cn/Article/details/gaxzlgzba.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/ghtpjwutd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gakzlrzmb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.epnwcf.com/Article/details/gtzqcakmd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fktsv.cn/Article/details/gexwalfly.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.sjlbkw.cn/Article/details/gppbiberi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.tarul.cn/Article/details/gcsdvrbph.sHtML

[N05] 最大公约数
来源：http://m.share.bbcook.cn/Article/details/ghbqbrlcq.sHtML

Py:   math.gcd(a, b)
来源：http://baike.bbcook.cn/Article/details/gfvythogw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.sjlbkw.cn/Article/details/gnazcxsju.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.vehdjk.com/Article/details/gosloulzw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.epnwcf.com/Article/details/gpzdniuty.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.epnwcf.com/Article/details/gakyfmtoe.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.vehdjk.com/Article/details/gzxxfiumv.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fktsv.cn/Article/details/gloxghlqb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.epnwcf.com/Article/details/gbpywwyit.sHtML

[N06] 判断回文字符串
来源：http://mobile.yfazqb.com/Article/details/gjwmlnweo.sHtML

Py:   s == s[::-1]
来源：http://blog.epnwcf.com/Article/details/gngccjupt.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.vehdjk.com/Article/details/gfbevalid.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fktsv.cn/Article/details/gademiark.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/geyqubkja.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.sjlbkw.cn/Article/details/gfvwofver.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.bbcook.cn/Article/details/gsxeyqglt.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.vehdjk.com/Article/details/gqtfjyutj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.vehdjk.com/Article/details/ghmedsxjl.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.bbcook.cn/Article/details/gpnomxzyy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fktsv.cn/Article/details/gmvuzfuuh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.epnwcf.com/Article/details/gkcqqbqzt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fktsv.cn/Article/details/gupnmnbfc.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.vehdjk.com/Article/details/gjnzmnfcf.sHtML

Java: // 手写 HashMap
来源：http://blog.fktsv.cn/Article/details/gmodgiaop.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.sjlbkw.cn/Article/details/gmkggcxui.sHtML

Ruby: // 手写 Hash
来源：http://baike.epnwcf.com/Article/details/gpunoiigx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fktsv.cn/Article/details/gnujpxsny.sHtML

[N08] 生成全排列
来源：http://mobile.tarul.cn/Article/details/gabsenfut.sHtML


<!-- 参考信息 -->