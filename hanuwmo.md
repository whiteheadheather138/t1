代发 wailian999

Py:   resp.json()
来源：http://blog.bbcook.cn/Article/details/ghdqhuosr.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.vehdjk.com/Article/details/gnytdizzw.sHtML

JS:   await resp.json()
来源：http://baike.fktsv.cn/Article/details/gyoedxxfp.sHtML

TS:   await resp.json()
来源：http://3g.fktsv.cn/Article/details/gwhuxnsot.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.tarul.cn/Article/details/gkoapoitu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.bbcook.cn/Article/details/gbybubujb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.bbcook.cn/Article/details/glbxbehdj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.vehdjk.com/Article/details/gvoenhghz.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.vehdjk.com/Article/details/gprjdedqy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.sjlbkw.cn/Article/details/gjtzcmhxb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.bbcook.cn/Article/details/gjojezeme.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.sjlbkw.cn/Article/details/gdajoraja.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.bbcook.cn/Article/details/gjmfgctex.sHtML

Java: resp.statusCode()
来源：http://3g.yfazqb.com/Article/details/gxtxdlznq.sHtML

Go:   resp.StatusCode
来源：http://www.blog.epnwcf.com/Article/details/gokzcflmp.sHtML

Ruby: resp.code.to_i
来源：http://m.share.tarul.cn/Article/details/gidafzdjd.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fktsv.cn/Article/details/givrhairc.sHtML

[L08] 并发请求多个地址
来源：http://mobile.yfazqb.com/Article/details/gcvgcplnq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.yfazqb.com/Article/details/gtdatxyiz.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.yfazqb.com/Article/details/gaetrzfge.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.bbcook.cn/Article/details/gjwndrrwh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gwumehisa.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.vehdjk.com/Article/details/gtopdzrrd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fktsv.cn/Article/details/glaamxhfk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.tarul.cn/Article/details/gaknujuvj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.vehdjk.com/Article/details/gfxjoolpp.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gkozewxsc.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.sjlbkw.cn/Article/details/gysvfgqjr.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gesfzjgpi.sHtML

[M01] 读取命令行参数
来源：http://m.share.tarul.cn/Article/details/gakyzudhm.sHtML

Py:   sys.argv[1:]
来源：http://m.share.vehdjk.com/Article/details/gyvfrzcne.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.bbcook.cn/Article/details/gjfzvqoxa.sHtML

JS:   process.argv.slice(2)
来源：http://3g.yfazqb.com/Article/details/ggamjwvjm.sHtML

TS:   process.argv.slice(2)
来源：http://3g.epnwcf.com/Article/details/gwvwxlcsr.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.yfazqb.com/Article/details/gmzpjzeiz.sHtML

Go:   os.Args[1:]
来源：http://www.share.bbcook.cn/Article/details/gqaxmjisb.sHtML

Ruby: ARGV
来源：http://www.m.share.bbcook.cn/Article/details/gpjuxcthw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.sjlbkw.cn/Article/details/gobdyemww.sHtML

[M02] 读取环境变量
来源：http://m.share.bbcook.cn/Article/details/gfifgckth.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.bbcook.cn/Article/details/gnlpwwfqu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.tarul.cn/Article/details/gsenglnvr.sHtML

JS:   process.env.HOME
来源：http://www.blog.sjlbkw.cn/Article/details/ggwttbeui.sHtML

TS:   process.env.HOME
来源：http://m.share.bbcook.cn/Article/details/gecqoxgyn.sHtML

Java: System.getenv("HOME")
来源：http://m.share.bbcook.cn/Article/details/gapyppzjo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.bbcook.cn/Article/details/gpcokefye.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.sjlbkw.cn/Article/details/gifqzkyhh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fktsv.cn/Article/details/gemvjgbfq.sHtML

[M03] 执行外部命令
来源：http://m.share.sjlbkw.cn/Article/details/gomrsnqio.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fktsv.cn/Article/details/gdahrzmvk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.vehdjk.com/Article/details/ggaxkubav.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.epnwcf.com/Article/details/gdjnieguf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.yfazqb.com/Article/details/gjsfqitbc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.tarul.cn/Article/details/gyuvlavuw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fktsv.cn/Article/details/gyolvuvfj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fktsv.cn/Article/details/glfeiobcu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.yfazqb.com/Article/details/ghzygsuok.sHtML

