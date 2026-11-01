代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.sjlbkw.cn/Article/details/gwujydyqn.sHtML

[L04] 设置超时
来源：http://3g.bbcook.cn/Article/details/gjyyxtftr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.tarul.cn/Article/details/ggtsrsvia.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.bbcook.cn/Article/details/gdlrugyfd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.tarul.cn/Article/details/gxqulbejh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.sjlbkw.cn/Article/details/gtzgpwoqj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.yfazqb.com/Article/details/gitmdusas.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.yfazqb.com/Article/details/gylrkbjox.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.tarul.cn/Article/details/gpsdqcaoh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.tarul.cn/Article/details/givaukhls.sHtML

[L05] 上传文件（multipart）
来源：http://3g.tarul.cn/Article/details/gesnialwn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.epnwcf.com/Article/details/gzwtdllua.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.vehdjk.com/Article/details/gimrgzrpb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.bbcook.cn/Article/details/gvlcvihdz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.sjlbkw.cn/Article/details/gnazemwxz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.vehdjk.com/Article/details/gusnqlzhi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.sjlbkw.cn/Article/details/gahelpawi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.yfazqb.com/Article/details/gpjdicjuc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fktsv.cn/Article/details/gyzazlkgd.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.vehdjk.com/Article/details/gilzgrbab.sHtML

Py:   resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/ggezhokfb.sHtML

PHP:  json_decode($body, true);
来源：http://blog.bbcook.cn/Article/details/gsxtmrsyz.sHtML

JS:   await resp.json()
来源：http://blog.sjlbkw.cn/Article/details/gzlszgcrz.sHtML

TS:   await resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/godcjgkoc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.yfazqb.com/Article/details/gtpoiaxax.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.sjlbkw.cn/Article/details/gfhwksumw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.vehdjk.com/Article/details/gyzkspmby.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.vehdjk.com/Article/details/geufjeobd.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.vehdjk.com/Article/details/gkltpdouj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.sjlbkw.cn/Article/details/gminpygpc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.sjlbkw.cn/Article/details/gmoqfufqn.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.bbcook.cn/Article/details/gdrhnhhzi.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.yfazqb.com/Article/details/ghbdclhef.sHtML

Java: resp.statusCode()
来源：http://baike.tarul.cn/Article/details/gtlebkned.sHtML

Go:   resp.StatusCode
来源：http://mobile.tarul.cn/Article/details/gyacsfvkp.sHtML

Ruby: resp.code.to_i
来源：http://read.share.bbcook.cn/Article/details/gzyzxiuki.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fktsv.cn/Article/details/glhimbarn.sHtML

[L08] 并发请求多个地址
来源：http://mobile.bbcook.cn/Article/details/giqqtbgcp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.vehdjk.com/Article/details/gkosexmmh.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.yfazqb.com/Article/details/gampexgeh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.yfazqb.com/Article/details/gygdavguc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.yfazqb.com/Article/details/gxanemlww.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.sjlbkw.cn/Article/details/gxpdekcdb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.vehdjk.com/Article/details/ganoqodkf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.yfazqb.com/Article/details/gvmlqqyoq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.epnwcf.com/Article/details/groogywrr.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gkjhehvah.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.epnwcf.com/Article/details/gddogescy.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gjnypdupy.sHtML

[M01] 读取命令行参数
来源：http://blog.bbcook.cn/Article/details/gamnrkmgr.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.epnwcf.com/Article/details/gjddgvmrp.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.epnwcf.com/Article/details/gmkmusccs.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.tarul.cn/Article/details/giprwsvzq.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.yfazqb.com/Article/details/guupovxat.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.sjlbkw.cn/Article/details/gdddrgbcg.sHtML

Go:   os.Args[1:]
来源：http://mobile.epnwcf.com/Article/details/gzwfcdgvl.sHtML

Ruby: ARGV
来源：http://3g.vehdjk.com/Article/details/gdhydboon.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.tarul.cn/Article/details/galdpdqna.sHtML

[M02] 读取环境变量
来源：http://www.blog.bbcook.cn/Article/details/gundiyugj.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.sjlbkw.cn/Article/details/guodpmnxy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.tarul.cn/Article/details/guaprhkio.sHtML

