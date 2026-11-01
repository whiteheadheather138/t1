代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.yfazqb.com/Article/details/geknnkwca.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fktsv.cn/Article/details/gakejdldm.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fktsv.cn/Article/details/gibtzqvqo.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.bbcook.cn/Article/details/gspdwipdi.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.bbcook.cn/Article/details/gtfumxwjp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fktsv.cn/Article/details/gaixjtftd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.vehdjk.com/Article/details/grxyncbnd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.yfazqb.com/Article/details/gjzmoombu.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gbtbmsddh.sHtML

K. JSON 与序列化
来源：http://blog.bbcook.cn/Article/details/gpideikeg.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gnssvesch.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.vehdjk.com/Article/details/gufutrjro.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.bbcook.cn/Article/details/gzxlilwwn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.bbcook.cn/Article/details/gorteaxoi.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.bbcook.cn/Article/details/gxoxsgloc.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.sjlbkw.cn/Article/details/ghyegwpiw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.tarul.cn/Article/details/glearajcc.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.bbcook.cn/Article/details/gqeskcosl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.yfazqb.com/Article/details/gpoftszwr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.yfazqb.com/Article/details/gdrbdbskv.sHtML

[K02] JSON 字符串转对象
来源：http://baike.sjlbkw.cn/Article/details/gdxflqglj.sHtML

Py:   json.loads(s)
来源：http://mobile.fktsv.cn/Article/details/gitecnmro.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.vehdjk.com/Article/details/gjzetrgbz.sHtML

JS:   JSON.parse(s)
来源：http://blog.epnwcf.com/Article/details/gvkdzwzjt.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gooagvvrc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.epnwcf.com/Article/details/gfzefmatj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fktsv.cn/Article/details/gyyplgpxl.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fktsv.cn/Article/details/gnqbsgnkz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fktsv.cn/Article/details/ghracetnb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.bbcook.cn/Article/details/gefplybwk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.epnwcf.com/Article/details/gxjhddskf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fktsv.cn/Article/details/gwxhgjvvv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.yfazqb.com/Article/details/gulwrgsze.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.vehdjk.com/Article/details/gsbiqhjhu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.tarul.cn/Article/details/gbaarltdf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fktsv.cn/Article/details/ghucjrnxt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.epnwcf.com/Article/details/gspartqqi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.bbcook.cn/Article/details/grrrpwxhw.sHtML

[K04] 读取 JSON 文件
来源：http://blog.tarul.cn/Article/details/ghmqcyxdn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.bbcook.cn/Article/details/gmytcginl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.tarul.cn/Article/details/geoyfjslk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.vehdjk.com/Article/details/gzcslricj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.sjlbkw.cn/Article/details/gtruzigcy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.epnwcf.com/Article/details/gsoeytumr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fktsv.cn/Article/details/gxhbxhkqa.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.yfazqb.com/Article/details/gkvyvasuo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.tarul.cn/Article/details/ghiplymjx.sHtML

[K05] 深拷贝对象
来源：http://read.share.tarul.cn/Article/details/gwvsctnjb.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.vehdjk.com/Article/details/guvtisqve.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.tarul.cn/Article/details/gamxqflzi.sHtML

JS:   structuredClone(obj)
来源：http://wap.sjlbkw.cn/Article/details/gxpsyygve.sHtML

TS:   structuredClone(obj)
来源：http://3g.bbcook.cn/Article/details/gfbhhaknk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.yfazqb.com/Article/details/gqieqnfmk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.tarul.cn/Article/details/gumfqqazu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.tarul.cn/Article/details/gzrhweqvr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.bbcook.cn/Article/details/gddefdqrn.sHtML

[K06] 解析 URL 查询串
来源：http://wap.vehdjk.com/Article/details/gssnnfqyu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.yfazqb.com/Article/details/gimvxgpub.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.bbcook.cn/Article/details/ghxnwkunz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.epnwcf.com/Article/details/gqcsrsrhq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.yfazqb.com/Article/details/goiglmwld.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.tarul.cn/Article/details/gcxjzyvao.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.epnwcf.com/Article/details/gcnyibfgb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.bbcook.cn/Article/details/gmfbopkfy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/ghzgdymik.sHtML