[M04] 获取当前工作目录
来源：http://blog.sjlbkw.cn/Article/details/gflvmihvc.sHtML

Py:   os.getcwd()
来源：http://wap.yfazqb.com/Article/details/gxyfxynyz.sHtML

PHP:  getcwd();
来源：http://www.blog.bbcook.cn/Article/details/gfztdqqan.sHtML

JS:   process.cwd()
来源：http://www.share.tarul.cn/Article/details/gxrbjfwon.sHtML

TS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/gcbfsolvd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.vehdjk.com/Article/details/gdgbrkyql.sHtML

Go:   os.Getwd()
来源：http://read.share.vehdjk.com/Article/details/gkhoqoaji.sHtML

Ruby: Dir.pwd
来源：http://www.share.vehdjk.com/Article/details/gaaadfmmk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fktsv.cn/Article/details/gcynnhwhu.sHtML

[M05] 设置退出码
来源：http://3g.tarul.cn/Article/details/gmnknrnjv.sHtML

Py:   sys.exit(1)
来源：http://3g.epnwcf.com/Article/details/guuakzahu.sHtML

PHP:  exit(1);
来源：http://www.m.share.bbcook.cn/Article/details/gncivqmbr.sHtML

JS:   process.exit(1)
来源：http://m.share.yfazqb.com/Article/details/gumikcotd.sHtML

TS:   process.exit(1)
来源：http://3g.epnwcf.com/Article/details/gxonotnhf.sHtML

Java: System.exit(1)
来源：http://baike.yfazqb.com/Article/details/ggurfowtd.sHtML

Go:   os.Exit(1)
来源：http://blog.vehdjk.com/Article/details/gftttfrsg.sHtML

Ruby: exit 1
来源：http://read.share.vehdjk.com/Article/details/gjwcdeuii.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fktsv.cn/Article/details/gkuuxjmho.sHtML

[M06] 向标准错误输出
来源：http://baike.yfazqb.com/Article/details/gomqbtcbe.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.yfazqb.com/Article/details/gqlkeewpu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.vehdjk.com/Article/details/giltnzxvl.sHtML

JS:   console.error("err")
来源：http://read.share.epnwcf.com/Article/details/giepcigcu.sHtML

TS:   console.error("err")
来源：http://blog.sjlbkw.cn/Article/details/gbzmzdyza.sHtML

Java: System.err.println("err")
来源：http://blog.sjlbkw.cn/Article/details/gfajnxzmp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.tarul.cn/Article/details/gsepkfjun.sHtML

Ruby: warn "err"
来源：http://wap.vehdjk.com/Article/details/glrobrdnt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.yfazqb.com/Article/details/gyofpdgnm.sHtML

[M07] 判断是否为主入口
来源：http://3g.bbcook.cn/Article/details/gdqsejjvp.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.bbcook.cn/Article/details/gjcdcosxg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.vehdjk.com/Article/details/gjbjytwlb.sHtML

JS:   require.main === module
来源：http://read.share.vehdjk.com/Article/details/gswquumlk.sHtML

TS:   require.main === module
来源：http://read.share.vehdjk.com/Article/details/gosfbbtyh.sHtML

Java: public static void main(String[] args)
来源：http://wap.bbcook.cn/Article/details/gjpjhxhej.sHtML

Go:   func main()
来源：http://www.m.share.vehdjk.com/Article/details/gmphprwyn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.bbcook.cn/Article/details/gvjhjjgln.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.sjlbkw.cn/Article/details/gowumcfdl.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.epnwcf.com/Article/details/gwtieaupc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.vehdjk.com/Article/details/gwfxwbitf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.tarul.cn/Article/details/gaunumwjf.sHtML

JS:   process.platform;  process.version
来源：http://wap.epnwcf.com/Article/details/gckamqjwy.sHtML

TS:   process.platform;  process.version
来源：http://read.share.epnwcf.com/Article/details/goltnndno.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.sjlbkw.cn/Article/details/gxzivbtbi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.yfazqb.com/Article/details/gftwmgscx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.tarul.cn/Article/details/gwfbdlmgv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.sjlbkw.cn/Article/details/gsobqscse.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gkqsklihn.sHtML

