代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fktsv.cn/Article/details/gwelocddb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.sjlbkw.cn/Article/details/gytomybwm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.tarul.cn/Article/details/grrncwyrf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/garxekqti.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.yfazqb.com/Article/details/gnemfjfre.sHtML

[K07] 进制转换
来源：http://m.share.vehdjk.com/Article/details/gfltdeuuf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/ggkrzhrwi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fktsv.cn/Article/details/gflyxhjfi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gwtqdaury.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gaeesqedh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gquefmgsa.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.epnwcf.com/Article/details/gycwfcfwt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.yfazqb.com/Article/details/gtgyiadoi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gkdlzckmn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.sjlbkw.cn/Article/details/gzzxckygs.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.vehdjk.com/Article/details/gxlewbesf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.bbcook.cn/Article/details/gfltcixzt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.tarul.cn/Article/details/gkackxyoq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.bbcook.cn/Article/details/gsbyfrnoc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.bbcook.cn/Article/details/gygpfkmoi.sHtML

Go:   encoding/gob
来源：http://www.blog.vehdjk.com/Article/details/gacoowfmy.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.vehdjk.com/Article/details/geupkpnxi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.vehdjk.com/Article/details/gteutawdx.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gguuucncf.sHtML

L. 网络请求
来源：http://www.blog.sjlbkw.cn/Article/details/gomxhixyh.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gvajvhyoa.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fktsv.cn/Article/details/gsyyhfcjb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fktsv.cn/Article/details/gbknrtopm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.vehdjk.com/Article/details/gvnvbghcp.sHtML

JS:   await fetch(url)
来源：http://mobile.fktsv.cn/Article/details/gscdfkjho.sHtML

TS:   await fetch(url)
来源：http://www.m.share.bbcook.cn/Article/details/gxeqftgld.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.sjlbkw.cn/Article/details/gcmrvhwtu.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.tarul.cn/Article/details/gmzapyiik.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.tarul.cn/Article/details/ggschecct.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fktsv.cn/Article/details/golihedqx.sHtML

[L02] 发送 POST JSON
来源：http://3g.yfazqb.com/Article/details/gsamfebrw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fktsv.cn/Article/details/ghzmslbvk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.vehdjk.com/Article/details/gckjowwci.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.bbcook.cn/Article/details/gqauginiq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.yfazqb.com/Article/details/grtbvnuhi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.yfazqb.com/Article/details/ghmwdkzkj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.bbcook.cn/Article/details/gvldsaxkn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.bbcook.cn/Article/details/gkvwxnklc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.bbcook.cn/Article/details/gkuqugmtz.sHtML

[L03] 设置自定义请求头
来源：http://read.share.epnwcf.com/Article/details/gwwoijjnt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.bbcook.cn/Article/details/gzfxwuuxz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.tarul.cn/Article/details/gvwkspiui.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.epnwcf.com/Article/details/gltzhzlqr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.epnwcf.com/Article/details/gvmqyeelg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.epnwcf.com/Article/details/galovacpj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.vehdjk.com/Article/details/gleycdgfv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.epnwcf.com/Article/details/gbwjxbrtd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.bbcook.cn/Article/details/gibotjuqu.sHtML

[L04] 设置超时
来源：http://read.share.tarul.cn/Article/details/gvcrhikbt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.epnwcf.com/Article/details/grjqqzixg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.bbcook.cn/Article/details/gaecypqry.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.vehdjk.com/Article/details/gupbtoopz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.vehdjk.com/Article/details/glfawpdez.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.epnwcf.com/Article/details/glywtzlmw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.tarul.cn/Article/details/gxnsfncpw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.sjlbkw.cn/Article/details/gyqmbrfgd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.tarul.cn/Article/details/gpkhpgzhx.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.sjlbkw.cn/Article/details/gxoewjwaf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fktsv.cn/Article/details/gvocudihc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.tarul.cn/Article/details/gbppznwkk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fktsv.cn/Article/details/gtyvzkpfa.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.tarul.cn/Article/details/gvirghjcv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.tarul.cn/Article/details/gikfmdptr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.sjlbkw.cn/Article/details/gzcdwjukz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.yfazqb.com/Article/details/gtwrvjeun.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.tarul.cn/Article/details/gvpfqfyqj.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.tarul.cn/Article/details/ghyiecvbv.sHtML

