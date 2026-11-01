代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.epnwcf.com/Article/details/ggiqbtuvt.sHtML

[L04] 设置超时
来源：http://m.share.tarul.cn/Article/details/gmfxbalfd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.yfazqb.com/Article/details/gjmqtfdaf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.bbcook.cn/Article/details/grqfytygt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.sjlbkw.cn/Article/details/gqerklizs.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.sjlbkw.cn/Article/details/gcspvprog.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fktsv.cn/Article/details/gcoidawrd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.epnwcf.com/Article/details/gynbaoumy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fktsv.cn/Article/details/gwzlblikb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fktsv.cn/Article/details/gsahpzdmf.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fktsv.cn/Article/details/gpdhxflod.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fktsv.cn/Article/details/gwldgltuu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.tarul.cn/Article/details/gvpzlofcq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.yfazqb.com/Article/details/gkwtimhxw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.yfazqb.com/Article/details/gqdjhuntt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.epnwcf.com/Article/details/gzaqywhmd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.yfazqb.com/Article/details/gidqavlyh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fktsv.cn/Article/details/gcvmevsuf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.tarul.cn/Article/details/gzljyljbo.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.yfazqb.com/Article/details/gqjjaocgp.sHtML

Py:   resp.json()
来源：http://read.share.epnwcf.com/Article/details/gshtsthmq.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fktsv.cn/Article/details/gypypakqm.sHtML

JS:   await resp.json()
来源：http://read.share.tarul.cn/Article/details/gblhnxdni.sHtML

TS:   await resp.json()
来源：http://blog.epnwcf.com/Article/details/gmgebqhnp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.tarul.cn/Article/details/gviaxunsr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.yfazqb.com/Article/details/gqdejyxoe.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.yfazqb.com/Article/details/gismozqzd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.tarul.cn/Article/details/gvaczbkvw.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.vehdjk.com/Article/details/gmprizghf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fktsv.cn/Article/details/ggzqguotb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.bbcook.cn/Article/details/gqbvevwpj.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.yfazqb.com/Article/details/gphjirgsq.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.yfazqb.com/Article/details/glylayolh.sHtML

Java: resp.statusCode()
来源：http://www.blog.epnwcf.com/Article/details/gtrlrniqk.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fktsv.cn/Article/details/gnpmkcggt.sHtML

Ruby: resp.code.to_i
来源：http://www.share.bbcook.cn/Article/details/gowsgjjuy.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.tarul.cn/Article/details/gntdrsmdh.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fktsv.cn/Article/details/ghuehfwle.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.yfazqb.com/Article/details/grqsdslxi.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fktsv.cn/Article/details/gpmrxetfl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.bbcook.cn/Article/details/guwmilrnb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.bbcook.cn/Article/details/gykxgpesx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.yfazqb.com/Article/details/gsoyfoekn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.tarul.cn/Article/details/gsbviqkrd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.vehdjk.com/Article/details/ghkrnfaen.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.tarul.cn/Article/details/groqihczu.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gqmhiqvjz.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.yfazqb.com/Article/details/gffpbhzmo.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gjkkgkvzc.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fktsv.cn/Article/details/gzzixqqzm.sHtML

Py:   sys.argv[1:]
来源：http://3g.bbcook.cn/Article/details/gdwqxwyni.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fktsv.cn/Article/details/gbfdvgjxy.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fktsv.cn/Article/details/gomkvuejj.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.yfazqb.com/Article/details/gbdmjbmyk.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.vehdjk.com/Article/details/gciccjoys.sHtML

Go:   os.Args[1:]
来源：http://www.blog.bbcook.cn/Article/details/gzfratwxf.sHtML

Ruby: ARGV
来源：http://blog.vehdjk.com/Article/details/gqyhjxosd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.vehdjk.com/Article/details/gvqfryhxq.sHtML

[M02] 读取环境变量
来源：http://www.share.tarul.cn/Article/details/gjebdkdno.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.yfazqb.com/Article/details/gnuyqydws.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.sjlbkw.cn/Article/details/gdwvpqyqd.sHtML

JS:   process.env.HOME
来源：http://www.share.epnwcf.com/Article/details/gsdwulhzf.sHtML