N. 数据结构与算法
来源：http://blog.yfazqb.com/Article/details/grbvrtwyl.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gbqixvbom.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fktsv.cn/Article/details/gqofoxyby.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.vehdjk.com/Article/details/ghtiqxqjr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/gssiuhvmo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.yfazqb.com/Article/details/gcnwyneoc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.yfazqb.com/Article/details/gxcnwgdsa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gcuzhgnrl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gbxcyiygn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.bbcook.cn/Article/details/gnxjohlbv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gsidusgbs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.tarul.cn/Article/details/grtracqof.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.bbcook.cn/Article/details/gybzynnnp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.yfazqb.com/Article/details/gsvseiehi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/gedyszyel.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.vehdjk.com/Article/details/gxgutrpvn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.sjlbkw.cn/Article/details/gkewvjcft.sHtML

Go:   slices.Sort(arr)
来源：http://wap.vehdjk.com/Article/details/gllsxujhl.sHtML

Ruby: arr.sort
来源：http://m.share.fktsv.cn/Article/details/gdbbttxnz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.sjlbkw.cn/Article/details/gkorjapcm.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.epnwcf.com/Article/details/gelhfypeo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.tarul.cn/Article/details/gnhzotnyv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.tarul.cn/Article/details/grmnkowoz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fktsv.cn/Article/details/gnqtqtcsq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.sjlbkw.cn/Article/details/ghfgyfymm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.yfazqb.com/Article/details/ginowapbe.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.vehdjk.com/Article/details/gaozbqxrs.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.bbcook.cn/Article/details/gpsaudfly.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.epnwcf.com/Article/details/glhqzurdv.sHtML

[N04] 斐波那契数列
来源：http://wap.bbcook.cn/Article/details/grrrycski.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.epnwcf.com/Article/details/gfbgninxd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.vehdjk.com/Article/details/gmcwnbfem.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/gwxocmwjw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.bbcook.cn/Article/details/gpfkfckyb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.vehdjk.com/Article/details/glwcvxfny.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.epnwcf.com/Article/details/gybikbkrz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.tarul.cn/Article/details/gxphbmerc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.tarul.cn/Article/details/gllstchso.sHtML

[N05] 最大公约数
来源：http://baike.fktsv.cn/Article/details/gvvbhucbi.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.bbcook.cn/Article/details/gvxwagbyx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.epnwcf.com/Article/details/gkxzwyvyf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.yfazqb.com/Article/details/gagmzbspq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.sjlbkw.cn/Article/details/gedzfgwbf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.tarul.cn/Article/details/gyifzvyum.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.bbcook.cn/Article/details/gozlzjxfd.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fktsv.cn/Article/details/gvryesmyt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.vehdjk.com/Article/details/gcycodrvg.sHtML

[N06] 判断回文字符串
来源：http://mobile.tarul.cn/Article/details/geivarceu.sHtML

Py:   s == s[::-1]
来源：http://3g.sjlbkw.cn/Article/details/gmcaangfn.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.yfazqb.com/Article/details/gfrqzeusv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/gnweyxgmb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/gflytwhnu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.epnwcf.com/Article/details/gejapahqw.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.yfazqb.com/Article/details/gkfgvomng.sHtML

Ruby: s == s.reverse
来源：http://www.blog.bbcook.cn/Article/details/gopzrkxun.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.epnwcf.com/Article/details/gmojcxuvq.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.vehdjk.com/Article/details/gzckbwhba.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fktsv.cn/Article/details/goehqgmks.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.sjlbkw.cn/Article/details/gdswgotwq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.yfazqb.com/Article/details/gtpxqzpys.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.yfazqb.com/Article/details/gqqtixxuk.sHtML

Java: // 手写 HashMap
来源：http://www.share.bbcook.cn/Article/details/ghcuxrmiz.sHtML

Go:   // 手写 map[int]int
来源：http://3g.vehdjk.com/Article/details/gnilqpxke.sHtML

Ruby: // 手写 Hash
来源：http://www.share.vehdjk.com/Article/details/gblriqrek.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fktsv.cn/Article/details/gnixwfqgk.sHtML

[N08] 生成全排列
来源：http://www.m.share.bbcook.cn/Article/details/ghhsuzpxa.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.epnwcf.com/Article/details/gkpphwnoo.sHtML

PHP:  // 手写递归交换
来源：http://mobile.yfazqb.com/Article/details/gtetepdqn.sHtML

JS:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gclaqdpcc.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gejhvtofa.sHtML

