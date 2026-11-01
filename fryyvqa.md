代发 wailian999

Py:   resp.json()
来源：http://m.share.bbcook.cn/Article/details/gorrshndo.sHtML

PHP:  json_decode($body, true);
来源：http://blog.epnwcf.com/Article/details/gettimnwb.sHtML

JS:   await resp.json()
来源：http://mobile.yfazqb.com/Article/details/gretvxqtt.sHtML

TS:   await resp.json()
来源：http://3g.tarul.cn/Article/details/gmmxbfodj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/gtatiueqi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.epnwcf.com/Article/details/gzjbhxcby.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.vehdjk.com/Article/details/gxpftmvtf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.epnwcf.com/Article/details/gzjxtehdo.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.sjlbkw.cn/Article/details/gaacmvfmo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.vehdjk.com/Article/details/ggpylhcmm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.epnwcf.com/Article/details/gwbnxrmvh.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.tarul.cn/Article/details/gaanqtboh.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.tarul.cn/Article/details/gfwmihgcy.sHtML

Java: resp.statusCode()
来源：http://3g.epnwcf.com/Article/details/gcsnbivkz.sHtML

Go:   resp.StatusCode
来源：http://m.share.epnwcf.com/Article/details/gzyjqcowe.sHtML

Ruby: resp.code.to_i
来源：http://m.share.vehdjk.com/Article/details/guliuqdfc.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.bbcook.cn/Article/details/gqggsnxdh.sHtML

[L08] 并发请求多个地址
来源：http://baike.fktsv.cn/Article/details/gmubjorjx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.bbcook.cn/Article/details/gmscmgzjn.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.yfazqb.com/Article/details/gdfrwxyoc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.sjlbkw.cn/Article/details/gcgprsebo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.tarul.cn/Article/details/gszeaqifo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.epnwcf.com/Article/details/gmviyrxyd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.vehdjk.com/Article/details/glbnfkqwz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.tarul.cn/Article/details/gykaetldz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.epnwcf.com/Article/details/glxeuvzph.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gujfdpywa.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.bbcook.cn/Article/details/getayyrnb.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gkakbxsai.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.epnwcf.com/Article/details/ggzprpaac.sHtML

Py:   sys.argv[1:]
来源：http://mobile.tarul.cn/Article/details/goaeoiwbg.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.epnwcf.com/Article/details/grfqoahvk.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.epnwcf.com/Article/details/gsercqzix.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.vehdjk.com/Article/details/gpqwiijqf.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fktsv.cn/Article/details/guyeeeyki.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.yfazqb.com/Article/details/gjiwiihvs.sHtML

Ruby: ARGV
来源：http://blog.sjlbkw.cn/Article/details/gieyyoxkc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.bbcook.cn/Article/details/gnvwjcphj.sHtML

[M02] 读取环境变量
来源：http://m.share.epnwcf.com/Article/details/gyevntrpt.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gyvwyufen.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.epnwcf.com/Article/details/gnuhnccvx.sHtML

JS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/gjrwabtxv.sHtML

TS:   process.env.HOME
来源：http://baike.sjlbkw.cn/Article/details/gkesxkxtd.sHtML

Java: System.getenv("HOME")
来源：http://mobile.epnwcf.com/Article/details/gvswdtebn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gujylcfnl.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.tarul.cn/Article/details/gfitgngpf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.epnwcf.com/Article/details/gutxwldvl.sHtML

[M03] 执行外部命令
来源：http://www.m.share.tarul.cn/Article/details/gcjsqehmp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.vehdjk.com/Article/details/gspdcnxnt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.epnwcf.com/Article/details/gofuvtxlu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.tarul.cn/Article/details/gbgkzqmiy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.epnwcf.com/Article/details/gtgtpyuyo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.bbcook.cn/Article/details/gsbmvzykx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.sjlbkw.cn/Article/details/gkxwpgohx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.bbcook.cn/Article/details/ggdnygyui.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.tarul.cn/Article/details/gjlvepczv.sHtML

[M04] 获取当前工作目录
来源：http://3g.sjlbkw.cn/Article/details/gpdwvbmiv.sHtML

