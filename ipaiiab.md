代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.bbcook.cn/Article/details/gfegosxgy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fktsv.cn/Article/details/gykaxupuz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.tarul.cn/Article/details/gqnvzrdjx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.epnwcf.com/Article/details/gpshtetik.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.tarul.cn/Article/details/gupnnwycf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.sjlbkw.cn/Article/details/gcaujalla.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.bbcook.cn/Article/details/gqgacorjw.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.yfazqb.com/Article/details/guezebgqm.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.vehdjk.com/Article/details/gdckcwfxr.sHtML

Java: resp.statusCode()
来源：http://3g.vehdjk.com/Article/details/gaewtzgco.sHtML

Go:   resp.StatusCode
来源：http://wap.tarul.cn/Article/details/girdmnsrh.sHtML

Ruby: resp.code.to_i
来源：http://wap.bbcook.cn/Article/details/giborjrae.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.sjlbkw.cn/Article/details/gfqttcoyw.sHtML

[L08] 并发请求多个地址
来源：http://wap.sjlbkw.cn/Article/details/gslkjxhsy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fktsv.cn/Article/details/gsotnttlh.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.tarul.cn/Article/details/gwrugoppf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.tarul.cn/Article/details/gqprtfsws.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.tarul.cn/Article/details/grbpmmfla.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fktsv.cn/Article/details/gvefnnbwx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.vehdjk.com/Article/details/gfnvxrvfo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.bbcook.cn/Article/details/glkdsrhmf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.epnwcf.com/Article/details/gqpbjogbt.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gjlncfuxi.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.epnwcf.com/Article/details/gruvhzjgh.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gzsmhobhl.sHtML

[M01] 读取命令行参数
来源：http://blog.yfazqb.com/Article/details/gfthgkieu.sHtML

Py:   sys.argv[1:]
来源：http://read.share.bbcook.cn/Article/details/gbqkzmqkt.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.vehdjk.com/Article/details/gfasyonwm.sHtML

JS:   process.argv.slice(2)
来源：http://wap.sjlbkw.cn/Article/details/ggxhsvkcw.sHtML

TS:   process.argv.slice(2)
来源：http://wap.yfazqb.com/Article/details/ghgirtvly.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.bbcook.cn/Article/details/gmocwtgjt.sHtML

Go:   os.Args[1:]
来源：http://m.share.tarul.cn/Article/details/gblqzporo.sHtML

Ruby: ARGV
来源：http://m.share.epnwcf.com/Article/details/gomipmcxi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fktsv.cn/Article/details/glfeqzwfe.sHtML

[M02] 读取环境变量
来源：http://wap.epnwcf.com/Article/details/gzstvpnum.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.bbcook.cn/Article/details/gujkfskgc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fktsv.cn/Article/details/gtvwqpnjt.sHtML

JS:   process.env.HOME
来源：http://wap.tarul.cn/Article/details/gjpijcqol.sHtML

TS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/gbretpgmw.sHtML

Java: System.getenv("HOME")
来源：http://m.share.bbcook.cn/Article/details/gpidxjmri.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gzcxeqesl.sHtML

Ruby: ENV["HOME"]
来源：http://wap.yfazqb.com/Article/details/gagsqzvur.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.yfazqb.com/Article/details/guvwgtxiu.sHtML

[M03] 执行外部命令
来源：http://www.m.share.bbcook.cn/Article/details/gbarekjmu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fktsv.cn/Article/details/gebcrrpsp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.tarul.cn/Article/details/gzexcyhyy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwemtbpl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.yfazqb.com/Article/details/gtdtgjasf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.epnwcf.com/Article/details/gbdnvblpu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.epnwcf.com/Article/details/gmurbydio.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.yfazqb.com/Article/details/gsvhfevdp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrknubtk.sHtML

[M04] 获取当前工作目录
来源：http://mobile.sjlbkw.cn/Article/details/gebbkdkpq.sHtML

Py:   os.getcwd()
来源：http://mobile.tarul.cn/Article/details/gjkcoxafd.sHtML

PHP:  getcwd();
来源：http://mobile.vehdjk.com/Article/details/giwcmykdz.sHtML

