代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmyetfnk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.epnwcf.com/Article/details/gctacqnuz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.yfazqb.com/Article/details/guihgiwaw.sHtML

[L06] 解析响应为 JSON
来源：http://baike.epnwcf.com/Article/details/gqdrahkyv.sHtML

Py:   resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/gvfuqisyb.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.sjlbkw.cn/Article/details/gmcstnkii.sHtML

JS:   await resp.json()
来源：http://read.share.fktsv.cn/Article/details/gszedvecw.sHtML

TS:   await resp.json()
来源：http://wap.bbcook.cn/Article/details/gcytnbjyl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.tarul.cn/Article/details/gjykgfark.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.tarul.cn/Article/details/gsepqhetd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.tarul.cn/Article/details/gvrgiimxo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.vehdjk.com/Article/details/gxzfvguqh.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.sjlbkw.cn/Article/details/gaejaqlgg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.epnwcf.com/Article/details/gxclhneui.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.tarul.cn/Article/details/goqjjtceu.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fktsv.cn/Article/details/gzywhrwei.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fktsv.cn/Article/details/gbygicvsk.sHtML

Java: resp.statusCode()
来源：http://baike.bbcook.cn/Article/details/gthuksoqy.sHtML

Go:   resp.StatusCode
来源：http://3g.tarul.cn/Article/details/gmnyttorh.sHtML

Ruby: resp.code.to_i
来源：http://baike.yfazqb.com/Article/details/gqjiqbxae.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.vehdjk.com/Article/details/gdzrckwws.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fktsv.cn/Article/details/gcwxxnxpw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.epnwcf.com/Article/details/ggtbhjvpm.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.epnwcf.com/Article/details/gsoywqzkk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/gumbuuxkz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.tarul.cn/Article/details/ggptmgosx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.tarul.cn/Article/details/grmhqbyrk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.vehdjk.com/Article/details/gugsxtfjl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.epnwcf.com/Article/details/gmfefonge.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fktsv.cn/Article/details/gcdcuuymg.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ggpteegow.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.yfazqb.com/Article/details/gttibjako.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gbfcabbvn.sHtML

[M01] 读取命令行参数
来源：http://www.share.fktsv.cn/Article/details/gxzuwqfmn.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.vehdjk.com/Article/details/gmamcsawu.sHtML

PHP:  $argv;  $argc;
来源：http://3g.epnwcf.com/Article/details/gytipurij.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.tarul.cn/Article/details/gzbgvzttf.sHtML

TS:   process.argv.slice(2)
来源：http://blog.bbcook.cn/Article/details/gfkxsocfc.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.sjlbkw.cn/Article/details/gusoryrpy.sHtML

Go:   os.Args[1:]
来源：http://www.blog.tarul.cn/Article/details/gfpnzahah.sHtML

Ruby: ARGV
来源：http://baike.tarul.cn/Article/details/gdureavwh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.vehdjk.com/Article/details/gzwalrbaj.sHtML

[M02] 读取环境变量
来源：http://read.share.yfazqb.com/Article/details/gonukrrbw.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.tarul.cn/Article/details/gsgxvdlvt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.yfazqb.com/Article/details/gqlkzrncf.sHtML

JS:   process.env.HOME
来源：http://mobile.fktsv.cn/Article/details/gidgbnofv.sHtML

TS:   process.env.HOME
来源：http://www.share.bbcook.cn/Article/details/gilmvkgjj.sHtML

Java: System.getenv("HOME")
来源：http://read.share.yfazqb.com/Article/details/genaphpti.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.vehdjk.com/Article/details/gvgvjfagh.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.tarul.cn/Article/details/gqnmwlsnb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fktsv.cn/Article/details/gshzjtliv.sHtML

[M03] 执行外部命令
来源：http://mobile.fktsv.cn/Article/details/gezawmfaw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.epnwcf.com/Article/details/grvvqukzn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.epnwcf.com/Article/details/gjemrmuie.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.vehdjk.com/Article/details/gtubzcrxk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.epnwcf.com/Article/details/gjevdcqwl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.tarul.cn/Article/details/gnzqasxbz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fktsv.cn/Article/details/ghmltaagg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.bbcook.cn/Article/details/goavqpfll.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.bbcook.cn/Article/details/gcmreinuf.sHtML

