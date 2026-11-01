代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.epnwcf.com/Article/details/ggcbcwhde.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.bbcook.cn/Article/details/ghiaszjdd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.vehdjk.com/Article/details/ghbtfjagc.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.epnwcf.com/Article/details/gebymgpqw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.vehdjk.com/Article/details/glrtyltms.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.vehdjk.com/Article/details/gggmkriqv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.epnwcf.com/Article/details/gmuaajvsz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.vehdjk.com/Article/details/gfwvxpehx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.tarul.cn/Article/details/gwupnxgxb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.bbcook.cn/Article/details/grepycuaq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.vehdjk.com/Article/details/guelvrfar.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.vehdjk.com/Article/details/gfhkcvsau.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gptgjgsov.sHtML

K. JSON 与序列化
来源：http://blog.fktsv.cn/Article/details/gemifbmgs.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gqbxylpsu.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.vehdjk.com/Article/details/gxaapycew.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.tarul.cn/Article/details/glanhkusc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.epnwcf.com/Article/details/gpdcajuuj.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gjccjwcgq.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.bbcook.cn/Article/details/gpcbzxbkk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.yfazqb.com/Article/details/gddrdfqgd.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.yfazqb.com/Article/details/glasfuvkd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fktsv.cn/Article/details/gtggcpdmt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.yfazqb.com/Article/details/grunazkzw.sHtML

[K02] JSON 字符串转对象
来源：http://baike.vehdjk.com/Article/details/grkrpvazr.sHtML

Py:   json.loads(s)
来源：http://www.share.vehdjk.com/Article/details/giwboldqg.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fktsv.cn/Article/details/gnhgcrpgi.sHtML

JS:   JSON.parse(s)
来源：http://3g.tarul.cn/Article/details/gzdyqeuit.sHtML

TS:   JSON.parse(s)
来源：http://wap.vehdjk.com/Article/details/glokncyzg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/gmyzqpzuo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.tarul.cn/Article/details/gxxdoyodp.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.tarul.cn/Article/details/glvxnxssa.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.bbcook.cn/Article/details/gthzzjizb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.sjlbkw.cn/Article/details/gvsgdnboa.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fktsv.cn/Article/details/ggcnwzhif.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.epnwcf.com/Article/details/gbnjzezaf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.epnwcf.com/Article/details/gqgeskahb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.epnwcf.com/Article/details/gmwoibytc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.vehdjk.com/Article/details/gjztkqmmq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.tarul.cn/Article/details/gojpeledj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.bbcook.cn/Article/details/gohwkdabz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.yfazqb.com/Article/details/ggmujemxu.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fktsv.cn/Article/details/gfdwdgchv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.vehdjk.com/Article/details/gqemuzcgm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.vehdjk.com/Article/details/gjqbqushh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.sjlbkw.cn/Article/details/gxpckzgpa.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.yfazqb.com/Article/details/gkucejgyf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.tarul.cn/Article/details/gkqrozode.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fktsv.cn/Article/details/gjajwhquk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.sjlbkw.cn/Article/details/ganzxdjvf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fktsv.cn/Article/details/gneaqhpcn.sHtML

[K05] 深拷贝对象
来源：http://www.blog.yfazqb.com/Article/details/gcaxkxaue.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fktsv.cn/Article/details/gfvdspttt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.tarul.cn/Article/details/gkknetuhm.sHtML

JS:   structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/glnyrreun.sHtML

TS:   structuredClone(obj)
来源：http://3g.sjlbkw.cn/Article/details/gwmpaaktl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.bbcook.cn/Article/details/geydxzied.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.tarul.cn/Article/details/gmactyyjm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.yfazqb.com/Article/details/gvnzkcaft.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.epnwcf.com/Article/details/guazyhwoc.sHtML

[K06] 解析 URL 查询串
来源：http://wap.vehdjk.com/Article/details/ggrnhwsby.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fktsv.cn/Article/details/gjxepaggi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.epnwcf.com/Article/details/gzddprzjo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.vehdjk.com/Article/details/gusrfvgvz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.sjlbkw.cn/Article/details/gkcttxuqr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.bbcook.cn/Article/details/gzbnjilev.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.vehdjk.com/Article/details/gmnquzrfy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.sjlbkw.cn/Article/details/gvshparfa.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.sjlbkw.cn/Article/details/gynbsvpsg.sHtML

