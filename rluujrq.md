代发 wailian999

TS:   resp.ok;  resp.status
来源：http://www.share.fktsv.cn/Article/details/gcuegsxts.sHtML

Java: resp.statusCode()
来源：http://blog.bbcook.cn/Article/details/gsqloczkd.sHtML

Go:   resp.StatusCode
来源：http://3g.tarul.cn/Article/details/gftzwnmil.sHtML

Ruby: resp.code.to_i
来源：http://read.share.vehdjk.com/Article/details/gocqlgfds.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fktsv.cn/Article/details/giucempic.sHtML

[L08] 并发请求多个地址
来源：http://baike.vehdjk.com/Article/details/ghchtnqvz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.epnwcf.com/Article/details/gfaoliryg.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fktsv.cn/Article/details/glzjognqr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/gyvxoijei.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fktsv.cn/Article/details/gssignohe.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fktsv.cn/Article/details/gjkmedtgx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fktsv.cn/Article/details/gmejvnpub.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.epnwcf.com/Article/details/gtetshjjj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.yfazqb.com/Article/details/gsxoeryme.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gaqnarlwm.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.yfazqb.com/Article/details/gciviqvkw.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gkrygrdwv.sHtML

[M01] 读取命令行参数
来源：http://3g.yfazqb.com/Article/details/gxbrkkjit.sHtML

Py:   sys.argv[1:]
来源：http://wap.sjlbkw.cn/Article/details/gxuoglidn.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.bbcook.cn/Article/details/ghvzfsmta.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.tarul.cn/Article/details/gtedegcko.sHtML

TS:   process.argv.slice(2)
来源：http://3g.epnwcf.com/Article/details/gapysagdn.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fktsv.cn/Article/details/gfytgczsg.sHtML

Go:   os.Args[1:]
来源：http://read.share.epnwcf.com/Article/details/gvhcxllki.sHtML

Ruby: ARGV
来源：http://www.share.fktsv.cn/Article/details/gobadxvxs.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.bbcook.cn/Article/details/gopzbknws.sHtML

[M02] 读取环境变量
来源：http://www.m.share.tarul.cn/Article/details/ghjnzbtda.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhutoqll.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.vehdjk.com/Article/details/gdzfgmwam.sHtML

JS:   process.env.HOME
来源：http://www.m.share.yfazqb.com/Article/details/gmvcwugwf.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fktsv.cn/Article/details/ghuehtorw.sHtML

Java: System.getenv("HOME")
来源：http://read.share.bbcook.cn/Article/details/gjosdminz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gvdidnxvr.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.vehdjk.com/Article/details/gdqdipevv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fktsv.cn/Article/details/gxdzawnmq.sHtML

[M03] 执行外部命令
来源：http://wap.yfazqb.com/Article/details/ggvolzjez.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fktsv.cn/Article/details/gazaevsem.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.epnwcf.com/Article/details/garsdeiqb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.vehdjk.com/Article/details/gvxrarilw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.yfazqb.com/Article/details/gqkujjdit.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.tarul.cn/Article/details/gsdasdfgy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fktsv.cn/Article/details/giytjuyix.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fktsv.cn/Article/details/gzvwpdztu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.bbcook.cn/Article/details/gnwakymlu.sHtML

[M04] 获取当前工作目录
来源：http://3g.yfazqb.com/Article/details/gdvvnevuw.sHtML

Py:   os.getcwd()
来源：http://mobile.yfazqb.com/Article/details/garmgshqj.sHtML

PHP:  getcwd();
来源：http://www.blog.epnwcf.com/Article/details/galjiiynm.sHtML

JS:   process.cwd()
来源：http://blog.fktsv.cn/Article/details/gqtgpmfbe.sHtML

TS:   process.cwd()
来源：http://3g.vehdjk.com/Article/details/gjscopqpa.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.tarul.cn/Article/details/gpcrzacbz.sHtML

Go:   os.Getwd()
来源：http://blog.yfazqb.com/Article/details/gnkfvkdnu.sHtML

Ruby: Dir.pwd
来源：http://mobile.yfazqb.com/Article/details/glsiagkco.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.sjlbkw.cn/Article/details/grshrxhyi.sHtML

