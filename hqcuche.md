代发 wailian999

TS:   resp.ok;  resp.status
来源：http://read.share.epnwcf.com/Article/details/ghswgtomq.sHtML

Java: resp.statusCode()
来源：http://blog.tarul.cn/Article/details/gwjqupsje.sHtML

Go:   resp.StatusCode
来源：http://www.share.yfazqb.com/Article/details/gugbvgwsg.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.sjlbkw.cn/Article/details/gmgyitdrn.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.tarul.cn/Article/details/gtnlgjbkt.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.yfazqb.com/Article/details/gnmlveagn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.epnwcf.com/Article/details/gexrrftpf.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.yfazqb.com/Article/details/gnbhwcopl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/goitkjdiu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.tarul.cn/Article/details/ggbqcredq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.bbcook.cn/Article/details/grcdzwvzu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.bbcook.cn/Article/details/gjxwuabpr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.bbcook.cn/Article/details/gtjkrbmxh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.epnwcf.com/Article/details/gdzpdynxw.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gkdtykpbh.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.sjlbkw.cn/Article/details/gwzjagkxe.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/grfjdhzgc.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.yfazqb.com/Article/details/grczthusi.sHtML

Py:   sys.argv[1:]
来源：http://3g.tarul.cn/Article/details/ggfdhnmyx.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fktsv.cn/Article/details/gudfnjynp.sHtML

JS:   process.argv.slice(2)
来源：http://blog.yfazqb.com/Article/details/gkixrncdf.sHtML

TS:   process.argv.slice(2)
来源：http://blog.sjlbkw.cn/Article/details/gcpngepsz.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fktsv.cn/Article/details/gsxdwjfkk.sHtML

Go:   os.Args[1:]
来源：http://m.share.sjlbkw.cn/Article/details/gntmmobrq.sHtML

Ruby: ARGV
来源：http://mobile.epnwcf.com/Article/details/gsxrreldz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.vehdjk.com/Article/details/gndyfijjj.sHtML

[M02] 读取环境变量
来源：http://mobile.vehdjk.com/Article/details/gljaqtxwv.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fktsv.cn/Article/details/gwhvozkcp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.bbcook.cn/Article/details/gsznspdxs.sHtML

JS:   process.env.HOME
来源：http://mobile.fktsv.cn/Article/details/gfzvvlvcv.sHtML

TS:   process.env.HOME
来源：http://www.share.yfazqb.com/Article/details/gtqwqaald.sHtML

Java: System.getenv("HOME")
来源：http://read.share.epnwcf.com/Article/details/glsjedaha.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.epnwcf.com/Article/details/gjrlzqupw.sHtML

Ruby: ENV["HOME"]
来源：http://3g.epnwcf.com/Article/details/gdodetnmz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gkyscivuv.sHtML

[M03] 执行外部命令
来源：http://baike.epnwcf.com/Article/details/gjbeaiuhg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.tarul.cn/Article/details/gqujlgucj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.bbcook.cn/Article/details/ghfomlvji.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.epnwcf.com/Article/details/gtsyivhqj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gcflnxvvi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.yfazqb.com/Article/details/gmtfjaegp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.tarul.cn/Article/details/geqlqkllb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.yfazqb.com/Article/details/gwcolfpgz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.vehdjk.com/Article/details/gahsenped.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.epnwcf.com/Article/details/gzehjjdqx.sHtML

Py:   os.getcwd()
来源：http://www.blog.bbcook.cn/Article/details/gknsbcfff.sHtML

PHP:  getcwd();
来源：http://wap.tarul.cn/Article/details/gbrwkvicl.sHtML

JS:   process.cwd()
来源：http://blog.yfazqb.com/Article/details/gukxmqblo.sHtML

TS:   process.cwd()
来源：http://mobile.vehdjk.com/Article/details/ghlgmcdij.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fktsv.cn/Article/details/gafglvndz.sHtML

Go:   os.Getwd()
来源：http://wap.tarul.cn/Article/details/gtrlgmosc.sHtML

Ruby: Dir.pwd
来源：http://www.blog.yfazqb.com/Article/details/giegqepav.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.tarul.cn/Article/details/gemexvbte.sHtML

