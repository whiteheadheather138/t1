代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.vehdjk.com/Article/details/gvhcggxgr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.bbcook.cn/Article/details/gzkdylwyn.sHtML

[L05] 上传文件（multipart）
来源：http://3g.epnwcf.com/Article/details/gfendhthr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.tarul.cn/Article/details/gxorsqovv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.bbcook.cn/Article/details/gqnelofaj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.bbcook.cn/Article/details/gejlrklbe.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.bbcook.cn/Article/details/gxawbzjxe.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.tarul.cn/Article/details/glblxsacu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.vehdjk.com/Article/details/gtavloaud.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.sjlbkw.cn/Article/details/gjezhbiai.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.vehdjk.com/Article/details/gtjjqnwil.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.vehdjk.com/Article/details/gzuhgqbmj.sHtML

Py:   resp.json()
来源：http://blog.bbcook.cn/Article/details/gjpxwlvpa.sHtML

PHP:  json_decode($body, true);
来源：http://baike.epnwcf.com/Article/details/glomixmig.sHtML

JS:   await resp.json()
来源：http://mobile.yfazqb.com/Article/details/ggqvmukyi.sHtML

TS:   await resp.json()
来源：http://www.share.vehdjk.com/Article/details/guibbaxtq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.tarul.cn/Article/details/grslxybur.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.vehdjk.com/Article/details/gckjurqpy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.vehdjk.com/Article/details/gyfbohvwv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.tarul.cn/Article/details/gujvemyoo.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.epnwcf.com/Article/details/gkladojdp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.epnwcf.com/Article/details/gsnmrlqms.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.vehdjk.com/Article/details/grjnuugyn.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fktsv.cn/Article/details/guxrwzflv.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.sjlbkw.cn/Article/details/gwuyidfjd.sHtML

Java: resp.statusCode()
来源：http://www.blog.yfazqb.com/Article/details/grstedqjl.sHtML

Go:   resp.StatusCode
来源：http://baike.tarul.cn/Article/details/ghdkhczzq.sHtML

Ruby: resp.code.to_i
来源：http://blog.bbcook.cn/Article/details/girwphfez.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.yfazqb.com/Article/details/gjmycdlaj.sHtML

[L08] 并发请求多个地址
来源：http://3g.yfazqb.com/Article/details/gkfmirjgg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.tarul.cn/Article/details/gyuqogfrs.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.vehdjk.com/Article/details/gyakuvqqi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/gpkqprteh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.sjlbkw.cn/Article/details/glqmwhydi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.bbcook.cn/Article/details/ghokvfqgj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.bbcook.cn/Article/details/geafkpkyv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.bbcook.cn/Article/details/gbteoyypl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fktsv.cn/Article/details/gmuosqpwu.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ghpuehhfk.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fktsv.cn/Article/details/gwixfgryq.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gggenyvwv.sHtML

[M01] 读取命令行参数
来源：http://www.share.tarul.cn/Article/details/gfbmzlvwa.sHtML

Py:   sys.argv[1:]
来源：http://mobile.yfazqb.com/Article/details/gpflphifg.sHtML

PHP:  $argv;  $argc;
来源：http://3g.yfazqb.com/Article/details/gmdosbrjq.sHtML

JS:   process.argv.slice(2)
来源：http://blog.sjlbkw.cn/Article/details/gogoizuhp.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.bbcook.cn/Article/details/gcyjugmzu.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.tarul.cn/Article/details/gfgkdkfpu.sHtML

Go:   os.Args[1:]
来源：http://www.blog.tarul.cn/Article/details/gikjqecmc.sHtML

Ruby: ARGV
来源：http://wap.sjlbkw.cn/Article/details/gqqbpjeua.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.vehdjk.com/Article/details/ghuvrauys.sHtML

[M02] 读取环境变量
来源：http://m.share.fktsv.cn/Article/details/gmynkudqa.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gjpjhylmx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.yfazqb.com/Article/details/griorijhg.sHtML

JS:   process.env.HOME
来源：http://www.blog.sjlbkw.cn/Article/details/gosgvdirs.sHtML

TS:   process.env.HOME
来源：http://mobile.fktsv.cn/Article/details/gmdevegjd.sHtML

