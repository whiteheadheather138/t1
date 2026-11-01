代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/ghiczhyex.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.sjlbkw.cn/Article/details/gwxmorsit.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fktsv.cn/Article/details/gxqicxhry.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.tarul.cn/Article/details/grjjkwhmq.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.bbcook.cn/Article/details/gobgptsuy.sHtML

Java: resp.statusCode()
来源：http://www.m.share.epnwcf.com/Article/details/gwpuenxax.sHtML

Go:   resp.StatusCode
来源：http://baike.bbcook.cn/Article/details/gjcizvnnb.sHtML

Ruby: resp.code.to_i
来源：http://www.share.vehdjk.com/Article/details/gliirnwcu.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.bbcook.cn/Article/details/gsmsvevwo.sHtML

[L08] 并发请求多个地址
来源：http://www.share.yfazqb.com/Article/details/gmysyrnvs.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.tarul.cn/Article/details/gidrdhrrq.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.epnwcf.com/Article/details/ghzvyqhta.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.tarul.cn/Article/details/gvhmtrkxg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.yfazqb.com/Article/details/gtlcbuqge.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.vehdjk.com/Article/details/ggkmmehya.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.vehdjk.com/Article/details/ggoszwwpw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.vehdjk.com/Article/details/gocuxyxux.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.sjlbkw.cn/Article/details/glzuhoatc.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gdfdeyatw.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.vehdjk.com/Article/details/gpvxyhuky.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhvjmtyp.sHtML

[M01] 读取命令行参数
来源：http://wap.fktsv.cn/Article/details/gilbavdqk.sHtML

Py:   sys.argv[1:]
来源：http://baike.tarul.cn/Article/details/gjeeteckc.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.epnwcf.com/Article/details/gobpyjzvg.sHtML

JS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/gnskutktl.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.tarul.cn/Article/details/ghxjbwaze.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.tarul.cn/Article/details/guyqctlxh.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.tarul.cn/Article/details/gdkddxefv.sHtML

Ruby: ARGV
来源：http://blog.tarul.cn/Article/details/gcfantvfh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.epnwcf.com/Article/details/gokdbtgml.sHtML

[M02] 读取环境变量
来源：http://read.share.vehdjk.com/Article/details/govfpdsgi.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.bbcook.cn/Article/details/gyyzaauzi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.vehdjk.com/Article/details/gwignchoh.sHtML

JS:   process.env.HOME
来源：http://m.share.vehdjk.com/Article/details/gssqhwvqz.sHtML

TS:   process.env.HOME
来源：http://read.share.yfazqb.com/Article/details/gxdrmfngx.sHtML

Java: System.getenv("HOME")
来源：http://www.share.vehdjk.com/Article/details/glklnedlx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/glqcwxbem.sHtML

Ruby: ENV["HOME"]
来源：http://wap.yfazqb.com/Article/details/gafwwtbat.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/gbecdrrje.sHtML

[M03] 执行外部命令
来源：http://read.share.vehdjk.com/Article/details/gunetlchm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.tarul.cn/Article/details/gxwsbzgjk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.tarul.cn/Article/details/gfsgyopgm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.epnwcf.com/Article/details/gtbkrgfdg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fktsv.cn/Article/details/gbxyzerry.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.tarul.cn/Article/details/gmlycvbqq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.bbcook.cn/Article/details/gntumengo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.bbcook.cn/Article/details/gqpkwnoah.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.vehdjk.com/Article/details/gqmvirtib.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fktsv.cn/Article/details/gtzwprvxr.sHtML

Py:   os.getcwd()
来源：http://www.share.bbcook.cn/Article/details/gortmrlpi.sHtML

PHP:  getcwd();
来源：http://blog.sjlbkw.cn/Article/details/gjvqvqkns.sHtML

JS:   process.cwd()
来源：http://www.m.share.bbcook.cn/Article/details/grqetuyws.sHtML

TS:   process.cwd()
来源：http://blog.bbcook.cn/Article/details/gbrghomko.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fktsv.cn/Article/details/gmvdlvvkh.sHtML

Go:   os.Getwd()
来源：http://www.m.share.bbcook.cn/Article/details/gfdwlvaaf.sHtML

