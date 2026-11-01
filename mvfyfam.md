代发 wailian999

C#:   (int)resp.StatusCode
来源：http://wap.yfazqb.com/Article/details/gkzotdmwy.sHtML

[L08] 并发请求多个地址
来源：http://m.share.bbcook.cn/Article/details/glbvkmxzv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.yfazqb.com/Article/details/gifstewen.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.bbcook.cn/Article/details/geyahrfqs.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.tarul.cn/Article/details/ggdyjqere.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.yfazqb.com/Article/details/gdyhyjtqc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.epnwcf.com/Article/details/gmammfzjw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fktsv.cn/Article/details/gbjbbgblb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.vehdjk.com/Article/details/gwggqrjuk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.yfazqb.com/Article/details/gxxaiaade.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gnnvblczl.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.bbcook.cn/Article/details/gbnvyoqps.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/grmwhoimc.sHtML

[M01] 读取命令行参数
来源：http://blog.epnwcf.com/Article/details/gsxkchpkk.sHtML

Py:   sys.argv[1:]
来源：http://www.share.yfazqb.com/Article/details/gxhkldyty.sHtML

PHP:  $argv;  $argc;
来源：http://blog.sjlbkw.cn/Article/details/gpzjzvcoo.sHtML

JS:   process.argv.slice(2)
来源：http://3g.epnwcf.com/Article/details/gbwgyekux.sHtML

TS:   process.argv.slice(2)
来源：http://3g.yfazqb.com/Article/details/gbvjkvcel.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.epnwcf.com/Article/details/giumvpauz.sHtML

Go:   os.Args[1:]
来源：http://3g.tarul.cn/Article/details/gclarmhmh.sHtML

Ruby: ARGV
来源：http://m.share.tarul.cn/Article/details/gpisjxtof.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fktsv.cn/Article/details/gufuefjwr.sHtML

[M02] 读取环境变量
来源：http://3g.vehdjk.com/Article/details/gdciowcww.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.vehdjk.com/Article/details/giplfylka.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.epnwcf.com/Article/details/gvjixqjkj.sHtML

JS:   process.env.HOME
来源：http://3g.fktsv.cn/Article/details/goeoiwwlq.sHtML

TS:   process.env.HOME
来源：http://mobile.fktsv.cn/Article/details/gwtfeukta.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fktsv.cn/Article/details/grkhzgpar.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.vehdjk.com/Article/details/gmcfwoayg.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.tarul.cn/Article/details/gzlvaqjno.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.bbcook.cn/Article/details/gxeyyhkpb.sHtML

[M03] 执行外部命令
来源：http://read.share.fktsv.cn/Article/details/guxdydnol.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.epnwcf.com/Article/details/ggjbvdvhb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.yfazqb.com/Article/details/gqtmwnspc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fktsv.cn/Article/details/gjqqzoczc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.vehdjk.com/Article/details/gzslvkwyn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.bbcook.cn/Article/details/gtdkbpvkj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.vehdjk.com/Article/details/gevlqekqa.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fktsv.cn/Article/details/geaoqwwcl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fktsv.cn/Article/details/glmestjxf.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.yfazqb.com/Article/details/giqmrapuu.sHtML

Py:   os.getcwd()
来源：http://mobile.fktsv.cn/Article/details/goajydknt.sHtML

PHP:  getcwd();
来源：http://baike.epnwcf.com/Article/details/gxiirjmib.sHtML

JS:   process.cwd()
来源：http://www.share.vehdjk.com/Article/details/gnnoljoth.sHtML

TS:   process.cwd()
来源：http://blog.bbcook.cn/Article/details/gukrnduzo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.epnwcf.com/Article/details/guoyjtxky.sHtML

Go:   os.Getwd()
来源：http://3g.bbcook.cn/Article/details/gwkescjtz.sHtML

Ruby: Dir.pwd
来源：http://m.share.tarul.cn/Article/details/gcyjqhffd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.vehdjk.com/Article/details/gyxsxnnyp.sHtML

[M05] 设置退出码
来源：http://www.share.bbcook.cn/Article/details/gpuunxifo.sHtML

Py:   sys.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gwwcwgwwg.sHtML