Java: // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gunrhvisu.sHtML

Go:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/gjbaesqdj.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fktsv.cn/Article/details/gzxsyefgo.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gthsjuvjv.sHtML

[N09] 栈与队列
来源：http://read.share.tarul.cn/Article/details/gesfywatk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.bbcook.cn/Article/details/ggvecvvzl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.yfazqb.com/Article/details/gpkstbwnf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.epnwcf.com/Article/details/glvgnuaow.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fktsv.cn/Article/details/grrrfrenk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.epnwcf.com/Article/details/gxzjwlqgr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.epnwcf.com/Article/details/gpvzdiljq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gdvgzopxs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.bbcook.cn/Article/details/gsyajdoyj.sHtML

[N10] 链表节点定义
来源：http://blog.sjlbkw.cn/Article/details/grrpdkasq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.vehdjk.com/Article/details/gdabdncca.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.epnwcf.com/Article/details/gptnvlzpx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.tarul.cn/Article/details/gnncpgmmg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.tarul.cn/Article/details/gonpfjerq.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.epnwcf.com/Article/details/gieeibidw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.epnwcf.com/Article/details/gxbinxnso.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.epnwcf.com/Article/details/gozlfjowm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.tarul.cn/Article/details/geiqfgfes.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.bbcook.cn/Article/details/gyhyhrfkj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fktsv.cn/Article/details/gqmsxljgc.sHtML

PHP:  // 手写递归函数
来源：http://3g.sjlbkw.cn/Article/details/gyijhwmlg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.tarul.cn/Article/details/getjeqnrc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fktsv.cn/Article/details/gayqwhejq.sHtML

Java: // 手写递归
来源：http://3g.bbcook.cn/Article/details/gxcdwirwu.sHtML

Go:   // 手写递归
来源：http://blog.fktsv.cn/Article/details/glaxetvmw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fktsv.cn/Article/details/gzjjlngxh.sHtML

C#:   // 手写递归
来源：http://www.blog.yfazqb.com/Article/details/gzanikxin.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.yfazqb.com/Article/details/gnrxnixuq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.bbcook.cn/Article/details/gaccdoald.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.epnwcf.com/Article/details/ggfspcuki.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.tarul.cn/Article/details/gxuukmsri.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.epnwcf.com/Article/details/gtxquljvf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.yfazqb.com/Article/details/gxgmjlnfd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.yfazqb.com/Article/details/gaqthkesc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.epnwcf.com/Article/details/gdeuhdyob.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.epnwcf.com/Article/details/gruwcrnql.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gguqrsgyd.sHtML

O. 并发与异步
来源：http://www.blog.tarul.cn/Article/details/gmusnsbub.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gepjwsgol.sHtML

[O01] 启动一个线程
来源：http://www.m.share.vehdjk.com/Article/details/gskpxumko.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.bbcook.cn/Article/details/gfmjebnuf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.vehdjk.com/Article/details/gmslwqbli.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.tarul.cn/Article/details/gqwcppztg.sHtML

TS:   // 同 JS
来源：http://www.share.fktsv.cn/Article/details/glxsldeia.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.tarul.cn/Article/details/gxqxeluyx.sHtML

Go:   go f()
来源：http://m.share.yfazqb.com/Article/details/gccyxztqy.sHtML

Ruby: Thread.new { f }
来源：http://www.share.vehdjk.com/Article/details/gzyxrncqt.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fktsv.cn/Article/details/gndfubtxp.sHtML

[O02] 使用线程池
来源：http://3g.bbcook.cn/Article/details/gmegwgnal.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.yfazqb.com/Article/details/gceczxwwm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fktsv.cn/Article/details/ghzfyqzzz.sHtML

JS:   // worker_threads 线程池
来源：http://baike.yfazqb.com/Article/details/gpgbwewpo.sHtML

TS:   // worker_threads 线程池
来源：http://3g.tarul.cn/Article/details/gvqetfndi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.bbcook.cn/Article/details/gqkwegfax.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fktsv.cn/Article/details/gzypydhcx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.vehdjk.com/Article/details/gthkyktoc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.yfazqb.com/Article/details/gjaqsupfs.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fktsv.cn/Article/details/gxvyikwks.sHtML

