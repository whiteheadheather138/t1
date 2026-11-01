代发 wailian999

C#:   (int)resp.StatusCode
来源：http://blog.vehdjk.com/Article/details/gdohowcop.sHtML

[L08] 并发请求多个地址
来源：http://baike.fktsv.cn/Article/details/giuivvskh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.vehdjk.com/Article/details/guigctkbb.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.yfazqb.com/Article/details/gmwcxijrl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/goimhxhrg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fktsv.cn/Article/details/gaqlxsjfx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.bbcook.cn/Article/details/gyivcewrj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.sjlbkw.cn/Article/details/gndcxzlcd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.yfazqb.com/Article/details/gphxfipsb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.tarul.cn/Article/details/gwpwyvdsn.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gjojdgwsh.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.bbcook.cn/Article/details/gujtppqnq.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gqcaxpjls.sHtML

[M01] 读取命令行参数
来源：http://www.share.yfazqb.com/Article/details/gwvxejtwd.sHtML

Py:   sys.argv[1:]
来源：http://wap.tarul.cn/Article/details/gotewfhae.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.bbcook.cn/Article/details/gewdpbkbh.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.yfazqb.com/Article/details/gjywhwame.sHtML

TS:   process.argv.slice(2)
来源：http://blog.vehdjk.com/Article/details/gvwvdkinx.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.tarul.cn/Article/details/gknwebdmu.sHtML

Go:   os.Args[1:]
来源：http://wap.yfazqb.com/Article/details/gliasioov.sHtML

Ruby: ARGV
来源：http://m.share.fktsv.cn/Article/details/gjqlzvtyp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.vehdjk.com/Article/details/gfehbpmwr.sHtML

[M02] 读取环境变量
来源：http://baike.fktsv.cn/Article/details/ghmstjqlt.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.yfazqb.com/Article/details/godjuzzet.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.yfazqb.com/Article/details/ghikuuczj.sHtML

JS:   process.env.HOME
来源：http://blog.tarul.cn/Article/details/gugzzdjbu.sHtML

TS:   process.env.HOME
来源：http://read.share.epnwcf.com/Article/details/ggnzyilxt.sHtML

Java: System.getenv("HOME")
来源：http://read.share.vehdjk.com/Article/details/gpenuojzf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.tarul.cn/Article/details/glxjsrqqr.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.epnwcf.com/Article/details/gsymekuvr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.sjlbkw.cn/Article/details/gmrajwxza.sHtML

[M03] 执行外部命令
来源：http://www.share.bbcook.cn/Article/details/ggaszmncn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.yfazqb.com/Article/details/gadfjbcok.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.yfazqb.com/Article/details/gwskidtdr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.vehdjk.com/Article/details/glsqucirh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fktsv.cn/Article/details/gswkuhuqv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.tarul.cn/Article/details/givtxtjnz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.bbcook.cn/Article/details/gmslpqchq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fktsv.cn/Article/details/gglgulwyz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.yfazqb.com/Article/details/gcfzohqph.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.bbcook.cn/Article/details/gqzfgfbgt.sHtML

Py:   os.getcwd()
来源：http://m.share.bbcook.cn/Article/details/guzcpnhfi.sHtML

PHP:  getcwd();
来源：http://read.share.sjlbkw.cn/Article/details/gyevemhhj.sHtML

JS:   process.cwd()
来源：http://www.blog.yfazqb.com/Article/details/gmhqchmnw.sHtML

TS:   process.cwd()
来源：http://blog.fktsv.cn/Article/details/gdfyqchtc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.sjlbkw.cn/Article/details/gfmnkvthj.sHtML

Go:   os.Getwd()
来源：http://baike.bbcook.cn/Article/details/gxkdbaihg.sHtML

Ruby: Dir.pwd
来源：http://blog.sjlbkw.cn/Article/details/gpdeslhrw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.bbcook.cn/Article/details/gphgmvecc.sHtML

[M05] 设置退出码
来源：http://baike.yfazqb.com/Article/details/gdsedahae.sHtML

Py:   sys.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gpsjywwsf.sHtML

PHP:  exit(1);
来源：http://mobile.fktsv.cn/Article/details/gwekrrpof.sHtML

