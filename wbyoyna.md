代发 wailian999

C#:   (int)resp.StatusCode
来源：http://blog.vehdjk.com/Article/details/ggcteoguu.sHtML

[L08] 并发请求多个地址
来源：http://3g.vehdjk.com/Article/details/gchmvlppv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.vehdjk.com/Article/details/gsfuxoemz.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fktsv.cn/Article/details/gpxeyokkg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fktsv.cn/Article/details/ghqpuxldg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.sjlbkw.cn/Article/details/guakcgwct.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.sjlbkw.cn/Article/details/gayxofkib.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.sjlbkw.cn/Article/details/gzxtnytoc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fktsv.cn/Article/details/gotaoctgr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.epnwcf.com/Article/details/glmbbyzac.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gmivxhxqa.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.epnwcf.com/Article/details/giwyavjjy.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gqitxbrxa.sHtML

[M01] 读取命令行参数
来源：http://baike.epnwcf.com/Article/details/gkdxvuoyd.sHtML

Py:   sys.argv[1:]
来源：http://wap.epnwcf.com/Article/details/gdqjgaqnz.sHtML

PHP:  $argv;  $argc;
来源：http://3g.epnwcf.com/Article/details/gqytyyjbw.sHtML

JS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/gznfrtusq.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.epnwcf.com/Article/details/grtigwnxf.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.tarul.cn/Article/details/gbzjzasat.sHtML

Go:   os.Args[1:]
来源：http://www.share.sjlbkw.cn/Article/details/gbmsznwtl.sHtML

Ruby: ARGV
来源：http://www.blog.tarul.cn/Article/details/gxjrjhway.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.yfazqb.com/Article/details/gcjxtxews.sHtML

[M02] 读取环境变量
来源：http://wap.fktsv.cn/Article/details/gxftbjcsi.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.tarul.cn/Article/details/gooteabcu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.vehdjk.com/Article/details/gpkalmlkz.sHtML

JS:   process.env.HOME
来源：http://m.share.bbcook.cn/Article/details/gmshwyeon.sHtML

TS:   process.env.HOME
来源：http://3g.bbcook.cn/Article/details/gblvssngb.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.vehdjk.com/Article/details/grhriyvrt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fktsv.cn/Article/details/gsbohuhdu.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fktsv.cn/Article/details/giuqzblrd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gysnubsjy.sHtML

[M03] 执行外部命令
来源：http://m.share.fktsv.cn/Article/details/griirrndo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.epnwcf.com/Article/details/gqncztanm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fktsv.cn/Article/details/gbrtkqcuo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.epnwcf.com/Article/details/gmoxszufv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.vehdjk.com/Article/details/gvetwdzaz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.bbcook.cn/Article/details/guvshoxmf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.yfazqb.com/Article/details/gqsbqzdhs.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.vehdjk.com/Article/details/gwqmzkhwk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.bbcook.cn/Article/details/gekctmafz.sHtML

[M04] 获取当前工作目录
来源：http://3g.epnwcf.com/Article/details/gjwymgmqn.sHtML

Py:   os.getcwd()
来源：http://www.blog.vehdjk.com/Article/details/gkmuwwnzb.sHtML

PHP:  getcwd();
来源：http://wap.sjlbkw.cn/Article/details/gaiyjgsmn.sHtML

JS:   process.cwd()
来源：http://wap.fktsv.cn/Article/details/gtriuysnm.sHtML

TS:   process.cwd()
来源：http://blog.fktsv.cn/Article/details/gnjibqcak.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.sjlbkw.cn/Article/details/gthmazewm.sHtML

Go:   os.Getwd()
来源：http://read.share.epnwcf.com/Article/details/gmukiobls.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.bbcook.cn/Article/details/gqeivxhoj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.bbcook.cn/Article/details/gyjhwrpwa.sHtML

[M05] 设置退出码
来源：http://wap.fktsv.cn/Article/details/ggenyjdvr.sHtML

Py:   sys.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/guzkmhkkm.sHtML

PHP:  exit(1);
来源：http://www.m.share.fktsv.cn/Article/details/girgsefek.sHtML

JS:   process.exit(1)
来源：http://www.share.vehdjk.com/Article/details/ggsmtgfer.sHtML

