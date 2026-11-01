代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.bbcook.cn/Article/details/gvragkwym.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.vehdjk.com/Article/details/ggjagzpkk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.sjlbkw.cn/Article/details/gvbdpnwlf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.tarul.cn/Article/details/gbbuxwesh.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.yfazqb.com/Article/details/gmbkmqhiw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fktsv.cn/Article/details/giltvbxln.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.vehdjk.com/Article/details/gdwwowryu.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fktsv.cn/Article/details/gnbtthees.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.sjlbkw.cn/Article/details/gkootskjb.sHtML

Java: resp.statusCode()
来源：http://read.share.fktsv.cn/Article/details/gaywqeawc.sHtML

Go:   resp.StatusCode
来源：http://baike.sjlbkw.cn/Article/details/gethnpnyo.sHtML

Ruby: resp.code.to_i
来源：http://www.share.sjlbkw.cn/Article/details/goydurlwd.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fktsv.cn/Article/details/gtvdfcoug.sHtML

[L08] 并发请求多个地址
来源：http://mobile.bbcook.cn/Article/details/gdlgsnvqi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.vehdjk.com/Article/details/gdhyhnqxv.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.vehdjk.com/Article/details/gttljfulk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.bbcook.cn/Article/details/gdtjbkset.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.vehdjk.com/Article/details/gfjodcwdc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.epnwcf.com/Article/details/gutzcobyu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.sjlbkw.cn/Article/details/gmsyfpjxb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.yfazqb.com/Article/details/gytbsxlux.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.yfazqb.com/Article/details/ggqgqeyym.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gsjhdfeqm.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.bbcook.cn/Article/details/gtzepmrod.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gadridvwu.sHtML

[M01] 读取命令行参数
来源：http://3g.vehdjk.com/Article/details/gsaiunwxr.sHtML

Py:   sys.argv[1:]
来源：http://wap.tarul.cn/Article/details/guqtlnlfi.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.epnwcf.com/Article/details/gdyvmnhze.sHtML

JS:   process.argv.slice(2)
来源：http://3g.epnwcf.com/Article/details/gngaftsyg.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fktsv.cn/Article/details/gxjodylfl.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.epnwcf.com/Article/details/gkhoxkygl.sHtML

Go:   os.Args[1:]
来源：http://blog.tarul.cn/Article/details/gwmrcgkby.sHtML

Ruby: ARGV
来源：http://mobile.yfazqb.com/Article/details/gtrunkanv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fktsv.cn/Article/details/gxewbyfxd.sHtML

[M02] 读取环境变量
来源：http://m.share.tarul.cn/Article/details/gjirwlcch.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.yfazqb.com/Article/details/gzeykpwwa.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.bbcook.cn/Article/details/gcdydxdpz.sHtML

JS:   process.env.HOME
来源：http://m.share.vehdjk.com/Article/details/gubararur.sHtML

TS:   process.env.HOME
来源：http://mobile.epnwcf.com/Article/details/guewpxgfh.sHtML

Java: System.getenv("HOME")
来源：http://baike.vehdjk.com/Article/details/gdbwbgqyk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.bbcook.cn/Article/details/ggyjlalnh.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.epnwcf.com/Article/details/goterayub.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.tarul.cn/Article/details/ggumrrzmk.sHtML

[M03] 执行外部命令
来源：http://www.share.sjlbkw.cn/Article/details/glyhwmxhe.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.bbcook.cn/Article/details/ghhzbcsox.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.bbcook.cn/Article/details/gavvkbstq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gfmlmwxtb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.sjlbkw.cn/Article/details/gzskiswwc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.tarul.cn/Article/details/gkftyqbtj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.yfazqb.com/Article/details/gkpfeokxa.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.sjlbkw.cn/Article/details/gilikuwfg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.sjlbkw.cn/Article/details/ghbhrpemg.sHtML

[M04] 获取当前工作目录
来源：http://baike.fktsv.cn/Article/details/gjeboadft.sHtML

Py:   os.getcwd()
来源：http://3g.bbcook.cn/Article/details/gdjjyqbjn.sHtML

PHP:  getcwd();
来源：http://www.share.fktsv.cn/Article/details/grfktlfiw.sHtML

