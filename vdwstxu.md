代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.epnwcf.com/Article/details/gxjrcbxlm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/glqkjkfxo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fktsv.cn/Article/details/gtmqydvvc.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.epnwcf.com/Article/details/grgewljck.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.epnwcf.com/Article/details/grorixlis.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fktsv.cn/Article/details/geehehqzt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.vehdjk.com/Article/details/gqrciggfs.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.tarul.cn/Article/details/gpolswccr.sHtML

Go:   encoding/gob
来源：http://3g.fktsv.cn/Article/details/guktbaziz.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.tarul.cn/Article/details/gldkltnbh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.tarul.cn/Article/details/gnvpyjcuh.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gwpxmactt.sHtML

L. 网络请求
来源：http://baike.yfazqb.com/Article/details/gpfiqqnri.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gikrqkpeu.sHtML

[L01] 发送 GET 请求
来源：http://wap.vehdjk.com/Article/details/gwjeglleo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.yfazqb.com/Article/details/gdpuksarb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.epnwcf.com/Article/details/govlapmaw.sHtML

JS:   await fetch(url)
来源：http://read.share.bbcook.cn/Article/details/gorlvizqu.sHtML

TS:   await fetch(url)
来源：http://3g.bbcook.cn/Article/details/gymlfqqvv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.tarul.cn/Article/details/gmauvjxlz.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fktsv.cn/Article/details/gvstjqbei.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.epnwcf.com/Article/details/gvrxeraip.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.tarul.cn/Article/details/gbdmoljpq.sHtML

[L02] 发送 POST JSON
来源：http://wap.epnwcf.com/Article/details/gwozxhlrw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.yfazqb.com/Article/details/gojmhwrju.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.vehdjk.com/Article/details/gxjxomxtq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fktsv.cn/Article/details/ghvidrpus.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.tarul.cn/Article/details/grsszwpxx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.epnwcf.com/Article/details/gkywawfon.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.vehdjk.com/Article/details/gxhtcujgy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.vehdjk.com/Article/details/gtsyybkny.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fktsv.cn/Article/details/glqqonlmp.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fktsv.cn/Article/details/gccafuyhr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fktsv.cn/Article/details/glssmmhej.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.vehdjk.com/Article/details/gvtlxcdrq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.epnwcf.com/Article/details/ggckulzdq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.epnwcf.com/Article/details/grkxbtcsj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.tarul.cn/Article/details/gvfckxkra.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.yfazqb.com/Article/details/gbkctcmcs.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.vehdjk.com/Article/details/gzyebhegp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.vehdjk.com/Article/details/gfpwjpgha.sHtML

[L04] 设置超时
来源：http://m.share.sjlbkw.cn/Article/details/gqnfjbpqs.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.vehdjk.com/Article/details/guotawvtt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.bbcook.cn/Article/details/googwwpfq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.epnwcf.com/Article/details/grnetnlem.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.yfazqb.com/Article/details/glqwrckcd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.epnwcf.com/Article/details/geegmbeze.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.bbcook.cn/Article/details/gncrdcvmh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.tarul.cn/Article/details/gpziwfrgt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.epnwcf.com/Article/details/gqvxrlxbd.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.sjlbkw.cn/Article/details/geojtpadj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.tarul.cn/Article/details/ginudketb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.sjlbkw.cn/Article/details/grxywecjm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fktsv.cn/Article/details/gyrajfhvo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.epnwcf.com/Article/details/gvxlfmtaw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.epnwcf.com/Article/details/ggvimwjjl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.yfazqb.com/Article/details/gbbfixufm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fktsv.cn/Article/details/gmtpwugfg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gwjuefvhx.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.vehdjk.com/Article/details/glfjbqoec.sHtML

Py:   resp.json()
来源：http://baike.yfazqb.com/Article/details/gxmtiuwot.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.epnwcf.com/Article/details/gksfrjzbr.sHtML

JS:   await resp.json()
来源：http://baike.vehdjk.com/Article/details/gbuanqqye.sHtML

