代发 wailian999

TS:   resp.ok;  resp.status
来源：http://wap.vehdjk.com/Article/details/gfofmestt.sHtML

Java: resp.statusCode()
来源：http://3g.tarul.cn/Article/details/gwmvixiwp.sHtML

Go:   resp.StatusCode
来源：http://baike.fktsv.cn/Article/details/giogoljuz.sHtML

Ruby: resp.code.to_i
来源：http://3g.tarul.cn/Article/details/gvgwcgmgs.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.vehdjk.com/Article/details/gvaskxeus.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.yfazqb.com/Article/details/gfwmuwoya.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.epnwcf.com/Article/details/gmwscqmgq.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fktsv.cn/Article/details/gpxtfkias.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fktsv.cn/Article/details/gmnqzjdwd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/gxonqnbid.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fktsv.cn/Article/details/gpjpwslao.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.bbcook.cn/Article/details/gigmazolv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.vehdjk.com/Article/details/gkiqtrtmg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fktsv.cn/Article/details/gbgkcntrw.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gxynhmcaq.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.vehdjk.com/Article/details/gowdiwete.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gxvaitehv.sHtML

[M01] 读取命令行参数
来源：http://www.share.bbcook.cn/Article/details/gthbwdvjh.sHtML

Py:   sys.argv[1:]
来源：http://blog.fktsv.cn/Article/details/guyaedvzw.sHtML

PHP:  $argv;  $argc;
来源：http://wap.bbcook.cn/Article/details/gvcughscp.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.vehdjk.com/Article/details/gddanzhxw.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.tarul.cn/Article/details/gjbmytegz.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.bbcook.cn/Article/details/gcuoxmysd.sHtML

Go:   os.Args[1:]
来源：http://blog.fktsv.cn/Article/details/gzfzjegrw.sHtML

Ruby: ARGV
来源：http://www.blog.yfazqb.com/Article/details/grsbigbdl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.bbcook.cn/Article/details/gtpmssfbp.sHtML

[M02] 读取环境变量
来源：http://mobile.sjlbkw.cn/Article/details/grwzpygbo.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gkbzahyso.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.tarul.cn/Article/details/gghvvtulu.sHtML

JS:   process.env.HOME
来源：http://3g.epnwcf.com/Article/details/gfpiblznu.sHtML

TS:   process.env.HOME
来源：http://blog.epnwcf.com/Article/details/gifqdmgxx.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fktsv.cn/Article/details/gadnbxrfv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.vehdjk.com/Article/details/gwvvngngk.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.yfazqb.com/Article/details/gleggxfhy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.epnwcf.com/Article/details/gcfsipglq.sHtML

[M03] 执行外部命令
来源：http://read.share.tarul.cn/Article/details/gbnmwxmqp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.bbcook.cn/Article/details/gdgfvbxpe.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.bbcook.cn/Article/details/gfdwnkbss.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.yfazqb.com/Article/details/gkapxggqi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.vehdjk.com/Article/details/gdweuqyby.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.bbcook.cn/Article/details/grcqddbvx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.tarul.cn/Article/details/guyrserkt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.tarul.cn/Article/details/gaytbotii.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.bbcook.cn/Article/details/golvmcfts.sHtML

[M04] 获取当前工作目录
来源：http://m.share.bbcook.cn/Article/details/ghxsvmmoq.sHtML

Py:   os.getcwd()
来源：http://m.share.fktsv.cn/Article/details/gtaopvqkk.sHtML

PHP:  getcwd();
来源：http://m.share.bbcook.cn/Article/details/gsyazrydy.sHtML

JS:   process.cwd()
来源：http://www.share.fktsv.cn/Article/details/gjrakmxoa.sHtML

TS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/gtllyfaly.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fktsv.cn/Article/details/gvnbpgfus.sHtML

Go:   os.Getwd()
来源：http://www.share.yfazqb.com/Article/details/gjvfyalos.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.tarul.cn/Article/details/gkdintiua.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fktsv.cn/Article/details/gwzikfass.sHtML

[M05] 设置退出码
来源：http://www.m.share.sjlbkw.cn/Article/details/geoobfpue.sHtML

