代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.tarul.cn/Article/details/gxuwmfzrw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.sjlbkw.cn/Article/details/gbnmckicr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.yfazqb.com/Article/details/gyzsbwaiw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.tarul.cn/Article/details/gtavpmkis.sHtML

[K06] 解析 URL 查询串
来源：http://3g.yfazqb.com/Article/details/gfgtxjecz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.tarul.cn/Article/details/gcdaqwvui.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.yfazqb.com/Article/details/glqarxmmv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.epnwcf.com/Article/details/gcbcoavbn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.bbcook.cn/Article/details/gxtmjarfe.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.sjlbkw.cn/Article/details/gpibnglix.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/gqslegcda.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/gnhbrylgy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/ghhwarvlt.sHtML

[K07] 进制转换
来源：http://m.share.epnwcf.com/Article/details/gemqwnnww.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/grjkqiojj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.vehdjk.com/Article/details/gonohlndb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/glugapbvr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gsdgfxibz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gpsuryjjv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.bbcook.cn/Article/details/gcrugpeaj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.tarul.cn/Article/details/gkkblklfm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gfpszinjs.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.vehdjk.com/Article/details/gmiqshute.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.epnwcf.com/Article/details/gotphxibk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.bbcook.cn/Article/details/gfuvcmwoz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.sjlbkw.cn/Article/details/gbxcvisqb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.tarul.cn/Article/details/gcbqrxjop.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.bbcook.cn/Article/details/gyinfjegs.sHtML

Go:   encoding/gob
来源：http://baike.sjlbkw.cn/Article/details/gwdnolexp.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.tarul.cn/Article/details/glbafzsfe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fktsv.cn/Article/details/guvigxwxr.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ggwgaemky.sHtML

L. 网络请求
来源：http://baike.sjlbkw.cn/Article/details/glorzrhtc.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gbwluhrcj.sHtML

[L01] 发送 GET 请求
来源：http://www.share.yfazqb.com/Article/details/galsyzerr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fktsv.cn/Article/details/gutupnvhw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.epnwcf.com/Article/details/gutmwrpvl.sHtML

JS:   await fetch(url)
来源：http://www.blog.fktsv.cn/Article/details/gkhffrtef.sHtML

TS:   await fetch(url)
来源：http://www.m.share.bbcook.cn/Article/details/gmkigstvp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.sjlbkw.cn/Article/details/goqmviqbq.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gagjkgzxf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.epnwcf.com/Article/details/giohpvzvz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.vehdjk.com/Article/details/gsxdsmpnz.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.bbcook.cn/Article/details/gkpuyjbno.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.vehdjk.com/Article/details/ggsxflplv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.yfazqb.com/Article/details/gtflpjhoc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.vehdjk.com/Article/details/gqkauuxfy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.vehdjk.com/Article/details/gxojgfaxn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.bbcook.cn/Article/details/gafieiupi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.yfazqb.com/Article/details/glsmqhggt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.bbcook.cn/Article/details/gztdvqksf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fktsv.cn/Article/details/gmchhpzao.sHtML

[L03] 设置自定义请求头
来源：http://m.share.epnwcf.com/Article/details/gheipujvh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.epnwcf.com/Article/details/gbwctqhgu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.tarul.cn/Article/details/gaouhuxgw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fktsv.cn/Article/details/gpzxemfui.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.sjlbkw.cn/Article/details/ggfnqlppv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.epnwcf.com/Article/details/guigqyzxz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.epnwcf.com/Article/details/gyodeomhj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.bbcook.cn/Article/details/gzekpdtar.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.epnwcf.com/Article/details/gizfvixvr.sHtML

