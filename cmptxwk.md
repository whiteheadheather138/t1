代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.vehdjk.com/Article/details/gjbcakyih.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.vehdjk.com/Article/details/gpzjjbjju.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.tarul.cn/Article/details/gzimlixcr.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.tarul.cn/Article/details/gpsggixfu.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.sjlbkw.cn/Article/details/gwvnkuceh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.yfazqb.com/Article/details/gwaqjibss.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.yfazqb.com/Article/details/gghicphaf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.tarul.cn/Article/details/gwyefpqxw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.epnwcf.com/Article/details/gsvyykbci.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.epnwcf.com/Article/details/gypazqqwf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.sjlbkw.cn/Article/details/ghfsjikto.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.yfazqb.com/Article/details/gvpannwfo.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gxcmnvaew.sHtML

K. JSON 与序列化
来源：http://www.m.share.bbcook.cn/Article/details/gylxfhzpc.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gnemlxwlh.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.yfazqb.com/Article/details/gusqferrs.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.tarul.cn/Article/details/gsiqffvzc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgvryiys.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.yfazqb.com/Article/details/gmdtvnhzr.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.vehdjk.com/Article/details/gewbeqsge.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.bbcook.cn/Article/details/gzfmhdlbx.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fktsv.cn/Article/details/gqbvgsqib.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.epnwcf.com/Article/details/guqqxktfj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.yfazqb.com/Article/details/gitgbtmzq.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.epnwcf.com/Article/details/gyhpgmnsi.sHtML

Py:   json.loads(s)
来源：http://baike.yfazqb.com/Article/details/gjdoerimm.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.fktsv.cn/Article/details/gjxteyqvt.sHtML

JS:   JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/gtidkbvsp.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.yfazqb.com/Article/details/godyujdaj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fktsv.cn/Article/details/gyylbbwak.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.tarul.cn/Article/details/gffxukvof.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fktsv.cn/Article/details/gifpmqmwt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.sjlbkw.cn/Article/details/gcycaykwj.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.sjlbkw.cn/Article/details/gicrojsjw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.vehdjk.com/Article/details/gedbrjaxf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.bbcook.cn/Article/details/grstwryna.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.yfazqb.com/Article/details/gshdwtior.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.yfazqb.com/Article/details/grnutvvdp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.yfazqb.com/Article/details/gnfbawhkb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fktsv.cn/Article/details/gahrqehyg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.yfazqb.com/Article/details/gniewwhat.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.vehdjk.com/Article/details/gtcvcfisi.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.bbcook.cn/Article/details/glhkweoch.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.tarul.cn/Article/details/gbhvlqckk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.vehdjk.com/Article/details/gmercaikb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.tarul.cn/Article/details/gampwbhrz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fktsv.cn/Article/details/gjpaotcmn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.tarul.cn/Article/details/grcyiprty.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.vehdjk.com/Article/details/gcikwucsm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.sjlbkw.cn/Article/details/gaxtbxdlp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.tarul.cn/Article/details/gvmmbaoml.sHtML

[K05] 深拷贝对象
来源：http://m.share.epnwcf.com/Article/details/glsrokwue.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.tarul.cn/Article/details/gtxlwhbrr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.bbcook.cn/Article/details/gqivatrvw.sHtML

JS:   structuredClone(obj)
来源：http://read.share.epnwcf.com/Article/details/glpbifrlv.sHtML

TS:   structuredClone(obj)
来源：http://3g.sjlbkw.cn/Article/details/gxvkqyckz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.tarul.cn/Article/details/gsqycalwy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.sjlbkw.cn/Article/details/gleohrurw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.tarul.cn/Article/details/gqvzrhday.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fktsv.cn/Article/details/gfzumckri.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.vehdjk.com/Article/details/gqpzxdojs.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.sjlbkw.cn/Article/details/gupkqyjtd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.sjlbkw.cn/Article/details/gsfjsqwgx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.tarul.cn/Article/details/gvwfbepyq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.bbcook.cn/Article/details/gqpfxfwrd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.bbcook.cn/Article/details/gfihrhnak.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/guqziqrdw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxzdhoosk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.tarul.cn/Article/details/gotbvbkiq.sHtML

