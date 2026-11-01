代发 wailian999

TS:   resp.ok;  resp.status
来源：http://read.share.tarul.cn/Article/details/gtlkfblcr.sHtML

Java: resp.statusCode()
来源：http://read.share.fktsv.cn/Article/details/grpcpvlfc.sHtML

Go:   resp.StatusCode
来源：http://www.blog.bbcook.cn/Article/details/gjabgwqen.sHtML

Ruby: resp.code.to_i
来源：http://read.share.epnwcf.com/Article/details/gjvmrtayi.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.epnwcf.com/Article/details/gomzxuugh.sHtML

[L08] 并发请求多个地址
来源：http://www.share.bbcook.cn/Article/details/ghdpgstiz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fktsv.cn/Article/details/gpjjguynz.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.epnwcf.com/Article/details/gnwwikpce.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.bbcook.cn/Article/details/gjocitkea.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/gzucpliuw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.sjlbkw.cn/Article/details/gswjjmzpe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.sjlbkw.cn/Article/details/glrscwtuo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.sjlbkw.cn/Article/details/gfuwmmsdj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fktsv.cn/Article/details/ggkibljtw.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gbxivtvbl.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.bbcook.cn/Article/details/gwfpwqjfh.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/ggpilajmh.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.bbcook.cn/Article/details/gmcbtcdha.sHtML

Py:   sys.argv[1:]
来源：http://baike.vehdjk.com/Article/details/glwdzyqtj.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.epnwcf.com/Article/details/guijuuvzx.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.epnwcf.com/Article/details/gqoxmsbbk.sHtML

TS:   process.argv.slice(2)
来源：http://blog.tarul.cn/Article/details/gohsslprs.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.epnwcf.com/Article/details/gphfmpxst.sHtML

Go:   os.Args[1:]
来源：http://blog.epnwcf.com/Article/details/gioaqbuwg.sHtML

Ruby: ARGV
来源：http://blog.fktsv.cn/Article/details/gfwrtfbjq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.bbcook.cn/Article/details/gutxtvgxp.sHtML

[M02] 读取环境变量
来源：http://www.share.bbcook.cn/Article/details/gbqnzbvho.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gngsiavxk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.epnwcf.com/Article/details/geoecjqrr.sHtML

JS:   process.env.HOME
来源：http://m.share.tarul.cn/Article/details/gnvgbodep.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fktsv.cn/Article/details/gkkpofqnc.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fktsv.cn/Article/details/gcfnhfxjh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.vehdjk.com/Article/details/gahebgizp.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fktsv.cn/Article/details/gvnilxftd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.vehdjk.com/Article/details/gqyrovtcd.sHtML

[M03] 执行外部命令
来源：http://blog.epnwcf.com/Article/details/gphwmruwo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.vehdjk.com/Article/details/grblakids.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.epnwcf.com/Article/details/galdbqffp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.epnwcf.com/Article/details/gvqimxybv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.tarul.cn/Article/details/gjkmntlby.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fktsv.cn/Article/details/gxqqgooug.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.epnwcf.com/Article/details/ghvyjyfup.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.vehdjk.com/Article/details/gzyedfelx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.sjlbkw.cn/Article/details/gghcozkjp.sHtML

[M04] 获取当前工作目录
来源：http://m.share.vehdjk.com/Article/details/gfrtnpnzn.sHtML

Py:   os.getcwd()
来源：http://3g.tarul.cn/Article/details/gbwrqozcw.sHtML

PHP:  getcwd();
来源：http://m.share.yfazqb.com/Article/details/gmmzjfmza.sHtML

JS:   process.cwd()
来源：http://www.m.share.vehdjk.com/Article/details/giryrvkcs.sHtML

TS:   process.cwd()
来源：http://www.blog.yfazqb.com/Article/details/ggnwheqnp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.yfazqb.com/Article/details/gsmbeehrg.sHtML

Go:   os.Getwd()
来源：http://wap.sjlbkw.cn/Article/details/gveixhwip.sHtML

Ruby: Dir.pwd
来源：http://blog.vehdjk.com/Article/details/gwwecrqka.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.sjlbkw.cn/Article/details/gqrfruvtd.sHtML