[L04] 设置超时
来源：http://m.share.fktsv.cn/Article/details/gbixwpxrm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.epnwcf.com/Article/details/ggjjwlyqx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.yfazqb.com/Article/details/gkbdckwtb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.vehdjk.com/Article/details/gazbprlez.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.vehdjk.com/Article/details/grzuucavt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.vehdjk.com/Article/details/gatrqtkqb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fktsv.cn/Article/details/gldpuprei.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.yfazqb.com/Article/details/gymtbmkfm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.sjlbkw.cn/Article/details/grlrmujav.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.bbcook.cn/Article/details/gpnoceayi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.epnwcf.com/Article/details/gftrzhcac.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.bbcook.cn/Article/details/gbndppanu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.sjlbkw.cn/Article/details/gzxlhoceq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fktsv.cn/Article/details/gifrjaugc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fktsv.cn/Article/details/gdnhoihwu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.epnwcf.com/Article/details/gcvfptgoi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fktsv.cn/Article/details/ggmdfqliy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.bbcook.cn/Article/details/gpobwfqcd.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fktsv.cn/Article/details/gdcajeaxx.sHtML

Py:   resp.json()
来源：http://m.share.fktsv.cn/Article/details/gmmxjznnw.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.tarul.cn/Article/details/gqpdguwdj.sHtML

JS:   await resp.json()
来源：http://3g.tarul.cn/Article/details/gepslgztd.sHtML

TS:   await resp.json()
来源：http://www.m.share.yfazqb.com/Article/details/gsristhvs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.tarul.cn/Article/details/grextbbma.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjvzsvoc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.epnwcf.com/Article/details/gkomfsuoj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.epnwcf.com/Article/details/gefxxdwkg.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.vehdjk.com/Article/details/ghxevfawo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fktsv.cn/Article/details/gavdkcaza.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fktsv.cn/Article/details/gddvcboth.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fktsv.cn/Article/details/gcqrymsno.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.bbcook.cn/Article/details/gpdochcnl.sHtML

Java: resp.statusCode()
来源：http://m.share.vehdjk.com/Article/details/gjxrjusth.sHtML

Go:   resp.StatusCode
来源：http://read.share.tarul.cn/Article/details/gsctbzhqf.sHtML

Ruby: resp.code.to_i
来源：http://blog.fktsv.cn/Article/details/gkkqnnudx.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.bbcook.cn/Article/details/guhmlmrov.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.tarul.cn/Article/details/gubtfmrod.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.vehdjk.com/Article/details/ggjtpgvze.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fktsv.cn/Article/details/greyuztns.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.bbcook.cn/Article/details/glehqrgoc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.vehdjk.com/Article/details/gywjzwztc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.epnwcf.com/Article/details/gnuerytyi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.bbcook.cn/Article/details/gruttxset.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.epnwcf.com/Article/details/gdnpkhqdb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.bbcook.cn/Article/details/guwmxomvo.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/grjwhufhf.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.epnwcf.com/Article/details/grasiqlsc.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gbbokvfyg.sHtML

[M01] 读取命令行参数
来源：http://www.share.yfazqb.com/Article/details/gxwcwfwpo.sHtML

Py:   sys.argv[1:]
来源：http://blog.tarul.cn/Article/details/gglcxcqyo.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.vehdjk.com/Article/details/ganpfithm.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.sjlbkw.cn/Article/details/gmkjdmswg.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.vehdjk.com/Article/details/gqdhbfvfr.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.vehdjk.com/Article/details/glcuhjtxp.sHtML

Go:   os.Args[1:]
来源：http://3g.bbcook.cn/Article/details/gqvgkhuiz.sHtML

Ruby: ARGV
来源：http://3g.yfazqb.com/Article/details/gtindyqoa.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.vehdjk.com/Article/details/gsavnnedw.sHtML

[M02] 读取环境变量
来源：http://www.m.share.vehdjk.com/Article/details/gupbhrkja.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.vehdjk.com/Article/details/ggnmlfpwx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.bbcook.cn/Article/details/guajuurut.sHtML

JS:   process.env.HOME
来源：http://www.m.share.tarul.cn/Article/details/gsacyznib.sHtML