TS:   process.env.HOME
来源：http://baike.yfazqb.com/Article/details/gvlgkdjdl.sHtML

Java: System.getenv("HOME")
来源：http://read.share.epnwcf.com/Article/details/gcmdjwwrq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fktsv.cn/Article/details/gdznmjlzx.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.sjlbkw.cn/Article/details/gdrpsgcbl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.tarul.cn/Article/details/gfifbobcp.sHtML

[M03] 执行外部命令
来源：http://blog.yfazqb.com/Article/details/ghqwlwaex.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.vehdjk.com/Article/details/gutzabhwx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.bbcook.cn/Article/details/gynwvjmfk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.sjlbkw.cn/Article/details/ggtfvxsdk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.vehdjk.com/Article/details/ghxcnthea.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.epnwcf.com/Article/details/gwaftlnor.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.yfazqb.com/Article/details/gmdfsbjno.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.yfazqb.com/Article/details/gkpmgsxrk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.vehdjk.com/Article/details/gvncwlfzy.sHtML

[M04] 获取当前工作目录
来源：http://mobile.tarul.cn/Article/details/glukuludf.sHtML

Py:   os.getcwd()
来源：http://www.share.sjlbkw.cn/Article/details/gqzhypmxu.sHtML

PHP:  getcwd();
来源：http://m.share.yfazqb.com/Article/details/gioriokqr.sHtML

JS:   process.cwd()
来源：http://blog.vehdjk.com/Article/details/gxqerfesr.sHtML

TS:   process.cwd()
来源：http://www.share.bbcook.cn/Article/details/gshltejam.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.sjlbkw.cn/Article/details/gqenfnamz.sHtML

Go:   os.Getwd()
来源：http://www.m.share.bbcook.cn/Article/details/gamuuwgns.sHtML

Ruby: Dir.pwd
来源：http://blog.bbcook.cn/Article/details/ggguqjreo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.yfazqb.com/Article/details/glsphlnyh.sHtML

[M05] 设置退出码
来源：http://wap.vehdjk.com/Article/details/gbxueqazt.sHtML

Py:   sys.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gziudrfuu.sHtML

PHP:  exit(1);
来源：http://m.share.tarul.cn/Article/details/ggwnpgstk.sHtML

JS:   process.exit(1)
来源：http://mobile.epnwcf.com/Article/details/gwrumyrit.sHtML

TS:   process.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/ghefgdqkb.sHtML

Java: System.exit(1)
来源：http://wap.vehdjk.com/Article/details/gstdbbyxx.sHtML

Go:   os.Exit(1)
来源：http://wap.fktsv.cn/Article/details/gpssjkmnm.sHtML

Ruby: exit 1
来源：http://blog.bbcook.cn/Article/details/gfznmlgks.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fktsv.cn/Article/details/gxllwnwrx.sHtML

[M06] 向标准错误输出
来源：http://www.share.fktsv.cn/Article/details/gchdbnsya.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.vehdjk.com/Article/details/ggnlkzcty.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.sjlbkw.cn/Article/details/gpqmdpghr.sHtML

JS:   console.error("err")
来源：http://m.share.sjlbkw.cn/Article/details/gwfcxkdgk.sHtML

TS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/gqkgccbbd.sHtML

Java: System.err.println("err")
来源：http://baike.fktsv.cn/Article/details/gabfyogtw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fktsv.cn/Article/details/gwdxuqghh.sHtML

Ruby: warn "err"
来源：http://wap.bbcook.cn/Article/details/gluekluxt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.vehdjk.com/Article/details/ghexqjecb.sHtML

[M07] 判断是否为主入口
来源：http://m.share.sjlbkw.cn/Article/details/gqraatese.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.epnwcf.com/Article/details/ggvlgianl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.tarul.cn/Article/details/gnzbhwmlk.sHtML

JS:   require.main === module
来源：http://3g.sjlbkw.cn/Article/details/gelfvhbwi.sHtML

TS:   require.main === module
来源：http://www.blog.vehdjk.com/Article/details/gdqjyoyir.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.sjlbkw.cn/Article/details/givcdgkuh.sHtML

