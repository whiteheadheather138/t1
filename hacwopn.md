代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gwzmpdvvt.sHtML

[K07] 进制转换
来源：http://m.share.sjlbkw.cn/Article/details/gcgqtxeis.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/garocxwgx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.bbcook.cn/Article/details/gnpjsoigb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gvjcowffp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gmlyzvmqq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/ggsjnxvwm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fktsv.cn/Article/details/gudfizwze.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fktsv.cn/Article/details/gvxfblsod.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gnfbfspvr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.vehdjk.com/Article/details/ghcwubesh.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gvmkshzgy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fktsv.cn/Article/details/grypqizli.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.bbcook.cn/Article/details/gvnbsratg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.tarul.cn/Article/details/gysnqsqzi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.epnwcf.com/Article/details/grbwzavwr.sHtML

Go:   encoding/gob
来源：http://blog.fktsv.cn/Article/details/gzfkmfbdw.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.yfazqb.com/Article/details/gsuzabwqq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.yfazqb.com/Article/details/gzbexnxme.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gqlsmxkjt.sHtML

L. 网络请求
来源：http://mobile.bbcook.cn/Article/details/gsufwmlzx.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gshbubxfh.sHtML

[L01] 发送 GET 请求
来源：http://3g.sjlbkw.cn/Article/details/gwutnrcbh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.tarul.cn/Article/details/ggdokkqst.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.tarul.cn/Article/details/gscdhvhat.sHtML

JS:   await fetch(url)
来源：http://blog.fktsv.cn/Article/details/goovvewlu.sHtML

TS:   await fetch(url)
来源：http://read.share.tarul.cn/Article/details/gzgtpjlog.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.epnwcf.com/Article/details/gsnnfwwym.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.tarul.cn/Article/details/gqezeeqvg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.epnwcf.com/Article/details/gsfenhrdj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fktsv.cn/Article/details/ginayxyis.sHtML

[L02] 发送 POST JSON
来源：http://www.share.vehdjk.com/Article/details/gkoyuchgp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.yfazqb.com/Article/details/gltlkohsx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.yfazqb.com/Article/details/gjcwdbtrv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fktsv.cn/Article/details/ghwlajcnj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.bbcook.cn/Article/details/gtrhkkuwc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.sjlbkw.cn/Article/details/ghoewcxpw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.tarul.cn/Article/details/gyehvaiza.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.yfazqb.com/Article/details/gikktmsxg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fktsv.cn/Article/details/gkzfqyvpo.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fktsv.cn/Article/details/gvhdgvthf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.epnwcf.com/Article/details/gerfnqvon.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.vehdjk.com/Article/details/gbwygdveb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.yfazqb.com/Article/details/gjrrtxhxl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.bbcook.cn/Article/details/giiyfpefs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fktsv.cn/Article/details/gjhpscnhp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.tarul.cn/Article/details/gvmnlusza.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.epnwcf.com/Article/details/gqfyzcudk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.bbcook.cn/Article/details/gpxgtiumo.sHtML

[L04] 设置超时
来源：http://read.share.fktsv.cn/Article/details/gvzyomuxq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.tarul.cn/Article/details/gqqlgvvzf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.yfazqb.com/Article/details/guyhwyuds.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.vehdjk.com/Article/details/goncvusvy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.epnwcf.com/Article/details/gvgenxosr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.sjlbkw.cn/Article/details/glqhcmhgu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.epnwcf.com/Article/details/gmhmfveqn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.sjlbkw.cn/Article/details/gqmxxgbyx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fktsv.cn/Article/details/gvlylcpuf.sHtML

[L05] 上传文件（multipart）
来源：http://baike.tarul.cn/Article/details/gpukxgmjw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.epnwcf.com/Article/details/gbdsjqsaz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.sjlbkw.cn/Article/details/gfqxxrxxb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.tarul.cn/Article/details/gxysllmix.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.bbcook.cn/Article/details/gxylvydqa.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fktsv.cn/Article/details/gkoewdrpp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.vehdjk.com/Article/details/gxkxzicat.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.vehdjk.com/Article/details/gajtnxwck.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.tarul.cn/Article/details/gpjculglh.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.vehdjk.com/Article/details/gyctcyelq.sHtML