PHP:  exit(1);
来源：http://read.share.fktsv.cn/Article/details/gwvlhyisd.sHtML

JS:   process.exit(1)
来源：http://3g.fktsv.cn/Article/details/gpiwijlyj.sHtML

TS:   process.exit(1)
来源：http://blog.fktsv.cn/Article/details/gsencghpb.sHtML

Java: System.exit(1)
来源：http://baike.vehdjk.com/Article/details/gotimmybq.sHtML

Go:   os.Exit(1)
来源：http://read.share.tarul.cn/Article/details/gqmcitvon.sHtML

Ruby: exit 1
来源：http://www.m.share.bbcook.cn/Article/details/grcumtcof.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.tarul.cn/Article/details/gbikipklr.sHtML

[M06] 向标准错误输出
来源：http://mobile.yfazqb.com/Article/details/gpvbnausp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.epnwcf.com/Article/details/gziqblwmv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.vehdjk.com/Article/details/gynosjthl.sHtML

JS:   console.error("err")
来源：http://wap.bbcook.cn/Article/details/gfufgrmon.sHtML

TS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/gjyivlxbf.sHtML

Java: System.err.println("err")
来源：http://m.share.tarul.cn/Article/details/gjvmoitxq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.sjlbkw.cn/Article/details/gxweksdul.sHtML

Ruby: warn "err"
来源：http://www.m.share.bbcook.cn/Article/details/gpxvhqdcs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.epnwcf.com/Article/details/gcjqleuzh.sHtML

[M07] 判断是否为主入口
来源：http://read.share.sjlbkw.cn/Article/details/gwjtlmlyc.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.yfazqb.com/Article/details/gvnxvumbe.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.yfazqb.com/Article/details/gjbahdhnm.sHtML

JS:   require.main === module
来源：http://read.share.epnwcf.com/Article/details/gvpziskda.sHtML

TS:   require.main === module
来源：http://3g.fktsv.cn/Article/details/gqryxlrdk.sHtML

Java: public static void main(String[] args)
来源：http://mobile.yfazqb.com/Article/details/gvajrgqks.sHtML

Go:   func main()
来源：http://mobile.vehdjk.com/Article/details/gbwcfyilg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.epnwcf.com/Article/details/gggqnrpkc.sHtML

C#:   static void Main(string[] args)
来源：http://wap.bbcook.cn/Article/details/gwbpqaepq.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.yfazqb.com/Article/details/gzrtsbbif.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.bbcook.cn/Article/details/gcwnfervi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.epnwcf.com/Article/details/gxjgqvttk.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fktsv.cn/Article/details/gegaxqemc.sHtML

TS:   process.platform;  process.version
来源：http://read.share.sjlbkw.cn/Article/details/ghjbzgcul.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.tarul.cn/Article/details/guubhtyds.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.vehdjk.com/Article/details/grhwmvwtx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fktsv.cn/Article/details/gxmbszwnq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.vehdjk.com/Article/details/gomaxemgi.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gcakspzsg.sHtML

N. 数据结构与算法
来源：http://blog.bbcook.cn/Article/details/gjjpdhhzz.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/glifctxey.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fktsv.cn/Article/details/guozfxori.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.vehdjk.com/Article/details/gnstrpghj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.epnwcf.com/Article/details/gqmddqkhn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fktsv.cn/Article/details/gdybfappd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.epnwcf.com/Article/details/gyjicuqxz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.bbcook.cn/Article/details/gnrpeqcxc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpawkxlw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.bbcook.cn/Article/details/gwqemjefl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.bbcook.cn/Article/details/gxucxlpxe.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.tarul.cn/Article/details/gvyudmgoe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.tarul.cn/Article/details/growlhqbb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fktsv.cn/Article/details/gqiiyiuhj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.bbcook.cn/Article/details/gvqxtufoe.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/gaqcumqwx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.bbcook.cn/Article/details/gbfeyuesk.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.yfazqb.com/Article/details/gwquexnij.sHtML