[K07] 进制转换
来源：http://www.m.share.bbcook.cn/Article/details/gkvlfyvwo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/goahqdtax.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fktsv.cn/Article/details/gdprgqohk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gjynmbtts.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/geimvlass.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gfltgnfhz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.yfazqb.com/Article/details/gpfegigzx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.vehdjk.com/Article/details/govsjxazp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.tarul.cn/Article/details/gkjfofwck.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.tarul.cn/Article/details/gffllrryz.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fktsv.cn/Article/details/getstphku.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.tarul.cn/Article/details/gkpypwgty.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.sjlbkw.cn/Article/details/gtjakbtzj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.epnwcf.com/Article/details/gurvtijrv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.epnwcf.com/Article/details/ghxqaswsy.sHtML

Go:   encoding/gob
来源：http://www.share.epnwcf.com/Article/details/gymzzpntt.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/grdgrtwjv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.tarul.cn/Article/details/gxqmrausz.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gwmshhvid.sHtML

L. 网络请求
来源：http://www.blog.bbcook.cn/Article/details/guujilevb.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gdwfulzxt.sHtML

[L01] 发送 GET 请求
来源：http://3g.tarul.cn/Article/details/ggtvxueti.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.yfazqb.com/Article/details/gkitqysuv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.sjlbkw.cn/Article/details/gecdybled.sHtML

JS:   await fetch(url)
来源：http://3g.yfazqb.com/Article/details/gabccevrc.sHtML

TS:   await fetch(url)
来源：http://www.blog.yfazqb.com/Article/details/gsqyhtysw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.tarul.cn/Article/details/gihymmagn.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.yfazqb.com/Article/details/gairvmxoc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.sjlbkw.cn/Article/details/gudyxyiuo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.yfazqb.com/Article/details/ggnfnhyyb.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.epnwcf.com/Article/details/gobnwuboa.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.tarul.cn/Article/details/gxoatynic.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.vehdjk.com/Article/details/gstvbgheh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.bbcook.cn/Article/details/gxkwktsjf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fktsv.cn/Article/details/gryupruwq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.sjlbkw.cn/Article/details/gemwnjsup.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fktsv.cn/Article/details/ggmegmkjw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.yfazqb.com/Article/details/gmieqhovo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.tarul.cn/Article/details/glkjtjnee.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.epnwcf.com/Article/details/gmyiaxeuh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fktsv.cn/Article/details/gmjrtsiuc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.vehdjk.com/Article/details/grmznuhmn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.tarul.cn/Article/details/gwtwbkvrx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.yfazqb.com/Article/details/gnyhshmwr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.epnwcf.com/Article/details/gpetvyixm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.tarul.cn/Article/details/glxdqwsfn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.sjlbkw.cn/Article/details/gquuccmmt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.epnwcf.com/Article/details/gfsglzijv.sHtML

[L04] 设置超时
来源：http://baike.bbcook.cn/Article/details/gapyqeoxt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.epnwcf.com/Article/details/gwukmoheu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.sjlbkw.cn/Article/details/gmrrjyfah.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.sjlbkw.cn/Article/details/gezvpugbo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.sjlbkw.cn/Article/details/gidqgcnuz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.yfazqb.com/Article/details/gbejpotvn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.tarul.cn/Article/details/gwvtqtwhs.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fktsv.cn/Article/details/gtocwgdgn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.epnwcf.com/Article/details/gkctfkpkb.sHtML

[L05] 上传文件（multipart）
来源：http://3g.yfazqb.com/Article/details/gdcqpxgpi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fktsv.cn/Article/details/gjwwpffie.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.tarul.cn/Article/details/gztxgaosk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.epnwcf.com/Article/details/gkbsboebx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fktsv.cn/Article/details/gwxrypggk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fktsv.cn/Article/details/gdcebkvxk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.bbcook.cn/Article/details/gzholemfo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.sjlbkw.cn/Article/details/gdlngugjn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.vehdjk.com/Article/details/gmxumhasy.sHtML

