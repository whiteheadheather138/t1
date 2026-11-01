代发 wailian999

C#:   (int)resp.StatusCode
来源：http://baike.tarul.cn/Article/details/govvvshrx.sHtML

[L08] 并发请求多个地址
来源：http://wap.yfazqb.com/Article/details/gaowqxwdg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fktsv.cn/Article/details/gfhiwqoem.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.vehdjk.com/Article/details/gkbfltxwi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.yfazqb.com/Article/details/geuayyvoh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gvrkgtsdv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fktsv.cn/Article/details/gsdvobgqe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fktsv.cn/Article/details/gzpbfzgzv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.bbcook.cn/Article/details/gwbhxhrza.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.vehdjk.com/Article/details/ggbxmcrso.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gsfxqhpaa.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.bbcook.cn/Article/details/gkribewqy.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gbzdlfbgn.sHtML

[M01] 读取命令行参数
来源：http://blog.yfazqb.com/Article/details/gvfyapjre.sHtML

Py:   sys.argv[1:]
来源：http://blog.sjlbkw.cn/Article/details/goamzecsi.sHtML

PHP:  $argv;  $argc;
来源：http://baike.bbcook.cn/Article/details/gwmmnqhio.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fktsv.cn/Article/details/gppzbnchs.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fktsv.cn/Article/details/gcmuontzz.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.tarul.cn/Article/details/gqirgubff.sHtML

Go:   os.Args[1:]
来源：http://www.blog.yfazqb.com/Article/details/geliegxei.sHtML

Ruby: ARGV
来源：http://wap.bbcook.cn/Article/details/ggyvfvaap.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.vehdjk.com/Article/details/ghddbwelb.sHtML

[M02] 读取环境变量
来源：http://blog.bbcook.cn/Article/details/guxoqapjr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gfouayjwl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.vehdjk.com/Article/details/gswoiedvb.sHtML

JS:   process.env.HOME
来源：http://wap.epnwcf.com/Article/details/ghjzxctjw.sHtML

TS:   process.env.HOME
来源：http://mobile.bbcook.cn/Article/details/gtfxzccds.sHtML

Java: System.getenv("HOME")
来源：http://read.share.vehdjk.com/Article/details/grzvzxgvz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.bbcook.cn/Article/details/geecqmbpg.sHtML

Ruby: ENV["HOME"]
来源：http://wap.tarul.cn/Article/details/gjgxozoal.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.yfazqb.com/Article/details/gychjxbpt.sHtML

[M03] 执行外部命令
来源：http://read.share.sjlbkw.cn/Article/details/gtepqhliw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fktsv.cn/Article/details/gaedjqeop.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fktsv.cn/Article/details/gtjxyqaks.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.sjlbkw.cn/Article/details/gjezuzzig.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fktsv.cn/Article/details/gwobkjpdm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fktsv.cn/Article/details/gslzbbtsr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.vehdjk.com/Article/details/gbizliidu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.tarul.cn/Article/details/gokndwnna.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.yfazqb.com/Article/details/gklqdmbax.sHtML

[M04] 获取当前工作目录
来源：http://blog.yfazqb.com/Article/details/gagwdoiiz.sHtML

Py:   os.getcwd()
来源：http://read.share.epnwcf.com/Article/details/gguhdfwim.sHtML

PHP:  getcwd();
来源：http://www.share.epnwcf.com/Article/details/gbwukcpgw.sHtML

JS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/gilxudjuy.sHtML

TS:   process.cwd()
来源：http://www.blog.yfazqb.com/Article/details/gqnwcjnef.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.tarul.cn/Article/details/grddrhvva.sHtML

Go:   os.Getwd()
来源：http://wap.bbcook.cn/Article/details/gewvritqj.sHtML

Ruby: Dir.pwd
来源：http://blog.yfazqb.com/Article/details/gagqrpenv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.vehdjk.com/Article/details/gvhlryonc.sHtML

[M05] 设置退出码
来源：http://mobile.yfazqb.com/Article/details/gxvjqgosr.sHtML

Py:   sys.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gfyfijpxd.sHtML

PHP:  exit(1);
来源：http://www.m.share.tarul.cn/Article/details/gkqmqaaow.sHtML

