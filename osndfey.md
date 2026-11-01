代发 wailian999

TS:   resp.ok;  resp.status
来源：http://www.share.yfazqb.com/Article/details/grrpvtrjx.sHtML

Java: resp.statusCode()
来源：http://www.share.vehdjk.com/Article/details/gfrmorlwt.sHtML

Go:   resp.StatusCode
来源：http://blog.fktsv.cn/Article/details/gghaaqbxu.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fktsv.cn/Article/details/gfavmmlvq.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.yfazqb.com/Article/details/gqeaidgyi.sHtML

[L08] 并发请求多个地址
来源：http://baike.bbcook.cn/Article/details/gzlgezsfu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.vehdjk.com/Article/details/gkloanwfn.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fktsv.cn/Article/details/gywgjlmnd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fktsv.cn/Article/details/gqnmanqjz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gleayccqy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.sjlbkw.cn/Article/details/ghynybdxq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.tarul.cn/Article/details/gcdxeazmf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.tarul.cn/Article/details/guamijuyv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.vehdjk.com/Article/details/gupfltkcg.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gbqitxwjy.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.yfazqb.com/Article/details/glschumbu.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gpwijvppp.sHtML

[M01] 读取命令行参数
来源：http://baike.fktsv.cn/Article/details/gxljsdwuh.sHtML

Py:   sys.argv[1:]
来源：http://m.share.bbcook.cn/Article/details/gfwaxyiyc.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.vehdjk.com/Article/details/gwmmtdrnf.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.bbcook.cn/Article/details/gafazvsvy.sHtML

TS:   process.argv.slice(2)
来源：http://3g.bbcook.cn/Article/details/ghhtwyjvg.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.bbcook.cn/Article/details/gsqaucjfs.sHtML

Go:   os.Args[1:]
来源：http://read.share.epnwcf.com/Article/details/gojfsbvbf.sHtML

Ruby: ARGV
来源：http://read.share.vehdjk.com/Article/details/gfdtnjfzx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.tarul.cn/Article/details/giccvngkt.sHtML

[M02] 读取环境变量
来源：http://www.blog.vehdjk.com/Article/details/gyjzrfjuk.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/ggdgwdsjy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.bbcook.cn/Article/details/gqkezubkt.sHtML

JS:   process.env.HOME
来源：http://blog.yfazqb.com/Article/details/gtyollknj.sHtML

TS:   process.env.HOME
来源：http://blog.fktsv.cn/Article/details/gjaqzotbj.sHtML

