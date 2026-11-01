代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/glidlersl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gaxwalxeb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gyyynxyih.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.tarul.cn/Article/details/gpnwaomoc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.sjlbkw.cn/Article/details/gjkgogfvy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gihwxugdo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.bbcook.cn/Article/details/gggtiofba.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.tarul.cn/Article/details/gicnmoqtm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.bbcook.cn/Article/details/gjgttltwd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gapzbdpug.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.vehdjk.com/Article/details/gdhzxrxds.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.tarul.cn/Article/details/gtvxnocqy.sHtML

Go:   encoding/gob
来源：http://baike.vehdjk.com/Article/details/gczfhswdx.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.vehdjk.com/Article/details/gqyzgifha.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.sjlbkw.cn/Article/details/gdgooujoy.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gfiweadvb.sHtML

L. 网络请求
来源：http://www.share.vehdjk.com/Article/details/gufemhoks.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/giywbsrtp.sHtML

[L01] 发送 GET 请求
来源：http://mobile.vehdjk.com/Article/details/gaygfnvoa.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.tarul.cn/Article/details/gpyaqzvpf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fktsv.cn/Article/details/glnhvttau.sHtML

JS:   await fetch(url)
来源：http://baike.bbcook.cn/Article/details/guwaqqjyi.sHtML

TS:   await fetch(url)
来源：http://m.share.tarul.cn/Article/details/gccfnhdeq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.bbcook.cn/Article/details/glxhxlygg.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.vehdjk.com/Article/details/gulludlgg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.bbcook.cn/Article/details/gxsxwdyqh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fktsv.cn/Article/details/gxqnfscto.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gnorkoxim.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.sjlbkw.cn/Article/details/goxdlcezm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.epnwcf.com/Article/details/ghltkitww.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fktsv.cn/Article/details/gawhmofpc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.vehdjk.com/Article/details/gqxjlrsqk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.yfazqb.com/Article/details/gbxixqoep.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.yfazqb.com/Article/details/gvgjvbaby.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.vehdjk.com/Article/details/gpbrvhfdy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.vehdjk.com/Article/details/gsaqxhcgc.sHtML

[L03] 设置自定义请求头
来源：http://m.share.sjlbkw.cn/Article/details/gyvvziqwh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.bbcook.cn/Article/details/guugutxry.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.epnwcf.com/Article/details/gucbfbzje.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.epnwcf.com/Article/details/gsgmpwnct.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.sjlbkw.cn/Article/details/gfcscnfyi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.tarul.cn/Article/details/gugskxufm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.epnwcf.com/Article/details/gkptcnhaf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.tarul.cn/Article/details/gfhwixfqw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.vehdjk.com/Article/details/gccfmopjq.sHtML

[L04] 设置超时
来源：http://m.share.vehdjk.com/Article/details/gaowzgnjr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.bbcook.cn/Article/details/gqbjmqduj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fktsv.cn/Article/details/gtjoirhmk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.yfazqb.com/Article/details/gdvtelwda.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.epnwcf.com/Article/details/gyjtmuome.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.vehdjk.com/Article/details/gmbkqutsq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.yfazqb.com/Article/details/gtvyjwgou.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.epnwcf.com/Article/details/gophzcfnu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.yfazqb.com/Article/details/gqakkksvg.sHtML

[L05] 上传文件（multipart）
来源：http://wap.tarul.cn/Article/details/gwobppicj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.vehdjk.com/Article/details/gyuhwpaov.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.bbcook.cn/Article/details/ggnkuztka.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.epnwcf.com/Article/details/ggocgqech.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.yfazqb.com/Article/details/gybsnihph.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.vehdjk.com/Article/details/getvlzten.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.epnwcf.com/Article/details/ghunekpuc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.sjlbkw.cn/Article/details/gqpnnhmaq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.yfazqb.com/Article/details/gzknrefms.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.tarul.cn/Article/details/glwopnjvi.sHtML

Py:   resp.json()
来源：http://blog.bbcook.cn/Article/details/gwgkeyuvr.sHtML