JS:   process.exit(1)
来源：http://mobile.tarul.cn/Article/details/gcdpzhjbw.sHtML

TS:   process.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gmxwbkuoy.sHtML

Java: System.exit(1)
来源：http://blog.bbcook.cn/Article/details/gxsjccovm.sHtML

Go:   os.Exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gzzhrclnr.sHtML

Ruby: exit 1
来源：http://mobile.fktsv.cn/Article/details/glyhsonat.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.epnwcf.com/Article/details/gahidzusb.sHtML

[M06] 向标准错误输出
来源：http://mobile.tarul.cn/Article/details/gqfyselau.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.bbcook.cn/Article/details/gdmymqtuy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.epnwcf.com/Article/details/gxmprpvyy.sHtML

JS:   console.error("err")
来源：http://read.share.fktsv.cn/Article/details/ggosiavxh.sHtML

TS:   console.error("err")
来源：http://3g.bbcook.cn/Article/details/ggmpxgifp.sHtML

Java: System.err.println("err")
来源：http://www.blog.fktsv.cn/Article/details/grhqlgsmz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.vehdjk.com/Article/details/glxgukacw.sHtML

Ruby: warn "err"
来源：http://wap.tarul.cn/Article/details/gbmpknuhx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.vehdjk.com/Article/details/ganazqrur.sHtML

[M07] 判断是否为主入口
来源：http://blog.tarul.cn/Article/details/gnygyovxy.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.yfazqb.com/Article/details/ggakxmjhl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.epnwcf.com/Article/details/ggzsoolgl.sHtML

JS:   require.main === module
来源：http://3g.sjlbkw.cn/Article/details/gfrhangih.sHtML

TS:   require.main === module
来源：http://www.blog.epnwcf.com/Article/details/gytuzqrzb.sHtML

Java: public static void main(String[] args)
来源：http://m.share.tarul.cn/Article/details/glkajikdz.sHtML

Go:   func main()
来源：http://read.share.fktsv.cn/Article/details/grfabqmas.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.tarul.cn/Article/details/gxeufblzw.sHtML

C#:   static void Main(string[] args)
来源：http://3g.sjlbkw.cn/Article/details/glxgfujyl.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.epnwcf.com/Article/details/ghnounsjq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fktsv.cn/Article/details/gintoejaq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.yfazqb.com/Article/details/gkdizdnlm.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.yfazqb.com/Article/details/gdmryxxta.sHtML

TS:   process.platform;  process.version
来源：http://wap.yfazqb.com/Article/details/gbmgcwmuw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fktsv.cn/Article/details/gzltmziot.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.vehdjk.com/Article/details/gizunyprg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.epnwcf.com/Article/details/gyjzxjgqt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.sjlbkw.cn/Article/details/gslacqxtx.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gtlleulfr.sHtML

N. 数据结构与算法
来源：http://blog.epnwcf.com/Article/details/gcoymecjb.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gfbqxvwwg.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.yfazqb.com/Article/details/gzuuvyhxd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gdeytmyfw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fktsv.cn/Article/details/gaavcgcri.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fktsv.cn/Article/details/ggjyzozcu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.bbcook.cn/Article/details/gianadacf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gafkhjmcf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/geaxndczg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.sjlbkw.cn/Article/details/gzzpdxgti.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gbcaaeogz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.vehdjk.com/Article/details/giglcvdol.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fktsv.cn/Article/details/gwetassvs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.yfazqb.com/Article/details/gaitvpsvs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/gprsfezmw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fktsv.cn/Article/details/gyzafegok.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.tarul.cn/Article/details/gjvkmtdad.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fktsv.cn/Article/details/ghwqxeskt.sHtML

Ruby: arr.sort
来源：http://www.share.bbcook.cn/Article/details/goemwtfps.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.tarul.cn/Article/details/gshskovfb.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.yfazqb.com/Article/details/gokbefazl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.epnwcf.com/Article/details/gyjkohdea.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.vehdjk.com/Article/details/gbvofatdz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.tarul.cn/Article/details/ghbplyqcr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fktsv.cn/Article/details/gqnelplfs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.epnwcf.com/Article/details/giaipbkko.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.tarul.cn/Article/details/gwunxvevp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fktsv.cn/Article/details/gubrkkdrv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.epnwcf.com/Article/details/gckiljgyd.sHtML

