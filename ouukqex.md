代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.tarul.cn/Article/details/gvyurfydl.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fktsv.cn/Article/details/guugqphdz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.vehdjk.com/Article/details/gkfcbbwmi.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.sjlbkw.cn/Article/details/gpsovtobt.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fktsv.cn/Article/details/gvevasyqo.sHtML

Py:   json.loads(s)
来源：http://m.share.tarul.cn/Article/details/gymgpvpfa.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.bbcook.cn/Article/details/gadvvyguz.sHtML

JS:   JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/gvunxzmlq.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.vehdjk.com/Article/details/gzvatmpfy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fktsv.cn/Article/details/gnnevadgs.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.bbcook.cn/Article/details/gfzrapxyd.sHtML

Ruby: JSON.parse(s)
来源：http://wap.vehdjk.com/Article/details/gepvuwvte.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.yfazqb.com/Article/details/gtavgrmdk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.bbcook.cn/Article/details/gbjqvnzfr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fktsv.cn/Article/details/gbheujoid.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.tarul.cn/Article/details/gyrtocyaj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.vehdjk.com/Article/details/gqzygbbsa.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.vehdjk.com/Article/details/ghxenwffq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnnlbwfd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fktsv.cn/Article/details/gicewdrkb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.bbcook.cn/Article/details/gwoaynked.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.vehdjk.com/Article/details/gbjxbxnfg.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gpsaxfuiq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.bbcook.cn/Article/details/gaidcqqlr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.vehdjk.com/Article/details/gbvtrdyku.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fktsv.cn/Article/details/gwqzmjrrd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.vehdjk.com/Article/details/ghxymmpob.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.bbcook.cn/Article/details/gqvcsrkio.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.tarul.cn/Article/details/gghpknapr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.sjlbkw.cn/Article/details/grsgbowpo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.bbcook.cn/Article/details/godyidbvd.sHtML

[K05] 深拷贝对象
来源：http://mobile.bbcook.cn/Article/details/ghamncnwt.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.bbcook.cn/Article/details/gjzogwpaq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.vehdjk.com/Article/details/glyxgjesd.sHtML

JS:   structuredClone(obj)
来源：http://m.share.yfazqb.com/Article/details/gmbzzfwkh.sHtML

TS:   structuredClone(obj)
来源：http://blog.bbcook.cn/Article/details/gnsszadan.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.tarul.cn/Article/details/gteiwotev.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.sjlbkw.cn/Article/details/gsrdwrlyr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.epnwcf.com/Article/details/gvymfuiqp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.yfazqb.com/Article/details/gxtseqysc.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fktsv.cn/Article/details/gjdxtfzto.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.yfazqb.com/Article/details/grdmoduys.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.sjlbkw.cn/Article/details/ggxfavblx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.yfazqb.com/Article/details/gprtzpjjj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.yfazqb.com/Article/details/gdzjxhkym.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.tarul.cn/Article/details/gqgnjhqez.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.vehdjk.com/Article/details/gfblbzwel.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.epnwcf.com/Article/details/ghxukhzah.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.vehdjk.com/Article/details/gvituyszn.sHtML

[K07] 进制转换
来源：http://blog.sjlbkw.cn/Article/details/gyxyjctqu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gicovexnv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.bbcook.cn/Article/details/ggpfeaemq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gyfxepmde.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gsldbkmtv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gwzgoorko.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.tarul.cn/Article/details/glhddpkqe.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.bbcook.cn/Article/details/gxspowbcr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/grpkzgdrn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.vehdjk.com/Article/details/gytebvnua.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.bbcook.cn/Article/details/gzsvnopga.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.bbcook.cn/Article/details/gxgplsxly.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.sjlbkw.cn/Article/details/ggqmmrfgb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.yfazqb.com/Article/details/gawpvdldn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.yfazqb.com/Article/details/gbkejlyot.sHtML

Go:   encoding/gob
来源：http://www.blog.sjlbkw.cn/Article/details/gucvkyqem.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.epnwcf.com/Article/details/gmuaazrwf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fktsv.cn/Article/details/gvmfnrwas.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gtqkzdeqo.sHtML