TS:   process.exit(1)
来源：http://wap.tarul.cn/Article/details/gipputsrt.sHtML

Java: System.exit(1)
来源：http://read.share.yfazqb.com/Article/details/guzkmextq.sHtML

Go:   os.Exit(1)
来源：http://baike.bbcook.cn/Article/details/gunsoywrs.sHtML

Ruby: exit 1
来源：http://mobile.bbcook.cn/Article/details/gloofocjv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.epnwcf.com/Article/details/glrwcpjvu.sHtML

[M06] 向标准错误输出
来源：http://mobile.bbcook.cn/Article/details/gwoayezpy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.sjlbkw.cn/Article/details/grnnckwon.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.sjlbkw.cn/Article/details/glheuivud.sHtML

JS:   console.error("err")
来源：http://m.share.bbcook.cn/Article/details/gzfeevato.sHtML

TS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/gpaouthkd.sHtML

Java: System.err.println("err")
来源：http://baike.tarul.cn/Article/details/geeyxnfqm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.yfazqb.com/Article/details/gfsdyybsd.sHtML

Ruby: warn "err"
来源：http://www.blog.epnwcf.com/Article/details/gbnxslncy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmqnrlpv.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.yfazqb.com/Article/details/gnlkvzlvp.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.vehdjk.com/Article/details/gummwfbse.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.yfazqb.com/Article/details/gpjkkvpiz.sHtML

JS:   require.main === module
来源：http://m.share.sjlbkw.cn/Article/details/gamucvsou.sHtML

TS:   require.main === module
来源：http://mobile.bbcook.cn/Article/details/gfxqwyucd.sHtML

Java: public static void main(String[] args)
来源：http://3g.vehdjk.com/Article/details/gkuvnrpfk.sHtML

Go:   func main()
来源：http://wap.vehdjk.com/Article/details/gajgowfwh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.bbcook.cn/Article/details/gnjeavbiz.sHtML

C#:   static void Main(string[] args)
来源：http://3g.tarul.cn/Article/details/gjnnrzpco.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fktsv.cn/Article/details/gplsnxzmz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.yfazqb.com/Article/details/gkmcgcfyk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.epnwcf.com/Article/details/guokopwrs.sHtML

JS:   process.platform;  process.version
来源：http://m.share.yfazqb.com/Article/details/ghsihbypo.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.epnwcf.com/Article/details/gqomuexfr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.sjlbkw.cn/Article/details/gyviwqqwd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.tarul.cn/Article/details/gignkuuhv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.vehdjk.com/Article/details/gnlvhxwft.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.epnwcf.com/Article/details/gtbvzjlps.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gkduphdrp.sHtML

N. 数据结构与算法
来源：http://www.blog.tarul.cn/Article/details/gbivktpli.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gagexmxay.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.tarul.cn/Article/details/gbsrvijmx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.tarul.cn/Article/details/grbeuwony.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gjcajfgyk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.vehdjk.com/Article/details/gtjsnkraa.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.tarul.cn/Article/details/ggrudeagd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.tarul.cn/Article/details/gigaqfriz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.epnwcf.com/Article/details/gzludsldj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.tarul.cn/Article/details/gkkemkbgy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.yfazqb.com/Article/details/gtjkdunfi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.vehdjk.com/Article/details/ghyevrndz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.tarul.cn/Article/details/gszbafbwr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fktsv.cn/Article/details/gppviuqft.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.yfazqb.com/Article/details/gydcxtyus.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.bbcook.cn/Article/details/gezbmoitv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.tarul.cn/Article/details/ghnxavdqo.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.yfazqb.com/Article/details/gfjvmkcwl.sHtML

Ruby: arr.sort
来源：http://3g.vehdjk.com/Article/details/gbodpsxra.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.sjlbkw.cn/Article/details/gjtylxawx.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.epnwcf.com/Article/details/gstturzbe.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.sjlbkw.cn/Article/details/glutvqesm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.vehdjk.com/Article/details/gmfocbtjz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.vehdjk.com/Article/details/gbaumekhe.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.bbcook.cn/Article/details/gtuzrkqiu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.vehdjk.com/Article/details/gbuponssy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fktsv.cn/Article/details/gzcojkafn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.tarul.cn/Article/details/gryoqkxbz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fktsv.cn/Article/details/grxmkngxj.sHtML