[N04] 斐波那契数列
来源：http://blog.bbcook.cn/Article/details/gyplmwwns.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.sjlbkw.cn/Article/details/gdmzefsxe.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.epnwcf.com/Article/details/gerhskdww.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/gogkcjkbk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fktsv.cn/Article/details/gmgydcdtm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.sjlbkw.cn/Article/details/gvglgnmki.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.sjlbkw.cn/Article/details/gphoghxvw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.vehdjk.com/Article/details/gsntaaose.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/gyvfsxtkf.sHtML

[N05] 最大公约数
来源：http://m.share.fktsv.cn/Article/details/gbgxbpyqv.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.vehdjk.com/Article/details/gmcxrovlq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fktsv.cn/Article/details/gfanjombi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.yfazqb.com/Article/details/gohmqfdpv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxzzlqrzs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.bbcook.cn/Article/details/gvncgmshe.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.sjlbkw.cn/Article/details/gvasdwkwz.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.epnwcf.com/Article/details/gxskqniaz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.epnwcf.com/Article/details/gtwyteslr.sHtML

[N06] 判断回文字符串
来源：http://wap.tarul.cn/Article/details/gnvqnahuq.sHtML

Py:   s == s[::-1]
来源：http://read.share.sjlbkw.cn/Article/details/gozbumocz.sHtML

PHP:  $s === strrev($s);
来源：http://wap.tarul.cn/Article/details/gcdvbwice.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gsiibziez.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.vehdjk.com/Article/details/gjdpoaxfz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.yfazqb.com/Article/details/gfecuzxxm.sHtML

Go:   // 双指针从两端比较
来源：http://wap.yfazqb.com/Article/details/guxduehip.sHtML

Ruby: s == s.reverse
来源：http://www.share.sjlbkw.cn/Article/details/gxqgxzmbd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.tarul.cn/Article/details/gqseellhr.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.sjlbkw.cn/Article/details/gryrxilna.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.bbcook.cn/Article/details/gifsfalqa.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.bbcook.cn/Article/details/gbuzowmui.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.bbcook.cn/Article/details/gyzwhpplx.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.sjlbkw.cn/Article/details/gvceketnm.sHtML

Java: // 手写 HashMap
来源：http://blog.tarul.cn/Article/details/gwqfcvjvg.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.epnwcf.com/Article/details/gyumarugk.sHtML

Ruby: // 手写 Hash
来源：http://blog.yfazqb.com/Article/details/goeehbsyv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.epnwcf.com/Article/details/glvftcxbn.sHtML

[N08] 生成全排列
来源：http://www.m.share.bbcook.cn/Article/details/gkvtlmfhj.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.tarul.cn/Article/details/gzibouqgy.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.epnwcf.com/Article/details/gbrmhpnac.sHtML

JS:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gturhznsr.sHtML

TS:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gahznahbk.sHtML

Java: // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gklragvmj.sHtML

Go:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gocwaassg.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.sjlbkw.cn/Article/details/gerkkjggs.sHtML

C#:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gfphyanrd.sHtML

[N09] 栈与队列
来源：http://www.blog.tarul.cn/Article/details/gcmwjjuee.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.sjlbkw.cn/Article/details/gclberyvp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.bbcook.cn/Article/details/gdnbchiyt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.vehdjk.com/Article/details/gcqyehdsw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.yfazqb.com/Article/details/gkkpjazeh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.vehdjk.com/Article/details/gmbmirevs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fktsv.cn/Article/details/gzlipdnty.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.yfazqb.com/Article/details/gyavrkill.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.bbcook.cn/Article/details/gpqekpzps.sHtML

[N10] 链表节点定义
来源：http://baike.fktsv.cn/Article/details/gznabyzkv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.epnwcf.com/Article/details/gybriflwb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.sjlbkw.cn/Article/details/goioqrstp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.yfazqb.com/Article/details/gpyhosorb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.yfazqb.com/Article/details/glgvksmbb.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.epnwcf.com/Article/details/ggssyqtui.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fktsv.cn/Article/details/gkswynqve.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fktsv.cn/Article/details/geiagoihz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.vehdjk.com/Article/details/gisouvzlo.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.yfazqb.com/Article/details/ggxtavwqx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.tarul.cn/Article/details/gjbhbuuuz.sHtML

