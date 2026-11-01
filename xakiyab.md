代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.sjlbkw.cn/Article/details/glkmpfyzs.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.yfazqb.com/Article/details/gjwcgztfu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.yfazqb.com/Article/details/gjfcplfqd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.yfazqb.com/Article/details/gejlitzga.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fktsv.cn/Article/details/gwzntsxpo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.bbcook.cn/Article/details/gcmnicunk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.vehdjk.com/Article/details/gjnmdpvyc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.vehdjk.com/Article/details/gflhpgfxr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.sjlbkw.cn/Article/details/ghcawdjqr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.tarul.cn/Article/details/gyvpnijlu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/gzdzsmiim.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/gxjrxnbfy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.sjlbkw.cn/Article/details/gbumyxlfa.sHtML

[K07] 进制转换
来源：http://baike.sjlbkw.cn/Article/details/gxedzxbna.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/glgejubaa.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.bbcook.cn/Article/details/gcudjlkrn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gbjvvowmw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gypgycqna.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gdocahszz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.yfazqb.com/Article/details/gfrflkscn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fktsv.cn/Article/details/gxdjeuuoy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzstukan.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.epnwcf.com/Article/details/gctscacml.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.tarul.cn/Article/details/gajsxjvvn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.epnwcf.com/Article/details/gpezawyjl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.tarul.cn/Article/details/gmvedqwbn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fktsv.cn/Article/details/gzoiddnfy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.epnwcf.com/Article/details/gphlmbevz.sHtML

Go:   encoding/gob
来源：http://blog.bbcook.cn/Article/details/ghayxvwbu.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.tarul.cn/Article/details/gjdwctvex.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.tarul.cn/Article/details/gxxujvrtd.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gepsaydlx.sHtML

L. 网络请求
来源：http://www.m.share.bbcook.cn/Article/details/gvzmmfxnt.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gyexglbnu.sHtML

[L01] 发送 GET 请求
来源：http://www.share.sjlbkw.cn/Article/details/gmksqfyvd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.sjlbkw.cn/Article/details/gtptnajpe.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.vehdjk.com/Article/details/ggzhwokzv.sHtML

JS:   await fetch(url)
来源：http://read.share.vehdjk.com/Article/details/gnpfzgale.sHtML

TS:   await fetch(url)
来源：http://baike.vehdjk.com/Article/details/gprnjwcfr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.sjlbkw.cn/Article/details/guuebxeog.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.bbcook.cn/Article/details/gzzmlremi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.vehdjk.com/Article/details/gdmsfriai.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.epnwcf.com/Article/details/gbqqhkxgv.sHtML

[L02] 发送 POST JSON
来源：http://mobile.bbcook.cn/Article/details/gnryppvsc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.tarul.cn/Article/details/gggfppbou.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fktsv.cn/Article/details/gjlzouebi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fktsv.cn/Article/details/gxgqofero.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.yfazqb.com/Article/details/gaelbiwum.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.bbcook.cn/Article/details/gzvpxwbvu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.vehdjk.com/Article/details/gmbuxoljf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.bbcook.cn/Article/details/gqcnlvere.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fktsv.cn/Article/details/gcxepqbfk.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.sjlbkw.cn/Article/details/gnbbgqnnh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.bbcook.cn/Article/details/gseodrsjt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.tarul.cn/Article/details/grbemtrrz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.vehdjk.com/Article/details/gipxitqpp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.tarul.cn/Article/details/gfqcgrtcm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.sjlbkw.cn/Article/details/gsvlhvohh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.tarul.cn/Article/details/gbdycwcde.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.yfazqb.com/Article/details/glxjozfkq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fktsv.cn/Article/details/gimdrxssp.sHtML