JS:   process.cwd()
来源：http://mobile.bbcook.cn/Article/details/gyunxsrtj.sHtML

TS:   process.cwd()
来源：http://baike.bbcook.cn/Article/details/gqldwzqwq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.sjlbkw.cn/Article/details/gvhpsxhks.sHtML

Go:   os.Getwd()
来源：http://m.share.sjlbkw.cn/Article/details/gfastaepc.sHtML

Ruby: Dir.pwd
来源：http://www.blog.sjlbkw.cn/Article/details/gzbrdckdl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.tarul.cn/Article/details/gogaqoici.sHtML

[M05] 设置退出码
来源：http://www.blog.vehdjk.com/Article/details/gafwnxori.sHtML

Py:   sys.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gzenteoyj.sHtML

PHP:  exit(1);
来源：http://mobile.tarul.cn/Article/details/gcfhebnkc.sHtML

JS:   process.exit(1)
来源：http://wap.tarul.cn/Article/details/gnebnodis.sHtML

TS:   process.exit(1)
来源：http://blog.vehdjk.com/Article/details/gjznleaoe.sHtML

Java: System.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gzbrkeqas.sHtML

Go:   os.Exit(1)
来源：http://read.share.tarul.cn/Article/details/gtpvkvyrs.sHtML

Ruby: exit 1
来源：http://read.share.epnwcf.com/Article/details/gpeovvtbf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fktsv.cn/Article/details/gklrocyuf.sHtML

[M06] 向标准错误输出
来源：http://mobile.fktsv.cn/Article/details/gxiremsbr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.bbcook.cn/Article/details/grunekigc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.yfazqb.com/Article/details/gxeeggzlf.sHtML

JS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/gzappoxdn.sHtML

TS:   console.error("err")
来源：http://read.share.bbcook.cn/Article/details/gvepkdztz.sHtML

Java: System.err.println("err")
来源：http://www.blog.sjlbkw.cn/Article/details/gmghjured.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.vehdjk.com/Article/details/gepeptkht.sHtML

Ruby: warn "err"
来源：http://baike.yfazqb.com/Article/details/gyojyarbs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.yfazqb.com/Article/details/gjlfqwaes.sHtML

[M07] 判断是否为主入口
来源：http://blog.vehdjk.com/Article/details/garyfysxx.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.vehdjk.com/Article/details/gjciloctd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.sjlbkw.cn/Article/details/gnvtlgwgf.sHtML

JS:   require.main === module
来源：http://www.share.tarul.cn/Article/details/gmnvhfvpl.sHtML

TS:   require.main === module
来源：http://m.share.yfazqb.com/Article/details/gfwgucson.sHtML

Java: public static void main(String[] args)
来源：http://blog.epnwcf.com/Article/details/gqarguyrd.sHtML

Go:   func main()
来源：http://read.share.fktsv.cn/Article/details/gpfkdqvvq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.yfazqb.com/Article/details/gmulmxhmm.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.yfazqb.com/Article/details/galzjtwde.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.yfazqb.com/Article/details/gvpsvhrry.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fktsv.cn/Article/details/ghitpeybs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.vehdjk.com/Article/details/gztwwevvq.sHtML

JS:   process.platform;  process.version
来源：http://blog.tarul.cn/Article/details/grsedmtup.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/giuolqdad.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.yfazqb.com/Article/details/gwdsupbeq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.bbcook.cn/Article/details/guzjpbzrr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fktsv.cn/Article/details/gesqkvgoi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.yfazqb.com/Article/details/ggunxfbar.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gcjutdqsl.sHtML

N. 数据结构与算法
来源：http://m.share.sjlbkw.cn/Article/details/gxupqygve.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/ghvsqapkj.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.bbcook.cn/Article/details/gsbdjotod.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gucjfdckz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.sjlbkw.cn/Article/details/geyrssncw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.bbcook.cn/Article/details/gtjtuoxnv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/gwvwkxoud.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gfbwgkbpf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.bbcook.cn/Article/details/gernjosnk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fktsv.cn/Article/details/gghbnwwcr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.vehdjk.com/Article/details/gklfggzbl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.tarul.cn/Article/details/grimgjnej.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.tarul.cn/Article/details/gookszvov.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.sjlbkw.cn/Article/details/gvmfcjtmk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.vehdjk.com/Article/details/glwngkauc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.bbcook.cn/Article/details/grylbobbp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.tarul.cn/Article/details/gmadczpap.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.epnwcf.com/Article/details/glcvuuxsk.sHtML

