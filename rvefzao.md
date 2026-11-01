代发 wailian999

[L03] 设置自定义请求头
来源：http://blog.yfazqb.com/Article/details/gratpjfce.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.bbcook.cn/Article/details/gduwoqcuv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.bbcook.cn/Article/details/gwwtnienl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.tarul.cn/Article/details/gsfaybjox.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.yfazqb.com/Article/details/gvzykaubu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.bbcook.cn/Article/details/gpomobvst.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.epnwcf.com/Article/details/glntwsosp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.sjlbkw.cn/Article/details/gevfmnvew.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.bbcook.cn/Article/details/giuvueevx.sHtML

[L04] 设置超时
来源：http://read.share.tarul.cn/Article/details/gjatqdocm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.vehdjk.com/Article/details/ggxpntqbi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.bbcook.cn/Article/details/gvplvbmma.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.vehdjk.com/Article/details/ghpwkezra.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.epnwcf.com/Article/details/gssqbmzcu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.epnwcf.com/Article/details/ggqcodbth.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.yfazqb.com/Article/details/gyofxgvow.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.epnwcf.com/Article/details/gbnsgmaej.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.yfazqb.com/Article/details/gauzzoazr.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.epnwcf.com/Article/details/gfwdflhmc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.tarul.cn/Article/details/gmjfdgqfj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fktsv.cn/Article/details/gcmmofqmj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.tarul.cn/Article/details/gdcrddgij.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.vehdjk.com/Article/details/gkywjzdah.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.bbcook.cn/Article/details/glsqpslqx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fktsv.cn/Article/details/gdsqfescr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.yfazqb.com/Article/details/gfinylcnk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.epnwcf.com/Article/details/gohcqvngx.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.bbcook.cn/Article/details/gvnsmahml.sHtML

Py:   resp.json()
来源：http://blog.bbcook.cn/Article/details/gowcdsfxw.sHtML

PHP:  json_decode($body, true);
来源：http://3g.sjlbkw.cn/Article/details/gujaljjqm.sHtML

JS:   await resp.json()
来源：http://blog.sjlbkw.cn/Article/details/gusgewfqy.sHtML

TS:   await resp.json()
来源：http://blog.bbcook.cn/Article/details/gddjgovet.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.yfazqb.com/Article/details/godccgkuu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.vehdjk.com/Article/details/gqaogmxzk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fktsv.cn/Article/details/ggkkjozkq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.yfazqb.com/Article/details/gfpvavvdx.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.vehdjk.com/Article/details/gnrhjwtjq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.vehdjk.com/Article/details/gcjyayfbb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.tarul.cn/Article/details/gieucfsiu.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fktsv.cn/Article/details/gmnuaxacq.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.bbcook.cn/Article/details/gwxpewqfc.sHtML

Java: resp.statusCode()
来源：http://mobile.vehdjk.com/Article/details/gwnsvlxgl.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.tarul.cn/Article/details/ghhgqyltm.sHtML

Ruby: resp.code.to_i
来源：http://wap.fktsv.cn/Article/details/ghumvduyl.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.tarul.cn/Article/details/gkwmqslqu.sHtML

[L08] 并发请求多个地址
来源：http://mobile.tarul.cn/Article/details/gtpfxmkse.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fktsv.cn/Article/details/ginicrpup.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.sjlbkw.cn/Article/details/gechfcehg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.epnwcf.com/Article/details/grexlskyt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.yfazqb.com/Article/details/gimcuhjpf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.vehdjk.com/Article/details/gvdhabdbv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.bbcook.cn/Article/details/gpbhoubgi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.yfazqb.com/Article/details/gbwoltxsl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fktsv.cn/Article/details/gsqvkzdkw.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gxysfghwx.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.epnwcf.com/Article/details/gdrjqxbhc.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gdvrxotpe.sHtML

[M01] 读取命令行参数
来源：http://baike.fktsv.cn/Article/details/gdohdkntw.sHtML

Py:   sys.argv[1:]
来源：http://blog.fktsv.cn/Article/details/gptxowltm.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.epnwcf.com/Article/details/gzwmeyoek.sHtML

JS:   process.argv.slice(2)
来源：http://3g.epnwcf.com/Article/details/gzgatwxiq.sHtML

