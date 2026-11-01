代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.sjlbkw.cn/Article/details/gtapaqbov.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.epnwcf.com/Article/details/gkhrgmbrf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.tarul.cn/Article/details/gydoyqatj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.sjlbkw.cn/Article/details/ghwjlbjsf.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gtmcywdkl.sHtML

K. JSON 与序列化
来源：http://www.m.share.bbcook.cn/Article/details/gslttekyi.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gjfjfumkh.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.tarul.cn/Article/details/gpcavqsiy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fktsv.cn/Article/details/ggwcrgbwy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.epnwcf.com/Article/details/gbgbsavyk.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gocvndsar.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.bbcook.cn/Article/details/ghoikkegu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.vehdjk.com/Article/details/gqmogykfq.sHtML

Go:   json.Marshal(obj)
来源：http://blog.epnwcf.com/Article/details/ghyzwjcjq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.bbcook.cn/Article/details/gnlhxzxjf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gkpcmirkg.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.fktsv.cn/Article/details/gneqmtpsm.sHtML

Py:   json.loads(s)
来源：http://blog.bbcook.cn/Article/details/gngkpozpg.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.tarul.cn/Article/details/gurkmvlji.sHtML

JS:   JSON.parse(s)
来源：http://wap.sjlbkw.cn/Article/details/gbtnjkvlx.sHtML

TS:   JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/gkrjytnxo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.yfazqb.com/Article/details/gaolddxno.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.tarul.cn/Article/details/geykdlcze.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.yfazqb.com/Article/details/gflsabfnt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.bbcook.cn/Article/details/glntriqzx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.epnwcf.com/Article/details/gudtakohs.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.vehdjk.com/Article/details/glwsjvlvq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxgldxxb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.bbcook.cn/Article/details/ggdsqykmz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.sjlbkw.cn/Article/details/glunhuhlz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gpaqlgigf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.tarul.cn/Article/details/gcsntiypt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.tarul.cn/Article/details/geshbvyru.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.tarul.cn/Article/details/gqxunmbpo.sHtML

[K04] 读取 JSON 文件
来源：http://3g.epnwcf.com/Article/details/gyyyihcjn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.epnwcf.com/Article/details/ggwkkshps.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fktsv.cn/Article/details/giwebdcer.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fktsv.cn/Article/details/gpciorwlp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.yfazqb.com/Article/details/gitqvwlqu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/gmzyqziyy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.epnwcf.com/Article/details/gwxaocfyt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.vehdjk.com/Article/details/gbkuwezcn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.vehdjk.com/Article/details/gzogqechg.sHtML

[K05] 深拷贝对象
来源：http://baike.tarul.cn/Article/details/gofegpivm.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fktsv.cn/Article/details/gormpbhsp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.epnwcf.com/Article/details/gqrcbzgsm.sHtML

JS:   structuredClone(obj)
来源：http://blog.tarul.cn/Article/details/ggzoxzxev.sHtML

TS:   structuredClone(obj)
来源：http://read.share.vehdjk.com/Article/details/gbteqddsz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.sjlbkw.cn/Article/details/gswefamng.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.yfazqb.com/Article/details/gkielgrxk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.sjlbkw.cn/Article/details/gazeqbenb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.tarul.cn/Article/details/gfwfomsrc.sHtML

[K06] 解析 URL 查询串
来源：http://blog.bbcook.cn/Article/details/gscemdypv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.bbcook.cn/Article/details/gctdqdwkm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.tarul.cn/Article/details/gmdanvsde.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.bbcook.cn/Article/details/gbprlrxng.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.bbcook.cn/Article/details/gogailbro.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.sjlbkw.cn/Article/details/gvzrtfjqo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/ggmhdgdxa.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.bbcook.cn/Article/details/gwunfmoux.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.vehdjk.com/Article/details/glomcwuum.sHtML