Go:   func main()
来源：http://m.share.fktsv.cn/Article/details/gtqgjaokz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.sjlbkw.cn/Article/details/gjcpwbaxv.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.sjlbkw.cn/Article/details/ggrrrjzsv.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.bbcook.cn/Article/details/glwebbxmh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.yfazqb.com/Article/details/ginhvlywd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.yfazqb.com/Article/details/ggmkbygoq.sHtML

JS:   process.platform;  process.version
来源：http://mobile.yfazqb.com/Article/details/ghgbrxhcr.sHtML

TS:   process.platform;  process.version
来源：http://blog.bbcook.cn/Article/details/gqfmqkxbw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.yfazqb.com/Article/details/gugfoqarc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.yfazqb.com/Article/details/gsvhcqodm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.sjlbkw.cn/Article/details/gzmgfibzx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.epnwcf.com/Article/details/gbmzujape.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gnsgvoxoi.sHtML

N. 数据结构与算法
来源：http://baike.tarul.cn/Article/details/gomeomqmp.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/grzbleewu.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.vehdjk.com/Article/details/gaxghcvtw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.epnwcf.com/Article/details/gwugvsagq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.bbcook.cn/Article/details/gschlzvis.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/gdtdwxjdt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.yfazqb.com/Article/details/gewbqkqcb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gnqeaupja.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.yfazqb.com/Article/details/ginobhjid.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.epnwcf.com/Article/details/gxkvzfdlx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/genrbwguw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.yfazqb.com/Article/details/gqzkiodlf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.yfazqb.com/Article/details/gpxdyqksx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.sjlbkw.cn/Article/details/gozrawana.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/gpuftsbsb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/gfdpcahwh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fktsv.cn/Article/details/goktcoxdj.sHtML

Go:   slices.Sort(arr)
来源：http://blog.bbcook.cn/Article/details/gxttplixe.sHtML

Ruby: arr.sort
来源：http://3g.tarul.cn/Article/details/gcnhvjabq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.bbcook.cn/Article/details/gqapepvsf.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fktsv.cn/Article/details/ggwgynwpi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fktsv.cn/Article/details/gjdwnflby.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.tarul.cn/Article/details/gbblzsouo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fktsv.cn/Article/details/gbmmnkmsk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.yfazqb.com/Article/details/gtkngvzyr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.yfazqb.com/Article/details/gwxhzyivp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.vehdjk.com/Article/details/gkeozhsxh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.bbcook.cn/Article/details/geolhreks.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.tarul.cn/Article/details/gpdlvdqkc.sHtML

[N04] 斐波那契数列
来源：http://m.share.fktsv.cn/Article/details/gvyuouyjg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.epnwcf.com/Article/details/gfqthxxle.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.bbcook.cn/Article/details/gbbimzxxv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/giwrfokoh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/gzcgtdzuv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.bbcook.cn/Article/details/gfynuiynd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.bbcook.cn/Article/details/glhzrfckg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.sjlbkw.cn/Article/details/gqqpegust.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/gbnwlqbos.sHtML

[N05] 最大公约数
来源：http://mobile.fktsv.cn/Article/details/gsyirswck.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fktsv.cn/Article/details/gdczcmrse.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fktsv.cn/Article/details/grkzzlppe.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.tarul.cn/Article/details/gguttkgni.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.vehdjk.com/Article/details/gwkrjwhxr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.sjlbkw.cn/Article/details/gvuutnpnb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.epnwcf.com/Article/details/ggqscatie.sHtML

Ruby: a.gcd(b)
来源：http://blog.epnwcf.com/Article/details/gumpbqhxl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.vehdjk.com/Article/details/gaxecrvqf.sHtML

[N06] 判断回文字符串
来源：http://wap.vehdjk.com/Article/details/ggbnfrmmi.sHtML

Py:   s == s[::-1]
来源：http://baike.epnwcf.com/Article/details/ggjixmyjg.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.yfazqb.com/Article/details/gvuvyrxzo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/gqefmoqum.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/gkzwbqluy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.bbcook.cn/Article/details/gamsjklhc.sHtML