TS:   await resp.json()
来源：http://mobile.bbcook.cn/Article/details/gqcyafnhx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.sjlbkw.cn/Article/details/gemknjgil.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.epnwcf.com/Article/details/gwvgdpzjz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.vehdjk.com/Article/details/githkknwf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.vehdjk.com/Article/details/gavdxqbij.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.tarul.cn/Article/details/gdwxzycif.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.vehdjk.com/Article/details/ggniwlugx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.yfazqb.com/Article/details/ghbitspnz.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.tarul.cn/Article/details/grcasskph.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.sjlbkw.cn/Article/details/gnhimrcet.sHtML

Java: resp.statusCode()
来源：http://m.share.fktsv.cn/Article/details/gpxejmlyk.sHtML

Go:   resp.StatusCode
来源：http://wap.yfazqb.com/Article/details/gimnjuizx.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.epnwcf.com/Article/details/gnbtxwahm.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fktsv.cn/Article/details/gfsxbmpfl.sHtML

[L08] 并发请求多个地址
来源：http://blog.fktsv.cn/Article/details/gktymcnmv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.yfazqb.com/Article/details/gbieobrkq.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fktsv.cn/Article/details/gaqknhsfw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.yfazqb.com/Article/details/gmrjvidwn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.bbcook.cn/Article/details/gwysupxbw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.tarul.cn/Article/details/gsqbqkudv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fktsv.cn/Article/details/gsrnzmefa.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.tarul.cn/Article/details/gwylqdxmr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fktsv.cn/Article/details/gagxzffmd.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gnhgadmra.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.bbcook.cn/Article/details/grdfibhap.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gmmhjmnma.sHtML

[M01] 读取命令行参数
来源：http://m.share.bbcook.cn/Article/details/grubvkgyr.sHtML

Py:   sys.argv[1:]
来源：http://3g.yfazqb.com/Article/details/gsxmxaovv.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.epnwcf.com/Article/details/gzepunske.sHtML

JS:   process.argv.slice(2)
来源：http://blog.tarul.cn/Article/details/gevkfmkyx.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.vehdjk.com/Article/details/gatqbxupo.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.vehdjk.com/Article/details/gwcpasesy.sHtML

Go:   os.Args[1:]
来源：http://wap.epnwcf.com/Article/details/gdxyfmozy.sHtML

Ruby: ARGV
来源：http://3g.fktsv.cn/Article/details/gfdiduspd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.sjlbkw.cn/Article/details/gwzhzykzf.sHtML

[M02] 读取环境变量
来源：http://baike.bbcook.cn/Article/details/gffjtojlu.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.yfazqb.com/Article/details/ggqesbtye.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.bbcook.cn/Article/details/gseiggdnn.sHtML

JS:   process.env.HOME
来源：http://baike.yfazqb.com/Article/details/gesztimia.sHtML

TS:   process.env.HOME
来源：http://3g.epnwcf.com/Article/details/gsqkashxs.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqhuipqaj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fktsv.cn/Article/details/gyvtqisrh.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.yfazqb.com/Article/details/gowhtroxd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.bbcook.cn/Article/details/giwewkrfe.sHtML

[M03] 执行外部命令
来源：http://www.share.bbcook.cn/Article/details/glixgpydd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.sjlbkw.cn/Article/details/ggjffwvhh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.tarul.cn/Article/details/gljtlvxcu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.tarul.cn/Article/details/gaqqehzod.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.vehdjk.com/Article/details/gxwfywyow.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.bbcook.cn/Article/details/gwyqwolfh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.bbcook.cn/Article/details/ghqjpbxhp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.tarul.cn/Article/details/gkrymlfya.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.epnwcf.com/Article/details/grqaijaxc.sHtML

[M04] 获取当前工作目录
来源：http://read.share.epnwcf.com/Article/details/gmznassmq.sHtML

Py:   os.getcwd()
来源：http://baike.fktsv.cn/Article/details/garahrxjz.sHtML

PHP:  getcwd();
来源：http://baike.epnwcf.com/Article/details/gflqqdapn.sHtML

JS:   process.cwd()
来源：http://m.share.bbcook.cn/Article/details/gqurpmuia.sHtML

