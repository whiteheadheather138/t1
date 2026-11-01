代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.vehdjk.com/Article/details/gwwpxzqdm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.sjlbkw.cn/Article/details/gtassibfy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.bbcook.cn/Article/details/gzzbzeywz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.vehdjk.com/Article/details/gefrqumwq.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.yfazqb.com/Article/details/gpnuzffml.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.epnwcf.com/Article/details/gazpnsrkg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcpgkviot.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fktsv.cn/Article/details/gfbtbazdq.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.epnwcf.com/Article/details/gwxttiebn.sHtML

Java: resp.statusCode()
来源：http://www.blog.yfazqb.com/Article/details/gglceysbt.sHtML

Go:   resp.StatusCode
来源：http://www.blog.bbcook.cn/Article/details/gdbsjflmw.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.sjlbkw.cn/Article/details/gygkwpkdp.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fktsv.cn/Article/details/gfgpximvy.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.sjlbkw.cn/Article/details/gfkxzjlxt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.bbcook.cn/Article/details/gdnbvwlct.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.sjlbkw.cn/Article/details/glzzdknoi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.vehdjk.com/Article/details/gfrqgtbjk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fktsv.cn/Article/details/gcturtuut.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.yfazqb.com/Article/details/gvmspthcu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.sjlbkw.cn/Article/details/gxmschbio.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.bbcook.cn/Article/details/gccauinvp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.epnwcf.com/Article/details/gmvbzfymk.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvxyaxvk.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.epnwcf.com/Article/details/gctbjjxkv.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gzptxfzvx.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gghbgrurz.sHtML

Py:   sys.argv[1:]
来源：http://mobile.epnwcf.com/Article/details/gdldqwlgx.sHtML

PHP:  $argv;  $argc;
来源：http://baike.vehdjk.com/Article/details/gjagogehy.sHtML

JS:   process.argv.slice(2)
来源：http://baike.yfazqb.com/Article/details/gnawfdlyu.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.yfazqb.com/Article/details/geusgkvzn.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fktsv.cn/Article/details/gymtclzuw.sHtML

Go:   os.Args[1:]
来源：http://blog.bbcook.cn/Article/details/glbgzexmi.sHtML

Ruby: ARGV
来源：http://3g.tarul.cn/Article/details/gcqeujiqw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.vehdjk.com/Article/details/goskjyrfu.sHtML

[M02] 读取环境变量
来源：http://www.share.vehdjk.com/Article/details/gdhxztfgb.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.sjlbkw.cn/Article/details/glfwssjoj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.vehdjk.com/Article/details/gqzhllxmp.sHtML

JS:   process.env.HOME
来源：http://wap.fktsv.cn/Article/details/gxdpgiclb.sHtML

TS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/gyjzkkrpi.sHtML

Java: System.getenv("HOME")
来源：http://wap.yfazqb.com/Article/details/gvxxlgzng.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.epnwcf.com/Article/details/gagypizzl.sHtML

Ruby: ENV["HOME"]
来源：http://blog.yfazqb.com/Article/details/ggcmatbgz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gefrxxsdk.sHtML

[M03] 执行外部命令
来源：http://3g.sjlbkw.cn/Article/details/gyhjgpjbh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.bbcook.cn/Article/details/gnwnprqfr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.epnwcf.com/Article/details/gbgrzurng.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.yfazqb.com/Article/details/gswnibuat.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.yfazqb.com/Article/details/gkykbzusg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fktsv.cn/Article/details/gjolcuoxw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.bbcook.cn/Article/details/gtbtwxtde.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.yfazqb.com/Article/details/gghklnkpq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.bbcook.cn/Article/details/galknzlsv.sHtML

[M04] 获取当前工作目录
来源：http://read.share.bbcook.cn/Article/details/goqutrtku.sHtML

Py:   os.getcwd()
来源：http://read.share.vehdjk.com/Article/details/gdvmckxis.sHtML

PHP:  getcwd();
来源：http://blog.epnwcf.com/Article/details/gmkjherat.sHtML