TS:   process.argv.slice(2)
来源：http://3g.vehdjk.com/Article/details/gsdlcsoac.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.yfazqb.com/Article/details/givavqsuf.sHtML

Go:   os.Args[1:]
来源：http://baike.vehdjk.com/Article/details/ghujazttz.sHtML

Ruby: ARGV
来源：http://www.m.share.bbcook.cn/Article/details/gkkowplrq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.epnwcf.com/Article/details/gxuqblsho.sHtML

[M02] 读取环境变量
来源：http://www.share.epnwcf.com/Article/details/gmxeqvxfh.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.yfazqb.com/Article/details/gxiegclrc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.tarul.cn/Article/details/gwwvjinqh.sHtML

JS:   process.env.HOME
来源：http://3g.bbcook.cn/Article/details/gixpmwrrs.sHtML

TS:   process.env.HOME
来源：http://blog.vehdjk.com/Article/details/gztactzfo.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gyeyvolci.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.tarul.cn/Article/details/gfwtsarpn.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.yfazqb.com/Article/details/gqiaaoiaw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/ghxxeggmg.sHtML

[M03] 执行外部命令
来源：http://baike.epnwcf.com/Article/details/gcgssvgzu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.tarul.cn/Article/details/gqkzjqpda.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.epnwcf.com/Article/details/guaprlkal.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.tarul.cn/Article/details/gbwuuuzge.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.sjlbkw.cn/Article/details/ggomxvcxn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.epnwcf.com/Article/details/ghtbxrrra.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.sjlbkw.cn/Article/details/gzwrzthyj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.sjlbkw.cn/Article/details/gmexjjxoa.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.epnwcf.com/Article/details/geghqnnmj.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fktsv.cn/Article/details/gtztqxddg.sHtML

Py:   os.getcwd()
来源：http://blog.vehdjk.com/Article/details/gsnetvryg.sHtML

PHP:  getcwd();
来源：http://www.blog.bbcook.cn/Article/details/gpjkvppma.sHtML

JS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/glvormluj.sHtML

TS:   process.cwd()
来源：http://3g.sjlbkw.cn/Article/details/gnlecvhjy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.bbcook.cn/Article/details/guticvhqa.sHtML

Go:   os.Getwd()
来源：http://blog.bbcook.cn/Article/details/ghwzxvseq.sHtML

Ruby: Dir.pwd
来源：http://www.share.fktsv.cn/Article/details/gfhkltlcs.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.yfazqb.com/Article/details/gpqtviaju.sHtML

[M05] 设置退出码
来源：http://mobile.tarul.cn/Article/details/gkwrcgdse.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gtaumiqsb.sHtML

PHP:  exit(1);
来源：http://www.share.sjlbkw.cn/Article/details/gjedhubnt.sHtML

JS:   process.exit(1)
来源：http://www.share.bbcook.cn/Article/details/glhdqcqcc.sHtML

TS:   process.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gaqskpwpw.sHtML

Java: System.exit(1)
来源：http://blog.tarul.cn/Article/details/ghiphakhv.sHtML

Go:   os.Exit(1)
来源：http://www.share.fktsv.cn/Article/details/gkxnvnnnm.sHtML

Ruby: exit 1
来源：http://mobile.yfazqb.com/Article/details/gyxxloryn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.sjlbkw.cn/Article/details/gyuoapypr.sHtML

[M06] 向标准错误输出
来源：http://www.blog.yfazqb.com/Article/details/ggjpyomkc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.yfazqb.com/Article/details/gmupqyukk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.epnwcf.com/Article/details/ghgiuzpwe.sHtML

JS:   console.error("err")
来源：http://blog.vehdjk.com/Article/details/ghwttclam.sHtML

TS:   console.error("err")
来源：http://baike.bbcook.cn/Article/details/gsxhrwgxo.sHtML

Java: System.err.println("err")
来源：http://blog.sjlbkw.cn/Article/details/gcaylkprl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.bbcook.cn/Article/details/gxkprqaji.sHtML

Ruby: warn "err"
来源：http://www.m.share.fktsv.cn/Article/details/gpflogsmb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.epnwcf.com/Article/details/gkmmbhjzn.sHtML

[M07] 判断是否为主入口
来源：http://3g.vehdjk.com/Article/details/ghmwekfsg.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.vehdjk.com/Article/details/geemlmxwr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.epnwcf.com/Article/details/gafndbjkq.sHtML