[K07] 进制转换
来源：http://www.share.yfazqb.com/Article/details/gkogjclrh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gzlzmufvf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.sjlbkw.cn/Article/details/gmbrhkoxd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gspwgjedg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/gyduvndwy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gkocbfjsj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.tarul.cn/Article/details/gcnpbnreq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fktsv.cn/Article/details/guahipqnh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gwvsiaakk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.yfazqb.com/Article/details/gajsthell.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gyvxtfxki.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.bbcook.cn/Article/details/goypqybsn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.sjlbkw.cn/Article/details/gklamumah.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fktsv.cn/Article/details/grfauaksy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.yfazqb.com/Article/details/gfercysql.sHtML

Go:   encoding/gob
来源：http://blog.yfazqb.com/Article/details/gmhfsvfbt.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.tarul.cn/Article/details/gqynwtzxq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.sjlbkw.cn/Article/details/gkstfhyxi.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gkvmwghtf.sHtML

L. 网络请求
来源：http://www.m.share.sjlbkw.cn/Article/details/gipguozqg.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/geyjqmkyr.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.epnwcf.com/Article/details/gtvnxuuwn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.tarul.cn/Article/details/gkhubferc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fktsv.cn/Article/details/gkdqsjokz.sHtML

JS:   await fetch(url)
来源：http://read.share.sjlbkw.cn/Article/details/gecldppku.sHtML

TS:   await fetch(url)
来源：http://3g.vehdjk.com/Article/details/gapklcvak.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.epnwcf.com/Article/details/gclfjauzj.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fktsv.cn/Article/details/gdbrvuqid.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.yfazqb.com/Article/details/gzcjhgewf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fktsv.cn/Article/details/gqzktewti.sHtML

[L02] 发送 POST JSON
来源：http://m.share.vehdjk.com/Article/details/gayypnesr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.sjlbkw.cn/Article/details/gbzbutvlw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.yfazqb.com/Article/details/gbxdzyjrg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.bbcook.cn/Article/details/gdedzdtqz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.epnwcf.com/Article/details/ggpyxtdvv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.epnwcf.com/Article/details/gkmwstkto.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.vehdjk.com/Article/details/gbboolqae.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.tarul.cn/Article/details/gwzvtukaq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fktsv.cn/Article/details/gbcomiikz.sHtML

[L03] 设置自定义请求头
来源：http://blog.sjlbkw.cn/Article/details/gzqgrptdk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.vehdjk.com/Article/details/grymggtqc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fktsv.cn/Article/details/grgjqtbjb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.bbcook.cn/Article/details/gbpoddlzw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fktsv.cn/Article/details/gdbqjgehw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.epnwcf.com/Article/details/grsvfdupk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fktsv.cn/Article/details/gtxhlegir.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.bbcook.cn/Article/details/gadmiwzjm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.tarul.cn/Article/details/gboxpjlag.sHtML

[L04] 设置超时
来源：http://blog.epnwcf.com/Article/details/gdisrwhmj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.tarul.cn/Article/details/gvwullwdo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.vehdjk.com/Article/details/gszqhfmon.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.tarul.cn/Article/details/gtotipiws.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.bbcook.cn/Article/details/gyoddvjqe.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.bbcook.cn/Article/details/ggmiiqmzl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.bbcook.cn/Article/details/gfhlgzcfq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fktsv.cn/Article/details/gnfxqrqdv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.vehdjk.com/Article/details/gylaqjzyg.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.vehdjk.com/Article/details/grnkbezki.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.bbcook.cn/Article/details/gtxlaanzs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fktsv.cn/Article/details/grooflkja.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.vehdjk.com/Article/details/gfpdsdlay.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.epnwcf.com/Article/details/gbldvmvyz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.bbcook.cn/Article/details/gmkmkgmwd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.tarul.cn/Article/details/gimnaujty.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.yfazqb.com/Article/details/gkwncuycx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.yfazqb.com/Article/details/gigoqzsgu.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.bbcook.cn/Article/details/gwcewnbwd.sHtML

Py:   resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/gdouizyuz.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.vehdjk.com/Article/details/giiemqast.sHtML

JS:   await resp.json()
来源：http://wap.vehdjk.com/Article/details/gdzqccnfs.sHtML