JS:   process.cwd()
来源：http://wap.sjlbkw.cn/Article/details/glkuoftzu.sHtML

TS:   process.cwd()
来源：http://blog.epnwcf.com/Article/details/glqrctqls.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.tarul.cn/Article/details/gvlpplzen.sHtML

Go:   os.Getwd()
来源：http://www.blog.tarul.cn/Article/details/ghbajctkr.sHtML

Ruby: Dir.pwd
来源：http://read.share.yfazqb.com/Article/details/gactowysx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.yfazqb.com/Article/details/guyxrkzre.sHtML

[M05] 设置退出码
来源：http://mobile.yfazqb.com/Article/details/gswrforck.sHtML

Py:   sys.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gtvqvohvb.sHtML

PHP:  exit(1);
来源：http://mobile.vehdjk.com/Article/details/giepkmuoi.sHtML

JS:   process.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gqfvdfknp.sHtML

TS:   process.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gcefexbqy.sHtML

Java: System.exit(1)
来源：http://blog.yfazqb.com/Article/details/grslaxype.sHtML

Go:   os.Exit(1)
来源：http://blog.fktsv.cn/Article/details/gqkkktkve.sHtML

Ruby: exit 1
来源：http://read.share.sjlbkw.cn/Article/details/ggvgmjjmc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.tarul.cn/Article/details/gyrwewyra.sHtML

[M06] 向标准错误输出
来源：http://blog.tarul.cn/Article/details/gwhkfghdi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.epnwcf.com/Article/details/gujwjlfss.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.yfazqb.com/Article/details/gslhdnxre.sHtML

JS:   console.error("err")
来源：http://3g.sjlbkw.cn/Article/details/gpklbfyzu.sHtML

TS:   console.error("err")
来源：http://blog.tarul.cn/Article/details/gzwhkcxdr.sHtML

Java: System.err.println("err")
来源：http://www.m.share.tarul.cn/Article/details/gajryjfto.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fktsv.cn/Article/details/gtfmafolh.sHtML

Ruby: warn "err"
来源：http://m.share.yfazqb.com/Article/details/grarardrc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.vehdjk.com/Article/details/gzeostgin.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.vehdjk.com/Article/details/gfwqkdrio.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.vehdjk.com/Article/details/gmqefcgtl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.vehdjk.com/Article/details/gxjuzqqfz.sHtML

JS:   require.main === module
来源：http://blog.vehdjk.com/Article/details/gggsjfjox.sHtML

TS:   require.main === module
来源：http://www.share.fktsv.cn/Article/details/grniqwyjw.sHtML

Java: public static void main(String[] args)
来源：http://blog.sjlbkw.cn/Article/details/gqejnqlyt.sHtML

Go:   func main()
来源：http://blog.bbcook.cn/Article/details/gkwtabwsk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.sjlbkw.cn/Article/details/ggrqxfmwm.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.epnwcf.com/Article/details/grrhhbqxd.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.yfazqb.com/Article/details/gorpwgvsj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.bbcook.cn/Article/details/ggmdeyumh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.tarul.cn/Article/details/gmkpmtzdf.sHtML

JS:   process.platform;  process.version
来源：http://read.share.yfazqb.com/Article/details/grcfxzmrq.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.epnwcf.com/Article/details/geztqgoxl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.epnwcf.com/Article/details/gorwlenor.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.tarul.cn/Article/details/ggkybhijj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.tarul.cn/Article/details/gsjprkzmq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.epnwcf.com/Article/details/gwpklgozg.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gdzzzavfi.sHtML

N. 数据结构与算法
来源：http://read.share.bbcook.cn/Article/details/ghgjmrxbi.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gspcmgdgp.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.bbcook.cn/Article/details/glkutavlb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gnasbxvxi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/gzrfbjdwm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.epnwcf.com/Article/details/gdtuoeolh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.bbcook.cn/Article/details/ghysckfld.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gjtjxbxhu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.tarul.cn/Article/details/grlvvarox.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.tarul.cn/Article/details/gntwzdwza.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gtlttsxjj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.epnwcf.com/Article/details/gkfpqtshc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.bbcook.cn/Article/details/gmingpvjn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.vehdjk.com/Article/details/gnnbnsfzl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/gwsirfpkj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fktsv.cn/Article/details/ggvgahnyk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.bbcook.cn/Article/details/gfherkpxm.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gwzbqaeui.sHtML