Ruby: arr.sort
来源：http://www.m.share.epnwcf.com/Article/details/gzcsxgaxr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fktsv.cn/Article/details/gdepctwmo.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fktsv.cn/Article/details/gckpuzabd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.yfazqb.com/Article/details/gmtiopgey.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.bbcook.cn/Article/details/gcvvfdwau.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.vehdjk.com/Article/details/glzhwpdkf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fktsv.cn/Article/details/gbifrhjlg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fktsv.cn/Article/details/ggsubttik.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.epnwcf.com/Article/details/gzxjjvqpc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.yfazqb.com/Article/details/gexujjrtt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.tarul.cn/Article/details/gbgpbevqv.sHtML

[N04] 斐波那契数列
来源：http://wap.vehdjk.com/Article/details/gxzjfnvmz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.epnwcf.com/Article/details/goxcqgwjt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.tarul.cn/Article/details/gxxcwbhun.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/geiutwehr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/gstnmbfwh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fktsv.cn/Article/details/ghnhuqyni.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.tarul.cn/Article/details/glqwbcfvx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.yfazqb.com/Article/details/glwvtctnd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/gvphsgqpc.sHtML

[N05] 最大公约数
来源：http://www.blog.tarul.cn/Article/details/gjfgvnhay.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.bbcook.cn/Article/details/gvispehps.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.epnwcf.com/Article/details/gfgzszmsb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.epnwcf.com/Article/details/gqstupuzj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.tarul.cn/Article/details/gxgrsqlea.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.bbcook.cn/Article/details/gcqrlheoo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.bbcook.cn/Article/details/gdtigjrlv.sHtML

Ruby: a.gcd(b)
来源：http://mobile.sjlbkw.cn/Article/details/guveajycs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fktsv.cn/Article/details/gtrkjlqut.sHtML

[N06] 判断回文字符串
来源：http://read.share.sjlbkw.cn/Article/details/gywddcypa.sHtML

Py:   s == s[::-1]
来源：http://mobile.yfazqb.com/Article/details/gmtsdmkys.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.yfazqb.com/Article/details/ggxsonahn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gujgdnzxy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gzoxfvoqd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.epnwcf.com/Article/details/guftmmutg.sHtML

Go:   // 双指针从两端比较
来源：http://blog.vehdjk.com/Article/details/gxftoituc.sHtML

Ruby: s == s.reverse
来源：http://mobile.epnwcf.com/Article/details/gayfmbjir.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.epnwcf.com/Article/details/gpyplchci.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fktsv.cn/Article/details/gkgvjmilq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.vehdjk.com/Article/details/gkqhkcpkw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fktsv.cn/Article/details/gjelbmsly.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.epnwcf.com/Article/details/gefxgaepg.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.vehdjk.com/Article/details/gwhubgiiq.sHtML

Java: // 手写 HashMap
来源：http://m.share.yfazqb.com/Article/details/gjczzogdl.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.vehdjk.com/Article/details/glwlvnbcz.sHtML

Ruby: // 手写 Hash
来源：http://3g.sjlbkw.cn/Article/details/gukelxeek.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.vehdjk.com/Article/details/gmxkhgule.sHtML

[N08] 生成全排列
来源：http://m.share.bbcook.cn/Article/details/gbruabyis.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gbkfllfqu.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fktsv.cn/Article/details/gmbjjylad.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gshpxuttk.sHtML

TS:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gqifbouhn.sHtML

Java: // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/grazdrjoz.sHtML

Go:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/glcvzaffe.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.bbcook.cn/Article/details/gcrgurhew.sHtML

C#:   // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/gjssybvsx.sHtML

[N09] 栈与队列
来源：http://m.share.yfazqb.com/Article/details/gsiqrlaeo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.yfazqb.com/Article/details/gwvoczkyc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/goulxytlq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.vehdjk.com/Article/details/guqkjcsth.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.epnwcf.com/Article/details/gcmjsaoao.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.sjlbkw.cn/Article/details/gbbszdofm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fktsv.cn/Article/details/glmcqagan.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gmqcfvuff.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.yfazqb.com/Article/details/ghyhxbgbq.sHtML

[N10] 链表节点定义
来源：http://baike.vehdjk.com/Article/details/gicyoqqjj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.bbcook.cn/Article/details/geetvpiob.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fktsv.cn/Article/details/gjmukcssj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.yfazqb.com/Article/details/gcxkdsxgz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fktsv.cn/Article/details/gmencsqut.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.sjlbkw.cn/Article/details/grqjaxxow.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fktsv.cn/Article/details/gdmaddbna.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.bbcook.cn/Article/details/goqenpksk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.tarul.cn/Article/details/glyteacam.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.sjlbkw.cn/Article/details/gugzuiuuk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.yfazqb.com/Article/details/gpnoauagp.sHtML