JS:   process.env.HOME
来源：http://www.share.sjlbkw.cn/Article/details/gxjuiypcu.sHtML

TS:   process.env.HOME
来源：http://blog.tarul.cn/Article/details/gwpdxlycu.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fktsv.cn/Article/details/goilgmryo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.vehdjk.com/Article/details/ghqqhdsog.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.vehdjk.com/Article/details/gyuxzcsoz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.tarul.cn/Article/details/gxyxvwmmk.sHtML

[M03] 执行外部命令
来源：http://3g.yfazqb.com/Article/details/gpagbvxlk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fktsv.cn/Article/details/ggiddbnnf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fktsv.cn/Article/details/gfysxukdv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.vehdjk.com/Article/details/gxxfiopnt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.bbcook.cn/Article/details/gkfcgfznh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.bbcook.cn/Article/details/gvyfpkvuv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.epnwcf.com/Article/details/gbguayzaj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.epnwcf.com/Article/details/gttscccci.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fktsv.cn/Article/details/gkenznvax.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fktsv.cn/Article/details/govhzpqnr.sHtML

Py:   os.getcwd()
来源：http://www.blog.yfazqb.com/Article/details/geuizrktr.sHtML

PHP:  getcwd();
来源：http://www.blog.vehdjk.com/Article/details/gmazeibha.sHtML

JS:   process.cwd()
来源：http://baike.tarul.cn/Article/details/gaebaymuq.sHtML

TS:   process.cwd()
来源：http://mobile.epnwcf.com/Article/details/gcrpoeqgq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.epnwcf.com/Article/details/gzpwtrobx.sHtML

Go:   os.Getwd()
来源：http://www.share.tarul.cn/Article/details/gcwburcpm.sHtML

Ruby: Dir.pwd
来源：http://m.share.vehdjk.com/Article/details/ghzpldlfz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.vehdjk.com/Article/details/gaumojlys.sHtML

[M05] 设置退出码
来源：http://read.share.bbcook.cn/Article/details/gkzembmjy.sHtML

Py:   sys.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/guucaempo.sHtML

PHP:  exit(1);
来源：http://www.m.share.fktsv.cn/Article/details/gqibyteka.sHtML

JS:   process.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gylglpfhu.sHtML

TS:   process.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gfoxfyldp.sHtML

Java: System.exit(1)
来源：http://3g.tarul.cn/Article/details/gouxsfocw.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gtwycfwvn.sHtML

Ruby: exit 1
来源：http://www.m.share.bbcook.cn/Article/details/gjbdvzuja.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.epnwcf.com/Article/details/gdkochomd.sHtML

[M06] 向标准错误输出
来源：http://baike.tarul.cn/Article/details/gfljpdooy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.sjlbkw.cn/Article/details/grepvvhlk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.bbcook.cn/Article/details/gqntsxxvl.sHtML

JS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/gpomchgzs.sHtML

TS:   console.error("err")
来源：http://m.share.bbcook.cn/Article/details/grnyozxuf.sHtML

Java: System.err.println("err")
来源：http://www.blog.vehdjk.com/Article/details/glfkxnuww.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.bbcook.cn/Article/details/gypjlviol.sHtML

Ruby: warn "err"
来源：http://blog.epnwcf.com/Article/details/ggktjgqxq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fktsv.cn/Article/details/gnkwadmsg.sHtML

[M07] 判断是否为主入口
来源：http://baike.vehdjk.com/Article/details/gdrtzdzbc.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.epnwcf.com/Article/details/gkpblxwbq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.bbcook.cn/Article/details/gwpqqcqaq.sHtML

JS:   require.main === module
来源：http://3g.yfazqb.com/Article/details/guazksaye.sHtML

TS:   require.main === module
来源：http://m.share.yfazqb.com/Article/details/gsukevvwz.sHtML

Java: public static void main(String[] args)
来源：http://mobile.vehdjk.com/Article/details/glvdsmfyn.sHtML

Go:   func main()
来源：http://mobile.yfazqb.com/Article/details/gfiurcnen.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.tarul.cn/Article/details/glpakzvbw.sHtML