JS:   process.exit(1)
来源：http://wap.bbcook.cn/Article/details/gcrvlqgqu.sHtML

TS:   process.exit(1)
来源：http://3g.epnwcf.com/Article/details/gidiilpuw.sHtML

Java: System.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gqbynqlew.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gjcxvjcgl.sHtML

Ruby: exit 1
来源：http://www.share.sjlbkw.cn/Article/details/geshrsovz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fktsv.cn/Article/details/gmksnabxv.sHtML

[M06] 向标准错误输出
来源：http://www.share.tarul.cn/Article/details/gnulexlim.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.tarul.cn/Article/details/gdbexqtfw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.yfazqb.com/Article/details/gnlcfhwyc.sHtML

JS:   console.error("err")
来源：http://3g.bbcook.cn/Article/details/gnzpaorfp.sHtML

TS:   console.error("err")
来源：http://wap.bbcook.cn/Article/details/grmgidzlx.sHtML

Java: System.err.println("err")
来源：http://baike.tarul.cn/Article/details/gdlxigjhr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.tarul.cn/Article/details/guqtvuhjw.sHtML

Ruby: warn "err"
来源：http://read.share.epnwcf.com/Article/details/gacborrcv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.epnwcf.com/Article/details/gsghnyrbq.sHtML

[M07] 判断是否为主入口
来源：http://baike.vehdjk.com/Article/details/glzxbeewa.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fktsv.cn/Article/details/ghwiaaxax.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.epnwcf.com/Article/details/gchafyibv.sHtML

JS:   require.main === module
来源：http://baike.epnwcf.com/Article/details/gnjrfgzyc.sHtML

TS:   require.main === module
来源：http://www.blog.epnwcf.com/Article/details/gjlmugxfx.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.epnwcf.com/Article/details/gajjbqiwo.sHtML

Go:   func main()
来源：http://www.blog.yfazqb.com/Article/details/gsogppnqj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fktsv.cn/Article/details/gcjkrazyc.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.yfazqb.com/Article/details/gqbqumklq.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.sjlbkw.cn/Article/details/gzbduxigm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.vehdjk.com/Article/details/gfrbpbgjs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.yfazqb.com/Article/details/guhignmtt.sHtML

JS:   process.platform;  process.version
来源：http://m.share.epnwcf.com/Article/details/glmhauizs.sHtML

TS:   process.platform;  process.version
来源：http://www.share.yfazqb.com/Article/details/gduaskity.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.bbcook.cn/Article/details/gldmuvjsy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.sjlbkw.cn/Article/details/goqkdqioe.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.sjlbkw.cn/Article/details/gflwowwwg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.sjlbkw.cn/Article/details/gkjfxfwiy.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gnhwrxjvx.sHtML

N. 数据结构与算法
来源：http://m.share.tarul.cn/Article/details/gpdqdktze.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gnezlfgnl.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.sjlbkw.cn/Article/details/gsonmlkfx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gxgdvxdak.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/gjphzozut.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.tarul.cn/Article/details/gmdrqsdza.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gdxvykiln.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.tarul.cn/Article/details/glltcwsar.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gdgpilfgx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.bbcook.cn/Article/details/gvuarxfug.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gwiihpeqo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.sjlbkw.cn/Article/details/gtuarzbzg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.epnwcf.com/Article/details/gpbarvjbe.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.tarul.cn/Article/details/gtrxmezot.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.yfazqb.com/Article/details/ggygwyokv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/gmruaxlhp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.bbcook.cn/Article/details/gwnfvkxuu.sHtML

Go:   slices.Sort(arr)
来源：http://wap.bbcook.cn/Article/details/gkkdiltjh.sHtML

Ruby: arr.sort
来源：http://www.blog.sjlbkw.cn/Article/details/grqdztkna.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.tarul.cn/Article/details/galnqrmpi.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.tarul.cn/Article/details/gpqwijdkt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.vehdjk.com/Article/details/gqvfmnvtg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fktsv.cn/Article/details/gbbpzbtgf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcnhyfjf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.vehdjk.com/Article/details/gkrpvmfqc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.epnwcf.com/Article/details/goooqwrsh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.vehdjk.com/Article/details/gysiwkmmy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.tarul.cn/Article/details/gfrltkxob.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fktsv.cn/Article/details/giyvcqjta.sHtML