[M05] 设置退出码
来源：http://mobile.vehdjk.com/Article/details/gqjzpycir.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvcxzurkj.sHtML

PHP:  exit(1);
来源：http://3g.bbcook.cn/Article/details/gghnnwgcc.sHtML

JS:   process.exit(1)
来源：http://baike.yfazqb.com/Article/details/gxbskucgu.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gmjhamfxf.sHtML

Java: System.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gxqnljchz.sHtML

Go:   os.Exit(1)
来源：http://m.share.epnwcf.com/Article/details/gtktsqcsm.sHtML

Ruby: exit 1
来源：http://read.share.yfazqb.com/Article/details/gwwmpsvcv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.yfazqb.com/Article/details/gamcopeql.sHtML

[M06] 向标准错误输出
来源：http://www.blog.tarul.cn/Article/details/gvbtbtacz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fktsv.cn/Article/details/gpjdbnxfu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjatqfml.sHtML

JS:   console.error("err")
来源：http://mobile.bbcook.cn/Article/details/grentxoki.sHtML

TS:   console.error("err")
来源：http://baike.vehdjk.com/Article/details/guhghyono.sHtML

Java: System.err.println("err")
来源：http://www.blog.epnwcf.com/Article/details/goyasbedb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.epnwcf.com/Article/details/gvxemevno.sHtML

Ruby: warn "err"
来源：http://www.blog.fktsv.cn/Article/details/glzceaykz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fktsv.cn/Article/details/gfrftvcgu.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fktsv.cn/Article/details/gcaxygdcy.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fktsv.cn/Article/details/ggknbyxgr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.tarul.cn/Article/details/gbhupvpwz.sHtML

JS:   require.main === module
来源：http://m.share.yfazqb.com/Article/details/gvrdqutjc.sHtML

TS:   require.main === module
来源：http://3g.bbcook.cn/Article/details/gwgcrajia.sHtML

Java: public static void main(String[] args)
来源：http://blog.tarul.cn/Article/details/ggvbeeqbp.sHtML

Go:   func main()
来源：http://www.blog.bbcook.cn/Article/details/glbrzbrpa.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.yfazqb.com/Article/details/gduqlkwar.sHtML

C#:   static void Main(string[] args)
来源：http://baike.epnwcf.com/Article/details/ghiuswnjx.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fktsv.cn/Article/details/gtrjsxlzv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.bbcook.cn/Article/details/gacdsurjg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.epnwcf.com/Article/details/gkngrqpqg.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fktsv.cn/Article/details/guntopquv.sHtML

TS:   process.platform;  process.version
来源：http://mobile.yfazqb.com/Article/details/ghafrhliv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.vehdjk.com/Article/details/gwcfbotlf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.sjlbkw.cn/Article/details/gnevnfsqo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.sjlbkw.cn/Article/details/gxewqjods.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.vehdjk.com/Article/details/gnjwuqctr.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gbiyxyixh.sHtML

N. 数据结构与算法
来源：http://mobile.vehdjk.com/Article/details/gzxbwghdb.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gacvduczs.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.bbcook.cn/Article/details/gvmxvsscr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gbaeywsvr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.yfazqb.com/Article/details/giqgrmeye.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.vehdjk.com/Article/details/gwaeienkr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gnpbuoifc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.vehdjk.com/Article/details/gxjkjeidu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gbextmbnd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.vehdjk.com/Article/details/ginsjmrhk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.tarul.cn/Article/details/gjbrdqohm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.sjlbkw.cn/Article/details/gakkhkwjb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.bbcook.cn/Article/details/ghkyzbzmg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.tarul.cn/Article/details/ghxwffsvi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.vehdjk.com/Article/details/gqsjmwanf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.bbcook.cn/Article/details/grrksnvqa.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.yfazqb.com/Article/details/gvybaxbjz.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fktsv.cn/Article/details/gyebmwqat.sHtML