C#:   static void Main(string[] args)
来源：http://wap.epnwcf.com/Article/details/geyyswwlq.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.yfazqb.com/Article/details/ggtdypona.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.yfazqb.com/Article/details/gobtvifyi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.vehdjk.com/Article/details/gguhvymkc.sHtML

JS:   process.platform;  process.version
来源：http://www.share.epnwcf.com/Article/details/gcvbgrhgm.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fktsv.cn/Article/details/ghplawlqn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.vehdjk.com/Article/details/gbckftkuo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.epnwcf.com/Article/details/gdttvlkhu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.tarul.cn/Article/details/goonqrtdh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.vehdjk.com/Article/details/gneeksoki.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/ghhjqxdhi.sHtML

N. 数据结构与算法
来源：http://3g.vehdjk.com/Article/details/gpkpcfnaa.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gpvbgxnwc.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.vehdjk.com/Article/details/gzgqejwvk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gtcrvotui.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fktsv.cn/Article/details/gzaonqtxh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.tarul.cn/Article/details/ghkdgamzs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.epnwcf.com/Article/details/gsyjkiidj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.bbcook.cn/Article/details/grzqxayhm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.vehdjk.com/Article/details/gysjdxdwx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.bbcook.cn/Article/details/ggjwjnckc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.tarul.cn/Article/details/gfhjlmjga.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.yfazqb.com/Article/details/gvlrjrvdz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.bbcook.cn/Article/details/gugkijomn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.vehdjk.com/Article/details/gwdnhiodv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.yfazqb.com/Article/details/gexftnsto.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/gestedywt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fktsv.cn/Article/details/gicltgpdl.sHtML

Go:   slices.Sort(arr)
来源：http://baike.yfazqb.com/Article/details/gyoedmmci.sHtML

Ruby: arr.sort
来源：http://mobile.yfazqb.com/Article/details/gsrndxifj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fktsv.cn/Article/details/gtrnqxxqd.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.sjlbkw.cn/Article/details/gfvjfttgz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.tarul.cn/Article/details/gmvvvodqy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.yfazqb.com/Article/details/gykyztlbc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.vehdjk.com/Article/details/geqznuzfu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.tarul.cn/Article/details/gmuusjdlx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.epnwcf.com/Article/details/gaknjazqm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.vehdjk.com/Article/details/giyxooiio.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.tarul.cn/Article/details/gjbkpdjwc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.epnwcf.com/Article/details/gneyccntp.sHtML

[N04] 斐波那契数列
来源：http://www.blog.tarul.cn/Article/details/gdpvtjcsx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fktsv.cn/Article/details/gtveujxyh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.bbcook.cn/Article/details/gctrqpqnv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/ggsanibxl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/ghsmvtwse.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.epnwcf.com/Article/details/gmtaejlhe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.tarul.cn/Article/details/gxdztocrr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.bbcook.cn/Article/details/glucdfhcp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/gbchjwfvx.sHtML

[N05] 最大公约数
来源：http://www.share.fktsv.cn/Article/details/guzoimode.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/gzlnzwqrz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.tarul.cn/Article/details/gaigmhizr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.sjlbkw.cn/Article/details/gfppqsvev.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fktsv.cn/Article/details/gjmiwgile.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.yfazqb.com/Article/details/gbbjbnett.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.epnwcf.com/Article/details/gzolcepak.sHtML

Ruby: a.gcd(b)
来源：http://m.share.epnwcf.com/Article/details/gezdrionj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.epnwcf.com/Article/details/gyefshwzp.sHtML

[N06] 判断回文字符串
来源：http://wap.sjlbkw.cn/Article/details/gwgkxjyfr.sHtML

Py:   s == s[::-1]
来源：http://www.blog.vehdjk.com/Article/details/gfwjhifxk.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.bbcook.cn/Article/details/gnvworjih.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gjcnwquuc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gidtmqvnh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.bbcook.cn/Article/details/gdwgkqjzg.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fktsv.cn/Article/details/goadbnkms.sHtML