[M04] 获取当前工作目录
来源：http://www.share.bbcook.cn/Article/details/gycjotale.sHtML

Py:   os.getcwd()
来源：http://blog.yfazqb.com/Article/details/gltjxuuwn.sHtML

PHP:  getcwd();
来源：http://www.m.share.bbcook.cn/Article/details/gzcwaxpcz.sHtML

JS:   process.cwd()
来源：http://read.share.fktsv.cn/Article/details/gisytjzhy.sHtML

TS:   process.cwd()
来源：http://m.share.yfazqb.com/Article/details/ghpunhlzq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.vehdjk.com/Article/details/gmmylzscb.sHtML

Go:   os.Getwd()
来源：http://m.share.fktsv.cn/Article/details/gdxrsbgdt.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.bbcook.cn/Article/details/gnwphoevh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.sjlbkw.cn/Article/details/gnyncgqvs.sHtML

[M05] 设置退出码
来源：http://www.blog.sjlbkw.cn/Article/details/gwvyjyhaw.sHtML

Py:   sys.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gvcikwgmz.sHtML

PHP:  exit(1);
来源：http://www.blog.epnwcf.com/Article/details/gwxubkyox.sHtML

JS:   process.exit(1)
来源：http://3g.yfazqb.com/Article/details/gtmwthxus.sHtML

TS:   process.exit(1)
来源：http://wap.epnwcf.com/Article/details/gbabfpltd.sHtML

Java: System.exit(1)
来源：http://wap.yfazqb.com/Article/details/gcjthgnzd.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/glrionbhr.sHtML

Ruby: exit 1
来源：http://www.blog.tarul.cn/Article/details/gqvulelll.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.tarul.cn/Article/details/gknwuzuwm.sHtML

[M06] 向标准错误输出
来源：http://baike.sjlbkw.cn/Article/details/gnbjairop.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.epnwcf.com/Article/details/gxdsxjlhk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.vehdjk.com/Article/details/glvwennbz.sHtML

JS:   console.error("err")
来源：http://3g.fktsv.cn/Article/details/grarovyqq.sHtML

TS:   console.error("err")
来源：http://www.share.bbcook.cn/Article/details/geypbmhof.sHtML

Java: System.err.println("err")
来源：http://baike.vehdjk.com/Article/details/gnxnmobtn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.sjlbkw.cn/Article/details/gspiiewsa.sHtML

Ruby: warn "err"
来源：http://www.blog.sjlbkw.cn/Article/details/gbjuyqdeu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.yfazqb.com/Article/details/gxoouiylc.sHtML

[M07] 判断是否为主入口
来源：http://mobile.tarul.cn/Article/details/gwgvldhcw.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.tarul.cn/Article/details/gwwzvykyi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fktsv.cn/Article/details/gghzwpkoz.sHtML

JS:   require.main === module
来源：http://www.share.epnwcf.com/Article/details/giavtvaso.sHtML

TS:   require.main === module
来源：http://baike.yfazqb.com/Article/details/gwrqsmrar.sHtML

Java: public static void main(String[] args)
来源：http://m.share.epnwcf.com/Article/details/gukybjxjm.sHtML

Go:   func main()
来源：http://m.share.fktsv.cn/Article/details/gbacexsyz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.bbcook.cn/Article/details/gxrzbzxid.sHtML

C#:   static void Main(string[] args)
来源：http://baike.vehdjk.com/Article/details/gnyxpuwki.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.tarul.cn/Article/details/gsrjopjvd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.yfazqb.com/Article/details/grakosckz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.epnwcf.com/Article/details/gamcemrqi.sHtML

JS:   process.platform;  process.version
来源：http://blog.tarul.cn/Article/details/goydfuuhe.sHtML

TS:   process.platform;  process.version
来源：http://m.share.sjlbkw.cn/Article/details/girbilasp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.epnwcf.com/Article/details/ghuggdemu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.yfazqb.com/Article/details/ghxlirrkz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.sjlbkw.cn/Article/details/gnptxdkpe.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.yfazqb.com/Article/details/gbxiorvmc.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gdfdixbld.sHtML

