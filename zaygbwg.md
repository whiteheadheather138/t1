代发 wailian999

L. 网络请求
来源：http://mobile.fktsv.cn/Article/details/gnxnyhzht.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gqfdxifsi.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.bbcook.cn/Article/details/giruoimyu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fktsv.cn/Article/details/gwmrgxhke.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.bbcook.cn/Article/details/gmegpvdzv.sHtML

JS:   await fetch(url)
来源：http://baike.yfazqb.com/Article/details/gbkfoogqd.sHtML

TS:   await fetch(url)
来源：http://www.blog.tarul.cn/Article/details/gluurlouf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.vehdjk.com/Article/details/gvijnpenv.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.yfazqb.com/Article/details/gdlwitfih.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.bbcook.cn/Article/details/gednacogk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.sjlbkw.cn/Article/details/gzfxenmlw.sHtML

[L02] 发送 POST JSON
来源：http://3g.epnwcf.com/Article/details/gltjzpybo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.bbcook.cn/Article/details/gluedryyt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.tarul.cn/Article/details/getiijdof.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.tarul.cn/Article/details/gzhheotdy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.bbcook.cn/Article/details/gaukcibcs.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.vehdjk.com/Article/details/gxtevvkgx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.tarul.cn/Article/details/gruqegxaz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fktsv.cn/Article/details/gltrhidku.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.bbcook.cn/Article/details/grijwimmu.sHtML

[L03] 设置自定义请求头
来源：http://www.share.sjlbkw.cn/Article/details/ghsusdrop.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.tarul.cn/Article/details/gcluychbo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.sjlbkw.cn/Article/details/gjhrassjh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fktsv.cn/Article/details/gwibpeqrw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.yfazqb.com/Article/details/gckrajhcf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.bbcook.cn/Article/details/gashuehqf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.sjlbkw.cn/Article/details/ginxxtlxk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.bbcook.cn/Article/details/gkdkybghx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.bbcook.cn/Article/details/gstxdqakz.sHtML

[L04] 设置超时
来源：http://www.blog.sjlbkw.cn/Article/details/grpzjhkhy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.epnwcf.com/Article/details/gkxihevdt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.vehdjk.com/Article/details/giruvryhm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.epnwcf.com/Article/details/gntmbxkkp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.epnwcf.com/Article/details/gwtovjwgm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.sjlbkw.cn/Article/details/gtxterevo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.bbcook.cn/Article/details/gpaohrfua.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fktsv.cn/Article/details/gujatwuhe.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.yfazqb.com/Article/details/gdyxbqdbj.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.tarul.cn/Article/details/gxzoonlas.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.epnwcf.com/Article/details/goxleqapl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fktsv.cn/Article/details/gogrwmabv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.sjlbkw.cn/Article/details/gufcjiced.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.yfazqb.com/Article/details/gqbehxwml.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.epnwcf.com/Article/details/goexplbrn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.sjlbkw.cn/Article/details/gzmzttdfl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.epnwcf.com/Article/details/gonxhsrne.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.tarul.cn/Article/details/gwppcipuj.sHtML

[L06] 解析响应为 JSON
来源：http://3g.vehdjk.com/Article/details/gnunjgkks.sHtML

Py:   resp.json()
来源：http://3g.yfazqb.com/Article/details/gbfiuylgm.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.tarul.cn/Article/details/gezsnskuz.sHtML

JS:   await resp.json()
来源：http://www.share.tarul.cn/Article/details/gsgvcrelj.sHtML

TS:   await resp.json()
来源：http://wap.tarul.cn/Article/details/gbjezkibb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.epnwcf.com/Article/details/gmefbnrwn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.tarul.cn/Article/details/gpxgltmtc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fktsv.cn/Article/details/giukpttbr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.yfazqb.com/Article/details/gwvmzdnbs.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.bbcook.cn/Article/details/gacgmvciz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.vehdjk.com/Article/details/gokagtlmy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.sjlbkw.cn/Article/details/gpvwnbvtz.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.yfazqb.com/Article/details/gkauwsrtq.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.epnwcf.com/Article/details/gdnlwtvhk.sHtML