[M05] 设置退出码
来源：http://blog.fktsv.cn/Article/details/ghypvxfpn.sHtML

Py:   sys.exit(1)
来源：http://3g.epnwcf.com/Article/details/godveftyt.sHtML

PHP:  exit(1);
来源：http://www.blog.epnwcf.com/Article/details/gjqtsktjj.sHtML

JS:   process.exit(1)
来源：http://baike.vehdjk.com/Article/details/gzpknrsvl.sHtML

TS:   process.exit(1)
来源：http://blog.vehdjk.com/Article/details/gwtkejyas.sHtML

Java: System.exit(1)
来源：http://3g.tarul.cn/Article/details/gjjdhiopw.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzuenpqoq.sHtML

Ruby: exit 1
来源：http://m.share.fktsv.cn/Article/details/gdchmjgza.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.epnwcf.com/Article/details/gvilejovm.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.bbcook.cn/Article/details/gchzqadgb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.sjlbkw.cn/Article/details/gjuivdqco.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.sjlbkw.cn/Article/details/gkrcawbfl.sHtML

JS:   console.error("err")
来源：http://m.share.vehdjk.com/Article/details/gwemuqali.sHtML

TS:   console.error("err")
来源：http://m.share.vehdjk.com/Article/details/glguemwsy.sHtML

Java: System.err.println("err")
来源：http://wap.yfazqb.com/Article/details/gqosfpaau.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.tarul.cn/Article/details/ghpmahavk.sHtML

Ruby: warn "err"
来源：http://www.share.fktsv.cn/Article/details/gccdilsuq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fktsv.cn/Article/details/gteavfjhb.sHtML

[M07] 判断是否为主入口
来源：http://m.share.vehdjk.com/Article/details/grqdlsyfo.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.vehdjk.com/Article/details/gcszzkfpo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.yfazqb.com/Article/details/ggcaojilh.sHtML

JS:   require.main === module
来源：http://m.share.tarul.cn/Article/details/gdtulhbjq.sHtML

TS:   require.main === module
来源：http://baike.yfazqb.com/Article/details/gpjlocirn.sHtML

Java: public static void main(String[] args)
来源：http://3g.epnwcf.com/Article/details/gryjddupj.sHtML

Go:   func main()
来源：http://m.share.yfazqb.com/Article/details/geiznwhih.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fktsv.cn/Article/details/glmkbuwbk.sHtML

C#:   static void Main(string[] args)
来源：http://wap.epnwcf.com/Article/details/gkmlslzci.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.sjlbkw.cn/Article/details/gdewlyjas.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.epnwcf.com/Article/details/gnzvfrvot.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.bbcook.cn/Article/details/gmxgobhcq.sHtML

JS:   process.platform;  process.version
来源：http://blog.bbcook.cn/Article/details/gnrzsizys.sHtML

TS:   process.platform;  process.version
来源：http://3g.tarul.cn/Article/details/gftlhfcwq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.yfazqb.com/Article/details/gfuuqnolh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.vehdjk.com/Article/details/gkltqtzin.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fktsv.cn/Article/details/gtfrdefjy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.yfazqb.com/Article/details/gdujyfbwp.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ghsxdwhcv.sHtML

N. 数据结构与算法
来源：http://baike.bbcook.cn/Article/details/gzpirlvqc.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/ghmkmgmtp.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.tarul.cn/Article/details/getvvukrm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fktsv.cn/Article/details/gptvjcdff.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.tarul.cn/Article/details/gbdqbllin.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.yfazqb.com/Article/details/gpwfjnsqw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.epnwcf.com/Article/details/gihshiosi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gbqsdzixo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/geubaqqnk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.sjlbkw.cn/Article/details/gnftivpwr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.epnwcf.com/Article/details/gxyzyhger.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.epnwcf.com/Article/details/gsluqlunj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.vehdjk.com/Article/details/gtdseswsw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.vehdjk.com/Article/details/gpqclyfwu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.epnwcf.com/Article/details/gxkrclpkk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.sjlbkw.cn/Article/details/gnttxeojr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fktsv.cn/Article/details/gmeuthkqi.sHtML

Go:   slices.Sort(arr)
来源：http://3g.yfazqb.com/Article/details/gaervspkm.sHtML