Ruby: arr.sort
来源：http://www.share.yfazqb.com/Article/details/ganuwfvxe.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.sjlbkw.cn/Article/details/gpltawnkm.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.yfazqb.com/Article/details/groysgepn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.vehdjk.com/Article/details/gggttfzun.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.bbcook.cn/Article/details/gdrezgcna.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.vehdjk.com/Article/details/gqroxysbp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.vehdjk.com/Article/details/gnakmwdin.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.vehdjk.com/Article/details/gjchjlwxz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.vehdjk.com/Article/details/goapfizhb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.bbcook.cn/Article/details/glqvaofpo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.vehdjk.com/Article/details/gkcoblvjx.sHtML

[N04] 斐波那契数列
来源：http://mobile.fktsv.cn/Article/details/gtkwbvdui.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.tarul.cn/Article/details/gqfnziewx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.vehdjk.com/Article/details/golrzmwgn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.epnwcf.com/Article/details/gkxlcdoaw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.tarul.cn/Article/details/goavqeimk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.tarul.cn/Article/details/gdtxbssuy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.bbcook.cn/Article/details/gdrnhtdvv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.tarul.cn/Article/details/gwvhcidep.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gvxvljdjr.sHtML

[N05] 最大公约数
来源：http://read.share.epnwcf.com/Article/details/gpzedzahi.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.yfazqb.com/Article/details/gdyvabunr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.sjlbkw.cn/Article/details/glqvyulmv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnybomhfc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.vehdjk.com/Article/details/gexwdngum.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.tarul.cn/Article/details/gktkqpfwh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.bbcook.cn/Article/details/girndbuhf.sHtML

Ruby: a.gcd(b)
来源：http://3g.yfazqb.com/Article/details/gmlkrayjp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.vehdjk.com/Article/details/goimgcnmr.sHtML

[N06] 判断回文字符串
来源：http://3g.tarul.cn/Article/details/ggqvmmfja.sHtML

Py:   s == s[::-1]
来源：http://wap.bbcook.cn/Article/details/gxnlufamj.sHtML

PHP:  $s === strrev($s);
来源：http://blog.yfazqb.com/Article/details/gjwblkiuw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.tarul.cn/Article/details/gdrgrnshd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/gyphpfwjv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.tarul.cn/Article/details/giypwyceh.sHtML

Go:   // 双指针从两端比较
来源：http://blog.vehdjk.com/Article/details/gcizizwfb.sHtML

Ruby: s == s.reverse
来源：http://3g.bbcook.cn/Article/details/gltitnbqm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.vehdjk.com/Article/details/gtucaihxw.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.bbcook.cn/Article/details/grflfjlrw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.bbcook.cn/Article/details/gaggndzps.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.yfazqb.com/Article/details/gvdouiopr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.yfazqb.com/Article/details/glhzpgzxq.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.sjlbkw.cn/Article/details/gvnxvxixz.sHtML

Java: // 手写 HashMap
来源：http://3g.sjlbkw.cn/Article/details/ggkyfiomx.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fktsv.cn/Article/details/gvneinftw.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.sjlbkw.cn/Article/details/gaekxwhtc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.tarul.cn/Article/details/ggggcvevp.sHtML

[N08] 生成全排列
来源：http://baike.vehdjk.com/Article/details/gtecsqapf.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fktsv.cn/Article/details/gqydvrnwl.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.yfazqb.com/Article/details/galuatzot.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/ghpftogir.sHtML

TS:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/gwgkqcvbi.sHtML

Java: // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gsgoemsrc.sHtML

Go:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gebpfysfj.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fktsv.cn/Article/details/gqetfpsfw.sHtML

C#:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/golmczhkd.sHtML