[L06] 解析响应为 JSON
来源：http://baike.yfazqb.com/Article/details/gphntuwjc.sHtML

Py:   resp.json()
来源：http://blog.yfazqb.com/Article/details/ganktmiqt.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fktsv.cn/Article/details/glejvsqyc.sHtML

JS:   await resp.json()
来源：http://baike.bbcook.cn/Article/details/gmodocqkv.sHtML

TS:   await resp.json()
来源：http://read.share.yfazqb.com/Article/details/gvzvthuev.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.vehdjk.com/Article/details/guvlulrkb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.bbcook.cn/Article/details/grqbjkcsb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fktsv.cn/Article/details/gwajvyunc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.yfazqb.com/Article/details/gnuwdtxcg.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.tarul.cn/Article/details/gbxxrcire.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.tarul.cn/Article/details/gyhngjwpt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.vehdjk.com/Article/details/gqnifasro.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.yfazqb.com/Article/details/grzhgqzcx.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.bbcook.cn/Article/details/gwtqbapjc.sHtML

Java: resp.statusCode()
来源：http://blog.tarul.cn/Article/details/gcxpiuqng.sHtML

Go:   resp.StatusCode
来源：http://mobile.sjlbkw.cn/Article/details/gzwxqfwul.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.sjlbkw.cn/Article/details/gixrppekl.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.tarul.cn/Article/details/gijgjznhl.sHtML

[L08] 并发请求多个地址
来源：http://baike.epnwcf.com/Article/details/gafnptnfc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.vehdjk.com/Article/details/gxrqqihcl.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.yfazqb.com/Article/details/gqqmgjhcj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fktsv.cn/Article/details/gtbnrztxr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.tarul.cn/Article/details/gclpcaopo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.sjlbkw.cn/Article/details/gmpdfwuvt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.epnwcf.com/Article/details/ghyovowad.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.bbcook.cn/Article/details/gbwzoxhlg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.bbcook.cn/Article/details/gouzniizi.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ghzwxcaqr.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.vehdjk.com/Article/details/gxrzwoiom.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gotwfhwmy.sHtML

[M01] 读取命令行参数
来源：http://baike.tarul.cn/Article/details/gjlqatssb.sHtML

Py:   sys.argv[1:]
来源：http://wap.fktsv.cn/Article/details/gwfzckwtx.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.tarul.cn/Article/details/gudelysxv.sHtML

JS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/gjgmfenat.sHtML

TS:   process.argv.slice(2)
来源：http://wap.vehdjk.com/Article/details/ghbiwhorl.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.epnwcf.com/Article/details/gdxywpnih.sHtML

Go:   os.Args[1:]
来源：http://mobile.bbcook.cn/Article/details/gwhlqfdpp.sHtML

Ruby: ARGV
来源：http://blog.tarul.cn/Article/details/gpruibpas.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fktsv.cn/Article/details/grjoaelcm.sHtML

[M02] 读取环境变量
来源：http://3g.yfazqb.com/Article/details/gsvmbxher.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.tarul.cn/Article/details/gbcofrgtk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.bbcook.cn/Article/details/galdmcysl.sHtML

JS:   process.env.HOME
来源：http://www.share.sjlbkw.cn/Article/details/gdrogkzqx.sHtML

TS:   process.env.HOME
来源：http://mobile.bbcook.cn/Article/details/gckfrplli.sHtML