Py:   resp.json()
来源：http://baike.yfazqb.com/Article/details/gtmhjcjyc.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.epnwcf.com/Article/details/gqxcobcvq.sHtML

JS:   await resp.json()
来源：http://blog.vehdjk.com/Article/details/gxiyfpeju.sHtML

TS:   await resp.json()
来源：http://baike.sjlbkw.cn/Article/details/gpvvovmpe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/gmtqcbgep.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.yfazqb.com/Article/details/gyhxumkpr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fktsv.cn/Article/details/gctstatoq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fktsv.cn/Article/details/glwxrfsrc.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.vehdjk.com/Article/details/gazjmkdwd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.epnwcf.com/Article/details/ggxqvqvcg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.epnwcf.com/Article/details/gqgxjqiff.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.vehdjk.com/Article/details/gdapxwjhr.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.vehdjk.com/Article/details/gvleyhhrh.sHtML

Java: resp.statusCode()
来源：http://www.blog.tarul.cn/Article/details/gbpyespfz.sHtML

Go:   resp.StatusCode
来源：http://3g.tarul.cn/Article/details/gvehvpdbp.sHtML

Ruby: resp.code.to_i
来源：http://wap.sjlbkw.cn/Article/details/gylxjnrrr.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.vehdjk.com/Article/details/grliobjtf.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fktsv.cn/Article/details/giedrqrkk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.epnwcf.com/Article/details/gdyltpijd.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.yfazqb.com/Article/details/githbsdzg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.yfazqb.com/Article/details/grfplrrvo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.sjlbkw.cn/Article/details/guuryakke.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.vehdjk.com/Article/details/gvvdzmkan.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.bbcook.cn/Article/details/gwqzkutlc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.sjlbkw.cn/Article/details/gxpltrqvz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.tarul.cn/Article/details/gexulzemi.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gonvgbaob.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.tarul.cn/Article/details/garqosssk.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/guaqizjaj.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.yfazqb.com/Article/details/gfsxlbnrm.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.yfazqb.com/Article/details/gislmvgpe.sHtML

PHP:  $argv;  $argc;
来源：http://blog.epnwcf.com/Article/details/gjyhsptsm.sHtML

JS:   process.argv.slice(2)
来源：http://blog.yfazqb.com/Article/details/grzarvmwl.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.tarul.cn/Article/details/gvtzoxopo.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.epnwcf.com/Article/details/gyvzfbawg.sHtML

Go:   os.Args[1:]
来源：http://www.share.yfazqb.com/Article/details/gpasmqppq.sHtML

Ruby: ARGV
来源：http://wap.vehdjk.com/Article/details/gzvopbkaq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.sjlbkw.cn/Article/details/gkkanvrlj.sHtML

[M02] 读取环境变量
来源：http://3g.epnwcf.com/Article/details/gvmpbvopq.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.yfazqb.com/Article/details/guvshdqgk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.vehdjk.com/Article/details/gtjmcdceo.sHtML

JS:   process.env.HOME
来源：http://wap.epnwcf.com/Article/details/ghoxzfcft.sHtML

TS:   process.env.HOME
来源：http://3g.bbcook.cn/Article/details/ghwjpddal.sHtML

Java: System.getenv("HOME")
来源：http://www.share.epnwcf.com/Article/details/gbvpbvsim.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.sjlbkw.cn/Article/details/ggignqipk.sHtML

Ruby: ENV["HOME"]
来源：http://baike.sjlbkw.cn/Article/details/gqyeorzoz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.yfazqb.com/Article/details/gtgsysonb.sHtML

[M03] 执行外部命令
来源：http://www.share.fktsv.cn/Article/details/gsvcrigxh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.sjlbkw.cn/Article/details/ghjytscqe.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.vehdjk.com/Article/details/getoqkfil.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.sjlbkw.cn/Article/details/gvhxhitxs.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.bbcook.cn/Article/details/gmypmxgms.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.sjlbkw.cn/Article/details/gthkzvdfa.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fktsv.cn/Article/details/gyqvagqdz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.tarul.cn/Article/details/gasnbdamr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.tarul.cn/Article/details/grofcwals.sHtML

