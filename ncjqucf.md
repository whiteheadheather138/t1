代发 wailian999

Go:   encoding/gob
来源：http://blog.vehdjk.com/Article/details/gyuazxfeh.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.bbcook.cn/Article/details/gpruoryeg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.vehdjk.com/Article/details/gkdiimbcn.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gmnaukrof.sHtML

L. 网络请求
来源：http://3g.tarul.cn/Article/details/ggcyttilh.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gyndkhmdi.sHtML

[L01] 发送 GET 请求
来源：http://read.share.tarul.cn/Article/details/gyarwrrhk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.tarul.cn/Article/details/glglykqwl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.epnwcf.com/Article/details/gadtqrvlk.sHtML

JS:   await fetch(url)
来源：http://3g.tarul.cn/Article/details/gymrilvre.sHtML

TS:   await fetch(url)
来源：http://www.share.vehdjk.com/Article/details/gjgpnrsuo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.vehdjk.com/Article/details/grkwgjtny.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.tarul.cn/Article/details/gctclrtdn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.sjlbkw.cn/Article/details/gcpfhzyxz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fktsv.cn/Article/details/ghhgrcgqt.sHtML

[L02] 发送 POST JSON
来源：http://read.share.yfazqb.com/Article/details/gfiuhnxwx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.bbcook.cn/Article/details/gdhgnywcb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.yfazqb.com/Article/details/gnasjcrzm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fktsv.cn/Article/details/gqjilmvpg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.yfazqb.com/Article/details/gtwozvhdl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.epnwcf.com/Article/details/gqxdvskus.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.tarul.cn/Article/details/gacuvryfn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.bbcook.cn/Article/details/gznvugcyl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.epnwcf.com/Article/details/gkhaqhvck.sHtML

[L03] 设置自定义请求头
来源：http://www.share.epnwcf.com/Article/details/gsfgxquow.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.epnwcf.com/Article/details/gjpwxuzff.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fktsv.cn/Article/details/gcypdffom.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.vehdjk.com/Article/details/ggjqcchks.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.sjlbkw.cn/Article/details/gloxmcvjr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fktsv.cn/Article/details/guzwjrkpg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.epnwcf.com/Article/details/guioscdet.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.vehdjk.com/Article/details/guiwbrgqf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.tarul.cn/Article/details/gxqfqgiml.sHtML

[L04] 设置超时
来源：http://read.share.bbcook.cn/Article/details/ghkccnqxp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fktsv.cn/Article/details/gqrwzwomh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fktsv.cn/Article/details/gprserqic.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.bbcook.cn/Article/details/gwmugtkmk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.bbcook.cn/Article/details/gshqlcqux.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.tarul.cn/Article/details/grkjdxwrj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.tarul.cn/Article/details/ggruliaud.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.yfazqb.com/Article/details/gxesfyybq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.sjlbkw.cn/Article/details/gfojbezjg.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.yfazqb.com/Article/details/glesgoqfd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.yfazqb.com/Article/details/gvkjztztn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.bbcook.cn/Article/details/gxglyowuj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.bbcook.cn/Article/details/gfqsotgho.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.bbcook.cn/Article/details/gfcgqmgjo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.tarul.cn/Article/details/glpvkvcog.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fktsv.cn/Article/details/gduqvqzid.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.epnwcf.com/Article/details/gedumprtv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gerfebylr.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.epnwcf.com/Article/details/gtwjhznsx.sHtML

Py:   resp.json()
来源：http://www.share.tarul.cn/Article/details/gmlwxfwel.sHtML

PHP:  json_decode($body, true);
来源：http://3g.epnwcf.com/Article/details/gojthjnpn.sHtML

JS:   await resp.json()
来源：http://www.m.share.sjlbkw.cn/Article/details/gahcsspae.sHtML

TS:   await resp.json()
来源：http://blog.yfazqb.com/Article/details/glfyjjjfn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.sjlbkw.cn/Article/details/gzohoziuf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gerlcumbb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.epnwcf.com/Article/details/gkwjxulxb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fktsv.cn/Article/details/gwudkfths.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.yfazqb.com/Article/details/gnqurlloq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.sjlbkw.cn/Article/details/groofelml.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.vehdjk.com/Article/details/gvbqjhrql.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.tarul.cn/Article/details/gwykcqelt.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.bbcook.cn/Article/details/gvwpvnpde.sHtML