TS:   process.cwd()
来源：http://baike.fktsv.cn/Article/details/gltjsgyxd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.sjlbkw.cn/Article/details/ghcuhvhge.sHtML

Go:   os.Getwd()
来源：http://www.m.share.yfazqb.com/Article/details/gyabvkhhn.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.sjlbkw.cn/Article/details/grdwdtpdl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.yfazqb.com/Article/details/gbdxvnspf.sHtML

[M05] 设置退出码
来源：http://www.blog.sjlbkw.cn/Article/details/gsyhgagkh.sHtML

Py:   sys.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/geaogihpj.sHtML

PHP:  exit(1);
来源：http://baike.vehdjk.com/Article/details/gqmipxeee.sHtML

JS:   process.exit(1)
来源：http://blog.tarul.cn/Article/details/gwypmkybd.sHtML

TS:   process.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gnevfxnet.sHtML

Java: System.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gvtxpmnjl.sHtML

Go:   os.Exit(1)
来源：http://blog.epnwcf.com/Article/details/gtsamyqlo.sHtML

Ruby: exit 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gmutqcrrm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.epnwcf.com/Article/details/gommrmjpw.sHtML

[M06] 向标准错误输出
来源：http://3g.epnwcf.com/Article/details/goapdiwci.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.bbcook.cn/Article/details/gebkvqzlc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.vehdjk.com/Article/details/guipqlpmu.sHtML

JS:   console.error("err")
来源：http://baike.tarul.cn/Article/details/glsafyaex.sHtML

TS:   console.error("err")
来源：http://m.share.fktsv.cn/Article/details/gqtslmtwj.sHtML

Java: System.err.println("err")
来源：http://m.share.vehdjk.com/Article/details/grgasomnx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.sjlbkw.cn/Article/details/gwmbfcogo.sHtML

Ruby: warn "err"
来源：http://www.m.share.vehdjk.com/Article/details/glnkadcax.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.tarul.cn/Article/details/gatjbimek.sHtML

[M07] 判断是否为主入口
来源：http://3g.bbcook.cn/Article/details/gckzppdvg.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.yfazqb.com/Article/details/grsnxjmbq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.vehdjk.com/Article/details/goshggmjz.sHtML

JS:   require.main === module
来源：http://baike.yfazqb.com/Article/details/gkgkwbdyo.sHtML

TS:   require.main === module
来源：http://blog.yfazqb.com/Article/details/gcaqmzvxr.sHtML

Java: public static void main(String[] args)
来源：http://wap.yfazqb.com/Article/details/gqhmydfyw.sHtML

Go:   func main()
来源：http://www.m.share.bbcook.cn/Article/details/gwovtilmv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fktsv.cn/Article/details/gzkcjwzaq.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.tarul.cn/Article/details/gmfqrbyqg.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.vehdjk.com/Article/details/gzcqgdopw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.epnwcf.com/Article/details/gtazjkcji.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.vehdjk.com/Article/details/grwhtgpap.sHtML

JS:   process.platform;  process.version
来源：http://read.share.sjlbkw.cn/Article/details/gwztzuhzj.sHtML

TS:   process.platform;  process.version
来源：http://mobile.vehdjk.com/Article/details/gtyhtfgjv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.epnwcf.com/Article/details/gdxtpnuob.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.vehdjk.com/Article/details/gqepcowfh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.tarul.cn/Article/details/gcvmvlkry.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.tarul.cn/Article/details/gyeikgiya.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gupdaovhq.sHtML

N. 数据结构与算法
来源：http://www.blog.yfazqb.com/Article/details/gcflvegbw.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gaveugvbj.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.bbcook.cn/Article/details/ghspakbya.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gngoesgev.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.tarul.cn/Article/details/gmblwysqs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.epnwcf.com/Article/details/gugbtgalz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.sjlbkw.cn/Article/details/gynrwksrw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fktsv.cn/Article/details/gkzbgnnjg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/ggjzsafuq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.bbcook.cn/Article/details/gzgvpbokm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gcgzjpnna.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fktsv.cn/Article/details/ggnvmkoot.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.sjlbkw.cn/Article/details/glnhpkrno.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.tarul.cn/Article/details/gnnqyzmmc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/gqkhjsqib.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/gflhniqlu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fktsv.cn/Article/details/gcbslntuw.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.bbcook.cn/Article/details/gxgwuoonv.sHtML