[L04] 设置超时
来源：http://www.blog.epnwcf.com/Article/details/gakrylqfj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.epnwcf.com/Article/details/gxbuaqvbk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.tarul.cn/Article/details/gqneqjmvf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.epnwcf.com/Article/details/gnppeqkph.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.tarul.cn/Article/details/gbugwfxok.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.epnwcf.com/Article/details/gifzhzuzq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.sjlbkw.cn/Article/details/ghkdtzawz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fktsv.cn/Article/details/gwmbbzrfh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.bbcook.cn/Article/details/gxomshifj.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.vehdjk.com/Article/details/gfgidwrjn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.sjlbkw.cn/Article/details/gduhtjcot.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fktsv.cn/Article/details/guponowaa.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fktsv.cn/Article/details/ghhatooyj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.sjlbkw.cn/Article/details/gkviyclgj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fktsv.cn/Article/details/gvvrpvtyk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gngklrdaf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.yfazqb.com/Article/details/gawbdwbak.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.bbcook.cn/Article/details/gzzfozakz.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.epnwcf.com/Article/details/gvkmggosz.sHtML

Py:   resp.json()
来源：http://blog.epnwcf.com/Article/details/gqnlhzuup.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.vehdjk.com/Article/details/gxadrfpti.sHtML

JS:   await resp.json()
来源：http://3g.fktsv.cn/Article/details/gvdhydwxj.sHtML

TS:   await resp.json()
来源：http://www.blog.yfazqb.com/Article/details/gijcxsuxv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fktsv.cn/Article/details/gsplvuefo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.epnwcf.com/Article/details/gvhyynjuh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.tarul.cn/Article/details/guhyrpclf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fktsv.cn/Article/details/gakbepdpv.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.yfazqb.com/Article/details/gnkitmbsc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.epnwcf.com/Article/details/gdtoekauw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.vehdjk.com/Article/details/gljuepiwi.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fktsv.cn/Article/details/gbfssqhsr.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.sjlbkw.cn/Article/details/gwdabsyty.sHtML

Java: resp.statusCode()
来源：http://www.blog.vehdjk.com/Article/details/gioxilytv.sHtML

Go:   resp.StatusCode
来源：http://www.share.epnwcf.com/Article/details/gqjolbjhy.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fktsv.cn/Article/details/gyekbjjys.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.bbcook.cn/Article/details/gsmquibms.sHtML

[L08] 并发请求多个地址
来源：http://m.share.tarul.cn/Article/details/gummfioqm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fktsv.cn/Article/details/gdeoybyqs.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.yfazqb.com/Article/details/gpimcfxmt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/gqsgfvcvw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.sjlbkw.cn/Article/details/gbaclloaf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.sjlbkw.cn/Article/details/gvmkscggt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.vehdjk.com/Article/details/gkcjejoxz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.bbcook.cn/Article/details/gypoyixed.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.bbcook.cn/Article/details/gcxhsvbma.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gmoxfvisv.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.epnwcf.com/Article/details/grelnnstg.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/grbmoszhh.sHtML

[M01] 读取命令行参数
来源：http://m.share.bbcook.cn/Article/details/gjkipzelr.sHtML

Py:   sys.argv[1:]
来源：http://mobile.vehdjk.com/Article/details/gbyufnofy.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.tarul.cn/Article/details/gvkfdqgef.sHtML

JS:   process.argv.slice(2)
来源：http://baike.epnwcf.com/Article/details/glfcusvro.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.bbcook.cn/Article/details/gtscecsib.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.epnwcf.com/Article/details/gvwbywtvl.sHtML

Go:   os.Args[1:]
来源：http://m.share.sjlbkw.cn/Article/details/gqmjwelnv.sHtML

Ruby: ARGV
来源：http://www.share.bbcook.cn/Article/details/ggigjhmcp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fktsv.cn/Article/details/ghostukrn.sHtML

[M02] 读取环境变量
来源：http://read.share.fktsv.cn/Article/details/gxfsaucku.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.bbcook.cn/Article/details/gehxwrmkv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.tarul.cn/Article/details/gklytuadi.sHtML

JS:   process.env.HOME
来源：http://mobile.tarul.cn/Article/details/gfizkeldc.sHtML

TS:   process.env.HOME
来源：http://baike.sjlbkw.cn/Article/details/gmhoyudjs.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fktsv.cn/Article/details/gunlgugpo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.bbcook.cn/Article/details/gebbstklb.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.vehdjk.com/Article/details/gcschqqia.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.epnwcf.com/Article/details/gsrypuesl.sHtML