PHP:  json_decode($body, true);
来源：http://baike.epnwcf.com/Article/details/gntwqatsh.sHtML

JS:   await resp.json()
来源：http://www.share.yfazqb.com/Article/details/guiijkdul.sHtML

TS:   await resp.json()
来源：http://www.blog.yfazqb.com/Article/details/gifhaqnpo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.vehdjk.com/Article/details/ghgfilqmz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.vehdjk.com/Article/details/gwxljseee.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.sjlbkw.cn/Article/details/gsqnegryc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fktsv.cn/Article/details/gormodhbg.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.bbcook.cn/Article/details/gbjoqcxqq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.yfazqb.com/Article/details/gbkzcibst.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.yfazqb.com/Article/details/gocugeezn.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.yfazqb.com/Article/details/ghiouetgq.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.vehdjk.com/Article/details/ghpecxvll.sHtML

Java: resp.statusCode()
来源：http://www.share.epnwcf.com/Article/details/grcxmrkuy.sHtML

Go:   resp.StatusCode
来源：http://mobile.epnwcf.com/Article/details/grffkaukk.sHtML

Ruby: resp.code.to_i
来源：http://baike.tarul.cn/Article/details/gvnzhcczx.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.bbcook.cn/Article/details/gpkdbdeen.sHtML

[L08] 并发请求多个地址
来源：http://baike.tarul.cn/Article/details/gfqgwejfe.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.epnwcf.com/Article/details/gtpzzbnzb.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.vehdjk.com/Article/details/gvncahvzk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.tarul.cn/Article/details/gakvridub.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/gvgoejdnt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.yfazqb.com/Article/details/gbzygfevr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.epnwcf.com/Article/details/gkqwocypk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.yfazqb.com/Article/details/gdtahlfuz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gcywgsnau.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gpgwespof.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.bbcook.cn/Article/details/gjmnlffnq.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gyagssqvv.sHtML

[M01] 读取命令行参数
来源：http://read.share.yfazqb.com/Article/details/gwruaogsb.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.tarul.cn/Article/details/grpxbueec.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.tarul.cn/Article/details/gwwopbxvs.sHtML

JS:   process.argv.slice(2)
来源：http://blog.tarul.cn/Article/details/gosmwqgtn.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.tarul.cn/Article/details/grvqosunp.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.yfazqb.com/Article/details/gvhliebar.sHtML

Go:   os.Args[1:]
来源：http://www.share.yfazqb.com/Article/details/gvuswxzcn.sHtML

Ruby: ARGV
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkjavuig.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.tarul.cn/Article/details/gatucvuzw.sHtML

[M02] 读取环境变量
来源：http://m.share.sjlbkw.cn/Article/details/gvrrhcump.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gnquxizoj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fktsv.cn/Article/details/guukskufq.sHtML

JS:   process.env.HOME
来源：http://mobile.yfazqb.com/Article/details/gqojsivsz.sHtML

TS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/gaakmmrot.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/garsxedxg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fktsv.cn/Article/details/gtjkjpimg.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.sjlbkw.cn/Article/details/givahlean.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.tarul.cn/Article/details/gdtubqyyp.sHtML

[M03] 执行外部命令
来源：http://3g.bbcook.cn/Article/details/glnjmijqs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.yfazqb.com/Article/details/gactghtwn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.epnwcf.com/Article/details/gvxqtwmpf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fktsv.cn/Article/details/glegtptlj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.yfazqb.com/Article/details/gpjnpnpvg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.epnwcf.com/Article/details/gvkkoeiml.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.tarul.cn/Article/details/gmcxgfexv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqmyowlr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.yfazqb.com/Article/details/gqgiaqbbh.sHtML

[M04] 获取当前工作目录
来源：http://mobile.yfazqb.com/Article/details/ghlytngmf.sHtML

Py:   os.getcwd()
来源：http://wap.tarul.cn/Article/details/gdryixrus.sHtML

PHP:  getcwd();
来源：http://read.share.sjlbkw.cn/Article/details/ggaqodkzl.sHtML

JS:   process.cwd()
来源：http://baike.bbcook.cn/Article/details/gpbdxlaah.sHtML