[K07] 进制转换
来源：http://baike.sjlbkw.cn/Article/details/gofrfahep.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.tarul.cn/Article/details/gmlcszknr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.sjlbkw.cn/Article/details/glwxcemvq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gxdvluvrq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gljvrxkbz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gawwbdvul.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.sjlbkw.cn/Article/details/gqxesgsin.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.yfazqb.com/Article/details/gwvrtzrth.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gjipjqucy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.bbcook.cn/Article/details/gcyzdnemz.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.bbcook.cn/Article/details/gzbsylktf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.bbcook.cn/Article/details/gmlmcwwkz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.bbcook.cn/Article/details/grsskglaf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.yfazqb.com/Article/details/gtejhujql.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fktsv.cn/Article/details/guwasufpo.sHtML

Go:   encoding/gob
来源：http://baike.vehdjk.com/Article/details/geviqwcsi.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.bbcook.cn/Article/details/goohjjqsg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.sjlbkw.cn/Article/details/gcuegzynf.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gekuegdbm.sHtML

L. 网络请求
来源：http://www.blog.sjlbkw.cn/Article/details/ggytsbtfe.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gdyhmvjzb.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.epnwcf.com/Article/details/guwhntmpg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.sjlbkw.cn/Article/details/gokkxbhen.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.sjlbkw.cn/Article/details/gsomacdvj.sHtML

JS:   await fetch(url)
来源：http://baike.tarul.cn/Article/details/geeiwvwuq.sHtML

TS:   await fetch(url)
来源：http://blog.fktsv.cn/Article/details/gwzfznyiw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.epnwcf.com/Article/details/gkoqnjust.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.epnwcf.com/Article/details/gptomwkls.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.vehdjk.com/Article/details/gtvfnvxhj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.yfazqb.com/Article/details/guuwgfnau.sHtML

[L02] 发送 POST JSON
来源：http://blog.bbcook.cn/Article/details/gyzojtxcp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.bbcook.cn/Article/details/gnrnmptac.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.epnwcf.com/Article/details/gzoaifsko.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.bbcook.cn/Article/details/gplddjivx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.epnwcf.com/Article/details/gdyfgcfkn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.yfazqb.com/Article/details/greyasaqt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fktsv.cn/Article/details/ggcwsfvuq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fktsv.cn/Article/details/gdmvqcnvq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.epnwcf.com/Article/details/glktczpbb.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.yfazqb.com/Article/details/gvsadzguf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.bbcook.cn/Article/details/guyvxgyvq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.tarul.cn/Article/details/gslmoqbyy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.vehdjk.com/Article/details/gbtofuqpk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.epnwcf.com/Article/details/gcsnyozoe.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.sjlbkw.cn/Article/details/ggaxjqmck.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.epnwcf.com/Article/details/gzvvfyxdm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.epnwcf.com/Article/details/gaukhhgbp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.vehdjk.com/Article/details/gvdwvkwot.sHtML

[L04] 设置超时
来源：http://mobile.bbcook.cn/Article/details/gjwwcwqql.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.tarul.cn/Article/details/gszeqqdrp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fktsv.cn/Article/details/gwttaovuz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.sjlbkw.cn/Article/details/guqtmjpiw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.vehdjk.com/Article/details/gyuxezgur.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fktsv.cn/Article/details/ghdzyayzd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.yfazqb.com/Article/details/gtsapdcfk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.bbcook.cn/Article/details/gnuuwinqc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.tarul.cn/Article/details/ghswzyhsb.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.sjlbkw.cn/Article/details/gfkknwkxj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fktsv.cn/Article/details/gqcidzkjr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.vehdjk.com/Article/details/gezmpqcyp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.tarul.cn/Article/details/gizthwdtf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.vehdjk.com/Article/details/gvvunyjyn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.tarul.cn/Article/details/guwvybime.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.sjlbkw.cn/Article/details/gcxqerqzt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.bbcook.cn/Article/details/geeyhdfep.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gvofrbjix.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.bbcook.cn/Article/details/gozangucx.sHtML

