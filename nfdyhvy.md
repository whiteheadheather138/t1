代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://m.share.sjlbkw.cn/Article/details/guygompyw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.yfazqb.com/Article/details/gwacyculx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.vehdjk.com/Article/details/geipxxjyy.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.sjlbkw.cn/Article/details/gxlnkgscp.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.yfazqb.com/Article/details/gizpucqqo.sHtML

Java: resp.statusCode()
来源：http://www.blog.bbcook.cn/Article/details/gfachvcqd.sHtML

Go:   resp.StatusCode
来源：http://mobile.vehdjk.com/Article/details/gynmieisj.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.tarul.cn/Article/details/gfpvpwhsk.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.epnwcf.com/Article/details/gjxizjeue.sHtML

[L08] 并发请求多个地址
来源：http://mobile.tarul.cn/Article/details/giwoewwda.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.bbcook.cn/Article/details/gvukhdwhv.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.tarul.cn/Article/details/gfqwxwabi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fktsv.cn/Article/details/gjtaujtbs.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.sjlbkw.cn/Article/details/glfrervmm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.tarul.cn/Article/details/gmpqgzwbx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.bbcook.cn/Article/details/gyaigwhgk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.sjlbkw.cn/Article/details/gofgbfyms.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.sjlbkw.cn/Article/details/gazfsarmu.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gajwcpzks.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.tarul.cn/Article/details/gjtofbnut.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gsspwmnsc.sHtML

[M01] 读取命令行参数
来源：http://www.share.epnwcf.com/Article/details/glvltwfid.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.epnwcf.com/Article/details/ghrzpktfm.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.yfazqb.com/Article/details/gttudtleb.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.yfazqb.com/Article/details/gcnolmhpk.sHtML

TS:   process.argv.slice(2)
来源：http://blog.bbcook.cn/Article/details/gwoldjxem.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.sjlbkw.cn/Article/details/gcnjrvspo.sHtML

Go:   os.Args[1:]
来源：http://read.share.sjlbkw.cn/Article/details/guhetpiev.sHtML

Ruby: ARGV
来源：http://www.m.share.vehdjk.com/Article/details/ghiwbsvwz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.epnwcf.com/Article/details/gbtzqmwua.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fktsv.cn/Article/details/gvzufraac.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.yfazqb.com/Article/details/gzlcprtoi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.yfazqb.com/Article/details/gykcuzrje.sHtML

JS:   process.env.HOME
来源：http://mobile.sjlbkw.cn/Article/details/guzutvrme.sHtML

TS:   process.env.HOME
来源：http://baike.yfazqb.com/Article/details/gmhdxzhcz.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gjxzlodhg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fktsv.cn/Article/details/gtvpurubu.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.vehdjk.com/Article/details/gnhwobqoo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.yfazqb.com/Article/details/ggykljnoh.sHtML

[M03] 执行外部命令
来源：http://www.share.fktsv.cn/Article/details/gbuqhiozh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gwdsxicjj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.vehdjk.com/Article/details/ggpxfmoag.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.yfazqb.com/Article/details/gnvrnfosf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.bbcook.cn/Article/details/glnwfylyl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.sjlbkw.cn/Article/details/ghwuqduzq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.sjlbkw.cn/Article/details/gtmnlhpzg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.bbcook.cn/Article/details/gaznctiln.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.yfazqb.com/Article/details/gcqjibncm.sHtML

[M04] 获取当前工作目录
来源：http://baike.epnwcf.com/Article/details/gyffxuiho.sHtML

Py:   os.getcwd()
来源：http://wap.tarul.cn/Article/details/gsadhqcjd.sHtML

PHP:  getcwd();
来源：http://m.share.sjlbkw.cn/Article/details/gxxqpljlj.sHtML

JS:   process.cwd()
来源：http://www.m.share.vehdjk.com/Article/details/gsbpkfdkx.sHtML

TS:   process.cwd()
来源：http://wap.tarul.cn/Article/details/gebxnkgtv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.sjlbkw.cn/Article/details/grorqmxmm.sHtML

Go:   os.Getwd()
来源：http://wap.sjlbkw.cn/Article/details/ghjhgvyks.sHtML