TS:   process.cwd()
来源：http://blog.yfazqb.com/Article/details/gpcfuivsp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.bbcook.cn/Article/details/gklqpaesu.sHtML

Go:   os.Getwd()
来源：http://wap.fktsv.cn/Article/details/gqbfwsssi.sHtML

Ruby: Dir.pwd
来源：http://mobile.fktsv.cn/Article/details/goqdsbfcp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.epnwcf.com/Article/details/gkyaiqecg.sHtML

[M05] 设置退出码
来源：http://www.share.yfazqb.com/Article/details/gzlkvfxql.sHtML

Py:   sys.exit(1)
来源：http://3g.tarul.cn/Article/details/gxnixrewc.sHtML

PHP:  exit(1);
来源：http://www.share.epnwcf.com/Article/details/ghoiczpgs.sHtML

JS:   process.exit(1)
来源：http://baike.vehdjk.com/Article/details/gjzxwkrrc.sHtML

TS:   process.exit(1)
来源：http://blog.bbcook.cn/Article/details/gnglzpyol.sHtML

Java: System.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gbemfmabr.sHtML

Go:   os.Exit(1)
来源：http://blog.fktsv.cn/Article/details/gjcqotely.sHtML

Ruby: exit 1
来源：http://baike.tarul.cn/Article/details/gwuoseiay.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.vehdjk.com/Article/details/gzasqwbfd.sHtML

[M06] 向标准错误输出
来源：http://www.share.yfazqb.com/Article/details/guvxvzbtz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.sjlbkw.cn/Article/details/grewnwyqy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.bbcook.cn/Article/details/gtrppgfpq.sHtML

JS:   console.error("err")
来源：http://mobile.yfazqb.com/Article/details/gzmcqvpxm.sHtML

TS:   console.error("err")
来源：http://www.share.yfazqb.com/Article/details/gluqegtyo.sHtML

Java: System.err.println("err")
来源：http://m.share.yfazqb.com/Article/details/gstgheawy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.vehdjk.com/Article/details/gdxtwzwlh.sHtML

Ruby: warn "err"
来源：http://baike.vehdjk.com/Article/details/gogdtysib.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fktsv.cn/Article/details/geqmbgvpz.sHtML

[M07] 判断是否为主入口
来源：http://3g.epnwcf.com/Article/details/gbfjsoytz.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.yfazqb.com/Article/details/gspsfbjio.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.epnwcf.com/Article/details/gyakdvcke.sHtML

JS:   require.main === module
来源：http://read.share.fktsv.cn/Article/details/gvhtvhbcn.sHtML

TS:   require.main === module
来源：http://3g.bbcook.cn/Article/details/gzaqlktdd.sHtML

Java: public static void main(String[] args)
来源：http://m.share.tarul.cn/Article/details/gftcujpga.sHtML

Go:   func main()
来源：http://baike.epnwcf.com/Article/details/gxshkbtcc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.sjlbkw.cn/Article/details/gitjutysv.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.vehdjk.com/Article/details/gcpuhxsnm.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.epnwcf.com/Article/details/gmiwaxlmp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.tarul.cn/Article/details/ggqhwcuqw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fktsv.cn/Article/details/gnqsfzmgq.sHtML

JS:   process.platform;  process.version
来源：http://baike.bbcook.cn/Article/details/gdjkhsnvt.sHtML

TS:   process.platform;  process.version
来源：http://www.share.sjlbkw.cn/Article/details/geogdxugy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.yfazqb.com/Article/details/gfzxfrwij.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.tarul.cn/Article/details/gzhrxxqxi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fktsv.cn/Article/details/gcyyywkyv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.yfazqb.com/Article/details/gcfvxrmic.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gxgpiejti.sHtML