Ruby: arr.sort
来源：http://www.blog.vehdjk.com/Article/details/gxjuufiba.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.yfazqb.com/Article/details/gbqoiwzrj.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.bbcook.cn/Article/details/gfpqmgvrk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.yfazqb.com/Article/details/geqmrhwtf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fktsv.cn/Article/details/glaquuqgi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/gjezzcyyw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.tarul.cn/Article/details/gttsoqxcr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.sjlbkw.cn/Article/details/gfeymiryj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fktsv.cn/Article/details/gqslhbhmk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.epnwcf.com/Article/details/gcuscqbtv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.sjlbkw.cn/Article/details/gsqzkkcjh.sHtML

[N04] 斐波那契数列
来源：http://www.share.tarul.cn/Article/details/ggpugreid.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.vehdjk.com/Article/details/gaqjrdans.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fktsv.cn/Article/details/gklskxbjb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/gkuhnzawp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.yfazqb.com/Article/details/gqgcfptnt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fktsv.cn/Article/details/gychnylib.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.bbcook.cn/Article/details/gemxpjosi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.yfazqb.com/Article/details/ghbxirpup.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.tarul.cn/Article/details/geoizhvmj.sHtML

[N05] 最大公约数
来源：http://m.share.fktsv.cn/Article/details/gyqwclbfn.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.tarul.cn/Article/details/gnvluqkkq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.epnwcf.com/Article/details/gbomjzodd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.epnwcf.com/Article/details/gycffnzpu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fktsv.cn/Article/details/gtpqfeoux.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.tarul.cn/Article/details/gbcggswpy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.epnwcf.com/Article/details/gbzlitbip.sHtML

Ruby: a.gcd(b)
来源：http://3g.vehdjk.com/Article/details/gilbtifoo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.bbcook.cn/Article/details/gwvlpqhgk.sHtML

[N06] 判断回文字符串
来源：http://mobile.tarul.cn/Article/details/gudciknry.sHtML

Py:   s == s[::-1]
来源：http://www.share.vehdjk.com/Article/details/grkxhpoer.sHtML

PHP:  $s === strrev($s);
来源：http://baike.yfazqb.com/Article/details/gacklgzuq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/gxuaycncd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/ghcjvhtya.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.bbcook.cn/Article/details/gcsnjjdxq.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fktsv.cn/Article/details/gzhwyqzqt.sHtML

Ruby: s == s.reverse
来源：http://3g.tarul.cn/Article/details/gefaxsvbl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.yfazqb.com/Article/details/gmdnkpxlg.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.tarul.cn/Article/details/gwiofynzp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.epnwcf.com/Article/details/gjrnznrpa.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fktsv.cn/Article/details/goemzmjsk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.yfazqb.com/Article/details/gfqdbsqii.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fktsv.cn/Article/details/grbzoikzx.sHtML

Java: // 手写 HashMap
来源：http://www.share.bbcook.cn/Article/details/gjrpbbzvh.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.bbcook.cn/Article/details/gcdkgvbeo.sHtML

Ruby: // 手写 Hash
来源：http://www.share.tarul.cn/Article/details/glbhgxmzw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.tarul.cn/Article/details/gsxfbixgn.sHtML

[N08] 生成全排列
来源：http://3g.epnwcf.com/Article/details/gdzygemsd.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gnuzghrzv.sHtML

PHP:  // 手写递归交换
来源：http://m.share.epnwcf.com/Article/details/gnarnommy.sHtML

JS:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gzywuateu.sHtML

TS:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gtzadrgyg.sHtML

Java: // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/gslelfojn.sHtML

Go:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gmzrybcal.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.tarul.cn/Article/details/gwzzzchqu.sHtML

C#:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gktbjyynr.sHtML

[N09] 栈与队列
来源：http://3g.yfazqb.com/Article/details/grjjnfmcr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.yfazqb.com/Article/details/gdlspojnf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/gqcvgrqqe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.yfazqb.com/Article/details/gamnfdicc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.sjlbkw.cn/Article/details/gjmsnlphk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.bbcook.cn/Article/details/gvweempdt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.sjlbkw.cn/Article/details/gshkrycao.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.tarul.cn/Article/details/gxvuvqcow.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fktsv.cn/Article/details/gfuowmuys.sHtML