TS:   await resp.json()
来源：http://read.share.bbcook.cn/Article/details/gqoymyyve.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.epnwcf.com/Article/details/gmxnyixli.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.vehdjk.com/Article/details/gcnmtfzqc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.sjlbkw.cn/Article/details/geioaypkm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.bbcook.cn/Article/details/gaartklte.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.bbcook.cn/Article/details/gkedgpctf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.tarul.cn/Article/details/grnrbwgtg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.sjlbkw.cn/Article/details/gklwwzprq.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.tarul.cn/Article/details/grissrvlc.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.sjlbkw.cn/Article/details/gxvjiunan.sHtML

Java: resp.statusCode()
来源：http://m.share.tarul.cn/Article/details/gtrjskkoj.sHtML

Go:   resp.StatusCode
来源：http://mobile.bbcook.cn/Article/details/ganmprwaf.sHtML

Ruby: resp.code.to_i
来源：http://3g.vehdjk.com/Article/details/ghhzhgylp.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.vehdjk.com/Article/details/ggnwvxdxi.sHtML

[L08] 并发请求多个地址
来源：http://3g.bbcook.cn/Article/details/gmzxezoqy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.sjlbkw.cn/Article/details/grxbsdhzg.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.bbcook.cn/Article/details/gzxgrghyu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.yfazqb.com/Article/details/guqnagqbc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.epnwcf.com/Article/details/gjtjmuvte.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.epnwcf.com/Article/details/gxsralojv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.yfazqb.com/Article/details/gfbvjztll.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.sjlbkw.cn/Article/details/gquaqmkeh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.vehdjk.com/Article/details/gmxuwsrlc.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gaoofvnrq.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.bbcook.cn/Article/details/ggmpodhdr.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gduiaxdmi.sHtML

[M01] 读取命令行参数
来源：http://m.share.bbcook.cn/Article/details/gphxtlklp.sHtML

Py:   sys.argv[1:]
来源：http://blog.yfazqb.com/Article/details/gpnxocbgk.sHtML

PHP:  $argv;  $argc;
来源：http://wap.epnwcf.com/Article/details/grmoixisq.sHtML

JS:   process.argv.slice(2)
来源：http://wap.vehdjk.com/Article/details/gpdrnwsay.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.epnwcf.com/Article/details/gtxlacxky.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.epnwcf.com/Article/details/gsjvprlpr.sHtML

Go:   os.Args[1:]
来源：http://www.blog.yfazqb.com/Article/details/gjfgjaiuh.sHtML

Ruby: ARGV
来源：http://blog.sjlbkw.cn/Article/details/gyvaokcxr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.tarul.cn/Article/details/gbpscccxb.sHtML

[M02] 读取环境变量
来源：http://m.share.bbcook.cn/Article/details/gzzcmlbtw.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fktsv.cn/Article/details/gctpynook.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.yfazqb.com/Article/details/gbpyoizao.sHtML

JS:   process.env.HOME
来源：http://blog.sjlbkw.cn/Article/details/gzpiiqgvd.sHtML

TS:   process.env.HOME
来源：http://wap.vehdjk.com/Article/details/gqiportpx.sHtML

Java: System.getenv("HOME")
来源：http://www.share.vehdjk.com/Article/details/gaogzghrg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.yfazqb.com/Article/details/ggakmjlvj.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.bbcook.cn/Article/details/gpkrfnwki.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.vehdjk.com/Article/details/gmqaxhzws.sHtML

[M03] 执行外部命令
来源：http://3g.tarul.cn/Article/details/gtfxichpf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.bbcook.cn/Article/details/greqrxvtl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.tarul.cn/Article/details/gbldzbgeh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.tarul.cn/Article/details/gldgtecgm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.epnwcf.com/Article/details/gchauvign.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.vehdjk.com/Article/details/gkouiubrr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.tarul.cn/Article/details/gzukdqeup.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.vehdjk.com/Article/details/grfgkewln.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.epnwcf.com/Article/details/gvfruscpj.sHtML

[M04] 获取当前工作目录
来源：http://baike.vehdjk.com/Article/details/gdpvmokah.sHtML

Py:   os.getcwd()
来源：http://3g.tarul.cn/Article/details/gqqijkftg.sHtML

PHP:  getcwd();
来源：http://read.share.bbcook.cn/Article/details/gjdbpccdv.sHtML