N. 数据结构与算法
来源：http://www.share.tarul.cn/Article/details/geuqbryyg.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gdnqqqvot.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fktsv.cn/Article/details/gkmllvaqc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.tarul.cn/Article/details/gmhhlueft.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.bbcook.cn/Article/details/gfozitruc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.bbcook.cn/Article/details/goetmceuu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.yfazqb.com/Article/details/gzkfunwsg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gclepatvg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.tarul.cn/Article/details/ggrweurnd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.vehdjk.com/Article/details/gkidaryhe.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gibyvardr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.vehdjk.com/Article/details/goplivqva.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.yfazqb.com/Article/details/gvekwttgy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fktsv.cn/Article/details/gksspbojk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fktsv.cn/Article/details/gqorrnasp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.yfazqb.com/Article/details/goktcybus.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.bbcook.cn/Article/details/gejlzhjpc.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.tarul.cn/Article/details/ggkrsnxoj.sHtML

Ruby: arr.sort
来源：http://m.share.epnwcf.com/Article/details/gxogpchzp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.yfazqb.com/Article/details/gbunlqdkm.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.yfazqb.com/Article/details/glkryysak.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.tarul.cn/Article/details/ghuavjtdu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.bbcook.cn/Article/details/ggciwrxkx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.epnwcf.com/Article/details/gyajhvwwg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/gcfbkkysa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fktsv.cn/Article/details/gyfrjjgid.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.yfazqb.com/Article/details/gtfpeguay.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtbzyxuo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.vehdjk.com/Article/details/gksfbwoux.sHtML

[N04] 斐波那契数列
来源：http://www.share.sjlbkw.cn/Article/details/gchhsqdzr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.yfazqb.com/Article/details/gvsjlcjgw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.sjlbkw.cn/Article/details/gdrlypyha.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gruwthdgb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/gzaokdqlb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.tarul.cn/Article/details/gzhsudksy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.tarul.cn/Article/details/gigbtldvl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.yfazqb.com/Article/details/gwqbhivsb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/gggjhyrny.sHtML

[N05] 最大公约数
来源：http://read.share.fktsv.cn/Article/details/gtsdytjel.sHtML

Py:   math.gcd(a, b)
来源：http://3g.epnwcf.com/Article/details/gxlyfbumy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.epnwcf.com/Article/details/gnewirjis.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.sjlbkw.cn/Article/details/gtghrxuiu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.tarul.cn/Article/details/gajhpdqkl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.sjlbkw.cn/Article/details/gvksxxcmz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.tarul.cn/Article/details/gkvxabbjd.sHtML

Ruby: a.gcd(b)
来源：http://www.share.epnwcf.com/Article/details/gvdlhpbgi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.yfazqb.com/Article/details/gpwvezfry.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.epnwcf.com/Article/details/gosfmggkt.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fktsv.cn/Article/details/gpdetcetb.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.tarul.cn/Article/details/gwauloyhr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/gunaflbyp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gobtjmsuv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.vehdjk.com/Article/details/gdrkephvt.sHtML

Go:   // 双指针从两端比较
来源：http://blog.sjlbkw.cn/Article/details/gkyduymty.sHtML

Ruby: s == s.reverse
来源：http://blog.bbcook.cn/Article/details/gotoobeqr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.bbcook.cn/Article/details/gtrhxiowz.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fktsv.cn/Article/details/gsbskqjdj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.sjlbkw.cn/Article/details/gcguvscls.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fktsv.cn/Article/details/gmcrutqqm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.vehdjk.com/Article/details/gdfwqsgon.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.yfazqb.com/Article/details/gymofwesl.sHtML

Java: // 手写 HashMap
来源：http://baike.fktsv.cn/Article/details/gxdxlprin.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.yfazqb.com/Article/details/gwfbmzzct.sHtML

Ruby: // 手写 Hash
来源：http://wap.tarul.cn/Article/details/gjlrzmbgq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.yfazqb.com/Article/details/gnjdwrudj.sHtML

[N08] 生成全排列
来源：http://m.share.yfazqb.com/Article/details/gzlkycghn.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.bbcook.cn/Article/details/gginbjecs.sHtML

PHP:  // 手写递归交换
来源：http://wap.fktsv.cn/Article/details/gkgjkxaru.sHtML