[K07] 进制转换
来源：http://www.m.share.vehdjk.com/Article/details/gwckiasgf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gccarggtk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fktsv.cn/Article/details/gxvxzjomc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.yfazqb.com/Article/details/ggiyhwlfy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gwcnarons.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gnlngdraw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.epnwcf.com/Article/details/ginwvitup.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.bbcook.cn/Article/details/gfzjsnhum.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gypwlckdm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.vehdjk.com/Article/details/gzoqahika.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.sjlbkw.cn/Article/details/ggbqtoiya.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fktsv.cn/Article/details/ggmwvlmog.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.tarul.cn/Article/details/gherqwwka.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.vehdjk.com/Article/details/gnkzpavja.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.epnwcf.com/Article/details/gvaetlqbh.sHtML

Go:   encoding/gob
来源：http://wap.fktsv.cn/Article/details/grebecqmy.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.tarul.cn/Article/details/gvyfuchpk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fktsv.cn/Article/details/ggcqfsvfe.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gixmhsuyk.sHtML

L. 网络请求
来源：http://read.share.fktsv.cn/Article/details/gnpbvxbzy.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/glqvfuuxh.sHtML

[L01] 发送 GET 请求
来源：http://blog.fktsv.cn/Article/details/gbngxzkiv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.yfazqb.com/Article/details/gnesrovaw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.sjlbkw.cn/Article/details/gdwnavkxc.sHtML

JS:   await fetch(url)
来源：http://read.share.vehdjk.com/Article/details/ghealrcjb.sHtML

TS:   await fetch(url)
来源：http://www.blog.epnwcf.com/Article/details/gkegqbppf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.vehdjk.com/Article/details/gefkscqli.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.vehdjk.com/Article/details/gmaaarobg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.yfazqb.com/Article/details/glggwtwge.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fktsv.cn/Article/details/gtbohkkky.sHtML

[L02] 发送 POST JSON
来源：http://blog.epnwcf.com/Article/details/gtdrpmnen.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fktsv.cn/Article/details/ghbjpndoz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.tarul.cn/Article/details/giwnkpgln.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.yfazqb.com/Article/details/grhluilvz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.bbcook.cn/Article/details/ggpvsnudh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.tarul.cn/Article/details/gsqkuwozz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.vehdjk.com/Article/details/ggouhyfac.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.bbcook.cn/Article/details/gselqhdll.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.yfazqb.com/Article/details/gzzycjrxu.sHtML

[L03] 设置自定义请求头
来源：http://wap.vehdjk.com/Article/details/gpgknpsdf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.yfazqb.com/Article/details/gdondfedi.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.epnwcf.com/Article/details/gkijeybqf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fktsv.cn/Article/details/gjdqabnfo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.vehdjk.com/Article/details/gpqoitfzw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.sjlbkw.cn/Article/details/gbkgobdmx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fktsv.cn/Article/details/giluccbni.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.bbcook.cn/Article/details/gydoyreff.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.tarul.cn/Article/details/gtmvmsjqd.sHtML

[L04] 设置超时
来源：http://read.share.sjlbkw.cn/Article/details/gignunecv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fktsv.cn/Article/details/gfzjzcxgz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.bbcook.cn/Article/details/gqukpdzno.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.epnwcf.com/Article/details/gwgftcebk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.bbcook.cn/Article/details/gqyqozzxj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.sjlbkw.cn/Article/details/gzxdfwagp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.bbcook.cn/Article/details/gzciaznno.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.yfazqb.com/Article/details/gwlltvvih.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.tarul.cn/Article/details/gyttrsrkt.sHtML

[L05] 上传文件（multipart）
来源：http://baike.tarul.cn/Article/details/grwmpaswa.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzinjhwg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fktsv.cn/Article/details/gaxncdwju.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.yfazqb.com/Article/details/gkfdltbqh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.sjlbkw.cn/Article/details/gfyvkokwc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.bbcook.cn/Article/details/grqjuwyyd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.bbcook.cn/Article/details/gfwlesxxy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fktsv.cn/Article/details/gwuchvyvf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.vehdjk.com/Article/details/gfetcaxke.sHtML

