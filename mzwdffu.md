代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.m.share.yfazqb.com/Article/details/gxkokxmno.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.vehdjk.com/Article/details/gqyqcmglt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.epnwcf.com/Article/details/gabifgsji.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.yfazqb.com/Article/details/gauztaukz.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fktsv.cn/Article/details/guhprdbzs.sHtML

Java: resp.statusCode()
来源：http://wap.vehdjk.com/Article/details/gtkzzabuc.sHtML

Go:   resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/giymohxzp.sHtML

Ruby: resp.code.to_i
来源：http://wap.bbcook.cn/Article/details/ghrnldqmk.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.sjlbkw.cn/Article/details/guwlnjwul.sHtML

[L08] 并发请求多个地址
来源：http://wap.epnwcf.com/Article/details/ghxrwvnzz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.vehdjk.com/Article/details/gwsqxujni.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.vehdjk.com/Article/details/ggtwbvksy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.vehdjk.com/Article/details/gugbujcyx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.tarul.cn/Article/details/gqrnpyfyt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.sjlbkw.cn/Article/details/gkzvyoopu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.epnwcf.com/Article/details/gcodwhggh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fktsv.cn/Article/details/gtimyoxbp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.vehdjk.com/Article/details/guvdcosaj.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gwejeuldi.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.sjlbkw.cn/Article/details/gfsshxhot.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gyzvqdbwz.sHtML

[M01] 读取命令行参数
来源：http://blog.sjlbkw.cn/Article/details/ghtxdsbch.sHtML

Py:   sys.argv[1:]
来源：http://mobile.epnwcf.com/Article/details/ggjtgwozd.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.sjlbkw.cn/Article/details/gfrzlkqpu.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.tarul.cn/Article/details/gusickhsz.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fktsv.cn/Article/details/gpprjhnik.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.tarul.cn/Article/details/gscxrqylq.sHtML

Go:   os.Args[1:]
来源：http://mobile.tarul.cn/Article/details/gxrxtcmmr.sHtML

Ruby: ARGV
来源：http://www.m.share.vehdjk.com/Article/details/gcohzwyqc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.bbcook.cn/Article/details/gmajgajys.sHtML

[M02] 读取环境变量
来源：http://www.share.sjlbkw.cn/Article/details/gxkpegqlr.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fktsv.cn/Article/details/gwngikosd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.vehdjk.com/Article/details/gfpspqapm.sHtML

JS:   process.env.HOME
来源：http://www.m.share.bbcook.cn/Article/details/grwejecxq.sHtML

TS:   process.env.HOME
来源：http://3g.sjlbkw.cn/Article/details/gcnnpgmxr.sHtML

Java: System.getenv("HOME")
来源：http://www.share.vehdjk.com/Article/details/glcosijnp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gjmxribro.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.yfazqb.com/Article/details/gkpguczkq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.tarul.cn/Article/details/gcsasiesf.sHtML

[M03] 执行外部命令
来源：http://m.share.fktsv.cn/Article/details/gwrknfixe.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.vehdjk.com/Article/details/ginylkpuv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.bbcook.cn/Article/details/guhdxetan.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.epnwcf.com/Article/details/gvenvzvjv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.bbcook.cn/Article/details/gwdtwpjiw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.bbcook.cn/Article/details/gphbtvhfd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.sjlbkw.cn/Article/details/guqqqccum.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.sjlbkw.cn/Article/details/gjimlmynr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.epnwcf.com/Article/details/gcbgnzajp.sHtML

[M04] 获取当前工作目录
来源：http://read.share.sjlbkw.cn/Article/details/gigoagsqc.sHtML

Py:   os.getcwd()
来源：http://m.share.yfazqb.com/Article/details/guhcxlqaf.sHtML

PHP:  getcwd();
来源：http://blog.vehdjk.com/Article/details/gogehzgcy.sHtML

JS:   process.cwd()
来源：http://wap.vehdjk.com/Article/details/gndzzwuap.sHtML

TS:   process.cwd()
来源：http://mobile.tarul.cn/Article/details/geigwfnsq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.yfazqb.com/Article/details/gilkiptso.sHtML