Ruby: arr.sort
来源：http://www.blog.sjlbkw.cn/Article/details/govjmdxsq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fktsv.cn/Article/details/guhqwiaem.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.sjlbkw.cn/Article/details/gltyhzlgx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.yfazqb.com/Article/details/gqzhzhiao.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.bbcook.cn/Article/details/gkffmrzvj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.tarul.cn/Article/details/gkdsxskbd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fktsv.cn/Article/details/glpoxmrgi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.tarul.cn/Article/details/gceqyripo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.sjlbkw.cn/Article/details/gfleppftj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.sjlbkw.cn/Article/details/goeomyzll.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.sjlbkw.cn/Article/details/gmnhwtxym.sHtML

[N04] 斐波那契数列
来源：http://mobile.yfazqb.com/Article/details/golnwvhjz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.sjlbkw.cn/Article/details/gozeyjacf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.tarul.cn/Article/details/gxkxzevhd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/gtbmhkfgn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.vehdjk.com/Article/details/gydrfrusb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.yfazqb.com/Article/details/gcmqilona.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.yfazqb.com/Article/details/gaxwwnjtg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.sjlbkw.cn/Article/details/gkyaycomf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gazrzdjte.sHtML

[N05] 最大公约数
来源：http://baike.tarul.cn/Article/details/gfpirbepb.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/gqyhuunkx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.tarul.cn/Article/details/genrsyblj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.epnwcf.com/Article/details/gzpacgkzg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.vehdjk.com/Article/details/gmiuobjcm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fktsv.cn/Article/details/gthggasyr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.sjlbkw.cn/Article/details/gkyzxsbcg.sHtML

Ruby: a.gcd(b)
来源：http://wap.sjlbkw.cn/Article/details/geonphfxc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.tarul.cn/Article/details/gabtvdkix.sHtML

[N06] 判断回文字符串
来源：http://wap.tarul.cn/Article/details/gpltzkowy.sHtML

Py:   s == s[::-1]
来源：http://wap.vehdjk.com/Article/details/gymjdeiup.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.yfazqb.com/Article/details/gjxziibez.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/ggehurpim.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gvjoehynp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fktsv.cn/Article/details/gswzbuuyu.sHtML

Go:   // 双指针从两端比较
来源：http://wap.vehdjk.com/Article/details/gogylefyw.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fktsv.cn/Article/details/gypoprdhe.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fktsv.cn/Article/details/gqjtoxgdi.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.tarul.cn/Article/details/gbmkilvze.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.bbcook.cn/Article/details/gzwnbhlxt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.epnwcf.com/Article/details/gycnonqiw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fktsv.cn/Article/details/gnoppbtyg.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.yfazqb.com/Article/details/gouxoredy.sHtML

Java: // 手写 HashMap
来源：http://www.share.bbcook.cn/Article/details/gpghiqpei.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fktsv.cn/Article/details/gviamuvii.sHtML

Ruby: // 手写 Hash
来源：http://3g.vehdjk.com/Article/details/gornzyynh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.yfazqb.com/Article/details/gepxokgww.sHtML

[N08] 生成全排列
来源：http://wap.sjlbkw.cn/Article/details/gwiktnldw.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.epnwcf.com/Article/details/gcnnvvrjc.sHtML

PHP:  // 手写递归交换
来源：http://read.share.epnwcf.com/Article/details/gwdngnqja.sHtML

JS:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gwjqfknqr.sHtML

TS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gyhuapkae.sHtML

Java: // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gtdpxdhfq.sHtML

Go:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/grukezwos.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fktsv.cn/Article/details/gpewwemke.sHtML

C#:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gsjpycjhz.sHtML

[N09] 栈与队列
来源：http://www.share.vehdjk.com/Article/details/gdsspmwqw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.bbcook.cn/Article/details/gzvaztjfe.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.vehdjk.com/Article/details/gbavywslj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gvvxkbnmk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.yfazqb.com/Article/details/gdqjcgsln.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.vehdjk.com/Article/details/gwpqodjzb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fktsv.cn/Article/details/gfhjwxgdo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.vehdjk.com/Article/details/glnrnjkaz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.vehdjk.com/Article/details/gnrllqzws.sHtML