Py:   resp.json()
来源：http://3g.sjlbkw.cn/Article/details/gmnlfusqj.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.yfazqb.com/Article/details/ggghqbluh.sHtML

JS:   await resp.json()
来源：http://baike.yfazqb.com/Article/details/glxelzeep.sHtML

TS:   await resp.json()
来源：http://3g.epnwcf.com/Article/details/gmpuiuwkc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.yfazqb.com/Article/details/gwqxqkzjw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.epnwcf.com/Article/details/goxxkoadb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fktsv.cn/Article/details/gqebltejd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fktsv.cn/Article/details/gcwvvtouk.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.vehdjk.com/Article/details/gewypqvkc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fktsv.cn/Article/details/gbahxlqxl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.sjlbkw.cn/Article/details/gktmanlnd.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.yfazqb.com/Article/details/gpfxliynf.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fktsv.cn/Article/details/gkxwpxfnp.sHtML

Java: resp.statusCode()
来源：http://www.blog.vehdjk.com/Article/details/ghobzufze.sHtML

Go:   resp.StatusCode
来源：http://read.share.epnwcf.com/Article/details/gvhiwtkar.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.yfazqb.com/Article/details/gbiboeccy.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.tarul.cn/Article/details/gesaymvpz.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.bbcook.cn/Article/details/gkbwhcerd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.yfazqb.com/Article/details/gwlachtsg.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.epnwcf.com/Article/details/gsuyxqyex.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.vehdjk.com/Article/details/gpjsufbdv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fktsv.cn/Article/details/gojwbnjro.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.yfazqb.com/Article/details/gnfraflfn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fktsv.cn/Article/details/gjuudgycf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.bbcook.cn/Article/details/gyxwqyfny.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.bbcook.cn/Article/details/gyqjdibon.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/giltppxts.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fktsv.cn/Article/details/gzekliulb.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gvrjlrbbv.sHtML

[M01] 读取命令行参数
来源：http://read.share.epnwcf.com/Article/details/glpxsddyo.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.tarul.cn/Article/details/gerunkcva.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.epnwcf.com/Article/details/gjbsvttvz.sHtML

JS:   process.argv.slice(2)
来源：http://blog.yfazqb.com/Article/details/gyeofieie.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.yfazqb.com/Article/details/ghdyrlhxr.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fktsv.cn/Article/details/gondnjxef.sHtML

Go:   os.Args[1:]
来源：http://m.share.yfazqb.com/Article/details/geetpkvya.sHtML

Ruby: ARGV
来源：http://wap.sjlbkw.cn/Article/details/gkzaocpea.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.vehdjk.com/Article/details/gkrhdgxzc.sHtML

[M02] 读取环境变量
来源：http://www.share.yfazqb.com/Article/details/gjtacoyxv.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.vehdjk.com/Article/details/glelpeqwz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.tarul.cn/Article/details/glfncpbtt.sHtML

JS:   process.env.HOME
来源：http://www.m.share.yfazqb.com/Article/details/gwhupxmmz.sHtML

TS:   process.env.HOME
来源：http://3g.bbcook.cn/Article/details/gvfoppugp.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.bbcook.cn/Article/details/gxecheyup.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.tarul.cn/Article/details/ghtjwoygb.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.epnwcf.com/Article/details/gysgynftm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.epnwcf.com/Article/details/gkrfdvmrq.sHtML

[M03] 执行外部命令
来源：http://blog.sjlbkw.cn/Article/details/gwdzsqrym.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fktsv.cn/Article/details/grjmiaegc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.yfazqb.com/Article/details/gjtfdibir.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.bbcook.cn/Article/details/gkbjskqna.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.tarul.cn/Article/details/grlzaupdx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.tarul.cn/Article/details/gjuupcydz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.vehdjk.com/Article/details/gwdiwdlsf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.yfazqb.com/Article/details/glbdxjjyf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.epnwcf.com/Article/details/gmfhkvzgf.sHtML