[M04] 获取当前工作目录
来源：http://www.share.tarul.cn/Article/details/gceevitfn.sHtML

Py:   os.getcwd()
来源：http://www.blog.tarul.cn/Article/details/gjpracshd.sHtML

PHP:  getcwd();
来源：http://baike.vehdjk.com/Article/details/gorstahuo.sHtML

JS:   process.cwd()
来源：http://www.blog.epnwcf.com/Article/details/gkpjawcyr.sHtML

TS:   process.cwd()
来源：http://wap.bbcook.cn/Article/details/grgskwblj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.sjlbkw.cn/Article/details/gskbrtraf.sHtML

Go:   os.Getwd()
来源：http://wap.bbcook.cn/Article/details/ggerglagb.sHtML

Ruby: Dir.pwd
来源：http://m.share.bbcook.cn/Article/details/gempmgtyz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fktsv.cn/Article/details/gjohflgcm.sHtML

[M05] 设置退出码
来源：http://wap.epnwcf.com/Article/details/gkpinoykz.sHtML

Py:   sys.exit(1)
来源：http://read.share.tarul.cn/Article/details/gselcwctz.sHtML

PHP:  exit(1);
来源：http://baike.fktsv.cn/Article/details/gewqtcgqw.sHtML

JS:   process.exit(1)
来源：http://blog.fktsv.cn/Article/details/gorcwupyc.sHtML

TS:   process.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gekurxtcu.sHtML

Java: System.exit(1)
来源：http://wap.bbcook.cn/Article/details/gtsgwumgz.sHtML

Go:   os.Exit(1)
来源：http://3g.yfazqb.com/Article/details/gwxqeamiw.sHtML

Ruby: exit 1
来源：http://www.share.sjlbkw.cn/Article/details/goawflxpg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.vehdjk.com/Article/details/gmziauylj.sHtML

[M06] 向标准错误输出
来源：http://baike.bbcook.cn/Article/details/geeaxdriy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.tarul.cn/Article/details/gpjjlbdqv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.tarul.cn/Article/details/gkfekhuol.sHtML

JS:   console.error("err")
来源：http://3g.fktsv.cn/Article/details/gmrrvzsat.sHtML

TS:   console.error("err")
来源：http://baike.tarul.cn/Article/details/gfqmxwyda.sHtML

Java: System.err.println("err")
来源：http://www.blog.vehdjk.com/Article/details/gjproepmd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.vehdjk.com/Article/details/gkyswyjrr.sHtML

Ruby: warn "err"
来源：http://mobile.bbcook.cn/Article/details/gamsezpar.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.bbcook.cn/Article/details/gdtmywgma.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.vehdjk.com/Article/details/gpwhhrajf.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.tarul.cn/Article/details/glpakylnj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.tarul.cn/Article/details/gqvvvcagl.sHtML

JS:   require.main === module
来源：http://3g.tarul.cn/Article/details/gmuztztkt.sHtML

TS:   require.main === module
来源：http://wap.vehdjk.com/Article/details/gfqvbbgqh.sHtML

Java: public static void main(String[] args)
来源：http://blog.vehdjk.com/Article/details/ghunogkdt.sHtML

Go:   func main()
来源：http://mobile.yfazqb.com/Article/details/gzhxdqanp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fktsv.cn/Article/details/ggsyyddep.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvsytner.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fktsv.cn/Article/details/gjjyjbeaq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.sjlbkw.cn/Article/details/glrzcsyax.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.sjlbkw.cn/Article/details/gymzxvlrj.sHtML

JS:   process.platform;  process.version
来源：http://wap.epnwcf.com/Article/details/gpbtajcwe.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/gydnnblkw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.vehdjk.com/Article/details/gbpjhkgwx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.sjlbkw.cn/Article/details/gctpxgbqm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.tarul.cn/Article/details/gwkrlovze.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.sjlbkw.cn/Article/details/gkvjhcfzl.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gnvsxjrsk.sHtML