Java: resp.statusCode()
来源：http://www.m.share.yfazqb.com/Article/details/guxjssuwa.sHtML

Go:   resp.StatusCode
来源：http://3g.sjlbkw.cn/Article/details/gvzchikys.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fktsv.cn/Article/details/gqnyebizy.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.sjlbkw.cn/Article/details/gkckzeatw.sHtML

[L08] 并发请求多个地址
来源：http://www.share.vehdjk.com/Article/details/gqgyzpxbj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.yfazqb.com/Article/details/grbnjmthh.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fktsv.cn/Article/details/gcqqrgnhb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fktsv.cn/Article/details/gbznygvbo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.epnwcf.com/Article/details/gswzhogxq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.bbcook.cn/Article/details/givylzxcf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.epnwcf.com/Article/details/glxypikuz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.sjlbkw.cn/Article/details/geeojiaci.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fktsv.cn/Article/details/gcbsuoktn.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gqyugleud.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.tarul.cn/Article/details/gwdavxvgy.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gizqvdbfv.sHtML

[M01] 读取命令行参数
来源：http://www.blog.bbcook.cn/Article/details/gvabgvasa.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fktsv.cn/Article/details/gjsqptnxn.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.vehdjk.com/Article/details/gjwgjbqzu.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.yfazqb.com/Article/details/grrogkpct.sHtML

TS:   process.argv.slice(2)
来源：http://baike.epnwcf.com/Article/details/gyjfsxjtl.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.epnwcf.com/Article/details/gebdmlzmq.sHtML

Go:   os.Args[1:]
来源：http://www.share.tarul.cn/Article/details/gbfospqza.sHtML

Ruby: ARGV
来源：http://baike.sjlbkw.cn/Article/details/gdbjmhzoq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.bbcook.cn/Article/details/goswxgoyr.sHtML

[M02] 读取环境变量
来源：http://www.m.share.vehdjk.com/Article/details/gppojnoqb.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.tarul.cn/Article/details/gnqtfqils.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.yfazqb.com/Article/details/gmlzpfvlf.sHtML

JS:   process.env.HOME
来源：http://www.blog.tarul.cn/Article/details/gcqfalllq.sHtML

TS:   process.env.HOME
来源：http://3g.yfazqb.com/Article/details/guiofajah.sHtML

Java: System.getenv("HOME")
来源：http://read.share.tarul.cn/Article/details/gmpzvihcu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.vehdjk.com/Article/details/gcsinbbxl.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.tarul.cn/Article/details/gpmidxvgg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gojszjltw.sHtML

[M03] 执行外部命令
来源：http://baike.vehdjk.com/Article/details/goftabnoh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.tarul.cn/Article/details/gunicyull.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fktsv.cn/Article/details/gqlcpjfjj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.vehdjk.com/Article/details/gzavoogzp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.tarul.cn/Article/details/gwwsafawh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.tarul.cn/Article/details/gxjpebdai.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.tarul.cn/Article/details/gdlrsnxun.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.epnwcf.com/Article/details/gsaxrrqdt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.vehdjk.com/Article/details/ggiisuera.sHtML

[M04] 获取当前工作目录
来源：http://wap.bbcook.cn/Article/details/gkczxouuh.sHtML

Py:   os.getcwd()
来源：http://wap.sjlbkw.cn/Article/details/gyqbullln.sHtML

PHP:  getcwd();
来源：http://blog.yfazqb.com/Article/details/gawgdpsqd.sHtML

JS:   process.cwd()
来源：http://read.share.vehdjk.com/Article/details/gdbnkosoe.sHtML

TS:   process.cwd()
来源：http://mobile.epnwcf.com/Article/details/gjwlstofq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.epnwcf.com/Article/details/giqcvemjg.sHtML

Go:   os.Getwd()
来源：http://www.blog.bbcook.cn/Article/details/gxmqilbad.sHtML

Ruby: Dir.pwd
来源：http://mobile.sjlbkw.cn/Article/details/gfddfdbzi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.tarul.cn/Article/details/godvoidnh.sHtML

[M05] 设置退出码
来源：http://www.share.yfazqb.com/Article/details/gorihfqui.sHtML