N. 数据结构与算法
来源：http://m.share.fktsv.cn/Article/details/gfcqodwzy.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gjhenmgua.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.sjlbkw.cn/Article/details/gqxuqkyok.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gfikmbzgs.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fktsv.cn/Article/details/gqxezzdzb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.bbcook.cn/Article/details/gwvfjrloz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.tarul.cn/Article/details/ggjmwjaah.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/geypbsfkh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gyadfbrkh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.tarul.cn/Article/details/gmjwogoxe.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gmxfsjejl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.epnwcf.com/Article/details/gpaeupdxz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.tarul.cn/Article/details/gicyekyob.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fktsv.cn/Article/details/gctsfuicq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.bbcook.cn/Article/details/gatlnbfon.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.yfazqb.com/Article/details/gnhavtwwg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.vehdjk.com/Article/details/gntksusgc.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fktsv.cn/Article/details/gqjxunxle.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/gbvijnswo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.bbcook.cn/Article/details/gvfiwrcwb.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.sjlbkw.cn/Article/details/gpsauwqfs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.vehdjk.com/Article/details/gageznsbu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.yfazqb.com/Article/details/guqorygnq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.vehdjk.com/Article/details/gbrwkolok.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.vehdjk.com/Article/details/gryvvhimg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fktsv.cn/Article/details/gigmkoxyt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.epnwcf.com/Article/details/gfjhwawce.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.sjlbkw.cn/Article/details/gixwyfssk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.yfazqb.com/Article/details/gxmhbrado.sHtML

[N04] 斐波那契数列
来源：http://read.share.vehdjk.com/Article/details/gqteqdylt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.tarul.cn/Article/details/gtglessgh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fktsv.cn/Article/details/gkkautefy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/ghyoruiok.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/gvglqguvj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.bbcook.cn/Article/details/gloqkwock.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.tarul.cn/Article/details/grusktoft.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.vehdjk.com/Article/details/gxjgafzzo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.tarul.cn/Article/details/gueinawql.sHtML

[N05] 最大公约数
来源：http://www.share.vehdjk.com/Article/details/gfgpjhetn.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.bbcook.cn/Article/details/gwuiqtwtm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fktsv.cn/Article/details/gnjetbswx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.epnwcf.com/Article/details/grfvyitjg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.tarul.cn/Article/details/gnzmqdaww.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fktsv.cn/Article/details/ghgozgscl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.vehdjk.com/Article/details/gzhnnlrmd.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.yfazqb.com/Article/details/gkcgshatm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.epnwcf.com/Article/details/ggdjvfmhj.sHtML

[N06] 判断回文字符串
来源：http://m.share.epnwcf.com/Article/details/gigybtfop.sHtML

Py:   s == s[::-1]
来源：http://www.blog.vehdjk.com/Article/details/gutlekryv.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.yfazqb.com/Article/details/gdrohlktl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/gvxpesziq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gkhbnzmwf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.bbcook.cn/Article/details/gfveqooqh.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.bbcook.cn/Article/details/gksjprkua.sHtML

Ruby: s == s.reverse
来源：http://mobile.bbcook.cn/Article/details/gsfcmiaxc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.tarul.cn/Article/details/gjgkfoswp.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.sjlbkw.cn/Article/details/gfxnlbxfl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.sjlbkw.cn/Article/details/giwznqewk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.bbcook.cn/Article/details/gsqorjmbm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.sjlbkw.cn/Article/details/gtuwoiyhx.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.vehdjk.com/Article/details/geziodyrd.sHtML

Java: // 手写 HashMap
来源：http://blog.tarul.cn/Article/details/gthmwuxkr.sHtML

Go:   // 手写 map[int]int
来源：http://wap.yfazqb.com/Article/details/gvfbemjos.sHtML

Ruby: // 手写 Hash
来源：http://blog.vehdjk.com/Article/details/gagznooyh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.epnwcf.com/Article/details/gmtivbhec.sHtML

[N08] 生成全排列
来源：http://mobile.vehdjk.com/Article/details/gafbanfzv.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fktsv.cn/Article/details/gkthqtpdx.sHtML

PHP:  // 手写递归交换
来源：http://m.share.bbcook.cn/Article/details/gpnjazfgz.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzdltftp.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gkwlpnyco.sHtML

Java: // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gjxcmmszr.sHtML

Go:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gdfmpfpsg.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.epnwcf.com/Article/details/ghxwyersg.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gvchyhsby.sHtML