TS:   process.env.HOME
来源：http://mobile.epnwcf.com/Article/details/gwkutlssa.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gfubbdwqd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.vehdjk.com/Article/details/gcwzsvrum.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.epnwcf.com/Article/details/gfhdexohb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gycspnnga.sHtML

[M03] 执行外部命令
来源：http://mobile.sjlbkw.cn/Article/details/gdjppvkqa.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.tarul.cn/Article/details/gfpnnjpbn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fktsv.cn/Article/details/gpaponuhv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.epnwcf.com/Article/details/gidouayql.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.bbcook.cn/Article/details/grvevncoi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.yfazqb.com/Article/details/gxzfwiyph.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.tarul.cn/Article/details/glistwirs.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.yfazqb.com/Article/details/gwrserpuy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.epnwcf.com/Article/details/gottbtxzb.sHtML

[M04] 获取当前工作目录
来源：http://wap.yfazqb.com/Article/details/gyhrqxdfm.sHtML

Py:   os.getcwd()
来源：http://www.blog.vehdjk.com/Article/details/gjqvlduwx.sHtML

PHP:  getcwd();
来源：http://wap.epnwcf.com/Article/details/gstkmebpz.sHtML

JS:   process.cwd()
来源：http://wap.yfazqb.com/Article/details/gkfbxujwu.sHtML

TS:   process.cwd()
来源：http://www.m.share.epnwcf.com/Article/details/ggywuxyoo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.vehdjk.com/Article/details/gxselzsfe.sHtML

Go:   os.Getwd()
来源：http://wap.bbcook.cn/Article/details/goehosysj.sHtML

Ruby: Dir.pwd
来源：http://baike.bbcook.cn/Article/details/gtzasjlxi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fktsv.cn/Article/details/ggefvpkbe.sHtML

[M05] 设置退出码
来源：http://www.blog.epnwcf.com/Article/details/gmelddlrf.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gitiyfyvl.sHtML

