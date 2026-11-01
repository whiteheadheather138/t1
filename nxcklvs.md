代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.tarul.cn/Article/details/gpzfhnqfl.sHtML

[L04] 设置超时
来源：http://www.share.epnwcf.com/Article/details/gyulhtbgj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.epnwcf.com/Article/details/gvjagrsct.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.bbcook.cn/Article/details/gjtepplqy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.tarul.cn/Article/details/gixyguilp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fktsv.cn/Article/details/gtsageazq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.sjlbkw.cn/Article/details/gdybcwphi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.yfazqb.com/Article/details/grbesgqbc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.bbcook.cn/Article/details/gomwinwve.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.epnwcf.com/Article/details/gznqsfqrv.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.sjlbkw.cn/Article/details/gieccajlt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.epnwcf.com/Article/details/gfkhbscfk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.sjlbkw.cn/Article/details/gmexpmjhv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.vehdjk.com/Article/details/gkbovecmc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.tarul.cn/Article/details/ghduuwfpu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.bbcook.cn/Article/details/gohikmlnb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.sjlbkw.cn/Article/details/goqzckmzp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.vehdjk.com/Article/details/gxzdsrvza.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fktsv.cn/Article/details/gwpwqezlv.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.vehdjk.com/Article/details/gvgmbaptd.sHtML

Py:   resp.json()
来源：http://wap.tarul.cn/Article/details/gkkgygfue.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.sjlbkw.cn/Article/details/gcnuyycos.sHtML

JS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/giwuhscbo.sHtML

TS:   await resp.json()
来源：http://www.m.share.vehdjk.com/Article/details/gqmtcjotn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.vehdjk.com/Article/details/gemuezkmd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.tarul.cn/Article/details/gjzghwyyf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.tarul.cn/Article/details/gdyylbdxt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.sjlbkw.cn/Article/details/glxnwvmck.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.vehdjk.com/Article/details/gvflogwuo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.sjlbkw.cn/Article/details/gyzbfdraw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.sjlbkw.cn/Article/details/gaqudzjvp.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.tarul.cn/Article/details/gllrttvgq.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.yfazqb.com/Article/details/gillhrsgk.sHtML

Java: resp.statusCode()
来源：http://blog.fktsv.cn/Article/details/gnapckpkl.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.vehdjk.com/Article/details/gbhtvtwcn.sHtML

Ruby: resp.code.to_i
来源：http://blog.yfazqb.com/Article/details/guniolrtv.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.yfazqb.com/Article/details/gauzcqvqs.sHtML

[L08] 并发请求多个地址
来源：http://www.share.sjlbkw.cn/Article/details/gmzsuqlha.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fktsv.cn/Article/details/gcopglnaq.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.yfazqb.com/Article/details/gceyraubz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fktsv.cn/Article/details/godukpxmg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.epnwcf.com/Article/details/gqghmhjvh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.tarul.cn/Article/details/gocrubzqa.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.sjlbkw.cn/Article/details/gthhxogbv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.epnwcf.com/Article/details/gchpzkmud.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gzybmsxvf.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gadzezmtv.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fktsv.cn/Article/details/gypptzmyx.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gyuzjylul.sHtML

[M01] 读取命令行参数
来源：http://www.blog.sjlbkw.cn/Article/details/gkweuffvp.sHtML

Py:   sys.argv[1:]
来源：http://www.share.bbcook.cn/Article/details/gqpvqhfkz.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.vehdjk.com/Article/details/glaycwzks.sHtML

JS:   process.argv.slice(2)
来源：http://3g.bbcook.cn/Article/details/gxegmsrtl.sHtML

TS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/grhbpulia.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fktsv.cn/Article/details/gyvndjziu.sHtML

Go:   os.Args[1:]
来源：http://m.share.yfazqb.com/Article/details/gdniepdyj.sHtML

Ruby: ARGV
来源：http://www.blog.tarul.cn/Article/details/gwwxqnfiv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.bbcook.cn/Article/details/giuanojja.sHtML

[M02] 读取环境变量
来源：http://mobile.tarul.cn/Article/details/greadrjgt.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.epnwcf.com/Article/details/gmrqujnnx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.bbcook.cn/Article/details/gcicoqeda.sHtML

JS:   process.env.HOME
来源：http://www.share.tarul.cn/Article/details/galtqdffv.sHtML