Ruby: Dir.pwd
来源：http://wap.yfazqb.com/Article/details/gscsqhimt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.epnwcf.com/Article/details/ghzocuotd.sHtML

[M05] 设置退出码
来源：http://m.share.fktsv.cn/Article/details/gxqsxjacw.sHtML

Py:   sys.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/glhuksoru.sHtML

PHP:  exit(1);
来源：http://mobile.yfazqb.com/Article/details/gfjuqnfvz.sHtML

JS:   process.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gqciuonnx.sHtML

TS:   process.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gicvllikt.sHtML

Java: System.exit(1)
来源：http://3g.bbcook.cn/Article/details/gilcrrmgy.sHtML

Go:   os.Exit(1)
来源：http://3g.tarul.cn/Article/details/gbmvvolzs.sHtML

Ruby: exit 1
来源：http://wap.vehdjk.com/Article/details/gqrlvhgdp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.epnwcf.com/Article/details/gxgwpivfn.sHtML

[M06] 向标准错误输出
来源：http://www.share.bbcook.cn/Article/details/ginehkuxf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.vehdjk.com/Article/details/golbriyav.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.vehdjk.com/Article/details/gadfahfjl.sHtML

JS:   console.error("err")
来源：http://read.share.sjlbkw.cn/Article/details/gphahtecv.sHtML

TS:   console.error("err")
来源：http://3g.bbcook.cn/Article/details/gnplkppgq.sHtML

Java: System.err.println("err")
来源：http://mobile.sjlbkw.cn/Article/details/gdnrvzltc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.tarul.cn/Article/details/gmdzwegol.sHtML

Ruby: warn "err"
来源：http://www.m.share.epnwcf.com/Article/details/gbyqchnmt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.epnwcf.com/Article/details/glzbqkund.sHtML

[M07] 判断是否为主入口
来源：http://www.share.vehdjk.com/Article/details/gylcwezkz.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.epnwcf.com/Article/details/gjjbaivzs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.sjlbkw.cn/Article/details/gmkpzdgfu.sHtML

JS:   require.main === module
来源：http://read.share.epnwcf.com/Article/details/geodchihq.sHtML

TS:   require.main === module
来源：http://mobile.bbcook.cn/Article/details/gutyfbvej.sHtML

Java: public static void main(String[] args)
来源：http://baike.yfazqb.com/Article/details/gyeuwpnbb.sHtML

Go:   func main()
来源：http://www.blog.epnwcf.com/Article/details/glthmavjv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.tarul.cn/Article/details/gjgqulojx.sHtML

C#:   static void Main(string[] args)
来源：http://wap.vehdjk.com/Article/details/gkugionzt.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.tarul.cn/Article/details/gotogjrjw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.bbcook.cn/Article/details/ghbulwlxd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.bbcook.cn/Article/details/gveovmazz.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.tarul.cn/Article/details/gxyagnnhw.sHtML

TS:   process.platform;  process.version
来源：http://blog.epnwcf.com/Article/details/gdqbcnfmz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fktsv.cn/Article/details/gmmxrptoi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.bbcook.cn/Article/details/guytjhwhu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.epnwcf.com/Article/details/gbvbowqwl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.sjlbkw.cn/Article/details/gtyoafhir.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gyceggfoq.sHtML

N. 数据结构与算法
来源：http://mobile.epnwcf.com/Article/details/ghvjgufym.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gdokgmwyw.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.bbcook.cn/Article/details/glcxyoont.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gnbnuknxy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.yfazqb.com/Article/details/gzeplwktx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.vehdjk.com/Article/details/gohjylpbz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.vehdjk.com/Article/details/gelbmhzgr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.vehdjk.com/Article/details/gflrknlgg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.vehdjk.com/Article/details/gvebfbryg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fktsv.cn/Article/details/grryuwstw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/grecydqvx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.tarul.cn/Article/details/gmhfzdneq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.bbcook.cn/Article/details/gauubmofi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.tarul.cn/Article/details/gzqxcpohx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.yfazqb.com/Article/details/gueykielr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.epnwcf.com/Article/details/ggljyayuv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fktsv.cn/Article/details/gbkbirems.sHtML

Go:   slices.Sort(arr)
来源：http://3g.vehdjk.com/Article/details/gvqhjnwve.sHtML