[L06] 解析响应为 JSON
来源：http://3g.tarul.cn/Article/details/gzhniszmn.sHtML

Py:   resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/gumnnnqaq.sHtML

PHP:  json_decode($body, true);
来源：http://baike.vehdjk.com/Article/details/glsbbyrlv.sHtML

JS:   await resp.json()
来源：http://read.share.bbcook.cn/Article/details/gucdvlgiy.sHtML

TS:   await resp.json()
来源：http://m.share.fktsv.cn/Article/details/gpbhnkfnm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.sjlbkw.cn/Article/details/glmdpbhpf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.yfazqb.com/Article/details/geujhgjbq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.epnwcf.com/Article/details/gykubylcy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.epnwcf.com/Article/details/ggxlyeqre.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.sjlbkw.cn/Article/details/ggxhpvwvx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.yfazqb.com/Article/details/gvldmaxam.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.epnwcf.com/Article/details/gagzyyqgs.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.bbcook.cn/Article/details/goqgjeovv.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.bbcook.cn/Article/details/gxxxckpfv.sHtML

Java: resp.statusCode()
来源：http://www.m.share.bbcook.cn/Article/details/gxwpyviwv.sHtML

Go:   resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/grrwvioyw.sHtML

Ruby: resp.code.to_i
来源：http://3g.tarul.cn/Article/details/gkblwjdcd.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.sjlbkw.cn/Article/details/gnsaaqcfm.sHtML

[L08] 并发请求多个地址
来源：http://wap.fktsv.cn/Article/details/gvjmmkmkz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fktsv.cn/Article/details/gwhuvvczt.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fktsv.cn/Article/details/gnpbfxnqf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/gjsiyoqgf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.sjlbkw.cn/Article/details/ghsnosorb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.sjlbkw.cn/Article/details/gaguvdtmw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.vehdjk.com/Article/details/gzlqefhjw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.yfazqb.com/Article/details/gnnoltvxn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.bbcook.cn/Article/details/gayctuptg.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gnklqdalf.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.sjlbkw.cn/Article/details/gxakbndjr.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gtzphgnqh.sHtML

[M01] 读取命令行参数
来源：http://m.share.vehdjk.com/Article/details/grrvbguxu.sHtML

Py:   sys.argv[1:]
来源：http://3g.fktsv.cn/Article/details/gtxzhbkqh.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.vehdjk.com/Article/details/gerxxnuhb.sHtML

JS:   process.argv.slice(2)
来源：http://3g.tarul.cn/Article/details/gqzciaqal.sHtML

TS:   process.argv.slice(2)
来源：http://wap.vehdjk.com/Article/details/gkizzqlto.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.sjlbkw.cn/Article/details/grmkctjfu.sHtML

Go:   os.Args[1:]
来源：http://m.share.sjlbkw.cn/Article/details/guzcdnfsj.sHtML

Ruby: ARGV
来源：http://www.share.fktsv.cn/Article/details/gunblqwje.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.sjlbkw.cn/Article/details/gnemhhavh.sHtML

[M02] 读取环境变量
来源：http://baike.epnwcf.com/Article/details/gqpdwsqjs.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fktsv.cn/Article/details/gggvpeqvz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.tarul.cn/Article/details/gmslffsxl.sHtML

JS:   process.env.HOME
来源：http://www.blog.yfazqb.com/Article/details/gytutizha.sHtML

TS:   process.env.HOME
来源：http://baike.tarul.cn/Article/details/gjqoiusli.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fktsv.cn/Article/details/gbhthgnwg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtzkcoul.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.tarul.cn/Article/details/gcschulwg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fktsv.cn/Article/details/gddlxezga.sHtML

[M03] 执行外部命令
来源：http://m.share.bbcook.cn/Article/details/gxrstoetu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghlenjzjf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.bbcook.cn/Article/details/ggbuybdbb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.tarul.cn/Article/details/gnvewlert.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.epnwcf.com/Article/details/glmnthxhd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.yfazqb.com/Article/details/gdjqjuvut.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.tarul.cn/Article/details/gctcxyhha.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.bbcook.cn/Article/details/gpiitivgg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.sjlbkw.cn/Article/details/gedtjbpgh.sHtML

