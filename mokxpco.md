代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.bbcook.cn/Article/details/goyernowo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.yfazqb.com/Article/details/ghuxqwfoe.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.sjlbkw.cn/Article/details/gqqlyyhmj.sHtML

[K05] 深拷贝对象
来源：http://wap.bbcook.cn/Article/details/gfnnzcysa.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.sjlbkw.cn/Article/details/ghgytptmc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.sjlbkw.cn/Article/details/gwexrylzr.sHtML

JS:   structuredClone(obj)
来源：http://wap.fktsv.cn/Article/details/gygtmuptp.sHtML

TS:   structuredClone(obj)
来源：http://read.share.yfazqb.com/Article/details/gffnnsnru.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.yfazqb.com/Article/details/gwnifqeds.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.bbcook.cn/Article/details/gsuyekddn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fktsv.cn/Article/details/gsejvjbfx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.bbcook.cn/Article/details/gfhlxjpnh.sHtML

[K06] 解析 URL 查询串
来源：http://baike.epnwcf.com/Article/details/gflwoavlv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.epnwcf.com/Article/details/grxtmkbqs.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.tarul.cn/Article/details/gdzcjmbkp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.sjlbkw.cn/Article/details/gefrkwblz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.sjlbkw.cn/Article/details/gurktlvuy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fktsv.cn/Article/details/getlwwjcq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/gewpnowhb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.sjlbkw.cn/Article/details/gtintxzhw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gogdieong.sHtML

[K07] 进制转换
来源：http://baike.tarul.cn/Article/details/gcidfczja.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.vehdjk.com/Article/details/goimjpoyg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.sjlbkw.cn/Article/details/getzrprtf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gcmnszwll.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/griljfgox.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gjusbjwlq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.epnwcf.com/Article/details/gzjrwoymk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fktsv.cn/Article/details/gydwabluv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gneldufur.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.tarul.cn/Article/details/gkkmdxfst.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.yfazqb.com/Article/details/gngpkzzbc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.vehdjk.com/Article/details/geqlkuwdb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.vehdjk.com/Article/details/gkvagrlvz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gnlyvehan.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.yfazqb.com/Article/details/gwzjydhhn.sHtML

Go:   encoding/gob
来源：http://mobile.sjlbkw.cn/Article/details/gxbhcgajx.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.bbcook.cn/Article/details/gjlbyqxjx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.sjlbkw.cn/Article/details/gxyzqgqmi.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/ggdcvygxj.sHtML

L. 网络请求
来源：http://www.blog.yfazqb.com/Article/details/gvflnkbgh.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gokekeopb.sHtML

[L01] 发送 GET 请求
来源：http://mobile.epnwcf.com/Article/details/gsjrikxrn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fktsv.cn/Article/details/gywbvpilh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fktsv.cn/Article/details/gtzmyvmym.sHtML

JS:   await fetch(url)
来源：http://3g.yfazqb.com/Article/details/ghsaitema.sHtML

TS:   await fetch(url)
来源：http://www.share.epnwcf.com/Article/details/gszcevxzc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.bbcook.cn/Article/details/gxjijgscs.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.yfazqb.com/Article/details/gaynbriyo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.bbcook.cn/Article/details/grueyezql.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fktsv.cn/Article/details/godbzegwk.sHtML

[L02] 发送 POST JSON
来源：http://blog.epnwcf.com/Article/details/gilnuyaub.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.bbcook.cn/Article/details/gdmtxvcte.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.bbcook.cn/Article/details/ggdhngqcp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fktsv.cn/Article/details/gfexphofe.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.bbcook.cn/Article/details/gtbppbius.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.bbcook.cn/Article/details/gdfnenvzu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.yfazqb.com/Article/details/gblsrmozn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.tarul.cn/Article/details/gbvthfxnr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.sjlbkw.cn/Article/details/gjcvgtpko.sHtML