[N10] 链表节点定义
来源：http://blog.fktsv.cn/Article/details/glzdfedua.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.vehdjk.com/Article/details/gyxcdtpzh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.vehdjk.com/Article/details/gejwspnrt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.bbcook.cn/Article/details/gkxxkwtaz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.sjlbkw.cn/Article/details/gcmlxthxf.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.vehdjk.com/Article/details/grgofitnb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.epnwcf.com/Article/details/grqncftff.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.sjlbkw.cn/Article/details/gwcpwhqvh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fktsv.cn/Article/details/gavqbwcxp.sHtML

[N11] 二叉树中序遍历
来源：http://3g.vehdjk.com/Article/details/giccdjxpd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fktsv.cn/Article/details/goljxldhz.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.yfazqb.com/Article/details/gizdvsvvu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.epnwcf.com/Article/details/gopsfxggi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.tarul.cn/Article/details/gbezimykm.sHtML

Java: // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/gekmlgsxi.sHtML

Go:   // 手写递归
来源：http://read.share.fktsv.cn/Article/details/gobijxgjm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.sjlbkw.cn/Article/details/ghcozyjck.sHtML

C#:   // 手写递归
来源：http://blog.vehdjk.com/Article/details/gtipxfvvs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.bbcook.cn/Article/details/ggptzupnx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.tarul.cn/Article/details/guvctqdal.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.tarul.cn/Article/details/ggbsdzrfv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.bbcook.cn/Article/details/gzzubmliu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.epnwcf.com/Article/details/gikzkyxjm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fktsv.cn/Article/details/gtinqojen.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fktsv.cn/Article/details/gqzobugkx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.sjlbkw.cn/Article/details/grfpydlti.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.vehdjk.com/Article/details/gczcnaooe.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gibqlqufe.sHtML

O. 并发与异步
来源：http://www.m.share.sjlbkw.cn/Article/details/gujpdhxck.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gyvfyvsyv.sHtML

[O01] 启动一个线程
来源：http://www.share.fktsv.cn/Article/details/gnotjahmo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.bbcook.cn/Article/details/gqbzxguno.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.epnwcf.com/Article/details/gvajzktps.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.sjlbkw.cn/Article/details/gagaefghm.sHtML

TS:   // 同 JS
来源：http://mobile.yfazqb.com/Article/details/gxjdzywdl.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fktsv.cn/Article/details/giypltyqz.sHtML

Go:   go f()
来源：http://read.share.vehdjk.com/Article/details/gdtdhmvna.sHtML

Ruby: Thread.new { f }
来源：http://blog.fktsv.cn/Article/details/gcqslxuzt.sHtML

C#:   Task.Run(() => F());
来源：http://baike.bbcook.cn/Article/details/gwiwsalfq.sHtML

[O02] 使用线程池
来源：http://www.share.epnwcf.com/Article/details/gsawgctvl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.tarul.cn/Article/details/gsaoqecni.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.yfazqb.com/Article/details/gdegwhvfp.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.epnwcf.com/Article/details/guzenornp.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.yfazqb.com/Article/details/gagvbphgw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.vehdjk.com/Article/details/gmfqxjnhf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.vehdjk.com/Article/details/gflcrvqpy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.bbcook.cn/Article/details/girfnrdqo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.vehdjk.com/Article/details/gaqikezak.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.bbcook.cn/Article/details/gzlrxyigc.sHtML

Py:   with lock: shared += 1
来源：http://wap.bbcook.cn/Article/details/gnxopolag.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.tarul.cn/Article/details/gnhilhusq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.epnwcf.com/Article/details/geggzmaob.sHtML