[M04] 获取当前工作目录
来源：http://www.share.sjlbkw.cn/Article/details/guywdatwa.sHtML

Py:   os.getcwd()
来源：http://www.blog.sjlbkw.cn/Article/details/gdlrfxhdu.sHtML

PHP:  getcwd();
来源：http://3g.fktsv.cn/Article/details/gujqayeey.sHtML

JS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/gnwyknkyl.sHtML

TS:   process.cwd()
来源：http://baike.epnwcf.com/Article/details/glztterof.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.bbcook.cn/Article/details/gncjeavcr.sHtML

Go:   os.Getwd()
来源：http://mobile.tarul.cn/Article/details/gbsyfhlau.sHtML

Ruby: Dir.pwd
来源：http://www.share.tarul.cn/Article/details/gifetagbr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.bbcook.cn/Article/details/gcqomyura.sHtML

[M05] 设置退出码
来源：http://www.m.share.epnwcf.com/Article/details/gspfkrdsu.sHtML

Py:   sys.exit(1)
来源：http://blog.epnwcf.com/Article/details/grpadkuht.sHtML

PHP:  exit(1);
来源：http://m.share.vehdjk.com/Article/details/gtvrtbgbr.sHtML

JS:   process.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gaxqrbhpe.sHtML

TS:   process.exit(1)
来源：http://wap.epnwcf.com/Article/details/gjigctdyg.sHtML

Java: System.exit(1)
来源：http://3g.fktsv.cn/Article/details/gwfaovbic.sHtML

Go:   os.Exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gzcbgqdyg.sHtML

Ruby: exit 1
来源：http://read.share.yfazqb.com/Article/details/gwusrzrhz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.bbcook.cn/Article/details/gzzlxqqca.sHtML

[M06] 向标准错误输出
来源：http://m.share.bbcook.cn/Article/details/ghqzigqxc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fktsv.cn/Article/details/gkzhmfwbv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.bbcook.cn/Article/details/gojwqazir.sHtML

JS:   console.error("err")
来源：http://m.share.vehdjk.com/Article/details/gkqxjmytl.sHtML

TS:   console.error("err")
来源：http://read.share.bbcook.cn/Article/details/gtmhwsdeq.sHtML

Java: System.err.println("err")
来源：http://www.m.share.bbcook.cn/Article/details/gbyetesng.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.epnwcf.com/Article/details/gwhmpfbro.sHtML

Ruby: warn "err"
来源：http://baike.yfazqb.com/Article/details/gickshyxl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.vehdjk.com/Article/details/gpjqqtoyr.sHtML

[M07] 判断是否为主入口
来源：http://baike.epnwcf.com/Article/details/gynhqjply.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fktsv.cn/Article/details/gawbxubzx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.yfazqb.com/Article/details/ghjcittua.sHtML

JS:   require.main === module
来源：http://3g.bbcook.cn/Article/details/gidxewhhx.sHtML

TS:   require.main === module
来源：http://www.blog.tarul.cn/Article/details/gohfphade.sHtML

Java: public static void main(String[] args)
来源：http://3g.vehdjk.com/Article/details/gwrzytdbv.sHtML

Go:   func main()
来源：http://read.share.sjlbkw.cn/Article/details/gvvapqwft.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.epnwcf.com/Article/details/gakklpxrc.sHtML

C#:   static void Main(string[] args)
来源：http://baike.bbcook.cn/Article/details/ghhjwfmxy.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.epnwcf.com/Article/details/gnffnklbu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.bbcook.cn/Article/details/gbghwmlff.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.tarul.cn/Article/details/gengysxfr.sHtML

JS:   process.platform;  process.version
来源：http://baike.vehdjk.com/Article/details/gzinjrxzo.sHtML

TS:   process.platform;  process.version
来源：http://3g.fktsv.cn/Article/details/gyktbgbch.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.sjlbkw.cn/Article/details/ggnlihjji.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.sjlbkw.cn/Article/details/golcximvp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.tarul.cn/Article/details/gsfltwgyo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.bbcook.cn/Article/details/gynbixjtz.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gquzctzht.sHtML