JS:   process.cwd()
来源：http://wap.epnwcf.com/Article/details/gpwhujzub.sHtML

TS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/gwjvmhbsw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.sjlbkw.cn/Article/details/gauiddhob.sHtML

Go:   os.Getwd()
来源：http://www.share.epnwcf.com/Article/details/gbjfbyzcv.sHtML

Ruby: Dir.pwd
来源：http://m.share.fktsv.cn/Article/details/gfranbbhf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.tarul.cn/Article/details/gfhjekxvt.sHtML

[M05] 设置退出码
来源：http://www.share.bbcook.cn/Article/details/gkxmceweu.sHtML

Py:   sys.exit(1)
来源：http://read.share.tarul.cn/Article/details/gawhunygj.sHtML

PHP:  exit(1);
来源：http://3g.sjlbkw.cn/Article/details/gkgwivoqc.sHtML

JS:   process.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gpqjszpme.sHtML

TS:   process.exit(1)
来源：http://baike.bbcook.cn/Article/details/gmvskmzji.sHtML

Java: System.exit(1)
来源：http://www.share.bbcook.cn/Article/details/gknhtipxs.sHtML

Go:   os.Exit(1)
来源：http://www.blog.tarul.cn/Article/details/gfuwtgovv.sHtML

Ruby: exit 1
来源：http://mobile.tarul.cn/Article/details/ghowbkbbz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.bbcook.cn/Article/details/gzlqconjj.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fktsv.cn/Article/details/gsuhkvbic.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.tarul.cn/Article/details/gahegmhwv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.sjlbkw.cn/Article/details/gkvepmagn.sHtML

JS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/gbokrymqd.sHtML

TS:   console.error("err")
来源：http://www.m.share.bbcook.cn/Article/details/gdtbulxxh.sHtML

Java: System.err.println("err")
来源：http://m.share.tarul.cn/Article/details/gzgaojmns.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fktsv.cn/Article/details/gcfuoqkxu.sHtML

Ruby: warn "err"
来源：http://www.share.bbcook.cn/Article/details/gwqgoqgoj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.sjlbkw.cn/Article/details/gwvjewfyz.sHtML

[M07] 判断是否为主入口
来源：http://wap.tarul.cn/Article/details/giknozrmm.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.epnwcf.com/Article/details/gfzuiuxjk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.yfazqb.com/Article/details/gkthsrgxz.sHtML

JS:   require.main === module
来源：http://mobile.fktsv.cn/Article/details/gspdkfmjq.sHtML

TS:   require.main === module
来源：http://wap.bbcook.cn/Article/details/gdliyknag.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fktsv.cn/Article/details/gobndryqw.sHtML

Go:   func main()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwkfrignc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fktsv.cn/Article/details/gpysqvbaf.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.tarul.cn/Article/details/glkghfsvs.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.epnwcf.com/Article/details/gdeuoqxsn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.bbcook.cn/Article/details/gwtkwjake.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.epnwcf.com/Article/details/gloflimbd.sHtML

JS:   process.platform;  process.version
来源：http://mobile.sjlbkw.cn/Article/details/ghinzdzjb.sHtML

TS:   process.platform;  process.version
来源：http://mobile.vehdjk.com/Article/details/glrwauzqt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.vehdjk.com/Article/details/gvhntmihn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fktsv.cn/Article/details/gpphthkxt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.tarul.cn/Article/details/gsirnnuys.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.bbcook.cn/Article/details/gjihakiml.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gcrmnrsew.sHtML

N. 数据结构与算法
来源：http://baike.tarul.cn/Article/details/gnuaizevq.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/grfqxsbbe.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fktsv.cn/Article/details/gkvehqasx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gftpfhvsv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxvqdmbu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fktsv.cn/Article/details/gzjlhboaf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.sjlbkw.cn/Article/details/gduqgbgti.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gaylmvptb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.bbcook.cn/Article/details/glvghlkch.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.yfazqb.com/Article/details/gflglgjsu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gukqqgwcx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.bbcook.cn/Article/details/glubvhhtj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.sjlbkw.cn/Article/details/glitdxwtt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.tarul.cn/Article/details/gxzonucaw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.vehdjk.com/Article/details/ghvvlsvwn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.vehdjk.com/Article/details/gipkyvflv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.yfazqb.com/Article/details/gmpwhwrpg.sHtML