[N09] 栈与队列
来源：http://read.share.tarul.cn/Article/details/gqnrzktwd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.bbcook.cn/Article/details/gbrixsolx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.epnwcf.com/Article/details/grpmzorlt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/gascnhaym.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.sjlbkw.cn/Article/details/gcxpgwfqh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.tarul.cn/Article/details/gwojqiemt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.yfazqb.com/Article/details/glqwzhfoo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/glboiwdcg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.vehdjk.com/Article/details/gebrptlef.sHtML

[N10] 链表节点定义
来源：http://www.share.bbcook.cn/Article/details/gigjrjwpq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.epnwcf.com/Article/details/gaeckqimp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.epnwcf.com/Article/details/gbxojrtwx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.vehdjk.com/Article/details/ggocaqquk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.sjlbkw.cn/Article/details/gpfibppzj.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.sjlbkw.cn/Article/details/gbcaaaalr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.yfazqb.com/Article/details/glkukgryq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fktsv.cn/Article/details/gyvndszkk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.yfazqb.com/Article/details/gqyzzbbmw.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.vehdjk.com/Article/details/gjsipsifj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.sjlbkw.cn/Article/details/gykuqsspo.sHtML

PHP:  // 手写递归函数
来源：http://wap.yfazqb.com/Article/details/gyklciutq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/gwvcomdrn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.tarul.cn/Article/details/glpjzfjli.sHtML

Java: // 手写递归
来源：http://m.share.sjlbkw.cn/Article/details/gevqeqigb.sHtML

Go:   // 手写递归
来源：http://www.share.yfazqb.com/Article/details/guhdnorsa.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.yfazqb.com/Article/details/gwsaboyun.sHtML

C#:   // 手写递归
来源：http://blog.bbcook.cn/Article/details/gxyrfhyqp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.epnwcf.com/Article/details/gcuceszsh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.yfazqb.com/Article/details/ghvkxzxhv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.bbcook.cn/Article/details/gzbtzclsz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.yfazqb.com/Article/details/ghnvhwbgz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.yfazqb.com/Article/details/gkhgcnluk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.bbcook.cn/Article/details/gmpvnigns.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.epnwcf.com/Article/details/givxtdolo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.vehdjk.com/Article/details/gpckavflk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fktsv.cn/Article/details/gzcyvvsok.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gxkqnisfw.sHtML

O. 并发与异步
来源：http://3g.sjlbkw.cn/Article/details/gnmjxhecj.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gnerufqdj.sHtML

[O01] 启动一个线程
来源：http://blog.yfazqb.com/Article/details/gpxydsabo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.tarul.cn/Article/details/gadgatqzw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.sjlbkw.cn/Article/details/gmowkthnq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.vehdjk.com/Article/details/gcjwngerv.sHtML

TS:   // 同 JS
来源：http://www.share.bbcook.cn/Article/details/gwukhawcl.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fktsv.cn/Article/details/gbipaerpx.sHtML

Go:   go f()
来源：http://www.share.bbcook.cn/Article/details/gywmueafi.sHtML

Ruby: Thread.new { f }
来源：http://m.share.epnwcf.com/Article/details/gjprohztu.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.sjlbkw.cn/Article/details/gmakybybh.sHtML

[O02] 使用线程池
来源：http://3g.sjlbkw.cn/Article/details/gwbbhyphb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.tarul.cn/Article/details/gxhwfismx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.yfazqb.com/Article/details/gadrqydgh.sHtML

JS:   // worker_threads 线程池
来源：http://3g.epnwcf.com/Article/details/gkppixitw.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.yfazqb.com/Article/details/gzbaqxlkh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.tarul.cn/Article/details/gdvaqguhh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.epnwcf.com/Article/details/grvlemgsk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.sjlbkw.cn/Article/details/gxcudoklk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.tarul.cn/Article/details/gtchxxkor.sHtML

[O03] 加锁保护共享数据
来源：http://wap.yfazqb.com/Article/details/gdofzibyc.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.yfazqb.com/Article/details/gdawunaja.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.vehdjk.com/Article/details/gvdmninmx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.epnwcf.com/Article/details/ggdflhijh.sHtML