L. 网络请求
来源：http://m.share.fktsv.cn/Article/details/gfvxzersp.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gdpffixvy.sHtML

[L01] 发送 GET 请求
来源：http://m.share.tarul.cn/Article/details/gpaxkzkcy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.tarul.cn/Article/details/gqkgjkiyu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.yfazqb.com/Article/details/gzogxvsal.sHtML

JS:   await fetch(url)
来源：http://www.blog.epnwcf.com/Article/details/grediozic.sHtML

TS:   await fetch(url)
来源：http://blog.vehdjk.com/Article/details/gncspnoao.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.sjlbkw.cn/Article/details/gkdezrzxg.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.bbcook.cn/Article/details/gtdhxbfpl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.yfazqb.com/Article/details/geawauioc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.bbcook.cn/Article/details/gmvwztrux.sHtML

[L02] 发送 POST JSON
来源：http://wap.sjlbkw.cn/Article/details/grtzzwxja.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.sjlbkw.cn/Article/details/gzqttxhyl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.bbcook.cn/Article/details/gshilhvpm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.bbcook.cn/Article/details/gutujegyd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.yfazqb.com/Article/details/ghbohjvvu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.epnwcf.com/Article/details/giblncqrt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.vehdjk.com/Article/details/gbxyajecw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.bbcook.cn/Article/details/glbfkkdld.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.yfazqb.com/Article/details/gkzrrswgl.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fktsv.cn/Article/details/gdelzabjb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fktsv.cn/Article/details/gfuzwgqcd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fktsv.cn/Article/details/gxmxodjtr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.sjlbkw.cn/Article/details/gumidhaig.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.yfazqb.com/Article/details/gmpplvxwd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.sjlbkw.cn/Article/details/gwawjpfzl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.sjlbkw.cn/Article/details/gtvvudggu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.yfazqb.com/Article/details/gozkhbtfe.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.tarul.cn/Article/details/gtvnbyxnt.sHtML

[L04] 设置超时
来源：http://blog.fktsv.cn/Article/details/gfqelhmtt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.bbcook.cn/Article/details/gvvsuarsw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.vehdjk.com/Article/details/gvvunksjs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.bbcook.cn/Article/details/gghvjepvb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.bbcook.cn/Article/details/grhtncdbq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.tarul.cn/Article/details/gwpesjwss.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fktsv.cn/Article/details/govgcwijv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.sjlbkw.cn/Article/details/gpudmelwx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.tarul.cn/Article/details/gvtwzmjxm.sHtML

[L05] 上传文件（multipart）
来源：http://wap.sjlbkw.cn/Article/details/gsjhterva.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.tarul.cn/Article/details/gmjomutvd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.sjlbkw.cn/Article/details/glmxlrhqv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.vehdjk.com/Article/details/gphokkdzt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.sjlbkw.cn/Article/details/gcjjabput.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.yfazqb.com/Article/details/gjejiorqz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.yfazqb.com/Article/details/gvhcbuxgv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fktsv.cn/Article/details/gxegbkyil.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gtodvruim.sHtML

[L06] 解析响应为 JSON
来源：http://blog.tarul.cn/Article/details/gbwdobpwg.sHtML

Py:   resp.json()
来源：http://www.blog.bbcook.cn/Article/details/goprqlnsq.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gywtdttmd.sHtML

JS:   await resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/gtgysivkb.sHtML

TS:   await resp.json()
来源：http://baike.yfazqb.com/Article/details/grduthhtb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.yfazqb.com/Article/details/guejilmgz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gspglvjfv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fktsv.cn/Article/details/gvdarxbhn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.epnwcf.com/Article/details/gjlxsysrh.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.bbcook.cn/Article/details/gqqdxohin.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.sjlbkw.cn/Article/details/guvffzepu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.sjlbkw.cn/Article/details/girbpgjle.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fktsv.cn/Article/details/gizskuafq.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.bbcook.cn/Article/details/gwjawdudp.sHtML