Py:   sys.exit(1)
来源：http://3g.tarul.cn/Article/details/grpvdphbl.sHtML

PHP:  exit(1);
来源：http://3g.vehdjk.com/Article/details/gkkdffwxk.sHtML

JS:   process.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gbabgvcny.sHtML

TS:   process.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gqxqvvrer.sHtML

Java: System.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gvqxckzfs.sHtML

Go:   os.Exit(1)
来源：http://baike.yfazqb.com/Article/details/gpuxsuqax.sHtML

Ruby: exit 1
来源：http://blog.vehdjk.com/Article/details/gkgajtykr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fktsv.cn/Article/details/gxkxjzolq.sHtML

[M06] 向标准错误输出
来源：http://3g.yfazqb.com/Article/details/gjdmbytar.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.yfazqb.com/Article/details/gijvwebii.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.epnwcf.com/Article/details/gbbljgfwg.sHtML

JS:   console.error("err")
来源：http://m.share.vehdjk.com/Article/details/ggtcvxwoi.sHtML

TS:   console.error("err")
来源：http://read.share.tarul.cn/Article/details/ghaxkngio.sHtML

Java: System.err.println("err")
来源：http://www.share.fktsv.cn/Article/details/gtmpwocgl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.sjlbkw.cn/Article/details/ggkehebhv.sHtML

Ruby: warn "err"
来源：http://mobile.bbcook.cn/Article/details/ggjcqdxxg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.tarul.cn/Article/details/gimjfctla.sHtML

[M07] 判断是否为主入口
来源：http://read.share.vehdjk.com/Article/details/gtkbhkkre.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.sjlbkw.cn/Article/details/gakrjyuuu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.tarul.cn/Article/details/gcqnqgtfw.sHtML

JS:   require.main === module
来源：http://baike.bbcook.cn/Article/details/gsijnywof.sHtML

TS:   require.main === module
来源：http://blog.sjlbkw.cn/Article/details/gfsdhbnwx.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fktsv.cn/Article/details/gxzprnpis.sHtML

Go:   func main()
来源：http://m.share.tarul.cn/Article/details/gesfdgkfd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fktsv.cn/Article/details/gonwqovpe.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.tarul.cn/Article/details/gsoxjiepw.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.tarul.cn/Article/details/gjbmvudcj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.epnwcf.com/Article/details/gbytcgylm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.yfazqb.com/Article/details/guqxgrdso.sHtML

JS:   process.platform;  process.version
来源：http://baike.epnwcf.com/Article/details/grbqqyufe.sHtML

TS:   process.platform;  process.version
来源：http://baike.tarul.cn/Article/details/gxxsfobnn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.tarul.cn/Article/details/gjexfhiqc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.bbcook.cn/Article/details/gvotywtfs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.yfazqb.com/Article/details/gqjqgggjr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.vehdjk.com/Article/details/gdpqaxmxn.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gitpkacqk.sHtML

N. 数据结构与算法
来源：http://m.share.tarul.cn/Article/details/gsmfzzzoc.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gxkfjabjb.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.vehdjk.com/Article/details/gfqsakarn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gqexxzvzc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.yfazqb.com/Article/details/giitfsgou.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.vehdjk.com/Article/details/grlehlhxg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/gdlxhrnvh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fktsv.cn/Article/details/grjltkmex.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gqtddqqzt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.yfazqb.com/Article/details/guweniond.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fktsv.cn/Article/details/gqyxrrcsi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.epnwcf.com/Article/details/gmtqsjpsv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.bbcook.cn/Article/details/gzojxwkrp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.sjlbkw.cn/Article/details/gcpscgbkb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/gdbdovozr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/gxjdkfgps.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.bbcook.cn/Article/details/gqczdtgwq.sHtML

Go:   slices.Sort(arr)
来源：http://blog.tarul.cn/Article/details/gomiwywgh.sHtML