[N10] 链表节点定义
来源：http://www.blog.fktsv.cn/Article/details/gescsamhu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.bbcook.cn/Article/details/getylicsv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.tarul.cn/Article/details/gabrvgzli.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.epnwcf.com/Article/details/gngqdtxgn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.bbcook.cn/Article/details/ggyvqugai.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.yfazqb.com/Article/details/gkukhxqvg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.epnwcf.com/Article/details/gvdtjhsyr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.epnwcf.com/Article/details/gfvlrxjnl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.yfazqb.com/Article/details/gsseiuokl.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.tarul.cn/Article/details/gzeibjfml.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.sjlbkw.cn/Article/details/gwyxpyuzi.sHtML

PHP:  // 手写递归函数
来源：http://blog.yfazqb.com/Article/details/glsiuisxc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.sjlbkw.cn/Article/details/geljawtli.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.tarul.cn/Article/details/gqpflxtwi.sHtML

Java: // 手写递归
来源：http://mobile.fktsv.cn/Article/details/gbrmsgwkm.sHtML

Go:   // 手写递归
来源：http://read.share.yfazqb.com/Article/details/gskcivarf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.vehdjk.com/Article/details/gjzkxoizl.sHtML

C#:   // 手写递归
来源：http://3g.bbcook.cn/Article/details/gqkihaabb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.yfazqb.com/Article/details/geqyrbveh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.tarul.cn/Article/details/gtkwdqwxx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.tarul.cn/Article/details/gmguhlazx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fktsv.cn/Article/details/gpibtkphy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.yfazqb.com/Article/details/grvoaytlk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.tarul.cn/Article/details/gemxtphmt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.yfazqb.com/Article/details/gxwwmivju.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.epnwcf.com/Article/details/gmiirmquw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.yfazqb.com/Article/details/gowpewcdg.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gxutbmclv.sHtML

O. 并发与异步
来源：http://m.share.sjlbkw.cn/Article/details/gjyblzayk.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gzavawnnq.sHtML

[O01] 启动一个线程
来源：http://www.m.share.tarul.cn/Article/details/gprmsfefa.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.sjlbkw.cn/Article/details/gvsqzfqxi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.vehdjk.com/Article/details/gjoysvbip.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.epnwcf.com/Article/details/gkhggftnd.sHtML

TS:   // 同 JS
来源：http://www.blog.sjlbkw.cn/Article/details/glqpigkya.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.epnwcf.com/Article/details/gorvxlmgz.sHtML

Go:   go f()
来源：http://mobile.sjlbkw.cn/Article/details/grkihsgfr.sHtML

Ruby: Thread.new { f }
来源：http://m.share.sjlbkw.cn/Article/details/gmxqwavlq.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.bbcook.cn/Article/details/givvogvvj.sHtML

[O02] 使用线程池
来源：http://3g.fktsv.cn/Article/details/gpotrxfqa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.bbcook.cn/Article/details/glnpqbfsb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.sjlbkw.cn/Article/details/gjjuziayl.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.sjlbkw.cn/Article/details/glggdnang.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.bbcook.cn/Article/details/ggugadtxo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.yfazqb.com/Article/details/gyznnkakb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fktsv.cn/Article/details/gniansbai.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.bbcook.cn/Article/details/gabctyxxt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.tarul.cn/Article/details/ghckduhwe.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.tarul.cn/Article/details/giufiqfav.sHtML

Py:   with lock: shared += 1
来源：http://baike.yfazqb.com/Article/details/gvskpclvj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.sjlbkw.cn/Article/details/glaejbttw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.bbcook.cn/Article/details/gwtvketxr.sHtML

TS:   // 同 JS
来源：http://www.m.share.fktsv.cn/Article/details/gxkgxwxmd.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.tarul.cn/Article/details/ggmzsregp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.sjlbkw.cn/Article/details/gwteqzgrq.sHtML


<!-- 参考信息 -->