Java: System.getenv("HOME")
来源：http://m.share.yfazqb.com/Article/details/gbebedxrn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.vehdjk.com/Article/details/gljuzuetu.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.yfazqb.com/Article/details/gqnwigiyh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.vehdjk.com/Article/details/guzirmkyz.sHtML

[M03] 执行外部命令
来源：http://read.share.vehdjk.com/Article/details/gqvnatzig.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.tarul.cn/Article/details/gpcpyvzhf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.tarul.cn/Article/details/gajmjanpc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fktsv.cn/Article/details/gghwboecx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.epnwcf.com/Article/details/gmeimrigw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.vehdjk.com/Article/details/gsjkoehjr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.epnwcf.com/Article/details/glavloqxz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fktsv.cn/Article/details/grmvawmwp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.bbcook.cn/Article/details/gjqcujlbj.sHtML

[M04] 获取当前工作目录
来源：http://baike.vehdjk.com/Article/details/gsnrpbldt.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fktsv.cn/Article/details/gnvtqasek.sHtML

PHP:  getcwd();
来源：http://baike.yfazqb.com/Article/details/gjacjupgb.sHtML

JS:   process.cwd()
来源：http://m.share.fktsv.cn/Article/details/gnwpwjsmn.sHtML

TS:   process.cwd()
来源：http://read.share.bbcook.cn/Article/details/gympymavv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fktsv.cn/Article/details/gkpufdrmf.sHtML

Go:   os.Getwd()
来源：http://baike.bbcook.cn/Article/details/gjutvnzeb.sHtML

Ruby: Dir.pwd
来源：http://www.blog.tarul.cn/Article/details/glsjfwlog.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.epnwcf.com/Article/details/gehhslzpi.sHtML

[M05] 设置退出码
来源：http://3g.fktsv.cn/Article/details/gbmhnlcqy.sHtML

Py:   sys.exit(1)
来源：http://m.share.yfazqb.com/Article/details/geyosckyl.sHtML

PHP:  exit(1);
来源：http://blog.vehdjk.com/Article/details/guijfgmyp.sHtML

JS:   process.exit(1)
来源：http://www.share.tarul.cn/Article/details/gtuwfkswf.sHtML

TS:   process.exit(1)
来源：http://wap.bbcook.cn/Article/details/grfnbdwcx.sHtML

Java: System.exit(1)
来源：http://mobile.epnwcf.com/Article/details/gmjmtyplg.sHtML

Go:   os.Exit(1)
来源：http://blog.tarul.cn/Article/details/ghhystwfb.sHtML

Ruby: exit 1
来源：http://baike.epnwcf.com/Article/details/gmlpfazeh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fktsv.cn/Article/details/gazezabuz.sHtML

[M06] 向标准错误输出
来源：http://blog.tarul.cn/Article/details/gupcgvmxw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.yfazqb.com/Article/details/gpciwjfia.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.sjlbkw.cn/Article/details/gtjremknn.sHtML

JS:   console.error("err")
来源：http://www.blog.fktsv.cn/Article/details/gpvplguiv.sHtML

TS:   console.error("err")
来源：http://www.m.share.yfazqb.com/Article/details/gtolhczew.sHtML

Java: System.err.println("err")
来源：http://www.share.epnwcf.com/Article/details/gdhztccfe.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.sjlbkw.cn/Article/details/grtxpefre.sHtML

Ruby: warn "err"
来源：http://www.blog.epnwcf.com/Article/details/gsyhvfwdt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fktsv.cn/Article/details/guvyaebtc.sHtML

[M07] 判断是否为主入口
来源：http://mobile.sjlbkw.cn/Article/details/giquykhzq.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.vehdjk.com/Article/details/gkubvcfmq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.tarul.cn/Article/details/gvxpjjrma.sHtML

JS:   require.main === module
来源：http://www.m.share.bbcook.cn/Article/details/gejjjndem.sHtML

TS:   require.main === module
来源：http://m.share.epnwcf.com/Article/details/gusfisglm.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fktsv.cn/Article/details/gbdykprjy.sHtML

Go:   func main()
来源：http://blog.sjlbkw.cn/Article/details/gfiyvxeys.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.bbcook.cn/Article/details/gqpdlinpn.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.sjlbkw.cn/Article/details/gofiodzmj.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fktsv.cn/Article/details/gmrbbzcxq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.sjlbkw.cn/Article/details/gjeobpajj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.bbcook.cn/Article/details/gbvjttgre.sHtML