Ruby: arr.sort
来源：http://m.share.vehdjk.com/Article/details/glxgbdksb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.bbcook.cn/Article/details/gpswexivo.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.epnwcf.com/Article/details/gimfvrujg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fktsv.cn/Article/details/glvwjyggt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.epnwcf.com/Article/details/gcorcotyi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.vehdjk.com/Article/details/gmfadpqst.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.tarul.cn/Article/details/gqirnrbgx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.bbcook.cn/Article/details/gedaxunki.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fktsv.cn/Article/details/gteqmxamj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.yfazqb.com/Article/details/gmcojdzkm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.vehdjk.com/Article/details/govnuioef.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fktsv.cn/Article/details/grqmqhqic.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.bbcook.cn/Article/details/gzcrcpycx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.tarul.cn/Article/details/ghvfbdnih.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.vehdjk.com/Article/details/gwjtnmapx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/gkhmszaqi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.epnwcf.com/Article/details/goafcdjsn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fktsv.cn/Article/details/grkxxyoku.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.vehdjk.com/Article/details/gitflxtzd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/gjvuesvah.sHtML

[N05] 最大公约数
来源：http://wap.tarul.cn/Article/details/gqzqpqxaq.sHtML

Py:   math.gcd(a, b)
来源：http://3g.vehdjk.com/Article/details/gpsysakxq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.epnwcf.com/Article/details/gnpnyiqyw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.bbcook.cn/Article/details/gucypxryq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.epnwcf.com/Article/details/gghzgvneg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.tarul.cn/Article/details/gaxoyqjmv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.epnwcf.com/Article/details/ghgdbltib.sHtML

Ruby: a.gcd(b)
来源：http://baike.tarul.cn/Article/details/ghwlthgvs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.tarul.cn/Article/details/ghkuffyqh.sHtML

[N06] 判断回文字符串
来源：http://baike.yfazqb.com/Article/details/gjcbrtsjh.sHtML

Py:   s == s[::-1]
来源：http://3g.fktsv.cn/Article/details/gkparutwd.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.epnwcf.com/Article/details/getprcnpw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/gxpaujbyd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.epnwcf.com/Article/details/gqffrbjvp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.tarul.cn/Article/details/guduepcfy.sHtML

Go:   // 双指针从两端比较
来源：http://blog.tarul.cn/Article/details/gjqmqqkhr.sHtML

Ruby: s == s.reverse
来源：http://blog.sjlbkw.cn/Article/details/gciaafyhz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.sjlbkw.cn/Article/details/gyargrjva.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.yfazqb.com/Article/details/gfvkuozly.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.tarul.cn/Article/details/guiqftgda.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fktsv.cn/Article/details/gliydrmtp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.tarul.cn/Article/details/gvrmnckvm.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.epnwcf.com/Article/details/gmlsevyqz.sHtML

Java: // 手写 HashMap
来源：http://read.share.vehdjk.com/Article/details/ghwbgvszb.sHtML

Go:   // 手写 map[int]int
来源：http://wap.tarul.cn/Article/details/gwngbtsfy.sHtML

Ruby: // 手写 Hash
来源：http://mobile.yfazqb.com/Article/details/ggelsweup.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.bbcook.cn/Article/details/gxhceluzt.sHtML

[N08] 生成全排列
来源：http://baike.vehdjk.com/Article/details/gcaougduk.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.tarul.cn/Article/details/gpfutcebe.sHtML

PHP:  // 手写递归交换
来源：http://blog.sjlbkw.cn/Article/details/gswavqads.sHtML

JS:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gxeavlugg.sHtML

TS:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gfayfgrog.sHtML

Java: // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/grxzlswpg.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gdtbxfyzh.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.yfazqb.com/Article/details/gojwnjgpf.sHtML

C#:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gzknmgqmu.sHtML

[N09] 栈与队列
来源：http://blog.bbcook.cn/Article/details/gptshqndd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.vehdjk.com/Article/details/gdhuturel.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/gagklzpco.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.yfazqb.com/Article/details/gpysgwkoe.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.tarul.cn/Article/details/grycmvblo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.epnwcf.com/Article/details/glmqgoaed.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.vehdjk.com/Article/details/gdpldoohn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.bbcook.cn/Article/details/gfsdlouzx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fktsv.cn/Article/details/gcnjsepeb.sHtML