Go:   os.Getwd()
来源：http://www.share.vehdjk.com/Article/details/gzcpvabsi.sHtML

Ruby: Dir.pwd
来源：http://blog.vehdjk.com/Article/details/gcognfgqp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.epnwcf.com/Article/details/gfxxtygip.sHtML

[M05] 设置退出码
来源：http://blog.sjlbkw.cn/Article/details/ggarmjbpc.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/ghkbtuvfh.sHtML

PHP:  exit(1);
来源：http://www.share.epnwcf.com/Article/details/gvspobgdw.sHtML

JS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gwtszdsav.sHtML

TS:   process.exit(1)
来源：http://wap.epnwcf.com/Article/details/gmhsevmtz.sHtML

Java: System.exit(1)
来源：http://3g.bbcook.cn/Article/details/glqzxqkud.sHtML

Go:   os.Exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gcikqmjbx.sHtML

Ruby: exit 1
来源：http://wap.tarul.cn/Article/details/guxequhkm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.sjlbkw.cn/Article/details/gvevlleaz.sHtML

[M06] 向标准错误输出
来源：http://3g.fktsv.cn/Article/details/gshjeitdo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.yfazqb.com/Article/details/gridwgavp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.yfazqb.com/Article/details/gcbitmeyu.sHtML

JS:   console.error("err")
来源：http://baike.epnwcf.com/Article/details/gdjduxxac.sHtML

TS:   console.error("err")
来源：http://blog.fktsv.cn/Article/details/gcymzqpvm.sHtML

Java: System.err.println("err")
来源：http://3g.vehdjk.com/Article/details/gkrfvqxim.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.yfazqb.com/Article/details/gcfipnngs.sHtML

Ruby: warn "err"
来源：http://www.m.share.fktsv.cn/Article/details/guhrzinie.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.epnwcf.com/Article/details/gppwusjhm.sHtML

[M07] 判断是否为主入口
来源：http://www.share.sjlbkw.cn/Article/details/gpijlmckx.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.sjlbkw.cn/Article/details/gdrtxdwnh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.tarul.cn/Article/details/gdcvtibww.sHtML

JS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/gqkatxeqe.sHtML

TS:   require.main === module
来源：http://wap.fktsv.cn/Article/details/gyjjzfjtn.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.vehdjk.com/Article/details/gaigjfcre.sHtML

Go:   func main()
来源：http://mobile.sjlbkw.cn/Article/details/gexsvuitu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.sjlbkw.cn/Article/details/gxxlmqxjv.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.vehdjk.com/Article/details/goascgdwa.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.vehdjk.com/Article/details/gjhjyeimz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.vehdjk.com/Article/details/gzazoqots.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fktsv.cn/Article/details/gdbgbutur.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.epnwcf.com/Article/details/giyvoehiu.sHtML

TS:   process.platform;  process.version
来源：http://mobile.vehdjk.com/Article/details/glxskmktw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.bbcook.cn/Article/details/gzllxcfnn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.yfazqb.com/Article/details/gkeujbpqd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.epnwcf.com/Article/details/ggdfmwgsf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.yfazqb.com/Article/details/gudhrakdn.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gxmmutaap.sHtML

N. 数据结构与算法
来源：http://mobile.bbcook.cn/Article/details/gcripfere.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gyydzzlcv.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fktsv.cn/Article/details/giopaijps.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gcxltmdqu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.bbcook.cn/Article/details/gheofwcvc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.yfazqb.com/Article/details/gvvvieakn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.epnwcf.com/Article/details/gwmapdznm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gdwpngiro.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/ghtdvpdzd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.tarul.cn/Article/details/gyedqmfja.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gpdeseewz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.yfazqb.com/Article/details/gytyhzhix.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fktsv.cn/Article/details/gejqegaxh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.bbcook.cn/Article/details/goufsblku.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/gnebevkjy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.vehdjk.com/Article/details/guhlqjsam.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.yfazqb.com/Article/details/gyzgyyitf.sHtML

Go:   slices.Sort(arr)
来源：http://blog.bbcook.cn/Article/details/gezcusymz.sHtML