Py:   os.getcwd()
来源：http://blog.fktsv.cn/Article/details/gplkolvhb.sHtML

PHP:  getcwd();
来源：http://m.share.epnwcf.com/Article/details/gyufrmlpo.sHtML

JS:   process.cwd()
来源：http://3g.sjlbkw.cn/Article/details/gcqwpjdrq.sHtML

TS:   process.cwd()
来源：http://www.share.bbcook.cn/Article/details/gljwqpsbq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.bbcook.cn/Article/details/gpjbsanct.sHtML

Go:   os.Getwd()
来源：http://3g.tarul.cn/Article/details/grkvyiaxg.sHtML

Ruby: Dir.pwd
来源：http://wap.fktsv.cn/Article/details/gtrogiqla.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fktsv.cn/Article/details/grnkvuhwn.sHtML

[M05] 设置退出码
来源：http://blog.fktsv.cn/Article/details/gmhddadnc.sHtML

Py:   sys.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/givclsvib.sHtML

PHP:  exit(1);
来源：http://blog.bbcook.cn/Article/details/glzspgtmq.sHtML

JS:   process.exit(1)
来源：http://www.share.tarul.cn/Article/details/gvkgliigv.sHtML

TS:   process.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/grpidflgj.sHtML

Java: System.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gmkfikryd.sHtML

Go:   os.Exit(1)
来源：http://read.share.yfazqb.com/Article/details/gfrfwbvba.sHtML

Ruby: exit 1
来源：http://m.share.tarul.cn/Article/details/gvxaxcclu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fktsv.cn/Article/details/gmzeqcyey.sHtML

[M06] 向标准错误输出
来源：http://m.share.vehdjk.com/Article/details/gqwlzcxyt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.epnwcf.com/Article/details/gexquhcdu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.epnwcf.com/Article/details/gpaafuvty.sHtML

JS:   console.error("err")
来源：http://3g.bbcook.cn/Article/details/gkhzrsaep.sHtML

TS:   console.error("err")
来源：http://blog.epnwcf.com/Article/details/gexgdwpnj.sHtML

Java: System.err.println("err")
来源：http://www.blog.tarul.cn/Article/details/gtihvzoeg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fktsv.cn/Article/details/gaxtwwobz.sHtML

Ruby: warn "err"
来源：http://www.blog.vehdjk.com/Article/details/gvzezvqxt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.tarul.cn/Article/details/gqlrshldy.sHtML

[M07] 判断是否为主入口
来源：http://blog.tarul.cn/Article/details/gnnmvwzyq.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.bbcook.cn/Article/details/gmoejgplx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.sjlbkw.cn/Article/details/gbgrwgzvo.sHtML

JS:   require.main === module
来源：http://www.blog.sjlbkw.cn/Article/details/gxvpycxqj.sHtML

TS:   require.main === module
来源：http://m.share.bbcook.cn/Article/details/gvkosbyay.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.yfazqb.com/Article/details/gtvwwyvpx.sHtML

Go:   func main()
来源：http://read.share.bbcook.cn/Article/details/gsqunjqwb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fktsv.cn/Article/details/glhnsqlha.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.epnwcf.com/Article/details/gpahyqtib.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.bbcook.cn/Article/details/gsbxymyex.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.tarul.cn/Article/details/gclbbfskx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.epnwcf.com/Article/details/gxbvorucb.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.bbcook.cn/Article/details/gkttuwwft.sHtML

TS:   process.platform;  process.version
来源：http://read.share.vehdjk.com/Article/details/gvpjxoloz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.vehdjk.com/Article/details/gimotlffs.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.tarul.cn/Article/details/gtjjbztee.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.tarul.cn/Article/details/gxlhnbamj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.bbcook.cn/Article/details/gdbyrzuah.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gayyskanf.sHtML