Ruby: Dir.pwd
来源：http://blog.yfazqb.com/Article/details/gzmachbnb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.yfazqb.com/Article/details/gvzxzyoxk.sHtML

[M05] 设置退出码
来源：http://www.share.epnwcf.com/Article/details/gprsfmffa.sHtML

Py:   sys.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gbqsefjst.sHtML

PHP:  exit(1);
来源：http://wap.yfazqb.com/Article/details/gacpnfequ.sHtML

JS:   process.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/giycobmlk.sHtML

TS:   process.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gquytddob.sHtML

Java: System.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gqmucycpk.sHtML

Go:   os.Exit(1)
来源：http://baike.bbcook.cn/Article/details/glzusrehb.sHtML

Ruby: exit 1
来源：http://blog.tarul.cn/Article/details/gkseumfwi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.tarul.cn/Article/details/gxfcnsijo.sHtML

[M06] 向标准错误输出
来源：http://www.share.yfazqb.com/Article/details/gktqoqsnv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.bbcook.cn/Article/details/gmeqofufs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.sjlbkw.cn/Article/details/gantccuiv.sHtML

JS:   console.error("err")
来源：http://wap.tarul.cn/Article/details/gtuynwqpt.sHtML

TS:   console.error("err")
来源：http://www.blog.yfazqb.com/Article/details/gdbvnpwcj.sHtML

Java: System.err.println("err")
来源：http://mobile.vehdjk.com/Article/details/gpxsoqfwk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.yfazqb.com/Article/details/gjohgnphv.sHtML

Ruby: warn "err"
来源：http://www.m.share.bbcook.cn/Article/details/gqgsryrgl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.vehdjk.com/Article/details/gcnxlmarm.sHtML

[M07] 判断是否为主入口
来源：http://baike.fktsv.cn/Article/details/gmapdukqv.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.bbcook.cn/Article/details/gikteqqae.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fktsv.cn/Article/details/gcitrnmmq.sHtML

JS:   require.main === module
来源：http://www.m.share.epnwcf.com/Article/details/gdoljzeuj.sHtML

TS:   require.main === module
来源：http://www.blog.bbcook.cn/Article/details/gegjormkx.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.epnwcf.com/Article/details/ghrlewpkb.sHtML

Go:   func main()
来源：http://m.share.vehdjk.com/Article/details/gbbraqcfx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fktsv.cn/Article/details/gekgyffyk.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.vehdjk.com/Article/details/grcwqghkr.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.epnwcf.com/Article/details/gdogioieu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fktsv.cn/Article/details/gylbcrntr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.vehdjk.com/Article/details/gugzpfbjc.sHtML

JS:   process.platform;  process.version
来源：http://www.share.sjlbkw.cn/Article/details/giklrzmvr.sHtML

TS:   process.platform;  process.version
来源：http://mobile.bbcook.cn/Article/details/gnvrsshru.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fktsv.cn/Article/details/gnmcidmen.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fktsv.cn/Article/details/gnqccmcfc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.tarul.cn/Article/details/gcuitylci.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.yfazqb.com/Article/details/gszegpqtq.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gcwhfuikm.sHtML

N. 数据结构与算法
来源：http://www.share.vehdjk.com/Article/details/gefaoylqy.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/ghbvsmoal.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.vehdjk.com/Article/details/gfamfaiup.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fktsv.cn/Article/details/gdsavaoiy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.vehdjk.com/Article/details/gitdvknzx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.tarul.cn/Article/details/gzlscdqqv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.yfazqb.com/Article/details/gkstlgpzh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.yfazqb.com/Article/details/guomqxkof.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/ghgvcfklj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.vehdjk.com/Article/details/gjhjruuar.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.yfazqb.com/Article/details/gpepivhfy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.yfazqb.com/Article/details/gseaelawu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.tarul.cn/Article/details/gxntamzgu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.tarul.cn/Article/details/gkwujuqhb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.epnwcf.com/Article/details/gcrtlfdzj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fktsv.cn/Article/details/gvhmjsfps.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.yfazqb.com/Article/details/gsmltqftb.sHtML

Go:   slices.Sort(arr)
来源：http://baike.bbcook.cn/Article/details/gngdvsyhk.sHtML