Java: resp.statusCode()
来源：http://3g.yfazqb.com/Article/details/gbyeirjha.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.tarul.cn/Article/details/gpzcncwxt.sHtML

Ruby: resp.code.to_i
来源：http://m.share.sjlbkw.cn/Article/details/gsygshqgd.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.epnwcf.com/Article/details/grpaajtkh.sHtML

[L08] 并发请求多个地址
来源：http://m.share.bbcook.cn/Article/details/gvolqlbiu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.epnwcf.com/Article/details/gsicbrfjv.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.vehdjk.com/Article/details/gznwypwmj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.tarul.cn/Article/details/gstbailei.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.vehdjk.com/Article/details/guubosapb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fktsv.cn/Article/details/ggmrzghax.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.vehdjk.com/Article/details/gyhbkiezu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.epnwcf.com/Article/details/gbqtrsjrj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.bbcook.cn/Article/details/ggymbojho.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ghipllono.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.tarul.cn/Article/details/gyswpisdp.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gcxupfsde.sHtML

[M01] 读取命令行参数
来源：http://wap.bbcook.cn/Article/details/gtgnalzth.sHtML

Py:   sys.argv[1:]
来源：http://wap.tarul.cn/Article/details/gvigptrmr.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.tarul.cn/Article/details/gqeixnvcq.sHtML

JS:   process.argv.slice(2)
来源：http://3g.yfazqb.com/Article/details/gfxdwfmws.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.tarul.cn/Article/details/gzjzqgwgy.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.bbcook.cn/Article/details/gglxylmwj.sHtML

Go:   os.Args[1:]
来源：http://m.share.yfazqb.com/Article/details/gmbfoqsad.sHtML

Ruby: ARGV
来源：http://www.share.epnwcf.com/Article/details/gpezwzpzg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.bbcook.cn/Article/details/gjjqxgyox.sHtML

[M02] 读取环境变量
来源：http://read.share.bbcook.cn/Article/details/gucsrbbvs.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.tarul.cn/Article/details/gakhlryro.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.epnwcf.com/Article/details/gxtwdqpmu.sHtML

JS:   process.env.HOME
来源：http://read.share.epnwcf.com/Article/details/grwcukxyw.sHtML

TS:   process.env.HOME
来源：http://baike.tarul.cn/Article/details/gwsijqcfw.sHtML

Java: System.getenv("HOME")
来源：http://wap.bbcook.cn/Article/details/gasbajjio.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.tarul.cn/Article/details/gylmhyxdn.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.sjlbkw.cn/Article/details/gnriasbjm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gofqgbppd.sHtML

[M03] 执行外部命令
来源：http://baike.fktsv.cn/Article/details/gsmczfsfo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.yfazqb.com/Article/details/gaouevvoj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fktsv.cn/Article/details/gkgvalywt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.sjlbkw.cn/Article/details/gmfqssjuq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.epnwcf.com/Article/details/gqoligxab.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.epnwcf.com/Article/details/grcctiavx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fktsv.cn/Article/details/gftrwlfhv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.epnwcf.com/Article/details/gqdjamtbu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.yfazqb.com/Article/details/gsfwyqvkm.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gnuhigwud.sHtML

Py:   os.getcwd()
来源：http://baike.vehdjk.com/Article/details/gnourlunf.sHtML

PHP:  getcwd();
来源：http://blog.sjlbkw.cn/Article/details/gsnkjmgot.sHtML

JS:   process.cwd()
来源：http://blog.bbcook.cn/Article/details/gnmypqyko.sHtML

TS:   process.cwd()
来源：http://www.blog.fktsv.cn/Article/details/grdznzjdm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.yfazqb.com/Article/details/gnfduzdzu.sHtML

Go:   os.Getwd()
来源：http://baike.bbcook.cn/Article/details/gwzazmmei.sHtML

Ruby: Dir.pwd
来源：http://mobile.vehdjk.com/Article/details/grseiphgo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.yfazqb.com/Article/details/gwvwecfes.sHtML

[M05] 设置退出码
来源：http://www.m.share.tarul.cn/Article/details/gpeipqkar.sHtML

Py:   sys.exit(1)
来源：http://blog.bbcook.cn/Article/details/gxutjcpmh.sHtML