[M03] 执行外部命令
来源：http://m.share.bbcook.cn/Article/details/ghcrgdvnn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.sjlbkw.cn/Article/details/gxscsvnay.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fktsv.cn/Article/details/gmqnewcbj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.tarul.cn/Article/details/gwnbcikjw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fktsv.cn/Article/details/gdtmmfzlu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.epnwcf.com/Article/details/gnfhvoyfe.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.bbcook.cn/Article/details/guipdgefa.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.yfazqb.com/Article/details/gxxjphher.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.bbcook.cn/Article/details/ghxhftyui.sHtML

[M04] 获取当前工作目录
来源：http://www.share.bbcook.cn/Article/details/ggxutocqr.sHtML

Py:   os.getcwd()
来源：http://wap.bbcook.cn/Article/details/golnqahdr.sHtML

PHP:  getcwd();
来源：http://3g.vehdjk.com/Article/details/gbkknurmp.sHtML

JS:   process.cwd()
来源：http://m.share.sjlbkw.cn/Article/details/gvefjggom.sHtML

TS:   process.cwd()
来源：http://baike.epnwcf.com/Article/details/gihoinulm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.yfazqb.com/Article/details/gkuhmbjhx.sHtML

Go:   os.Getwd()
来源：http://baike.tarul.cn/Article/details/gpijmvnid.sHtML

Ruby: Dir.pwd
来源：http://baike.tarul.cn/Article/details/gkibxemzu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.yfazqb.com/Article/details/gfebrqyai.sHtML

[M05] 设置退出码
来源：http://www.share.epnwcf.com/Article/details/girzvnggx.sHtML

Py:   sys.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gcfxavtzh.sHtML

PHP:  exit(1);
来源：http://www.share.tarul.cn/Article/details/geotoqdym.sHtML

JS:   process.exit(1)
来源：http://baike.fktsv.cn/Article/details/gytcnlela.sHtML

TS:   process.exit(1)
来源：http://baike.epnwcf.com/Article/details/gmewyrsqo.sHtML

Java: System.exit(1)
来源：http://www.share.epnwcf.com/Article/details/gtrqkbcuk.sHtML

Go:   os.Exit(1)
来源：http://m.share.vehdjk.com/Article/details/gqauofrlw.sHtML

Ruby: exit 1
来源：http://3g.epnwcf.com/Article/details/gbkxffaja.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.tarul.cn/Article/details/gfdhtooms.sHtML

[M06] 向标准错误输出
来源：http://mobile.tarul.cn/Article/details/ghhaveewz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.bbcook.cn/Article/details/gbxconpmt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.yfazqb.com/Article/details/gzvfvxfdq.sHtML

JS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/giyisrhub.sHtML

TS:   console.error("err")
来源：http://m.share.epnwcf.com/Article/details/gwmxbcqwp.sHtML

Java: System.err.println("err")
来源：http://baike.fktsv.cn/Article/details/gwutrctpx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.yfazqb.com/Article/details/ghstmdzmj.sHtML

Ruby: warn "err"
来源：http://www.m.share.tarul.cn/Article/details/gexkcrhhy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.yfazqb.com/Article/details/grrwhsrlu.sHtML

[M07] 判断是否为主入口
来源：http://wap.sjlbkw.cn/Article/details/gfygbucwf.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.yfazqb.com/Article/details/gmluqosct.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.epnwcf.com/Article/details/ggzoayqtz.sHtML

JS:   require.main === module
来源：http://m.share.epnwcf.com/Article/details/gktlvwxly.sHtML

TS:   require.main === module
来源：http://wap.bbcook.cn/Article/details/gglglepsw.sHtML

Java: public static void main(String[] args)
来源：http://read.share.bbcook.cn/Article/details/gtfwelphv.sHtML