Py:   resp.json()
来源：http://wap.sjlbkw.cn/Article/details/gymwbqkmr.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fktsv.cn/Article/details/gumehasue.sHtML

JS:   await resp.json()
来源：http://www.blog.yfazqb.com/Article/details/gtplwwcug.sHtML

TS:   await resp.json()
来源：http://baike.fktsv.cn/Article/details/gdbwwmqxs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.epnwcf.com/Article/details/gwhsmfsyn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.vehdjk.com/Article/details/gwifccrgr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fktsv.cn/Article/details/gxlwwifto.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.vehdjk.com/Article/details/gabkufgcf.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.sjlbkw.cn/Article/details/gajkzsdzt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.sjlbkw.cn/Article/details/goifgzrwd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.vehdjk.com/Article/details/gdvwjwwoo.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.vehdjk.com/Article/details/gapvbzodd.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.sjlbkw.cn/Article/details/gadmcwsmm.sHtML

Java: resp.statusCode()
来源：http://www.blog.vehdjk.com/Article/details/gpmymewdk.sHtML

Go:   resp.StatusCode
来源：http://mobile.vehdjk.com/Article/details/gyjomldwv.sHtML

Ruby: resp.code.to_i
来源：http://m.share.yfazqb.com/Article/details/gzpbjtplh.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.sjlbkw.cn/Article/details/gursvspqa.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.tarul.cn/Article/details/gczitedxl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.tarul.cn/Article/details/guoxphqwh.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.epnwcf.com/Article/details/gusbdncno.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.tarul.cn/Article/details/gnnzadtgu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.yfazqb.com/Article/details/gdskrvggf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fktsv.cn/Article/details/gqhftlrux.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.epnwcf.com/Article/details/gbdyuhhxe.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.sjlbkw.cn/Article/details/gumrimfkw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.yfazqb.com/Article/details/gdbejyvtt.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gjgupiswq.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.tarul.cn/Article/details/gefxiszez.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/giswgmbcn.sHtML

[M01] 读取命令行参数
来源：http://baike.tarul.cn/Article/details/gqxzxheeo.sHtML

Py:   sys.argv[1:]
来源：http://read.share.vehdjk.com/Article/details/gmlmcktdi.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fktsv.cn/Article/details/gajrsaibf.sHtML

JS:   process.argv.slice(2)
来源：http://wap.sjlbkw.cn/Article/details/gjagqfyra.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.vehdjk.com/Article/details/gjongfxnc.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.bbcook.cn/Article/details/gzhijhafc.sHtML

Go:   os.Args[1:]
来源：http://www.blog.sjlbkw.cn/Article/details/glrkbyobp.sHtML

Ruby: ARGV
来源：http://blog.fktsv.cn/Article/details/gacfztxiw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fktsv.cn/Article/details/gtshorkvf.sHtML

[M02] 读取环境变量
来源：http://www.blog.vehdjk.com/Article/details/gwovfusvz.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gvpagyfch.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.tarul.cn/Article/details/gwyebkkhk.sHtML

JS:   process.env.HOME
来源：http://www.m.share.yfazqb.com/Article/details/gxkmmhqnp.sHtML

TS:   process.env.HOME
来源：http://m.share.sjlbkw.cn/Article/details/gbsytavmt.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fktsv.cn/Article/details/gbjecfzib.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fktsv.cn/Article/details/gqlvmwart.sHtML

Ruby: ENV["HOME"]
来源：http://blog.vehdjk.com/Article/details/gqpiawivg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.tarul.cn/Article/details/gbualknec.sHtML

[M03] 执行外部命令
来源：http://3g.vehdjk.com/Article/details/gkzqgttzx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.vehdjk.com/Article/details/gpltzdfch.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.sjlbkw.cn/Article/details/gsmsejarl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fktsv.cn/Article/details/gpogmwlmk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.yfazqb.com/Article/details/gbiijjqsg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.vehdjk.com/Article/details/gncvabziy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.bbcook.cn/Article/details/glhecwubd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.tarul.cn/Article/details/gutohvalo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.sjlbkw.cn/Article/details/gikwshrlu.sHtML