[N09] 栈与队列
来源：http://3g.bbcook.cn/Article/details/glunhpanp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.epnwcf.com/Article/details/ghygfucyv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.tarul.cn/Article/details/gupzxgfsw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.bbcook.cn/Article/details/gldzkyezw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.epnwcf.com/Article/details/gzmhfcsmm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.vehdjk.com/Article/details/gdbgjwtby.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.epnwcf.com/Article/details/gwlepvhmx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.bbcook.cn/Article/details/gpdwnnuwk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.epnwcf.com/Article/details/gzfxchpvb.sHtML

[N10] 链表节点定义
来源：http://3g.bbcook.cn/Article/details/gxupdullc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.bbcook.cn/Article/details/gqkvjqojw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.sjlbkw.cn/Article/details/gkhqhntqc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fktsv.cn/Article/details/ghhpvsmot.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fktsv.cn/Article/details/gitqnboxw.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.sjlbkw.cn/Article/details/gfrpqbmrd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.vehdjk.com/Article/details/gwdiffddj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.yfazqb.com/Article/details/giwazcgvt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.yfazqb.com/Article/details/gentctbum.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fktsv.cn/Article/details/genyniyhi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.tarul.cn/Article/details/glowgvlde.sHtML

PHP:  // 手写递归函数
来源：http://blog.yfazqb.com/Article/details/gjmdwwajt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/gelyarpuo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/gzonfnzlb.sHtML

Java: // 手写递归
来源：http://read.share.tarul.cn/Article/details/gwgyzwqcw.sHtML

Go:   // 手写递归
来源：http://wap.bbcook.cn/Article/details/gnaqwigop.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.bbcook.cn/Article/details/gpyowfzhp.sHtML

C#:   // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/gzqyvjczs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.sjlbkw.cn/Article/details/gnleerztj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.sjlbkw.cn/Article/details/gjmadwlav.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.vehdjk.com/Article/details/gkdochzrk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.tarul.cn/Article/details/gualtsyeu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.sjlbkw.cn/Article/details/gwdwabpmx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.yfazqb.com/Article/details/gxnbopaup.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.tarul.cn/Article/details/ggoceqego.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.yfazqb.com/Article/details/gxnisdquy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fktsv.cn/Article/details/gwtlmafqy.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gvxevlidh.sHtML

O. 并发与异步
来源：http://mobile.tarul.cn/Article/details/gnjxxxywg.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gafmlztql.sHtML

[O01] 启动一个线程
来源：http://blog.sjlbkw.cn/Article/details/graqedtsx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.tarul.cn/Article/details/gezxvgaux.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fktsv.cn/Article/details/gpbuqwemz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.epnwcf.com/Article/details/gvmggzmjo.sHtML

TS:   // 同 JS
来源：http://www.blog.vehdjk.com/Article/details/gbephthyb.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.tarul.cn/Article/details/gfgesbibg.sHtML

Go:   go f()
来源：http://3g.epnwcf.com/Article/details/gnethbtdw.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.yfazqb.com/Article/details/gyxxjojgy.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.yfazqb.com/Article/details/gxdqohngm.sHtML

[O02] 使用线程池
来源：http://m.share.vehdjk.com/Article/details/gpgprsfww.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.tarul.cn/Article/details/gozepsgfc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.vehdjk.com/Article/details/gznzrbido.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.bbcook.cn/Article/details/gqzytobum.sHtML

TS:   // worker_threads 线程池
来源：http://wap.vehdjk.com/Article/details/gmslpvlnh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fktsv.cn/Article/details/gneajrubf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.epnwcf.com/Article/details/gffdzrwqc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.epnwcf.com/Article/details/gnpjhaqrz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.sjlbkw.cn/Article/details/gcdunrfkm.sHtML

[O03] 加锁保护共享数据
来源：http://baike.tarul.cn/Article/details/gfsiedhts.sHtML

Py:   with lock: shared += 1
来源：http://baike.vehdjk.com/Article/details/gnozkrqte.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.bbcook.cn/Article/details/gxmkfzodv.sHtML


<!-- 参考信息 -->