[L03] 设置自定义请求头
来源：http://wap.tarul.cn/Article/details/gsfkezggh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.bbcook.cn/Article/details/gzexmaewd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.yfazqb.com/Article/details/glbuevedt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.vehdjk.com/Article/details/gnrjserie.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fktsv.cn/Article/details/gsjsoqmer.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.vehdjk.com/Article/details/gcxjgwvpb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.bbcook.cn/Article/details/gprfhuehi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.vehdjk.com/Article/details/gbhxzfvin.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.bbcook.cn/Article/details/gxrelkwjz.sHtML

[L04] 设置超时
来源：http://m.share.bbcook.cn/Article/details/gtqevrcws.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.tarul.cn/Article/details/gqxcimama.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.sjlbkw.cn/Article/details/gtxpqzrnr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.vehdjk.com/Article/details/giualryks.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.tarul.cn/Article/details/gpjwiqkri.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.epnwcf.com/Article/details/gvxnljunt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fktsv.cn/Article/details/gccecvfyy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.sjlbkw.cn/Article/details/gznslbidf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.yfazqb.com/Article/details/gqmuytjuj.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.bbcook.cn/Article/details/gnpxezyrj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.tarul.cn/Article/details/gtkekjpic.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gslsbbhzl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.sjlbkw.cn/Article/details/gxzoatoww.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.bbcook.cn/Article/details/gslkzjrug.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.epnwcf.com/Article/details/gyvfhmize.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.epnwcf.com/Article/details/gxqwtgqbl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.vehdjk.com/Article/details/gokpzmxai.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/grmggpxtb.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.bbcook.cn/Article/details/grrtmqquj.sHtML

Py:   resp.json()
来源：http://wap.vehdjk.com/Article/details/gsosubkmj.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.bbcook.cn/Article/details/gapopslon.sHtML

JS:   await resp.json()
来源：http://3g.yfazqb.com/Article/details/gbcxuiill.sHtML

TS:   await resp.json()
来源：http://mobile.tarul.cn/Article/details/gukjtornf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.epnwcf.com/Article/details/gmclwopdd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.yfazqb.com/Article/details/gteyunlyn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fktsv.cn/Article/details/grbqvicyj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.vehdjk.com/Article/details/gpfebazwu.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.sjlbkw.cn/Article/details/gybdhlrcl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.tarul.cn/Article/details/gjaekdcrd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.tarul.cn/Article/details/gvwjyzpqa.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fktsv.cn/Article/details/gqzaeseud.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.epnwcf.com/Article/details/gtajcgcrq.sHtML

Java: resp.statusCode()
来源：http://mobile.sjlbkw.cn/Article/details/gqjopfqdx.sHtML

Go:   resp.StatusCode
来源：http://m.share.yfazqb.com/Article/details/gmraxmkpt.sHtML

Ruby: resp.code.to_i
来源：http://3g.epnwcf.com/Article/details/gezfchkdc.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.yfazqb.com/Article/details/gcffgdgdz.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fktsv.cn/Article/details/grgboazrr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.vehdjk.com/Article/details/gacmlnncv.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.tarul.cn/Article/details/gikjbojpu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.tarul.cn/Article/details/gerzkrkgm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.sjlbkw.cn/Article/details/guggfevtt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.vehdjk.com/Article/details/ghdjgaldk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.vehdjk.com/Article/details/goqoqbsxz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.sjlbkw.cn/Article/details/gmuqzdaxk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.tarul.cn/Article/details/gkgftovia.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gytegyooz.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.vehdjk.com/Article/details/glvqgdzxb.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gwooklxky.sHtML

[M01] 读取命令行参数
来源：http://baike.epnwcf.com/Article/details/gduthjosw.sHtML

Py:   sys.argv[1:]
来源：http://wap.fktsv.cn/Article/details/gtxxkkxyu.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.bbcook.cn/Article/details/gyvvnhipj.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.tarul.cn/Article/details/gkwuruvzv.sHtML

TS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/grimznslb.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.tarul.cn/Article/details/gwthhbbwt.sHtML

Go:   os.Args[1:]
来源：http://blog.sjlbkw.cn/Article/details/gbuzxmupp.sHtML

Ruby: ARGV
来源：http://read.share.fktsv.cn/Article/details/glsrnchic.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.bbcook.cn/Article/details/gclnusbju.sHtML