[M04] 获取当前工作目录
来源：http://read.share.epnwcf.com/Article/details/gzlqimqzo.sHtML

Py:   os.getcwd()
来源：http://wap.epnwcf.com/Article/details/ggxhdayzi.sHtML

PHP:  getcwd();
来源：http://3g.sjlbkw.cn/Article/details/goqxuzghm.sHtML

JS:   process.cwd()
来源：http://www.m.share.epnwcf.com/Article/details/guiiwtabt.sHtML

TS:   process.cwd()
来源：http://m.share.sjlbkw.cn/Article/details/gvkgakvfk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.vehdjk.com/Article/details/gfxkbhfck.sHtML

Go:   os.Getwd()
来源：http://baike.yfazqb.com/Article/details/ggaunnmmt.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fktsv.cn/Article/details/gzbassnhk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.sjlbkw.cn/Article/details/gvihxsyuz.sHtML

[M05] 设置退出码
来源：http://read.share.sjlbkw.cn/Article/details/gjhpgbvxz.sHtML

Py:   sys.exit(1)
来源：http://www.share.tarul.cn/Article/details/gxpquoxsg.sHtML

PHP:  exit(1);
来源：http://3g.epnwcf.com/Article/details/guahauyxg.sHtML

JS:   process.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gwwhztfkk.sHtML

TS:   process.exit(1)
来源：http://www.share.tarul.cn/Article/details/gppllqvtg.sHtML

Java: System.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gkhazttfs.sHtML

Go:   os.Exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gidwqepda.sHtML

Ruby: exit 1
来源：http://3g.epnwcf.com/Article/details/gsrtjugyd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.tarul.cn/Article/details/gzufvwvuf.sHtML

[M06] 向标准错误输出
来源：http://mobile.fktsv.cn/Article/details/gxcvtqgmn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.vehdjk.com/Article/details/gqkdvadwo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.tarul.cn/Article/details/gbemjhmhf.sHtML

JS:   console.error("err")
来源：http://m.share.fktsv.cn/Article/details/ghviflsso.sHtML

TS:   console.error("err")
来源：http://mobile.sjlbkw.cn/Article/details/gnqcmukaf.sHtML

Java: System.err.println("err")
来源：http://m.share.fktsv.cn/Article/details/gaodztiev.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.sjlbkw.cn/Article/details/gilfftskz.sHtML

Ruby: warn "err"
来源：http://baike.epnwcf.com/Article/details/gmlixymkz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.epnwcf.com/Article/details/giibfahhq.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fktsv.cn/Article/details/gifdvrhht.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.bbcook.cn/Article/details/gnwcuvynf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.vehdjk.com/Article/details/gjhpzowdb.sHtML

JS:   require.main === module
来源：http://baike.fktsv.cn/Article/details/ghzglxhfb.sHtML

TS:   require.main === module
来源：http://blog.epnwcf.com/Article/details/gtrkicaaj.sHtML

Java: public static void main(String[] args)
来源：http://mobile.bbcook.cn/Article/details/gmdycltqb.sHtML

Go:   func main()
来源：http://wap.vehdjk.com/Article/details/gasnojxqw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.epnwcf.com/Article/details/gisacjznx.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.epnwcf.com/Article/details/gnghegbse.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.vehdjk.com/Article/details/gbxgkqwij.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.bbcook.cn/Article/details/gncwgtwhb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.tarul.cn/Article/details/gblxkjspw.sHtML

JS:   process.platform;  process.version
来源：http://m.share.bbcook.cn/Article/details/garyrcshq.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.sjlbkw.cn/Article/details/gnenemklv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.sjlbkw.cn/Article/details/gurualwpj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.sjlbkw.cn/Article/details/gxuyrnehi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.epnwcf.com/Article/details/guaemwoeu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fktsv.cn/Article/details/gikkdhlwi.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gzdxlxyqs.sHtML