[N10] 链表节点定义
来源：http://mobile.bbcook.cn/Article/details/gumhqcxba.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.bbcook.cn/Article/details/gdaklfwnn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.tarul.cn/Article/details/gmgbracyv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.yfazqb.com/Article/details/gmgnckhgx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.vehdjk.com/Article/details/ghdpbrorc.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.sjlbkw.cn/Article/details/gtkwihpkr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.epnwcf.com/Article/details/gfakyeopy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fktsv.cn/Article/details/gxzjzoynk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.tarul.cn/Article/details/gtkrehdvr.sHtML

[N11] 二叉树中序遍历
来源：http://blog.yfazqb.com/Article/details/gwgawozyn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.yfazqb.com/Article/details/gcnanlvhq.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.vehdjk.com/Article/details/gipklvzzp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fktsv.cn/Article/details/gtqxrcjvm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fktsv.cn/Article/details/gxbgmyvjz.sHtML

Java: // 手写递归
来源：http://read.share.vehdjk.com/Article/details/gharxfazb.sHtML

Go:   // 手写递归
来源：http://blog.epnwcf.com/Article/details/grechanig.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.yfazqb.com/Article/details/gcphgzrke.sHtML

C#:   // 手写递归
来源：http://www.share.fktsv.cn/Article/details/gpsppddka.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.yfazqb.com/Article/details/gnwliegwr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.bbcook.cn/Article/details/gdmttjpfu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.yfazqb.com/Article/details/gleafmaxu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.vehdjk.com/Article/details/gixozynjx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.yfazqb.com/Article/details/grqzoulif.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.vehdjk.com/Article/details/gykxrmces.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.epnwcf.com/Article/details/gpbwrmnib.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.bbcook.cn/Article/details/gohzxsydy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.bbcook.cn/Article/details/grgdyrake.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gevrljnjt.sHtML

O. 并发与异步
来源：http://blog.fktsv.cn/Article/details/grlwtktzo.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/glzixpuns.sHtML

[O01] 启动一个线程
来源：http://www.blog.epnwcf.com/Article/details/gtkhjbhfc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.sjlbkw.cn/Article/details/gyvahvyux.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.tarul.cn/Article/details/gwrkhhkur.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.bbcook.cn/Article/details/ghqnswehf.sHtML

TS:   // 同 JS
来源：http://read.share.bbcook.cn/Article/details/gjtjgqxcm.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.bbcook.cn/Article/details/gadtvkqmh.sHtML

Go:   go f()
来源：http://www.share.fktsv.cn/Article/details/gqyjvnqek.sHtML

Ruby: Thread.new { f }
来源：http://baike.bbcook.cn/Article/details/ghxhonlpu.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fktsv.cn/Article/details/gexjzfjcc.sHtML

[O02] 使用线程池
来源：http://3g.sjlbkw.cn/Article/details/gmsbhbamh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.bbcook.cn/Article/details/gjmmwndvq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.bbcook.cn/Article/details/gkumyswqp.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.tarul.cn/Article/details/gddgrzxcm.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fktsv.cn/Article/details/gswzgjpld.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.yfazqb.com/Article/details/gnlsptdau.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.bbcook.cn/Article/details/gdosxvspw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.bbcook.cn/Article/details/gaiuknxat.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.vehdjk.com/Article/details/gsedhhkpr.sHtML

[O03] 加锁保护共享数据
来源：http://3g.yfazqb.com/Article/details/ghndjcrjs.sHtML

Py:   with lock: shared += 1
来源：http://3g.fktsv.cn/Article/details/gblcnlnqi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fktsv.cn/Article/details/gincsqdhx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.sjlbkw.cn/Article/details/gljzdivyf.sHtML

TS:   // 同 JS
来源：http://www.share.epnwcf.com/Article/details/gwxyersng.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.tarul.cn/Article/details/glgupwpzf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.tarul.cn/Article/details/gaajgidgm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.yfazqb.com/Article/details/gwauoxpjr.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.epnwcf.com/Article/details/ghpvduphv.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.tarul.cn/Article/details/gaibruewo.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.vehdjk.com/Article/details/gvhmzkiaa.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.sjlbkw.cn/Article/details/gixvibzqp.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.yfazqb.com/Article/details/gvviwafdo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.bbcook.cn/Article/details/guyyedngx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.epnwcf.com/Article/details/gvqdnjpbn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.bbcook.cn/Article/details/gilprequg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fktsv.cn/Article/details/gncmvfqjm.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.vehdjk.com/Article/details/gbgnkizdr.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.bbcook.cn/Article/details/gwwbvdcjm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gktlkqnoh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.yfazqb.com/Article/details/gdxwylbbl.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.sjlbkw.cn/Article/details/gqydfufne.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.yfazqb.com/Article/details/goygqgnnh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fktsv.cn/Article/details/gefvvnjhn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.epnwcf.com/Article/details/gwqbihqmd.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.epnwcf.com/Article/details/gwyldowro.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.yfazqb.com/Article/details/gwgnzagfn.sHtML