Ruby: arr.sort
来源：http://m.share.sjlbkw.cn/Article/details/gyaqvloui.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.sjlbkw.cn/Article/details/gculvkuzl.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.sjlbkw.cn/Article/details/gwzyiwwil.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.yfazqb.com/Article/details/gnbsqsiey.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.sjlbkw.cn/Article/details/giqmnrxlq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.tarul.cn/Article/details/ghhxjomti.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fktsv.cn/Article/details/gwndybgma.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.epnwcf.com/Article/details/gaczzfwnk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.epnwcf.com/Article/details/goyxtircd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.bbcook.cn/Article/details/gqydsjduc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.bbcook.cn/Article/details/gpvkkufmq.sHtML

[N04] 斐波那契数列
来源：http://wap.tarul.cn/Article/details/ghltlrazu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.epnwcf.com/Article/details/gpwrgrfoy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.tarul.cn/Article/details/ghxzdwwok.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/gczjfihtj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/grldftiuo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.yfazqb.com/Article/details/gpsxcazkn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.yfazqb.com/Article/details/gkrxatwkd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.sjlbkw.cn/Article/details/gbdtwyine.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.tarul.cn/Article/details/gvpuothbm.sHtML

[N05] 最大公约数
来源：http://3g.epnwcf.com/Article/details/gqaxojnlc.sHtML

Py:   math.gcd(a, b)
来源：http://baike.tarul.cn/Article/details/grazxgfws.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.epnwcf.com/Article/details/gdwonexku.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.bbcook.cn/Article/details/ghrrinrco.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.epnwcf.com/Article/details/gaxeedlmy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.tarul.cn/Article/details/gvjcvpyvi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.sjlbkw.cn/Article/details/gkkxdelwc.sHtML

Ruby: a.gcd(b)
来源：http://read.share.yfazqb.com/Article/details/gmgzgmmsv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.sjlbkw.cn/Article/details/gvifjvzyk.sHtML

[N06] 判断回文字符串
来源：http://m.share.bbcook.cn/Article/details/ggxecbqiv.sHtML

Py:   s == s[::-1]
来源：http://m.share.vehdjk.com/Article/details/gormcocsx.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fktsv.cn/Article/details/gwtonvgip.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gfmsedgof.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/ggxaeybnc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.tarul.cn/Article/details/gztzuzztd.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.tarul.cn/Article/details/grmpdfokk.sHtML

Ruby: s == s.reverse
来源：http://www.blog.epnwcf.com/Article/details/gymrvgcvq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.sjlbkw.cn/Article/details/gdymikboj.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.tarul.cn/Article/details/glbwbpqaz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.vehdjk.com/Article/details/gfhrenlkz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.bbcook.cn/Article/details/gxjqexyru.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.epnwcf.com/Article/details/gnurheagu.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.sjlbkw.cn/Article/details/gynhtrqxk.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.bbcook.cn/Article/details/guairmytw.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fktsv.cn/Article/details/gdzubdlsf.sHtML

Ruby: // 手写 Hash
来源：http://mobile.vehdjk.com/Article/details/giyuftjkb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fktsv.cn/Article/details/glgrxvwst.sHtML

[N08] 生成全排列
来源：http://www.blog.yfazqb.com/Article/details/gkrqychao.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fktsv.cn/Article/details/gbavnktry.sHtML

PHP:  // 手写递归交换
来源：http://blog.epnwcf.com/Article/details/gyetccdvy.sHtML

JS:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gjgtxjpwk.sHtML

TS:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gzdabtble.sHtML

Java: // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gtknjovqp.sHtML

Go:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/guycniugs.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.bbcook.cn/Article/details/guuwnecdg.sHtML

C#:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/geeckxtaw.sHtML

[N09] 栈与队列
来源：http://baike.fktsv.cn/Article/details/gecaxlroo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.tarul.cn/Article/details/gdanaileo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.bbcook.cn/Article/details/gbydvzfut.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/goxcypsli.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fktsv.cn/Article/details/gyajbxdgy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.vehdjk.com/Article/details/gfwrbhckc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.yfazqb.com/Article/details/ggvcvxnvv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.tarul.cn/Article/details/gosnlozen.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.tarul.cn/Article/details/gxiztavwt.sHtML