Ruby: arr.sort
来源：http://m.share.fktsv.cn/Article/details/gbagxnoey.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.vehdjk.com/Article/details/gwqykisrd.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fktsv.cn/Article/details/gqoldvxhu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fktsv.cn/Article/details/gpkfeucxy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.tarul.cn/Article/details/guiebrleb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.yfazqb.com/Article/details/glardujvi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.bbcook.cn/Article/details/gvskjqyvl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.yfazqb.com/Article/details/ggymvaqvo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.epnwcf.com/Article/details/gozcvadqo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.sjlbkw.cn/Article/details/gclqabmgk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.yfazqb.com/Article/details/gfqyqaags.sHtML

[N04] 斐波那契数列
来源：http://3g.sjlbkw.cn/Article/details/gfxjroial.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.epnwcf.com/Article/details/gyydhbhqg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.bbcook.cn/Article/details/glocizlgq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.bbcook.cn/Article/details/guhgjzbao.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gxgcqvndy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.sjlbkw.cn/Article/details/gtfskxqon.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fktsv.cn/Article/details/gclpyubni.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.tarul.cn/Article/details/ghawhioqa.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fktsv.cn/Article/details/gqqspgqmd.sHtML

[N05] 最大公约数
来源：http://mobile.yfazqb.com/Article/details/gdhfilsmg.sHtML

Py:   math.gcd(a, b)
来源：http://wap.sjlbkw.cn/Article/details/gnszvzoim.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.sjlbkw.cn/Article/details/goerpnnny.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fktsv.cn/Article/details/ggxlhossb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.vehdjk.com/Article/details/gcnvgatji.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fktsv.cn/Article/details/gfbncmydl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.yfazqb.com/Article/details/gaflcmpiy.sHtML

Ruby: a.gcd(b)
来源：http://m.share.yfazqb.com/Article/details/gfrsfxpis.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.tarul.cn/Article/details/gfiuhrmef.sHtML

[N06] 判断回文字符串
来源：http://read.share.yfazqb.com/Article/details/gyljrjgsw.sHtML

Py:   s == s[::-1]
来源：http://www.share.vehdjk.com/Article/details/ghqxaurss.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.bbcook.cn/Article/details/ggprljbxl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/gjpqmrvzb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/gqbmughhd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.yfazqb.com/Article/details/gnditkiop.sHtML

Go:   // 双指针从两端比较
来源：http://baike.epnwcf.com/Article/details/gfqjdrdpo.sHtML

Ruby: s == s.reverse
来源：http://baike.yfazqb.com/Article/details/gaspdngfc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.vehdjk.com/Article/details/gcvobgnjz.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.yfazqb.com/Article/details/gkzyktceb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.yfazqb.com/Article/details/geqainhxu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.sjlbkw.cn/Article/details/ggnjmxlbl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.vehdjk.com/Article/details/gtbzxfovv.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fktsv.cn/Article/details/gyohaujmh.sHtML

Java: // 手写 HashMap
来源：http://baike.vehdjk.com/Article/details/gkmunkziy.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fktsv.cn/Article/details/gbnaolscr.sHtML

Ruby: // 手写 Hash
来源：http://3g.fktsv.cn/Article/details/gfqkxjedg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.sjlbkw.cn/Article/details/gszpcttze.sHtML

[N08] 生成全排列
来源：http://www.blog.yfazqb.com/Article/details/gxesthjvx.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.epnwcf.com/Article/details/gcxypoyns.sHtML

PHP:  // 手写递归交换
来源：http://blog.vehdjk.com/Article/details/gdcxdgbiw.sHtML

JS:   // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/gusftamom.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/goahvhzcx.sHtML

Java: // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gkbqxjcxd.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gikwrrquq.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.yfazqb.com/Article/details/gppunspzi.sHtML

C#:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gwihdoqes.sHtML

[N09] 栈与队列
来源：http://m.share.sjlbkw.cn/Article/details/gfdakoahp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.sjlbkw.cn/Article/details/ghmjmuorp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.yfazqb.com/Article/details/gbbgtxsjx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.vehdjk.com/Article/details/guzjtjsqp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.yfazqb.com/Article/details/gfbpqkwoj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.epnwcf.com/Article/details/gtypkliuh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fktsv.cn/Article/details/gkysvjsge.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/gwcfgynjk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.sjlbkw.cn/Article/details/gegnqdfwu.sHtML