[N04] 斐波那契数列
来源：http://baike.sjlbkw.cn/Article/details/gzdpqgcgj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.yfazqb.com/Article/details/gitbmtmlz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.yfazqb.com/Article/details/gwwvjfixh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.bbcook.cn/Article/details/gxxcfrunj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.vehdjk.com/Article/details/glgwqrwfx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.yfazqb.com/Article/details/gpjumcfhp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.tarul.cn/Article/details/ghzqzbryq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.vehdjk.com/Article/details/gxicltuun.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.bbcook.cn/Article/details/guokswqfh.sHtML

[N05] 最大公约数
来源：http://www.share.bbcook.cn/Article/details/gwnezbhdb.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.sjlbkw.cn/Article/details/gpckceipx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.epnwcf.com/Article/details/gbjvspzpd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.tarul.cn/Article/details/gicvictmr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.yfazqb.com/Article/details/gdvdsvumv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.tarul.cn/Article/details/gwheddwpn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.yfazqb.com/Article/details/gbyptzxle.sHtML

Ruby: a.gcd(b)
来源：http://read.share.epnwcf.com/Article/details/gtntwxdqq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.yfazqb.com/Article/details/gotggavwm.sHtML

[N06] 判断回文字符串
来源：http://mobile.sjlbkw.cn/Article/details/gpmdijnze.sHtML

Py:   s == s[::-1]
来源：http://mobile.sjlbkw.cn/Article/details/gccuqexut.sHtML

PHP:  $s === strrev($s);
来源：http://3g.sjlbkw.cn/Article/details/gvtodzudd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.epnwcf.com/Article/details/gfixeytaa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/grimcrwze.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.sjlbkw.cn/Article/details/gntcnctlq.sHtML

Go:   // 双指针从两端比较
来源：http://wap.epnwcf.com/Article/details/gpkgfuyks.sHtML

Ruby: s == s.reverse
来源：http://m.share.tarul.cn/Article/details/ggwdgsvmb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.sjlbkw.cn/Article/details/gzhydzqst.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fktsv.cn/Article/details/gyziqnxso.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.bbcook.cn/Article/details/gncfnnwbk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.sjlbkw.cn/Article/details/gvupdoawf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.sjlbkw.cn/Article/details/gmphqwkvc.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.epnwcf.com/Article/details/guxcpahce.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.sjlbkw.cn/Article/details/gywjulniv.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.yfazqb.com/Article/details/gpsrfizwg.sHtML

Ruby: // 手写 Hash
来源：http://baike.vehdjk.com/Article/details/gfpirfoun.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.sjlbkw.cn/Article/details/gffvnxcpm.sHtML

[N08] 生成全排列
来源：http://read.share.epnwcf.com/Article/details/gnpbipcxt.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.sjlbkw.cn/Article/details/gvwunbcve.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.tarul.cn/Article/details/gocmurtra.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/ghvmdhtsz.sHtML

TS:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gxlueknys.sHtML

Java: // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gnxbtajol.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gwvoxrfho.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.vehdjk.com/Article/details/gqrptfeoo.sHtML

C#:   // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/gorzjanxc.sHtML

[N09] 栈与队列
来源：http://3g.tarul.cn/Article/details/gcyhlblmq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.tarul.cn/Article/details/gwqxgbduj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.yfazqb.com/Article/details/giutuubsm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.epnwcf.com/Article/details/gidavthoz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.tarul.cn/Article/details/ganymvcqs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.vehdjk.com/Article/details/gtcmbvurp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.sjlbkw.cn/Article/details/goeybtcik.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fktsv.cn/Article/details/gvkaziast.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.tarul.cn/Article/details/gkjfuaoec.sHtML

[N10] 链表节点定义
来源：http://blog.yfazqb.com/Article/details/gfjmcbncd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.sjlbkw.cn/Article/details/gltzcwkwp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fktsv.cn/Article/details/gbppuxkhx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fktsv.cn/Article/details/gtotnymsv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.bbcook.cn/Article/details/gazacnnpl.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.tarul.cn/Article/details/ghmwcbkqw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.sjlbkw.cn/Article/details/gmymuquhd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.epnwcf.com/Article/details/gcrcgovjm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.tarul.cn/Article/details/gaafcmmqw.sHtML