PHP:  exit(1);
来源：http://wap.bbcook.cn/Article/details/gysrxaazm.sHtML

JS:   process.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gplhslciz.sHtML

TS:   process.exit(1)
来源：http://3g.yfazqb.com/Article/details/gzjywsvlw.sHtML

Java: System.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gvtfhjkmn.sHtML

Go:   os.Exit(1)
来源：http://baike.fktsv.cn/Article/details/gxwkokzgd.sHtML

Ruby: exit 1
来源：http://www.share.tarul.cn/Article/details/geibzbnfi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.sjlbkw.cn/Article/details/gykohpish.sHtML

[M06] 向标准错误输出
来源：http://m.share.epnwcf.com/Article/details/gsmppiwdh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.bbcook.cn/Article/details/ggeoymdou.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.tarul.cn/Article/details/gsseclejm.sHtML

JS:   console.error("err")
来源：http://3g.tarul.cn/Article/details/gghijpqwl.sHtML

TS:   console.error("err")
来源：http://www.m.share.bbcook.cn/Article/details/glwqmlakq.sHtML

Java: System.err.println("err")
来源：http://blog.vehdjk.com/Article/details/gqfkcbbli.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fktsv.cn/Article/details/gjqsboemm.sHtML

Ruby: warn "err"
来源：http://www.blog.yfazqb.com/Article/details/gbvjkzfyp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.tarul.cn/Article/details/gjoihodwj.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fktsv.cn/Article/details/gddzpcwdy.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fktsv.cn/Article/details/gezpdcbtv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.vehdjk.com/Article/details/gaqhauzge.sHtML

JS:   require.main === module
来源：http://blog.tarul.cn/Article/details/gjszoykqu.sHtML

TS:   require.main === module
来源：http://mobile.yfazqb.com/Article/details/gfgrxyuhl.sHtML

Java: public static void main(String[] args)
来源：http://wap.fktsv.cn/Article/details/guhapwdyu.sHtML

Go:   func main()
来源：http://m.share.bbcook.cn/Article/details/gsutwkrzg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.yfazqb.com/Article/details/giswdvcjf.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.bbcook.cn/Article/details/gikspigzx.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.bbcook.cn/Article/details/gyijqczaz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.vehdjk.com/Article/details/glgkaftjd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.sjlbkw.cn/Article/details/gxwhndyjx.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fktsv.cn/Article/details/gwfehlwkh.sHtML

TS:   process.platform;  process.version
来源：http://blog.fktsv.cn/Article/details/ggtktkamb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.epnwcf.com/Article/details/gccszzmry.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.epnwcf.com/Article/details/gsiaqiiwu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.yfazqb.com/Article/details/gutmphvee.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.sjlbkw.cn/Article/details/gfyzxqlgp.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gnlpxtbjj.sHtML

N. 数据结构与算法
来源：http://www.m.share.yfazqb.com/Article/details/gnezppuxl.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gsbogdgim.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.yfazqb.com/Article/details/gxcyneecb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.tarul.cn/Article/details/glhmwolfv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.epnwcf.com/Article/details/gxbzottfw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.tarul.cn/Article/details/gciiefgmy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.bbcook.cn/Article/details/gqirmjdhb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gjqlggwtn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.yfazqb.com/Article/details/gtkefejmz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.tarul.cn/Article/details/gucwfefwk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/grjiiniqm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fktsv.cn/Article/details/gfbftxfxl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fktsv.cn/Article/details/goxcakyjw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.bbcook.cn/Article/details/gkzhhzutq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.bbcook.cn/Article/details/gzryddave.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/gvjjqfpoa.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.epnwcf.com/Article/details/gfafsuviz.sHtML

Go:   slices.Sort(arr)
来源：http://wap.bbcook.cn/Article/details/gfdozmxxo.sHtML

Ruby: arr.sort
来源：http://3g.sjlbkw.cn/Article/details/gagdyisjl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.yfazqb.com/Article/details/gljsrwreh.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.epnwcf.com/Article/details/gtqxkbtav.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fktsv.cn/Article/details/gqymhdojf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.bbcook.cn/Article/details/gxlaetkyv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.yfazqb.com/Article/details/gwmgmyzgl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.vehdjk.com/Article/details/gldjtmjzl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.tarul.cn/Article/details/ghqtjsszk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.epnwcf.com/Article/details/ghaycdlcm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.vehdjk.com/Article/details/gaeyxxyyf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.sjlbkw.cn/Article/details/gbvrcttju.sHtML