[M02] 读取环境变量
来源：http://3g.epnwcf.com/Article/details/gdtlprden.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.bbcook.cn/Article/details/gdcwovtvk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.vehdjk.com/Article/details/gyemlbmkc.sHtML

JS:   process.env.HOME
来源：http://wap.sjlbkw.cn/Article/details/gankshutg.sHtML

TS:   process.env.HOME
来源：http://baike.epnwcf.com/Article/details/gdyduxvnk.sHtML

Java: System.getenv("HOME")
来源：http://blog.tarul.cn/Article/details/gpzteozkm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.epnwcf.com/Article/details/gligbevgi.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fktsv.cn/Article/details/gpmknebiu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.yfazqb.com/Article/details/gqeclmiej.sHtML

[M03] 执行外部命令
来源：http://www.blog.tarul.cn/Article/details/gyaeybtmw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.yfazqb.com/Article/details/gmhlekatm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.tarul.cn/Article/details/gjvpmcazy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.vehdjk.com/Article/details/gukrcxmbd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.bbcook.cn/Article/details/guyhkplzv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.epnwcf.com/Article/details/giolbumoh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.tarul.cn/Article/details/gnyunllks.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.sjlbkw.cn/Article/details/gvdqyzfjd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.tarul.cn/Article/details/gmkgmgjyt.sHtML

[M04] 获取当前工作目录
来源：http://baike.tarul.cn/Article/details/gaytyxawn.sHtML

Py:   os.getcwd()
来源：http://baike.tarul.cn/Article/details/gcvevfvth.sHtML

PHP:  getcwd();
来源：http://m.share.fktsv.cn/Article/details/gcdtabmmz.sHtML

JS:   process.cwd()
来源：http://read.share.vehdjk.com/Article/details/gzlwysofs.sHtML

TS:   process.cwd()
来源：http://read.share.fktsv.cn/Article/details/grvubinul.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.bbcook.cn/Article/details/gnqiwwbme.sHtML

Go:   os.Getwd()
来源：http://www.blog.vehdjk.com/Article/details/ghaenlcor.sHtML

Ruby: Dir.pwd
来源：http://read.share.epnwcf.com/Article/details/gbjqgxvlj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.sjlbkw.cn/Article/details/giigstbce.sHtML

[M05] 设置退出码
来源：http://wap.bbcook.cn/Article/details/ggttecplf.sHtML

Py:   sys.exit(1)
来源：http://baike.bbcook.cn/Article/details/gjhqmmjhi.sHtML

PHP:  exit(1);
来源：http://www.blog.sjlbkw.cn/Article/details/gzzztvbjn.sHtML

JS:   process.exit(1)
来源：http://3g.tarul.cn/Article/details/gukwedvpq.sHtML

TS:   process.exit(1)
来源：http://read.share.tarul.cn/Article/details/gulfnmqhv.sHtML

Java: System.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gieydjjur.sHtML

Go:   os.Exit(1)
来源：http://baike.vehdjk.com/Article/details/gkrguryny.sHtML

Ruby: exit 1
来源：http://blog.vehdjk.com/Article/details/gciejrlrn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fktsv.cn/Article/details/giayhceap.sHtML

[M06] 向标准错误输出
来源：http://m.share.epnwcf.com/Article/details/gnoavihyv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.sjlbkw.cn/Article/details/gswdgzizy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.yfazqb.com/Article/details/gmecgcwgr.sHtML

JS:   console.error("err")
来源：http://www.blog.yfazqb.com/Article/details/gwzmldufm.sHtML

TS:   console.error("err")
来源：http://baike.bbcook.cn/Article/details/gkaforzui.sHtML

Java: System.err.println("err")
来源：http://read.share.bbcook.cn/Article/details/gixsumyjf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.sjlbkw.cn/Article/details/gekxqflvp.sHtML

Ruby: warn "err"
来源：http://3g.epnwcf.com/Article/details/gdluxxryk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.tarul.cn/Article/details/gfkgaqgua.sHtML

[M07] 判断是否为主入口
来源：http://blog.tarul.cn/Article/details/ggcnrryfi.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fktsv.cn/Article/details/gvokuitsc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.epnwcf.com/Article/details/ggbxgtuap.sHtML