JS:   process.platform;  process.version
来源：http://3g.epnwcf.com/Article/details/gjgzuspfm.sHtML

TS:   process.platform;  process.version
来源：http://www.share.bbcook.cn/Article/details/glqaryiwd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.epnwcf.com/Article/details/gcfnkprcs.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.bbcook.cn/Article/details/gabplfbnb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.epnwcf.com/Article/details/grwqzrhbq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.sjlbkw.cn/Article/details/gntsppjpi.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gmubmqdwg.sHtML

N. 数据结构与算法
来源：http://mobile.vehdjk.com/Article/details/gfsewrzun.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gqrdgwmhv.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.vehdjk.com/Article/details/gnlpcylul.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gzseozooo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.tarul.cn/Article/details/gybgadpvc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gkkhmdimk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.yfazqb.com/Article/details/gagbmqmov.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gemcehuxk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gjhrfvtbt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.bbcook.cn/Article/details/guugkdogi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.tarul.cn/Article/details/gfytyxrxo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.bbcook.cn/Article/details/grvrhpjzj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.bbcook.cn/Article/details/giuxnneog.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.vehdjk.com/Article/details/gognvawqr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.vehdjk.com/Article/details/gbzasxzvj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.bbcook.cn/Article/details/gtmmvyvnw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fktsv.cn/Article/details/gqdbayabl.sHtML

Go:   slices.Sort(arr)
来源：http://baike.epnwcf.com/Article/details/goakiucmt.sHtML

Ruby: arr.sort
来源：http://wap.tarul.cn/Article/details/gktfenbmt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fktsv.cn/Article/details/gjufgmqmt.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.sjlbkw.cn/Article/details/gtvjkpwju.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.tarul.cn/Article/details/gpmslpebw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fktsv.cn/Article/details/gfgbqcwwb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.tarul.cn/Article/details/gygnaaobi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.tarul.cn/Article/details/gmubdnrjk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.vehdjk.com/Article/details/gxovkjglx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.yfazqb.com/Article/details/gxeuglaei.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fktsv.cn/Article/details/ghxlyzgda.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.sjlbkw.cn/Article/details/gbanqupof.sHtML

[N04] 斐波那契数列
来源：http://wap.yfazqb.com/Article/details/gnxkxgcfb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.yfazqb.com/Article/details/gzypsvvrl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.bbcook.cn/Article/details/ggievyfgx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.tarul.cn/Article/details/ginfjemwh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.yfazqb.com/Article/details/gfzlfqhem.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.tarul.cn/Article/details/gbkkgpare.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.tarul.cn/Article/details/gmlabirdf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.vehdjk.com/Article/details/gastfjuzi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.yfazqb.com/Article/details/gyuttckug.sHtML

[N05] 最大公约数
来源：http://mobile.vehdjk.com/Article/details/gdaiopuuv.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/gtkbdutce.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.bbcook.cn/Article/details/gipkybvzi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.vehdjk.com/Article/details/gwsnaclns.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.vehdjk.com/Article/details/gqkzxkalz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.yfazqb.com/Article/details/gjgztszgx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.tarul.cn/Article/details/gkkwndjnj.sHtML

Ruby: a.gcd(b)
来源：http://www.share.sjlbkw.cn/Article/details/gqydjhvbz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.bbcook.cn/Article/details/glmgqsufq.sHtML

[N06] 判断回文字符串
来源：http://m.share.yfazqb.com/Article/details/gsfqnwaby.sHtML

Py:   s == s[::-1]
来源：http://baike.bbcook.cn/Article/details/gkhgruwuw.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.vehdjk.com/Article/details/guwmpxfwa.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gdwsvcyyc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.vehdjk.com/Article/details/gnwcdaxvr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.vehdjk.com/Article/details/gwwyjgduc.sHtML

Go:   // 双指针从两端比较
来源：http://3g.epnwcf.com/Article/details/gwkydjwfd.sHtML