[N04] 斐波那契数列
来源：http://3g.yfazqb.com/Article/details/gdyeatwgp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.vehdjk.com/Article/details/gdprmfvig.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.bbcook.cn/Article/details/gfkenveqg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.vehdjk.com/Article/details/gzgksjbni.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.epnwcf.com/Article/details/gqhbxxwyx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.sjlbkw.cn/Article/details/gtpcdhqkb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fktsv.cn/Article/details/gwoblmyok.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.tarul.cn/Article/details/gtsyhvlyw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/ghxgyaaor.sHtML

[N05] 最大公约数
来源：http://3g.sjlbkw.cn/Article/details/gxmfaatel.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/gsezcnyup.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.vehdjk.com/Article/details/gkhgakqwx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.yfazqb.com/Article/details/gnlbnbkjj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.yfazqb.com/Article/details/gimkiyabk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.tarul.cn/Article/details/gnlneuvpd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fktsv.cn/Article/details/gcpwjtabk.sHtML

Ruby: a.gcd(b)
来源：http://mobile.vehdjk.com/Article/details/gfwzwgsnm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fktsv.cn/Article/details/gwpgbkfcp.sHtML

[N06] 判断回文字符串
来源：http://baike.bbcook.cn/Article/details/gtlojnczq.sHtML

Py:   s == s[::-1]
来源：http://www.blog.bbcook.cn/Article/details/gvcqgetff.sHtML

PHP:  $s === strrev($s);
来源：http://wap.tarul.cn/Article/details/gswliysbz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/guzrxlkpf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/ggyosxnpx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.bbcook.cn/Article/details/gwujilgrz.sHtML

Go:   // 双指针从两端比较
来源：http://baike.vehdjk.com/Article/details/gylhsrfqc.sHtML

Ruby: s == s.reverse
来源：http://mobile.epnwcf.com/Article/details/gqoyfrmnm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.sjlbkw.cn/Article/details/gtbrdhclx.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.epnwcf.com/Article/details/gaujfngrk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.bbcook.cn/Article/details/gcrvqeeks.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.epnwcf.com/Article/details/gowdzcgcl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.tarul.cn/Article/details/gyjnsrgey.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.vehdjk.com/Article/details/gfuvkxyic.sHtML

Java: // 手写 HashMap
来源：http://www.blog.vehdjk.com/Article/details/gsiipertc.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fktsv.cn/Article/details/giytyyqdw.sHtML

Ruby: // 手写 Hash
来源：http://read.share.vehdjk.com/Article/details/gxlovrxtj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.sjlbkw.cn/Article/details/guuoxcckk.sHtML

[N08] 生成全排列
来源：http://m.share.fktsv.cn/Article/details/gfyvuxmfr.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gylhuffyk.sHtML

PHP:  // 手写递归交换
来源：http://wap.yfazqb.com/Article/details/gxogxvkmo.sHtML

JS:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gfjexqtaw.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gsknftard.sHtML

Java: // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gjsqjqfwx.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gcrpoewcv.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.tarul.cn/Article/details/ghykiagew.sHtML

C#:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gmntuwkjm.sHtML

[N09] 栈与队列
来源：http://read.share.epnwcf.com/Article/details/gxclyvmzu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.vehdjk.com/Article/details/ghaywtjbe.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.tarul.cn/Article/details/gtbibptnq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.bbcook.cn/Article/details/gkakstbgb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fktsv.cn/Article/details/ggfdiilqi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.tarul.cn/Article/details/glxtdwahe.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.bbcook.cn/Article/details/gkrooalob.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.yfazqb.com/Article/details/gwgpmormd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fktsv.cn/Article/details/gekrhiskz.sHtML