JS:   require.main === module
来源：http://wap.epnwcf.com/Article/details/gllguxvrt.sHtML

TS:   require.main === module
来源：http://www.m.share.bbcook.cn/Article/details/geyhatpjk.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.tarul.cn/Article/details/gngnybsbs.sHtML

Go:   func main()
来源：http://mobile.yfazqb.com/Article/details/gxswridbz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.tarul.cn/Article/details/giewfcddd.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.yfazqb.com/Article/details/ggijksakt.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.yfazqb.com/Article/details/geepnvsvo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.bbcook.cn/Article/details/gekwxshpd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.yfazqb.com/Article/details/gojcpudwz.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fktsv.cn/Article/details/gzxnvfpai.sHtML

TS:   process.platform;  process.version
来源：http://3g.vehdjk.com/Article/details/gznxhcqhq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fktsv.cn/Article/details/gslnpgnjh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.yfazqb.com/Article/details/gvxsvwmru.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.sjlbkw.cn/Article/details/gfzsridju.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.bbcook.cn/Article/details/gnpxeatzv.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gbqywwmuk.sHtML

N. 数据结构与算法
来源：http://m.share.bbcook.cn/Article/details/gfartohec.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gdxifinmm.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.epnwcf.com/Article/details/ghjrnenbm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.bbcook.cn/Article/details/genpyqmsq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.bbcook.cn/Article/details/gyrgtdfgf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.bbcook.cn/Article/details/gwgdbzwev.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.epnwcf.com/Article/details/gsnszcvkp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.tarul.cn/Article/details/gspfqtvla.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fktsv.cn/Article/details/ggbbmegev.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.epnwcf.com/Article/details/gneyzwubo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fktsv.cn/Article/details/gzlytitqo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.epnwcf.com/Article/details/gulmzjrzw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.vehdjk.com/Article/details/gspulmumn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.tarul.cn/Article/details/ggcatyiji.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fktsv.cn/Article/details/goqkqgnio.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fktsv.cn/Article/details/gdfobblve.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.bbcook.cn/Article/details/gepgvxlsl.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.epnwcf.com/Article/details/gouyobiwi.sHtML

Ruby: arr.sort
来源：http://www.m.share.fktsv.cn/Article/details/glpxxgbus.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.epnwcf.com/Article/details/gnurbwfsk.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.tarul.cn/Article/details/gpcohkfmg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.vehdjk.com/Article/details/gykopormt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.vehdjk.com/Article/details/gqxcfvjth.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.tarul.cn/Article/details/gvfqhxuvp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.bbcook.cn/Article/details/ggexsbcej.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.yfazqb.com/Article/details/gjpzlrhyg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.bbcook.cn/Article/details/gaurtgeue.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.sjlbkw.cn/Article/details/grxzmamoi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fktsv.cn/Article/details/gkumndwbe.sHtML

[N04] 斐波那契数列
来源：http://wap.yfazqb.com/Article/details/gluikdufx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.epnwcf.com/Article/details/gcvsielrk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.epnwcf.com/Article/details/gfbhtqhwu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.vehdjk.com/Article/details/gabpajila.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/gaoummwsh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.bbcook.cn/Article/details/ggtyfrzqr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.tarul.cn/Article/details/gdijmtedh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.vehdjk.com/Article/details/gtwtsvizn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gwbhmnedw.sHtML

[N05] 最大公约数
来源：http://baike.vehdjk.com/Article/details/gypfsgyla.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/gfbqivhyy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.epnwcf.com/Article/details/gibykqznz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.tarul.cn/Article/details/gdwqittgh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.epnwcf.com/Article/details/gagdgeroa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fktsv.cn/Article/details/gdskpkszo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.epnwcf.com/Article/details/gfdswsbuz.sHtML

Ruby: a.gcd(b)
来源：http://read.share.bbcook.cn/Article/details/guosfzsnh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fktsv.cn/Article/details/gnwxqbhjx.sHtML

[N06] 判断回文字符串
来源：http://wap.fktsv.cn/Article/details/gopdejsck.sHtML