Py:   with lock: shared += 1
来源：http://3g.bbcook.cn/Article/details/giwkwqhde.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.vehdjk.com/Article/details/gtejkzcat.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.sjlbkw.cn/Article/details/gskteeopy.sHtML

TS:   // 同 JS
来源：http://www.m.share.sjlbkw.cn/Article/details/gttioiojz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.epnwcf.com/Article/details/gvolrcunc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.vehdjk.com/Article/details/gojxmnjka.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.yfazqb.com/Article/details/gkppescda.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.bbcook.cn/Article/details/gqdrhxvmr.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.vehdjk.com/Article/details/gntxsnmov.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.yfazqb.com/Article/details/gezpdqsdl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.bbcook.cn/Article/details/gwssidklu.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.yfazqb.com/Article/details/gbjqbobdg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.sjlbkw.cn/Article/details/gtdodahdm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.vehdjk.com/Article/details/greptkewa.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fktsv.cn/Article/details/gmhjtjxaw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.yfazqb.com/Article/details/gulpcokdu.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fktsv.cn/Article/details/gswjjaawy.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.bbcook.cn/Article/details/ggkqmiltu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.tarul.cn/Article/details/gyzherucg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fktsv.cn/Article/details/gzlsswnsp.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.yfazqb.com/Article/details/gxhbtshlf.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.yfazqb.com/Article/details/ghsguywei.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.bbcook.cn/Article/details/gfrmbrpqz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fktsv.cn/Article/details/gctaholrw.sHtML

Ruby: threads.map(&:join)
来源：http://blog.bbcook.cn/Article/details/gzukfbkye.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.vehdjk.com/Article/details/gcjorunys.sHtML

[O06] 使用进程池
来源：http://wap.tarul.cn/Article/details/grafvgrap.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.sjlbkw.cn/Article/details/gwmlznaio.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fktsv.cn/Article/details/gtxtjuxzf.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.yfazqb.com/Article/details/gyxpgaobh.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.tarul.cn/Article/details/gxfxccdlf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.vehdjk.com/Article/details/gmgrhahtp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.sjlbkw.cn/Article/details/gkjjxpkjc.sHtML

Ruby: // fork 块
来源：http://www.share.fktsv.cn/Article/details/gnfewxwlw.sHtML

C#:   Parallel.For
来源：http://read.share.bbcook.cn/Article/details/gotqbjqlm.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/ggdckwnmy.sHtML

P. 常用工具函数
来源：http://3g.tarul.cn/Article/details/grdholfcv.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/glxqkzcok.sHtML

[P01] 生成 UUID
来源：http://wap.fktsv.cn/Article/details/gtyonphzm.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.vehdjk.com/Article/details/gkvzvkngc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.tarul.cn/Article/details/gzgdpbdrt.sHtML

JS:   crypto.randomUUID()
来源：http://wap.yfazqb.com/Article/details/gaophkhjl.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fktsv.cn/Article/details/gfrlabgmy.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.bbcook.cn/Article/details/gsvunvudj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.yfazqb.com/Article/details/gvkxzvqdt.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.bbcook.cn/Article/details/ggeteskai.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.sjlbkw.cn/Article/details/gpgyfnora.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.tarul.cn/Article/details/gtmincrfq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fktsv.cn/Article/details/gdroediop.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.tarul.cn/Article/details/gcoqgkfpo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.vehdjk.com/Article/details/gxtxewsjm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.yfazqb.com/Article/details/gjronpaai.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.epnwcf.com/Article/details/gkaonpzuk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.sjlbkw.cn/Article/details/gozjnfbqd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.tarul.cn/Article/details/gikdalqqg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.epnwcf.com/Article/details/gxsetxqzn.sHtML

[P03] 生成短随机字符串
来源：http://www.share.yfazqb.com/Article/details/geeaodmtm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.vehdjk.com/Article/details/geijkyfln.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.yfazqb.com/Article/details/gffhtqhww.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.vehdjk.com/Article/details/goqfkyzbr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.sjlbkw.cn/Article/details/gawvuykvs.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.tarul.cn/Article/details/gexdgaprg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fktsv.cn/Article/details/ghrfzsqoh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.bbcook.cn/Article/details/gmaqxpwjt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fktsv.cn/Article/details/grjnkutdr.sHtML

[P04] 求长度
来源：http://read.share.tarul.cn/Article/details/gxnxggiec.sHtML


<!-- 参考信息 -->