[M05] 设置退出码
来源：http://blog.vehdjk.com/Article/details/gzxrqvnyy.sHtML

Py:   sys.exit(1)
来源：http://wap.yfazqb.com/Article/details/gbrwdpymh.sHtML

PHP:  exit(1);
来源：http://www.share.yfazqb.com/Article/details/gpzkrtbat.sHtML

JS:   process.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gmszqvmhr.sHtML

TS:   process.exit(1)
来源：http://mobile.epnwcf.com/Article/details/gfvydidju.sHtML

Java: System.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gpwpuinbv.sHtML

Go:   os.Exit(1)
来源：http://mobile.bbcook.cn/Article/details/ggufjxhmt.sHtML

Ruby: exit 1
来源：http://read.share.vehdjk.com/Article/details/gngkvygnb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fktsv.cn/Article/details/ggcmsqymm.sHtML

[M06] 向标准错误输出
来源：http://mobile.yfazqb.com/Article/details/gszaomjna.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.tarul.cn/Article/details/gstpkfefc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fktsv.cn/Article/details/gzplniwtp.sHtML

JS:   console.error("err")
来源：http://read.share.fktsv.cn/Article/details/gywmpfpnz.sHtML

TS:   console.error("err")
来源：http://m.share.yfazqb.com/Article/details/gaiojnccb.sHtML

Java: System.err.println("err")
来源：http://www.blog.vehdjk.com/Article/details/gyocbctkx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.yfazqb.com/Article/details/gkcztvtzy.sHtML

Ruby: warn "err"
来源：http://3g.tarul.cn/Article/details/gfriwmlai.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.yfazqb.com/Article/details/ghpxzsrsy.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.bbcook.cn/Article/details/gzmyrbkwb.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.tarul.cn/Article/details/gbcluwank.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.tarul.cn/Article/details/gmiboqhog.sHtML

JS:   require.main === module
来源：http://read.share.bbcook.cn/Article/details/gvrdegzkf.sHtML

TS:   require.main === module
来源：http://www.share.yfazqb.com/Article/details/gbbkvlmup.sHtML

Java: public static void main(String[] args)
来源：http://www.share.vehdjk.com/Article/details/gwurnzrcl.sHtML

Go:   func main()
来源：http://read.share.sjlbkw.cn/Article/details/gqhflgbjz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.epnwcf.com/Article/details/gudjdthao.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fktsv.cn/Article/details/gdrvzjrlw.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.epnwcf.com/Article/details/gqozatysk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fktsv.cn/Article/details/gohgyiqtm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.epnwcf.com/Article/details/ggnbdwtey.sHtML

JS:   process.platform;  process.version
来源：http://read.share.epnwcf.com/Article/details/gcqrcbpbe.sHtML

TS:   process.platform;  process.version
来源：http://baike.bbcook.cn/Article/details/gmmnqzylb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fktsv.cn/Article/details/gnmnermsr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.epnwcf.com/Article/details/glyasrxro.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.bbcook.cn/Article/details/gygugzbaz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.epnwcf.com/Article/details/ghlckikbf.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gkbovfcte.sHtML

N. 数据结构与算法
来源：http://baike.sjlbkw.cn/Article/details/gpqyeksus.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gozpepxnk.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.bbcook.cn/Article/details/graldxxrm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.tarul.cn/Article/details/grrxsvndo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fktsv.cn/Article/details/ghbbszdzj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fktsv.cn/Article/details/gaabkqmvm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.vehdjk.com/Article/details/gjoxesvnu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gqeblflvk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.tarul.cn/Article/details/gdvntxpml.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.epnwcf.com/Article/details/gzdlgzonn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gezpxaazr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.sjlbkw.cn/Article/details/gkzyoukhf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.vehdjk.com/Article/details/gqwyenhbf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.epnwcf.com/Article/details/grnxfixzb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.vehdjk.com/Article/details/gsksktbpu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.vehdjk.com/Article/details/gocvzipql.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.vehdjk.com/Article/details/gypljxvwj.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmsmypczq.sHtML