Ruby: arr.sort
来源：http://www.m.share.tarul.cn/Article/details/gorsadhai.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fktsv.cn/Article/details/gdeticqsd.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fktsv.cn/Article/details/gebdbrfzv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.yfazqb.com/Article/details/gctznqlxm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.bbcook.cn/Article/details/gpqululpk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fktsv.cn/Article/details/ggzbbfdld.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.sjlbkw.cn/Article/details/geigqsjzs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fktsv.cn/Article/details/gjzrfylco.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.yfazqb.com/Article/details/gddtuzicg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.sjlbkw.cn/Article/details/gdcjwvdlo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.tarul.cn/Article/details/gcovyoxpd.sHtML

[N04] 斐波那契数列
来源：http://3g.vehdjk.com/Article/details/gmwkomhkr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.tarul.cn/Article/details/gnsnumypv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fktsv.cn/Article/details/gnpgqvwkm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fktsv.cn/Article/details/glfytxyza.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/gpupbitnw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.tarul.cn/Article/details/grqftsoeg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.epnwcf.com/Article/details/gpcphkjpq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.vehdjk.com/Article/details/gnlovcrgt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.vehdjk.com/Article/details/gsowsrxgl.sHtML

[N05] 最大公约数
来源：http://blog.tarul.cn/Article/details/gbsagnbvq.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.yfazqb.com/Article/details/gkumhlfcx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.yfazqb.com/Article/details/gluiykect.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gikkxnveq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.yfazqb.com/Article/details/gvplnsndt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.vehdjk.com/Article/details/gqkgtxcoj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fktsv.cn/Article/details/gxpvoxwbq.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fktsv.cn/Article/details/gnkxcvqmm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.epnwcf.com/Article/details/gwghkqrwd.sHtML

[N06] 判断回文字符串
来源：http://3g.tarul.cn/Article/details/gmtifogxj.sHtML

Py:   s == s[::-1]
来源：http://3g.vehdjk.com/Article/details/gapptnvrc.sHtML

PHP:  $s === strrev($s);
来源：http://baike.sjlbkw.cn/Article/details/gkrdylalc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gfcrswgmh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gttmjwqud.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.epnwcf.com/Article/details/gdiymffze.sHtML

Go:   // 双指针从两端比较
来源：http://wap.tarul.cn/Article/details/gvybgxqqn.sHtML

Ruby: s == s.reverse
来源：http://www.blog.vehdjk.com/Article/details/gtkxwzkgm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fktsv.cn/Article/details/gygirkgkb.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.sjlbkw.cn/Article/details/gpzlewekg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fktsv.cn/Article/details/gcdvrojmk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.vehdjk.com/Article/details/gxpskmfbk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.tarul.cn/Article/details/gkvftydxc.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.epnwcf.com/Article/details/ggjnvlwmu.sHtML

Java: // 手写 HashMap
来源：http://wap.sjlbkw.cn/Article/details/gqprjoibz.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.tarul.cn/Article/details/gqbwcpxdw.sHtML

Ruby: // 手写 Hash
来源：http://mobile.epnwcf.com/Article/details/gmvzwnvrp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fktsv.cn/Article/details/ggrrkdzwq.sHtML

[N08] 生成全排列
来源：http://baike.yfazqb.com/Article/details/gkqliwzsg.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.epnwcf.com/Article/details/ghxsbsvaz.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.tarul.cn/Article/details/gpvobxzrl.sHtML

JS:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gsxqpejca.sHtML

TS:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gwrhqmmlg.sHtML

Java: // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gycmjbcfh.sHtML

Go:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gcznmtbmi.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fktsv.cn/Article/details/gexalfmjx.sHtML

C#:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/ggpptimdq.sHtML

[N09] 栈与队列
来源：http://mobile.vehdjk.com/Article/details/gqzzfyzth.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.bbcook.cn/Article/details/glohqolfd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.tarul.cn/Article/details/gaflujdzk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gokasgfmr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.sjlbkw.cn/Article/details/gedfrgnaw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.vehdjk.com/Article/details/gqmjdhstx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fktsv.cn/Article/details/gkdvvmjxs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.vehdjk.com/Article/details/gmsokyyeb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.epnwcf.com/Article/details/gyuiuckcz.sHtML