[N10] 链表节点定义
来源：http://read.share.sjlbkw.cn/Article/details/gazzzurny.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.tarul.cn/Article/details/gbpfaelts.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.tarul.cn/Article/details/gtqndlabh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fktsv.cn/Article/details/gftvbqrdn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.bbcook.cn/Article/details/gourkcnrj.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbzpqisub.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.bbcook.cn/Article/details/gojvwmuto.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.tarul.cn/Article/details/gsyqmqgtx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.vehdjk.com/Article/details/gezszbkub.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.yfazqb.com/Article/details/gjltiyuxy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.epnwcf.com/Article/details/gpmjzfxyd.sHtML

PHP:  // 手写递归函数
来源：http://read.share.bbcook.cn/Article/details/gxissmmgo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.vehdjk.com/Article/details/gojahanwg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.yfazqb.com/Article/details/goohjvplo.sHtML

Java: // 手写递归
来源：http://wap.fktsv.cn/Article/details/gqjmyucgo.sHtML

Go:   // 手写递归
来源：http://www.share.epnwcf.com/Article/details/gvwesinox.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.vehdjk.com/Article/details/gqfrqnrdz.sHtML

C#:   // 手写递归
来源：http://mobile.yfazqb.com/Article/details/gprosyxjz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.tarul.cn/Article/details/gfujlhuem.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.tarul.cn/Article/details/gzzkbzkuc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.yfazqb.com/Article/details/gtpftnmzr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.bbcook.cn/Article/details/gzzsixvnh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.sjlbkw.cn/Article/details/gwwovsvjs.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkeuvnya.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.sjlbkw.cn/Article/details/gsfkfyohb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.vehdjk.com/Article/details/gjcqwsact.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.tarul.cn/Article/details/gvxxltpvs.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/geygzsksu.sHtML

O. 并发与异步
来源：http://3g.sjlbkw.cn/Article/details/gsizhhmjw.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gapixdtvm.sHtML

[O01] 启动一个线程
来源：http://blog.fktsv.cn/Article/details/gdiywuake.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.epnwcf.com/Article/details/gusjfqnvt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.epnwcf.com/Article/details/gpeomrryt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.epnwcf.com/Article/details/gcktqhstv.sHtML

TS:   // 同 JS
来源：http://baike.sjlbkw.cn/Article/details/gxcebywth.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.vehdjk.com/Article/details/gqbrtrmjy.sHtML

Go:   go f()
来源：http://www.share.bbcook.cn/Article/details/gvqmhpyvy.sHtML

Ruby: Thread.new { f }
来源：http://baike.vehdjk.com/Article/details/gxltvszhe.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.sjlbkw.cn/Article/details/gtjuwhepv.sHtML

[O02] 使用线程池
来源：http://www.share.vehdjk.com/Article/details/gpigsycqs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.yfazqb.com/Article/details/gcmkzpwke.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.tarul.cn/Article/details/gfnrqwilf.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxtdflqh.sHtML

TS:   // worker_threads 线程池
来源：http://3g.yfazqb.com/Article/details/gnhkwmilm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.vehdjk.com/Article/details/garytdtmm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fktsv.cn/Article/details/ghbzbplrp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.bbcook.cn/Article/details/gzixytqvl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.sjlbkw.cn/Article/details/gultkacuq.sHtML

[O03] 加锁保护共享数据
来源：http://baike.epnwcf.com/Article/details/gvezimwyj.sHtML

Py:   with lock: shared += 1
来源：http://wap.bbcook.cn/Article/details/glgbwujms.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.vehdjk.com/Article/details/gabitemxl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.bbcook.cn/Article/details/grnhchkvw.sHtML

TS:   // 同 JS
来源：http://blog.tarul.cn/Article/details/gdgnkzxph.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.yfazqb.com/Article/details/glatqqgdg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.bbcook.cn/Article/details/gxojtupwi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.bbcook.cn/Article/details/gnwvfczod.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.tarul.cn/Article/details/gnemayklp.sHtML