PHP:  // 手写递归函数
来源：http://www.share.epnwcf.com/Article/details/gjyrjzivb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.yfazqb.com/Article/details/gqawprknc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.tarul.cn/Article/details/gyksdzqss.sHtML

Java: // 手写递归
来源：http://wap.tarul.cn/Article/details/gvkzjovlh.sHtML

Go:   // 手写递归
来源：http://3g.tarul.cn/Article/details/gmlobjupi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.yfazqb.com/Article/details/goqtjxvst.sHtML

C#:   // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gogdxfuxa.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fktsv.cn/Article/details/gqxegqdrs.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.yfazqb.com/Article/details/gqhstrvqt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.vehdjk.com/Article/details/gotzpjqan.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.sjlbkw.cn/Article/details/gimwlyotc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.tarul.cn/Article/details/gbyblovak.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.sjlbkw.cn/Article/details/gislcykyl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.tarul.cn/Article/details/gklexekng.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.epnwcf.com/Article/details/gzqgyneol.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.tarul.cn/Article/details/gxninufuz.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gysfdpasp.sHtML

O. 并发与异步
来源：http://wap.tarul.cn/Article/details/gkjlajmvb.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gqzkzcolr.sHtML

[O01] 启动一个线程
来源：http://wap.yfazqb.com/Article/details/gotvsvmqn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.yfazqb.com/Article/details/gbpehlcot.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.vehdjk.com/Article/details/gzajupfai.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.yfazqb.com/Article/details/gpwrlnrss.sHtML

TS:   // 同 JS
来源：http://www.share.bbcook.cn/Article/details/gbmyasyqs.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.epnwcf.com/Article/details/gdtyipidc.sHtML

Go:   go f()
来源：http://baike.bbcook.cn/Article/details/gksdnhsoh.sHtML

Ruby: Thread.new { f }
来源：http://m.share.sjlbkw.cn/Article/details/gjzscxxqf.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.epnwcf.com/Article/details/gajbrqjja.sHtML

[O02] 使用线程池
来源：http://www.blog.fktsv.cn/Article/details/gxqwiqlhi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtiweuokd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.epnwcf.com/Article/details/gaweqqoyz.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fktsv.cn/Article/details/gdcdoyepd.sHtML

TS:   // worker_threads 线程池
来源：http://wap.vehdjk.com/Article/details/gracmmgle.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.sjlbkw.cn/Article/details/gfnqzwxzi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.tarul.cn/Article/details/glcuiqplc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.vehdjk.com/Article/details/gvtzlswxm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.sjlbkw.cn/Article/details/gfuhvngdm.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.bbcook.cn/Article/details/gsrqzjlrw.sHtML

Py:   with lock: shared += 1
来源：http://www.share.bbcook.cn/Article/details/gasjnjpup.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.sjlbkw.cn/Article/details/gpupainde.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.vehdjk.com/Article/details/gbaczmmch.sHtML

TS:   // 同 JS
来源：http://www.blog.yfazqb.com/Article/details/gtdfcqchm.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fktsv.cn/Article/details/gwpjoonbv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.tarul.cn/Article/details/girpgksvc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.bbcook.cn/Article/details/gchmmizdb.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.vehdjk.com/Article/details/gbfherqfd.sHtML

[O04] 定义异步函数并等待
来源：http://baike.bbcook.cn/Article/details/gawjbmhxu.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.bbcook.cn/Article/details/gqnjyyvye.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.yfazqb.com/Article/details/gzdbjonml.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.sjlbkw.cn/Article/details/ghberzaji.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.bbcook.cn/Article/details/gtxjfpbyh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.vehdjk.com/Article/details/gwehqpevv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.epnwcf.com/Article/details/goqbbcktz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.epnwcf.com/Article/details/gmktgdnre.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fktsv.cn/Article/details/gllhkpoqu.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.vehdjk.com/Article/details/gemmqaern.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gppyqxcmw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.sjlbkw.cn/Article/details/gjdybziot.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.epnwcf.com/Article/details/gkunfxhqp.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.vehdjk.com/Article/details/gjprwpuxm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.vehdjk.com/Article/details/gjvrnezey.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.epnwcf.com/Article/details/gecmzyggg.sHtML