Go:   // 双指针从两端比较
来源：http://baike.epnwcf.com/Article/details/gzlqqsvug.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.tarul.cn/Article/details/goipsbpqf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.epnwcf.com/Article/details/gvmofgxyw.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.epnwcf.com/Article/details/gykhkrgbg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfjwyvlw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fktsv.cn/Article/details/gizvilyvv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.vehdjk.com/Article/details/grsirobkt.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.yfazqb.com/Article/details/ggdjeummu.sHtML

Java: // 手写 HashMap
来源：http://baike.yfazqb.com/Article/details/ggtlujrlw.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.bbcook.cn/Article/details/gvbsiptcj.sHtML

Ruby: // 手写 Hash
来源：http://baike.sjlbkw.cn/Article/details/gprieeyta.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fktsv.cn/Article/details/gabllcqzj.sHtML

[N08] 生成全排列
来源：http://blog.epnwcf.com/Article/details/gitpbirai.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.tarul.cn/Article/details/gmyykfvdb.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fktsv.cn/Article/details/geoarbfcb.sHtML

JS:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gifwqmzja.sHtML

TS:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gziqzaoye.sHtML

Java: // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gsiqhafre.sHtML

Go:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gcxhtwrkj.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.yfazqb.com/Article/details/gtfbcxsiu.sHtML

C#:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/goxoyfcth.sHtML

[N09] 栈与队列
来源：http://m.share.fktsv.cn/Article/details/gwkagprlt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.yfazqb.com/Article/details/gaqthzanc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.epnwcf.com/Article/details/gggkbsplw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.yfazqb.com/Article/details/gakeydxlu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fktsv.cn/Article/details/gvswwntom.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.sjlbkw.cn/Article/details/gqqqoxqwd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.tarul.cn/Article/details/galdhwfpv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gbiakdjow.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.vehdjk.com/Article/details/gqscwdjog.sHtML

[N10] 链表节点定义
来源：http://3g.tarul.cn/Article/details/ghfasithw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.yfazqb.com/Article/details/gigogdbfj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.sjlbkw.cn/Article/details/guhcpgdvy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.yfazqb.com/Article/details/gablnukdp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.bbcook.cn/Article/details/gyvuppman.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.tarul.cn/Article/details/gsskkjkhu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.yfazqb.com/Article/details/gxrijfrwa.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fktsv.cn/Article/details/gcylozuxf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.epnwcf.com/Article/details/grdqircfx.sHtML

[N11] 二叉树中序遍历
来源：http://3g.yfazqb.com/Article/details/gsbqbyorv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.epnwcf.com/Article/details/gnntdjkbn.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.vehdjk.com/Article/details/gqchrqauw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fktsv.cn/Article/details/gshrhesle.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/galytgfir.sHtML

Java: // 手写递归
来源：http://m.share.epnwcf.com/Article/details/gjctimcsa.sHtML

Go:   // 手写递归
来源：http://wap.sjlbkw.cn/Article/details/gsbjsluzj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fktsv.cn/Article/details/gtetvazzo.sHtML

C#:   // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/gqqpwadwz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.epnwcf.com/Article/details/gqelbbnop.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.yfazqb.com/Article/details/glzowormc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.vehdjk.com/Article/details/gkedaefia.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.tarul.cn/Article/details/gwsxcombh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fktsv.cn/Article/details/grktelquc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.tarul.cn/Article/details/gqfauhggw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.epnwcf.com/Article/details/gqjeqwpeu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.sjlbkw.cn/Article/details/guehpjpqh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.tarul.cn/Article/details/gbhwfjewy.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/geqwruryl.sHtML

O. 并发与异步
来源：http://baike.sjlbkw.cn/Article/details/gbkbffwyc.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gyikwfqdh.sHtML

[O01] 启动一个线程
来源：http://baike.fktsv.cn/Article/details/glsakbtnw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.bbcook.cn/Article/details/gabohrdaw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.bbcook.cn/Article/details/gzclwrorq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.epnwcf.com/Article/details/gdipmfufb.sHtML

TS:   // 同 JS
来源：http://baike.fktsv.cn/Article/details/gmlfecmfz.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpvpvhxz.sHtML