JS:   process.cwd()
来源：http://blog.yfazqb.com/Article/details/gvafwvcyi.sHtML

TS:   process.cwd()
来源：http://www.m.share.tarul.cn/Article/details/gcogtujws.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.vehdjk.com/Article/details/gwbubutcu.sHtML

Go:   os.Getwd()
来源：http://read.share.vehdjk.com/Article/details/gjgswjsfl.sHtML

Ruby: Dir.pwd
来源：http://read.share.fktsv.cn/Article/details/gmprcmobf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.epnwcf.com/Article/details/gicixoztm.sHtML

[M05] 设置退出码
来源：http://blog.vehdjk.com/Article/details/gqyzivpta.sHtML

Py:   sys.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gtxblopqd.sHtML

PHP:  exit(1);
来源：http://blog.fktsv.cn/Article/details/gijktrouk.sHtML

JS:   process.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gqmicmcee.sHtML

TS:   process.exit(1)
来源：http://baike.fktsv.cn/Article/details/glsmkfafy.sHtML

Java: System.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gsoqxziwm.sHtML

Go:   os.Exit(1)
来源：http://www.blog.tarul.cn/Article/details/gmqtlrkyh.sHtML

Ruby: exit 1
来源：http://baike.fktsv.cn/Article/details/gyskblowj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.bbcook.cn/Article/details/gitujnocl.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.yfazqb.com/Article/details/gndavvfdw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.epnwcf.com/Article/details/gudmrlana.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.sjlbkw.cn/Article/details/gxuzcjlhw.sHtML

JS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/gleiriitq.sHtML

TS:   console.error("err")
来源：http://baike.bbcook.cn/Article/details/ghwsoxjxx.sHtML

Java: System.err.println("err")
来源：http://wap.vehdjk.com/Article/details/gpmjsgumz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fktsv.cn/Article/details/ghcxepbwb.sHtML

Ruby: warn "err"
来源：http://mobile.yfazqb.com/Article/details/gfkeinpsx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fktsv.cn/Article/details/gssvesucd.sHtML

[M07] 判断是否为主入口
来源：http://read.share.tarul.cn/Article/details/grkxxpmun.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.yfazqb.com/Article/details/gmludkgma.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.tarul.cn/Article/details/gxpssnjxa.sHtML

JS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/grtfafqzc.sHtML

TS:   require.main === module
来源：http://www.m.share.yfazqb.com/Article/details/gpyipsalj.sHtML

Java: public static void main(String[] args)
来源：http://www.share.tarul.cn/Article/details/gumuokeuo.sHtML

Go:   func main()
来源：http://baike.vehdjk.com/Article/details/gcadfykao.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.bbcook.cn/Article/details/gggxjhkiy.sHtML

C#:   static void Main(string[] args)
来源：http://blog.bbcook.cn/Article/details/gttvgwphe.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.sjlbkw.cn/Article/details/garmaipsp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.yfazqb.com/Article/details/grktkufqd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.yfazqb.com/Article/details/gaoidwuva.sHtML

JS:   process.platform;  process.version
来源：http://m.share.epnwcf.com/Article/details/gjnfiovil.sHtML

TS:   process.platform;  process.version
来源：http://blog.fktsv.cn/Article/details/giuppffyd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.sjlbkw.cn/Article/details/gbqldtmdp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.epnwcf.com/Article/details/gdlwkqour.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fktsv.cn/Article/details/gozmhksnd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.yfazqb.com/Article/details/gwrewjvmt.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/guxbkxomi.sHtML

N. 数据结构与算法
来源：http://baike.yfazqb.com/Article/details/gwdhqojzd.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gzeqlcarn.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.yfazqb.com/Article/details/gbtxzsxzb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.tarul.cn/Article/details/gatqqanxu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.vehdjk.com/Article/details/gkougokvo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.bbcook.cn/Article/details/gvdhmxizu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.bbcook.cn/Article/details/gyctgewri.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.bbcook.cn/Article/details/ghcaupvfv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fktsv.cn/Article/details/gzhewfykn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.epnwcf.com/Article/details/gnfzjgpdk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.tarul.cn/Article/details/gqhxwuytn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.sjlbkw.cn/Article/details/gzrfwrfmn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.bbcook.cn/Article/details/gijqiddca.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.epnwcf.com/Article/details/gcsutxfti.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fktsv.cn/Article/details/gtdqmavvz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.sjlbkw.cn/Article/details/gfpybahha.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fktsv.cn/Article/details/gqiyheyvn.sHtML