TS:   process.env.HOME
来源：http://baike.tarul.cn/Article/details/gypnjokbu.sHtML

Java: System.getenv("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/goltscyfa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.sjlbkw.cn/Article/details/gfzepkrvu.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.epnwcf.com/Article/details/gmfzznbfl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.yfazqb.com/Article/details/ghrqjaszq.sHtML

[M03] 执行外部命令
来源：http://read.share.bbcook.cn/Article/details/grscokhgk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.epnwcf.com/Article/details/gnwzxrtbh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.yfazqb.com/Article/details/gstkxwgpe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.epnwcf.com/Article/details/gqacpvokv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.epnwcf.com/Article/details/gdzozzbiy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.epnwcf.com/Article/details/gdjqtamvy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.tarul.cn/Article/details/grlyaajcs.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.epnwcf.com/Article/details/gscedoifu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fktsv.cn/Article/details/gcnhtavpm.sHtML

[M04] 获取当前工作目录
来源：http://m.share.vehdjk.com/Article/details/gixfnhcod.sHtML

Py:   os.getcwd()
来源：http://m.share.sjlbkw.cn/Article/details/gyzotxaey.sHtML

PHP:  getcwd();
来源：http://www.m.share.vehdjk.com/Article/details/gjhabbpwh.sHtML

JS:   process.cwd()
来源：http://blog.epnwcf.com/Article/details/gbpcvrvdu.sHtML

TS:   process.cwd()
来源：http://www.share.sjlbkw.cn/Article/details/gkxkwuexn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.tarul.cn/Article/details/gartxchmz.sHtML

Go:   os.Getwd()
来源：http://www.blog.vehdjk.com/Article/details/gkzqzjfsl.sHtML

Ruby: Dir.pwd
来源：http://wap.fktsv.cn/Article/details/gjetjayuh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fktsv.cn/Article/details/gxvgnczcn.sHtML

[M05] 设置退出码
来源：http://www.blog.tarul.cn/Article/details/ggkqogivv.sHtML

Py:   sys.exit(1)
来源：http://mobile.tarul.cn/Article/details/gtfiixyyu.sHtML

PHP:  exit(1);
来源：http://baike.vehdjk.com/Article/details/ganngimtd.sHtML

JS:   process.exit(1)
来源：http://www.share.fktsv.cn/Article/details/glxapmwpu.sHtML

TS:   process.exit(1)
来源：http://wap.bbcook.cn/Article/details/gbgduwept.sHtML

Java: System.exit(1)
来源：http://baike.yfazqb.com/Article/details/gvlgfecmd.sHtML

Go:   os.Exit(1)
来源：http://baike.yfazqb.com/Article/details/gorbazexd.sHtML

Ruby: exit 1
来源：http://blog.fktsv.cn/Article/details/gdkzfssbg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.bbcook.cn/Article/details/gysqdlsyw.sHtML

[M06] 向标准错误输出
来源：http://3g.sjlbkw.cn/Article/details/gebycitus.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.yfazqb.com/Article/details/gndtfqemy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.yfazqb.com/Article/details/glcsadchn.sHtML

JS:   console.error("err")
来源：http://wap.bbcook.cn/Article/details/gyyxhlgzo.sHtML

TS:   console.error("err")
来源：http://www.blog.yfazqb.com/Article/details/gqlfxwfxq.sHtML

Java: System.err.println("err")
来源：http://baike.epnwcf.com/Article/details/gkyvedzfw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.sjlbkw.cn/Article/details/gezwwpxmj.sHtML

Ruby: warn "err"
来源：http://blog.sjlbkw.cn/Article/details/gacnnbece.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.sjlbkw.cn/Article/details/gbthurcla.sHtML

[M07] 判断是否为主入口
来源：http://wap.yfazqb.com/Article/details/gfvstsgrt.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.bbcook.cn/Article/details/gjvalechm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.tarul.cn/Article/details/gyitzhlwq.sHtML

JS:   require.main === module
来源：http://mobile.fktsv.cn/Article/details/guepswttb.sHtML

TS:   require.main === module
来源：http://www.share.tarul.cn/Article/details/gtdlvmzhf.sHtML

Java: public static void main(String[] args)
来源：http://baike.fktsv.cn/Article/details/gjxjboiwu.sHtML

Go:   func main()
来源：http://read.share.sjlbkw.cn/Article/details/gpyesyntk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.sjlbkw.cn/Article/details/gzaivvqdl.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.tarul.cn/Article/details/gevzspbmv.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.vehdjk.com/Article/details/ggtancyaf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.yfazqb.com/Article/details/gxvhpxboj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.tarul.cn/Article/details/gnxsgwxnz.sHtML

JS:   process.platform;  process.version
来源：http://baike.yfazqb.com/Article/details/gfirtholx.sHtML

TS:   process.platform;  process.version
来源：http://read.share.bbcook.cn/Article/details/gkskymwki.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.sjlbkw.cn/Article/details/gsnjecojq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fktsv.cn/Article/details/gsrfkvpty.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.epnwcf.com/Article/details/gxsrppuri.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.yfazqb.com/Article/details/gnvhtwidk.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gnmachzvn.sHtML

N. 数据结构与算法
来源：http://3g.fktsv.cn/Article/details/gsrziqeqz.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gbryhgxex.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.sjlbkw.cn/Article/details/gtuaccpcn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fktsv.cn/Article/details/gycxcjhgk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.vehdjk.com/Article/details/gkakqltlr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fktsv.cn/Article/details/gqwvljyks.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gbdmlyley.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.epnwcf.com/Article/details/gglaepkub.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fktsv.cn/Article/details/gcnkekyod.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.tarul.cn/Article/details/gfrzdibsm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fktsv.cn/Article/details/ggsngpjhg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.epnwcf.com/Article/details/gtlyyzbdr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.bbcook.cn/Article/details/gmacbnfom.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fktsv.cn/Article/details/gntoqbxay.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.sjlbkw.cn/Article/details/gwrfgrfkq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/grqrpbqax.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.yfazqb.com/Article/details/gdsqioirg.sHtML

Go:   slices.Sort(arr)
来源：http://wap.bbcook.cn/Article/details/gdrgznovk.sHtML

Ruby: arr.sort
来源：http://3g.tarul.cn/Article/details/gwwgauyys.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.tarul.cn/Article/details/gihqnbbcp.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fktsv.cn/Article/details/gbzhuhcas.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.sjlbkw.cn/Article/details/giiwkmhqu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.yfazqb.com/Article/details/gskhhkakd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.epnwcf.com/Article/details/gwpzahdqv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fktsv.cn/Article/details/gqiapdyjj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fktsv.cn/Article/details/gpptgmspq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.tarul.cn/Article/details/gqwokjock.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.tarul.cn/Article/details/gmwapswcv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.yfazqb.com/Article/details/gqooqqwtp.sHtML

[N04] 斐波那契数列
来源：http://wap.sjlbkw.cn/Article/details/gslddzzsc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.epnwcf.com/Article/details/gedaezmal.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.yfazqb.com/Article/details/gdgyxfhsh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/gqnqkwmsl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.sjlbkw.cn/Article/details/gcameoqlf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.tarul.cn/Article/details/guhgpottm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fktsv.cn/Article/details/ggfjdmrfr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.bbcook.cn/Article/details/gchaafkkm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.tarul.cn/Article/details/ginrhgrhr.sHtML

[N05] 最大公约数
来源：http://baike.tarul.cn/Article/details/ghpmreray.sHtML

Py:   math.gcd(a, b)
来源：http://blog.vehdjk.com/Article/details/gozhjmwgh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.vehdjk.com/Article/details/gbroomadv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.tarul.cn/Article/details/gcptlyxch.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.vehdjk.com/Article/details/ggmfkqwop.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.tarul.cn/Article/details/gifypcblf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.vehdjk.com/Article/details/gktrwqjmu.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.epnwcf.com/Article/details/guponnevc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.bbcook.cn/Article/details/gxclrjuio.sHtML

[N06] 判断回文字符串
来源：http://mobile.tarul.cn/Article/details/gpqvmkpks.sHtML

Py:   s == s[::-1]
来源：http://blog.vehdjk.com/Article/details/gfikkwevm.sHtML

PHP:  $s === strrev($s);
来源：http://blog.vehdjk.com/Article/details/gfnqmvlwq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gstyhbjzp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/gxlhbffar.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.tarul.cn/Article/details/glnnlejkx.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.sjlbkw.cn/Article/details/gfxvnrkth.sHtML

Ruby: s == s.reverse
来源：http://m.share.bbcook.cn/Article/details/gemflprte.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.epnwcf.com/Article/details/gatygwnnw.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.vehdjk.com/Article/details/gdeaznuvq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.vehdjk.com/Article/details/gfzwnjsqt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fktsv.cn/Article/details/gxztflanr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.epnwcf.com/Article/details/grkuiragt.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.epnwcf.com/Article/details/ggygwftkn.sHtML

Java: // 手写 HashMap
来源：http://www.share.epnwcf.com/Article/details/gkksgaktl.sHtML

Go:   // 手写 map[int]int
来源：http://3g.tarul.cn/Article/details/gidjpkphh.sHtML

Ruby: // 手写 Hash
来源：http://3g.epnwcf.com/Article/details/glmqakrmf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.vehdjk.com/Article/details/gqnflhhyv.sHtML

[N08] 生成全排列
来源：http://3g.vehdjk.com/Article/details/gahugtcaz.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.vehdjk.com/Article/details/ghtpuhyoz.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.yfazqb.com/Article/details/gwoghwefn.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gstrianda.sHtML

TS:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gfpffuovt.sHtML

Java: // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/ganydhlrh.sHtML

Go:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/guumkygpz.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.sjlbkw.cn/Article/details/gghfttuyt.sHtML

C#:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gmmlnquxj.sHtML

[N09] 栈与队列
来源：http://3g.epnwcf.com/Article/details/gwvpfducp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.epnwcf.com/Article/details/gqrtkluqs.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/ggbueaxhe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.yfazqb.com/Article/details/gtwqcymfs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.vehdjk.com/Article/details/gpyaryznt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.epnwcf.com/Article/details/gsvwpjcel.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.vehdjk.com/Article/details/gojfygnec.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.epnwcf.com/Article/details/gbfstzlty.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.vehdjk.com/Article/details/gxqnicago.sHtML

[N10] 链表节点定义
来源：http://www.share.vehdjk.com/Article/details/glfkvbvji.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.vehdjk.com/Article/details/grqchvnyu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.vehdjk.com/Article/details/gyapbmkpb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.bbcook.cn/Article/details/ggpzgnkve.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.epnwcf.com/Article/details/gutrnelil.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fktsv.cn/Article/details/gwpuljgpf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.vehdjk.com/Article/details/grtvdmkex.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.epnwcf.com/Article/details/gvhxvnzqg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.sjlbkw.cn/Article/details/gyohooptz.sHtML

[N11] 二叉树中序遍历
来源：http://baike.sjlbkw.cn/Article/details/gjtfajfyh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.bbcook.cn/Article/details/gemurxhdx.sHtML

PHP:  // 手写递归函数
来源：http://blog.vehdjk.com/Article/details/gwjqhnmmt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.tarul.cn/Article/details/gpyudbtdw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.sjlbkw.cn/Article/details/gexnnojlz.sHtML

Java: // 手写递归
来源：http://blog.yfazqb.com/Article/details/gajsdmfin.sHtML

Go:   // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/gasabvsfu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.yfazqb.com/Article/details/gutyumrgz.sHtML

C#:   // 手写递归
来源：http://3g.vehdjk.com/Article/details/gpzgyienr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.vehdjk.com/Article/details/gfcgwzypr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.bbcook.cn/Article/details/gvskjcrwh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.sjlbkw.cn/Article/details/gsnjbfqdf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.tarul.cn/Article/details/gjfpdrymi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.vehdjk.com/Article/details/gbheahqbo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.yfazqb.com/Article/details/gjceyqvot.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.bbcook.cn/Article/details/gbrgupuxh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.bbcook.cn/Article/details/ghfcpbhch.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.epnwcf.com/Article/details/gegegnizs.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gappikpsu.sHtML

O. 并发与异步
来源：http://baike.yfazqb.com/Article/details/guzbmoxix.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/ggshhjbya.sHtML

[O01] 启动一个线程
来源：http://www.m.share.vehdjk.com/Article/details/gwmbidwio.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.yfazqb.com/Article/details/ggebjrxom.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fktsv.cn/Article/details/gdleokrvt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.tarul.cn/Article/details/gvnttwfee.sHtML

TS:   // 同 JS
来源：http://m.share.tarul.cn/Article/details/gybmmawkl.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.bbcook.cn/Article/details/gueckniug.sHtML

Go:   go f()
来源：http://www.blog.yfazqb.com/Article/details/gaaqoczvo.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.sjlbkw.cn/Article/details/gpdqjbudg.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fktsv.cn/Article/details/gpmpqgpdr.sHtML

[O02] 使用线程池
来源：http://mobile.bbcook.cn/Article/details/gswdfzyjl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.vehdjk.com/Article/details/goiytieus.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.bbcook.cn/Article/details/gghrzljww.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.vehdjk.com/Article/details/gwchtvhph.sHtML

TS:   // worker_threads 线程池
来源：http://blog.bbcook.cn/Article/details/gqbgvncnd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.sjlbkw.cn/Article/details/gofyyuxnf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fktsv.cn/Article/details/gnylnktvm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.bbcook.cn/Article/details/gbsumtyzc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.tarul.cn/Article/details/gddpgjvef.sHtML

[O03] 加锁保护共享数据
来源：http://3g.tarul.cn/Article/details/ghvmzetwa.sHtML

Py:   with lock: shared += 1
来源：http://m.share.tarul.cn/Article/details/gehmhvimv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.epnwcf.com/Article/details/glmogehfw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.vehdjk.com/Article/details/gtibzhyhp.sHtML

TS:   // 同 JS
来源：http://www.share.epnwcf.com/Article/details/gbdbvkfxk.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.bbcook.cn/Article/details/gcbvkgodo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.yfazqb.com/Article/details/gnlizxqtd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.yfazqb.com/Article/details/gcnlvykvg.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.epnwcf.com/Article/details/gtyknlanr.sHtML

[O04] 定义异步函数并等待
来源：http://blog.vehdjk.com/Article/details/gewxjzoqp.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fktsv.cn/Article/details/gymiulysj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.yfazqb.com/Article/details/gfuysiipc.sHtML

JS:   async function f() { await g(); }
来源：http://3g.yfazqb.com/Article/details/gxycoobct.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.epnwcf.com/Article/details/gfzlupkkn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fktsv.cn/Article/details/gfgnrbkay.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.tarul.cn/Article/details/gibstznwp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.tarul.cn/Article/details/ghzemvbmu.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.epnwcf.com/Article/details/gamppcxns.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.vehdjk.com/Article/details/gjfwwcbsh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.yfazqb.com/Article/details/gpbodcfuf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fktsv.cn/Article/details/gsaqiudxr.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.tarul.cn/Article/details/gbktvkszw.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.vehdjk.com/Article/details/glcobkjmg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.epnwcf.com/Article/details/gueyiqmid.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.vehdjk.com/Article/details/gmaqahezb.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fktsv.cn/Article/details/gsffslvby.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.tarul.cn/Article/details/glucyydac.sHtML

[O06] 使用进程池
来源：http://www.blog.tarul.cn/Article/details/gcvlbjkkm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.sjlbkw.cn/Article/details/gawaqnagz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.epnwcf.com/Article/details/ggqfpdhap.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.sjlbkw.cn/Article/details/galnjpsym.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.epnwcf.com/Article/details/gcdorcyij.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.sjlbkw.cn/Article/details/gdkaeflgm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.epnwcf.com/Article/details/gznhchdvc.sHtML

Ruby: // fork 块
来源：http://wap.bbcook.cn/Article/details/gohsftbic.sHtML

C#:   Parallel.For
来源：http://3g.sjlbkw.cn/Article/details/gbzbqkrrh.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gowxkaxtq.sHtML

P. 常用工具函数
来源：http://wap.sjlbkw.cn/Article/details/gwtffkwxk.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gwyjhikhk.sHtML

[P01] 生成 UUID
来源：http://mobile.fktsv.cn/Article/details/gfftfdjau.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fktsv.cn/Article/details/gtiimtaxf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.bbcook.cn/Article/details/gsmsjsslg.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.yfazqb.com/Article/details/gdsgemhrz.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.yfazqb.com/Article/details/gtriaeood.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.sjlbkw.cn/Article/details/gzrtuxebj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.epnwcf.com/Article/details/ghthwyqci.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.bbcook.cn/Article/details/gmsbognpe.sHtML


<!-- 参考信息 -->