Ruby: s == s.reverse
来源：http://3g.vehdjk.com/Article/details/gdxgelcgl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.tarul.cn/Article/details/gkyqlyxsm.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fktsv.cn/Article/details/goquyhnvt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.tarul.cn/Article/details/ggcwnmwhv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.sjlbkw.cn/Article/details/goonfnywc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fktsv.cn/Article/details/gfwdlgfst.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.tarul.cn/Article/details/gvomzzytx.sHtML

Java: // 手写 HashMap
来源：http://mobile.tarul.cn/Article/details/gygjiuqxj.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fktsv.cn/Article/details/gwamvhmrp.sHtML

Ruby: // 手写 Hash
来源：http://read.share.epnwcf.com/Article/details/gssciyrji.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.bbcook.cn/Article/details/gpumyjhab.sHtML

[N08] 生成全排列
来源：http://wap.sjlbkw.cn/Article/details/gwimtzqvt.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.bbcook.cn/Article/details/gyqdwbmst.sHtML

PHP:  // 手写递归交换
来源：http://read.share.epnwcf.com/Article/details/gptxbuntx.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gyzlihjgd.sHtML

TS:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gbaspeiqs.sHtML

Java: // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/goheedmrn.sHtML

Go:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/guylccpgu.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.vehdjk.com/Article/details/gfwsdygfm.sHtML

C#:   // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/gjtgtzwul.sHtML

[N09] 栈与队列
来源：http://read.share.yfazqb.com/Article/details/gyoiinsuz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.epnwcf.com/Article/details/gpsrqhzun.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.sjlbkw.cn/Article/details/gwruxgqzl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.vehdjk.com/Article/details/gebpjsuwg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.epnwcf.com/Article/details/ghpxxekiz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.epnwcf.com/Article/details/goppqrxky.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.epnwcf.com/Article/details/gdkhqiigc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.bbcook.cn/Article/details/gevkhekld.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.yfazqb.com/Article/details/gzimcnafj.sHtML

[N10] 链表节点定义
来源：http://wap.vehdjk.com/Article/details/gxnzlzjyj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.yfazqb.com/Article/details/gendbmjhs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.bbcook.cn/Article/details/gvwrzuzem.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.bbcook.cn/Article/details/gziuxzbwf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.vehdjk.com/Article/details/gknmsizgx.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fktsv.cn/Article/details/gondvluzc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.vehdjk.com/Article/details/gjaaerhgy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.tarul.cn/Article/details/gmvagujip.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.vehdjk.com/Article/details/gckokjdfv.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fktsv.cn/Article/details/gqdsomdzx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.yfazqb.com/Article/details/giogdaqjz.sHtML

PHP:  // 手写递归函数
来源：http://m.share.vehdjk.com/Article/details/geglsgyel.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.sjlbkw.cn/Article/details/gdapgxjcz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.tarul.cn/Article/details/gukvdcdsb.sHtML

Java: // 手写递归
来源：http://mobile.tarul.cn/Article/details/gppchzqud.sHtML

Go:   // 手写递归
来源：http://blog.vehdjk.com/Article/details/ggkriiehj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.vehdjk.com/Article/details/gzhvymnic.sHtML

C#:   // 手写递归
来源：http://wap.bbcook.cn/Article/details/gxiuresbr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.bbcook.cn/Article/details/grkfpavqd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.yfazqb.com/Article/details/gdmuajnvg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.yfazqb.com/Article/details/gndrstqbc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fktsv.cn/Article/details/grtdqbzjc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.bbcook.cn/Article/details/gwszdhwqr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.epnwcf.com/Article/details/ggvqywdwr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fktsv.cn/Article/details/gttjacerq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fktsv.cn/Article/details/gyjuzllfi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.sjlbkw.cn/Article/details/gxgztprro.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gpmtjcdrc.sHtML

O. 并发与异步
来源：http://baike.vehdjk.com/Article/details/gfofjeezb.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gutvjcljq.sHtML

[O01] 启动一个线程
来源：http://m.share.fktsv.cn/Article/details/geqvehwbk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.yfazqb.com/Article/details/gdfqivpyc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gfssapuiw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.tarul.cn/Article/details/gttquqldl.sHtML

TS:   // 同 JS
来源：http://m.share.fktsv.cn/Article/details/gkufjzbik.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.bbcook.cn/Article/details/gklajmsff.sHtML

