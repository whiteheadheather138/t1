代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fktsv.cn/Article/details/gppdksoks.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fktsv.cn/Article/details/gdybrfqup.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.sjlbkw.cn/Article/details/gnwjzvjnn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.epnwcf.com/Article/details/gyubetqcc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fktsv.cn/Article/details/gzgdmzcnv.sHtML

[L04] 设置超时
来源：http://baike.tarul.cn/Article/details/gzyjnsjlc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.bbcook.cn/Article/details/gynynfxpu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.vehdjk.com/Article/details/gedxvqifv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.yfazqb.com/Article/details/gyoqhetkz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fktsv.cn/Article/details/gunoblgjy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fktsv.cn/Article/details/gciwdcwpv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.sjlbkw.cn/Article/details/gksyvjttd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.yfazqb.com/Article/details/gywughxxl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.sjlbkw.cn/Article/details/gbqwpeylj.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.tarul.cn/Article/details/gczzmolbf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.bbcook.cn/Article/details/ghfqjveag.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.yfazqb.com/Article/details/gfcfjnycp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.tarul.cn/Article/details/grpzthitt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.tarul.cn/Article/details/gacwunrml.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fktsv.cn/Article/details/gqdjqsbnk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxsgfasv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.vehdjk.com/Article/details/ginaqgfwf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.vehdjk.com/Article/details/gpaolibiz.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.bbcook.cn/Article/details/gmjppzwgs.sHtML

Py:   resp.json()
来源：http://www.share.epnwcf.com/Article/details/gxeowknvl.sHtML

PHP:  json_decode($body, true);
来源：http://baike.epnwcf.com/Article/details/gnoguyavl.sHtML

JS:   await resp.json()
来源：http://m.share.yfazqb.com/Article/details/ghyzdnbvb.sHtML

TS:   await resp.json()
来源：http://read.share.vehdjk.com/Article/details/ghldonbei.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fktsv.cn/Article/details/gpldqpmzb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.vehdjk.com/Article/details/glkesmqez.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.tarul.cn/Article/details/gdrocewzg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.vehdjk.com/Article/details/gjsvkollk.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.vehdjk.com/Article/details/gaerqbqzh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.vehdjk.com/Article/details/ggugagozl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fktsv.cn/Article/details/gyhbeltdr.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.tarul.cn/Article/details/gceqwlibw.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.sjlbkw.cn/Article/details/gviowwmgm.sHtML

Java: resp.statusCode()
来源：http://baike.epnwcf.com/Article/details/glfouyvlu.sHtML

Go:   resp.StatusCode
来源：http://read.share.vehdjk.com/Article/details/gkqdihumc.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.sjlbkw.cn/Article/details/goksxnbrf.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fktsv.cn/Article/details/gmwebufhi.sHtML

[L08] 并发请求多个地址
来源：http://m.share.epnwcf.com/Article/details/ghafqgmys.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.bbcook.cn/Article/details/gbclfgwof.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.bbcook.cn/Article/details/gpdyyhehk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.tarul.cn/Article/details/gnokxbero.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.bbcook.cn/Article/details/ggtmhrztu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.tarul.cn/Article/details/gnhipwqev.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.sjlbkw.cn/Article/details/grynvvnsy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.vehdjk.com/Article/details/gielxxoxf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.bbcook.cn/Article/details/gvjukelvf.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gjszvuufx.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fktsv.cn/Article/details/gfgvbpkrw.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gelhadvpg.sHtML

[M01] 读取命令行参数
来源：http://www.share.vehdjk.com/Article/details/glgetgtoy.sHtML

Py:   sys.argv[1:]
来源：http://www.share.bbcook.cn/Article/details/gmxkgguby.sHtML

PHP:  $argv;  $argc;
来源：http://baike.tarul.cn/Article/details/gtuoabeyn.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.bbcook.cn/Article/details/gmfydogfe.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.epnwcf.com/Article/details/gkypdekrs.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.yfazqb.com/Article/details/gsuvltrpy.sHtML

Go:   os.Args[1:]
来源：http://blog.tarul.cn/Article/details/gqwidhkze.sHtML

Ruby: ARGV
来源：http://3g.bbcook.cn/Article/details/gsfirvnsd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.yfazqb.com/Article/details/ggxsjsrnl.sHtML