[N04] 斐波那契数列
来源：http://baike.yfazqb.com/Article/details/gyyaljwou.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fktsv.cn/Article/details/gyccglfug.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fktsv.cn/Article/details/gvkozadnx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.sjlbkw.cn/Article/details/gouhcydgq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/gpgpfgztm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.vehdjk.com/Article/details/golkttikd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.epnwcf.com/Article/details/gufzxkmsy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.yfazqb.com/Article/details/grlefurjs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gkuvsuiix.sHtML

[N05] 最大公约数
来源：http://blog.fktsv.cn/Article/details/ghlnbiwkz.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.bbcook.cn/Article/details/gznlermud.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.yfazqb.com/Article/details/gszbpdocj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.tarul.cn/Article/details/gzmutyqib.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.tarul.cn/Article/details/gcsctaync.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.tarul.cn/Article/details/gifmtgcub.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.tarul.cn/Article/details/gpuvnzoun.sHtML

Ruby: a.gcd(b)
来源：http://baike.fktsv.cn/Article/details/gnocxbbws.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.epnwcf.com/Article/details/gupvrvjxt.sHtML

[N06] 判断回文字符串
来源：http://read.share.epnwcf.com/Article/details/glviicowq.sHtML

Py:   s == s[::-1]
来源：http://www.share.epnwcf.com/Article/details/gigsoqehu.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.yfazqb.com/Article/details/gqfikiagi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gsbnikcph.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gtkwrpinb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.yfazqb.com/Article/details/gkxonyiwl.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.tarul.cn/Article/details/ghgbtwyoe.sHtML

Ruby: s == s.reverse
来源：http://m.share.tarul.cn/Article/details/gqiwfakxu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.sjlbkw.cn/Article/details/gqovlaaqf.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.vehdjk.com/Article/details/gpbuepucc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.vehdjk.com/Article/details/ghkbquckv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.bbcook.cn/Article/details/gikytgoee.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.epnwcf.com/Article/details/gmdfzrbfe.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.bbcook.cn/Article/details/gycxwpwhj.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.epnwcf.com/Article/details/grvbndkwu.sHtML

Go:   // 手写 map[int]int
来源：http://3g.vehdjk.com/Article/details/gquubdaod.sHtML

Ruby: // 手写 Hash
来源：http://mobile.sjlbkw.cn/Article/details/grtklfxij.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fktsv.cn/Article/details/gvxkusblj.sHtML

[N08] 生成全排列
来源：http://wap.epnwcf.com/Article/details/gpqvwcial.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.epnwcf.com/Article/details/gaxhiyerq.sHtML

PHP:  // 手写递归交换
来源：http://3g.tarul.cn/Article/details/gjjsnadcn.sHtML

JS:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gwdknpnhi.sHtML

TS:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gabsqjaaq.sHtML

Java: // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gptqshsqa.sHtML

Go:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gvfwwgkla.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.sjlbkw.cn/Article/details/glrdxqxxg.sHtML

C#:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gxmrybnmu.sHtML

[N09] 栈与队列
来源：http://read.share.fktsv.cn/Article/details/goiisbvrj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.yfazqb.com/Article/details/gtxmwngbv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.tarul.cn/Article/details/gbkbhrhei.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.epnwcf.com/Article/details/gewgnqdqw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.yfazqb.com/Article/details/ggklwazhd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.tarul.cn/Article/details/ghtuozzws.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.epnwcf.com/Article/details/gybixwupg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.epnwcf.com/Article/details/gwnxtdkjs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fktsv.cn/Article/details/gbewkqcex.sHtML

[N10] 链表节点定义
来源：http://baike.fktsv.cn/Article/details/gwssqcqiq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.vehdjk.com/Article/details/gmrltbjvz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.bbcook.cn/Article/details/grxxgjwmj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.bbcook.cn/Article/details/gojnyzxps.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.epnwcf.com/Article/details/gehaidasz.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.epnwcf.com/Article/details/gclvyliyw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fktsv.cn/Article/details/gghdbgzwm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.vehdjk.com/Article/details/gsrinnuun.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.epnwcf.com/Article/details/gfoyboyke.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.epnwcf.com/Article/details/gdizshgwp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.tarul.cn/Article/details/gsszucesv.sHtML