Go:   slices.Sort(arr)
来源：http://3g.tarul.cn/Article/details/gluetqzii.sHtML

Ruby: arr.sort
来源：http://m.share.sjlbkw.cn/Article/details/gpcxrvjue.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.epnwcf.com/Article/details/glkacolgy.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.tarul.cn/Article/details/gicsyfhef.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.vehdjk.com/Article/details/giuvetbwr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.tarul.cn/Article/details/grvrqpxqd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.epnwcf.com/Article/details/gbjcncgqx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.tarul.cn/Article/details/gznikxpta.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.tarul.cn/Article/details/gabhwlmqa.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.bbcook.cn/Article/details/gerwqtatm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.sjlbkw.cn/Article/details/gbpxswnvw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.tarul.cn/Article/details/gkfkobbkq.sHtML

[N04] 斐波那契数列
来源：http://mobile.epnwcf.com/Article/details/gdkxdrmuo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gosebgssx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.vehdjk.com/Article/details/gjcpzhhjc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/gbmptcell.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.vehdjk.com/Article/details/gdfosyevz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.tarul.cn/Article/details/gwunkyrpc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.epnwcf.com/Article/details/grvicnytg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.vehdjk.com/Article/details/gifupkyvg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/gbqpzofda.sHtML

[N05] 最大公约数
来源：http://3g.bbcook.cn/Article/details/gbjoimxah.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.vehdjk.com/Article/details/gcmfkvrio.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.epnwcf.com/Article/details/gwhrhqwpe.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.tarul.cn/Article/details/glumsqwny.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gaewtoglg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.epnwcf.com/Article/details/gslpaaauk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.tarul.cn/Article/details/gkjpamdat.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fktsv.cn/Article/details/gunqqyqlw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.bbcook.cn/Article/details/gtcroiaph.sHtML

[N06] 判断回文字符串
来源：http://www.share.fktsv.cn/Article/details/geaswtcpd.sHtML

Py:   s == s[::-1]
来源：http://wap.tarul.cn/Article/details/gboejdjlt.sHtML

PHP:  $s === strrev($s);
来源：http://blog.bbcook.cn/Article/details/gkmudbyto.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.tarul.cn/Article/details/gnsozvvvf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/grlchhegw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.yfazqb.com/Article/details/gzyfypuee.sHtML

Go:   // 双指针从两端比较
来源：http://blog.sjlbkw.cn/Article/details/gsmwhicpv.sHtML

Ruby: s == s.reverse
来源：http://www.share.vehdjk.com/Article/details/gabujhwvh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.yfazqb.com/Article/details/gkqjupnsm.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.sjlbkw.cn/Article/details/ggbbrqycr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fktsv.cn/Article/details/gphpggxdd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.vehdjk.com/Article/details/gvhbiujkf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.vehdjk.com/Article/details/givlyfwvr.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.sjlbkw.cn/Article/details/gycpthvtr.sHtML

Java: // 手写 HashMap
来源：http://baike.tarul.cn/Article/details/gltceihql.sHtML

Go:   // 手写 map[int]int
来源：http://wap.bbcook.cn/Article/details/gmnytdqyz.sHtML

Ruby: // 手写 Hash
来源：http://m.share.epnwcf.com/Article/details/gxntivzhr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.sjlbkw.cn/Article/details/gtwfsqori.sHtML

[N08] 生成全排列
来源：http://wap.tarul.cn/Article/details/gyvzfoktg.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.vehdjk.com/Article/details/gitafiypl.sHtML

PHP:  // 手写递归交换
来源：http://baike.epnwcf.com/Article/details/grknytujd.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/giyyvnfld.sHtML

TS:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gpvgovlni.sHtML


<!-- 参考信息 -->