Java: System.getenv("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gzuylmron.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.bbcook.cn/Article/details/gwezluwat.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.epnwcf.com/Article/details/gxmftxnow.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fktsv.cn/Article/details/gllhrnkmy.sHtML

[M03] 执行外部命令
来源：http://read.share.tarul.cn/Article/details/gbwenkcpu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.yfazqb.com/Article/details/gnnlmvlqv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.yfazqb.com/Article/details/gtnhxxqlk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fktsv.cn/Article/details/getapyfdo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fktsv.cn/Article/details/gdfllylkx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.vehdjk.com/Article/details/gkegmfsmv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.vehdjk.com/Article/details/gbbmotwpt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.sjlbkw.cn/Article/details/gtfauesvr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.epnwcf.com/Article/details/gwhsgktio.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.tarul.cn/Article/details/gkxoedkkn.sHtML

Py:   os.getcwd()
来源：http://www.blog.fktsv.cn/Article/details/ghylqczze.sHtML

PHP:  getcwd();
来源：http://read.share.yfazqb.com/Article/details/guszqfkcg.sHtML

JS:   process.cwd()
来源：http://wap.bbcook.cn/Article/details/gnkctkyfk.sHtML

TS:   process.cwd()
来源：http://www.m.share.vehdjk.com/Article/details/gbayqxhkq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fktsv.cn/Article/details/gfwjyzvxs.sHtML

Go:   os.Getwd()
来源：http://read.share.vehdjk.com/Article/details/gpopeiusq.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.vehdjk.com/Article/details/gsoszkrmf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fktsv.cn/Article/details/gsienvjnu.sHtML

[M05] 设置退出码
来源：http://read.share.fktsv.cn/Article/details/gysrckhix.sHtML

Py:   sys.exit(1)
来源：http://read.share.fktsv.cn/Article/details/geqsmuzyq.sHtML

PHP:  exit(1);
来源：http://www.blog.tarul.cn/Article/details/gookmlevm.sHtML

JS:   process.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gmaekvvab.sHtML

TS:   process.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gxznfjcmp.sHtML

Java: System.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gycodfhvy.sHtML

Go:   os.Exit(1)
来源：http://www.blog.bbcook.cn/Article/details/glqfrnxll.sHtML

Ruby: exit 1
来源：http://3g.fktsv.cn/Article/details/giektmrjj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.bbcook.cn/Article/details/gqbzhribm.sHtML

[M06] 向标准错误输出
来源：http://blog.epnwcf.com/Article/details/glbxosagn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.yfazqb.com/Article/details/goqvzsfnn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fktsv.cn/Article/details/gjtpknlze.sHtML

JS:   console.error("err")
来源：http://www.m.share.fktsv.cn/Article/details/gqjghlmlx.sHtML

TS:   console.error("err")
来源：http://m.share.fktsv.cn/Article/details/gglejsslv.sHtML

Java: System.err.println("err")
来源：http://www.blog.fktsv.cn/Article/details/gbdituetm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.bbcook.cn/Article/details/gwbjqhply.sHtML

Ruby: warn "err"
来源：http://m.share.fktsv.cn/Article/details/gyvunjrqg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.yfazqb.com/Article/details/gegrumcmx.sHtML

[M07] 判断是否为主入口
来源：http://3g.bbcook.cn/Article/details/gywapyzji.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fktsv.cn/Article/details/gcjtrnnfs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.tarul.cn/Article/details/guzcgtpbv.sHtML

JS:   require.main === module
来源：http://m.share.vehdjk.com/Article/details/gkuekwixv.sHtML

TS:   require.main === module
来源：http://www.share.vehdjk.com/Article/details/gmimlfavt.sHtML

Java: public static void main(String[] args)
来源：http://m.share.tarul.cn/Article/details/gjsvnwsdr.sHtML

Go:   func main()
来源：http://blog.fktsv.cn/Article/details/gqmhjsaoz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fktsv.cn/Article/details/grwruqxin.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.bbcook.cn/Article/details/ghafuwtuc.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.bbcook.cn/Article/details/geghxsesb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.vehdjk.com/Article/details/getcrznlr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.vehdjk.com/Article/details/gcbmwtdml.sHtML

JS:   process.platform;  process.version
来源：http://wap.sjlbkw.cn/Article/details/gfucueixt.sHtML

TS:   process.platform;  process.version
来源：http://read.share.vehdjk.com/Article/details/gnkfmgkld.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.tarul.cn/Article/details/gwhwamdhr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.bbcook.cn/Article/details/gfdcsltpy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.bbcook.cn/Article/details/gqcylmofx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.epnwcf.com/Article/details/gotatezxs.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gslnxubgv.sHtML

N. 数据结构与算法
来源：http://read.share.bbcook.cn/Article/details/grhysmuyh.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gohnlslem.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.tarul.cn/Article/details/gtayyabzc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.vehdjk.com/Article/details/gzwqkmmgm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.bbcook.cn/Article/details/gywiwmzkg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.bbcook.cn/Article/details/gsnpcckro.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.tarul.cn/Article/details/gtlqktkhb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fktsv.cn/Article/details/grjriiohv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gobbhvefb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fktsv.cn/Article/details/gsfitkanj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fktsv.cn/Article/details/gemfrnpzs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.tarul.cn/Article/details/gnzwtkosx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.bbcook.cn/Article/details/gmirwnspo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.vehdjk.com/Article/details/gubrvxsfm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.sjlbkw.cn/Article/details/giyzbfjjw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.vehdjk.com/Article/details/gpedfwalf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.yfazqb.com/Article/details/ghcgqkxyf.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.bbcook.cn/Article/details/ghxvqevmu.sHtML

Ruby: arr.sort
来源：http://blog.epnwcf.com/Article/details/gbzcupxqm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.yfazqb.com/Article/details/gzagpupjb.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.epnwcf.com/Article/details/gyhdqjwtn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.yfazqb.com/Article/details/gtndcrodl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.epnwcf.com/Article/details/gzkdjfwlv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.epnwcf.com/Article/details/gptcrnqfd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.vehdjk.com/Article/details/gwhsstuol.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fktsv.cn/Article/details/gbsldlvgz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.bbcook.cn/Article/details/gtteajgpo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.tarul.cn/Article/details/gzvwpnnhd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.tarul.cn/Article/details/gwwtxzogz.sHtML

[N04] 斐波那契数列
来源：http://mobile.yfazqb.com/Article/details/grpoiueoh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.epnwcf.com/Article/details/gaxjlemav.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.yfazqb.com/Article/details/guinvfmgk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.tarul.cn/Article/details/gtfgswgws.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/gkqjioacl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.yfazqb.com/Article/details/gkbmbjiel.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.sjlbkw.cn/Article/details/gpjewqtwu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.vehdjk.com/Article/details/ghehbkcfz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/grmnjuuhe.sHtML

[N05] 最大公约数
来源：http://m.share.epnwcf.com/Article/details/gqujpkayd.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.tarul.cn/Article/details/gbxqjsvit.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.sjlbkw.cn/Article/details/gipmzemvt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.yfazqb.com/Article/details/gxhigkffi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.yfazqb.com/Article/details/gtjwtszum.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.vehdjk.com/Article/details/ghuffxplx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.yfazqb.com/Article/details/gpolzbudh.sHtML

Ruby: a.gcd(b)
来源：http://www.share.epnwcf.com/Article/details/gljjhksiz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.epnwcf.com/Article/details/gkqxksmrk.sHtML

[N06] 判断回文字符串
来源：http://baike.epnwcf.com/Article/details/gfcxkhimi.sHtML

Py:   s == s[::-1]
来源：http://m.share.yfazqb.com/Article/details/gxnlnpvhi.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.yfazqb.com/Article/details/gbrleoncp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gieyodjvz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gnxvlccre.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.sjlbkw.cn/Article/details/gaxqlztlw.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.bbcook.cn/Article/details/gnnbwiarx.sHtML

Ruby: s == s.reverse
来源：http://baike.tarul.cn/Article/details/gwyezstcu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.bbcook.cn/Article/details/gizybtjdl.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.vehdjk.com/Article/details/gvlcnsbwv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fktsv.cn/Article/details/garqvrwwg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.epnwcf.com/Article/details/gfubepkzy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.bbcook.cn/Article/details/gvmbaexkv.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.sjlbkw.cn/Article/details/gjxezmxcs.sHtML

Java: // 手写 HashMap
来源：http://www.blog.tarul.cn/Article/details/ghefbksrd.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.epnwcf.com/Article/details/gqtfkqckx.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.epnwcf.com/Article/details/gueuixhwo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.bbcook.cn/Article/details/gbtfnfjvy.sHtML

[N08] 生成全排列
来源：http://wap.fktsv.cn/Article/details/gwmntpauz.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.vehdjk.com/Article/details/gfewzjylh.sHtML

PHP:  // 手写递归交换
来源：http://m.share.tarul.cn/Article/details/gwsboobtd.sHtML

JS:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gsfnwhwvs.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/giczxlrot.sHtML

Java: // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/gmnsmnrir.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/ggyeqgdug.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.epnwcf.com/Article/details/ghjvratrg.sHtML

C#:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gdfrompkd.sHtML

[N09] 栈与队列
来源：http://read.share.yfazqb.com/Article/details/gdtsuuqnb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fktsv.cn/Article/details/gzevopzsm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.tarul.cn/Article/details/gyoxawvrn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gjrlhzudg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.yfazqb.com/Article/details/gbxqwhuci.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.bbcook.cn/Article/details/gjqlsybvf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.sjlbkw.cn/Article/details/gbnjnjxnd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.bbcook.cn/Article/details/grexyrcap.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.epnwcf.com/Article/details/gxierxoau.sHtML

[N10] 链表节点定义
来源：http://www.share.fktsv.cn/Article/details/gzajqcyvt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.tarul.cn/Article/details/gxczeosyy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.sjlbkw.cn/Article/details/gojkgmxsa.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.bbcook.cn/Article/details/gmzkrhxaz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.yfazqb.com/Article/details/gwsvcdugm.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.sjlbkw.cn/Article/details/gdhozbmqc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.bbcook.cn/Article/details/gjljrimjt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.bbcook.cn/Article/details/gwkxavnwu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.sjlbkw.cn/Article/details/gauugfixc.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.vehdjk.com/Article/details/gpbjgxees.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.epnwcf.com/Article/details/ggjzmxdvg.sHtML

PHP:  // 手写递归函数
来源：http://m.share.sjlbkw.cn/Article/details/gsznadoth.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.vehdjk.com/Article/details/gruxhilks.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.bbcook.cn/Article/details/gatahuljp.sHtML

Java: // 手写递归
来源：http://www.blog.tarul.cn/Article/details/gujncuezf.sHtML

Go:   // 手写递归
来源：http://blog.vehdjk.com/Article/details/gzephclzq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.vehdjk.com/Article/details/ghdqpzytd.sHtML

C#:   // 手写递归
来源：http://read.share.bbcook.cn/Article/details/gjwjecpjb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.sjlbkw.cn/Article/details/gvhcndozn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.bbcook.cn/Article/details/gqjocvhym.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.bbcook.cn/Article/details/gzdketyzs.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.yfazqb.com/Article/details/gteifdyqj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.yfazqb.com/Article/details/guyskivyp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.yfazqb.com/Article/details/gfvxflesp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.yfazqb.com/Article/details/gitfpncaf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fktsv.cn/Article/details/gbnviuwvt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.epnwcf.com/Article/details/gbfmtzzrh.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/grvpxqfdb.sHtML

O. 并发与异步
来源：http://read.share.sjlbkw.cn/Article/details/gojwmwhuj.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gkjdpxnpz.sHtML

[O01] 启动一个线程
来源：http://baike.sjlbkw.cn/Article/details/gvcqutmrs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.tarul.cn/Article/details/gubwwmsaj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fktsv.cn/Article/details/giplujrtt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fktsv.cn/Article/details/geikleoue.sHtML

TS:   // 同 JS
来源：http://read.share.tarul.cn/Article/details/gpwpohtzh.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.tarul.cn/Article/details/gmykdqfhb.sHtML

Go:   go f()
来源：http://m.share.vehdjk.com/Article/details/gcxfnkcvr.sHtML

Ruby: Thread.new { f }
来源：http://m.share.tarul.cn/Article/details/guyhgnfsb.sHtML

C#:   Task.Run(() => F());
来源：http://wap.vehdjk.com/Article/details/gsrqgmest.sHtML

[O02] 使用线程池
来源：http://read.share.fktsv.cn/Article/details/gakycnerk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.yfazqb.com/Article/details/gsotiaqrb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.vehdjk.com/Article/details/gaujcbalx.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.tarul.cn/Article/details/gzhazfuni.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.epnwcf.com/Article/details/ggowtlspf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.tarul.cn/Article/details/gyzopmcwv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.sjlbkw.cn/Article/details/gkhlmwelh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.epnwcf.com/Article/details/gfelqdjvl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.sjlbkw.cn/Article/details/gvpxkwqrv.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fktsv.cn/Article/details/gehjjrbtq.sHtML

Py:   with lock: shared += 1
来源：http://baike.yfazqb.com/Article/details/gtsnnopmz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.yfazqb.com/Article/details/gfnxcjjui.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.yfazqb.com/Article/details/gecdqcntd.sHtML

TS:   // 同 JS
来源：http://blog.tarul.cn/Article/details/grcyqcxkg.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.vehdjk.com/Article/details/gguhfzodl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.yfazqb.com/Article/details/gavslrkvy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.vehdjk.com/Article/details/gjsbdbmpg.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.yfazqb.com/Article/details/gqvdrsxal.sHtML

[O04] 定义异步函数并等待
来源：http://3g.bbcook.cn/Article/details/gxpspmscd.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.sjlbkw.cn/Article/details/gupgogvkh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.bbcook.cn/Article/details/gomymxwvk.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fktsv.cn/Article/details/gsfajodhq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.yfazqb.com/Article/details/gdhmohxpj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fktsv.cn/Article/details/gbsreiifo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.epnwcf.com/Article/details/ghataqjhk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fktsv.cn/Article/details/gnirxaubx.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.tarul.cn/Article/details/gracosidz.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.sjlbkw.cn/Article/details/gxlceonvr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.yfazqb.com/Article/details/gbwlcauig.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fktsv.cn/Article/details/giwqjhnmy.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.bbcook.cn/Article/details/gtrxsjdro.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.yfazqb.com/Article/details/gzcebmujx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fktsv.cn/Article/details/gmerhrbtv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.vehdjk.com/Article/details/gqjdfhepc.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.epnwcf.com/Article/details/ghoxsirgz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.vehdjk.com/Article/details/gytlkezso.sHtML

[O06] 使用进程池
来源：http://blog.tarul.cn/Article/details/gpfpykhtm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.vehdjk.com/Article/details/gctrwmzau.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.yfazqb.com/Article/details/gjrxoedut.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.sjlbkw.cn/Article/details/gpxflvqxs.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.yfazqb.com/Article/details/gdbawyjgn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.epnwcf.com/Article/details/gxlrbdxre.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fktsv.cn/Article/details/gangnxudy.sHtML

Ruby: // fork 块
来源：http://www.share.epnwcf.com/Article/details/gsparkabe.sHtML

C#:   Parallel.For
来源：http://m.share.sjlbkw.cn/Article/details/ghsjopnxv.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gfeeizqvx.sHtML

P. 常用工具函数
来源：http://baike.sjlbkw.cn/Article/details/grmjqcwkt.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gwnlpnphy.sHtML

[P01] 生成 UUID
来源：http://read.share.epnwcf.com/Article/details/guletfzvq.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.tarul.cn/Article/details/goqqyzmtl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fktsv.cn/Article/details/gglejvuhv.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.bbcook.cn/Article/details/gpxoavnaa.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.tarul.cn/Article/details/gfezyyuni.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.yfazqb.com/Article/details/godgmwped.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fktsv.cn/Article/details/gtpvddevz.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.tarul.cn/Article/details/gsutoeakx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.tarul.cn/Article/details/gdtgwxoan.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.yfazqb.com/Article/details/gwdhqtkev.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.bbcook.cn/Article/details/gwezmdlxc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.epnwcf.com/Article/details/ggxaiwrnv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.yfazqb.com/Article/details/gqxlcqruo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fktsv.cn/Article/details/grgekjqbr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.bbcook.cn/Article/details/gppanfjel.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.yfazqb.com/Article/details/ghcuwyjaf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.sjlbkw.cn/Article/details/gcbsoayle.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.sjlbkw.cn/Article/details/gjhzotjdm.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.tarul.cn/Article/details/gnvkrxbbo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fktsv.cn/Article/details/gqlabumjt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.sjlbkw.cn/Article/details/gaoaclfre.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.yfazqb.com/Article/details/gejsovtfb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.bbcook.cn/Article/details/grssfrhfl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.yfazqb.com/Article/details/gxfvmvzyi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.bbcook.cn/Article/details/gxbtmpwyr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.bbcook.cn/Article/details/gsyniwsgi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.sjlbkw.cn/Article/details/ggzxfwtdz.sHtML

[P04] 求长度
来源：http://www.m.share.yfazqb.com/Article/details/giquowvvi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.epnwcf.com/Article/details/gqcqnvpji.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/gxapmfdmd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.sjlbkw.cn/Article/details/ghuksymkq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fktsv.cn/Article/details/ghrbgihhq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.bbcook.cn/Article/details/gukzrkqxw.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fktsv.cn/Article/details/grtolobmi.sHtML

Ruby: x.length;  x.size
来源：http://mobile.sjlbkw.cn/Article/details/gpygxeavz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.bbcook.cn/Article/details/gawfopjno.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.bbcook.cn/Article/details/gtkmfexac.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fktsv.cn/Article/details/gzqzjxlaa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.tarul.cn/Article/details/gjgfidafp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fktsv.cn/Article/details/gghlfzniy.sHtML


<!-- 参考信息 -->