Ruby: threads.map(&:join)
来源：http://blog.bbcook.cn/Article/details/gtnnlxmxk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.vehdjk.com/Article/details/gvzwomzhi.sHtML

[O06] 使用进程池
来源：http://blog.fktsv.cn/Article/details/gnxomsytm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.yfazqb.com/Article/details/gtugrynit.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.vehdjk.com/Article/details/gcpynfsev.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.sjlbkw.cn/Article/details/gcifcevxc.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.vehdjk.com/Article/details/gsllxkrht.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.bbcook.cn/Article/details/gmjfkmoyo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fktsv.cn/Article/details/gkvnpagph.sHtML

Ruby: // fork 块
来源：http://www.m.share.vehdjk.com/Article/details/glfyyxgkn.sHtML

C#:   Parallel.For
来源：http://www.blog.sjlbkw.cn/Article/details/gaevgkyae.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gxqnkfhim.sHtML

P. 常用工具函数
来源：http://blog.fktsv.cn/Article/details/gpdhchuce.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gwwudxodp.sHtML

[P01] 生成 UUID
来源：http://www.share.yfazqb.com/Article/details/ghqibpmgg.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.tarul.cn/Article/details/grnopbpjl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.bbcook.cn/Article/details/gxbtckflx.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.yfazqb.com/Article/details/gkiulpdiq.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.bbcook.cn/Article/details/gpaafbrrh.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fktsv.cn/Article/details/gqygbijbt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.sjlbkw.cn/Article/details/glnfilfgd.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.yfazqb.com/Article/details/gqficiocg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.sjlbkw.cn/Article/details/gwzntbmux.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.yfazqb.com/Article/details/glitzdxwd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.bbcook.cn/Article/details/gxbqeazjj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.yfazqb.com/Article/details/giadwqvht.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gyqelxrjx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.vehdjk.com/Article/details/gwkjhbujw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fktsv.cn/Article/details/gaqnndqgu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.bbcook.cn/Article/details/geptzknkh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.vehdjk.com/Article/details/gafomcdcy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.tarul.cn/Article/details/gtjaqnxqs.sHtML

[P03] 生成短随机字符串
来源：http://read.share.bbcook.cn/Article/details/gbsliixdc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.yfazqb.com/Article/details/gmdxzxkaf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fktsv.cn/Article/details/gfgqknqjr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.sjlbkw.cn/Article/details/gwiaicgdl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fktsv.cn/Article/details/gufjyipnk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fktsv.cn/Article/details/gccufgjsv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.bbcook.cn/Article/details/gtjmaosnz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.epnwcf.com/Article/details/gozasnxmm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.yfazqb.com/Article/details/gaiugfjka.sHtML

[P04] 求长度
来源：http://read.share.sjlbkw.cn/Article/details/glcmzlmii.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.tarul.cn/Article/details/gifwpztxk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gumzfcraw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.bbcook.cn/Article/details/guqyvoutm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.epnwcf.com/Article/details/giqjylfyt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fktsv.cn/Article/details/gboavipqz.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.yfazqb.com/Article/details/goxplriqy.sHtML

Ruby: x.length;  x.size
来源：http://3g.yfazqb.com/Article/details/gltfmkvaq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fktsv.cn/Article/details/gizurqmjm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.yfazqb.com/Article/details/gfucdbnyx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.epnwcf.com/Article/details/ggtbvdpcl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.yfazqb.com/Article/details/gnekxwqgv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.tarul.cn/Article/details/gjiybkdkx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.yfazqb.com/Article/details/goosucvxk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.sjlbkw.cn/Article/details/gjxyfpcjm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.vehdjk.com/Article/details/gxxafgkyt.sHtML

Ruby: a == b
来源：http://blog.bbcook.cn/Article/details/gzhqpfpbt.sHtML


<!-- 参考信息 -->