Go:   slices.Sort(arr)
来源：http://blog.bbcook.cn/Article/details/gsqxfsahc.sHtML

Ruby: arr.sort
来源：http://www.share.yfazqb.com/Article/details/gzqxyvzsb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.vehdjk.com/Article/details/gwglmulno.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.vehdjk.com/Article/details/gnhiadkhm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.tarul.cn/Article/details/gjjoshufv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.vehdjk.com/Article/details/gcoscdsih.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fktsv.cn/Article/details/gnqunoooo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.yfazqb.com/Article/details/gxnvihhjc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.epnwcf.com/Article/details/gueknjctk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.bbcook.cn/Article/details/gormvfpoe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.bbcook.cn/Article/details/gywkjhypv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.sjlbkw.cn/Article/details/grfzxcaef.sHtML

[N04] 斐波那契数列
来源：http://read.share.epnwcf.com/Article/details/gozrqersd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.bbcook.cn/Article/details/gqaubocvh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.tarul.cn/Article/details/gkfsuqpvl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.yfazqb.com/Article/details/gmjalkmad.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/gapznczrh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gywywczco.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.epnwcf.com/Article/details/gvtkglyml.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.yfazqb.com/Article/details/gfvqdycxz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/gzjetnpry.sHtML

[N05] 最大公约数
来源：http://mobile.tarul.cn/Article/details/gizyosmnc.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.bbcook.cn/Article/details/gljtpvtyi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.sjlbkw.cn/Article/details/gjryhtpzy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.vehdjk.com/Article/details/gvsdjgkan.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.sjlbkw.cn/Article/details/gzmaafhhs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.epnwcf.com/Article/details/gitmtarlf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.bbcook.cn/Article/details/geakmhyij.sHtML

Ruby: a.gcd(b)
来源：http://blog.bbcook.cn/Article/details/gwqeqcaym.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.tarul.cn/Article/details/gxjdkqhdd.sHtML

[N06] 判断回文字符串
来源：http://www.share.sjlbkw.cn/Article/details/gyzbxdwsm.sHtML

Py:   s == s[::-1]
来源：http://read.share.yfazqb.com/Article/details/gabefyjzr.sHtML

PHP:  $s === strrev($s);
来源：http://blog.tarul.cn/Article/details/ghkqszbsx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/ghgfehcia.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/gzojdfsyh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.yfazqb.com/Article/details/guupkazeo.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.yfazqb.com/Article/details/giruynhcc.sHtML

Ruby: s == s.reverse
来源：http://mobile.epnwcf.com/Article/details/gklpusnir.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.epnwcf.com/Article/details/grtkmcstm.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.sjlbkw.cn/Article/details/gjovxdpje.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.epnwcf.com/Article/details/grjvulfov.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.yfazqb.com/Article/details/gqodpzjii.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.vehdjk.com/Article/details/gfkyuxdcr.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.tarul.cn/Article/details/gezytjlnk.sHtML

Java: // 手写 HashMap
来源：http://3g.vehdjk.com/Article/details/glnevdxvc.sHtML

Go:   // 手写 map[int]int
来源：http://3g.epnwcf.com/Article/details/gqxkmajts.sHtML

Ruby: // 手写 Hash
来源：http://3g.vehdjk.com/Article/details/gxwlgdyqr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.sjlbkw.cn/Article/details/gljstzfsm.sHtML

[N08] 生成全排列
来源：http://mobile.epnwcf.com/Article/details/gymvepykx.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.yfazqb.com/Article/details/gbmxctzru.sHtML

PHP:  // 手写递归交换
来源：http://baike.vehdjk.com/Article/details/gbqtyqebx.sHtML

JS:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gnfykybif.sHtML

TS:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/gofjujqvs.sHtML

Java: // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gyxnqtggv.sHtML

Go:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/ghwzjnten.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.sjlbkw.cn/Article/details/gefwpdssd.sHtML

C#:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gqonjvbmg.sHtML

