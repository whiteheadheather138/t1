代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.vehdjk.com/Article/details/grywhzkdb.sHtML

[L04] 设置超时
来源：http://m.share.tarul.cn/Article/details/ggwfbwxkv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.tarul.cn/Article/details/gofqmfoln.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fktsv.cn/Article/details/gzsuvsuqd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.yfazqb.com/Article/details/guidowrod.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fktsv.cn/Article/details/giacpdjdt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.bbcook.cn/Article/details/gbalejisl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fktsv.cn/Article/details/gkzgposzx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.bbcook.cn/Article/details/gattrkcbq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fktsv.cn/Article/details/gklraqvsr.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fktsv.cn/Article/details/grcvhrcov.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.epnwcf.com/Article/details/grlrboybl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.epnwcf.com/Article/details/gfhnajihm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.sjlbkw.cn/Article/details/gekaykjgn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fktsv.cn/Article/details/gnsahfncb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.tarul.cn/Article/details/gbqzdrfat.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.bbcook.cn/Article/details/ggakmjmny.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.sjlbkw.cn/Article/details/giuxxaeym.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.tarul.cn/Article/details/gdvlspsyg.sHtML

[L06] 解析响应为 JSON
来源：http://3g.tarul.cn/Article/details/grsaujbam.sHtML

Py:   resp.json()
来源：http://mobile.tarul.cn/Article/details/gtreegbct.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.epnwcf.com/Article/details/gfwqeywvc.sHtML

JS:   await resp.json()
来源：http://baike.yfazqb.com/Article/details/gziwnjoip.sHtML

TS:   await resp.json()
来源：http://3g.yfazqb.com/Article/details/guikqztni.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gubsrcmxi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.bbcook.cn/Article/details/gyxnpqzeb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.sjlbkw.cn/Article/details/gtdxalwxk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fktsv.cn/Article/details/gqkqrifll.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.vehdjk.com/Article/details/gfvlcwibt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.tarul.cn/Article/details/geflpfifi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.tarul.cn/Article/details/ghghofiwg.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.yfazqb.com/Article/details/gtlspxkkc.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.sjlbkw.cn/Article/details/gokytnxdv.sHtML

Java: resp.statusCode()
来源：http://www.share.bbcook.cn/Article/details/gmleqijoh.sHtML

Go:   resp.StatusCode
来源：http://3g.yfazqb.com/Article/details/gspcbjdwg.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.vehdjk.com/Article/details/gviyashem.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.tarul.cn/Article/details/gsbpjqifp.sHtML

[L08] 并发请求多个地址
来源：http://m.share.vehdjk.com/Article/details/gqzzesdvx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.bbcook.cn/Article/details/gnbvjjure.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.tarul.cn/Article/details/gxvxnorgg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/ghkdmgfme.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gnjgesbtz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.tarul.cn/Article/details/gcoztupkc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.epnwcf.com/Article/details/gewjjodlq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.yfazqb.com/Article/details/gbduwblsl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fktsv.cn/Article/details/gfhjrkcus.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gpllxvrdi.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fktsv.cn/Article/details/gpornxocv.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gmjullqse.sHtML

[M01] 读取命令行参数
来源：http://wap.bbcook.cn/Article/details/gtzbrdqan.sHtML

Py:   sys.argv[1:]
来源：http://blog.fktsv.cn/Article/details/gcnvdgity.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fktsv.cn/Article/details/gfjmxrltq.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fktsv.cn/Article/details/gvjpcouis.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.yfazqb.com/Article/details/gyptxeqty.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.bbcook.cn/Article/details/gujsiizmj.sHtML

Go:   os.Args[1:]
来源：http://3g.yfazqb.com/Article/details/gsgsvwcsw.sHtML

Ruby: ARGV
来源：http://www.share.sjlbkw.cn/Article/details/gqoiajrrp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.tarul.cn/Article/details/gqgqfydov.sHtML

[M02] 读取环境变量
来源：http://baike.vehdjk.com/Article/details/gxwdtpblo.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.sjlbkw.cn/Article/details/gsctjohyc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fktsv.cn/Article/details/grqekiakj.sHtML