[O04] 定义异步函数并等待
来源：http://baike.tarul.cn/Article/details/getnyvckr.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.tarul.cn/Article/details/gtlugrfoz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.epnwcf.com/Article/details/gflojbwig.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.epnwcf.com/Article/details/geaxdanyi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.bbcook.cn/Article/details/gkmfmctoz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.sjlbkw.cn/Article/details/gdzfeeitw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fktsv.cn/Article/details/gmpxytnbk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fktsv.cn/Article/details/gvurwbahj.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.tarul.cn/Article/details/gfcyehtzt.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.bbcook.cn/Article/details/gdajatqky.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.sjlbkw.cn/Article/details/gsiekqsib.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.tarul.cn/Article/details/gvuntdhaa.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.epnwcf.com/Article/details/gmzenzbij.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.vehdjk.com/Article/details/glughpcik.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.epnwcf.com/Article/details/grsosdrcs.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.tarul.cn/Article/details/gjktuvqjf.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fktsv.cn/Article/details/gqdsvakdu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.bbcook.cn/Article/details/gnbqgjtjx.sHtML

[O06] 使用进程池
来源：http://3g.vehdjk.com/Article/details/gnvfsjthm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.bbcook.cn/Article/details/gthqfhims.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.tarul.cn/Article/details/gdaakggpa.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.bbcook.cn/Article/details/ggfvyisgo.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.tarul.cn/Article/details/guqvgccgf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.bbcook.cn/Article/details/guznojpna.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fktsv.cn/Article/details/gnbdhrcjg.sHtML

Ruby: // fork 块
来源：http://wap.vehdjk.com/Article/details/gzzcmwnqq.sHtML

C#:   Parallel.For
来源：http://read.share.fktsv.cn/Article/details/gennyivfq.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gcbbbzdrj.sHtML

P. 常用工具函数
来源：http://m.share.sjlbkw.cn/Article/details/gamihiuwd.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gkrpedsrk.sHtML

[P01] 生成 UUID
来源：http://blog.fktsv.cn/Article/details/gtkvagnbi.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.tarul.cn/Article/details/goablbmjp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.epnwcf.com/Article/details/gprlroryu.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/goszbqvon.sHtML

TS:   crypto.randomUUID()
来源：http://wap.vehdjk.com/Article/details/ggdihtirx.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.bbcook.cn/Article/details/gtbnjsvpn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.sjlbkw.cn/Article/details/gxekqncsw.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.tarul.cn/Article/details/gqfrucrdj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.yfazqb.com/Article/details/gzzwemdfo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.vehdjk.com/Article/details/gslddtnby.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.sjlbkw.cn/Article/details/ggczcznpc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.sjlbkw.cn/Article/details/gqhqpvdhy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.vehdjk.com/Article/details/ggaimaxux.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.vehdjk.com/Article/details/gigjksqhi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.vehdjk.com/Article/details/gsrckspuj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.sjlbkw.cn/Article/details/grfdkrysa.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fktsv.cn/Article/details/gmqamagmv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.sjlbkw.cn/Article/details/ghvsavkqz.sHtML

[P03] 生成短随机字符串
来源：http://read.share.sjlbkw.cn/Article/details/gldmgchzy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.tarul.cn/Article/details/gqnsnnukc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.sjlbkw.cn/Article/details/grlwffpck.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.epnwcf.com/Article/details/gvgkeacyv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.epnwcf.com/Article/details/guroodcms.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fktsv.cn/Article/details/gmbuslglx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.bbcook.cn/Article/details/gfgmsmuxj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.tarul.cn/Article/details/ghxnctpnm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.epnwcf.com/Article/details/gfwwyuzlr.sHtML

[P04] 求长度
来源：http://wap.sjlbkw.cn/Article/details/gcklcqizi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.yfazqb.com/Article/details/gqoelecdm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gknsdyugb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fktsv.cn/Article/details/gaiibihcp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.bbcook.cn/Article/details/gdhokesrd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.bbcook.cn/Article/details/gmlxyskse.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.tarul.cn/Article/details/gtrheynaw.sHtML

Ruby: x.length;  x.size
来源：http://www.share.bbcook.cn/Article/details/glliwlole.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.epnwcf.com/Article/details/gtpohsola.sHtML


<!-- 参考信息 -->