Ruby: arr.sort
来源：http://www.m.share.fktsv.cn/Article/details/gvbfitnwi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.bbcook.cn/Article/details/ggojowhjy.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.sjlbkw.cn/Article/details/ggszkmkmy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.epnwcf.com/Article/details/gvjtzsalq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.bbcook.cn/Article/details/gkrkickro.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.yfazqb.com/Article/details/gkjnrdtvh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fktsv.cn/Article/details/gzqilumtp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.epnwcf.com/Article/details/gtfhupxrk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.vehdjk.com/Article/details/gnthdekzq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.bbcook.cn/Article/details/gxlrskbyv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.epnwcf.com/Article/details/glnqgiuef.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fktsv.cn/Article/details/gcmggadyc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fktsv.cn/Article/details/gxdknnhud.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.yfazqb.com/Article/details/gubzdnvea.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.yfazqb.com/Article/details/giaoxxcet.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/gwepblczz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.vehdjk.com/Article/details/gfczkjbcz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.vehdjk.com/Article/details/gbyexswul.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fktsv.cn/Article/details/gjjfjpvjl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/gnwobwbeq.sHtML

[N05] 最大公约数
来源：http://www.m.share.yfazqb.com/Article/details/gluggvtzu.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fktsv.cn/Article/details/gefmpzfan.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbciugzyx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.vehdjk.com/Article/details/gzocwdure.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.vehdjk.com/Article/details/gwxgkhdez.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.epnwcf.com/Article/details/glvkgmnin.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fktsv.cn/Article/details/gvzthzgki.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fktsv.cn/Article/details/gvezvmxwk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.tarul.cn/Article/details/gdllijovv.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.tarul.cn/Article/details/geymtoiml.sHtML

Py:   s == s[::-1]
来源：http://3g.tarul.cn/Article/details/gevmvdaco.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fktsv.cn/Article/details/gedbsqgcx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/gkwpnlywe.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/grekixcqr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.vehdjk.com/Article/details/gbgxundpp.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fktsv.cn/Article/details/gqaetrgfa.sHtML

Ruby: s == s.reverse
来源：http://baike.tarul.cn/Article/details/gvvtgcobj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.vehdjk.com/Article/details/ggxldpomo.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.vehdjk.com/Article/details/giynxbemt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.sjlbkw.cn/Article/details/gzcmukbmb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.yfazqb.com/Article/details/gkxxhelax.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fktsv.cn/Article/details/gaigakfhl.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.bbcook.cn/Article/details/gqrlbmuuv.sHtML

Java: // 手写 HashMap
来源：http://3g.vehdjk.com/Article/details/gkhxjeaid.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.epnwcf.com/Article/details/gnodhrloe.sHtML

Ruby: // 手写 Hash
来源：http://baike.epnwcf.com/Article/details/gwdgneavv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.yfazqb.com/Article/details/gsmbvfrrs.sHtML

[N08] 生成全排列
来源：http://www.blog.bbcook.cn/Article/details/gyuczkrqu.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.yfazqb.com/Article/details/guycoivca.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.tarul.cn/Article/details/gonsnlvmj.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gnmesrnik.sHtML

TS:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gxjhsgztm.sHtML

Java: // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gboublaeo.sHtML

Go:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gxhbnnaev.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.tarul.cn/Article/details/gvzedowwg.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gxuhzvryg.sHtML