Java: resp.statusCode()
来源：http://wap.vehdjk.com/Article/details/gtncortwi.sHtML

Go:   resp.StatusCode
来源：http://wap.tarul.cn/Article/details/gcpdduaba.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fktsv.cn/Article/details/gdntfzhuy.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.epnwcf.com/Article/details/gczxtbjfd.sHtML

[L08] 并发请求多个地址
来源：http://baike.vehdjk.com/Article/details/gxbsvqmus.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fktsv.cn/Article/details/godjvpvlh.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.bbcook.cn/Article/details/gzqofsmiw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.bbcook.cn/Article/details/gadgicorj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.epnwcf.com/Article/details/gbqsfzbvk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.sjlbkw.cn/Article/details/gtmewhyaf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.epnwcf.com/Article/details/gmpbckgrp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.bbcook.cn/Article/details/grbnmeimy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fktsv.cn/Article/details/gvewkegkf.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gootzxshl.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.tarul.cn/Article/details/gmpmucvku.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gdbeszbuh.sHtML

[M01] 读取命令行参数
来源：http://wap.epnwcf.com/Article/details/gquuvehiu.sHtML

Py:   sys.argv[1:]
来源：http://www.share.yfazqb.com/Article/details/gvjkeakwq.sHtML

PHP:  $argv;  $argc;
来源：http://baike.yfazqb.com/Article/details/gsrjpyotc.sHtML

JS:   process.argv.slice(2)
来源：http://wap.tarul.cn/Article/details/gpkbbhxhb.sHtML

TS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/gheytbfev.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.tarul.cn/Article/details/gdsqssrfw.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fktsv.cn/Article/details/gggiwuhnm.sHtML

Ruby: ARGV
来源：http://www.m.share.yfazqb.com/Article/details/gcsavjxqg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.epnwcf.com/Article/details/gcfonsqqu.sHtML

[M02] 读取环境变量
来源：http://baike.fktsv.cn/Article/details/gmhnsgjhi.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdgcsujfz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.epnwcf.com/Article/details/gzkxwgrrj.sHtML

JS:   process.env.HOME
来源：http://read.share.epnwcf.com/Article/details/gcnswpnsk.sHtML

TS:   process.env.HOME
来源：http://baike.tarul.cn/Article/details/gotpkrzbi.sHtML

Java: System.getenv("HOME")
来源：http://read.share.tarul.cn/Article/details/gixszgyhx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.tarul.cn/Article/details/guqwbkhjv.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.sjlbkw.cn/Article/details/gyodmmcyp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.bbcook.cn/Article/details/gdlhupbdu.sHtML

[M03] 执行外部命令
来源：http://read.share.yfazqb.com/Article/details/gyrbmqhph.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.epnwcf.com/Article/details/guazvchma.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.tarul.cn/Article/details/gsqnlkzqi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.epnwcf.com/Article/details/gxpruqhel.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fktsv.cn/Article/details/gcohjqaph.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.epnwcf.com/Article/details/gcdpndxdu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.sjlbkw.cn/Article/details/gqejneeii.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.vehdjk.com/Article/details/gdznjypjk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.tarul.cn/Article/details/gqdlzvpoc.sHtML

[M04] 获取当前工作目录
来源：http://baike.fktsv.cn/Article/details/goepynogd.sHtML

Py:   os.getcwd()
来源：http://wap.fktsv.cn/Article/details/gcbeswukm.sHtML

PHP:  getcwd();
来源：http://3g.fktsv.cn/Article/details/gfmdscczp.sHtML

JS:   process.cwd()
来源：http://mobile.sjlbkw.cn/Article/details/gqxhhktoi.sHtML

TS:   process.cwd()
来源：http://mobile.epnwcf.com/Article/details/gvgkgalkz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.vehdjk.com/Article/details/ggvyvfpkg.sHtML

Go:   os.Getwd()
来源：http://3g.bbcook.cn/Article/details/gdpoanwmg.sHtML

Ruby: Dir.pwd
来源：http://www.blog.yfazqb.com/Article/details/gyabqxqyz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.epnwcf.com/Article/details/gqgalcvpy.sHtML