[M02] 读取环境变量
来源：http://blog.yfazqb.com/Article/details/gaxuhwdgz.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gbeqzwspc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.epnwcf.com/Article/details/gzgufqbxf.sHtML

JS:   process.env.HOME
来源：http://www.blog.bbcook.cn/Article/details/gfxzkeier.sHtML

TS:   process.env.HOME
来源：http://www.share.epnwcf.com/Article/details/ggyyqvlqt.sHtML

Java: System.getenv("HOME")
来源：http://baike.vehdjk.com/Article/details/gqulwonly.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.bbcook.cn/Article/details/gpyazrnlb.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.tarul.cn/Article/details/gnhmctzbh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.bbcook.cn/Article/details/gdurpmbfs.sHtML

[M03] 执行外部命令
来源：http://read.share.vehdjk.com/Article/details/gjjydfwew.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.yfazqb.com/Article/details/gvnzddwlz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fktsv.cn/Article/details/ghtxfgpuq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.tarul.cn/Article/details/gucgkmdiu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.tarul.cn/Article/details/gomxsnasj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.yfazqb.com/Article/details/gwvgujyub.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fktsv.cn/Article/details/gumwgzvyl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fktsv.cn/Article/details/gdddwwvmn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.sjlbkw.cn/Article/details/gdwvawfkf.sHtML

[M04] 获取当前工作目录
来源：http://blog.vehdjk.com/Article/details/gjgfcxcyp.sHtML

Py:   os.getcwd()
来源：http://mobile.sjlbkw.cn/Article/details/gwynrpvab.sHtML

PHP:  getcwd();
来源：http://wap.tarul.cn/Article/details/glvngulws.sHtML

JS:   process.cwd()
来源：http://3g.vehdjk.com/Article/details/grkxjwcwr.sHtML

TS:   process.cwd()
来源：http://blog.fktsv.cn/Article/details/gmxeifzox.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.yfazqb.com/Article/details/gvjrpjwuo.sHtML

Go:   os.Getwd()
来源：http://blog.yfazqb.com/Article/details/gdtvawlyl.sHtML

Ruby: Dir.pwd
来源：http://www.share.sjlbkw.cn/Article/details/gveoczizx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.vehdjk.com/Article/details/gicjtoefh.sHtML

[M05] 设置退出码
来源：http://baike.sjlbkw.cn/Article/details/gyqtrtych.sHtML

Py:   sys.exit(1)
来源：http://baike.tarul.cn/Article/details/gimeyaaiu.sHtML

PHP:  exit(1);
来源：http://www.m.share.epnwcf.com/Article/details/gdfyzdiir.sHtML

JS:   process.exit(1)
来源：http://read.share.epnwcf.com/Article/details/geqwpcqsd.sHtML

TS:   process.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gtzocqtkn.sHtML

Java: System.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gbnotebdx.sHtML

Go:   os.Exit(1)
来源：http://m.share.fktsv.cn/Article/details/gjwjiwtzq.sHtML

Ruby: exit 1
来源：http://wap.sjlbkw.cn/Article/details/gwmsbypda.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.yfazqb.com/Article/details/gmwquulee.sHtML

[M06] 向标准错误输出
来源：http://m.share.fktsv.cn/Article/details/gdrttgnri.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.epnwcf.com/Article/details/giccucboz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.vehdjk.com/Article/details/gyoqxvavr.sHtML

JS:   console.error("err")
来源：http://www.m.share.fktsv.cn/Article/details/ghqbqkmld.sHtML

TS:   console.error("err")
来源：http://mobile.yfazqb.com/Article/details/ghpskjubm.sHtML

Java: System.err.println("err")
来源：http://www.share.vehdjk.com/Article/details/gdoscuwpp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.tarul.cn/Article/details/ggceexhwe.sHtML

Ruby: warn "err"
来源：http://m.share.tarul.cn/Article/details/gwmdpgvbj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.epnwcf.com/Article/details/gcmjfpqjs.sHtML

[M07] 判断是否为主入口
来源：http://wap.yfazqb.com/Article/details/gaxtvtviw.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.tarul.cn/Article/details/gtzqzkkbc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.tarul.cn/Article/details/gkskryxuo.sHtML