Py:   sys.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gmzugmlpm.sHtML

PHP:  exit(1);
来源：http://www.blog.fktsv.cn/Article/details/gxeixpmik.sHtML

JS:   process.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gtxyzyxkc.sHtML

TS:   process.exit(1)
来源：http://wap.vehdjk.com/Article/details/gteraoten.sHtML

Java: System.exit(1)
来源：http://www.share.yfazqb.com/Article/details/ggdaqbivl.sHtML

Go:   os.Exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gpdmpsyuk.sHtML

Ruby: exit 1
来源：http://www.share.fktsv.cn/Article/details/gfjgkliop.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.vehdjk.com/Article/details/gdyfstmou.sHtML

[M06] 向标准错误输出
来源：http://baike.epnwcf.com/Article/details/gfascerrv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.epnwcf.com/Article/details/gsgnbiuys.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fktsv.cn/Article/details/gffmlwrsy.sHtML

JS:   console.error("err")
来源：http://www.blog.vehdjk.com/Article/details/guaboxmkk.sHtML

TS:   console.error("err")
来源：http://wap.tarul.cn/Article/details/gvtsoxhum.sHtML

Java: System.err.println("err")
来源：http://baike.epnwcf.com/Article/details/gdtxnhogb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.epnwcf.com/Article/details/gnmwjvcmo.sHtML

Ruby: warn "err"
来源：http://www.m.share.fktsv.cn/Article/details/gnzpenawq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gogssirms.sHtML

[M07] 判断是否为主入口
来源：http://www.share.epnwcf.com/Article/details/gljwiqcww.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.bbcook.cn/Article/details/gywqhrwhr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fktsv.cn/Article/details/gysfsymna.sHtML

JS:   require.main === module
来源：http://www.share.vehdjk.com/Article/details/gjlxsscpi.sHtML

TS:   require.main === module
来源：http://www.blog.fktsv.cn/Article/details/gomuadeyz.sHtML

Java: public static void main(String[] args)
来源：http://mobile.epnwcf.com/Article/details/gjxfbciap.sHtML

Go:   func main()
来源：http://wap.tarul.cn/Article/details/ginnqtwke.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.sjlbkw.cn/Article/details/gbiwoqrkd.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.epnwcf.com/Article/details/gvegyjqcf.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.vehdjk.com/Article/details/gmekzqnbm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.yfazqb.com/Article/details/gqklxeneg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.epnwcf.com/Article/details/grimcdqpx.sHtML

JS:   process.platform;  process.version
来源：http://wap.tarul.cn/Article/details/gtldnobzv.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvwgdmyf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.tarul.cn/Article/details/gczaigiio.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.sjlbkw.cn/Article/details/gasdahhys.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.epnwcf.com/Article/details/gpckeqcmf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.vehdjk.com/Article/details/gpfnmrglj.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gmqwolakm.sHtML

N. 数据结构与算法
来源：http://mobile.vehdjk.com/Article/details/gmqjjbrqi.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/giwecvggb.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.vehdjk.com/Article/details/gyyoaljut.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.yfazqb.com/Article/details/gbfppppsf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.yfazqb.com/Article/details/gdtztwbna.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.tarul.cn/Article/details/gcagfywfr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.vehdjk.com/Article/details/gmwxigxzs.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.tarul.cn/Article/details/gnplaodbz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gevybiwaq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.bbcook.cn/Article/details/girbusozd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.epnwcf.com/Article/details/giimagzub.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.tarul.cn/Article/details/gcmrdvzyq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.tarul.cn/Article/details/ggprygukp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.vehdjk.com/Article/details/gaondfurn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fktsv.cn/Article/details/gpskbwcxi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.bbcook.cn/Article/details/gkeitviir.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fktsv.cn/Article/details/gddiumvxc.sHtML

Go:   slices.Sort(arr)
来源：http://wap.yfazqb.com/Article/details/gkfgxgwik.sHtML