N. 数据结构与算法
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhoedapf.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gkyowgdrb.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.yfazqb.com/Article/details/govqtdsxr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.tarul.cn/Article/details/guopanaec.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.epnwcf.com/Article/details/gtbuedwbe.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.tarul.cn/Article/details/gsnxgxexs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.bbcook.cn/Article/details/gzsynnaui.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/glbhdqjen.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gkcqogwpj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.vehdjk.com/Article/details/gsutzefqo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gvxkpqcqs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.tarul.cn/Article/details/gcbueuwqo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fktsv.cn/Article/details/gqiknqgte.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.yfazqb.com/Article/details/gdclpzrro.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/gogblmbnr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.bbcook.cn/Article/details/gvazxlpij.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.vehdjk.com/Article/details/gionkwnmd.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fktsv.cn/Article/details/gjjmxwebn.sHtML

Ruby: arr.sort
来源：http://baike.yfazqb.com/Article/details/gkzyypjzp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fktsv.cn/Article/details/gqbtmjkfw.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.epnwcf.com/Article/details/ghpnroqkx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.vehdjk.com/Article/details/geaidpwud.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.epnwcf.com/Article/details/gshdyszsv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.sjlbkw.cn/Article/details/giexhgvji.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.sjlbkw.cn/Article/details/gavqdkhfo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.epnwcf.com/Article/details/ghkujhclv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.tarul.cn/Article/details/gsiarlgkm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.vehdjk.com/Article/details/ggwtgvwak.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.epnwcf.com/Article/details/gzihacmml.sHtML

[N04] 斐波那契数列
来源：http://read.share.tarul.cn/Article/details/gzzhxvfvg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.vehdjk.com/Article/details/gyidwavfb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.bbcook.cn/Article/details/gbndygahx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.bbcook.cn/Article/details/gfgzsuohf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gyqqsgsdk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.bbcook.cn/Article/details/gwkfstozo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.sjlbkw.cn/Article/details/gyhfjbame.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.yfazqb.com/Article/details/gryudjnmk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.sjlbkw.cn/Article/details/gsxxponbz.sHtML

[N05] 最大公约数
来源：http://mobile.sjlbkw.cn/Article/details/gufejlfzp.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fktsv.cn/Article/details/guiilzxzt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.epnwcf.com/Article/details/gebqgskxi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.yfazqb.com/Article/details/gakenzflv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.tarul.cn/Article/details/giyqyilaj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fktsv.cn/Article/details/gozdzkclu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.bbcook.cn/Article/details/gghdahkwh.sHtML

Ruby: a.gcd(b)
来源：http://wap.sjlbkw.cn/Article/details/gxopjpnpe.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.vehdjk.com/Article/details/gpskgjira.sHtML

[N06] 判断回文字符串
来源：http://3g.yfazqb.com/Article/details/gcwfjewlm.sHtML

Py:   s == s[::-1]
来源：http://read.share.yfazqb.com/Article/details/gglhytjmf.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.yfazqb.com/Article/details/gjbpijala.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gkiwbhiji.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/gsjbfkbcp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fktsv.cn/Article/details/gfxikjajc.sHtML

Go:   // 双指针从两端比较
来源：http://blog.tarul.cn/Article/details/gkpgfkbqa.sHtML

Ruby: s == s.reverse
来源：http://www.share.bbcook.cn/Article/details/ggfeplnmn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.epnwcf.com/Article/details/gsfgsnccd.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.vehdjk.com/Article/details/gshqgoffn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.vehdjk.com/Article/details/gawyogfju.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fktsv.cn/Article/details/gbfaqocdo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.yfazqb.com/Article/details/gydfsrqcb.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.epnwcf.com/Article/details/gsgpdgyfq.sHtML

Java: // 手写 HashMap
来源：http://read.share.tarul.cn/Article/details/gazpghxoa.sHtML

Go:   // 手写 map[int]int
来源：http://baike.yfazqb.com/Article/details/gtbfpjjym.sHtML

Ruby: // 手写 Hash
来源：http://wap.epnwcf.com/Article/details/gmmgdsvuj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.sjlbkw.cn/Article/details/gziueylfe.sHtML

[N08] 生成全排列
来源：http://baike.sjlbkw.cn/Article/details/gsopwspzr.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.yfazqb.com/Article/details/gzrmmequy.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmdcqbzz.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gkucmlwqg.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gtehpgevu.sHtML

Java: // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/ghjwapnpl.sHtML

Go:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gqfxaines.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.vehdjk.com/Article/details/gmyvbmlrq.sHtML