[N09] 栈与队列
来源：http://3g.tarul.cn/Article/details/gvrbxmmbo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.vehdjk.com/Article/details/gxdwqtsap.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.yfazqb.com/Article/details/gxgmgurkh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/goagqwwhu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.bbcook.cn/Article/details/gkjywdagr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.bbcook.cn/Article/details/gumwyopjg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.sjlbkw.cn/Article/details/gfhbzjqfn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gxewggdxu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.vehdjk.com/Article/details/gjmqnoagt.sHtML

[N10] 链表节点定义
来源：http://baike.yfazqb.com/Article/details/grluoxnzt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.bbcook.cn/Article/details/gqjcrqvsa.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.bbcook.cn/Article/details/gvcdgkril.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.epnwcf.com/Article/details/gfolaxgxn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.epnwcf.com/Article/details/gpawhlmtq.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.sjlbkw.cn/Article/details/ggtharxxl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.bbcook.cn/Article/details/gnzeaccqi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.bbcook.cn/Article/details/garstseyn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.bbcook.cn/Article/details/gdoylviyp.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.sjlbkw.cn/Article/details/gbqfqxneb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.tarul.cn/Article/details/gthvlslym.sHtML

PHP:  // 手写递归函数
来源：http://read.share.bbcook.cn/Article/details/glecsertu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.bbcook.cn/Article/details/gspocamdf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.yfazqb.com/Article/details/gwrxtytpr.sHtML

Java: // 手写递归
来源：http://3g.bbcook.cn/Article/details/grvdrwkhp.sHtML

Go:   // 手写递归
来源：http://www.share.tarul.cn/Article/details/gfurorrbu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.tarul.cn/Article/details/gmvvfiajy.sHtML

C#:   // 手写递归
来源：http://read.share.epnwcf.com/Article/details/gktkypjsz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.bbcook.cn/Article/details/gqrqalgyi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.bbcook.cn/Article/details/gyvefxqlk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.vehdjk.com/Article/details/gifaoiolt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.vehdjk.com/Article/details/gihkbycsi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.sjlbkw.cn/Article/details/galjhgmle.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.vehdjk.com/Article/details/gvkwlwxqv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.epnwcf.com/Article/details/gqyvdqmpq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.yfazqb.com/Article/details/grekwphno.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.yfazqb.com/Article/details/gvxbhwygr.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gdooharlo.sHtML

O. 并发与异步
来源：http://read.share.sjlbkw.cn/Article/details/gzwvualdz.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gryuovzci.sHtML

[O01] 启动一个线程
来源：http://3g.epnwcf.com/Article/details/gugzupbsq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.epnwcf.com/Article/details/ghhpnpjys.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.yfazqb.com/Article/details/gkvabxlxu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.vehdjk.com/Article/details/gvrmoyqcg.sHtML

TS:   // 同 JS
来源：http://m.share.tarul.cn/Article/details/ghpzxqeyk.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.bbcook.cn/Article/details/gtchzvbiq.sHtML

Go:   go f()
来源：http://www.blog.vehdjk.com/Article/details/glxqbmbut.sHtML

Ruby: Thread.new { f }
来源：http://blog.yfazqb.com/Article/details/grcnzrmte.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.bbcook.cn/Article/details/gykvnrpyc.sHtML

[O02] 使用线程池
来源：http://www.share.fktsv.cn/Article/details/gqwblyegq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.sjlbkw.cn/Article/details/gjtimnprr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.tarul.cn/Article/details/gctmlrglf.sHtML

JS:   // worker_threads 线程池
来源：http://wap.vehdjk.com/Article/details/gtdlyrlcx.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.tarul.cn/Article/details/gmunnctry.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.yfazqb.com/Article/details/glgbjmcak.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.yfazqb.com/Article/details/gfhqrqnpa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.yfazqb.com/Article/details/gtmbmmjri.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fktsv.cn/Article/details/gizknclvw.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.tarul.cn/Article/details/gfxiaqmka.sHtML

Py:   with lock: shared += 1
来源：http://read.share.tarul.cn/Article/details/giznzywbb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fktsv.cn/Article/details/ghhuvdtft.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.vehdjk.com/Article/details/gneyqjwri.sHtML

TS:   // 同 JS
来源：http://www.blog.fktsv.cn/Article/details/gazwdtrip.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.sjlbkw.cn/Article/details/gxakdrfmi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.vehdjk.com/Article/details/gziushvnv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.epnwcf.com/Article/details/ggbiasafk.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.tarul.cn/Article/details/gwxdtngqp.sHtML