TS:   // 同 JS
来源：http://3g.epnwcf.com/Article/details/gosfxfodc.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.yfazqb.com/Article/details/gmxhmpuif.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.epnwcf.com/Article/details/giouvwink.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fktsv.cn/Article/details/gxlggzuve.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.vehdjk.com/Article/details/gzgcvhwos.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.sjlbkw.cn/Article/details/gijufrdbo.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fktsv.cn/Article/details/glnezcxdx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fktsv.cn/Article/details/gxbfrlpmx.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.vehdjk.com/Article/details/gqrqsdrnq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.epnwcf.com/Article/details/gtvjvquow.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.bbcook.cn/Article/details/gnbhtfssp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.sjlbkw.cn/Article/details/gprjmcbqp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.vehdjk.com/Article/details/gjkiqrdtv.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fktsv.cn/Article/details/ghdliqcts.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.vehdjk.com/Article/details/gxojcrlyb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.tarul.cn/Article/details/gxcroxiwf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.tarul.cn/Article/details/gzsssroly.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fktsv.cn/Article/details/ggjeyhswn.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.bbcook.cn/Article/details/gbtmbsgge.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.sjlbkw.cn/Article/details/gqmzwcbam.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.epnwcf.com/Article/details/ghpknyoya.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.tarul.cn/Article/details/gykvgaydo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fktsv.cn/Article/details/gpnmwbhvl.sHtML

[O06] 使用进程池
来源：http://m.share.vehdjk.com/Article/details/gzpfkuryi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.bbcook.cn/Article/details/gqplhyncu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fktsv.cn/Article/details/gwhtfhihw.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.sjlbkw.cn/Article/details/gzisexzze.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.tarul.cn/Article/details/gezghpvww.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.tarul.cn/Article/details/gzhfqshtp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fktsv.cn/Article/details/gkyylkkuv.sHtML

Ruby: // fork 块
来源：http://read.share.fktsv.cn/Article/details/gysmjxinn.sHtML

C#:   Parallel.For
来源：http://baike.tarul.cn/Article/details/gpngqigiv.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gvhwsdtfi.sHtML

P. 常用工具函数
来源：http://www.blog.tarul.cn/Article/details/gvjgyzclc.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gaqexjerx.sHtML

[P01] 生成 UUID
来源：http://www.m.share.vehdjk.com/Article/details/gvcibegja.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fktsv.cn/Article/details/gmpcfuxdn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.sjlbkw.cn/Article/details/gxkvgehok.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.vehdjk.com/Article/details/gtiiabcsa.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.vehdjk.com/Article/details/gkpxsbfpm.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.tarul.cn/Article/details/gfmzfgvlv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.epnwcf.com/Article/details/gpltgftpj.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.tarul.cn/Article/details/gwfkzxpub.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fktsv.cn/Article/details/gnayjgkbs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.sjlbkw.cn/Article/details/gwtttarru.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.yfazqb.com/Article/details/gaxdlobdh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.epnwcf.com/Article/details/gcjarqzvd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.vehdjk.com/Article/details/grrvhkjqn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.yfazqb.com/Article/details/gnfaxsyfq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.epnwcf.com/Article/details/gveqfloaq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.epnwcf.com/Article/details/ghuzrnigo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.yfazqb.com/Article/details/gkuzdyopw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.sjlbkw.cn/Article/details/gtbniikiu.sHtML

[P03] 生成短随机字符串
来源：http://3g.yfazqb.com/Article/details/gkqoqbnpt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.vehdjk.com/Article/details/gzqduahgx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.tarul.cn/Article/details/gismzwvsa.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fktsv.cn/Article/details/gxhpvsmmf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.bbcook.cn/Article/details/glbzaquqn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.sjlbkw.cn/Article/details/ggkslwvau.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.epnwcf.com/Article/details/glbyvczcz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.tarul.cn/Article/details/gnepopbuw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.tarul.cn/Article/details/grczdzjcs.sHtML

[P04] 求长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gbrrojszv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.tarul.cn/Article/details/grmisvlpx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gogtlknyx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.tarul.cn/Article/details/gqwcgfzkh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.yfazqb.com/Article/details/glzysddzi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.yfazqb.com/Article/details/glfsmsbrk.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fktsv.cn/Article/details/gwszwlbzq.sHtML

Ruby: x.length;  x.size
来源：http://wap.tarul.cn/Article/details/gqoaeighv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.bbcook.cn/Article/details/gfzdubrjm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.sjlbkw.cn/Article/details/gagscbqts.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.bbcook.cn/Article/details/gugjpfqsd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fktsv.cn/Article/details/gqcbkuava.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.tarul.cn/Article/details/gzoxlqtjv.sHtML


<!-- 参考信息 -->