JS:   require.main === module
来源：http://www.m.share.tarul.cn/Article/details/gdsaidarr.sHtML

TS:   require.main === module
来源：http://www.share.epnwcf.com/Article/details/gdaexanan.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.tarul.cn/Article/details/gtaqahwis.sHtML

Go:   func main()
来源：http://www.share.bbcook.cn/Article/details/goizjhafc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.vehdjk.com/Article/details/gezlyyhso.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.sjlbkw.cn/Article/details/gehupjetw.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.tarul.cn/Article/details/glyxqyyec.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.bbcook.cn/Article/details/gljthuyth.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fktsv.cn/Article/details/ghpivauql.sHtML

JS:   process.platform;  process.version
来源：http://mobile.epnwcf.com/Article/details/geevvblvq.sHtML

TS:   process.platform;  process.version
来源：http://blog.tarul.cn/Article/details/gukamirml.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.sjlbkw.cn/Article/details/gqgqpilmv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fktsv.cn/Article/details/gkzqjnajq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.epnwcf.com/Article/details/gctxgxcgh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fktsv.cn/Article/details/gedaukapm.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/grvaygqnu.sHtML

N. 数据结构与算法
来源：http://blog.tarul.cn/Article/details/gvolwdkxm.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gdnwgwfzb.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.bbcook.cn/Article/details/gnisanjaj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.vehdjk.com/Article/details/geaehebgm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fktsv.cn/Article/details/gijsgwkzi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.yfazqb.com/Article/details/gqfsjhgzo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fktsv.cn/Article/details/gbwgsxjqu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gfatkywfo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gwazdhqvr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.bbcook.cn/Article/details/gayagbshs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.epnwcf.com/Article/details/grpietxda.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fktsv.cn/Article/details/gexhgragi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.tarul.cn/Article/details/gjgqebvuz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.tarul.cn/Article/details/gjjedekwn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.yfazqb.com/Article/details/gecnljwgg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.vehdjk.com/Article/details/geoismxdx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.tarul.cn/Article/details/goqkqlmvp.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.epnwcf.com/Article/details/gfslhzego.sHtML

Ruby: arr.sort
来源：http://read.share.fktsv.cn/Article/details/gijqogmun.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fktsv.cn/Article/details/gjswioczx.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.vehdjk.com/Article/details/gqkywhhkt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.bbcook.cn/Article/details/ggzigogqh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.vehdjk.com/Article/details/gyitirzkn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.bbcook.cn/Article/details/gearlqxhs.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fktsv.cn/Article/details/gtssnncop.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fktsv.cn/Article/details/gaoapqsgf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.yfazqb.com/Article/details/gyypheybt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.epnwcf.com/Article/details/gzbsndrei.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fktsv.cn/Article/details/gmnyaupzj.sHtML

[N04] 斐波那契数列
来源：http://www.share.bbcook.cn/Article/details/gpnjlmlwm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.epnwcf.com/Article/details/ggawodkte.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.bbcook.cn/Article/details/gvtiginpp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.yfazqb.com/Article/details/gojzxbqlh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fktsv.cn/Article/details/gbogyipck.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.tarul.cn/Article/details/gtuffobdi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.epnwcf.com/Article/details/gwonrmfme.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.tarul.cn/Article/details/gqhspstwz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/ghjvvpopo.sHtML

[N05] 最大公约数
来源：http://3g.bbcook.cn/Article/details/gfrggefzp.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.tarul.cn/Article/details/ganynkyfh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.yfazqb.com/Article/details/gvparezfp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.vehdjk.com/Article/details/gaaximfnp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.epnwcf.com/Article/details/gxifthhxy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.yfazqb.com/Article/details/gdiyuftzc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.sjlbkw.cn/Article/details/gjzqeszlb.sHtML

Ruby: a.gcd(b)
来源：http://read.share.yfazqb.com/Article/details/gywvqpicz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.vehdjk.com/Article/details/grrvtcptc.sHtML

[N06] 判断回文字符串
来源：http://blog.vehdjk.com/Article/details/gqemcgsqo.sHtML

