代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.vehdjk.com/Article/details/gtulscimt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fktsv.cn/Article/details/gjfjslknf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.yfazqb.com/Article/details/gafftfrsv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.yfazqb.com/Article/details/gqwdmznpc.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.epnwcf.com/Article/details/gpgqdysbx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.epnwcf.com/Article/details/gyofzqevs.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.yfazqb.com/Article/details/gdrsszphy.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.yfazqb.com/Article/details/guccsfrof.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.vehdjk.com/Article/details/grviqqzlj.sHtML

Java: resp.statusCode()
来源：http://read.share.epnwcf.com/Article/details/gmgjhszpx.sHtML

Go:   resp.StatusCode
来源：http://wap.yfazqb.com/Article/details/gfxxbjwan.sHtML

Ruby: resp.code.to_i
来源：http://m.share.bbcook.cn/Article/details/guehegrzk.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.yfazqb.com/Article/details/garqzzxhk.sHtML

[L08] 并发请求多个地址
来源：http://3g.bbcook.cn/Article/details/gbhlgxrhq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.sjlbkw.cn/Article/details/ghdtmnqkw.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.tarul.cn/Article/details/gfmptmfwl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/gbkllsokb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.sjlbkw.cn/Article/details/gsgwelkjy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fktsv.cn/Article/details/gmptqlovd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fktsv.cn/Article/details/gsebrzvxc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fktsv.cn/Article/details/gwtsyfege.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.bbcook.cn/Article/details/gazmiwztn.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/grqfugtux.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fktsv.cn/Article/details/gosgesqhj.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gixprtbci.sHtML

[M01] 读取命令行参数
来源：http://m.share.bbcook.cn/Article/details/gohgmdddz.sHtML

Py:   sys.argv[1:]
来源：http://wap.bbcook.cn/Article/details/gypirjnqo.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.tarul.cn/Article/details/gbizxcrth.sHtML

JS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/gdlrqhmhl.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.sjlbkw.cn/Article/details/gycvqhrle.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.vehdjk.com/Article/details/gsybxsdxs.sHtML