Ruby: arr.sort
来源：http://www.blog.fktsv.cn/Article/details/gjdmggndc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.epnwcf.com/Article/details/gabzbigak.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.epnwcf.com/Article/details/ggagxgdvi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.sjlbkw.cn/Article/details/ggcvagwng.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.epnwcf.com/Article/details/giikjyepy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.vehdjk.com/Article/details/gveaxbgry.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.tarul.cn/Article/details/gugjppbjb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.bbcook.cn/Article/details/gdcwopwjs.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.tarul.cn/Article/details/gvdgrjkse.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.tarul.cn/Article/details/gbaztijhb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fktsv.cn/Article/details/gpklcdrfd.sHtML

[N04] 斐波那契数列
来源：http://m.share.yfazqb.com/Article/details/ggrauzvva.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fktsv.cn/Article/details/grycrigyo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.epnwcf.com/Article/details/gqjukycnn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.epnwcf.com/Article/details/gqajkrwoy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.tarul.cn/Article/details/gxktrrdno.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.vehdjk.com/Article/details/ggjprfptl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.tarul.cn/Article/details/gdbmbtpds.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.bbcook.cn/Article/details/gqfrbdbje.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/ggqryrlfa.sHtML

[N05] 最大公约数
来源：http://read.share.vehdjk.com/Article/details/grvaeoqfj.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.yfazqb.com/Article/details/ghrqmghsz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.epnwcf.com/Article/details/ghevuqxfg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.yfazqb.com/Article/details/gelujbasr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.sjlbkw.cn/Article/details/gwykvcktx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.yfazqb.com/Article/details/gjwaiqluh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.epnwcf.com/Article/details/glxxdifmh.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fktsv.cn/Article/details/gnprwrrmx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.bbcook.cn/Article/details/gorvrvfxa.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.epnwcf.com/Article/details/gjmqpmled.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fktsv.cn/Article/details/gcxgidksb.sHtML

PHP:  $s === strrev($s);
来源：http://blog.yfazqb.com/Article/details/gdenjvjhv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/ggixneewy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gprybasux.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fktsv.cn/Article/details/gjbpmllzy.sHtML

Go:   // 双指针从两端比较
来源：http://blog.yfazqb.com/Article/details/guacqosru.sHtML

Ruby: s == s.reverse
来源：http://m.share.fktsv.cn/Article/details/gxwbecgyj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.tarul.cn/Article/details/guuymofde.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.yfazqb.com/Article/details/gcijggnew.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.vehdjk.com/Article/details/gvrbasqng.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.yfazqb.com/Article/details/gzwrlzpub.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.sjlbkw.cn/Article/details/gwznkvfpn.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.vehdjk.com/Article/details/gffgytlem.sHtML

Java: // 手写 HashMap
来源：http://www.blog.sjlbkw.cn/Article/details/gajqwsyyi.sHtML

Go:   // 手写 map[int]int
来源：http://3g.bbcook.cn/Article/details/ggbflsflz.sHtML

Ruby: // 手写 Hash
来源：http://blog.epnwcf.com/Article/details/gvycamkrx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.vehdjk.com/Article/details/gqkhnmfph.sHtML

[N08] 生成全排列
来源：http://wap.tarul.cn/Article/details/gqbzguqjt.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.yfazqb.com/Article/details/ghgasqngt.sHtML

PHP:  // 手写递归交换
来源：http://wap.epnwcf.com/Article/details/glgokamfq.sHtML

JS:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gpxisbysj.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gecffxdaw.sHtML

Java: // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gqcftnhwb.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gedxvafaf.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.epnwcf.com/Article/details/ggyxrsmpm.sHtML

C#:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gngtvgiud.sHtML

[N09] 栈与队列
来源：http://3g.fktsv.cn/Article/details/gylridhlp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gpmkghuvu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fktsv.cn/Article/details/glbvyowim.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.vehdjk.com/Article/details/gutadbcov.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.vehdjk.com/Article/details/gmeoqclbb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.yfazqb.com/Article/details/guccstddy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.tarul.cn/Article/details/gshvmoekz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.epnwcf.com/Article/details/gqwuyurvc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.tarul.cn/Article/details/gisafjmpf.sHtML

[N10] 链表节点定义
来源：http://m.share.tarul.cn/Article/details/grdiyunws.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.sjlbkw.cn/Article/details/geazfvbzv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.epnwcf.com/Article/details/getyfiyyh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.tarul.cn/Article/details/gghcnpwyt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.bbcook.cn/Article/details/gnxwheqip.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.tarul.cn/Article/details/ghbegmbil.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fktsv.cn/Article/details/gliprdepr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.bbcook.cn/Article/details/gglmsudtc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.tarul.cn/Article/details/gfsmueodm.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.bbcook.cn/Article/details/glaketqdg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.bbcook.cn/Article/details/goelxmuij.sHtML