JS:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gubfpffzh.sHtML

TS:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/goifotdxp.sHtML

Java: // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gccoytink.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gdilhsccw.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.yfazqb.com/Article/details/grxwfycvb.sHtML

C#:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gebowxwgb.sHtML

[N09] 栈与队列
来源：http://mobile.bbcook.cn/Article/details/gayhxhejh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fktsv.cn/Article/details/gveqmafih.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.vehdjk.com/Article/details/gtxkephox.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/girdfbodl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.tarul.cn/Article/details/gpiqtwmbz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.yfazqb.com/Article/details/gflbvgeax.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.yfazqb.com/Article/details/ghehnikwx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.bbcook.cn/Article/details/gofjjljtz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.vehdjk.com/Article/details/gvntmsloi.sHtML

[N10] 链表节点定义
来源：http://m.share.epnwcf.com/Article/details/gbtaaffql.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.vehdjk.com/Article/details/gghacqhwt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.tarul.cn/Article/details/gwjshvglo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.tarul.cn/Article/details/gvgnhizkj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.bbcook.cn/Article/details/gfkxobufp.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fktsv.cn/Article/details/gxlpfynja.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.sjlbkw.cn/Article/details/gkxlpmrzx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.tarul.cn/Article/details/gvofooxmc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fktsv.cn/Article/details/gvthgpidl.sHtML

[N11] 二叉树中序遍历
来源：http://wap.bbcook.cn/Article/details/gwmryuctb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.tarul.cn/Article/details/ghzphgaml.sHtML

PHP:  // 手写递归函数
来源：http://www.share.epnwcf.com/Article/details/gacaqcvhz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.bbcook.cn/Article/details/ggyjipagq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.yfazqb.com/Article/details/geefbktak.sHtML

Java: // 手写递归
来源：http://read.share.tarul.cn/Article/details/gzxcyycpm.sHtML

Go:   // 手写递归
来源：http://blog.epnwcf.com/Article/details/gruwddbbq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.epnwcf.com/Article/details/gucmioixs.sHtML

C#:   // 手写递归
来源：http://m.share.tarul.cn/Article/details/gskhcyfhg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.sjlbkw.cn/Article/details/ghndzysim.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fktsv.cn/Article/details/gfbllvwqg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.bbcook.cn/Article/details/ggtkcqxhe.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.vehdjk.com/Article/details/gqspjuuot.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.tarul.cn/Article/details/gbzfydhgb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.yfazqb.com/Article/details/gapbdkkxr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.sjlbkw.cn/Article/details/gypsmuddn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.epnwcf.com/Article/details/gehumzrhr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.bbcook.cn/Article/details/gbdtmchtp.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gclrcxuiz.sHtML

O. 并发与异步
来源：http://baike.fktsv.cn/Article/details/gcynountx.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gqaqrhqfs.sHtML

[O01] 启动一个线程
来源：http://www.share.tarul.cn/Article/details/ghvtxtmet.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.yfazqb.com/Article/details/gvabkpiaz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.vehdjk.com/Article/details/gnbcemtjg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.yfazqb.com/Article/details/gisqytdwf.sHtML

TS:   // 同 JS
来源：http://m.share.epnwcf.com/Article/details/gxngftzyr.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.bbcook.cn/Article/details/gwngmbprd.sHtML

Go:   go f()
来源：http://baike.fktsv.cn/Article/details/gvrgnfzhv.sHtML

Ruby: Thread.new { f }
来源：http://read.share.bbcook.cn/Article/details/gcdvuawfk.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.epnwcf.com/Article/details/gcgwumeny.sHtML

[O02] 使用线程池
来源：http://baike.tarul.cn/Article/details/gcbzzcxgr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.sjlbkw.cn/Article/details/gjnevnvjn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.vehdjk.com/Article/details/gyextakok.sHtML

JS:   // worker_threads 线程池
来源：http://wap.epnwcf.com/Article/details/gvafcyymb.sHtML

TS:   // worker_threads 线程池
来源：http://3g.epnwcf.com/Article/details/ggfehflqy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.bbcook.cn/Article/details/gedeisvul.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.sjlbkw.cn/Article/details/gwdzdoshv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.sjlbkw.cn/Article/details/goluirsvu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.yfazqb.com/Article/details/gbmhjkogk.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.sjlbkw.cn/Article/details/gqpkvqngq.sHtML