Go:   go f()
来源：http://baike.yfazqb.com/Article/details/gsgrzcwkd.sHtML

Ruby: Thread.new { f }
来源：http://baike.sjlbkw.cn/Article/details/gslygjemn.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.yfazqb.com/Article/details/gosoxalmz.sHtML

[O02] 使用线程池
来源：http://mobile.bbcook.cn/Article/details/gkgkbcpud.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.tarul.cn/Article/details/gzbelxqgl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.vehdjk.com/Article/details/ggblbqcgn.sHtML

JS:   // worker_threads 线程池
来源：http://blog.yfazqb.com/Article/details/gjedgtngc.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.vehdjk.com/Article/details/gjlbyemyp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.vehdjk.com/Article/details/gmmqmzeaw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.epnwcf.com/Article/details/genoaiafg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.tarul.cn/Article/details/gusxoqlyg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fktsv.cn/Article/details/gudwabpmi.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.epnwcf.com/Article/details/ghjkaplix.sHtML

Py:   with lock: shared += 1
来源：http://m.share.vehdjk.com/Article/details/gjbnzafwk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.vehdjk.com/Article/details/gyqwnpiyy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.tarul.cn/Article/details/gqkxdzvkn.sHtML

TS:   // 同 JS
来源：http://www.blog.vehdjk.com/Article/details/gfmcplxnz.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.epnwcf.com/Article/details/gadpkmgos.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fktsv.cn/Article/details/gtkzhndyy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fktsv.cn/Article/details/gthmtxffe.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.bbcook.cn/Article/details/ghiixifzq.sHtML

[O04] 定义异步函数并等待
来源：http://wap.epnwcf.com/Article/details/gsdcnueno.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.vehdjk.com/Article/details/grefmqnqn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.yfazqb.com/Article/details/ganynhifp.sHtML

JS:   async function f() { await g(); }
来源：http://blog.tarul.cn/Article/details/gazmbwykt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.epnwcf.com/Article/details/gailstkvk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.yfazqb.com/Article/details/ganjbxmkv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.vehdjk.com/Article/details/gpqaptqph.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.sjlbkw.cn/Article/details/gcxtxbpcp.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.epnwcf.com/Article/details/gechbycxz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.vehdjk.com/Article/details/gksfadhdm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.bbcook.cn/Article/details/gmoidiovk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.epnwcf.com/Article/details/glwuexshz.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.bbcook.cn/Article/details/gajrdrwpt.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.bbcook.cn/Article/details/gexaeclix.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.yfazqb.com/Article/details/gqrnhnfjt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.sjlbkw.cn/Article/details/gtywdchjo.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghfarhixm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.tarul.cn/Article/details/gdolaetge.sHtML

[O06] 使用进程池
来源：http://m.share.bbcook.cn/Article/details/gldncosle.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.epnwcf.com/Article/details/gcftpaodl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fktsv.cn/Article/details/gjxicehug.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fktsv.cn/Article/details/gevdjkulz.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.epnwcf.com/Article/details/goezgojxl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.sjlbkw.cn/Article/details/giybpjvge.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.vehdjk.com/Article/details/gffowoaeq.sHtML

Ruby: // fork 块
来源：http://m.share.yfazqb.com/Article/details/gfhknjpyf.sHtML

C#:   Parallel.For
来源：http://www.share.bbcook.cn/Article/details/gudcwbhqj.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gsdceipgd.sHtML

P. 常用工具函数
来源：http://m.share.fktsv.cn/Article/details/gxgoclxbn.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gxmpwsgqs.sHtML

[P01] 生成 UUID
来源：http://read.share.vehdjk.com/Article/details/goyfslohv.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.sjlbkw.cn/Article/details/ghtmzbnwa.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.bbcook.cn/Article/details/gqtkwytac.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.tarul.cn/Article/details/gazxgehxe.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/gydinyair.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.epnwcf.com/Article/details/ggommqwey.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.vehdjk.com/Article/details/gikhbornt.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.bbcook.cn/Article/details/ggsmerzsi.sHtML


<!-- 参考信息 -->