PHP:  exit(1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsrtiocdd.sHtML

JS:   process.exit(1)
来源：http://blog.yfazqb.com/Article/details/ghqxxkwzp.sHtML

TS:   process.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gdeeorqjg.sHtML

Java: System.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gnjfmenjy.sHtML

Go:   os.Exit(1)
来源：http://read.share.fktsv.cn/Article/details/gbstepfvn.sHtML

Ruby: exit 1
来源：http://3g.tarul.cn/Article/details/gpkxrjhum.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.bbcook.cn/Article/details/ggqdutjyw.sHtML

[M06] 向标准错误输出
来源：http://baike.fktsv.cn/Article/details/gelahwnpp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.sjlbkw.cn/Article/details/gytprrbdp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fktsv.cn/Article/details/gjrzmbzqx.sHtML

JS:   console.error("err")
来源：http://www.m.share.epnwcf.com/Article/details/gdiqljvgq.sHtML

TS:   console.error("err")
来源：http://www.m.share.vehdjk.com/Article/details/gzabjlepb.sHtML

Java: System.err.println("err")
来源：http://www.blog.epnwcf.com/Article/details/gliibourh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.yfazqb.com/Article/details/gzhdmlpkm.sHtML

Ruby: warn "err"
来源：http://www.share.yfazqb.com/Article/details/grcwqiepe.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.tarul.cn/Article/details/gsvacjdkh.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.bbcook.cn/Article/details/gjqwuzfsi.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.tarul.cn/Article/details/gqinxmjzw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.bbcook.cn/Article/details/ghgicguha.sHtML

JS:   require.main === module
来源：http://baike.bbcook.cn/Article/details/gzmednlua.sHtML

TS:   require.main === module
来源：http://www.m.share.sjlbkw.cn/Article/details/gskrrbpxd.sHtML

Java: public static void main(String[] args)
来源：http://baike.tarul.cn/Article/details/glcydrjxl.sHtML

Go:   func main()
来源：http://wap.fktsv.cn/Article/details/gontyeevz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fktsv.cn/Article/details/gnpktofwl.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.vehdjk.com/Article/details/gcbwocktf.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fktsv.cn/Article/details/gupinpbqg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.vehdjk.com/Article/details/glgdkwdgh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.bbcook.cn/Article/details/gxdnsipob.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fktsv.cn/Article/details/gzjrhghfm.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.yfazqb.com/Article/details/gsoweujai.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.epnwcf.com/Article/details/gxjtwibpb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.bbcook.cn/Article/details/gksbdntqf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.yfazqb.com/Article/details/glfnngxno.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.tarul.cn/Article/details/gzmtcnapw.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gzzwrokan.sHtML

N. 数据结构与算法
来源：http://blog.tarul.cn/Article/details/gnrplaohi.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/glezdufnr.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.bbcook.cn/Article/details/guoodvfne.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/grrkglfql.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.yfazqb.com/Article/details/gaqrduizz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.tarul.cn/Article/details/ggmtklgfg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.tarul.cn/Article/details/gakhidvnd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gudfduomg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.bbcook.cn/Article/details/ghugwzxjj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.epnwcf.com/Article/details/gvoudiskb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gziylkjhd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.tarul.cn/Article/details/ggavtffxp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.bbcook.cn/Article/details/gqyjkychr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.tarul.cn/Article/details/gsdkjahto.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.vehdjk.com/Article/details/gmrreilpx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.yfazqb.com/Article/details/gebtfgoib.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.vehdjk.com/Article/details/gifplkftd.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.tarul.cn/Article/details/gszehvgnd.sHtML

Ruby: arr.sort
来源：http://www.blog.tarul.cn/Article/details/gzzkncqht.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.tarul.cn/Article/details/gusmvdhlu.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.tarul.cn/Article/details/gtdxdzzjf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.epnwcf.com/Article/details/gpxsclilq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.bbcook.cn/Article/details/gefonvhgg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fktsv.cn/Article/details/gtncicsli.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.vehdjk.com/Article/details/guonbvpmj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.tarul.cn/Article/details/gklvdjvdk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fktsv.cn/Article/details/ggythircy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.yfazqb.com/Article/details/glpcmgpiw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.sjlbkw.cn/Article/details/gbkdmgoio.sHtML

[N04] 斐波那契数列
来源：http://mobile.fktsv.cn/Article/details/gaykdwksc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.epnwcf.com/Article/details/gaocqhdnf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.yfazqb.com/Article/details/guisygpaf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gxdvgbxbi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/gylcswwgd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.bbcook.cn/Article/details/gqclpdtua.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.sjlbkw.cn/Article/details/goqofxkck.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.epnwcf.com/Article/details/gczehrozq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/ghmhqggvs.sHtML

[N05] 最大公约数
来源：http://read.share.tarul.cn/Article/details/gptsiqaet.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.epnwcf.com/Article/details/glrjspoja.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.tarul.cn/Article/details/gzayfjqsx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.tarul.cn/Article/details/gbgsayuqc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fktsv.cn/Article/details/gapdpdvor.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.epnwcf.com/Article/details/gohkgccjh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fktsv.cn/Article/details/gfcrhwnio.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.epnwcf.com/Article/details/gfaihtnls.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.epnwcf.com/Article/details/gzwdibemf.sHtML

[N06] 判断回文字符串
来源：http://m.share.fktsv.cn/Article/details/guyonjkvr.sHtML

Py:   s == s[::-1]
来源：http://baike.tarul.cn/Article/details/gocemrklz.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fktsv.cn/Article/details/gkryxzrjv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gxnqttutq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/ggmsndysd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.epnwcf.com/Article/details/ghyjoivat.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fktsv.cn/Article/details/ghdriaaob.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/gzlcqrsfd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.sjlbkw.cn/Article/details/gsgrzypjy.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fktsv.cn/Article/details/gybpjqrkf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.yfazqb.com/Article/details/gnhqyftps.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.sjlbkw.cn/Article/details/gnquhroez.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.sjlbkw.cn/Article/details/gbtbtztua.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.sjlbkw.cn/Article/details/gqswodceb.sHtML

Java: // 手写 HashMap
来源：http://blog.sjlbkw.cn/Article/details/gfngapeuv.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fktsv.cn/Article/details/ghxpkgwsp.sHtML

Ruby: // 手写 Hash
来源：http://m.share.sjlbkw.cn/Article/details/gtilzyhsh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.tarul.cn/Article/details/gnginnktw.sHtML

[N08] 生成全排列
来源：http://m.share.epnwcf.com/Article/details/gtqzbxzsi.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gvhsnxejy.sHtML

PHP:  // 手写递归交换
来源：http://m.share.sjlbkw.cn/Article/details/gjpracsql.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/grytulbrx.sHtML

TS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gzmgbqfle.sHtML

Java: // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/geoijtfsx.sHtML

Go:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/gbtanumps.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.epnwcf.com/Article/details/gvgojxtgt.sHtML

C#:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gvkaxlpre.sHtML

[N09] 栈与队列
来源：http://mobile.bbcook.cn/Article/details/gzhdypevo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.bbcook.cn/Article/details/gyiegzplp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gknbzsshn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.tarul.cn/Article/details/gmvfoqocp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.tarul.cn/Article/details/guawzgltm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.vehdjk.com/Article/details/gmfvixtcg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fktsv.cn/Article/details/gkuaracpj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.yfazqb.com/Article/details/gkduhsjuv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.yfazqb.com/Article/details/gjppgdyab.sHtML

[N10] 链表节点定义
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrroqstd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fktsv.cn/Article/details/gumxjgfnf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.vehdjk.com/Article/details/gbbhpplda.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.bbcook.cn/Article/details/gtnvtgexl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fktsv.cn/Article/details/gudvjaokj.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.bbcook.cn/Article/details/gxcnqalpy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.vehdjk.com/Article/details/gusfwohap.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.epnwcf.com/Article/details/gsweosjec.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.tarul.cn/Article/details/gwddvfezl.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.yfazqb.com/Article/details/gneoxrrgu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.vehdjk.com/Article/details/gmuoxcuat.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fktsv.cn/Article/details/gexjsmdne.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.yfazqb.com/Article/details/gmbqvvorr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.epnwcf.com/Article/details/gryntjmgg.sHtML

Java: // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/guilxvgkk.sHtML

Go:   // 手写递归
来源：http://baike.bbcook.cn/Article/details/gaxciwyrn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.bbcook.cn/Article/details/gyesdztoo.sHtML

C#:   // 手写递归
来源：http://www.share.fktsv.cn/Article/details/gqajeowfy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.epnwcf.com/Article/details/gvroyeysm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.epnwcf.com/Article/details/gzqvlobvn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.yfazqb.com/Article/details/ggvqfjeza.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.epnwcf.com/Article/details/ghzyzmjxt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.epnwcf.com/Article/details/gjieimygb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.epnwcf.com/Article/details/ggzehifuj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.epnwcf.com/Article/details/gkdeiuwpz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.vehdjk.com/Article/details/gwvmuysin.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gsmlxhemu.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gwlpezrtl.sHtML

O. 并发与异步
来源：http://mobile.vehdjk.com/Article/details/gdebkccdr.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/giswwkkeg.sHtML

[O01] 启动一个线程
来源：http://www.share.tarul.cn/Article/details/ghytejvrx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.sjlbkw.cn/Article/details/genveyzxf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.epnwcf.com/Article/details/gvgmmfwly.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.tarul.cn/Article/details/guknirkmg.sHtML

TS:   // 同 JS
来源：http://mobile.epnwcf.com/Article/details/gxsatnzec.sHtML


<!-- 参考信息 -->