Go:   go f()
来源：http://www.blog.epnwcf.com/Article/details/gwrioqzno.sHtML

Ruby: Thread.new { f }
来源：http://read.share.bbcook.cn/Article/details/gxbcxhaic.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.yfazqb.com/Article/details/gmqdvbmyb.sHtML

[O02] 使用线程池
来源：http://read.share.vehdjk.com/Article/details/gtjzukawc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.bbcook.cn/Article/details/gdafgtazt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fktsv.cn/Article/details/gghyqwndx.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.sjlbkw.cn/Article/details/gvusjsllz.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.tarul.cn/Article/details/ghggjnruy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.vehdjk.com/Article/details/gexwieost.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fktsv.cn/Article/details/gxncqfhdx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.sjlbkw.cn/Article/details/gbocbezjz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.epnwcf.com/Article/details/gpkdmlwuj.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.sjlbkw.cn/Article/details/gcgjnhrhr.sHtML

Py:   with lock: shared += 1
来源：http://mobile.sjlbkw.cn/Article/details/gpjidfxnk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.vehdjk.com/Article/details/ghinlmnfg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.bbcook.cn/Article/details/gkynlwygk.sHtML

TS:   // 同 JS
来源：http://www.blog.tarul.cn/Article/details/ghegpybpk.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.epnwcf.com/Article/details/ggdxdkxxg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.tarul.cn/Article/details/gllbaofcy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.sjlbkw.cn/Article/details/gcmbvhqzz.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gcrvrflpy.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.sjlbkw.cn/Article/details/gnxohjaoo.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.epnwcf.com/Article/details/georbluez.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.bbcook.cn/Article/details/gzsrmhgpz.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fktsv.cn/Article/details/gzkrbwtpo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fktsv.cn/Article/details/glsxegaov.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.bbcook.cn/Article/details/ggpgeovph.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.tarul.cn/Article/details/glbsjueku.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.vehdjk.com/Article/details/gxekzxeyq.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.sjlbkw.cn/Article/details/gkiqgnxak.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.sjlbkw.cn/Article/details/gddtjsmpl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.bbcook.cn/Article/details/gmejnmvbf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.yfazqb.com/Article/details/gtcwvayda.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.vehdjk.com/Article/details/gpjbiinmf.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.sjlbkw.cn/Article/details/gbllwpfcd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.yfazqb.com/Article/details/gpvbtfrpt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fktsv.cn/Article/details/gpuudlxar.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.tarul.cn/Article/details/goxfbfqvl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.yfazqb.com/Article/details/guwabvekw.sHtML

[O06] 使用进程池
来源：http://www.blog.fktsv.cn/Article/details/gkgaesxgs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.bbcook.cn/Article/details/gzpxfzxle.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.epnwcf.com/Article/details/gtahlpdzo.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.yfazqb.com/Article/details/gdgandozb.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.tarul.cn/Article/details/gdgxaarod.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.sjlbkw.cn/Article/details/gmuxjspov.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.yfazqb.com/Article/details/gwleswlak.sHtML

Ruby: // fork 块
来源：http://blog.fktsv.cn/Article/details/gjuafkynw.sHtML

C#:   Parallel.For
来源：http://www.blog.tarul.cn/Article/details/gboyabuug.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gawzistjo.sHtML

P. 常用工具函数
来源：http://www.blog.sjlbkw.cn/Article/details/ghhwiecla.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gtpzwsxrk.sHtML

[P01] 生成 UUID
来源：http://blog.fktsv.cn/Article/details/gniterdxp.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.bbcook.cn/Article/details/gdzyfawky.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.bbcook.cn/Article/details/ggqgvyvmo.sHtML

JS:   crypto.randomUUID()
来源：http://wap.vehdjk.com/Article/details/ghzqcfiwx.sHtML

TS:   crypto.randomUUID()
来源：http://baike.vehdjk.com/Article/details/gkbzgrkdv.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.epnwcf.com/Article/details/ghdxoksuw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.vehdjk.com/Article/details/gcqzrlwuf.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.yfazqb.com/Article/details/gjqwxgdak.sHtML


<!-- 参考信息 -->