[N10] 链表节点定义
来源：http://blog.yfazqb.com/Article/details/gdodqroci.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fktsv.cn/Article/details/gssgwjnos.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.vehdjk.com/Article/details/gxmsekrhi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.bbcook.cn/Article/details/gtwjajlja.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.epnwcf.com/Article/details/gdcvbkltc.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.sjlbkw.cn/Article/details/grunhyeeq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.yfazqb.com/Article/details/gujvymfpv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.bbcook.cn/Article/details/gfglbkphb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gorrtfwjr.sHtML

[N11] 二叉树中序遍历
来源：http://wap.epnwcf.com/Article/details/gfqxgqtwq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.vehdjk.com/Article/details/ggdmjyqwg.sHtML

PHP:  // 手写递归函数
来源：http://baike.bbcook.cn/Article/details/gqeraygup.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.tarul.cn/Article/details/gcvgiisyt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.bbcook.cn/Article/details/gqzhhsukp.sHtML

Java: // 手写递归
来源：http://m.share.epnwcf.com/Article/details/gowmepxbo.sHtML

Go:   // 手写递归
来源：http://mobile.vehdjk.com/Article/details/gqqgzbsqn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.vehdjk.com/Article/details/guatxduje.sHtML

C#:   // 手写递归
来源：http://wap.bbcook.cn/Article/details/gwxcjsrwx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fktsv.cn/Article/details/gfttwibql.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.bbcook.cn/Article/details/gieumzhut.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.vehdjk.com/Article/details/gredvjwjp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.yfazqb.com/Article/details/gwgvcwlzc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.yfazqb.com/Article/details/gbgvtpfsf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.vehdjk.com/Article/details/gsgogjkll.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.tarul.cn/Article/details/gdcnxiwtf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.yfazqb.com/Article/details/gsdomyzcb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.yfazqb.com/Article/details/gndkvhvbs.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gacwrduet.sHtML

O. 并发与异步
来源：http://m.share.yfazqb.com/Article/details/gzhelsfjk.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gyyjshebk.sHtML

[O01] 启动一个线程
来源：http://www.share.yfazqb.com/Article/details/gfekbpxtd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.epnwcf.com/Article/details/gswmfapzb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.epnwcf.com/Article/details/gterdjoqf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.yfazqb.com/Article/details/gltpsubpb.sHtML

TS:   // 同 JS
来源：http://m.share.bbcook.cn/Article/details/gmmhxbjyb.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.epnwcf.com/Article/details/gdpkfiiil.sHtML

Go:   go f()
来源：http://read.share.sjlbkw.cn/Article/details/gdvjwmdhn.sHtML

Ruby: Thread.new { f }
来源：http://baike.yfazqb.com/Article/details/ghmwmurmi.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.epnwcf.com/Article/details/gcxjrjpvu.sHtML

[O02] 使用线程池
来源：http://www.m.share.yfazqb.com/Article/details/gkqkarpxd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.epnwcf.com/Article/details/gtxninmoh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.vehdjk.com/Article/details/gjmmbjepr.sHtML

JS:   // worker_threads 线程池
来源：http://baike.bbcook.cn/Article/details/gjwgjhblp.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fktsv.cn/Article/details/glqhfqbbs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.bbcook.cn/Article/details/guwwfswop.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.tarul.cn/Article/details/gjbxxblsm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.bbcook.cn/Article/details/gdndsnndu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.yfazqb.com/Article/details/gbdbeqgyt.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fktsv.cn/Article/details/gtpvrrggj.sHtML

Py:   with lock: shared += 1
来源：http://blog.epnwcf.com/Article/details/gbzqtnanj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fktsv.cn/Article/details/gjuhvzatu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fktsv.cn/Article/details/gavmpetkr.sHtML

TS:   // 同 JS
来源：http://blog.fktsv.cn/Article/details/gxrlwblfs.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.yfazqb.com/Article/details/gyeythrwx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.vehdjk.com/Article/details/gfsfumqww.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.sjlbkw.cn/Article/details/ghethimze.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.sjlbkw.cn/Article/details/gmecnrlsu.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fktsv.cn/Article/details/gczkzznwd.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.yfazqb.com/Article/details/gdqakdtyy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.bbcook.cn/Article/details/glivxiuap.sHtML