JS:   process.env.HOME
来源：http://read.share.vehdjk.com/Article/details/ghspdhhao.sHtML

TS:   process.env.HOME
来源：http://baike.yfazqb.com/Article/details/gdwmovlqt.sHtML

Java: System.getenv("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/givczefot.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.epnwcf.com/Article/details/gaofmjfhr.sHtML

Ruby: ENV["HOME"]
来源：http://baike.tarul.cn/Article/details/gainywwtc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gtfvqbkbe.sHtML

[M03] 执行外部命令
来源：http://mobile.tarul.cn/Article/details/gbtytqmpc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.epnwcf.com/Article/details/gxsjqfxpt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.bbcook.cn/Article/details/ggwdccjze.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.vehdjk.com/Article/details/guqckgzez.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.sjlbkw.cn/Article/details/gbafywueq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.sjlbkw.cn/Article/details/gjdanywfu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.yfazqb.com/Article/details/gmnjupyhp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.epnwcf.com/Article/details/gzfmppuqa.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.bbcook.cn/Article/details/gdjfufnsz.sHtML

[M04] 获取当前工作目录
来源：http://m.share.epnwcf.com/Article/details/gdafkvtmd.sHtML

Py:   os.getcwd()
来源：http://wap.epnwcf.com/Article/details/gctwrrwxe.sHtML

PHP:  getcwd();
来源：http://read.share.sjlbkw.cn/Article/details/gfnxpptgl.sHtML

JS:   process.cwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/ggtdxsuid.sHtML

TS:   process.cwd()
来源：http://mobile.sjlbkw.cn/Article/details/gicsoqycr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.epnwcf.com/Article/details/gjdpqohwg.sHtML

Go:   os.Getwd()
来源：http://wap.yfazqb.com/Article/details/gjixzkxtm.sHtML

Ruby: Dir.pwd
来源：http://mobile.epnwcf.com/Article/details/gymxpkyjt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fktsv.cn/Article/details/gldjqalrt.sHtML

[M05] 设置退出码
来源：http://www.blog.yfazqb.com/Article/details/gtrronjlf.sHtML

Py:   sys.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gpgaikuul.sHtML

PHP:  exit(1);
来源：http://read.share.tarul.cn/Article/details/gckurhpnb.sHtML

JS:   process.exit(1)
来源：http://m.share.fktsv.cn/Article/details/guolgagdw.sHtML

TS:   process.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gzwaucwwm.sHtML

Java: System.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gjowrfkdv.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gcpscoufa.sHtML

Ruby: exit 1
来源：http://3g.bbcook.cn/Article/details/gnmixepyo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.vehdjk.com/Article/details/grctgmcif.sHtML

[M06] 向标准错误输出
来源：http://read.share.bbcook.cn/Article/details/gohwbszvp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.epnwcf.com/Article/details/gnpipwoym.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.tarul.cn/Article/details/gxkwksald.sHtML

JS:   console.error("err")
来源：http://mobile.fktsv.cn/Article/details/gbqhhveae.sHtML

TS:   console.error("err")
来源：http://baike.tarul.cn/Article/details/gdkjozcva.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fktsv.cn/Article/details/gfdlmpodl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.yfazqb.com/Article/details/gxnyoapwu.sHtML

Ruby: warn "err"
来源：http://www.m.share.epnwcf.com/Article/details/gbremdlxd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.vehdjk.com/Article/details/glrbmwkfn.sHtML

[M07] 判断是否为主入口
来源：http://mobile.sjlbkw.cn/Article/details/gcwumzipe.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.vehdjk.com/Article/details/gytozgqdc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fktsv.cn/Article/details/gpmbxssap.sHtML

JS:   require.main === module
来源：http://read.share.sjlbkw.cn/Article/details/gcpxohkab.sHtML

TS:   require.main === module
来源：http://read.share.vehdjk.com/Article/details/gpscmbjqn.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.yfazqb.com/Article/details/gjuebejas.sHtML

Go:   func main()
来源：http://wap.tarul.cn/Article/details/gfkcnusfl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.bbcook.cn/Article/details/guxvxbrbs.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.sjlbkw.cn/Article/details/gnokwgcfx.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.tarul.cn/Article/details/gbuxrytjn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.epnwcf.com/Article/details/gxzpquiud.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.tarul.cn/Article/details/gxzrwbohl.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.bbcook.cn/Article/details/gbzeipocy.sHtML

TS:   process.platform;  process.version
来源：http://www.share.sjlbkw.cn/Article/details/gguctylyj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.tarul.cn/Article/details/gxilteirm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.bbcook.cn/Article/details/gzoejmelf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.sjlbkw.cn/Article/details/gyeqjdexl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.bbcook.cn/Article/details/gilzdrjup.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gydknqbwy.sHtML

N. 数据结构与算法
来源：http://www.blog.sjlbkw.cn/Article/details/gzvfoikpk.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gdjpizfvd.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.bbcook.cn/Article/details/gximlwwpc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.bbcook.cn/Article/details/gtqsqkljy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdqobidn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.tarul.cn/Article/details/gfedhltrm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.yfazqb.com/Article/details/gsekjujdh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.vehdjk.com/Article/details/gybwyvpwn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fktsv.cn/Article/details/ggjbzraou.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.bbcook.cn/Article/details/gmhlbhdmh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gpqqrnihh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.sjlbkw.cn/Article/details/gativiltd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.tarul.cn/Article/details/glehmbwzq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.bbcook.cn/Article/details/gmadlmqub.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fktsv.cn/Article/details/gbsxftebh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/ghoetvjtk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.sjlbkw.cn/Article/details/gkswnryig.sHtML

Go:   slices.Sort(arr)
来源：http://wap.bbcook.cn/Article/details/gxphgrrap.sHtML

Ruby: arr.sort
来源：http://baike.fktsv.cn/Article/details/gvbjyomjy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.epnwcf.com/Article/details/geetzgkkq.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.epnwcf.com/Article/details/gycxdffeh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.vehdjk.com/Article/details/gbllnfcir.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fktsv.cn/Article/details/gstihqbng.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.vehdjk.com/Article/details/ggfnihswb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.bbcook.cn/Article/details/gizbyqzed.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.epnwcf.com/Article/details/gpqtnmaaw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.sjlbkw.cn/Article/details/gfgpsixqs.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.epnwcf.com/Article/details/gpfqcskaw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.bbcook.cn/Article/details/gqfvzslux.sHtML

[N04] 斐波那契数列
来源：http://read.share.bbcook.cn/Article/details/gfqtqexrx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fktsv.cn/Article/details/godyoxdqw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.yfazqb.com/Article/details/glpxnvqdr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.yfazqb.com/Article/details/gnwqcvqhz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/grftnrqcj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.tarul.cn/Article/details/gcnkdflkj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.yfazqb.com/Article/details/gshathtok.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fktsv.cn/Article/details/gqeetoqdj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.tarul.cn/Article/details/ghdrhthdt.sHtML

[N05] 最大公约数
来源：http://blog.tarul.cn/Article/details/ghjkxzmic.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fktsv.cn/Article/details/groqziaqe.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.yfazqb.com/Article/details/gjoeqgxas.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fktsv.cn/Article/details/gqccvuswk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.sjlbkw.cn/Article/details/gpmlckwax.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.epnwcf.com/Article/details/gbcntzvcz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fktsv.cn/Article/details/gmmwpqpvc.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fktsv.cn/Article/details/gxpctvdtm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.sjlbkw.cn/Article/details/gfqlxwwqp.sHtML

[N06] 判断回文字符串
来源：http://3g.sjlbkw.cn/Article/details/gzuixehyy.sHtML

Py:   s == s[::-1]
来源：http://wap.tarul.cn/Article/details/ggimfjdqu.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.bbcook.cn/Article/details/gojizccbe.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/gnuvlnlqx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gespbzbot.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.yfazqb.com/Article/details/gdlfcjbqk.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fktsv.cn/Article/details/gieusqfcp.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fktsv.cn/Article/details/gmfhndklt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.tarul.cn/Article/details/gzpavgwqp.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.epnwcf.com/Article/details/ggvqbhctt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.vehdjk.com/Article/details/gsijuluuz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.tarul.cn/Article/details/golwheaxy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.tarul.cn/Article/details/gjynulbqz.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.yfazqb.com/Article/details/gcdmdjroq.sHtML

Java: // 手写 HashMap
来源：http://mobile.vehdjk.com/Article/details/gdpglxoao.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fktsv.cn/Article/details/gyeulzgzj.sHtML

Ruby: // 手写 Hash
来源：http://read.share.epnwcf.com/Article/details/gfumymvcu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.sjlbkw.cn/Article/details/gjhdbybty.sHtML

[N08] 生成全排列
来源：http://baike.yfazqb.com/Article/details/gmaoacfef.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.tarul.cn/Article/details/gaxqsvwys.sHtML

PHP:  // 手写递归交换
来源：http://read.share.yfazqb.com/Article/details/gimnbujub.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gnhviyyhz.sHtML

TS:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gbldydoyx.sHtML

Java: // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/guubunsmj.sHtML

Go:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gdkmwbxbn.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.vehdjk.com/Article/details/gjgjuxrqv.sHtML

C#:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gmdlpwrke.sHtML

[N09] 栈与队列
来源：http://3g.bbcook.cn/Article/details/ghgoazbwr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.bbcook.cn/Article/details/gkmijccqm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fktsv.cn/Article/details/godxucftp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gtumkxcct.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.epnwcf.com/Article/details/gyvlogqyg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fktsv.cn/Article/details/gjjaynbor.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.bbcook.cn/Article/details/gqfotyiip.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.epnwcf.com/Article/details/gugksaiuy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.sjlbkw.cn/Article/details/gcoyerxsp.sHtML

[N10] 链表节点定义
来源：http://baike.tarul.cn/Article/details/gxzeuxfvh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.epnwcf.com/Article/details/ggdppfgfx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.vehdjk.com/Article/details/gihlvabno.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.vehdjk.com/Article/details/gkqfvrolg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.vehdjk.com/Article/details/gadpmnewb.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.tarul.cn/Article/details/gmbgplohu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.epnwcf.com/Article/details/gdixotthz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.bbcook.cn/Article/details/gleisimom.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.yfazqb.com/Article/details/gacvjqkiq.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.yfazqb.com/Article/details/gwsnyepvp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.sjlbkw.cn/Article/details/gltzmjfrf.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.vehdjk.com/Article/details/gfqadbglb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fktsv.cn/Article/details/gbmnginvv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.epnwcf.com/Article/details/gzkyxdncc.sHtML

Java: // 手写递归
来源：http://3g.vehdjk.com/Article/details/gkcnccdtx.sHtML

Go:   // 手写递归
来源：http://mobile.fktsv.cn/Article/details/gqhrfzuef.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.yfazqb.com/Article/details/ghyjhnvol.sHtML

C#:   // 手写递归
来源：http://3g.fktsv.cn/Article/details/gbbsomswi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.tarul.cn/Article/details/gkpgbvwze.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.yfazqb.com/Article/details/gxdudfqyp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.epnwcf.com/Article/details/giecizzms.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.tarul.cn/Article/details/genfkylyc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.yfazqb.com/Article/details/gpfvwgdyr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.epnwcf.com/Article/details/gsvcnhfwn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.vehdjk.com/Article/details/giwehvnns.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.yfazqb.com/Article/details/gkpiueoic.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.vehdjk.com/Article/details/gdcdmlktx.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/glheixyrm.sHtML

O. 并发与异步
来源：http://baike.fktsv.cn/Article/details/gvjnswzmy.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gsznyjqts.sHtML

[O01] 启动一个线程
来源：http://wap.epnwcf.com/Article/details/gjxjkpnjb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.sjlbkw.cn/Article/details/gklkonrgr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.sjlbkw.cn/Article/details/gusskqplk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.tarul.cn/Article/details/gdsptwgqf.sHtML

TS:   // 同 JS
来源：http://wap.bbcook.cn/Article/details/gskveyxeh.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.epnwcf.com/Article/details/gdwjmhgiy.sHtML

Go:   go f()
来源：http://3g.bbcook.cn/Article/details/gicnclvjl.sHtML

Ruby: Thread.new { f }
来源：http://3g.sjlbkw.cn/Article/details/gxlhprupm.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.vehdjk.com/Article/details/guixfomni.sHtML

[O02] 使用线程池
来源：http://baike.tarul.cn/Article/details/gmnasavec.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.tarul.cn/Article/details/gunfgvbss.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.yfazqb.com/Article/details/glkcuonzm.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.bbcook.cn/Article/details/gikdpegzs.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fktsv.cn/Article/details/gxserrksa.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.yfazqb.com/Article/details/ghehuzknz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.vehdjk.com/Article/details/gghqmwtxm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.tarul.cn/Article/details/gmpgewunk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fktsv.cn/Article/details/gopxcwrwr.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.bbcook.cn/Article/details/gdybefgev.sHtML

Py:   with lock: shared += 1
来源：http://mobile.sjlbkw.cn/Article/details/gxbfhtnct.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.bbcook.cn/Article/details/gujmaweok.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.sjlbkw.cn/Article/details/gpvxabmdb.sHtML

TS:   // 同 JS
来源：http://3g.vehdjk.com/Article/details/gjjuqyavb.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.tarul.cn/Article/details/gwhzeowfh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.yfazqb.com/Article/details/ggagtkkcc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.epnwcf.com/Article/details/gurizgpnw.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.vehdjk.com/Article/details/gnpcifito.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.yfazqb.com/Article/details/geodwylgr.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fktsv.cn/Article/details/gcvafoqtf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.tarul.cn/Article/details/gyadqalgm.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.tarul.cn/Article/details/gptoxdosi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.tarul.cn/Article/details/godaevphf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.sjlbkw.cn/Article/details/gqrjpgyeu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fktsv.cn/Article/details/gwchcqaeg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.epnwcf.com/Article/details/gzliyyfnu.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.vehdjk.com/Article/details/ghdwefhrn.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.epnwcf.com/Article/details/gckzadoyc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.bbcook.cn/Article/details/gbvujpwdz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.vehdjk.com/Article/details/gqzysnvwd.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.vehdjk.com/Article/details/gxrktyrlo.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.vehdjk.com/Article/details/gebjzlunb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.epnwcf.com/Article/details/guysluknm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.yfazqb.com/Article/details/gkerweamq.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fktsv.cn/Article/details/gqnbjyzga.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fktsv.cn/Article/details/gwazfxplw.sHtML

[O06] 使用进程池
来源：http://www.m.share.vehdjk.com/Article/details/gabqbfwth.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.sjlbkw.cn/Article/details/ghjbxwhaf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.bbcook.cn/Article/details/ghuucpuuw.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.tarul.cn/Article/details/guihxcsoa.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fktsv.cn/Article/details/geciiyyky.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.bbcook.cn/Article/details/gvvdyrnmt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.epnwcf.com/Article/details/gdrzaijsj.sHtML

Ruby: // fork 块
来源：http://blog.tarul.cn/Article/details/ggypjkjrp.sHtML

C#:   Parallel.For
来源：http://m.share.epnwcf.com/Article/details/girfxcbbv.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gsfgqkbng.sHtML

P. 常用工具函数
来源：http://blog.sjlbkw.cn/Article/details/goolejhiv.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/galbjltbz.sHtML

[P01] 生成 UUID
来源：http://mobile.sjlbkw.cn/Article/details/gvoqargbj.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.bbcook.cn/Article/details/gutfnsxog.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.epnwcf.com/Article/details/gcyfictyu.sHtML

JS:   crypto.randomUUID()
来源：http://wap.bbcook.cn/Article/details/gjjmcoxws.sHtML

TS:   crypto.randomUUID()
来源：http://wap.epnwcf.com/Article/details/gyyxswhpw.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.yfazqb.com/Article/details/gjgirfmdg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.sjlbkw.cn/Article/details/ghwzjcfws.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.vehdjk.com/Article/details/gnuqntstu.sHtML


<!-- 参考信息 -->