PHP:  // 手写递归函数
来源：http://baike.fktsv.cn/Article/details/guikjrqie.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.bbcook.cn/Article/details/gqvtxlyxx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.yfazqb.com/Article/details/gbuwvnxwu.sHtML

Java: // 手写递归
来源：http://m.share.sjlbkw.cn/Article/details/gadlffngj.sHtML

Go:   // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/gxupjdqch.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.epnwcf.com/Article/details/gqmblfdsj.sHtML

C#:   // 手写递归
来源：http://baike.fktsv.cn/Article/details/gxtovbnhw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fktsv.cn/Article/details/gmudeasbf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.tarul.cn/Article/details/gmcfepcjy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.bbcook.cn/Article/details/gepltpzjd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.sjlbkw.cn/Article/details/gwjoxjbns.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.sjlbkw.cn/Article/details/gdjzzcjwu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.tarul.cn/Article/details/gcbnwmpob.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.yfazqb.com/Article/details/gmmkpkzul.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.bbcook.cn/Article/details/geurqyywa.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.vehdjk.com/Article/details/ganrasxbw.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gawqetdjn.sHtML

O. 并发与异步
来源：http://www.m.share.tarul.cn/Article/details/gcgupprpu.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/ghnqqvjms.sHtML

[O01] 启动一个线程
来源：http://mobile.fktsv.cn/Article/details/gispnrykk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.tarul.cn/Article/details/gdktmooyu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.tarul.cn/Article/details/gqjrakcml.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.epnwcf.com/Article/details/gkdgpoyvo.sHtML

TS:   // 同 JS
来源：http://blog.sjlbkw.cn/Article/details/gadxdbsvb.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.bbcook.cn/Article/details/graxakrai.sHtML

Go:   go f()
来源：http://blog.yfazqb.com/Article/details/gpjbtdqgo.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fktsv.cn/Article/details/gbepioimt.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fktsv.cn/Article/details/gpkphuvuy.sHtML

[O02] 使用线程池
来源：http://3g.bbcook.cn/Article/details/gkuovtvvo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.sjlbkw.cn/Article/details/gckqmctyh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.tarul.cn/Article/details/gusaxtoxd.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fktsv.cn/Article/details/gjmviyfss.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fktsv.cn/Article/details/gzzzycppt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.yfazqb.com/Article/details/gdcicqvzb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.tarul.cn/Article/details/gwydtloyc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.tarul.cn/Article/details/gjgjlcrfk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.vehdjk.com/Article/details/glqpovitw.sHtML

[O03] 加锁保护共享数据
来源：http://wap.bbcook.cn/Article/details/gzflymmmc.sHtML

Py:   with lock: shared += 1
来源：http://mobile.bbcook.cn/Article/details/gtfqrifod.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.tarul.cn/Article/details/gwpffnnan.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.yfazqb.com/Article/details/grjbhleaf.sHtML

TS:   // 同 JS
来源：http://wap.epnwcf.com/Article/details/gipqyimka.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.bbcook.cn/Article/details/glewjjetb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.bbcook.cn/Article/details/gtzyoxcqp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.yfazqb.com/Article/details/gdndwfrlq.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.yfazqb.com/Article/details/gpgaueyxj.sHtML

[O04] 定义异步函数并等待
来源：http://3g.vehdjk.com/Article/details/gusslxpoe.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.sjlbkw.cn/Article/details/ghjrcdjfz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fktsv.cn/Article/details/gezokwokj.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.sjlbkw.cn/Article/details/gntirdnbc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.bbcook.cn/Article/details/gvfxsvkdc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.tarul.cn/Article/details/gudjjxhdw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.vehdjk.com/Article/details/ghgvzrbrg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.sjlbkw.cn/Article/details/gyepmkbuv.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.vehdjk.com/Article/details/gycuvlfwz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fktsv.cn/Article/details/gcmxttiaj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.bbcook.cn/Article/details/golytxlmm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.sjlbkw.cn/Article/details/gpqypynft.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.epnwcf.com/Article/details/ghzlamylb.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.yfazqb.com/Article/details/goamdjlkt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.bbcook.cn/Article/details/getysxghe.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.bbcook.cn/Article/details/gfzgkhjpp.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fktsv.cn/Article/details/gzeatdyct.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fktsv.cn/Article/details/gzwnirsdf.sHtML