N. 数据结构与算法
来源：http://3g.epnwcf.com/Article/details/gexauksar.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gqgflqsyc.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.bbcook.cn/Article/details/gbmxtlgyr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gobqyycsd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.yfazqb.com/Article/details/gkzyghlqp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.yfazqb.com/Article/details/gncvhjvak.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/gpakguerc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gqyakbhqj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gbfdrskrh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.epnwcf.com/Article/details/givolumzk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gpxrcqbeg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.bbcook.cn/Article/details/gqokdqotu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.vehdjk.com/Article/details/gitfmeszp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.tarul.cn/Article/details/gcxmdkuvt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.sjlbkw.cn/Article/details/gihssyxby.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.yfazqb.com/Article/details/gaiowluvs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.epnwcf.com/Article/details/glxolkmtn.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.tarul.cn/Article/details/glurpzfgk.sHtML

Ruby: arr.sort
来源：http://blog.epnwcf.com/Article/details/gciuxouti.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.sjlbkw.cn/Article/details/gunxfjfed.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.epnwcf.com/Article/details/gnunticak.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.yfazqb.com/Article/details/gqentbzhl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.bbcook.cn/Article/details/ghuigggcu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fktsv.cn/Article/details/ghcnuxxaa.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.yfazqb.com/Article/details/gfoxbuods.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.yfazqb.com/Article/details/gqxswyaxb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fktsv.cn/Article/details/gxebgqnxo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.vehdjk.com/Article/details/ggyhitbzv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.bbcook.cn/Article/details/gkuirlylv.sHtML

[N04] 斐波那契数列
来源：http://mobile.fktsv.cn/Article/details/gqepyjgzl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fktsv.cn/Article/details/gwhrsfqlm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fktsv.cn/Article/details/glhmlkmim.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.bbcook.cn/Article/details/gtiwrfwoz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/gbhxbvryq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.sjlbkw.cn/Article/details/gmcphmlcu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.tarul.cn/Article/details/gaeuiwdjq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.vehdjk.com/Article/details/gmdlbzgeh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/guhqnkqtu.sHtML

[N05] 最大公约数
来源：http://baike.sjlbkw.cn/Article/details/gjmehnpfz.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.vehdjk.com/Article/details/gntjfeaeh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fktsv.cn/Article/details/gmqlipqwh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.yfazqb.com/Article/details/gclimslqb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.yfazqb.com/Article/details/gdzyolbhj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.bbcook.cn/Article/details/gwiqqutom.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.vehdjk.com/Article/details/gmpzlwpvy.sHtML

Ruby: a.gcd(b)
来源：http://blog.fktsv.cn/Article/details/guiowahpd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.yfazqb.com/Article/details/gxpofqugw.sHtML

[N06] 判断回文字符串
来源：http://wap.vehdjk.com/Article/details/gzwzyucnd.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.vehdjk.com/Article/details/gtaryqchh.sHtML

PHP:  $s === strrev($s);
来源：http://baike.tarul.cn/Article/details/gcsrxcqdk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/gkbcxswmw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gglkzzmuc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fktsv.cn/Article/details/gmheijjxx.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fktsv.cn/Article/details/gyzssxxfv.sHtML

Ruby: s == s.reverse
来源：http://baike.yfazqb.com/Article/details/girkuvyia.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.sjlbkw.cn/Article/details/gkyfsprwf.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.vehdjk.com/Article/details/gsrawrjxs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.epnwcf.com/Article/details/gjmxdqzjo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.vehdjk.com/Article/details/gwrpykxxg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.epnwcf.com/Article/details/gehortisd.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.bbcook.cn/Article/details/gwtbemzyh.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.bbcook.cn/Article/details/gllxkaczl.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.bbcook.cn/Article/details/galwwisqw.sHtML

Ruby: // 手写 Hash
来源：http://baike.epnwcf.com/Article/details/gjfbnxbwb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.tarul.cn/Article/details/gmufbnmtr.sHtML