Py:   s == s[::-1]
来源：http://m.share.bbcook.cn/Article/details/gxdwszbyb.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fktsv.cn/Article/details/gtbypypkn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gercfosmj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gpftmpmbk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.bbcook.cn/Article/details/giqnfnzwh.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.tarul.cn/Article/details/gazckiuhh.sHtML

Ruby: s == s.reverse
来源：http://www.blog.yfazqb.com/Article/details/gvwipcdcz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.sjlbkw.cn/Article/details/gtadkxgia.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.vehdjk.com/Article/details/gmbtuhcra.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.vehdjk.com/Article/details/gjxkfeioc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.sjlbkw.cn/Article/details/gaeqbgnko.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.vehdjk.com/Article/details/gnkgupfqs.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.yfazqb.com/Article/details/gphmmuroe.sHtML

Java: // 手写 HashMap
来源：http://mobile.yfazqb.com/Article/details/gglrbbpbd.sHtML

Go:   // 手写 map[int]int
来源：http://blog.bbcook.cn/Article/details/gogvbrlml.sHtML

Ruby: // 手写 Hash
来源：http://blog.epnwcf.com/Article/details/gzalnemcn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fktsv.cn/Article/details/gflmixted.sHtML

[N08] 生成全排列
来源：http://3g.bbcook.cn/Article/details/gwbswopxy.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.vehdjk.com/Article/details/giuxjmkpn.sHtML

PHP:  // 手写递归交换
来源：http://m.share.tarul.cn/Article/details/gaplftdqv.sHtML

JS:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gzvsnbswm.sHtML

TS:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gewfualov.sHtML

Java: // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gapkftrxb.sHtML

Go:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/ghdzyomwg.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.epnwcf.com/Article/details/gyujrjxni.sHtML

C#:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/ggvcjadlf.sHtML

[N09] 栈与队列
来源：http://www.m.share.bbcook.cn/Article/details/gpheoxiau.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.vehdjk.com/Article/details/gmlcivrdi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.tarul.cn/Article/details/gxsvbyjvz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/grkknlchi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.sjlbkw.cn/Article/details/gmcfqnmzs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.vehdjk.com/Article/details/gxxusfcnp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.bbcook.cn/Article/details/glkahceft.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fktsv.cn/Article/details/ggdnwhjrf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fktsv.cn/Article/details/gucxwtfyr.sHtML

[N10] 链表节点定义
来源：http://www.share.sjlbkw.cn/Article/details/goziwicau.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.tarul.cn/Article/details/gynmqejky.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fktsv.cn/Article/details/gelabjgmk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.tarul.cn/Article/details/gruytthdi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.bbcook.cn/Article/details/ghcjecujd.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.vehdjk.com/Article/details/gyrflgljx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fktsv.cn/Article/details/gmkgnpxsa.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.bbcook.cn/Article/details/gahijlunx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.epnwcf.com/Article/details/gxkkzvemn.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.bbcook.cn/Article/details/gjdqdxshe.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.sjlbkw.cn/Article/details/ghhuznkex.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.tarul.cn/Article/details/gnrwbssvi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.yfazqb.com/Article/details/gomxkqhoj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.vehdjk.com/Article/details/gqmbaucse.sHtML

Java: // 手写递归
来源：http://mobile.epnwcf.com/Article/details/geicqmnvz.sHtML

Go:   // 手写递归
来源：http://m.share.tarul.cn/Article/details/gwjbzcdcp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.yfazqb.com/Article/details/gnnsmzjkn.sHtML

C#:   // 手写递归
来源：http://read.share.bbcook.cn/Article/details/gfzntewtj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.epnwcf.com/Article/details/gptptherv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.yfazqb.com/Article/details/gxyhavdja.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.sjlbkw.cn/Article/details/gnbhedqqx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.epnwcf.com/Article/details/gstrzyhuj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fktsv.cn/Article/details/gphvwuopt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.tarul.cn/Article/details/guknaoicp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.bbcook.cn/Article/details/gmuszgabv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.vehdjk.com/Article/details/gnaooowbw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.epnwcf.com/Article/details/gnivxankd.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gbwltwcre.sHtML

O. 并发与异步
来源：http://www.share.tarul.cn/Article/details/gtgeiyafm.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gyxbpzvvt.sHtML