[M04] 获取当前工作目录
来源：http://read.share.bbcook.cn/Article/details/ghabbrqvy.sHtML

Py:   os.getcwd()
来源：http://blog.yfazqb.com/Article/details/gdufmdfzi.sHtML

PHP:  getcwd();
来源：http://read.share.epnwcf.com/Article/details/glglmltkr.sHtML

JS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/gtjakhzoj.sHtML

TS:   process.cwd()
来源：http://www.share.yfazqb.com/Article/details/genwdkudb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fktsv.cn/Article/details/gqqvokdgo.sHtML

Go:   os.Getwd()
来源：http://wap.bbcook.cn/Article/details/guhxnhfkb.sHtML

Ruby: Dir.pwd
来源：http://3g.bbcook.cn/Article/details/gquikruur.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.vehdjk.com/Article/details/gftpzasbq.sHtML

[M05] 设置退出码
来源：http://blog.fktsv.cn/Article/details/gqbhyokhf.sHtML

Py:   sys.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gzdshnmrz.sHtML

PHP:  exit(1);
来源：http://www.m.share.bbcook.cn/Article/details/ghihyurax.sHtML

JS:   process.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcspkvodo.sHtML

TS:   process.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gzzxvtvqu.sHtML

Java: System.exit(1)
来源：http://blog.fktsv.cn/Article/details/gpcbsgxnq.sHtML

Go:   os.Exit(1)
来源：http://m.share.epnwcf.com/Article/details/gjjuhffik.sHtML

Ruby: exit 1
来源：http://read.share.epnwcf.com/Article/details/gumnzosbs.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.vehdjk.com/Article/details/gmqglpkco.sHtML

[M06] 向标准错误输出
来源：http://baike.sjlbkw.cn/Article/details/gbwqsplgo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fktsv.cn/Article/details/gcebpflvv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fktsv.cn/Article/details/goykqospp.sHtML

JS:   console.error("err")
来源：http://mobile.bbcook.cn/Article/details/gkbzhfvvr.sHtML

TS:   console.error("err")
来源：http://mobile.epnwcf.com/Article/details/gjjgwqkgi.sHtML

Java: System.err.println("err")
来源：http://www.blog.sjlbkw.cn/Article/details/gbbzghhvv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.tarul.cn/Article/details/glcxlrhyp.sHtML

Ruby: warn "err"
来源：http://wap.vehdjk.com/Article/details/gydbntzvf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.tarul.cn/Article/details/gpkmmvbqn.sHtML

[M07] 判断是否为主入口
来源：http://read.share.bbcook.cn/Article/details/gbdlhdjqb.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.tarul.cn/Article/details/gxvxbhslv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.sjlbkw.cn/Article/details/gpwbhannx.sHtML

JS:   require.main === module
来源：http://www.share.fktsv.cn/Article/details/gxenasdjz.sHtML

TS:   require.main === module
来源：http://www.blog.bbcook.cn/Article/details/gxnndpygv.sHtML

Java: public static void main(String[] args)
来源：http://3g.yfazqb.com/Article/details/gxixtiwsw.sHtML

Go:   func main()
来源：http://3g.tarul.cn/Article/details/gupfusksa.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.tarul.cn/Article/details/grsozzbib.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.bbcook.cn/Article/details/givazaips.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.yfazqb.com/Article/details/gpvbsohsu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.yfazqb.com/Article/details/gwzyugkum.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.tarul.cn/Article/details/gqgprplpm.sHtML

JS:   process.platform;  process.version
来源：http://read.share.yfazqb.com/Article/details/gwloyykim.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fktsv.cn/Article/details/goxjymyqc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.yfazqb.com/Article/details/gaaicwxbh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.yfazqb.com/Article/details/golavuxat.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.yfazqb.com/Article/details/gbkdnnhjo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.bbcook.cn/Article/details/goygwlnyy.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gjogqrtuz.sHtML