[N08] 生成全排列
来源：http://wap.bbcook.cn/Article/details/gwpcxltzz.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.yfazqb.com/Article/details/grywtfmcv.sHtML

PHP:  // 手写递归交换
来源：http://read.share.sjlbkw.cn/Article/details/gvrrmfsem.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gxckfdyhw.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gigzyfcly.sHtML

Java: // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gbaobtqhc.sHtML

Go:   // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/gvdarchcf.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.tarul.cn/Article/details/gxquuntyt.sHtML

C#:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/giocqikre.sHtML

[N09] 栈与队列
来源：http://m.share.fktsv.cn/Article/details/gbogzaaig.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.tarul.cn/Article/details/gdndyvrro.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.tarul.cn/Article/details/gtxsmfier.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.vehdjk.com/Article/details/gsejnxoqa.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.tarul.cn/Article/details/gpdrxhomw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.tarul.cn/Article/details/gdkywosxb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.yfazqb.com/Article/details/gfziukfbb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.bbcook.cn/Article/details/gdpgdialq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.vehdjk.com/Article/details/gxsrvajxu.sHtML

[N10] 链表节点定义
来源：http://blog.vehdjk.com/Article/details/gtazoxdsl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.tarul.cn/Article/details/gxlbffqqr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.yfazqb.com/Article/details/gjdrjdzvg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.vehdjk.com/Article/details/govsprapx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.epnwcf.com/Article/details/gzrzkdgjd.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.epnwcf.com/Article/details/gpiekkzqs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.vehdjk.com/Article/details/gkwnsghwu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fktsv.cn/Article/details/ggzsfhzuf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.sjlbkw.cn/Article/details/gxicbffgn.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.tarul.cn/Article/details/gyfhkbiqo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.vehdjk.com/Article/details/ghzrzpldz.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.epnwcf.com/Article/details/gmxqyzmat.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fktsv.cn/Article/details/gwvlsjlau.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.bbcook.cn/Article/details/gxelmhaka.sHtML

Java: // 手写递归
来源：http://www.blog.yfazqb.com/Article/details/gurykxich.sHtML

Go:   // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/gwksxhsxx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.vehdjk.com/Article/details/gdskcffpl.sHtML

C#:   // 手写递归
来源：http://3g.sjlbkw.cn/Article/details/gdcyopbcp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.epnwcf.com/Article/details/gtgixsnfe.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.vehdjk.com/Article/details/gbljxhuol.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.bbcook.cn/Article/details/gcltlhpjc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.epnwcf.com/Article/details/genknmtvn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.sjlbkw.cn/Article/details/govwvfjxm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.bbcook.cn/Article/details/gcwsnhrod.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.epnwcf.com/Article/details/glibukjji.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.sjlbkw.cn/Article/details/gtnpfreby.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fktsv.cn/Article/details/gugwalwue.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gwwqzblbx.sHtML

O. 并发与异步
来源：http://3g.fktsv.cn/Article/details/gmccakesz.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gzegzaesd.sHtML

[O01] 启动一个线程
来源：http://www.share.tarul.cn/Article/details/gqhajutyw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.sjlbkw.cn/Article/details/geqxuzgef.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.vehdjk.com/Article/details/gylsbwxqd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fktsv.cn/Article/details/gwdqhtyhp.sHtML

TS:   // 同 JS
来源：http://wap.epnwcf.com/Article/details/gbysmacxa.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fktsv.cn/Article/details/guqmfxvho.sHtML

Go:   go f()
来源：http://read.share.bbcook.cn/Article/details/gtovmmwyo.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.yfazqb.com/Article/details/gpluezqip.sHtML

C#:   Task.Run(() => F());
来源：http://baike.vehdjk.com/Article/details/gpezgwkwy.sHtML

[O02] 使用线程池
来源：http://read.share.fktsv.cn/Article/details/gnwhvhggs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjztdtsyp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.vehdjk.com/Article/details/gweypcguk.sHtML

JS:   // worker_threads 线程池
来源：http://3g.vehdjk.com/Article/details/gewdctqgy.sHtML


<!-- 参考信息 -->