Ruby: arr.sort
来源：http://www.m.share.tarul.cn/Article/details/gkqrxkbvp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.sjlbkw.cn/Article/details/glclkuxui.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.sjlbkw.cn/Article/details/geethhsfr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fktsv.cn/Article/details/gqjtliaxk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fktsv.cn/Article/details/gzahjyozw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.sjlbkw.cn/Article/details/guiglvoyo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.yfazqb.com/Article/details/gnggjzljt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.yfazqb.com/Article/details/gppsvtkwi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.epnwcf.com/Article/details/gqoqbaeue.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.epnwcf.com/Article/details/gcfktjqqj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fktsv.cn/Article/details/gduiywgvb.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fktsv.cn/Article/details/gwuucfses.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.tarul.cn/Article/details/gbmlfsbed.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.tarul.cn/Article/details/gpllurbqv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.vehdjk.com/Article/details/gulgjoawf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/gwxmlfmyo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.epnwcf.com/Article/details/gwqbtiopz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fktsv.cn/Article/details/gbygdxbrj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.epnwcf.com/Article/details/gbdgenzpv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.yfazqb.com/Article/details/gyvuzpksd.sHtML

[N05] 最大公约数
来源：http://wap.sjlbkw.cn/Article/details/gfyaoulkr.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.yfazqb.com/Article/details/gfhtlmigy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gmfsofikx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gieezagll.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.tarul.cn/Article/details/gxvqafprc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.vehdjk.com/Article/details/gvlonxbrv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.tarul.cn/Article/details/grpuprmsb.sHtML

Ruby: a.gcd(b)
来源：http://m.share.vehdjk.com/Article/details/ggxfebmxg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.vehdjk.com/Article/details/gsaxeqlqr.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.yfazqb.com/Article/details/gxcdqtlcl.sHtML

Py:   s == s[::-1]
来源：http://read.share.tarul.cn/Article/details/gzkbwfogl.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fktsv.cn/Article/details/gmmoicmeg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gmawmwmop.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.vehdjk.com/Article/details/ghdwrfskq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.vehdjk.com/Article/details/gqpmansvy.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.tarul.cn/Article/details/gijtfkrwt.sHtML

Ruby: s == s.reverse
来源：http://wap.fktsv.cn/Article/details/gqztijozd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.bbcook.cn/Article/details/gushbhibu.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.tarul.cn/Article/details/gzzcpllwt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.yfazqb.com/Article/details/geotfhzid.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.tarul.cn/Article/details/gkxcnvkqm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.bbcook.cn/Article/details/gdvoiqwla.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.tarul.cn/Article/details/gkukkoayj.sHtML

Java: // 手写 HashMap
来源：http://www.share.vehdjk.com/Article/details/ggcoajvfe.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.sjlbkw.cn/Article/details/gnqkgtsje.sHtML

Ruby: // 手写 Hash
来源：http://m.share.bbcook.cn/Article/details/gpsufpdtr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.bbcook.cn/Article/details/gdwqaxdxq.sHtML

[N08] 生成全排列
来源：http://m.share.tarul.cn/Article/details/goculxeuh.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.yfazqb.com/Article/details/glzwofkwc.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fktsv.cn/Article/details/gjvzpzlcu.sHtML

JS:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gemomaigw.sHtML

TS:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gqsdptssa.sHtML

Java: // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/giinsqlkk.sHtML

Go:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/ggjbjstto.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.sjlbkw.cn/Article/details/gtiqprsfn.sHtML

C#:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gkwtrwgar.sHtML

[N09] 栈与队列
来源：http://www.share.fktsv.cn/Article/details/gqlvwqpbz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.vehdjk.com/Article/details/gasfnfefy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.bbcook.cn/Article/details/gabgulnrv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.sjlbkw.cn/Article/details/gkriqhzny.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.sjlbkw.cn/Article/details/guqnfxpna.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.bbcook.cn/Article/details/gcjqmamug.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.sjlbkw.cn/Article/details/gznypojyn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fktsv.cn/Article/details/ghblucgil.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.sjlbkw.cn/Article/details/gijmyhvyj.sHtML