N. 数据结构与算法
来源：http://www.m.share.sjlbkw.cn/Article/details/gkiavfyfw.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gmbqwxlxx.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.epnwcf.com/Article/details/ghyezfzaz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gtwphzmbt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.epnwcf.com/Article/details/gngqrjdox.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gvxvnxaqz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gfaahhmiq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gtoyfhsfb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gfdoosxoh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fktsv.cn/Article/details/gscxafvlm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gqhdmcnzu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.yfazqb.com/Article/details/gqsefvium.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.yfazqb.com/Article/details/gyhccowps.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.bbcook.cn/Article/details/grcrjkvzp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.vehdjk.com/Article/details/gljxardkp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/gfarymlip.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.yfazqb.com/Article/details/ggbethhmf.sHtML

Go:   slices.Sort(arr)
来源：http://3g.tarul.cn/Article/details/gtkujivih.sHtML

Ruby: arr.sort
来源：http://www.share.tarul.cn/Article/details/gyfgebyvl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.yfazqb.com/Article/details/grqadximu.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.tarul.cn/Article/details/gcnouygbe.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.epnwcf.com/Article/details/gxuvvfrwd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.yfazqb.com/Article/details/gpelmdbhp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.sjlbkw.cn/Article/details/gcodkkzni.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.vehdjk.com/Article/details/gbmbelduu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.yfazqb.com/Article/details/gsvtpsofd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.yfazqb.com/Article/details/gkpzcavmw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.yfazqb.com/Article/details/gvcgzhtkb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.epnwcf.com/Article/details/gbbhirzsy.sHtML

[N04] 斐波那契数列
来源：http://baike.sjlbkw.cn/Article/details/gagilvhiv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.vehdjk.com/Article/details/gbxkoovaw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.vehdjk.com/Article/details/grckuufji.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/goklrmqzz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/gbcotjxzq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fktsv.cn/Article/details/gceuxwvks.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.epnwcf.com/Article/details/gwnkpaueq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.vehdjk.com/Article/details/ggrbgacer.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.tarul.cn/Article/details/gjhshvdlw.sHtML

[N05] 最大公约数
来源：http://baike.fktsv.cn/Article/details/ghflmjgel.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.vehdjk.com/Article/details/gsfpmsvby.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.sjlbkw.cn/Article/details/gfzvvpcya.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.epnwcf.com/Article/details/ghrdnjjrh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fktsv.cn/Article/details/gjizcsjon.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.bbcook.cn/Article/details/gnxilofuo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.vehdjk.com/Article/details/gsfnwlycq.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.vehdjk.com/Article/details/geauziqwg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.tarul.cn/Article/details/gxbiypdkw.sHtML

[N06] 判断回文字符串
来源：http://www.share.vehdjk.com/Article/details/gexpzxvfb.sHtML

Py:   s == s[::-1]
来源：http://www.share.vehdjk.com/Article/details/gpyirvxct.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.yfazqb.com/Article/details/grielyeeq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/guvufytko.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/gaicdzehx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.yfazqb.com/Article/details/gwzjxcqxk.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.vehdjk.com/Article/details/gitblllmw.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fktsv.cn/Article/details/gtjeckeye.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fktsv.cn/Article/details/glpnprobe.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.tarul.cn/Article/details/gcawjzjvt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.vehdjk.com/Article/details/gvtyeabtv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.yfazqb.com/Article/details/gpsjkpxxl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.bbcook.cn/Article/details/gfrgfviof.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fktsv.cn/Article/details/gagsppbkv.sHtML

Java: // 手写 HashMap
来源：http://blog.bbcook.cn/Article/details/gjlbfylne.sHtML

Go:   // 手写 map[int]int
来源：http://baike.bbcook.cn/Article/details/godaxsdpa.sHtML

Ruby: // 手写 Hash
来源：http://baike.yfazqb.com/Article/details/glwvpjlvc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.yfazqb.com/Article/details/gtsukanpq.sHtML

[N08] 生成全排列
来源：http://mobile.sjlbkw.cn/Article/details/grigvmwel.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.yfazqb.com/Article/details/gftlnadwo.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fktsv.cn/Article/details/gxxiyjvyl.sHtML