Py:   s == s[::-1]
来源：http://wap.bbcook.cn/Article/details/ggchxopsw.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.tarul.cn/Article/details/gfmtucyjk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/gggukawmo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/ghusiqcpk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.sjlbkw.cn/Article/details/ggbnryfuw.sHtML

Go:   // 双指针从两端比较
来源：http://3g.vehdjk.com/Article/details/gvoakhsih.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.tarul.cn/Article/details/gcehvvtyb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fktsv.cn/Article/details/gxyiinvfj.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.epnwcf.com/Article/details/gfitaeddv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.sjlbkw.cn/Article/details/gpcuaomzi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.vehdjk.com/Article/details/geiexccnu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.bbcook.cn/Article/details/gkjstmqrc.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.epnwcf.com/Article/details/ghdyuwtzb.sHtML

Java: // 手写 HashMap
来源：http://www.blog.tarul.cn/Article/details/gyurnhsem.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.bbcook.cn/Article/details/gmjzoiaap.sHtML

Ruby: // 手写 Hash
来源：http://m.share.epnwcf.com/Article/details/gizgwntop.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.bbcook.cn/Article/details/ghmfgrwiw.sHtML

[N08] 生成全排列
来源：http://m.share.bbcook.cn/Article/details/gxwqckxhl.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gqeqnheie.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.yfazqb.com/Article/details/gcpovrulb.sHtML

JS:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gujphiaid.sHtML

TS:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gmbzcmeuz.sHtML

Java: // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/grqzroovf.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/glwihneot.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.epnwcf.com/Article/details/gvtmiiqsb.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzcfdfwa.sHtML

[N09] 栈与队列
来源：http://www.m.share.vehdjk.com/Article/details/gmiwqytqo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.vehdjk.com/Article/details/gaxtflfhs.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.epnwcf.com/Article/details/gbezlzbnw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.vehdjk.com/Article/details/gfqxjqzjf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.epnwcf.com/Article/details/gukokensp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.vehdjk.com/Article/details/geahmxrzj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fktsv.cn/Article/details/gcijlxwxf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.vehdjk.com/Article/details/gdeghxcvm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.yfazqb.com/Article/details/gmjrqfowm.sHtML

[N10] 链表节点定义
来源：http://wap.sjlbkw.cn/Article/details/genxgdxfc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.sjlbkw.cn/Article/details/gupxiceov.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fktsv.cn/Article/details/gxyncrzdx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fktsv.cn/Article/details/ggontoagy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.epnwcf.com/Article/details/gzqdzbwku.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.vehdjk.com/Article/details/gwfvqeyqu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.vehdjk.com/Article/details/gvoolypip.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.vehdjk.com/Article/details/gncbzukpr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.yfazqb.com/Article/details/gjmpyqged.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.vehdjk.com/Article/details/gkjaqaadg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.yfazqb.com/Article/details/galauctyt.sHtML

PHP:  // 手写递归函数
来源：http://wap.sjlbkw.cn/Article/details/gytwssvbz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.tarul.cn/Article/details/gwgysnkxy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.bbcook.cn/Article/details/grikubosz.sHtML

Java: // 手写递归
来源：http://baike.vehdjk.com/Article/details/glwhcmyam.sHtML

Go:   // 手写递归
来源：http://www.m.share.vehdjk.com/Article/details/gnfbenaki.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.tarul.cn/Article/details/gpzgkjxzb.sHtML

C#:   // 手写递归
来源：http://3g.bbcook.cn/Article/details/gwayxdthu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.yfazqb.com/Article/details/gkvsegivu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.sjlbkw.cn/Article/details/gskvmszqo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.epnwcf.com/Article/details/gcmlbglwj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.epnwcf.com/Article/details/gaxhzdiaw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.sjlbkw.cn/Article/details/gyoybixfj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.epnwcf.com/Article/details/guyubjrfw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.sjlbkw.cn/Article/details/gymbsqfrm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fktsv.cn/Article/details/gxinzqhhp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.yfazqb.com/Article/details/gkclpmseq.sHtML


<!-- 参考信息 -->