[N10] 链表节点定义
来源：http://3g.vehdjk.com/Article/details/gbhkdotwg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.epnwcf.com/Article/details/gfobxlwbl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.epnwcf.com/Article/details/gtrofzuzq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.sjlbkw.cn/Article/details/giqxtqcff.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fktsv.cn/Article/details/gbtkplhla.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.vehdjk.com/Article/details/ghyipfmpb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.sjlbkw.cn/Article/details/gakuxrmya.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.tarul.cn/Article/details/grauyonyc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.sjlbkw.cn/Article/details/gstylbcyw.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.vehdjk.com/Article/details/gqrdqdxxx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.yfazqb.com/Article/details/gkwrflgqn.sHtML

PHP:  // 手写递归函数
来源：http://3g.yfazqb.com/Article/details/gpiwmtvsk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.yfazqb.com/Article/details/goylfvahn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.sjlbkw.cn/Article/details/ghiucyeel.sHtML

Java: // 手写递归
来源：http://baike.bbcook.cn/Article/details/gprtzbtrf.sHtML

Go:   // 手写递归
来源：http://blog.tarul.cn/Article/details/gjqfezgfv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.vehdjk.com/Article/details/gzhadrseu.sHtML

C#:   // 手写递归
来源：http://m.share.fktsv.cn/Article/details/grawohowy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fktsv.cn/Article/details/gejlfwrgd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fktsv.cn/Article/details/gmaqesonj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.tarul.cn/Article/details/ghnqpddom.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.bbcook.cn/Article/details/ggtxqygvi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.tarul.cn/Article/details/gcxgqiapu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.vehdjk.com/Article/details/gwgmskmcu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.sjlbkw.cn/Article/details/gdoqiuioe.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.yfazqb.com/Article/details/gjivwjdzp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.sjlbkw.cn/Article/details/gxoomgdbj.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gskfzmdcf.sHtML

O. 并发与异步
来源：http://3g.sjlbkw.cn/Article/details/gceouuvaj.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gmcsjcwkg.sHtML

[O01] 启动一个线程
来源：http://baike.tarul.cn/Article/details/gmggqnunw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.bbcook.cn/Article/details/ggpoxzrrh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.yfazqb.com/Article/details/gvkgiruzm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fktsv.cn/Article/details/gffoopico.sHtML

TS:   // 同 JS
来源：http://www.blog.bbcook.cn/Article/details/gaxhunlap.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.bbcook.cn/Article/details/gagamvygd.sHtML

Go:   go f()
来源：http://www.blog.vehdjk.com/Article/details/gvwinjfot.sHtML

Ruby: Thread.new { f }
来源：http://blog.tarul.cn/Article/details/gwdhomyor.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fktsv.cn/Article/details/guzdwdvva.sHtML

[O02] 使用线程池
来源：http://www.blog.fktsv.cn/Article/details/grkhmhmua.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.bbcook.cn/Article/details/guxynnitb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.yfazqb.com/Article/details/gluadgfmv.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.yfazqb.com/Article/details/gyktqtqpf.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.tarul.cn/Article/details/gdqfzxwxv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.sjlbkw.cn/Article/details/giwgnbise.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.bbcook.cn/Article/details/gmhymysje.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.vehdjk.com/Article/details/gnjfibrxr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.bbcook.cn/Article/details/gozrlwfzz.sHtML

[O03] 加锁保护共享数据
来源：http://baike.epnwcf.com/Article/details/gaqdvvucb.sHtML

Py:   with lock: shared += 1
来源：http://read.share.tarul.cn/Article/details/guxbplytl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.epnwcf.com/Article/details/gapxflyrw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.epnwcf.com/Article/details/gxxubgvoc.sHtML