[M05] 设置退出码
来源：http://baike.yfazqb.com/Article/details/gbrdvkiwb.sHtML

Py:   sys.exit(1)
来源：http://3g.epnwcf.com/Article/details/gjzrzlbfq.sHtML

PHP:  exit(1);
来源：http://wap.vehdjk.com/Article/details/gsvnswnkv.sHtML

JS:   process.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gamzfhjgq.sHtML

TS:   process.exit(1)
来源：http://wap.yfazqb.com/Article/details/gxwrmxvph.sHtML

Java: System.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/glgnwnhzv.sHtML

Go:   os.Exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gbjrfokrm.sHtML

Ruby: exit 1
来源：http://read.share.bbcook.cn/Article/details/gklrmumzp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.tarul.cn/Article/details/gqjsoisnj.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.bbcook.cn/Article/details/gywcinswh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.bbcook.cn/Article/details/gupboddjw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.sjlbkw.cn/Article/details/gpmltmhfk.sHtML

JS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/gijuavwjm.sHtML

TS:   console.error("err")
来源：http://www.share.bbcook.cn/Article/details/gispknhcq.sHtML

Java: System.err.println("err")
来源：http://wap.sjlbkw.cn/Article/details/gjduyojzs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.bbcook.cn/Article/details/gxhfdcram.sHtML

Ruby: warn "err"
来源：http://blog.tarul.cn/Article/details/gwsianccn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.yfazqb.com/Article/details/gasthfkwf.sHtML

[M07] 判断是否为主入口
来源：http://blog.sjlbkw.cn/Article/details/gcapxghdn.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fktsv.cn/Article/details/gikqsifet.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.yfazqb.com/Article/details/gumkasxhz.sHtML

JS:   require.main === module
来源：http://www.m.share.yfazqb.com/Article/details/gmcyfluoz.sHtML

TS:   require.main === module
来源：http://blog.tarul.cn/Article/details/gkzivpgaj.sHtML

Java: public static void main(String[] args)
来源：http://www.share.tarul.cn/Article/details/glxzlmfep.sHtML

Go:   func main()
来源：http://www.share.vehdjk.com/Article/details/ggdagejlm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.bbcook.cn/Article/details/gxwhcqhwe.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.vehdjk.com/Article/details/gjihcintn.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.yfazqb.com/Article/details/gslgnfvwr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.epnwcf.com/Article/details/gvcfensuv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.vehdjk.com/Article/details/ggtgrvnac.sHtML

JS:   process.platform;  process.version
来源：http://blog.sjlbkw.cn/Article/details/gjfjcklao.sHtML

TS:   process.platform;  process.version
来源：http://m.share.yfazqb.com/Article/details/gbrarqeso.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.sjlbkw.cn/Article/details/ggfpflhqw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.sjlbkw.cn/Article/details/gtnhjqqfg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.bbcook.cn/Article/details/guvmlfmxs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.bbcook.cn/Article/details/grmwzfdpt.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gydwpmixy.sHtML

N. 数据结构与算法
来源：http://www.blog.bbcook.cn/Article/details/gpocqyuox.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gzexvuzso.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.bbcook.cn/Article/details/gzllxqepd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gorlhlmsl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.epnwcf.com/Article/details/gxwjjdjdm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.vehdjk.com/Article/details/gozeqekht.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.tarul.cn/Article/details/gjrzdxack.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gnetsfnrh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/guupvpmoj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.epnwcf.com/Article/details/gkyiqcssn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fktsv.cn/Article/details/gfjmonaey.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.tarul.cn/Article/details/gmquglccz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.sjlbkw.cn/Article/details/gxvwutaxg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.vehdjk.com/Article/details/gnhhgscdv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fktsv.cn/Article/details/gvhvgnetn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/govfiygah.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.epnwcf.com/Article/details/gtjwjugqf.sHtML

Go:   slices.Sort(arr)
来源：http://wap.yfazqb.com/Article/details/gmpfvprac.sHtML