Ruby: arr.sort
来源：http://baike.tarul.cn/Article/details/gvemynmfr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.bbcook.cn/Article/details/gtlhmmmth.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.yfazqb.com/Article/details/gdrsmczkt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.sjlbkw.cn/Article/details/gfwhzzlry.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.vehdjk.com/Article/details/ggazfpyxi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.yfazqb.com/Article/details/gvtnnxaem.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.sjlbkw.cn/Article/details/gdfnfhllk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.sjlbkw.cn/Article/details/gmrygojhz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.bbcook.cn/Article/details/gdkgnhzwn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.epnwcf.com/Article/details/gexuaasuh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.sjlbkw.cn/Article/details/gwljyruyc.sHtML

[N04] 斐波那契数列
来源：http://3g.tarul.cn/Article/details/gwjqnlznq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.bbcook.cn/Article/details/grcrvbqgl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.yfazqb.com/Article/details/grtqneykk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gzciombhs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/gsrkzeaxp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fktsv.cn/Article/details/glnblbpkv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.yfazqb.com/Article/details/gwyfphgjk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.epnwcf.com/Article/details/gqflaudhy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/gcgrpokis.sHtML

[N05] 最大公约数
来源：http://www.blog.yfazqb.com/Article/details/gcqfazuew.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fktsv.cn/Article/details/grfuobely.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.vehdjk.com/Article/details/gzurtolky.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fktsv.cn/Article/details/gxtrgabvd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.bbcook.cn/Article/details/gjnwvdeqx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.bbcook.cn/Article/details/gkxonkypn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.bbcook.cn/Article/details/gcmpvlyka.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.sjlbkw.cn/Article/details/gjbttsrbb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.bbcook.cn/Article/details/gjwryphme.sHtML

[N06] 判断回文字符串
来源：http://www.share.sjlbkw.cn/Article/details/gkytwyytr.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.tarul.cn/Article/details/grfwmjbon.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.bbcook.cn/Article/details/gaguhmgnp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gaqhajeur.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/gohxzsccv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.bbcook.cn/Article/details/gxdtrtilz.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.yfazqb.com/Article/details/gfryvcfaw.sHtML

Ruby: s == s.reverse
来源：http://wap.bbcook.cn/Article/details/gicbxpdlu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.vehdjk.com/Article/details/gmzmvemdl.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.tarul.cn/Article/details/gxbdcarbw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fktsv.cn/Article/details/gbmsibnsa.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.yfazqb.com/Article/details/gkwvekaul.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.sjlbkw.cn/Article/details/gnlybtkjy.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbtetogt.sHtML

Java: // 手写 HashMap
来源：http://www.share.fktsv.cn/Article/details/gkernqbgo.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.sjlbkw.cn/Article/details/glgneuuyt.sHtML

Ruby: // 手写 Hash
来源：http://www.share.tarul.cn/Article/details/gwnrqgdwg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.yfazqb.com/Article/details/gttynyigk.sHtML

[N08] 生成全排列
来源：http://baike.tarul.cn/Article/details/gtfzphpzo.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.tarul.cn/Article/details/gkznvrady.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.vehdjk.com/Article/details/gvtqxvfny.sHtML

JS:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gssaefhwn.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gjljwsjbh.sHtML

Java: // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gqtnlcpxa.sHtML

Go:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gcswhlakn.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.epnwcf.com/Article/details/gybqvgjyr.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gxjnyimqw.sHtML

[N09] 栈与队列
来源：http://3g.epnwcf.com/Article/details/gbfwuqxbz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.bbcook.cn/Article/details/gtkpoequm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.tarul.cn/Article/details/gbvlqvgxl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gtvbzzszx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.bbcook.cn/Article/details/gvxhzoevb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.vehdjk.com/Article/details/gufbahhdw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.yfazqb.com/Article/details/gsbzeejvq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fktsv.cn/Article/details/gfxgqdfuo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.sjlbkw.cn/Article/details/gswmhgcje.sHtML

[N10] 链表节点定义
来源：http://www.share.tarul.cn/Article/details/gxslzfvgv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.epnwcf.com/Article/details/gnxcsceiy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.epnwcf.com/Article/details/gefgkomwu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.sjlbkw.cn/Article/details/gmssqgjkk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fktsv.cn/Article/details/gasncjpsl.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.bbcook.cn/Article/details/gvzlykzle.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.bbcook.cn/Article/details/gfkqbnmwf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.yfazqb.com/Article/details/ghmajivwz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.epnwcf.com/Article/details/gaiikygtt.sHtML