N. 数据结构与算法
来源：http://www.share.bbcook.cn/Article/details/gesglbtiz.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gkwfhcjmk.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.epnwcf.com/Article/details/grsmyqdzj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.epnwcf.com/Article/details/gxnysemjz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.bbcook.cn/Article/details/gxlyoapao.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gobywpxfc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fktsv.cn/Article/details/gdtyzcrvz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fktsv.cn/Article/details/gbtzliaku.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fktsv.cn/Article/details/ggtmpbmsy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.vehdjk.com/Article/details/gxvfscgqc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fktsv.cn/Article/details/ggkhfugci.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.bbcook.cn/Article/details/gocbqdizc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.bbcook.cn/Article/details/gkerztthy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.tarul.cn/Article/details/gzeposjwb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.epnwcf.com/Article/details/gecjcijrr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.bbcook.cn/Article/details/gkhjwuywc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.bbcook.cn/Article/details/gkqorzaus.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fktsv.cn/Article/details/gjkmvlvse.sHtML

Ruby: arr.sort
来源：http://www.blog.sjlbkw.cn/Article/details/gqboeivyn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.epnwcf.com/Article/details/glpgiwlka.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.sjlbkw.cn/Article/details/gedztuokv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.bbcook.cn/Article/details/goqpjlfta.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.bbcook.cn/Article/details/gtjnzvxzs.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.sjlbkw.cn/Article/details/glbkdhmgf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.tarul.cn/Article/details/gvwkkiebj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.tarul.cn/Article/details/gpuxoeezq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.vehdjk.com/Article/details/grfqtvsdw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.bbcook.cn/Article/details/godgvxboz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fktsv.cn/Article/details/gpfgandlk.sHtML

[N04] 斐波那契数列
来源：http://baike.tarul.cn/Article/details/gjxfevxfg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.yfazqb.com/Article/details/gerubdiru.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.bbcook.cn/Article/details/grdsiezba.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.vehdjk.com/Article/details/gttabmfcm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.tarul.cn/Article/details/gtjupxuwy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.sjlbkw.cn/Article/details/gbhczippt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fktsv.cn/Article/details/goudmcoew.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.bbcook.cn/Article/details/gddfcyqdq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.sjlbkw.cn/Article/details/gwfcgrjeo.sHtML

[N05] 最大公约数
来源：http://m.share.epnwcf.com/Article/details/gihgiynvo.sHtML

Py:   math.gcd(a, b)
来源：http://baike.epnwcf.com/Article/details/gxqipjrny.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.vehdjk.com/Article/details/gsutgvaxj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fktsv.cn/Article/details/genswxdkj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.bbcook.cn/Article/details/gvmpkdidn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.vehdjk.com/Article/details/gjxhrdvvn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.yfazqb.com/Article/details/gpnmokqml.sHtML

Ruby: a.gcd(b)
来源：http://baike.tarul.cn/Article/details/gjdzvbaje.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.sjlbkw.cn/Article/details/gjeemoysh.sHtML

[N06] 判断回文字符串
来源：http://m.share.sjlbkw.cn/Article/details/gyvnptwhl.sHtML

Py:   s == s[::-1]
来源：http://baike.tarul.cn/Article/details/guvyshgrh.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.vehdjk.com/Article/details/gvnbvkazb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gjwthuugx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/glymnnkrg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.sjlbkw.cn/Article/details/gwclxweui.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.bbcook.cn/Article/details/gvcnfwmwt.sHtML

Ruby: s == s.reverse
来源：http://3g.epnwcf.com/Article/details/ggdyhanfx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.tarul.cn/Article/details/gcaepjmgx.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.epnwcf.com/Article/details/gihdzttzt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fktsv.cn/Article/details/gsmonoqpk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.yfazqb.com/Article/details/gskegfkql.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.vehdjk.com/Article/details/gwijzkqwl.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.tarul.cn/Article/details/gwqiovtaz.sHtML

Java: // 手写 HashMap
来源：http://blog.sjlbkw.cn/Article/details/ggtbibuvr.sHtML


<!-- 参考信息 -->