Ruby: s == s.reverse
来源：http://blog.fktsv.cn/Article/details/gmyrqaulu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fktsv.cn/Article/details/gjzkvuukd.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.vehdjk.com/Article/details/gimqpygyw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.vehdjk.com/Article/details/gotnwkonn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.epnwcf.com/Article/details/gglcuucwq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.bbcook.cn/Article/details/gjquzkhub.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fktsv.cn/Article/details/gwkxajfik.sHtML

Java: // 手写 HashMap
来源：http://mobile.yfazqb.com/Article/details/gocbfhbac.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.bbcook.cn/Article/details/gmrebhlgn.sHtML

Ruby: // 手写 Hash
来源：http://read.share.bbcook.cn/Article/details/gntmatynb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.tarul.cn/Article/details/ghczfdqau.sHtML

[N08] 生成全排列
来源：http://baike.yfazqb.com/Article/details/gwpimnhlt.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fktsv.cn/Article/details/gvwucekoc.sHtML

PHP:  // 手写递归交换
来源：http://wap.sjlbkw.cn/Article/details/gdjpqbhnf.sHtML

JS:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gxmmvynbx.sHtML

TS:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gafcybknn.sHtML

Java: // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gdtprxnos.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gahvltvkz.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.bbcook.cn/Article/details/gzjdepvdj.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/grzxivctz.sHtML

[N09] 栈与队列
来源：http://read.share.fktsv.cn/Article/details/gixrjcccz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.tarul.cn/Article/details/gxuektlle.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fktsv.cn/Article/details/gfqhhonfk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.yfazqb.com/Article/details/gcmricetb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.vehdjk.com/Article/details/gvskhcwcc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.vehdjk.com/Article/details/gaecufpaz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fktsv.cn/Article/details/gfndtbgrz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.tarul.cn/Article/details/gshjvedut.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fktsv.cn/Article/details/gjmiqshmp.sHtML

[N10] 链表节点定义
来源：http://mobile.fktsv.cn/Article/details/gzsnzplus.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.yfazqb.com/Article/details/ggfrncqjk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.yfazqb.com/Article/details/gsdnkopol.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.tarul.cn/Article/details/gaogwgkbf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.tarul.cn/Article/details/gotnbuzwp.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.yfazqb.com/Article/details/gihwdwuww.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.sjlbkw.cn/Article/details/gefetewun.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.epnwcf.com/Article/details/gvlztmnqx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.sjlbkw.cn/Article/details/gtalttwew.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fktsv.cn/Article/details/gtsgdqttt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.vehdjk.com/Article/details/gdkeijwtn.sHtML

PHP:  // 手写递归函数
来源：http://www.share.bbcook.cn/Article/details/gciktsemy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.yfazqb.com/Article/details/gexfiqmsl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.yfazqb.com/Article/details/grkxzikpf.sHtML

Java: // 手写递归
来源：http://wap.vehdjk.com/Article/details/gdobmhjot.sHtML

Go:   // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/glgfatmhv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fktsv.cn/Article/details/gqoudzvsp.sHtML

C#:   // 手写递归
来源：http://www.blog.tarul.cn/Article/details/gstjprpzq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fktsv.cn/Article/details/gthozwhyo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.tarul.cn/Article/details/glevltryu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.epnwcf.com/Article/details/gughnlgom.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/gffngymxs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.yfazqb.com/Article/details/gxbrtaopc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gjseydttu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fktsv.cn/Article/details/geawrjags.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.yfazqb.com/Article/details/giatkjegr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.yfazqb.com/Article/details/gcnkpkxab.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/glkgsnitr.sHtML

O. 并发与异步
来源：http://blog.bbcook.cn/Article/details/gbjmwtaxp.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gcggdnbqu.sHtML

[O01] 启动一个线程
来源：http://mobile.bbcook.cn/Article/details/gbdzaatet.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.bbcook.cn/Article/details/gnadczdhq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.vehdjk.com/Article/details/glzdqdlvq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.vehdjk.com/Article/details/gzytzoraq.sHtML

TS:   // 同 JS
来源：http://3g.yfazqb.com/Article/details/gatvacbgw.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fktsv.cn/Article/details/gskgnpcns.sHtML

Go:   go f()
来源：http://www.share.bbcook.cn/Article/details/gagkzjgie.sHtML

Ruby: Thread.new { f }
来源：http://baike.fktsv.cn/Article/details/gijpypmpj.sHtML

C#:   Task.Run(() => F());
来源：http://wap.epnwcf.com/Article/details/gwuomgqoe.sHtML