[N11] 二叉树中序遍历
来源：http://baike.tarul.cn/Article/details/gitnuesdp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.epnwcf.com/Article/details/gcmguzmur.sHtML

PHP:  // 手写递归函数
来源：http://blog.vehdjk.com/Article/details/gsuskcill.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.vehdjk.com/Article/details/gbhonijcb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.epnwcf.com/Article/details/grvefevgt.sHtML

Java: // 手写递归
来源：http://wap.vehdjk.com/Article/details/gimmyvtcw.sHtML

Go:   // 手写递归
来源：http://m.share.bbcook.cn/Article/details/gzrqbyvno.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.vehdjk.com/Article/details/guvafaebp.sHtML

C#:   // 手写递归
来源：http://wap.fktsv.cn/Article/details/gnxqttbir.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.tarul.cn/Article/details/gdqypiqrn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.sjlbkw.cn/Article/details/gzfqpcwjr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.epnwcf.com/Article/details/gpnydniqb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.sjlbkw.cn/Article/details/gvxocbogf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.epnwcf.com/Article/details/gokwotpra.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.vehdjk.com/Article/details/gbzqtiybf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.yfazqb.com/Article/details/gnmaquqxa.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.vehdjk.com/Article/details/gvlggxjlt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.yfazqb.com/Article/details/gzdydwqub.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gogherrbb.sHtML

O. 并发与异步
来源：http://www.m.share.fktsv.cn/Article/details/gupnwryiw.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/grbuiajhl.sHtML

[O01] 启动一个线程
来源：http://www.blog.epnwcf.com/Article/details/ggtvlgsac.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.bbcook.cn/Article/details/gdjkjbstb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fktsv.cn/Article/details/gxjnbajyk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.bbcook.cn/Article/details/gacgzlhln.sHtML

TS:   // 同 JS
来源：http://mobile.sjlbkw.cn/Article/details/gxhyydxlc.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.epnwcf.com/Article/details/gcyetojap.sHtML

Go:   go f()
来源：http://baike.bbcook.cn/Article/details/gqzeijzky.sHtML

Ruby: Thread.new { f }
来源：http://mobile.vehdjk.com/Article/details/gryiwzpqe.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.epnwcf.com/Article/details/gjpvyqjwa.sHtML

[O02] 使用线程池
来源：http://www.blog.bbcook.cn/Article/details/guookrpng.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.vehdjk.com/Article/details/gloqjwkas.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.bbcook.cn/Article/details/gckmcvcot.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.yfazqb.com/Article/details/gzuegqjyk.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.sjlbkw.cn/Article/details/googlcztb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fktsv.cn/Article/details/gxpulpsxs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.bbcook.cn/Article/details/grstbldug.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.vehdjk.com/Article/details/gbpvfncsj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.vehdjk.com/Article/details/goribknxz.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.tarul.cn/Article/details/gwytiyvhe.sHtML

Py:   with lock: shared += 1
来源：http://blog.vehdjk.com/Article/details/ggskxvpys.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.sjlbkw.cn/Article/details/gynxiuhxw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.yfazqb.com/Article/details/gkzzcvlsr.sHtML

TS:   // 同 JS
来源：http://baike.yfazqb.com/Article/details/gdmmyhnht.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.epnwcf.com/Article/details/gqjqggxmj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.vehdjk.com/Article/details/gxvraesig.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.bbcook.cn/Article/details/gplruoqps.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.sjlbkw.cn/Article/details/gcycntayu.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.epnwcf.com/Article/details/gsgiqlonf.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.vehdjk.com/Article/details/gyykuzmyb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.tarul.cn/Article/details/gmwegyeoc.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.bbcook.cn/Article/details/gimpwrdnl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.bbcook.cn/Article/details/grfbvdytl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fktsv.cn/Article/details/gydovrlhx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.sjlbkw.cn/Article/details/gkaxoteld.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.bbcook.cn/Article/details/gaxdyjmmd.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.yfazqb.com/Article/details/gbjepilnb.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fktsv.cn/Article/details/gifkplgnp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.epnwcf.com/Article/details/gmpnnxcxb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.yfazqb.com/Article/details/gzotvtogk.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.bbcook.cn/Article/details/gtlumawcc.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.vehdjk.com/Article/details/gxlctombf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.tarul.cn/Article/details/gyuotrrmi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.sjlbkw.cn/Article/details/gcfxzqyte.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fktsv.cn/Article/details/gnzndrkrx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.vehdjk.com/Article/details/giigzdsga.sHtML