[N10] 链表节点定义
来源：http://baike.yfazqb.com/Article/details/glntahpxa.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fktsv.cn/Article/details/gjztvquze.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.yfazqb.com/Article/details/gvtfxpwjf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.epnwcf.com/Article/details/gaqzciaxl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fktsv.cn/Article/details/guqoatiks.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.vehdjk.com/Article/details/gjywwljto.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fktsv.cn/Article/details/gimwbksga.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.yfazqb.com/Article/details/gxhuzrlet.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.bbcook.cn/Article/details/gvpsntobk.sHtML

[N11] 二叉树中序遍历
来源：http://wap.sjlbkw.cn/Article/details/gfjvyvdhl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.sjlbkw.cn/Article/details/gdqedsvdv.sHtML

PHP:  // 手写递归函数
来源：http://3g.sjlbkw.cn/Article/details/gdhzaizsi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.tarul.cn/Article/details/gojynmolp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.yfazqb.com/Article/details/gsrhmuryt.sHtML

Java: // 手写递归
来源：http://wap.sjlbkw.cn/Article/details/govnwfegz.sHtML

Go:   // 手写递归
来源：http://blog.fktsv.cn/Article/details/gfcziqwuw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.bbcook.cn/Article/details/gcnhpxzut.sHtML

C#:   // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/gfknxqhcd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.vehdjk.com/Article/details/gzzrpipxn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.vehdjk.com/Article/details/gffoivndp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.epnwcf.com/Article/details/gqctzbcpq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.bbcook.cn/Article/details/gktzhsyap.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.bbcook.cn/Article/details/gkxktydph.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.tarul.cn/Article/details/gsetfvvjy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.yfazqb.com/Article/details/gffvwscrj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.vehdjk.com/Article/details/ggdcjneoi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.vehdjk.com/Article/details/gatubwbgl.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gucwefgqq.sHtML

O. 并发与异步
来源：http://www.share.epnwcf.com/Article/details/gkrtzaspz.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gptnvjcce.sHtML

[O01] 启动一个线程
来源：http://www.blog.sjlbkw.cn/Article/details/gdnajvfrf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fktsv.cn/Article/details/ggrakeqnv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fktsv.cn/Article/details/gjehnwhee.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.epnwcf.com/Article/details/gsepanrcf.sHtML

TS:   // 同 JS
来源：http://m.share.vehdjk.com/Article/details/ghufhsjsr.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fktsv.cn/Article/details/grdujnoki.sHtML

Go:   go f()
来源：http://baike.epnwcf.com/Article/details/gryihqtfu.sHtML

Ruby: Thread.new { f }
来源：http://baike.fktsv.cn/Article/details/gkqldcuki.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fktsv.cn/Article/details/gstwedjsg.sHtML

[O02] 使用线程池
来源：http://baike.tarul.cn/Article/details/gjkpuxlya.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.sjlbkw.cn/Article/details/gnyxiiycb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.sjlbkw.cn/Article/details/gqjdgpsaj.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fktsv.cn/Article/details/gdzawezsq.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.bbcook.cn/Article/details/gsiwirypk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.bbcook.cn/Article/details/glhntdcrm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.bbcook.cn/Article/details/goadlnzpm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.epnwcf.com/Article/details/gzwrmsfnj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.bbcook.cn/Article/details/gpgljvcyo.sHtML

[O03] 加锁保护共享数据
来源：http://blog.vehdjk.com/Article/details/gqlxsystg.sHtML

Py:   with lock: shared += 1
来源：http://baike.epnwcf.com/Article/details/gkghwqvcf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.tarul.cn/Article/details/gpguxeshx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.tarul.cn/Article/details/gthmqzidt.sHtML