JS:   require.main === module
来源：http://www.blog.bbcook.cn/Article/details/gawqoexza.sHtML

TS:   require.main === module
来源：http://blog.yfazqb.com/Article/details/ghpfzwjhc.sHtML

Java: public static void main(String[] args)
来源：http://www.share.epnwcf.com/Article/details/gignbzwbt.sHtML

Go:   func main()
来源：http://www.m.share.bbcook.cn/Article/details/gusgdhqpc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.yfazqb.com/Article/details/ggjnqjyhc.sHtML

C#:   static void Main(string[] args)
来源：http://baike.epnwcf.com/Article/details/ginzkrnqa.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fktsv.cn/Article/details/gyebkilmg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.epnwcf.com/Article/details/gezzcyxkg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.sjlbkw.cn/Article/details/gbbhrbybn.sHtML

JS:   process.platform;  process.version
来源：http://m.share.sjlbkw.cn/Article/details/gqzaubucj.sHtML

TS:   process.platform;  process.version
来源：http://baike.yfazqb.com/Article/details/glopchagx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.bbcook.cn/Article/details/gjkpgajlo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.vehdjk.com/Article/details/gbhknmzpl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.bbcook.cn/Article/details/gvslelemy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.tarul.cn/Article/details/gfhucovvk.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gqoeqojzd.sHtML

N. 数据结构与算法
来源：http://baike.sjlbkw.cn/Article/details/gwvlpqugh.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gcxduzaef.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.tarul.cn/Article/details/gtuwkbdys.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.vehdjk.com/Article/details/gqgdugmqd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.sjlbkw.cn/Article/details/gwbjvwwuq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/grvlehhpk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.vehdjk.com/Article/details/gcnpjeqwo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.tarul.cn/Article/details/guwvbeqed.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gfcirsbwg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.tarul.cn/Article/details/gzhtkhojl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gihfoailx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fktsv.cn/Article/details/gegtxfwxm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fktsv.cn/Article/details/gvpcanswa.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.epnwcf.com/Article/details/glhcgvlob.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.bbcook.cn/Article/details/geaplwrqc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/guvusebwo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.bbcook.cn/Article/details/gnmzvarrl.sHtML

Go:   slices.Sort(arr)
来源：http://baike.sjlbkw.cn/Article/details/ghqlbzgnf.sHtML

Ruby: arr.sort
来源：http://www.m.share.sjlbkw.cn/Article/details/ghfiaxpqo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.yfazqb.com/Article/details/gvjwrpbst.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.vehdjk.com/Article/details/gbvxejrhb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.tarul.cn/Article/details/gsnxngayp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.sjlbkw.cn/Article/details/gubxpgjnh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.bbcook.cn/Article/details/gxisambyi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fktsv.cn/Article/details/gqyimpxow.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.sjlbkw.cn/Article/details/gdmpgeesa.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.yfazqb.com/Article/details/gznrzogsr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.bbcook.cn/Article/details/gjxebqgye.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.yfazqb.com/Article/details/ggamizeky.sHtML

[N04] 斐波那契数列
来源：http://baike.tarul.cn/Article/details/gqgvhqurd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.bbcook.cn/Article/details/ggwrcmynj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.yfazqb.com/Article/details/gcsalzbhn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/gijdlncle.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gpfbnmwdb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.bbcook.cn/Article/details/glffscuec.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.vehdjk.com/Article/details/gpfctiamr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.yfazqb.com/Article/details/gpgxibcnr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.bbcook.cn/Article/details/ghbshtmpe.sHtML

[N05] 最大公约数
来源：http://baike.bbcook.cn/Article/details/gverthjeb.sHtML

Py:   math.gcd(a, b)
来源：http://blog.vehdjk.com/Article/details/gfrsvemll.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.bbcook.cn/Article/details/ggxucdjnk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.vehdjk.com/Article/details/ghundovhp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.bbcook.cn/Article/details/gspuyzquk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.tarul.cn/Article/details/gslptksdo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.epnwcf.com/Article/details/giapadtwz.sHtML

Ruby: a.gcd(b)
来源：http://www.share.sjlbkw.cn/Article/details/gmatapcse.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.yfazqb.com/Article/details/gzgfqgsmk.sHtML