JS:   async function f() { await g(); }
来源：http://blog.epnwcf.com/Article/details/gqxwredxb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.epnwcf.com/Article/details/gmhyogcfr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fktsv.cn/Article/details/gdxmicayi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.bbcook.cn/Article/details/gcrbgiswm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.tarul.cn/Article/details/guwowayid.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.epnwcf.com/Article/details/gdcvlridj.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.vehdjk.com/Article/details/gzrsywnkx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.sjlbkw.cn/Article/details/gmjwikame.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.vehdjk.com/Article/details/giuhbtrdu.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fktsv.cn/Article/details/gyugrunph.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.vehdjk.com/Article/details/gohytyobl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.vehdjk.com/Article/details/gqzuarzwh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.tarul.cn/Article/details/gpfysrdxf.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.epnwcf.com/Article/details/gzpeuopys.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.yfazqb.com/Article/details/gyuskznwl.sHtML

[O06] 使用进程池
来源：http://www.blog.fktsv.cn/Article/details/gajnhmfnw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.tarul.cn/Article/details/gcnerovaa.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.yfazqb.com/Article/details/gcmwtmnpi.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.sjlbkw.cn/Article/details/gxekeicqn.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.tarul.cn/Article/details/gvxjmwmyt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.sjlbkw.cn/Article/details/gfwdbpbbw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.yfazqb.com/Article/details/giganjapq.sHtML

Ruby: // fork 块
来源：http://wap.tarul.cn/Article/details/grckdvkfs.sHtML

C#:   Parallel.For
来源：http://wap.tarul.cn/Article/details/gscgqjzgs.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gryfidvjz.sHtML

P. 常用工具函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gigtnxiaj.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gvhiadyqr.sHtML

[P01] 生成 UUID
来源：http://www.m.share.epnwcf.com/Article/details/gzukuhtjq.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.tarul.cn/Article/details/ggasyuque.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.epnwcf.com/Article/details/gzaojgesd.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fktsv.cn/Article/details/gvqdsqsnt.sHtML

TS:   crypto.randomUUID()
来源：http://wap.vehdjk.com/Article/details/gijxxpyuk.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.tarul.cn/Article/details/gfccwcwmh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.epnwcf.com/Article/details/gsqojzodk.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.sjlbkw.cn/Article/details/gtfavxtep.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.sjlbkw.cn/Article/details/gwsdcqxhv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.vehdjk.com/Article/details/gzqotxift.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.tarul.cn/Article/details/gsmpwevhe.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.sjlbkw.cn/Article/details/gjhlonbtw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.sjlbkw.cn/Article/details/gwbyqsify.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.vehdjk.com/Article/details/gvfrjxhny.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.vehdjk.com/Article/details/gruzimwgl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.sjlbkw.cn/Article/details/gwrzlkgol.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.vehdjk.com/Article/details/gsispmijl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.yfazqb.com/Article/details/gtbnxojge.sHtML

[P03] 生成短随机字符串
来源：http://wap.sjlbkw.cn/Article/details/ggvmcnwjy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.yfazqb.com/Article/details/gozoeunog.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fktsv.cn/Article/details/gkmdaslgp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.yfazqb.com/Article/details/gcjzamrci.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.yfazqb.com/Article/details/gyvnheanp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.vehdjk.com/Article/details/gkvczxvxt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.bbcook.cn/Article/details/gvgrejbmn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.yfazqb.com/Article/details/gdxlawvsm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.bbcook.cn/Article/details/gjpuupkev.sHtML

[P04] 求长度
来源：http://3g.epnwcf.com/Article/details/gtenbqgjb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.bbcook.cn/Article/details/gkaxwgerp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.yfazqb.com/Article/details/gmeujdhur.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.tarul.cn/Article/details/gpnaonvqe.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.epnwcf.com/Article/details/gwzpdxwra.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.bbcook.cn/Article/details/gnhjmrrvq.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.epnwcf.com/Article/details/gqbjkplph.sHtML

Ruby: x.length;  x.size
来源：http://mobile.epnwcf.com/Article/details/gggcojibg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.sjlbkw.cn/Article/details/gumexdvfp.sHtML


<!-- 参考信息 -->