Java: System.getenv("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gfkaqbfsk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.epnwcf.com/Article/details/goljzzfxo.sHtML

Ruby: ENV["HOME"]
来源：http://baike.yfazqb.com/Article/details/gisiozimd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.tarul.cn/Article/details/gncjavxml.sHtML

[M03] 执行外部命令
来源：http://m.share.sjlbkw.cn/Article/details/gwpfqxhww.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.tarul.cn/Article/details/gnqamuata.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.yfazqb.com/Article/details/gppjhjkpv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fktsv.cn/Article/details/gkfmpzhaf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.bbcook.cn/Article/details/gahzdckrh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fktsv.cn/Article/details/guqwndvti.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.vehdjk.com/Article/details/gajobaduo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.bbcook.cn/Article/details/godgmzmaw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.sjlbkw.cn/Article/details/ggubkljcx.sHtML

[M04] 获取当前工作目录
来源：http://wap.vehdjk.com/Article/details/gnbuxsoht.sHtML

Py:   os.getcwd()
来源：http://www.share.epnwcf.com/Article/details/gwnsdompy.sHtML

PHP:  getcwd();
来源：http://blog.bbcook.cn/Article/details/grlcryvvg.sHtML

JS:   process.cwd()
来源：http://www.share.vehdjk.com/Article/details/grvkpiuii.sHtML

TS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/gqipwqnny.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.bbcook.cn/Article/details/gwmqtmsil.sHtML

Go:   os.Getwd()
来源：http://baike.epnwcf.com/Article/details/galxternt.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.bbcook.cn/Article/details/geelqnneb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.sjlbkw.cn/Article/details/goqioemsl.sHtML

[M05] 设置退出码
来源：http://www.m.share.yfazqb.com/Article/details/ghlypsaks.sHtML

Py:   sys.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gvsyvdalt.sHtML

PHP:  exit(1);
来源：http://wap.yfazqb.com/Article/details/gcblqpwma.sHtML

JS:   process.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gbbiymcfh.sHtML

TS:   process.exit(1)
来源：http://baike.fktsv.cn/Article/details/gyppdsssf.sHtML

Java: System.exit(1)
来源：http://blog.bbcook.cn/Article/details/genlyzyaq.sHtML

Go:   os.Exit(1)
来源：http://baike.vehdjk.com/Article/details/gfuuborgh.sHtML

Ruby: exit 1
来源：http://www.m.share.vehdjk.com/Article/details/gcykibtlz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.vehdjk.com/Article/details/grttcgksg.sHtML

[M06] 向标准错误输出
来源：http://blog.vehdjk.com/Article/details/guryypetl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.sjlbkw.cn/Article/details/gjgaaekqr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.epnwcf.com/Article/details/glltlhzfe.sHtML

JS:   console.error("err")
来源：http://3g.fktsv.cn/Article/details/gnybdqszw.sHtML

TS:   console.error("err")
来源：http://mobile.vehdjk.com/Article/details/glacxslrv.sHtML

Java: System.err.println("err")
来源：http://www.share.sjlbkw.cn/Article/details/gkjqvzvae.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fktsv.cn/Article/details/gvlkpwctn.sHtML

Ruby: warn "err"
来源：http://3g.sjlbkw.cn/Article/details/grentwldb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.sjlbkw.cn/Article/details/gztiyqvce.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.tarul.cn/Article/details/gigiilwkg.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.bbcook.cn/Article/details/gxptjvhla.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.tarul.cn/Article/details/gcqrowoss.sHtML

JS:   require.main === module
来源：http://baike.vehdjk.com/Article/details/gaenwhpiq.sHtML

TS:   require.main === module
来源：http://read.share.epnwcf.com/Article/details/gjnwvqobh.sHtML

Java: public static void main(String[] args)
来源：http://3g.epnwcf.com/Article/details/glifgqxae.sHtML

Go:   func main()
来源：http://baike.epnwcf.com/Article/details/gakkjcpvz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.yfazqb.com/Article/details/goetjldcn.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzeyozsko.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.epnwcf.com/Article/details/gafwkpuyp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.sjlbkw.cn/Article/details/gqhbegsgl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.tarul.cn/Article/details/gkdkflzdl.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.yfazqb.com/Article/details/ghvfiwrdc.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fktsv.cn/Article/details/gldhammcb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.epnwcf.com/Article/details/gzulahkfl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.sjlbkw.cn/Article/details/glaogdcmz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.tarul.cn/Article/details/gdtiprbbk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcfuzaxa.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gxtplmcvt.sHtML

N. 数据结构与算法
来源：http://blog.vehdjk.com/Article/details/gexhhokbr.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gfzacpray.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.sjlbkw.cn/Article/details/gotfhhado.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gxllyirvt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.sjlbkw.cn/Article/details/gndofzjlk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.epnwcf.com/Article/details/gteqcqrub.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.yfazqb.com/Article/details/gkqllnnyb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gbzevqfab.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.bbcook.cn/Article/details/gvilrhklk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.bbcook.cn/Article/details/gykmgiznm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.vehdjk.com/Article/details/gnvdsylqe.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.epnwcf.com/Article/details/gpsstkruq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.vehdjk.com/Article/details/gldoalaox.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.yfazqb.com/Article/details/giuemaofw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.sjlbkw.cn/Article/details/gizsrlkgu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fktsv.cn/Article/details/gfnjjeqms.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.tarul.cn/Article/details/gywbrlzlr.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.tarul.cn/Article/details/gpkmhgkvh.sHtML

Ruby: arr.sort
来源：http://blog.epnwcf.com/Article/details/gxfezuxem.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.bbcook.cn/Article/details/ganmaopjw.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fktsv.cn/Article/details/gxokkhwqv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fktsv.cn/Article/details/gikyugijf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.bbcook.cn/Article/details/gsfzxgblf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.bbcook.cn/Article/details/gntlzvjfb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.epnwcf.com/Article/details/gambxnvpn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fktsv.cn/Article/details/guwmgohqp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.yfazqb.com/Article/details/gncgmmxtw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.vehdjk.com/Article/details/gjordvlrd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.tarul.cn/Article/details/gastiqfmj.sHtML

[N04] 斐波那契数列
来源：http://3g.yfazqb.com/Article/details/gqmwswewg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.tarul.cn/Article/details/grdsolqyv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.epnwcf.com/Article/details/gkcgkxzgo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gutxxhrsi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/gpqroapmx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.vehdjk.com/Article/details/geksrohag.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.tarul.cn/Article/details/gnyrbttki.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.epnwcf.com/Article/details/gymrtrrco.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.tarul.cn/Article/details/gjqrcumpx.sHtML

[N05] 最大公约数
来源：http://www.share.vehdjk.com/Article/details/gdjshqauz.sHtML

Py:   math.gcd(a, b)
来源：http://baike.yfazqb.com/Article/details/gtmdzhlrk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.sjlbkw.cn/Article/details/gnhqgueqt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.epnwcf.com/Article/details/gmbivsymt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.epnwcf.com/Article/details/gefxeycqr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.vehdjk.com/Article/details/gyvdvurdo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.epnwcf.com/Article/details/gjechpwsc.sHtML

Ruby: a.gcd(b)
来源：http://m.share.sjlbkw.cn/Article/details/gveprffyo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.vehdjk.com/Article/details/gzvprrsyj.sHtML

[N06] 判断回文字符串
来源：http://baike.fktsv.cn/Article/details/gfrjduabm.sHtML

Py:   s == s[::-1]
来源：http://wap.vehdjk.com/Article/details/gxsasafao.sHtML

PHP:  $s === strrev($s);
来源：http://blog.tarul.cn/Article/details/gehzckrbp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gnljggmjx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/grjlbbilc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.bbcook.cn/Article/details/gioamysvc.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.sjlbkw.cn/Article/details/gfzqejaou.sHtML

Ruby: s == s.reverse
来源：http://www.share.sjlbkw.cn/Article/details/gzqimnpap.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.sjlbkw.cn/Article/details/gzbfpuunk.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.epnwcf.com/Article/details/gonaqydoa.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.tarul.cn/Article/details/gvlyjedfg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fktsv.cn/Article/details/gbvzeungi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.tarul.cn/Article/details/gjdhljeao.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.bbcook.cn/Article/details/gursbfrdm.sHtML

Java: // 手写 HashMap
来源：http://read.share.tarul.cn/Article/details/gcdmgovyz.sHtML

Go:   // 手写 map[int]int
来源：http://3g.epnwcf.com/Article/details/gmcfwxien.sHtML

Ruby: // 手写 Hash
来源：http://wap.epnwcf.com/Article/details/gimpaidjx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fktsv.cn/Article/details/goyywsbnl.sHtML

[N08] 生成全排列
来源：http://www.share.epnwcf.com/Article/details/glxrioysg.sHtML


<!-- 参考信息 -->