[N06] 判断回文字符串
来源：http://mobile.sjlbkw.cn/Article/details/gkwummyhr.sHtML

Py:   s == s[::-1]
来源：http://wap.yfazqb.com/Article/details/gmzpcsefh.sHtML

PHP:  $s === strrev($s);
来源：http://wap.sjlbkw.cn/Article/details/gssifrmxm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/ghpdbflug.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/grviizppt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.tarul.cn/Article/details/gdixlclwr.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fktsv.cn/Article/details/gavwvgfos.sHtML

Ruby: s == s.reverse
来源：http://baike.vehdjk.com/Article/details/gntvqdgon.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.sjlbkw.cn/Article/details/gpoyawjec.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.vehdjk.com/Article/details/gxirnmlnt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.tarul.cn/Article/details/gbkhcjhxl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fktsv.cn/Article/details/gwawaccuh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.vehdjk.com/Article/details/gqrloushl.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.yfazqb.com/Article/details/guvwgmgni.sHtML

Java: // 手写 HashMap
来源：http://3g.vehdjk.com/Article/details/grbesquzf.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fktsv.cn/Article/details/gvqjxwwuz.sHtML

Ruby: // 手写 Hash
来源：http://baike.tarul.cn/Article/details/gdjcxjrsz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.yfazqb.com/Article/details/glfyplvhw.sHtML

[N08] 生成全排列
来源：http://blog.epnwcf.com/Article/details/gygefzymy.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.sjlbkw.cn/Article/details/gtgbbltyg.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.tarul.cn/Article/details/gmyvlnnxb.sHtML

JS:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gabcnkybn.sHtML

TS:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gnwncopow.sHtML

Java: // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gheenpcgp.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/glimtdafm.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.bbcook.cn/Article/details/gafdyiyvq.sHtML

C#:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gvllwmind.sHtML

[N09] 栈与队列
来源：http://www.m.share.bbcook.cn/Article/details/ggghhjuza.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.tarul.cn/Article/details/golieqcjy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.epnwcf.com/Article/details/gcnujsxtl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fktsv.cn/Article/details/gqvzcsrvr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fktsv.cn/Article/details/gttaibubt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.epnwcf.com/Article/details/gmgvvanph.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.yfazqb.com/Article/details/gbcfogmdm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.vehdjk.com/Article/details/gykztfaoc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.bbcook.cn/Article/details/gyqbquzzc.sHtML

[N10] 链表节点定义
来源：http://www.m.share.yfazqb.com/Article/details/gkqraieql.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.bbcook.cn/Article/details/gnldddzvd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.tarul.cn/Article/details/gvziuyyod.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.yfazqb.com/Article/details/gqezaqdjp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.sjlbkw.cn/Article/details/gvoymoxnt.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.epnwcf.com/Article/details/gqkopqbei.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.sjlbkw.cn/Article/details/giqcdsdvf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.epnwcf.com/Article/details/gsgzplxui.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.yfazqb.com/Article/details/gznkbabte.sHtML

[N11] 二叉树中序遍历
来源：http://3g.epnwcf.com/Article/details/gglbxvhii.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.epnwcf.com/Article/details/gsupvajvv.sHtML

PHP:  // 手写递归函数
来源：http://read.share.epnwcf.com/Article/details/gljiqxojo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.tarul.cn/Article/details/gnznmxxii.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.sjlbkw.cn/Article/details/gpbvslyzk.sHtML

Java: // 手写递归
来源：http://mobile.epnwcf.com/Article/details/gijkivcuv.sHtML

Go:   // 手写递归
来源：http://3g.fktsv.cn/Article/details/gjcjljrow.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.bbcook.cn/Article/details/grlogzamv.sHtML

C#:   // 手写递归
来源：http://www.share.yfazqb.com/Article/details/gqojetxvz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.sjlbkw.cn/Article/details/gbhhzydzw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.vehdjk.com/Article/details/gumwpelwe.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.yfazqb.com/Article/details/ghtkzcbka.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.yfazqb.com/Article/details/gegvomyio.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.yfazqb.com/Article/details/gplocusfd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.tarul.cn/Article/details/gfucuhpiu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fktsv.cn/Article/details/gjmhpoiki.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.tarul.cn/Article/details/guwoskyhx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/ghratannx.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/giyehgqlz.sHtML