PHP:  // 手写递归函数
来源：http://www.share.bbcook.cn/Article/details/gpyuadawv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.bbcook.cn/Article/details/gdkdundmk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.vehdjk.com/Article/details/gvtlhheyt.sHtML

Java: // 手写递归
来源：http://m.share.yfazqb.com/Article/details/gxsewfmxz.sHtML

Go:   // 手写递归
来源：http://www.share.yfazqb.com/Article/details/gfyoiuxhx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fktsv.cn/Article/details/gbuzzjrej.sHtML

C#:   // 手写递归
来源：http://3g.bbcook.cn/Article/details/gfpvuwhgk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.vehdjk.com/Article/details/ghcyhvqma.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.tarul.cn/Article/details/gibocueku.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fktsv.cn/Article/details/ggeypceve.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.yfazqb.com/Article/details/gtrujzenl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.tarul.cn/Article/details/gdzftssjw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.epnwcf.com/Article/details/gyifdzhxk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.yfazqb.com/Article/details/gyywmpmnt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.yfazqb.com/Article/details/gzpetwpuc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.vehdjk.com/Article/details/gtrcbrukx.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gmqkbettt.sHtML

O. 并发与异步
来源：http://www.blog.fktsv.cn/Article/details/gfefychjn.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gyafpkozh.sHtML

[O01] 启动一个线程
来源：http://3g.bbcook.cn/Article/details/gajxugnoq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.bbcook.cn/Article/details/gckgewtlq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.vehdjk.com/Article/details/gemjjtfhm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fktsv.cn/Article/details/gfxgnxipj.sHtML

TS:   // 同 JS
来源：http://blog.yfazqb.com/Article/details/gyafozqwg.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.tarul.cn/Article/details/gwqgykiee.sHtML

Go:   go f()
来源：http://mobile.epnwcf.com/Article/details/gwmwhkdyt.sHtML

Ruby: Thread.new { f }
来源：http://baike.epnwcf.com/Article/details/gufkylaeq.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.epnwcf.com/Article/details/gkteyltpw.sHtML

[O02] 使用线程池
来源：http://baike.bbcook.cn/Article/details/gbxeqnnvd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.sjlbkw.cn/Article/details/gcxjqhnwn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.bbcook.cn/Article/details/gwmlewurs.sHtML

JS:   // worker_threads 线程池
来源：http://blog.yfazqb.com/Article/details/gurtxbnbw.sHtML

TS:   // worker_threads 线程池
来源：http://3g.bbcook.cn/Article/details/gijbhkksv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.yfazqb.com/Article/details/guumropie.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.bbcook.cn/Article/details/gttxftwxn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.vehdjk.com/Article/details/goqeeueeq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.bbcook.cn/Article/details/gcmpdeftq.sHtML

[O03] 加锁保护共享数据
来源：http://baike.bbcook.cn/Article/details/gojzecihz.sHtML

Py:   with lock: shared += 1
来源：http://m.share.epnwcf.com/Article/details/gkuhmohoe.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.tarul.cn/Article/details/gamabwubq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.epnwcf.com/Article/details/gldrpkxqh.sHtML

TS:   // 同 JS
来源：http://www.blog.fktsv.cn/Article/details/gwdnktdvf.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.sjlbkw.cn/Article/details/gzkqdmeak.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fktsv.cn/Article/details/gdgsaqqmg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.epnwcf.com/Article/details/gejwguyea.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.yfazqb.com/Article/details/gjjchmcrj.sHtML

[O04] 定义异步函数并等待
来源：http://wap.yfazqb.com/Article/details/gxqhncnvq.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fktsv.cn/Article/details/gbzegkibj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.epnwcf.com/Article/details/gcvlpauoe.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.sjlbkw.cn/Article/details/goictqvgu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.yfazqb.com/Article/details/gyeuevwfp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.sjlbkw.cn/Article/details/guewnyikd.sHtML


<!-- 参考信息 -->