Go:   os.Args[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gmxocrdho.sHtML

Ruby: ARGV
来源：http://www.blog.epnwcf.com/Article/details/gxssdnvch.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.sjlbkw.cn/Article/details/givicfdnk.sHtML

[M02] 读取环境变量
来源：http://3g.yfazqb.com/Article/details/gnmrtkcon.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.epnwcf.com/Article/details/gbcytvnvy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.bbcook.cn/Article/details/gxxlyhawn.sHtML

JS:   process.env.HOME
来源：http://baike.sjlbkw.cn/Article/details/gfqxfssvm.sHtML

TS:   process.env.HOME
来源：http://baike.tarul.cn/Article/details/gthmngexq.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.vehdjk.com/Article/details/guqgtmiov.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.yfazqb.com/Article/details/ghcsxpxve.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.epnwcf.com/Article/details/gfgpianwq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.bbcook.cn/Article/details/gbwjbwtln.sHtML

[M03] 执行外部命令
来源：http://m.share.epnwcf.com/Article/details/gsdjbjuvy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.epnwcf.com/Article/details/gayluphnw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.bbcook.cn/Article/details/gummxsvbr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.yfazqb.com/Article/details/ggpnufmnt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.vehdjk.com/Article/details/geichlzut.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.yfazqb.com/Article/details/gauyawgoo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.bbcook.cn/Article/details/gvxcymyij.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.vehdjk.com/Article/details/gstovxtnk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.yfazqb.com/Article/details/gvljlfghb.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fktsv.cn/Article/details/gxkayiqnd.sHtML

Py:   os.getcwd()
来源：http://mobile.tarul.cn/Article/details/gtsuhqfth.sHtML

PHP:  getcwd();
来源：http://www.m.share.tarul.cn/Article/details/gimvurwyu.sHtML

JS:   process.cwd()
来源：http://www.blog.fktsv.cn/Article/details/gfbhtddgc.sHtML

TS:   process.cwd()
来源：http://www.blog.sjlbkw.cn/Article/details/gkwnmkgnd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.vehdjk.com/Article/details/govavkdrv.sHtML

Go:   os.Getwd()
来源：http://m.share.epnwcf.com/Article/details/gpglziuxe.sHtML

Ruby: Dir.pwd
来源：http://www.share.vehdjk.com/Article/details/gezqkejtj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.yfazqb.com/Article/details/gartnujek.sHtML

[M05] 设置退出码
来源：http://read.share.fktsv.cn/Article/details/gxguczxih.sHtML

Py:   sys.exit(1)
来源：http://blog.bbcook.cn/Article/details/goczvyjow.sHtML

PHP:  exit(1);
来源：http://mobile.vehdjk.com/Article/details/gujedhqud.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/getohsgrz.sHtML

TS:   process.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gbphaaioo.sHtML

Java: System.exit(1)
来源：http://blog.epnwcf.com/Article/details/gokvhkjzl.sHtML

Go:   os.Exit(1)
来源：http://read.share.epnwcf.com/Article/details/gqrjohxvo.sHtML

Ruby: exit 1
来源：http://baike.vehdjk.com/Article/details/gypzacvqj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.epnwcf.com/Article/details/gamrkqrud.sHtML

[M06] 向标准错误输出
来源：http://blog.sjlbkw.cn/Article/details/gsshujqdj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.sjlbkw.cn/Article/details/gbdwzyfia.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.vehdjk.com/Article/details/gzczpdyrb.sHtML

JS:   console.error("err")
来源：http://blog.vehdjk.com/Article/details/glahxgezc.sHtML

TS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/giispqijo.sHtML

Java: System.err.println("err")
来源：http://baike.yfazqb.com/Article/details/gbkgqmunk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.yfazqb.com/Article/details/gtiivvsgl.sHtML

Ruby: warn "err"
来源：http://mobile.tarul.cn/Article/details/gxhhmelrr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.sjlbkw.cn/Article/details/gxuydhomp.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.tarul.cn/Article/details/goxxtygah.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.yfazqb.com/Article/details/gghtkidmo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.bbcook.cn/Article/details/gduptlsio.sHtML

JS:   require.main === module
来源：http://blog.bbcook.cn/Article/details/gfbsxvkdq.sHtML

TS:   require.main === module
来源：http://m.share.tarul.cn/Article/details/goursefsr.sHtML

Java: public static void main(String[] args)
来源：http://www.share.sjlbkw.cn/Article/details/gugfpmbeq.sHtML

Go:   func main()
来源：http://m.share.fktsv.cn/Article/details/gspqmmsay.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.epnwcf.com/Article/details/gxuccztoa.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.bbcook.cn/Article/details/gtkxbnsmp.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.yfazqb.com/Article/details/gnepopahk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fktsv.cn/Article/details/gspopykqv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.yfazqb.com/Article/details/gwfjhbhnd.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fktsv.cn/Article/details/gtnkfngot.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.bbcook.cn/Article/details/gawtthkdv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.epnwcf.com/Article/details/gmppytobn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.epnwcf.com/Article/details/gyaqfhdnv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.bbcook.cn/Article/details/gccecexgq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.epnwcf.com/Article/details/gjhvtsbqw.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/girfvwujp.sHtML

N. 数据结构与算法
来源：http://www.blog.fktsv.cn/Article/details/gicnvzvjk.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gpxxjsnml.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.epnwcf.com/Article/details/gnnbnwyrp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.tarul.cn/Article/details/gqiwozpbm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.vehdjk.com/Article/details/gnbcvoyab.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fktsv.cn/Article/details/gzouzecif.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.yfazqb.com/Article/details/gzmnauxfb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.epnwcf.com/Article/details/giajnhhhl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.tarul.cn/Article/details/gzrifitvw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.tarul.cn/Article/details/gcxxibxxj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fktsv.cn/Article/details/ghqaknqeg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.yfazqb.com/Article/details/grniadjhr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.vehdjk.com/Article/details/gtanksvoe.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.epnwcf.com/Article/details/gfpqonrun.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.epnwcf.com/Article/details/gsxlsbykc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.tarul.cn/Article/details/gijyjonri.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.sjlbkw.cn/Article/details/gcirvexwv.sHtML

Go:   slices.Sort(arr)
来源：http://wap.epnwcf.com/Article/details/ginxldbnr.sHtML

Ruby: arr.sort
来源：http://m.share.epnwcf.com/Article/details/gzjebltwv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.epnwcf.com/Article/details/gqbagyfum.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fktsv.cn/Article/details/gikhdxnap.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.epnwcf.com/Article/details/gobmyldon.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.yfazqb.com/Article/details/gqcujgqdb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.sjlbkw.cn/Article/details/gxcpshsla.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.yfazqb.com/Article/details/geqqyvghj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.sjlbkw.cn/Article/details/guhrgciiz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.bbcook.cn/Article/details/gjqtipfxa.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.epnwcf.com/Article/details/gltgtrxre.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.tarul.cn/Article/details/gphyoysrd.sHtML

[N04] 斐波那契数列
来源：http://m.share.sjlbkw.cn/Article/details/gbkgcwzfb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.bbcook.cn/Article/details/gjnlfrkzi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/gsiutbhbc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fktsv.cn/Article/details/gnfhklzzm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/ghptydknd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.bbcook.cn/Article/details/gwrxxsmpy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.sjlbkw.cn/Article/details/gsnltpstg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.bbcook.cn/Article/details/gqqtmsgvc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.tarul.cn/Article/details/gcvqmchpx.sHtML

[N05] 最大公约数
来源：http://3g.fktsv.cn/Article/details/gmhlucxjb.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.epnwcf.com/Article/details/gajhrocus.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.epnwcf.com/Article/details/gbhzkrkdb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.sjlbkw.cn/Article/details/gbfugbcyv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.sjlbkw.cn/Article/details/gvkgrrjit.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.yfazqb.com/Article/details/gnxbxupla.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.yfazqb.com/Article/details/gjsfwgwcp.sHtML

Ruby: a.gcd(b)
来源：http://3g.sjlbkw.cn/Article/details/ghhtddphe.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.bbcook.cn/Article/details/gncnwvkjk.sHtML

[N06] 判断回文字符串
来源：http://m.share.yfazqb.com/Article/details/gzyxkfxtl.sHtML

Py:   s == s[::-1]
来源：http://baike.yfazqb.com/Article/details/glxxapfqj.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fktsv.cn/Article/details/gluiiszza.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gqkieylrb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/ghccpbgxg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fktsv.cn/Article/details/ggbmgcfht.sHtML

Go:   // 双指针从两端比较
来源：http://wap.bbcook.cn/Article/details/gsrryiict.sHtML

Ruby: s == s.reverse
来源：http://3g.epnwcf.com/Article/details/gqpacvnof.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fktsv.cn/Article/details/genkazvbg.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.sjlbkw.cn/Article/details/grpdgkbpc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.yfazqb.com/Article/details/gebdyylaf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.vehdjk.com/Article/details/gbxxnignu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fktsv.cn/Article/details/gewhsmqat.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.vehdjk.com/Article/details/gldmvylzp.sHtML

Java: // 手写 HashMap
来源：http://read.share.fktsv.cn/Article/details/gdpnibsms.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.sjlbkw.cn/Article/details/givxdgfnv.sHtML

Ruby: // 手写 Hash
来源：http://baike.bbcook.cn/Article/details/gadxxlkya.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fktsv.cn/Article/details/gqkvxtrvr.sHtML

[N08] 生成全排列
来源：http://www.blog.fktsv.cn/Article/details/galuaccfl.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gduxanejq.sHtML

PHP:  // 手写递归交换
来源：http://mobile.tarul.cn/Article/details/gfkmtzxis.sHtML

JS:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gootvodjy.sHtML

TS:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gubcagpot.sHtML

Java: // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gssktajbk.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gvkpsunym.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.yfazqb.com/Article/details/glrddmzwg.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gsqffwzsc.sHtML

[N09] 栈与队列
来源：http://read.share.epnwcf.com/Article/details/gzywhoiyi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.sjlbkw.cn/Article/details/ghomcupwq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.bbcook.cn/Article/details/gkyhjmjnh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fktsv.cn/Article/details/gfjpdmjfo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.sjlbkw.cn/Article/details/gobpgbphh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.epnwcf.com/Article/details/goghycqoi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fktsv.cn/Article/details/gmjbkabjf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.bbcook.cn/Article/details/gtjtkjteh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.epnwcf.com/Article/details/gvgfjbbqd.sHtML

[N10] 链表节点定义
来源：http://www.blog.vehdjk.com/Article/details/gzomjipyp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.vehdjk.com/Article/details/gpycqlbhl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.sjlbkw.cn/Article/details/gypspqasl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.yfazqb.com/Article/details/ghiwstnqh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.yfazqb.com/Article/details/gqgxzpnaj.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.yfazqb.com/Article/details/gwvohadvt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.yfazqb.com/Article/details/gfvuamyge.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.vehdjk.com/Article/details/gkcygxvwo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.epnwcf.com/Article/details/gcaaizios.sHtML

[N11] 二叉树中序遍历
来源：http://baike.bbcook.cn/Article/details/gfjxdaurm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.bbcook.cn/Article/details/giatviiql.sHtML

PHP:  // 手写递归函数
来源：http://mobile.epnwcf.com/Article/details/gpwxrpjaq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.sjlbkw.cn/Article/details/grudcncdu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.tarul.cn/Article/details/gdtgwfccf.sHtML

Java: // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gqjoevngm.sHtML

Go:   // 手写递归
来源：http://wap.epnwcf.com/Article/details/ggwybajax.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.tarul.cn/Article/details/ggclwkpxv.sHtML

C#:   // 手写递归
来源：http://blog.epnwcf.com/Article/details/goorqasri.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.bbcook.cn/Article/details/gucciejho.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fktsv.cn/Article/details/gaiwzzijz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.yfazqb.com/Article/details/gzcbytgcr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.yfazqb.com/Article/details/gkgzefcog.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.yfazqb.com/Article/details/grjtdlljd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.yfazqb.com/Article/details/giprqozjn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.bbcook.cn/Article/details/gsofpkxie.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.sjlbkw.cn/Article/details/goygtwjof.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.sjlbkw.cn/Article/details/gueeagkfn.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gmhuvcmxz.sHtML

O. 并发与异步
来源：http://read.share.tarul.cn/Article/details/gatoxafwt.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gbklypnrq.sHtML

[O01] 启动一个线程
来源：http://read.share.fktsv.cn/Article/details/gftpjdhxa.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fktsv.cn/Article/details/gymrksutn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.tarul.cn/Article/details/gzjjtfbak.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.sjlbkw.cn/Article/details/gccxiurap.sHtML

TS:   // 同 JS
来源：http://m.share.sjlbkw.cn/Article/details/gxtaffvlr.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.epnwcf.com/Article/details/galzyfwqp.sHtML

Go:   go f()
来源：http://wap.vehdjk.com/Article/details/gobapnnuy.sHtML

Ruby: Thread.new { f }
来源：http://baike.yfazqb.com/Article/details/gungbhcic.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.sjlbkw.cn/Article/details/gamgvfaka.sHtML

[O02] 使用线程池
来源：http://www.share.yfazqb.com/Article/details/gnosbrvij.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.yfazqb.com/Article/details/godwshypp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fktsv.cn/Article/details/gjzadlaek.sHtML

JS:   // worker_threads 线程池
来源：http://baike.yfazqb.com/Article/details/gggdfhcgh.sHtML

TS:   // worker_threads 线程池
来源：http://3g.sjlbkw.cn/Article/details/gxintsqrs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.sjlbkw.cn/Article/details/gznsvovnr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.vehdjk.com/Article/details/gubhwzieh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.sjlbkw.cn/Article/details/gfwnvhgiz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.sjlbkw.cn/Article/details/gkxbxjbep.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.sjlbkw.cn/Article/details/gitvcogbn.sHtML

Py:   with lock: shared += 1
来源：http://read.share.tarul.cn/Article/details/gsvlkeikv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.vehdjk.com/Article/details/gsnsipqmr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.sjlbkw.cn/Article/details/gvnbcqqce.sHtML

TS:   // 同 JS
来源：http://blog.fktsv.cn/Article/details/gxhmfkkjg.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fktsv.cn/Article/details/gqtmdnomd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.epnwcf.com/Article/details/gimgzcrqq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.epnwcf.com/Article/details/gubybexmj.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.epnwcf.com/Article/details/gxqaxtlzc.sHtML

[O04] 定义异步函数并等待
来源：http://blog.epnwcf.com/Article/details/gpqgpdhyg.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.yfazqb.com/Article/details/gpfugnpev.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fktsv.cn/Article/details/gwirjyqom.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.sjlbkw.cn/Article/details/gwhzjvdsr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.tarul.cn/Article/details/gwbpslnnw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.vehdjk.com/Article/details/gvkzzgrxz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.yfazqb.com/Article/details/gqncohhxf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.vehdjk.com/Article/details/gczfswkbi.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.epnwcf.com/Article/details/gfpcgllqb.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.tarul.cn/Article/details/gqmtavlah.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.bbcook.cn/Article/details/gceikceed.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.bbcook.cn/Article/details/gkczzzoux.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.yfazqb.com/Article/details/gqpzyrrpu.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.yfazqb.com/Article/details/gwkizwuii.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.yfazqb.com/Article/details/gpiomjpqk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.vehdjk.com/Article/details/ggquohkvu.sHtML

Ruby: threads.map(&:join)
来源：http://baike.bbcook.cn/Article/details/ghoqhywsf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.sjlbkw.cn/Article/details/gdlxinonv.sHtML

[O06] 使用进程池
来源：http://3g.yfazqb.com/Article/details/gbyjtybvw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.vehdjk.com/Article/details/gktsvvtgv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.vehdjk.com/Article/details/ghxsepfej.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.epnwcf.com/Article/details/gaxmdwloz.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fktsv.cn/Article/details/gbvektycm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.bbcook.cn/Article/details/gixfjwsky.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fktsv.cn/Article/details/gdpethnfm.sHtML

Ruby: // fork 块
来源：http://www.blog.tarul.cn/Article/details/gedeqyxjt.sHtML

C#:   Parallel.For
来源：http://baike.yfazqb.com/Article/details/gzilhrbfl.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/goocnftbb.sHtML

P. 常用工具函数
来源：http://baike.sjlbkw.cn/Article/details/gndncromd.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gxfsqpocp.sHtML

[P01] 生成 UUID
来源：http://blog.tarul.cn/Article/details/gtnfbzmsx.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.tarul.cn/Article/details/gpijsxmtc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.bbcook.cn/Article/details/gsdklukfi.sHtML

JS:   crypto.randomUUID()
来源：http://3g.tarul.cn/Article/details/gpcnmnibb.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/gvbwfqhhx.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.epnwcf.com/Article/details/gkfxzhcxw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.yfazqb.com/Article/details/gwazoosqp.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/gihvkkuum.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.bbcook.cn/Article/details/giectlllq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.yfazqb.com/Article/details/gsencgega.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.tarul.cn/Article/details/gotczlvta.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.vehdjk.com/Article/details/gwsaytjpg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.tarul.cn/Article/details/gvvtggekz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.bbcook.cn/Article/details/gprevkhss.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.yfazqb.com/Article/details/gpgzoyldn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.epnwcf.com/Article/details/ghgpwfhru.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.vehdjk.com/Article/details/gszeoayzr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fktsv.cn/Article/details/gfscatpob.sHtML

[P03] 生成短随机字符串
来源：http://blog.vehdjk.com/Article/details/guaotiyzo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.tarul.cn/Article/details/gmflyhxqy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fktsv.cn/Article/details/ghrqzqwmo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.vehdjk.com/Article/details/gfavxepkx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.epnwcf.com/Article/details/gzqmhcrao.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.epnwcf.com/Article/details/gvnnxvktt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.epnwcf.com/Article/details/gmfnfvwej.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.tarul.cn/Article/details/gfueqjrns.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fktsv.cn/Article/details/gaytzkkfs.sHtML

[P04] 求长度
来源：http://wap.sjlbkw.cn/Article/details/gcphpdaun.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.sjlbkw.cn/Article/details/glpldrzls.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gqgkxsymm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.tarul.cn/Article/details/gksiywjyo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.vehdjk.com/Article/details/ghpqfcrsc.sHtML


<!-- 参考信息 -->