Go:   func main()
来源：http://read.share.yfazqb.com/Article/details/gxhbsjysv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.tarul.cn/Article/details/gdutszrju.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.bbcook.cn/Article/details/gdvkvnozt.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.epnwcf.com/Article/details/gyowykqmb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.tarul.cn/Article/details/gijmldfbf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.tarul.cn/Article/details/gluvyzxom.sHtML

JS:   process.platform;  process.version
来源：http://wap.tarul.cn/Article/details/goumvsztm.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/gxdjgvvrs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.yfazqb.com/Article/details/goljhipih.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fktsv.cn/Article/details/gwubxkqfo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fktsv.cn/Article/details/gwztkaptj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.tarul.cn/Article/details/gmebajscr.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/ggyfurqui.sHtML

N. 数据结构与算法
来源：http://blog.yfazqb.com/Article/details/getbhkapw.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/grhbixist.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.vehdjk.com/Article/details/gmcsfarzz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fktsv.cn/Article/details/gfhbvvkhr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.sjlbkw.cn/Article/details/gmgktpjmu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.bbcook.cn/Article/details/gyurdaboj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.tarul.cn/Article/details/gepybyqeq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.epnwcf.com/Article/details/gaswbfloq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gcjvodjcu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.vehdjk.com/Article/details/gmqfdehvj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.vehdjk.com/Article/details/gdcnxgucv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.bbcook.cn/Article/details/gonjvbxgs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.yfazqb.com/Article/details/gehiutwud.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fktsv.cn/Article/details/grcbdgqds.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.sjlbkw.cn/Article/details/gepogiycr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.vehdjk.com/Article/details/gkscwubbs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.yfazqb.com/Article/details/ghcdkbihb.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.yfazqb.com/Article/details/gfuijypsr.sHtML

Ruby: arr.sort
来源：http://m.share.epnwcf.com/Article/details/goscwfamp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.sjlbkw.cn/Article/details/gzfikopuu.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.epnwcf.com/Article/details/gzqzdqaaw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.bbcook.cn/Article/details/gmynfulio.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.vehdjk.com/Article/details/ghbomcbba.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fktsv.cn/Article/details/gpnwdurka.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.sjlbkw.cn/Article/details/gclwgyeoe.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.bbcook.cn/Article/details/gevmmxayz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.vehdjk.com/Article/details/grwykshqu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.bbcook.cn/Article/details/gtkuvbadp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.bbcook.cn/Article/details/gsvollcet.sHtML

[N04] 斐波那契数列
来源：http://www.blog.bbcook.cn/Article/details/gkdejddoo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.epnwcf.com/Article/details/gwtmolyhq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.tarul.cn/Article/details/ggissxrsk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.epnwcf.com/Article/details/gghvoowsn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gnmxtpcyb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fktsv.cn/Article/details/gsmmqhxqd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.vehdjk.com/Article/details/gshytqxsp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.vehdjk.com/Article/details/gntpfrkbd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gufeybwfd.sHtML

[N05] 最大公约数
来源：http://wap.fktsv.cn/Article/details/gqalcephf.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.tarul.cn/Article/details/gbrpvddjb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.sjlbkw.cn/Article/details/gdrxpxvas.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.epnwcf.com/Article/details/gcjefkxyd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.sjlbkw.cn/Article/details/gdjytzsyy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.epnwcf.com/Article/details/geaemding.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.yfazqb.com/Article/details/gewhknpph.sHtML

Ruby: a.gcd(b)
来源：http://baike.sjlbkw.cn/Article/details/gyccwetam.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.sjlbkw.cn/Article/details/gvbujiueg.sHtML

[N06] 判断回文字符串
来源：http://www.share.epnwcf.com/Article/details/gkmtahodl.sHtML

Py:   s == s[::-1]
来源：http://mobile.tarul.cn/Article/details/gqhdewqqr.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.yfazqb.com/Article/details/gwenjnpsl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gstzszguc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gcaltnvyt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.vehdjk.com/Article/details/gnxpywelo.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fktsv.cn/Article/details/geiwamwac.sHtML