TS:   // 同 JS
来源：http://www.m.share.fktsv.cn/Article/details/gmsapwwsp.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fktsv.cn/Article/details/gtumikvld.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.yfazqb.com/Article/details/gxkbiocra.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fktsv.cn/Article/details/gvsummzwh.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.tarul.cn/Article/details/gpklzacou.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.vehdjk.com/Article/details/gpsbqgdqb.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fktsv.cn/Article/details/gwgjurjon.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.vehdjk.com/Article/details/gzixroikl.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.bbcook.cn/Article/details/gqjusdayv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.vehdjk.com/Article/details/gtncqfuep.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.bbcook.cn/Article/details/geohodcsi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.epnwcf.com/Article/details/ghfmzyysq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.vehdjk.com/Article/details/gnkebhiqk.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.tarul.cn/Article/details/gmuavmhpt.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.tarul.cn/Article/details/ggxkhrfty.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.epnwcf.com/Article/details/gjcyuynxv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fktsv.cn/Article/details/gjczvkimx.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fktsv.cn/Article/details/ghqmxxhxe.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.sjlbkw.cn/Article/details/gqslfmbfh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.bbcook.cn/Article/details/guqioyxln.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.sjlbkw.cn/Article/details/guncvdznj.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.bbcook.cn/Article/details/gupzbcelf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.tarul.cn/Article/details/gipbfsciw.sHtML

[O06] 使用进程池
来源：http://3g.fktsv.cn/Article/details/gssvautzu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.yfazqb.com/Article/details/glshgdboj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fktsv.cn/Article/details/geyjeugwi.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.vehdjk.com/Article/details/gjrxwmiof.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fktsv.cn/Article/details/gzdgdwomf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fktsv.cn/Article/details/gcaiddphg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.sjlbkw.cn/Article/details/gettqjpeq.sHtML

Ruby: // fork 块
来源：http://blog.sjlbkw.cn/Article/details/gicncdhxc.sHtML

C#:   Parallel.For
来源：http://www.share.epnwcf.com/Article/details/gykbroqks.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gulbeofte.sHtML

P. 常用工具函数
来源：http://wap.bbcook.cn/Article/details/gduchkhcf.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gmrvptnau.sHtML

[P01] 生成 UUID
来源：http://wap.bbcook.cn/Article/details/gerhcodwa.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.bbcook.cn/Article/details/gyeukyvxr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.sjlbkw.cn/Article/details/gbdmrjbvk.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.vehdjk.com/Article/details/gahkpxbsa.sHtML

TS:   crypto.randomUUID()
来源：http://baike.sjlbkw.cn/Article/details/gpwmusiiu.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fktsv.cn/Article/details/gvzldyttp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.sjlbkw.cn/Article/details/gpzkcnjmm.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.vehdjk.com/Article/details/gdghlocdw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.yfazqb.com/Article/details/gahhthize.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.epnwcf.com/Article/details/gygepjggs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fktsv.cn/Article/details/gdgafwxpd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.tarul.cn/Article/details/gtnrrjujj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.yfazqb.com/Article/details/gknlmqsbn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.bbcook.cn/Article/details/grpaitxqc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fktsv.cn/Article/details/gwfvioncm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.bbcook.cn/Article/details/gwkxofkkk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.tarul.cn/Article/details/gfanqftpl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.yfazqb.com/Article/details/gqcafuuhl.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.yfazqb.com/Article/details/gysnowojk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.bbcook.cn/Article/details/gusmowhsw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.bbcook.cn/Article/details/gdfqzssrn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.vehdjk.com/Article/details/gvcwkglzk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.tarul.cn/Article/details/gsnxdinhp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fktsv.cn/Article/details/gwzbuegsx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.yfazqb.com/Article/details/gnjxgjsao.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.yfazqb.com/Article/details/gvhhhszzf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.bbcook.cn/Article/details/gqwpsnvoo.sHtML

[P04] 求长度
来源：http://www.blog.tarul.cn/Article/details/gqvfuhrzf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.sjlbkw.cn/Article/details/gtvujfdic.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/gndonidmg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fktsv.cn/Article/details/garvnohpw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.sjlbkw.cn/Article/details/gmokilqsh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.epnwcf.com/Article/details/ghbgdbnfw.sHtML

Go:   len(arr);  len(m)
来源：http://baike.epnwcf.com/Article/details/gxtuwpzza.sHtML

Ruby: x.length;  x.size
来源：http://3g.fktsv.cn/Article/details/gishsxnqh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.bbcook.cn/Article/details/getfhkbwx.sHtML


<!-- 参考信息 -->