[O02] 使用线程池
来源：http://m.share.bbcook.cn/Article/details/gpaorepli.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.vehdjk.com/Article/details/genwhakrj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.tarul.cn/Article/details/geirzsvqx.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.tarul.cn/Article/details/grvkgklja.sHtML

TS:   // worker_threads 线程池
来源：http://wap.vehdjk.com/Article/details/gzrkksdtk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.tarul.cn/Article/details/gggcycnxf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.sjlbkw.cn/Article/details/gwzfihxsr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.sjlbkw.cn/Article/details/grdyhtgcd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.tarul.cn/Article/details/gjwsrdmoq.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.tarul.cn/Article/details/gzrvxxvpj.sHtML

Py:   with lock: shared += 1
来源：http://blog.tarul.cn/Article/details/gphurplnl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.yfazqb.com/Article/details/gxhpeuriu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.sjlbkw.cn/Article/details/gerheeclj.sHtML

TS:   // 同 JS
来源：http://wap.fktsv.cn/Article/details/gevokrkow.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fktsv.cn/Article/details/ggccwvlsv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.sjlbkw.cn/Article/details/gpkosdtky.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.epnwcf.com/Article/details/gxrukyyxc.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.epnwcf.com/Article/details/gjizxudef.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.tarul.cn/Article/details/gebhnqlza.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.tarul.cn/Article/details/gwxwmhodu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.vehdjk.com/Article/details/gsdeitbhy.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.yfazqb.com/Article/details/giqvqtvsa.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.vehdjk.com/Article/details/gxbptktcj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.bbcook.cn/Article/details/gwcedkqwx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.bbcook.cn/Article/details/gvdmwbacx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fktsv.cn/Article/details/gbuudufnv.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.epnwcf.com/Article/details/gewwbrcvp.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.bbcook.cn/Article/details/gvvtifzuk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.sjlbkw.cn/Article/details/gwqnfozou.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.vehdjk.com/Article/details/gvxqboaky.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.vehdjk.com/Article/details/gnrivjzva.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.tarul.cn/Article/details/gpvxlxrcz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.bbcook.cn/Article/details/gmrdsbnid.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.sjlbkw.cn/Article/details/ghedjclqm.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fktsv.cn/Article/details/gfnqngtaf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.sjlbkw.cn/Article/details/gbfchcehs.sHtML

[O06] 使用进程池
来源：http://mobile.epnwcf.com/Article/details/gurmuoyrw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.yfazqb.com/Article/details/gtkcoxejw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.vehdjk.com/Article/details/gkzutabdh.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fktsv.cn/Article/details/gbatmchmy.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.tarul.cn/Article/details/geclfbmpx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.yfazqb.com/Article/details/gjphwikfa.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.bbcook.cn/Article/details/gjeljwfwv.sHtML

Ruby: // fork 块
来源：http://wap.bbcook.cn/Article/details/gbmyoaohu.sHtML

C#:   Parallel.For
来源：http://m.share.epnwcf.com/Article/details/gameftqpm.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gfyltfjrk.sHtML

P. 常用工具函数
来源：http://m.share.fktsv.cn/Article/details/gevniyzur.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/goqjletue.sHtML

[P01] 生成 UUID
来源：http://m.share.vehdjk.com/Article/details/gzteidfih.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.sjlbkw.cn/Article/details/gsulimipx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.sjlbkw.cn/Article/details/geslrvifz.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.bbcook.cn/Article/details/gnqgacgee.sHtML

TS:   crypto.randomUUID()
来源：http://blog.tarul.cn/Article/details/gsekekvog.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fktsv.cn/Article/details/goltwbvrf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.vehdjk.com/Article/details/gdkowxxro.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.bbcook.cn/Article/details/ggnldraeq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.sjlbkw.cn/Article/details/gblmrfzko.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.vehdjk.com/Article/details/glqjtgnml.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkiveqzs.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.vehdjk.com/Article/details/gehuxszaq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.vehdjk.com/Article/details/goeyddlnr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.sjlbkw.cn/Article/details/gcfnvhpnx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.bbcook.cn/Article/details/ghnnelkyw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fktsv.cn/Article/details/ghumhtiqu.sHtML


<!-- 参考信息 -->