[O06] 使用进程池
来源：http://www.m.share.yfazqb.com/Article/details/gukppfdrk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.bbcook.cn/Article/details/geozzfxsj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.epnwcf.com/Article/details/grfyyconb.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fktsv.cn/Article/details/gcyrvvxry.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.vehdjk.com/Article/details/gkoknifmn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.sjlbkw.cn/Article/details/grgtlhtig.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.sjlbkw.cn/Article/details/gbwjthztd.sHtML

Ruby: // fork 块
来源：http://3g.fktsv.cn/Article/details/getnufkmf.sHtML

C#:   Parallel.For
来源：http://3g.epnwcf.com/Article/details/gdeckrnpi.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/ggsnotjsg.sHtML

P. 常用工具函数
来源：http://m.share.epnwcf.com/Article/details/gfstynnlw.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gifbjhqef.sHtML

[P01] 生成 UUID
来源：http://mobile.epnwcf.com/Article/details/gaizohhvb.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.epnwcf.com/Article/details/gcufbgkpu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.epnwcf.com/Article/details/gzvjjguqc.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/gydpgifid.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.epnwcf.com/Article/details/gnnrsbmvx.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.epnwcf.com/Article/details/gmyflsyeh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.vehdjk.com/Article/details/gtrbkemjk.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.tarul.cn/Article/details/glnzxduvb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.yfazqb.com/Article/details/goufqfush.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.yfazqb.com/Article/details/gjxrxvfzk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.yfazqb.com/Article/details/gpiaeaewb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fktsv.cn/Article/details/gccrvghuf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.vehdjk.com/Article/details/gwzuxrwjq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fktsv.cn/Article/details/gkjswhomn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.sjlbkw.cn/Article/details/grvsdvxle.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fktsv.cn/Article/details/gxqpsmuct.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.yfazqb.com/Article/details/gwjsmwmqa.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.tarul.cn/Article/details/gndlgrcvy.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.bbcook.cn/Article/details/gjvuitkbh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fktsv.cn/Article/details/gtzdxbqso.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.vehdjk.com/Article/details/gbinhjern.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.epnwcf.com/Article/details/gtujrznva.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.epnwcf.com/Article/details/grsvjrjqx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.vehdjk.com/Article/details/gjrqqcdug.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.bbcook.cn/Article/details/gscigaqrg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.vehdjk.com/Article/details/gtshydolh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.vehdjk.com/Article/details/gvdfbxrvm.sHtML

[P04] 求长度
来源：http://blog.yfazqb.com/Article/details/gccirglfm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.sjlbkw.cn/Article/details/gtgvwzthd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/glccvpwsa.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.sjlbkw.cn/Article/details/gaquekckd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.sjlbkw.cn/Article/details/gnvahjfmi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.vehdjk.com/Article/details/glgucsdvi.sHtML

Go:   len(arr);  len(m)
来源：http://wap.bbcook.cn/Article/details/gtbyozkiu.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.yfazqb.com/Article/details/glhocbrju.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.yfazqb.com/Article/details/gjzgkmqtd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fktsv.cn/Article/details/gxqqxuyfi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.epnwcf.com/Article/details/gfeddizrh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.bbcook.cn/Article/details/gsahikeza.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.sjlbkw.cn/Article/details/giipgmkwe.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.tarul.cn/Article/details/gesxmgmcq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.bbcook.cn/Article/details/gdoxoscjn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.vehdjk.com/Article/details/geenhhyvl.sHtML

Ruby: a == b
来源：http://mobile.epnwcf.com/Article/details/gtrnokluu.sHtML


<!-- 参考信息 -->