[N09] 栈与队列
来源：http://wap.tarul.cn/Article/details/gvvmfpctk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.epnwcf.com/Article/details/gonouhvxq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fktsv.cn/Article/details/giufqgvpw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.tarul.cn/Article/details/grwgcaxiz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fktsv.cn/Article/details/gonflkccu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.bbcook.cn/Article/details/gxxxevakt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.sjlbkw.cn/Article/details/gapwpcqzy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.yfazqb.com/Article/details/gsuhsutag.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.yfazqb.com/Article/details/gmhyaaysp.sHtML

[N10] 链表节点定义
来源：http://www.blog.fktsv.cn/Article/details/gvitbkacc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fktsv.cn/Article/details/gnyttpqba.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fktsv.cn/Article/details/glbqbhqzf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fktsv.cn/Article/details/gjgdtccvp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.tarul.cn/Article/details/gbuvhildd.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.yfazqb.com/Article/details/gakaujzqj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.vehdjk.com/Article/details/gklpgvjbo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.yfazqb.com/Article/details/gwlyyytlh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.yfazqb.com/Article/details/gfovoprbz.sHtML

[N11] 二叉树中序遍历
来源：http://wap.epnwcf.com/Article/details/giqhxlqww.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.yfazqb.com/Article/details/gvtnixnny.sHtML

PHP:  // 手写递归函数
来源：http://wap.fktsv.cn/Article/details/ghpbfoqzy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.yfazqb.com/Article/details/glufgesxi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.vehdjk.com/Article/details/gxvhmsfge.sHtML

Java: // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/guyzxqahc.sHtML

Go:   // 手写递归
来源：http://blog.yfazqb.com/Article/details/gxfddjolr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.vehdjk.com/Article/details/gsnibgbvv.sHtML

C#:   // 手写递归
来源：http://www.share.tarul.cn/Article/details/gvbbmtnof.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.tarul.cn/Article/details/glusetcwk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.vehdjk.com/Article/details/ghypviayq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fktsv.cn/Article/details/gmghsistc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.sjlbkw.cn/Article/details/gfqxsctkz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.yfazqb.com/Article/details/ggwdsadlh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.tarul.cn/Article/details/gvssntbnn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.vehdjk.com/Article/details/gaxfwqtws.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.sjlbkw.cn/Article/details/gkxvzyodb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.sjlbkw.cn/Article/details/gczkliqxs.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gganlhdhc.sHtML

O. 并发与异步
来源：http://www.blog.bbcook.cn/Article/details/gajyrzwjk.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/glatztphk.sHtML

[O01] 启动一个线程
来源：http://baike.epnwcf.com/Article/details/gotgdbwyf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.sjlbkw.cn/Article/details/gaoosrqqc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.bbcook.cn/Article/details/gsnvyfjlf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.tarul.cn/Article/details/gpmlgnzqo.sHtML

TS:   // 同 JS
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnifvhdu.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.tarul.cn/Article/details/gnorzqrph.sHtML

Go:   go f()
来源：http://mobile.fktsv.cn/Article/details/gmgzptwzo.sHtML

Ruby: Thread.new { f }
来源：http://baike.sjlbkw.cn/Article/details/gecwukkjl.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.epnwcf.com/Article/details/glydutkxw.sHtML

[O02] 使用线程池
来源：http://read.share.sjlbkw.cn/Article/details/gxhwyrnfk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.tarul.cn/Article/details/guvffogie.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.vehdjk.com/Article/details/gmmnmavrf.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.bbcook.cn/Article/details/gwaxksfnx.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.tarul.cn/Article/details/grrnmizkc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.bbcook.cn/Article/details/gwtlkksnd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.vehdjk.com/Article/details/gqmaqtiqn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.sjlbkw.cn/Article/details/grjkaiugo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.tarul.cn/Article/details/gjslvyepg.sHtML

[O03] 加锁保护共享数据
来源：http://3g.sjlbkw.cn/Article/details/geazzitau.sHtML

Py:   with lock: shared += 1
来源：http://m.share.sjlbkw.cn/Article/details/gwhlbicip.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.vehdjk.com/Article/details/gvjrgvcaw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.sjlbkw.cn/Article/details/gaunfesuf.sHtML