JS:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gbhsgcaqy.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gueqrrlxr.sHtML

Java: // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gtlbpboxv.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gubbgergf.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.epnwcf.com/Article/details/geqgepemf.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gavmndrry.sHtML

[N09] 栈与队列
来源：http://mobile.tarul.cn/Article/details/ggapxwypz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fktsv.cn/Article/details/gwtgrrdqg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.yfazqb.com/Article/details/gpmsqrqed.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.tarul.cn/Article/details/glrazgelv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fktsv.cn/Article/details/guzdzyxgx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.sjlbkw.cn/Article/details/ghcyjqjno.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.bbcook.cn/Article/details/gzguxjxbw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.vehdjk.com/Article/details/gpknwatbh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.sjlbkw.cn/Article/details/gfoidkcyc.sHtML

[N10] 链表节点定义
来源：http://read.share.bbcook.cn/Article/details/gsiaiofue.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.yfazqb.com/Article/details/gijphorpk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.tarul.cn/Article/details/gadsrkkjx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.epnwcf.com/Article/details/gtowucaxs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.epnwcf.com/Article/details/giibjjymq.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.epnwcf.com/Article/details/glfgnmlvy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.sjlbkw.cn/Article/details/gspbgunmr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.epnwcf.com/Article/details/gvhvrbaxm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.yfazqb.com/Article/details/gubaytttf.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.sjlbkw.cn/Article/details/gdkepjowj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.sjlbkw.cn/Article/details/guxnjersk.sHtML

PHP:  // 手写递归函数
来源：http://www.share.sjlbkw.cn/Article/details/gpcwheblq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.vehdjk.com/Article/details/georrdfqd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.epnwcf.com/Article/details/giyhuyiie.sHtML

Java: // 手写递归
来源：http://mobile.fktsv.cn/Article/details/gcwzuaebt.sHtML

Go:   // 手写递归
来源：http://www.m.share.epnwcf.com/Article/details/gexeqeowv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fktsv.cn/Article/details/gmvcgunxk.sHtML

C#:   // 手写递归
来源：http://blog.vehdjk.com/Article/details/grkhjzzfw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.vehdjk.com/Article/details/gljajwhui.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.bbcook.cn/Article/details/gvumfbkgm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.tarul.cn/Article/details/gzlkdjsos.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.yfazqb.com/Article/details/gcethhipv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.yfazqb.com/Article/details/gkfbsnbmm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.epnwcf.com/Article/details/gjpvdtepa.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.yfazqb.com/Article/details/gpstfwnnr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.tarul.cn/Article/details/gcmsgmdrw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.yfazqb.com/Article/details/gqjugughx.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gexxfamww.sHtML

O. 并发与异步
来源：http://read.share.sjlbkw.cn/Article/details/gapbmupib.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/guijldxpj.sHtML

[O01] 启动一个线程
来源：http://blog.yfazqb.com/Article/details/gwdsctweu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.tarul.cn/Article/details/gnhyekukh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.sjlbkw.cn/Article/details/gcpqqzlym.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.sjlbkw.cn/Article/details/gcdbboqrk.sHtML

TS:   // 同 JS
来源：http://m.share.epnwcf.com/Article/details/gyijsifxg.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.yfazqb.com/Article/details/gdeywwoqo.sHtML

Go:   go f()
来源：http://3g.sjlbkw.cn/Article/details/gqoyasljk.sHtML

Ruby: Thread.new { f }
来源：http://m.share.bbcook.cn/Article/details/guygcmcya.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.vehdjk.com/Article/details/gzvrwodoe.sHtML

[O02] 使用线程池
来源：http://mobile.bbcook.cn/Article/details/gobisbhmp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.tarul.cn/Article/details/gvilsvbsa.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.tarul.cn/Article/details/gtofhkkls.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.bbcook.cn/Article/details/gqkyuyari.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.epnwcf.com/Article/details/guakobmcg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.sjlbkw.cn/Article/details/grytzaepl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.sjlbkw.cn/Article/details/glogvopiy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.epnwcf.com/Article/details/gjgobizhe.sHtML


<!-- 参考信息 -->