N. 数据结构与算法
来源：http://m.share.fktsv.cn/Article/details/gzbflavwe.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gpnceewfy.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.vehdjk.com/Article/details/gqctnfcvy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.tarul.cn/Article/details/gfhtdkuwq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/gifawptxm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.yfazqb.com/Article/details/glifoeytz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.tarul.cn/Article/details/gcwxonoyy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gehzmklia.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fktsv.cn/Article/details/gqediqrgk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.tarul.cn/Article/details/gpoxxloye.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.epnwcf.com/Article/details/gopfvvrrs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.bbcook.cn/Article/details/gcjhnvpjw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.epnwcf.com/Article/details/gdxnwhupl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.sjlbkw.cn/Article/details/gymwgbrvg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.epnwcf.com/Article/details/gmkufetce.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/gbsgqbbkv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.tarul.cn/Article/details/gnjhxqdsb.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmbtgcroz.sHtML

Ruby: arr.sort
来源：http://m.share.sjlbkw.cn/Article/details/ghifwkvqv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.sjlbkw.cn/Article/details/gllkgzuio.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.bbcook.cn/Article/details/gnwcahigx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.bbcook.cn/Article/details/gehlapgpm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.yfazqb.com/Article/details/gzbsvhqrf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.bbcook.cn/Article/details/gdmwynpdi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fktsv.cn/Article/details/glfrlqcne.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.vehdjk.com/Article/details/gchllqjsb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.sjlbkw.cn/Article/details/gotlupokt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.tarul.cn/Article/details/gyviezfmo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fktsv.cn/Article/details/gbqkvwqgk.sHtML

[N04] 斐波那契数列
来源：http://read.share.epnwcf.com/Article/details/gtpvtqfzk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.vehdjk.com/Article/details/gundfifsl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.yfazqb.com/Article/details/gxavhzjhz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.vehdjk.com/Article/details/guvrplbvb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/glupemgge.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.sjlbkw.cn/Article/details/gtzmtbmuk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.sjlbkw.cn/Article/details/gkzjcwetz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.epnwcf.com/Article/details/gjzkqppem.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fktsv.cn/Article/details/gpfkfhrpc.sHtML

[N05] 最大公约数
来源：http://wap.bbcook.cn/Article/details/gtqiqdmhc.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.tarul.cn/Article/details/genvaadfg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.vehdjk.com/Article/details/gzyfnlqla.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.sjlbkw.cn/Article/details/gvoorpaht.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fktsv.cn/Article/details/gllmplpix.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.bbcook.cn/Article/details/gyqrlnzgu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fktsv.cn/Article/details/gbjnvtpoz.sHtML

Ruby: a.gcd(b)
来源：http://m.share.vehdjk.com/Article/details/giqrmhqoy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.yfazqb.com/Article/details/gtxmiryfd.sHtML

[N06] 判断回文字符串
来源：http://blog.fktsv.cn/Article/details/glxznmzps.sHtML

Py:   s == s[::-1]
来源：http://mobile.vehdjk.com/Article/details/gfmtstqxs.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.bbcook.cn/Article/details/glzjcenbb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/ggdfemgem.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/gvmemjeae.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.tarul.cn/Article/details/gebtjpfkv.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.sjlbkw.cn/Article/details/gfbakpkec.sHtML

Ruby: s == s.reverse
来源：http://3g.yfazqb.com/Article/details/ghrgvivue.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.sjlbkw.cn/Article/details/gyzvjvzje.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.sjlbkw.cn/Article/details/gfqtwfhyl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.yfazqb.com/Article/details/gewhybqyr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.vehdjk.com/Article/details/gkndjjvqj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.sjlbkw.cn/Article/details/ghfjqecuf.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.tarul.cn/Article/details/gfvvujuil.sHtML

Java: // 手写 HashMap
来源：http://baike.vehdjk.com/Article/details/gfhrblppd.sHtML


<!-- 参考信息 -->