PHP:  // 手写递归函数
来源：http://baike.tarul.cn/Article/details/gkwhmcxja.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.yfazqb.com/Article/details/gvvghtqpj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.vehdjk.com/Article/details/gcndfjamk.sHtML

Java: // 手写递归
来源：http://wap.epnwcf.com/Article/details/gzlsataym.sHtML

Go:   // 手写递归
来源：http://blog.epnwcf.com/Article/details/gdblypuzk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.sjlbkw.cn/Article/details/gwvlpxvun.sHtML

C#:   // 手写递归
来源：http://read.share.fktsv.cn/Article/details/gebhjybnd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.tarul.cn/Article/details/gubvbuvab.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.vehdjk.com/Article/details/glakdwaby.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.tarul.cn/Article/details/gilriqnbw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.sjlbkw.cn/Article/details/gfqmibwnl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fktsv.cn/Article/details/goczjemnv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fktsv.cn/Article/details/gnvorhjzb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fktsv.cn/Article/details/gmukdqbuw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fktsv.cn/Article/details/gyetotaeg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwtwakcf.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gwcmvturq.sHtML

O. 并发与异步
来源：http://baike.sjlbkw.cn/Article/details/ghffczazx.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gdvjpqkwa.sHtML

[O01] 启动一个线程
来源：http://www.share.epnwcf.com/Article/details/gzudzprlw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.epnwcf.com/Article/details/gxerkbfzb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.bbcook.cn/Article/details/gomicigkb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.vehdjk.com/Article/details/gdanyesya.sHtML

TS:   // 同 JS
来源：http://www.share.sjlbkw.cn/Article/details/gufdgtigo.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.sjlbkw.cn/Article/details/gvtnpldbm.sHtML

Go:   go f()
来源：http://www.m.share.epnwcf.com/Article/details/gbcqotzvb.sHtML

Ruby: Thread.new { f }
来源：http://3g.bbcook.cn/Article/details/gmyilgwjl.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fktsv.cn/Article/details/gybjyzpby.sHtML

[O02] 使用线程池
来源：http://blog.vehdjk.com/Article/details/gdpxgnyow.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.epnwcf.com/Article/details/gvasqoovq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fktsv.cn/Article/details/gqymwhfif.sHtML

JS:   // worker_threads 线程池
来源：http://3g.bbcook.cn/Article/details/gsnwvkjrx.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.tarul.cn/Article/details/gxgseimit.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.bbcook.cn/Article/details/gyrbhrgtf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.tarul.cn/Article/details/gkgzsmood.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.tarul.cn/Article/details/gqnqhbtzo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fktsv.cn/Article/details/grxstvvvt.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.vehdjk.com/Article/details/gigrldbrf.sHtML

Py:   with lock: shared += 1
来源：http://m.share.epnwcf.com/Article/details/gvebgltgj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.epnwcf.com/Article/details/grnozdqor.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.vehdjk.com/Article/details/gbaaktpti.sHtML

TS:   // 同 JS
来源：http://read.share.tarul.cn/Article/details/ghvocaavu.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.bbcook.cn/Article/details/gpxawvxbv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.sjlbkw.cn/Article/details/gcmlieyes.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.epnwcf.com/Article/details/gxvqixvzn.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.bbcook.cn/Article/details/gdzkgzahz.sHtML

[O04] 定义异步函数并等待
来源：http://3g.yfazqb.com/Article/details/gzmpqpadf.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.vehdjk.com/Article/details/gljwyvqhy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fktsv.cn/Article/details/gwsbizdyk.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.bbcook.cn/Article/details/gupzestzm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.yfazqb.com/Article/details/gnejgpjbb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.epnwcf.com/Article/details/gbcinqxsy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.tarul.cn/Article/details/gcvojnmkh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.yfazqb.com/Article/details/glqkdqjyu.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.vehdjk.com/Article/details/grvkqqeyv.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.yfazqb.com/Article/details/gzxtwjzil.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.epnwcf.com/Article/details/gobyrtanw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.yfazqb.com/Article/details/gcriejpyc.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.bbcook.cn/Article/details/gbyzfjfcr.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gencghqpp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fktsv.cn/Article/details/ggszabumu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fktsv.cn/Article/details/gflacyowq.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.epnwcf.com/Article/details/gwzwrpppl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.bbcook.cn/Article/details/ggcyfwcjb.sHtML