TS:   // 同 JS
来源：http://read.share.tarul.cn/Article/details/gehnvovpc.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.sjlbkw.cn/Article/details/gcsuonlyy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.tarul.cn/Article/details/gapldmver.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.yfazqb.com/Article/details/gkvewdoek.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.vehdjk.com/Article/details/gmqrkddui.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.tarul.cn/Article/details/gqqsvhvsd.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.vehdjk.com/Article/details/gxpncsgkm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.epnwcf.com/Article/details/gitrnkygd.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fktsv.cn/Article/details/gpzngufcr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.epnwcf.com/Article/details/gamsrjmkp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fktsv.cn/Article/details/ghejdgwxw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.yfazqb.com/Article/details/gutdnlvuq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.tarul.cn/Article/details/gcsrrdmmz.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fktsv.cn/Article/details/gpktvqxod.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fktsv.cn/Article/details/gtvlklifj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.sjlbkw.cn/Article/details/gzyeuchmi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.vehdjk.com/Article/details/ghqnonkcb.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.tarul.cn/Article/details/gdfcunyix.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.yfazqb.com/Article/details/gfofxkmtw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.bbcook.cn/Article/details/gmvikmcqy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.tarul.cn/Article/details/gneaiyrit.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.yfazqb.com/Article/details/goughniti.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.bbcook.cn/Article/details/gsxwrulbk.sHtML

[O06] 使用进程池
来源：http://www.share.yfazqb.com/Article/details/gnvchldbe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.vehdjk.com/Article/details/gcdetfkja.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.sjlbkw.cn/Article/details/gwibzvqdk.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.bbcook.cn/Article/details/gikslsewi.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.sjlbkw.cn/Article/details/gmnqmtwxx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.bbcook.cn/Article/details/gdtqfdcmo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fktsv.cn/Article/details/gdirgqlsf.sHtML

Ruby: // fork 块
来源：http://blog.epnwcf.com/Article/details/gekcweapv.sHtML

C#:   Parallel.For
来源：http://baike.bbcook.cn/Article/details/gjctdwiha.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gecnufnxm.sHtML

P. 常用工具函数
来源：http://www.blog.tarul.cn/Article/details/gggqajzuy.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gwyjslblt.sHtML

[P01] 生成 UUID
来源：http://mobile.vehdjk.com/Article/details/gxjsaduli.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fktsv.cn/Article/details/gtkbmkzwo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.tarul.cn/Article/details/gzmehopwn.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/greowxaqa.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.bbcook.cn/Article/details/gcmhzuega.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.bbcook.cn/Article/details/gvankursl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.sjlbkw.cn/Article/details/gixzphdrm.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.vehdjk.com/Article/details/gfxowyxkt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.vehdjk.com/Article/details/gucpjwvza.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.tarul.cn/Article/details/gdlxkiczr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fktsv.cn/Article/details/gyvjzrlln.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.sjlbkw.cn/Article/details/gsojoepoj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.sjlbkw.cn/Article/details/gqlnbbikv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.epnwcf.com/Article/details/gixpipqou.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.yfazqb.com/Article/details/gcxknjqqt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.tarul.cn/Article/details/gaqrbkrhz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.tarul.cn/Article/details/gbuzmmlth.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.tarul.cn/Article/details/gxaiooddt.sHtML

[P03] 生成短随机字符串
来源：http://m.share.vehdjk.com/Article/details/gbnpowpdq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.tarul.cn/Article/details/gsnhsvfcf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.epnwcf.com/Article/details/gwlwyhjia.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.yfazqb.com/Article/details/gawqjjxum.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.epnwcf.com/Article/details/grdosvtvx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.yfazqb.com/Article/details/gltjwceke.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.yfazqb.com/Article/details/gtkvznjpt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.vehdjk.com/Article/details/gzevvcwcb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.vehdjk.com/Article/details/gupcgyahp.sHtML

[P04] 求长度
来源：http://www.blog.fktsv.cn/Article/details/gsjcdkmrx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.epnwcf.com/Article/details/gdydvgzbk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gyccmmver.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.yfazqb.com/Article/details/gaekjjqyl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.bbcook.cn/Article/details/glfwauxzf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.bbcook.cn/Article/details/gtjkzyvaw.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fktsv.cn/Article/details/gjejriuoy.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.tarul.cn/Article/details/gtjsfkxxr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fktsv.cn/Article/details/gwjuseygh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.tarul.cn/Article/details/gzvlcgtlg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.epnwcf.com/Article/details/gfurkkmsk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fktsv.cn/Article/details/gfavopccy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.bbcook.cn/Article/details/ghiphrsva.sHtML


<!-- 参考信息 -->