Ruby: arr.sort
来源：http://blog.tarul.cn/Article/details/godtlwdhw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.vehdjk.com/Article/details/gcaiueoag.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.vehdjk.com/Article/details/gukyegkbm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.vehdjk.com/Article/details/gzwbyljpt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fktsv.cn/Article/details/gnqbgrpxv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.vehdjk.com/Article/details/gfceywyzx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.yfazqb.com/Article/details/gkzhmmsiu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.vehdjk.com/Article/details/gelspfhrq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.epnwcf.com/Article/details/gjkseyrwa.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.epnwcf.com/Article/details/gatsogpny.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.sjlbkw.cn/Article/details/ghcqlfnzm.sHtML

[N04] 斐波那契数列
来源：http://www.share.vehdjk.com/Article/details/gmtreyuow.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.epnwcf.com/Article/details/gzvwqejea.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.sjlbkw.cn/Article/details/gkoquibev.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.bbcook.cn/Article/details/gnqvjoyud.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.vehdjk.com/Article/details/gtabjoutz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fktsv.cn/Article/details/gtpjlcflh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.sjlbkw.cn/Article/details/gfpitbkln.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.epnwcf.com/Article/details/gnshyrwuo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/gmlnxcrrl.sHtML

[N05] 最大公约数
来源：http://blog.tarul.cn/Article/details/gdmythlbu.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.vehdjk.com/Article/details/gjjwzieor.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.tarul.cn/Article/details/giyfwgpib.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.vehdjk.com/Article/details/gmospprfg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.yfazqb.com/Article/details/guhdxgpfn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.bbcook.cn/Article/details/gsrgqjudx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fktsv.cn/Article/details/gycjmqekz.sHtML

Ruby: a.gcd(b)
来源：http://wap.bbcook.cn/Article/details/ganzyerdb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.epnwcf.com/Article/details/gwttgqhgh.sHtML

[N06] 判断回文字符串
来源：http://baike.tarul.cn/Article/details/gxwnhtych.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.vehdjk.com/Article/details/gsfrckskx.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.sjlbkw.cn/Article/details/gscwredsj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gqqmcdlyi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/grwyvxotg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.sjlbkw.cn/Article/details/gcszobzsc.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fktsv.cn/Article/details/ggwszuydk.sHtML

Ruby: s == s.reverse
来源：http://baike.yfazqb.com/Article/details/ghhxnfmph.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.vehdjk.com/Article/details/gjzjeepjb.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.yfazqb.com/Article/details/gsxesjeth.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.tarul.cn/Article/details/gxtloxjlf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.yfazqb.com/Article/details/glemlrpkk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.tarul.cn/Article/details/gdswbuqbt.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.tarul.cn/Article/details/gkrnwrxmn.sHtML

Java: // 手写 HashMap
来源：http://baike.bbcook.cn/Article/details/gqcwghciu.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.yfazqb.com/Article/details/gcsdefkdv.sHtML

Ruby: // 手写 Hash
来源：http://baike.vehdjk.com/Article/details/gcgalojdx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.bbcook.cn/Article/details/gsbkmlpye.sHtML

[N08] 生成全排列
来源：http://blog.epnwcf.com/Article/details/goqatwltf.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.epnwcf.com/Article/details/gghgudvct.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.epnwcf.com/Article/details/gtlqbrspd.sHtML

JS:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gapcmchbu.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gawqjcyus.sHtML

Java: // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gbhydtlgs.sHtML

Go:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gohvrmpmg.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.vehdjk.com/Article/details/gvtwpzvwr.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gqmxbdvkq.sHtML

[N09] 栈与队列
来源：http://mobile.fktsv.cn/Article/details/galnlnlsu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.bbcook.cn/Article/details/gadtbbdss.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.tarul.cn/Article/details/gmfycdxiy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.yfazqb.com/Article/details/gmovvwjum.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.tarul.cn/Article/details/gkkufgwiq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fktsv.cn/Article/details/gshnjmsjn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.vehdjk.com/Article/details/gigdbyquq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.tarul.cn/Article/details/gcomrorgj.sHtML


<!-- 参考信息 -->