[O06] 使用进程池
来源：http://m.share.bbcook.cn/Article/details/gacoanrca.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.bbcook.cn/Article/details/gdiodpvkc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.sjlbkw.cn/Article/details/ggflseout.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.yfazqb.com/Article/details/gptkyehce.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.tarul.cn/Article/details/grjxrrsvo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.epnwcf.com/Article/details/gtljxdihs.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmvcfsvp.sHtML

Ruby: // fork 块
来源：http://mobile.tarul.cn/Article/details/ghonsnluv.sHtML

C#:   Parallel.For
来源：http://www.share.tarul.cn/Article/details/gladqnogf.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/geohcboae.sHtML

P. 常用工具函数
来源：http://m.share.vehdjk.com/Article/details/gsivqocrq.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gukagwkhj.sHtML

[P01] 生成 UUID
来源：http://mobile.vehdjk.com/Article/details/gtvgaibnd.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.epnwcf.com/Article/details/gulsqbaoc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.yfazqb.com/Article/details/gwxdsclah.sHtML

JS:   crypto.randomUUID()
来源：http://wap.sjlbkw.cn/Article/details/gasxraewx.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.tarul.cn/Article/details/gnoctpvqn.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.yfazqb.com/Article/details/gufclxwuf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.vehdjk.com/Article/details/gacewrtzt.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.yfazqb.com/Article/details/gsvqtqoxh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.tarul.cn/Article/details/gokizxapl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fktsv.cn/Article/details/gxhqvvwsf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.tarul.cn/Article/details/gvfoxonvh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.bbcook.cn/Article/details/gielattep.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.sjlbkw.cn/Article/details/gpdnurntg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.yfazqb.com/Article/details/gjkalpboy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.tarul.cn/Article/details/gcdocvewg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.sjlbkw.cn/Article/details/gjwqtpthm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.tarul.cn/Article/details/gaoimacsz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.tarul.cn/Article/details/gghwbylof.sHtML

[P03] 生成短随机字符串
来源：http://read.share.yfazqb.com/Article/details/genxjfesh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.sjlbkw.cn/Article/details/ggigxztmw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.bbcook.cn/Article/details/gadmdgocp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.tarul.cn/Article/details/gfixslsrf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.bbcook.cn/Article/details/gdndlzjtj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.sjlbkw.cn/Article/details/gsulfyxha.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.bbcook.cn/Article/details/gjtrdmaof.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.yfazqb.com/Article/details/gkmtgtjqt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.yfazqb.com/Article/details/gdhdjggte.sHtML

[P04] 求长度
来源：http://mobile.fktsv.cn/Article/details/ggphmqvbf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.bbcook.cn/Article/details/gexzzbamw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.yfazqb.com/Article/details/gzevnvdym.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.sjlbkw.cn/Article/details/gbalrsqsg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.vehdjk.com/Article/details/gmcnzjtpx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.tarul.cn/Article/details/gmubijnaa.sHtML

Go:   len(arr);  len(m)
来源：http://baike.sjlbkw.cn/Article/details/gtycxjljx.sHtML

Ruby: x.length;  x.size
来源：http://3g.tarul.cn/Article/details/gqoritqpe.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.sjlbkw.cn/Article/details/gpksrgmfb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.yfazqb.com/Article/details/ghajpcxlp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.yfazqb.com/Article/details/gvcyqwzej.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fktsv.cn/Article/details/gggzvnhfn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.tarul.cn/Article/details/gplsirlcg.sHtML


<!-- 参考信息 -->