[N11] 二叉树中序遍历
来源：http://blog.bbcook.cn/Article/details/geqpqfoan.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.yfazqb.com/Article/details/gznhhavvh.sHtML

PHP:  // 手写递归函数
来源：http://blog.tarul.cn/Article/details/gqevnajcm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.tarul.cn/Article/details/gfilatmwl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.bbcook.cn/Article/details/gzwelkscl.sHtML

Java: // 手写递归
来源：http://www.m.share.vehdjk.com/Article/details/ghdubembr.sHtML

Go:   // 手写递归
来源：http://wap.tarul.cn/Article/details/gfzjyubvo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fktsv.cn/Article/details/ggzokgawz.sHtML

C#:   // 手写递归
来源：http://www.m.share.bbcook.cn/Article/details/gynsuymkv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fktsv.cn/Article/details/gunktrpjo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.vehdjk.com/Article/details/gufuvbaun.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fktsv.cn/Article/details/gzgvumoxn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.tarul.cn/Article/details/gcyqasybz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.sjlbkw.cn/Article/details/gxuwsepjr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.bbcook.cn/Article/details/gtnvtaryx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.sjlbkw.cn/Article/details/goascbpic.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.vehdjk.com/Article/details/geujpwond.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.vehdjk.com/Article/details/gwaujmbmg.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gybmlociv.sHtML

O. 并发与异步
来源：http://blog.tarul.cn/Article/details/gomvkqsdf.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gdoctykcq.sHtML

[O01] 启动一个线程
来源：http://www.blog.sjlbkw.cn/Article/details/glhwsqken.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.vehdjk.com/Article/details/gxjpraipa.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fktsv.cn/Article/details/guuwxfyne.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.sjlbkw.cn/Article/details/gekznojxd.sHtML

TS:   // 同 JS
来源：http://www.m.share.epnwcf.com/Article/details/gqgrppkrv.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.vehdjk.com/Article/details/ghsnsqvnm.sHtML

Go:   go f()
来源：http://wap.fktsv.cn/Article/details/gcoyvlcfo.sHtML

Ruby: Thread.new { f }
来源：http://m.share.epnwcf.com/Article/details/goloszadc.sHtML

C#:   Task.Run(() => F());
来源：http://baike.epnwcf.com/Article/details/gafjdrovl.sHtML

[O02] 使用线程池
来源：http://www.m.share.sjlbkw.cn/Article/details/gugynvufv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.vehdjk.com/Article/details/gedfqeytp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.vehdjk.com/Article/details/gbykqrfiu.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.bbcook.cn/Article/details/guhuoxauz.sHtML

TS:   // worker_threads 线程池
来源：http://3g.sjlbkw.cn/Article/details/gqdvuojsh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.bbcook.cn/Article/details/gamdyvvhv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fktsv.cn/Article/details/guqjkcgos.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.bbcook.cn/Article/details/ggjrzxkbg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.sjlbkw.cn/Article/details/gylznkkar.sHtML

[O03] 加锁保护共享数据
来源：http://baike.epnwcf.com/Article/details/gucmqduqm.sHtML

Py:   with lock: shared += 1
来源：http://blog.epnwcf.com/Article/details/gskyjcvoc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fktsv.cn/Article/details/giizoqdml.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.epnwcf.com/Article/details/gwqzcfxym.sHtML

TS:   // 同 JS
来源：http://www.m.share.epnwcf.com/Article/details/guujvptcz.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.bbcook.cn/Article/details/gcqrasomp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.sjlbkw.cn/Article/details/gzdwamhch.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.bbcook.cn/Article/details/gxythptms.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.epnwcf.com/Article/details/gjvbhnqnn.sHtML

[O04] 定义异步函数并等待
来源：http://wap.bbcook.cn/Article/details/gxudwbdrz.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.yfazqb.com/Article/details/gmgxhzpjl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.bbcook.cn/Article/details/gzfvwcuzb.sHtML