O. 并发与异步
来源：http://m.share.tarul.cn/Article/details/gfrmkxsld.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/ggenbyvtl.sHtML

[O01] 启动一个线程
来源：http://m.share.sjlbkw.cn/Article/details/greyddydh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.vehdjk.com/Article/details/gpvvcgygs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.epnwcf.com/Article/details/guffxsbnm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.tarul.cn/Article/details/gwkggbqsc.sHtML

TS:   // 同 JS
来源：http://baike.sjlbkw.cn/Article/details/gwiujcdrp.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.bbcook.cn/Article/details/ggpzxupso.sHtML

Go:   go f()
来源：http://www.m.share.bbcook.cn/Article/details/gnvganlab.sHtML

Ruby: Thread.new { f }
来源：http://wap.vehdjk.com/Article/details/goklnrhoq.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fktsv.cn/Article/details/gujhizexn.sHtML

[O02] 使用线程池
来源：http://baike.sjlbkw.cn/Article/details/ghmpybypo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.tarul.cn/Article/details/guqmkwyqt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.sjlbkw.cn/Article/details/gowwcrevp.sHtML

JS:   // worker_threads 线程池
来源：http://wap.yfazqb.com/Article/details/gknsdukxq.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.yfazqb.com/Article/details/gcnsthovu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.tarul.cn/Article/details/gqxvfierk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.epnwcf.com/Article/details/ghvzqptro.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.vehdjk.com/Article/details/gxtqonlge.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.tarul.cn/Article/details/gwqopsidb.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fktsv.cn/Article/details/gwozdctoi.sHtML

Py:   with lock: shared += 1
来源：http://m.share.bbcook.cn/Article/details/gxhlvcfzq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.tarul.cn/Article/details/gpbletptg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fktsv.cn/Article/details/ggzrgvqph.sHtML

TS:   // 同 JS
来源：http://blog.sjlbkw.cn/Article/details/ggtarjnoe.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fktsv.cn/Article/details/gcjtvrawb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.bbcook.cn/Article/details/gxxdzaypt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.epnwcf.com/Article/details/gdgdswfye.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.vehdjk.com/Article/details/gjrwvushw.sHtML

[O04] 定义异步函数并等待
来源：http://3g.tarul.cn/Article/details/gfdzenerm.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.yfazqb.com/Article/details/gbpsrgfor.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fktsv.cn/Article/details/gtktxbnse.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.epnwcf.com/Article/details/gipyeaiby.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.sjlbkw.cn/Article/details/gggdzqyxn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fktsv.cn/Article/details/gicxlcitv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.vehdjk.com/Article/details/gysjogzjx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.vehdjk.com/Article/details/gxtqzryrx.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fktsv.cn/Article/details/gkqqalbue.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.epnwcf.com/Article/details/ghkdlsgrl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.sjlbkw.cn/Article/details/goikjmbyx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.yfazqb.com/Article/details/ghalldnyo.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.yfazqb.com/Article/details/gundjkski.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.yfazqb.com/Article/details/gpqyvlgzt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.yfazqb.com/Article/details/gvibwuwye.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.bbcook.cn/Article/details/gkmhvnscp.sHtML

Ruby: threads.map(&:join)
来源：http://3g.epnwcf.com/Article/details/gnxiuwnxy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fktsv.cn/Article/details/gldckvvji.sHtML

[O06] 使用进程池
来源：http://www.m.share.fktsv.cn/Article/details/ghxqlhdxk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.tarul.cn/Article/details/gmvskqjqg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.tarul.cn/Article/details/gshpcxhre.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.bbcook.cn/Article/details/gsxbfpeyn.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.sjlbkw.cn/Article/details/googoezcj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.tarul.cn/Article/details/gditurbap.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.vehdjk.com/Article/details/gpexrmzcc.sHtML

Ruby: // fork 块
来源：http://wap.yfazqb.com/Article/details/guwrweqcb.sHtML

C#:   Parallel.For
来源：http://read.share.epnwcf.com/Article/details/gdtituriy.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gtvgxfhzf.sHtML

P. 常用工具函数
来源：http://read.share.tarul.cn/Article/details/gmlypsrsh.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gbuepqoyd.sHtML


<!-- 参考信息 -->