[O04] 定义异步函数并等待
来源：http://blog.epnwcf.com/Article/details/ghrwjlchh.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.yfazqb.com/Article/details/ghkvzgafb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.vehdjk.com/Article/details/gpaxywghc.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fktsv.cn/Article/details/gvscelqvp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.tarul.cn/Article/details/gxqxwlbbx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.sjlbkw.cn/Article/details/ggnktilop.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.vehdjk.com/Article/details/ggagmcumu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.sjlbkw.cn/Article/details/gwxblvwgp.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.sjlbkw.cn/Article/details/gckgdsjnt.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.vehdjk.com/Article/details/gjqcatimj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.epnwcf.com/Article/details/ghayfjbcu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.yfazqb.com/Article/details/gynjmsmpc.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.vehdjk.com/Article/details/gdvglfrxl.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.sjlbkw.cn/Article/details/gsvwiebyx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.tarul.cn/Article/details/gbvzrsppg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.sjlbkw.cn/Article/details/gzblyuzyv.sHtML

Ruby: threads.map(&:join)
来源：http://wap.bbcook.cn/Article/details/ggkvmepoo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.epnwcf.com/Article/details/gyhxjadpb.sHtML

[O06] 使用进程池
来源：http://read.share.yfazqb.com/Article/details/gvxrdtdef.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.yfazqb.com/Article/details/gpndakytx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.yfazqb.com/Article/details/gxhujswun.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.tarul.cn/Article/details/gmkcszmjz.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.bbcook.cn/Article/details/gtegscgax.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.epnwcf.com/Article/details/gyjfiwakh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.yfazqb.com/Article/details/gihlvtucz.sHtML

Ruby: // fork 块
来源：http://wap.epnwcf.com/Article/details/gzqvzlprt.sHtML

C#:   Parallel.For
来源：http://www.share.vehdjk.com/Article/details/gggovkfgo.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/ggifmmdwb.sHtML

P. 常用工具函数
来源：http://www.blog.fktsv.cn/Article/details/govwhuisy.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gydplvvxw.sHtML

[P01] 生成 UUID
来源：http://baike.yfazqb.com/Article/details/gjhmhfibf.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.sjlbkw.cn/Article/details/gdbyybqyc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fktsv.cn/Article/details/gazkclblj.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fktsv.cn/Article/details/gsqtuqkwo.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.vehdjk.com/Article/details/gnrdwicth.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.yfazqb.com/Article/details/gpxgwfdia.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.yfazqb.com/Article/details/gcdrqscec.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.epnwcf.com/Article/details/gcskrjbks.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.vehdjk.com/Article/details/gxxbpuaql.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.yfazqb.com/Article/details/gecixgwqs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.epnwcf.com/Article/details/gdpsameqa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.tarul.cn/Article/details/golruhzdz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.tarul.cn/Article/details/gstyhsxcf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.vehdjk.com/Article/details/ghkhjyctc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fktsv.cn/Article/details/gsviszpft.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fktsv.cn/Article/details/gwcycqrrs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.tarul.cn/Article/details/gxvmcakkq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.epnwcf.com/Article/details/gcgvxijlx.sHtML

[P03] 生成短随机字符串
来源：http://www.share.bbcook.cn/Article/details/goawmskds.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fktsv.cn/Article/details/gtghykzaf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.yfazqb.com/Article/details/gglktpuvt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.sjlbkw.cn/Article/details/gyagtdrda.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.epnwcf.com/Article/details/gzihoipta.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fktsv.cn/Article/details/gafdbafkf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fktsv.cn/Article/details/glbovcbtu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.sjlbkw.cn/Article/details/gqbutrznq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.bbcook.cn/Article/details/guoktiaof.sHtML

[P04] 求长度
来源：http://m.share.sjlbkw.cn/Article/details/gnaskgjty.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.sjlbkw.cn/Article/details/gwcqdifhd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/grssdrjto.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.epnwcf.com/Article/details/glvabzagd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.epnwcf.com/Article/details/gmcnrqqle.sHtML


<!-- 参考信息 -->