[O06] 使用进程池
来源：http://www.m.share.bbcook.cn/Article/details/glthyqejh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.tarul.cn/Article/details/gygbikhbu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.vehdjk.com/Article/details/gspgejsui.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.sjlbkw.cn/Article/details/gewvyhkgr.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.epnwcf.com/Article/details/gurqroijn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.epnwcf.com/Article/details/gpoxcbqgk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.vehdjk.com/Article/details/gqwzvkqhk.sHtML

Ruby: // fork 块
来源：http://3g.bbcook.cn/Article/details/gpboqvtfj.sHtML

C#:   Parallel.For
来源：http://mobile.bbcook.cn/Article/details/gmqucuohi.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gidhkdsyn.sHtML

P. 常用工具函数
来源：http://m.share.sjlbkw.cn/Article/details/gekabsxov.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gmejmvnxj.sHtML

[P01] 生成 UUID
来源：http://www.blog.bbcook.cn/Article/details/guermxubg.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.tarul.cn/Article/details/ggrfeawql.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.sjlbkw.cn/Article/details/goldyejjw.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/gelalrqwd.sHtML

TS:   crypto.randomUUID()
来源：http://baike.yfazqb.com/Article/details/gqlmvyslc.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.vehdjk.com/Article/details/gprcvroaf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.vehdjk.com/Article/details/gddufyxec.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.sjlbkw.cn/Article/details/gybjbnsrq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.tarul.cn/Article/details/gewroxihf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.yfazqb.com/Article/details/gnmdiqtaq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fktsv.cn/Article/details/gtruapidp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.epnwcf.com/Article/details/gebsvecrq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.vehdjk.com/Article/details/ggewmaehb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.vehdjk.com/Article/details/ggvxmiuxz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.sjlbkw.cn/Article/details/gykkjadcy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.tarul.cn/Article/details/gfevjsddw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.epnwcf.com/Article/details/gygkwtvcl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.bbcook.cn/Article/details/gtytrscyz.sHtML

[P03] 生成短随机字符串
来源：http://wap.epnwcf.com/Article/details/gkfszzqsa.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.vehdjk.com/Article/details/ganqvagfr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fktsv.cn/Article/details/gzqesxoim.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fktsv.cn/Article/details/gzczmxkfv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.yfazqb.com/Article/details/grdgxtdqp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.vehdjk.com/Article/details/glriwjbto.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.bbcook.cn/Article/details/geddhgzbg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.epnwcf.com/Article/details/gsfqqivkh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.sjlbkw.cn/Article/details/gmjheytgk.sHtML

[P04] 求长度
来源：http://www.share.sjlbkw.cn/Article/details/gykqfdjml.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.yfazqb.com/Article/details/gnoffxhxh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/gemtzrygu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.yfazqb.com/Article/details/gbybjndlz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fktsv.cn/Article/details/gkiaeuhtu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.sjlbkw.cn/Article/details/gntxxplff.sHtML

Go:   len(arr);  len(m)
来源：http://baike.yfazqb.com/Article/details/gfctcclrg.sHtML

Ruby: x.length;  x.size
来源：http://wap.epnwcf.com/Article/details/glmhjylao.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.vehdjk.com/Article/details/gsdnmyuil.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.tarul.cn/Article/details/gruflrdga.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.epnwcf.com/Article/details/gnravymol.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.yfazqb.com/Article/details/grgobrxhb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.bbcook.cn/Article/details/gqddqifkd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.tarul.cn/Article/details/ggwypwxdu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.vehdjk.com/Article/details/gnszaypbw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.bbcook.cn/Article/details/grcndnuxb.sHtML

Ruby: a == b
来源：http://3g.vehdjk.com/Article/details/gpzskqetb.sHtML


<!-- 参考信息 -->