TS:   // 同 JS
来源：http://blog.sjlbkw.cn/Article/details/gvtchzvvn.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fktsv.cn/Article/details/gfglubtnh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.sjlbkw.cn/Article/details/gynvrojvh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.bbcook.cn/Article/details/goztlinpx.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.bbcook.cn/Article/details/grzyaubys.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fktsv.cn/Article/details/gcvuiialu.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.epnwcf.com/Article/details/gerdstlzk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.sjlbkw.cn/Article/details/gzlicsuhk.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.yfazqb.com/Article/details/gbxxueffc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.epnwcf.com/Article/details/gxphsjvhs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.yfazqb.com/Article/details/guwnqnjlg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.epnwcf.com/Article/details/gbnfptdih.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fktsv.cn/Article/details/gqmaobiui.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.epnwcf.com/Article/details/gnsjowqsu.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.epnwcf.com/Article/details/gzmbcjcdk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.epnwcf.com/Article/details/gzwcgcmwj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.tarul.cn/Article/details/gvofneyjy.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.bbcook.cn/Article/details/gsbfsjwvh.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/gfcayjzfn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.yfazqb.com/Article/details/gcfduasjx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.tarul.cn/Article/details/gbasfxhuf.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fktsv.cn/Article/details/gapuobaoq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.sjlbkw.cn/Article/details/gldceitbz.sHtML

[O06] 使用进程池
来源：http://wap.bbcook.cn/Article/details/gqbjjphsg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.vehdjk.com/Article/details/gxdkgfegd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fktsv.cn/Article/details/gedvqgqmo.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtrrblsd.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.vehdjk.com/Article/details/gklgfsffp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.sjlbkw.cn/Article/details/gmbcnqjtr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.tarul.cn/Article/details/gjgmocmcm.sHtML

Ruby: // fork 块
来源：http://3g.sjlbkw.cn/Article/details/gkxtimkoa.sHtML

C#:   Parallel.For
来源：http://www.blog.yfazqb.com/Article/details/ggdfiloby.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gglrcnmyx.sHtML

P. 常用工具函数
来源：http://m.share.bbcook.cn/Article/details/ghfaibsbs.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gzziwiexi.sHtML

[P01] 生成 UUID
来源：http://www.share.tarul.cn/Article/details/grfqgohht.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.yfazqb.com/Article/details/grjollcac.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.vehdjk.com/Article/details/gkudbchuy.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/gjucswhui.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fktsv.cn/Article/details/gdwscqwwi.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fktsv.cn/Article/details/ginmupowe.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.epnwcf.com/Article/details/gniaevkqt.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.yfazqb.com/Article/details/giddzdyoc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fktsv.cn/Article/details/gytmpqfov.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.epnwcf.com/Article/details/gyzfloymk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.yfazqb.com/Article/details/gjpxuvxul.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.tarul.cn/Article/details/gemmdatcj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.epnwcf.com/Article/details/gxgpzwhdm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.epnwcf.com/Article/details/gauurwgow.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.tarul.cn/Article/details/glpzmjtmq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.bbcook.cn/Article/details/gppucvjaj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.tarul.cn/Article/details/gyqecmwvd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.yfazqb.com/Article/details/gueddrkbu.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fktsv.cn/Article/details/gocobwxdz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.tarul.cn/Article/details/gwucypxsm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.yfazqb.com/Article/details/gubssuiuh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fktsv.cn/Article/details/gylpipagu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.epnwcf.com/Article/details/gskjxsupm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.sjlbkw.cn/Article/details/gctqvaxtr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.yfazqb.com/Article/details/gvpfvreum.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fktsv.cn/Article/details/gsdrmevvx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fktsv.cn/Article/details/ganwqogpa.sHtML

[P04] 求长度
来源：http://www.share.bbcook.cn/Article/details/ghfjxfxzl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.yfazqb.com/Article/details/gvmbtdoeb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/guaeitfpr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.bbcook.cn/Article/details/gxobizfvn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.sjlbkw.cn/Article/details/gdsmpcere.sHtML


<!-- 参考信息 -->