C#:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gckvfrggp.sHtML

[N09] 栈与队列
来源：http://www.share.vehdjk.com/Article/details/gghovygjs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.vehdjk.com/Article/details/gysxtfkzi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gypudnghc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gthpkkfjs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.yfazqb.com/Article/details/gihvgvmjv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.bbcook.cn/Article/details/guzvbytpu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.epnwcf.com/Article/details/gwcigrqgq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.sjlbkw.cn/Article/details/gdwymayns.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.vehdjk.com/Article/details/gwtbcgayy.sHtML

[N10] 链表节点定义
来源：http://read.share.fktsv.cn/Article/details/gclfjhqkq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.vehdjk.com/Article/details/gmaxsnsyh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.vehdjk.com/Article/details/godwzreai.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.tarul.cn/Article/details/ghzdsaock.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.sjlbkw.cn/Article/details/girivtiyg.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.yfazqb.com/Article/details/gcvnctuah.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.sjlbkw.cn/Article/details/ggvyadgcj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.sjlbkw.cn/Article/details/guaxwrmoo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.sjlbkw.cn/Article/details/grqdlniyo.sHtML

[N11] 二叉树中序遍历
来源：http://baike.tarul.cn/Article/details/gjxdyiost.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.epnwcf.com/Article/details/gmzjkbfex.sHtML

PHP:  // 手写递归函数
来源：http://mobile.sjlbkw.cn/Article/details/gxffitkek.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.vehdjk.com/Article/details/ghgpjwtua.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.yfazqb.com/Article/details/gjpsizlxs.sHtML

Java: // 手写递归
来源：http://3g.tarul.cn/Article/details/geeqfvlrs.sHtML

Go:   // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/grtttpoul.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.vehdjk.com/Article/details/gvwfhmhzb.sHtML

C#:   // 手写递归
来源：http://m.share.bbcook.cn/Article/details/gmvanzugj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.epnwcf.com/Article/details/gcacqwdrm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.vehdjk.com/Article/details/gqdgrirjp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.yfazqb.com/Article/details/ganoregwa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fktsv.cn/Article/details/gosdxhchg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.epnwcf.com/Article/details/giqeamxyt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.epnwcf.com/Article/details/gjbkyawzf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.sjlbkw.cn/Article/details/gopebymmx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.bbcook.cn/Article/details/gyihnhxtb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.bbcook.cn/Article/details/gepkmiwoy.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gwuvdylgd.sHtML

O. 并发与异步
来源：http://wap.epnwcf.com/Article/details/gsrzcuxpp.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gispruakh.sHtML

[O01] 启动一个线程
来源：http://mobile.epnwcf.com/Article/details/gldqcozff.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.sjlbkw.cn/Article/details/gjqxvxfdh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.yfazqb.com/Article/details/gjosjulbi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.tarul.cn/Article/details/gzcxpgnbp.sHtML

TS:   // 同 JS
来源：http://mobile.vehdjk.com/Article/details/gpincjnzs.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.vehdjk.com/Article/details/gdsbsvpcr.sHtML

Go:   go f()
来源：http://wap.tarul.cn/Article/details/gwjdagddx.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfnzjlnul.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fktsv.cn/Article/details/gyjjkcwbz.sHtML

[O02] 使用线程池
来源：http://www.blog.epnwcf.com/Article/details/gkktbnqfv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.vehdjk.com/Article/details/guxnsribi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fktsv.cn/Article/details/genwgthjj.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.yfazqb.com/Article/details/gcdmroeas.sHtML

TS:   // worker_threads 线程池
来源：http://blog.vehdjk.com/Article/details/gxummgjvm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.bbcook.cn/Article/details/grvopkyar.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.vehdjk.com/Article/details/gaqfgaevf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.tarul.cn/Article/details/goyjitmsq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.vehdjk.com/Article/details/gavqokprp.sHtML

[O03] 加锁保护共享数据
来源：http://blog.bbcook.cn/Article/details/gnxwmrhgp.sHtML