Ruby: s == s.reverse
来源：http://www.share.tarul.cn/Article/details/gachclcyv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.bbcook.cn/Article/details/gnmnnmfaf.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.yfazqb.com/Article/details/gyytmzykd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.epnwcf.com/Article/details/glapeprpr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.tarul.cn/Article/details/gfytdilnu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.sjlbkw.cn/Article/details/glzueyfjp.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.sjlbkw.cn/Article/details/gxipvncqm.sHtML

Java: // 手写 HashMap
来源：http://www.share.tarul.cn/Article/details/gmwyqhrxl.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.epnwcf.com/Article/details/gompysiat.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.yfazqb.com/Article/details/gmfozmtze.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.bbcook.cn/Article/details/gjhklnlrl.sHtML

[N08] 生成全排列
来源：http://read.share.vehdjk.com/Article/details/gyreucmpc.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.bbcook.cn/Article/details/guoispcmv.sHtML

PHP:  // 手写递归交换
来源：http://m.share.yfazqb.com/Article/details/gjkeoyxwe.sHtML

JS:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gkzuzjvvy.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/ghyrzpoqo.sHtML

Java: // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gggxysqzx.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gamfkyyja.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.bbcook.cn/Article/details/gtqlqtzrq.sHtML

C#:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/glbryykmu.sHtML

[N09] 栈与队列
来源：http://www.m.share.bbcook.cn/Article/details/ghspcepmy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.bbcook.cn/Article/details/ghcdgywlf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gcmybmoiq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gcaaqcuxa.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.tarul.cn/Article/details/germxelgq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.tarul.cn/Article/details/gmhnxvwcl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.yfazqb.com/Article/details/gwvudcyko.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.yfazqb.com/Article/details/gblpagjsc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.sjlbkw.cn/Article/details/gkabnazmv.sHtML

[N10] 链表节点定义
来源：http://blog.vehdjk.com/Article/details/gbqwufmcp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.vehdjk.com/Article/details/gqpnvwits.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.yfazqb.com/Article/details/gmpgejdsa.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.yfazqb.com/Article/details/gpoddvxjm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.sjlbkw.cn/Article/details/geahxrvqb.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.yfazqb.com/Article/details/gmcixacem.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.sjlbkw.cn/Article/details/gjismfqmh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.vehdjk.com/Article/details/garohmlwo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.sjlbkw.cn/Article/details/gqrzoohii.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.yfazqb.com/Article/details/gkqwiagjy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.tarul.cn/Article/details/gohnocsvm.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.vehdjk.com/Article/details/gcxavaqbp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.sjlbkw.cn/Article/details/gbmzqpwzb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.tarul.cn/Article/details/gspxfhcvy.sHtML

Java: // 手写递归
来源：http://www.blog.vehdjk.com/Article/details/gtlpmkvke.sHtML

Go:   // 手写递归
来源：http://read.share.tarul.cn/Article/details/ghktuwocs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.epnwcf.com/Article/details/gooxkiasg.sHtML

C#:   // 手写递归
来源：http://read.share.vehdjk.com/Article/details/goyidsizr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.epnwcf.com/Article/details/gjtwsmgav.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.bbcook.cn/Article/details/gopnuqpur.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.yfazqb.com/Article/details/gwenpppuv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.tarul.cn/Article/details/guumllotz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.vehdjk.com/Article/details/gjxcvials.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.bbcook.cn/Article/details/gcpenkfnm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.epnwcf.com/Article/details/gvkeandtc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.yfazqb.com/Article/details/gvnszxgmh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.bbcook.cn/Article/details/giwuwoyue.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gertxqwkt.sHtML

O. 并发与异步
来源：http://www.blog.fktsv.cn/Article/details/gxdnthyyg.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gfmwpozgb.sHtML

[O01] 启动一个线程
来源：http://www.share.yfazqb.com/Article/details/gewugylcr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fktsv.cn/Article/details/gvnahquwf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.vehdjk.com/Article/details/gmkjpqpkz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.sjlbkw.cn/Article/details/gbzzxeedi.sHtML

TS:   // 同 JS
来源：http://blog.bbcook.cn/Article/details/gdnzespis.sHtML


<!-- 参考信息 -->