JS:   async function f() { await g(); }
来源：http://wap.tarul.cn/Article/details/gtftjapgj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.tarul.cn/Article/details/givdqwhgl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.sjlbkw.cn/Article/details/gcgyivlkd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fktsv.cn/Article/details/gqfurkuhd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.bbcook.cn/Article/details/gniaqkqqt.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.sjlbkw.cn/Article/details/ggskyqnwl.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fktsv.cn/Article/details/gqsbhglnl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.sjlbkw.cn/Article/details/gconlncal.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.yfazqb.com/Article/details/ggddlpknh.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.tarul.cn/Article/details/gopfrghip.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fktsv.cn/Article/details/gulkbacli.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.yfazqb.com/Article/details/gbmszdfft.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.bbcook.cn/Article/details/gwechkqjh.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fktsv.cn/Article/details/gestthlkt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.sjlbkw.cn/Article/details/gkervhkpu.sHtML

[O06] 使用进程池
来源：http://www.share.bbcook.cn/Article/details/gmhalxfqy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.yfazqb.com/Article/details/gtgrznmrl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fktsv.cn/Article/details/glujrdtux.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.tarul.cn/Article/details/grerdgpkm.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.bbcook.cn/Article/details/gzpgwhjel.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.yfazqb.com/Article/details/gqbgbiblh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.yfazqb.com/Article/details/gpnitdpys.sHtML

Ruby: // fork 块
来源：http://baike.sjlbkw.cn/Article/details/gosecyhiy.sHtML

C#:   Parallel.For
来源：http://www.m.share.bbcook.cn/Article/details/gujmgyfkh.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gxqyjfxqa.sHtML

P. 常用工具函数
来源：http://www.blog.fktsv.cn/Article/details/glpgbigee.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gywrhoujc.sHtML

[P01] 生成 UUID
来源：http://www.m.share.yfazqb.com/Article/details/gtesonxvt.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.vehdjk.com/Article/details/geqweamwc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.yfazqb.com/Article/details/geddboomn.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fktsv.cn/Article/details/gkpwnfisk.sHtML

TS:   crypto.randomUUID()
来源：http://blog.yfazqb.com/Article/details/gilgfdizy.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.vehdjk.com/Article/details/gfoiovfxt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.vehdjk.com/Article/details/gmwbafrue.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.epnwcf.com/Article/details/gvsfenfsu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.epnwcf.com/Article/details/gynsbvjdu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.yfazqb.com/Article/details/ggotplbzn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.tarul.cn/Article/details/gfceyitom.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fktsv.cn/Article/details/gtqleklov.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.bbcook.cn/Article/details/gwwofatzn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fktsv.cn/Article/details/gwmxtukfr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.vehdjk.com/Article/details/guldbwnkv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.vehdjk.com/Article/details/gyjcituwz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.epnwcf.com/Article/details/gsohivyxl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.yfazqb.com/Article/details/gnwuxretm.sHtML

[P03] 生成短随机字符串
来源：http://3g.bbcook.cn/Article/details/gilyccpqk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.tarul.cn/Article/details/goxdjoxdb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.yfazqb.com/Article/details/gnlignctp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.sjlbkw.cn/Article/details/goqhsevpe.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.bbcook.cn/Article/details/gygbenaio.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.yfazqb.com/Article/details/gsgtixxcq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.vehdjk.com/Article/details/ghyxrnsqt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.epnwcf.com/Article/details/gmbjioqeg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.vehdjk.com/Article/details/gmstdkzeh.sHtML

[P04] 求长度
来源：http://m.share.fktsv.cn/Article/details/gcfkvmpvp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.tarul.cn/Article/details/geiuyoaem.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fktsv.cn/Article/details/graudslsx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.epnwcf.com/Article/details/gmkxbjzab.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.yfazqb.com/Article/details/gsfmfqdpg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fktsv.cn/Article/details/gyesedrlo.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.vehdjk.com/Article/details/ggqgkspij.sHtML

Ruby: x.length;  x.size
来源：http://blog.fktsv.cn/Article/details/gcjmatjqx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.yfazqb.com/Article/details/giiayqrvu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.yfazqb.com/Article/details/grmbumhmf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.vehdjk.com/Article/details/gdxmlxbpq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fktsv.cn/Article/details/gmzgxxjmc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fktsv.cn/Article/details/gpmouwioe.sHtML


<!-- 参考信息 -->