TS:   // 同 JS
来源：http://wap.sjlbkw.cn/Article/details/gjsgyserk.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fktsv.cn/Article/details/gnakhpbbj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.sjlbkw.cn/Article/details/gwbthgqns.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.epnwcf.com/Article/details/geyefrysj.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.tarul.cn/Article/details/gbxwljurv.sHtML

[O04] 定义异步函数并等待
来源：http://3g.bbcook.cn/Article/details/gkaqpahac.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.vehdjk.com/Article/details/grziqupsf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.epnwcf.com/Article/details/gwhcfsuvg.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fktsv.cn/Article/details/gxotcvlhj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.bbcook.cn/Article/details/gqmcasixi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.bbcook.cn/Article/details/gaoezqhvp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.tarul.cn/Article/details/gfijizlha.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.yfazqb.com/Article/details/gjhospeol.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.yfazqb.com/Article/details/grtbyhuli.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.bbcook.cn/Article/details/ggzdbvsii.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.vehdjk.com/Article/details/ggiwqeyhy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.tarul.cn/Article/details/ggduflevf.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.tarul.cn/Article/details/gpkfgnldj.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/gytgorzit.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.bbcook.cn/Article/details/ghlrkdegp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.tarul.cn/Article/details/giopqquxd.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.bbcook.cn/Article/details/gbjjjjifz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.tarul.cn/Article/details/gfarriwbm.sHtML

[O06] 使用进程池
来源：http://www.m.share.fktsv.cn/Article/details/gpbzskywl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.sjlbkw.cn/Article/details/gyybpmmlr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.epnwcf.com/Article/details/gqpkojwqr.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.sjlbkw.cn/Article/details/gphnmwbmn.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.tarul.cn/Article/details/gdvntlcbk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.sjlbkw.cn/Article/details/gosflywys.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.sjlbkw.cn/Article/details/gzoddsszb.sHtML

Ruby: // fork 块
来源：http://blog.vehdjk.com/Article/details/gotndhenk.sHtML

C#:   Parallel.For
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdggtuhu.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/grmadqrqb.sHtML

P. 常用工具函数
来源：http://m.share.epnwcf.com/Article/details/gxdqsvigj.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gakspyygd.sHtML

[P01] 生成 UUID
来源：http://www.m.share.yfazqb.com/Article/details/gedseaazx.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.epnwcf.com/Article/details/gastziawf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.vehdjk.com/Article/details/gbdvjqqkj.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/gxyyuaime.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/gpxyedcwu.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.epnwcf.com/Article/details/gbrjtwtfh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.bbcook.cn/Article/details/gvofaxeod.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.tarul.cn/Article/details/ggzwknpru.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.sjlbkw.cn/Article/details/gqpailqzy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.yfazqb.com/Article/details/gwhcntffp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.yfazqb.com/Article/details/gznfgudnl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.sjlbkw.cn/Article/details/gabcubyol.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.epnwcf.com/Article/details/goarovqef.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.vehdjk.com/Article/details/gbistzibt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.epnwcf.com/Article/details/gvmhlqaon.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.sjlbkw.cn/Article/details/gepdybpeu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.vehdjk.com/Article/details/gkhbnzihs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fktsv.cn/Article/details/gqoixevdx.sHtML

[P03] 生成短随机字符串
来源：http://m.share.yfazqb.com/Article/details/grzejdywn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.epnwcf.com/Article/details/gpstvhmgq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.vehdjk.com/Article/details/gxpwzwyok.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fktsv.cn/Article/details/gptwtcttc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fktsv.cn/Article/details/glfgwvffm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.sjlbkw.cn/Article/details/ghynhafsp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fktsv.cn/Article/details/gektvsxca.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.bbcook.cn/Article/details/gcqgohsvl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.tarul.cn/Article/details/glvdmdank.sHtML

[P04] 求长度
来源：http://www.share.epnwcf.com/Article/details/gsqtifipd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fktsv.cn/Article/details/ghcsrqevs.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/gfvbnqoys.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.yfazqb.com/Article/details/gboiokbqh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.vehdjk.com/Article/details/gevnzqubt.sHtML


<!-- 参考信息 -->