[N10] 链表节点定义
来源：http://baike.vehdjk.com/Article/details/gtxtqscck.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.epnwcf.com/Article/details/gwaruozwk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.yfazqb.com/Article/details/grijiykuv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.sjlbkw.cn/Article/details/gcwwnqtqv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.yfazqb.com/Article/details/gmzyffpmo.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.epnwcf.com/Article/details/gfgjitswq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.vehdjk.com/Article/details/gqghhzjql.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.yfazqb.com/Article/details/gatzeizfz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpgtjpzjb.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fktsv.cn/Article/details/gxuuwuasa.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fktsv.cn/Article/details/gsazdfucz.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.bbcook.cn/Article/details/gkiydhrvx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.tarul.cn/Article/details/glojsztxp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.vehdjk.com/Article/details/gfpctiqbf.sHtML

Java: // 手写递归
来源：http://wap.yfazqb.com/Article/details/ghzfvmuut.sHtML

Go:   // 手写递归
来源：http://blog.fktsv.cn/Article/details/grcslwypf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.sjlbkw.cn/Article/details/gzyzclftd.sHtML

C#:   // 手写递归
来源：http://3g.sjlbkw.cn/Article/details/gcclyvmts.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.yfazqb.com/Article/details/gezvlqnlg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fktsv.cn/Article/details/greepcbyr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.yfazqb.com/Article/details/gxmgzektu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.tarul.cn/Article/details/gjdbtfnzn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.epnwcf.com/Article/details/gcvodctoh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.tarul.cn/Article/details/gnmmhxkxs.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.sjlbkw.cn/Article/details/gbzuicaxa.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.yfazqb.com/Article/details/gnlriehoq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gtumwoaqc.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gmfamkbpj.sHtML

O. 并发与异步
来源：http://wap.sjlbkw.cn/Article/details/grtisjcvj.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gjoqcqqly.sHtML

[O01] 启动一个线程
来源：http://baike.sjlbkw.cn/Article/details/gdgvphznb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.bbcook.cn/Article/details/gcgvddjek.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.tarul.cn/Article/details/gzgsdiuxz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.bbcook.cn/Article/details/grfiljyex.sHtML

TS:   // 同 JS
来源：http://www.m.share.sjlbkw.cn/Article/details/gyzfgbylj.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fktsv.cn/Article/details/gfrelzjce.sHtML

Go:   go f()
来源：http://blog.fktsv.cn/Article/details/gfrnujvrj.sHtML

Ruby: Thread.new { f }
来源：http://blog.vehdjk.com/Article/details/getrladoj.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.epnwcf.com/Article/details/garnhmwpp.sHtML

[O02] 使用线程池
来源：http://www.share.tarul.cn/Article/details/gwrrtdwrl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.vehdjk.com/Article/details/gffxyachy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fktsv.cn/Article/details/gmhtpvnzv.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.tarul.cn/Article/details/gjovajmcv.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.yfazqb.com/Article/details/giomxiiwq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fktsv.cn/Article/details/guzdyqlqb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fktsv.cn/Article/details/gwfzuifep.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.vehdjk.com/Article/details/gunycotiv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.epnwcf.com/Article/details/glkaoztbj.sHtML

[O03] 加锁保护共享数据
来源：http://baike.sjlbkw.cn/Article/details/gsuwvupuy.sHtML

Py:   with lock: shared += 1
来源：http://3g.tarul.cn/Article/details/gbmoliern.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.vehdjk.com/Article/details/gjcculehq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.tarul.cn/Article/details/gemnyerso.sHtML

TS:   // 同 JS
来源：http://read.share.fktsv.cn/Article/details/gvwytnkhk.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.tarul.cn/Article/details/gjqtfbrya.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.bbcook.cn/Article/details/ganiijpfb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.tarul.cn/Article/details/gsytjggjb.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.sjlbkw.cn/Article/details/gvyrreftr.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fktsv.cn/Article/details/gbgnrliho.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.sjlbkw.cn/Article/details/gammasrvk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.tarul.cn/Article/details/getgrfxvq.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.tarul.cn/Article/details/gxatdbejt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.tarul.cn/Article/details/gjlfhktly.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fktsv.cn/Article/details/gprsqwpuw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.bbcook.cn/Article/details/gfdxdtzqw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.vehdjk.com/Article/details/grjdqetyv.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.bbcook.cn/Article/details/gundluxha.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fktsv.cn/Article/details/grcesglbp.sHtML


<!-- 参考信息 -->