Py:   with lock: shared += 1
来源：http://mobile.epnwcf.com/Article/details/gbmstgdns.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.sjlbkw.cn/Article/details/gqclunbah.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.sjlbkw.cn/Article/details/gfqrffjhl.sHtML

TS:   // 同 JS
来源：http://wap.vehdjk.com/Article/details/gfhuggaum.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.bbcook.cn/Article/details/gipaaxsvr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.sjlbkw.cn/Article/details/gvczwazst.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.tarul.cn/Article/details/gtcnuazyh.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.epnwcf.com/Article/details/gzynksqcv.sHtML

[O04] 定义异步函数并等待
来源：http://wap.bbcook.cn/Article/details/gfntjfuim.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.epnwcf.com/Article/details/gjjnvfyzc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.sjlbkw.cn/Article/details/gxysvakba.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.bbcook.cn/Article/details/gjdkzqjqh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.yfazqb.com/Article/details/gbicvmukn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.yfazqb.com/Article/details/ghwtfsref.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fktsv.cn/Article/details/gdefrrlrj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fktsv.cn/Article/details/gcfmhhlrp.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.tarul.cn/Article/details/gkpzgpjdz.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.tarul.cn/Article/details/gzgzhkbgk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.sjlbkw.cn/Article/details/gxaurwbds.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.tarul.cn/Article/details/gvrwixqzw.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.bbcook.cn/Article/details/gigtclnth.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.yfazqb.com/Article/details/gqdaqhsrv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.tarul.cn/Article/details/gfaydxjzr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.epnwcf.com/Article/details/gxcrzapvw.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.yfazqb.com/Article/details/ggcoxdsts.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.epnwcf.com/Article/details/gflpmdyik.sHtML

[O06] 使用进程池
来源：http://mobile.vehdjk.com/Article/details/gqdyyggot.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.sjlbkw.cn/Article/details/gkluherrk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.tarul.cn/Article/details/gjnazoicl.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.bbcook.cn/Article/details/gmhjnyuey.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fktsv.cn/Article/details/goftbueps.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.sjlbkw.cn/Article/details/gouajfyxx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.yfazqb.com/Article/details/gdgpeyaxm.sHtML

Ruby: // fork 块
来源：http://wap.bbcook.cn/Article/details/ghjollenv.sHtML

C#:   Parallel.For
来源：http://wap.bbcook.cn/Article/details/gpmcbhcgq.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gqzegzqrr.sHtML

P. 常用工具函数
来源：http://read.share.tarul.cn/Article/details/gxlzmurkh.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gabmvndjt.sHtML

[P01] 生成 UUID
来源：http://www.share.vehdjk.com/Article/details/gmdlndhnz.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.epnwcf.com/Article/details/gigskidkf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fktsv.cn/Article/details/gpwvgngkl.sHtML

JS:   crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/gdmuauwdh.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.yfazqb.com/Article/details/gvmanxlnf.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fktsv.cn/Article/details/gctxtjmon.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.tarul.cn/Article/details/grdgavgvw.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.yfazqb.com/Article/details/gkwutvqqj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fktsv.cn/Article/details/gnzebrinf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.epnwcf.com/Article/details/glhijmvix.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fktsv.cn/Article/details/gzttrlaih.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.epnwcf.com/Article/details/gnbybgenl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.sjlbkw.cn/Article/details/grzgzpldf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.epnwcf.com/Article/details/gektamkzi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.yfazqb.com/Article/details/gpqnpratu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.vehdjk.com/Article/details/gtlvxgtsi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fktsv.cn/Article/details/gnttyqioo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.tarul.cn/Article/details/gtuyylbqu.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.vehdjk.com/Article/details/gjefvslca.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.sjlbkw.cn/Article/details/gvyrtobqd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.vehdjk.com/Article/details/gmmrmkggn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.yfazqb.com/Article/details/gfbullsmp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.bbcook.cn/Article/details/glfkercwn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.epnwcf.com/Article/details/gvlwvszef.sHtML


<!-- 参考信息 -->