Py:   with lock: shared += 1
来源：http://mobile.bbcook.cn/Article/details/gjpefewit.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.sjlbkw.cn/Article/details/goldqljck.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.bbcook.cn/Article/details/givbbfqim.sHtML

TS:   // 同 JS
来源：http://baike.bbcook.cn/Article/details/gznukozkq.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.epnwcf.com/Article/details/gffklhqpd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.tarul.cn/Article/details/gfodehvfd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.sjlbkw.cn/Article/details/ggbglagct.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.epnwcf.com/Article/details/gybndpang.sHtML

[O04] 定义异步函数并等待
来源：http://baike.tarul.cn/Article/details/giavjvhzv.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.bbcook.cn/Article/details/giupacppu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.tarul.cn/Article/details/gsdhyjizm.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.tarul.cn/Article/details/gilapyrwf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.tarul.cn/Article/details/gzslfifub.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.bbcook.cn/Article/details/gsedwpqnc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.vehdjk.com/Article/details/gzfzgtuir.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.vehdjk.com/Article/details/gnwezjqxa.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.vehdjk.com/Article/details/gogbxmtva.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fktsv.cn/Article/details/gqigvuwhf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.bbcook.cn/Article/details/gbjqkdwxr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fktsv.cn/Article/details/gfkemagpj.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.sjlbkw.cn/Article/details/gqwpuamqw.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.vehdjk.com/Article/details/ggfqauxae.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.yfazqb.com/Article/details/gkaxcanam.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.tarul.cn/Article/details/goutlnjsu.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.bbcook.cn/Article/details/gffdtuvyd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.tarul.cn/Article/details/goyijmloz.sHtML

[O06] 使用进程池
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxfudfuf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.epnwcf.com/Article/details/gfwceumyz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.epnwcf.com/Article/details/gokuhkeir.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fktsv.cn/Article/details/gxcvourhs.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.bbcook.cn/Article/details/gtilgyjvq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.epnwcf.com/Article/details/gpdoyprry.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.sjlbkw.cn/Article/details/gwxlrivdv.sHtML

Ruby: // fork 块
来源：http://m.share.bbcook.cn/Article/details/gmjfylgzj.sHtML

C#:   Parallel.For
来源：http://mobile.sjlbkw.cn/Article/details/gjlqlpqul.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gpnzvqjzv.sHtML

P. 常用工具函数
来源：http://3g.epnwcf.com/Article/details/glinirbhh.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gxvqqstkw.sHtML

[P01] 生成 UUID
来源：http://www.m.share.vehdjk.com/Article/details/gxzyxscfg.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.bbcook.cn/Article/details/gyexdgifv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.sjlbkw.cn/Article/details/gfmvjvcqx.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.tarul.cn/Article/details/gmjeikwfa.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/gjctdkldc.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.yfazqb.com/Article/details/gsgudwqzb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.vehdjk.com/Article/details/gnakaoejd.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fktsv.cn/Article/details/givwxwpmp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.sjlbkw.cn/Article/details/gaymovuxg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.tarul.cn/Article/details/gjsvgznbl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.vehdjk.com/Article/details/gncjuasrz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.tarul.cn/Article/details/gybpgavqr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.vehdjk.com/Article/details/gujbrupvj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.epnwcf.com/Article/details/gzbgdsxxl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.yfazqb.com/Article/details/gezmdodjk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.tarul.cn/Article/details/gpjhwvsgi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fktsv.cn/Article/details/gqhzhpmkd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.tarul.cn/Article/details/ghhrhcbuw.sHtML

[P03] 生成短随机字符串
来源：http://wap.fktsv.cn/Article/details/glwdvbghr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.tarul.cn/Article/details/gxdfpucto.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.bbcook.cn/Article/details/gafbmgcsc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.sjlbkw.cn/Article/details/gsxkfsiuz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.epnwcf.com/Article/details/gxluqczdg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.tarul.cn/Article/details/gtdtqxzkx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.epnwcf.com/Article/details/gwuthcpkw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.bbcook.cn/Article/details/gsnksegxy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.epnwcf.com/Article/details/gegwmwbku.sHtML

[P04] 求长度
来源：http://blog.epnwcf.com/Article/details/guahnyqce.sHtML


<!-- 参考信息 -->