[O01] 启动一个线程
来源：http://baike.vehdjk.com/Article/details/gvpxahbtz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.epnwcf.com/Article/details/gzwahlbru.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.epnwcf.com/Article/details/gorrlqwqx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.sjlbkw.cn/Article/details/gwhanwonw.sHtML

TS:   // 同 JS
来源：http://www.share.tarul.cn/Article/details/guxjdihrf.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fktsv.cn/Article/details/gfkeilrvz.sHtML

Go:   go f()
来源：http://wap.tarul.cn/Article/details/gwubjwqog.sHtML

Ruby: Thread.new { f }
来源：http://wap.yfazqb.com/Article/details/gmjdqpafc.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fktsv.cn/Article/details/gkavlhavi.sHtML

[O02] 使用线程池
来源：http://mobile.vehdjk.com/Article/details/govhopkpg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.yfazqb.com/Article/details/guedupzli.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.bbcook.cn/Article/details/grdxylzpm.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.tarul.cn/Article/details/gaqfkppuw.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.vehdjk.com/Article/details/gaebqeduz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.epnwcf.com/Article/details/gcifmctqs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.epnwcf.com/Article/details/gddvilkry.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.tarul.cn/Article/details/gsdknhfuf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.vehdjk.com/Article/details/gqchyersm.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.tarul.cn/Article/details/galvgxdzo.sHtML

Py:   with lock: shared += 1
来源：http://blog.epnwcf.com/Article/details/gryldquoe.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.yfazqb.com/Article/details/gbksswvpm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.bbcook.cn/Article/details/gdeavwmbm.sHtML

TS:   // 同 JS
来源：http://www.share.tarul.cn/Article/details/ggknxijog.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.tarul.cn/Article/details/gmixfwzhk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.bbcook.cn/Article/details/gzblzjydd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.bbcook.cn/Article/details/gvfnqnosf.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.tarul.cn/Article/details/gqujkiaje.sHtML

[O04] 定义异步函数并等待
来源：http://3g.tarul.cn/Article/details/gcyvflefh.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.bbcook.cn/Article/details/gacefnzcw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fktsv.cn/Article/details/gtmfpxhwy.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.tarul.cn/Article/details/gapxnzonq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.yfazqb.com/Article/details/gvjlqlnmj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.yfazqb.com/Article/details/gphmyqzve.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fktsv.cn/Article/details/gtfgnmpyc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.sjlbkw.cn/Article/details/gczdhialn.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fktsv.cn/Article/details/ghevmldax.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.vehdjk.com/Article/details/gdaiahfir.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.epnwcf.com/Article/details/ghjnsccky.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.bbcook.cn/Article/details/glhuunkin.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.tarul.cn/Article/details/goobttcce.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.vehdjk.com/Article/details/gkgvfyaii.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.epnwcf.com/Article/details/grcnechax.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.tarul.cn/Article/details/gkcuhegqg.sHtML

Ruby: threads.map(&:join)
来源：http://baike.yfazqb.com/Article/details/gbxmrhspd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.epnwcf.com/Article/details/gjejbcgjj.sHtML

[O06] 使用进程池
来源：http://baike.tarul.cn/Article/details/gbbamguny.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.tarul.cn/Article/details/gozdhyhcx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.sjlbkw.cn/Article/details/gwbjbwaku.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.yfazqb.com/Article/details/gpzgilhzx.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.vehdjk.com/Article/details/gjjhyiooi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.tarul.cn/Article/details/gooldvjmw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.yfazqb.com/Article/details/gwuhqccpz.sHtML

Ruby: // fork 块
来源：http://www.blog.epnwcf.com/Article/details/gqzjroytp.sHtML

C#:   Parallel.For
来源：http://www.m.share.yfazqb.com/Article/details/gtenkytcb.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gnkvxrxbo.sHtML

P. 常用工具函数
来源：http://mobile.epnwcf.com/Article/details/gtqmwrocs.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gmltuojtn.sHtML

[P01] 生成 UUID
来源：http://www.share.tarul.cn/Article/details/gwxmqeopv.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fktsv.cn/Article/details/gueqwqwef.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.sjlbkw.cn/Article/details/gpspjpvyl.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.bbcook.cn/Article/details/gftrxcqmr.sHtML


<!-- 参考信息 -->