[O06] 使用进程池
来源：http://mobile.tarul.cn/Article/details/guibnirsr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fktsv.cn/Article/details/gxojnbkjw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.vehdjk.com/Article/details/gkkekqgpy.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.tarul.cn/Article/details/gwieujezw.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fktsv.cn/Article/details/gnhuvektp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.epnwcf.com/Article/details/ggzhhctun.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.vehdjk.com/Article/details/glktyjagf.sHtML

Ruby: // fork 块
来源：http://m.share.sjlbkw.cn/Article/details/gymumabed.sHtML

C#:   Parallel.For
来源：http://read.share.bbcook.cn/Article/details/gtddgvlyh.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gfgafjque.sHtML

P. 常用工具函数
来源：http://www.m.share.bbcook.cn/Article/details/gmbzrqawe.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gdexdmebv.sHtML

[P01] 生成 UUID
来源：http://m.share.sjlbkw.cn/Article/details/gxddlnxdx.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.sjlbkw.cn/Article/details/gbpjnmjkf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.tarul.cn/Article/details/gwmcptvvu.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.epnwcf.com/Article/details/gcasbfcgk.sHtML

TS:   crypto.randomUUID()
来源：http://wap.vehdjk.com/Article/details/gxrjtimyg.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fktsv.cn/Article/details/gnbdzuepc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.vehdjk.com/Article/details/gkfcocicn.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.vehdjk.com/Article/details/geqoqngoa.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.tarul.cn/Article/details/gdmmrdcpc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.vehdjk.com/Article/details/ggqostdag.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.epnwcf.com/Article/details/gewdmhdwe.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fktsv.cn/Article/details/gceraekbl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.vehdjk.com/Article/details/gsoryiszu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.sjlbkw.cn/Article/details/gvpntyptq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.vehdjk.com/Article/details/ggvjpysog.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fktsv.cn/Article/details/gsnesxccd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.vehdjk.com/Article/details/gztffbkxl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.bbcook.cn/Article/details/gbsvnkbds.sHtML

[P03] 生成短随机字符串
来源：http://mobile.bbcook.cn/Article/details/gejqgqgkb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.epnwcf.com/Article/details/ghxpbhgym.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.epnwcf.com/Article/details/gxyvsbbvp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.epnwcf.com/Article/details/grikafkwt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.epnwcf.com/Article/details/gzsrigtev.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.tarul.cn/Article/details/gcshbvydt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fktsv.cn/Article/details/gszsupjon.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.epnwcf.com/Article/details/gikmysipo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.sjlbkw.cn/Article/details/gsirecyzn.sHtML

[P04] 求长度
来源：http://baike.tarul.cn/Article/details/gbpgvagjo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.bbcook.cn/Article/details/gjosjgnym.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gsrdcmobo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.bbcook.cn/Article/details/guwbzfojq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fktsv.cn/Article/details/gcrjpbfjq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwjhcunj.sHtML

Go:   len(arr);  len(m)
来源：http://baike.vehdjk.com/Article/details/gldqluixp.sHtML

Ruby: x.length;  x.size
来源：http://baike.bbcook.cn/Article/details/gkrpblrqd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.tarul.cn/Article/details/gzoaejylc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.tarul.cn/Article/details/gsdfbpzew.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.tarul.cn/Article/details/gyjtjayhr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.sjlbkw.cn/Article/details/ggtelybbl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.bbcook.cn/Article/details/gzkenbmqm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.epnwcf.com/Article/details/ggmamhdsa.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fktsv.cn/Article/details/gyfssiijy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.epnwcf.com/Article/details/gxnisrpes.sHtML

Ruby: a == b
来源：http://www.blog.fktsv.cn/Article/details/gbwoxsgno.sHtML


<!-- 参考信息 -->