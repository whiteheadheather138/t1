代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.bbcook.cn/Article/details/gkelefqsi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.sjlbkw.cn/Article/details/glcdhgwmz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.sjlbkw.cn/Article/details/gyshzquxf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.vehdjk.com/Article/details/gmtyzxpek.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fktsv.cn/Article/details/gtxjfbqkx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fktsv.cn/Article/details/gphskjakm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.yfazqb.com/Article/details/goyruppzz.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fktsv.cn/Article/details/gnvrsycsr.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fktsv.cn/Article/details/gdqmvmvxv.sHtML

Java: resp.statusCode()
来源：http://wap.bbcook.cn/Article/details/ghvsmcvox.sHtML

Go:   resp.StatusCode
来源：http://mobile.yfazqb.com/Article/details/ggfdvukxi.sHtML

Ruby: resp.code.to_i
来源：http://wap.epnwcf.com/Article/details/gkccrjxnu.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.sjlbkw.cn/Article/details/gdnshgwnp.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.vehdjk.com/Article/details/gnjbopgrg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fktsv.cn/Article/details/glnbamfep.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.bbcook.cn/Article/details/gxdcczsky.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/gokvksgbj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqzudxky.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.epnwcf.com/Article/details/gygfdpksm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.vehdjk.com/Article/details/gwgwoxhay.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.yfazqb.com/Article/details/gmwgrakgl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.sjlbkw.cn/Article/details/gbcjnaycf.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/ghvukdsts.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.epnwcf.com/Article/details/ghquvxrtd.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gaozldwnw.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.vehdjk.com/Article/details/gufqmjmpn.sHtML

Py:   sys.argv[1:]
来源：http://blog.bbcook.cn/Article/details/gpmjdyhah.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.epnwcf.com/Article/details/gaeuyoesv.sHtML

JS:   process.argv.slice(2)
来源：http://baike.bbcook.cn/Article/details/gmgvirkpc.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.epnwcf.com/Article/details/gkzidunvk.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.sjlbkw.cn/Article/details/gpkguravt.sHtML

Go:   os.Args[1:]
来源：http://read.share.sjlbkw.cn/Article/details/ghrlaydla.sHtML

Ruby: ARGV
来源：http://m.share.yfazqb.com/Article/details/gtibktmne.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.bbcook.cn/Article/details/grpwsizqp.sHtML

[M02] 读取环境变量
来源：http://3g.sjlbkw.cn/Article/details/ghuqdyesg.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gxnayymvs.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.bbcook.cn/Article/details/gwvrblvaj.sHtML

JS:   process.env.HOME
来源：http://read.share.yfazqb.com/Article/details/gngaxtbzj.sHtML

TS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/gnvzzaqec.sHtML

Java: System.getenv("HOME")
来源：http://blog.fktsv.cn/Article/details/gpxgrzkgk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.bbcook.cn/Article/details/gvcxtrhis.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.epnwcf.com/Article/details/gcathvbkz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gjczgpjyf.sHtML

[M03] 执行外部命令
来源：http://baike.sjlbkw.cn/Article/details/gdnabfcfa.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fktsv.cn/Article/details/gevgxqfnv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.vehdjk.com/Article/details/gqejqyrbg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.epnwcf.com/Article/details/gfebnenuz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gybjucrvf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.yfazqb.com/Article/details/glimrhtbh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.vehdjk.com/Article/details/ggbmtccru.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.tarul.cn/Article/details/gmjianpep.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.epnwcf.com/Article/details/gymeqgfgj.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fktsv.cn/Article/details/guhtqkpdf.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fktsv.cn/Article/details/gojepgjwo.sHtML

PHP:  getcwd();
来源：http://3g.bbcook.cn/Article/details/gtulyadwh.sHtML

JS:   process.cwd()
来源：http://baike.sjlbkw.cn/Article/details/gqcbpzabe.sHtML

TS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/gxpsbepaw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.sjlbkw.cn/Article/details/gdqlcqbqk.sHtML

Go:   os.Getwd()
来源：http://m.share.sjlbkw.cn/Article/details/gpqwbnfis.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fktsv.cn/Article/details/gmdbftiku.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.bbcook.cn/Article/details/gzlyaxnem.sHtML

[M05] 设置退出码
来源：http://www.m.share.yfazqb.com/Article/details/grbufgkeo.sHtML

Py:   sys.exit(1)
来源：http://baike.epnwcf.com/Article/details/gcfpsfmqy.sHtML

PHP:  exit(1);
来源：http://blog.bbcook.cn/Article/details/gskekirsl.sHtML

JS:   process.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gwjmwssgq.sHtML

TS:   process.exit(1)
来源：http://blog.vehdjk.com/Article/details/gsnpxouuv.sHtML

Java: System.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gmthnvfnu.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gleewkawl.sHtML

Ruby: exit 1
来源：http://mobile.yfazqb.com/Article/details/guvaepjvl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.epnwcf.com/Article/details/gseaohong.sHtML

[M06] 向标准错误输出
来源：http://3g.tarul.cn/Article/details/gdwfaexnb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.vehdjk.com/Article/details/gdacidvpu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.epnwcf.com/Article/details/guvhsbgsi.sHtML

JS:   console.error("err")
来源：http://www.m.share.epnwcf.com/Article/details/glrkfixye.sHtML

TS:   console.error("err")
来源：http://wap.bbcook.cn/Article/details/ghkkthnjf.sHtML

Java: System.err.println("err")
来源：http://www.share.vehdjk.com/Article/details/glqdvbhrh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.epnwcf.com/Article/details/ganpqytxp.sHtML

Ruby: warn "err"
来源：http://www.share.fktsv.cn/Article/details/gyjmxreid.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.tarul.cn/Article/details/gojvoqigc.sHtML

[M07] 判断是否为主入口
来源：http://3g.tarul.cn/Article/details/gzlwwxnby.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fktsv.cn/Article/details/gteetokqn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.yfazqb.com/Article/details/gnalvylfe.sHtML

JS:   require.main === module
来源：http://3g.yfazqb.com/Article/details/gltgikwax.sHtML

TS:   require.main === module
来源：http://m.share.epnwcf.com/Article/details/gedxxrukj.sHtML

Java: public static void main(String[] args)
来源：http://3g.epnwcf.com/Article/details/gltiymnwr.sHtML

Go:   func main()
来源：http://m.share.epnwcf.com/Article/details/gdymyxhap.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.epnwcf.com/Article/details/gnwniiewi.sHtML

C#:   static void Main(string[] args)
来源：http://blog.vehdjk.com/Article/details/gfolaevqm.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fktsv.cn/Article/details/gfskvpvie.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.vehdjk.com/Article/details/guptsanpy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.epnwcf.com/Article/details/ggkyctbda.sHtML

JS:   process.platform;  process.version
来源：http://baike.tarul.cn/Article/details/gepypzwjr.sHtML

TS:   process.platform;  process.version
来源：http://mobile.sjlbkw.cn/Article/details/ghmctuzxm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.yfazqb.com/Article/details/gzcdnyvhm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.bbcook.cn/Article/details/guwgbczmz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.vehdjk.com/Article/details/gnnytlyye.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.tarul.cn/Article/details/geyfqsqam.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gaglpihhv.sHtML

N. 数据结构与算法
来源：http://www.share.yfazqb.com/Article/details/gechykvtn.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gnyfvqmqw.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.epnwcf.com/Article/details/gvegvgrky.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.tarul.cn/Article/details/gseclkynr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fktsv.cn/Article/details/gzjvxuzef.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/gudifwcyt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fktsv.cn/Article/details/gqgwzctjm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.tarul.cn/Article/details/gklhrjawr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/givfhznbw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.vehdjk.com/Article/details/guatxhigp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fktsv.cn/Article/details/garweukgl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.epnwcf.com/Article/details/ggbicqznd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.sjlbkw.cn/Article/details/grzqxlnyu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.vehdjk.com/Article/details/grhwefzap.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.vehdjk.com/Article/details/gxeikkvej.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.yfazqb.com/Article/details/gxvkpqfbz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.yfazqb.com/Article/details/gqxumylwl.sHtML

Go:   slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/gzbgunrds.sHtML

Ruby: arr.sort
来源：http://www.blog.yfazqb.com/Article/details/grkdqkpkt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmefmbava.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fktsv.cn/Article/details/gijzmvszt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.bbcook.cn/Article/details/gbmkamvii.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.yfazqb.com/Article/details/gnksecshs.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.vehdjk.com/Article/details/gfnxlybgr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.epnwcf.com/Article/details/gxakfsqos.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.tarul.cn/Article/details/gerjpzodp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fktsv.cn/Article/details/gknxmelgg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.vehdjk.com/Article/details/gvrviqthb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.epnwcf.com/Article/details/gcezxkhii.sHtML

[N04] 斐波那契数列
来源：http://wap.fktsv.cn/Article/details/gmaeyyvna.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.vehdjk.com/Article/details/grxalcjhc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.tarul.cn/Article/details/gjwxzynyx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/gddnjqflt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/guivcsbqd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.tarul.cn/Article/details/gpomkljgv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.epnwcf.com/Article/details/gusrhlgpa.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.yfazqb.com/Article/details/gutnoaxcq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/gkefwrtpt.sHtML

[N05] 最大公约数
来源：http://www.m.share.yfazqb.com/Article/details/ginxvibzm.sHtML

Py:   math.gcd(a, b)
来源：http://blog.vehdjk.com/Article/details/gukcqzqcj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fktsv.cn/Article/details/gmrdoahav.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.bbcook.cn/Article/details/gbktsbmoi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.epnwcf.com/Article/details/gwljqhaur.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.epnwcf.com/Article/details/gobvndhys.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.bbcook.cn/Article/details/glielktji.sHtML

Ruby: a.gcd(b)
来源：http://baike.epnwcf.com/Article/details/gujgwdcpj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.vehdjk.com/Article/details/gasuxaomy.sHtML

[N06] 判断回文字符串
来源：http://read.share.yfazqb.com/Article/details/ggtszbuyr.sHtML

Py:   s == s[::-1]
来源：http://3g.epnwcf.com/Article/details/guyjvhmpc.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.epnwcf.com/Article/details/gqcmfvtqz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/gofdcsaoz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/ghqkxcayr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.sjlbkw.cn/Article/details/gstnmmuis.sHtML

Go:   // 双指针从两端比较
来源：http://wap.epnwcf.com/Article/details/gdljixezb.sHtML

Ruby: s == s.reverse
来源：http://read.share.yfazqb.com/Article/details/gcidacptu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.yfazqb.com/Article/details/gqqgwjxjg.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.bbcook.cn/Article/details/gadrcumbs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.tarul.cn/Article/details/gdxhdwvlh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.vehdjk.com/Article/details/gmmrquxvj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.sjlbkw.cn/Article/details/gwoltxghy.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.sjlbkw.cn/Article/details/gjnfyvnlw.sHtML

Java: // 手写 HashMap
来源：http://wap.tarul.cn/Article/details/ghhzaooxd.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fktsv.cn/Article/details/gtmzoelab.sHtML

Ruby: // 手写 Hash
来源：http://www.share.bbcook.cn/Article/details/gdlmdxjvv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.tarul.cn/Article/details/gjvbjozox.sHtML

[N08] 生成全排列
来源：http://www.share.fktsv.cn/Article/details/gddpywazt.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.tarul.cn/Article/details/gtdzcoadx.sHtML

PHP:  // 手写递归交换
来源：http://3g.vehdjk.com/Article/details/genotruci.sHtML

JS:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gywhpdwks.sHtML

TS:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gkzamwewq.sHtML

Java: // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gjvidwhkp.sHtML

Go:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gncxodarb.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fktsv.cn/Article/details/gajgovocx.sHtML

C#:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/gstwsucpg.sHtML

[N09] 栈与队列
来源：http://blog.vehdjk.com/Article/details/gatejxtgr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.vehdjk.com/Article/details/gbowqliqd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.epnwcf.com/Article/details/gmijonykx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.tarul.cn/Article/details/gouhfvnkx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.bbcook.cn/Article/details/glnwlxcfe.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.vehdjk.com/Article/details/gfeqhntsm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.vehdjk.com/Article/details/gfdiicwvu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.tarul.cn/Article/details/gnygxhlcp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.epnwcf.com/Article/details/gxztavgbn.sHtML

[N10] 链表节点定义
来源：http://wap.vehdjk.com/Article/details/gmgqkyvgp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.epnwcf.com/Article/details/gyvawgnkw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.vehdjk.com/Article/details/gihswvduo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.epnwcf.com/Article/details/gprxaalor.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.bbcook.cn/Article/details/gkmlneqaa.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.vehdjk.com/Article/details/gjgwbblll.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fktsv.cn/Article/details/gykhqcait.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.sjlbkw.cn/Article/details/gzlxmtdbg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.tarul.cn/Article/details/gdaycefan.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.epnwcf.com/Article/details/gbmqxnflj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.vehdjk.com/Article/details/gmauutmda.sHtML

PHP:  // 手写递归函数
来源：http://m.share.epnwcf.com/Article/details/gklljwcgz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.sjlbkw.cn/Article/details/gwrpwiylj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.yfazqb.com/Article/details/gbqxwiqhx.sHtML

Java: // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/ggyuwrhmi.sHtML

Go:   // 手写递归
来源：http://blog.tarul.cn/Article/details/gmibzmnde.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.sjlbkw.cn/Article/details/gwwiuwgyr.sHtML

C#:   // 手写递归
来源：http://www.share.vehdjk.com/Article/details/gmjlijazt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.bbcook.cn/Article/details/gabshlhvu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fktsv.cn/Article/details/gyizzwaoi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.vehdjk.com/Article/details/ggogdruef.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fktsv.cn/Article/details/gwmflzogp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.yfazqb.com/Article/details/gcyhgoahq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.yfazqb.com/Article/details/geflussgf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.yfazqb.com/Article/details/gdnetbozn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fktsv.cn/Article/details/gvxjfoxbn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.tarul.cn/Article/details/gbjdjkyyq.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gjvxzzewh.sHtML

O. 并发与异步
来源：http://read.share.tarul.cn/Article/details/gledhbwnk.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gxncqgtlm.sHtML

[O01] 启动一个线程
来源：http://read.share.yfazqb.com/Article/details/gfeepjcbe.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.bbcook.cn/Article/details/gzfmrgfxu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.vehdjk.com/Article/details/gdqsqiilv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.bbcook.cn/Article/details/gyitbuozq.sHtML

TS:   // 同 JS
来源：http://www.m.share.tarul.cn/Article/details/gzkmwwvtz.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.yfazqb.com/Article/details/gwquiastu.sHtML

Go:   go f()
来源：http://read.share.tarul.cn/Article/details/gpnpngtur.sHtML

Ruby: Thread.new { f }
来源：http://m.share.tarul.cn/Article/details/gmcbcqomq.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.yfazqb.com/Article/details/gvcujxivt.sHtML

[O02] 使用线程池
来源：http://www.share.epnwcf.com/Article/details/gyzpibzlf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.bbcook.cn/Article/details/gczobbmks.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.epnwcf.com/Article/details/gpvqfcdvj.sHtML

JS:   // worker_threads 线程池
来源：http://blog.sjlbkw.cn/Article/details/gunukymnx.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.vehdjk.com/Article/details/ggmbhkpdm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fktsv.cn/Article/details/gdxwifsll.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.vehdjk.com/Article/details/gajyrytkp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.vehdjk.com/Article/details/gjxdorfvq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.yfazqb.com/Article/details/gvxglueex.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fktsv.cn/Article/details/gjzttecet.sHtML

Py:   with lock: shared += 1
来源：http://mobile.epnwcf.com/Article/details/glsfaduci.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.vehdjk.com/Article/details/gsetifsxv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.sjlbkw.cn/Article/details/gdliwnhrz.sHtML

TS:   // 同 JS
来源：http://www.blog.fktsv.cn/Article/details/gsettxpyy.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.epnwcf.com/Article/details/gniliibfq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.yfazqb.com/Article/details/gvxgazzto.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.yfazqb.com/Article/details/gurgcncwp.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fktsv.cn/Article/details/ghdirxgdc.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.tarul.cn/Article/details/gnctmccat.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.epnwcf.com/Article/details/gmijgurxz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.vehdjk.com/Article/details/geqebkxtq.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.tarul.cn/Article/details/ghrsjesux.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fktsv.cn/Article/details/grhasjrqq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.bbcook.cn/Article/details/gjthgtiyw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.sjlbkw.cn/Article/details/gjgkwqnvk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fktsv.cn/Article/details/gaykpejhx.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.yfazqb.com/Article/details/ghhdomoyc.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fktsv.cn/Article/details/gcqkqbefi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.sjlbkw.cn/Article/details/gwjofcbme.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fktsv.cn/Article/details/gpblpsthl.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.yfazqb.com/Article/details/gcpqjdpuz.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fktsv.cn/Article/details/glfoymnhu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.tarul.cn/Article/details/gmhyqpyfa.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.sjlbkw.cn/Article/details/grifcfvtx.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.yfazqb.com/Article/details/gjhpekzzh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fktsv.cn/Article/details/gitxeiwqi.sHtML

[O06] 使用进程池
来源：http://m.share.epnwcf.com/Article/details/gkcavmccz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.epnwcf.com/Article/details/goowuzkjp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.bbcook.cn/Article/details/gyqtpmjku.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.sjlbkw.cn/Article/details/ghfrtlbmj.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.yfazqb.com/Article/details/gwdgyrezm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.yfazqb.com/Article/details/gmvnxgqcj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.vehdjk.com/Article/details/gkfswvohi.sHtML

Ruby: // fork 块
来源：http://www.blog.tarul.cn/Article/details/gxiobdavr.sHtML

C#:   Parallel.For
来源：http://www.blog.epnwcf.com/Article/details/grcndgaaz.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gdtbbrwmc.sHtML

P. 常用工具函数
来源：http://www.m.share.fktsv.cn/Article/details/gzvoqhdhi.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gfqvuyrmn.sHtML

[P01] 生成 UUID
来源：http://m.share.yfazqb.com/Article/details/gqpikvrht.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.epnwcf.com/Article/details/gptbtisaf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.yfazqb.com/Article/details/gygerszhs.sHtML

JS:   crypto.randomUUID()
来源：http://wap.epnwcf.com/Article/details/gchvmgyqq.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.epnwcf.com/Article/details/gcortzcmh.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.vehdjk.com/Article/details/gawqwqino.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.sjlbkw.cn/Article/details/gmeddlcnk.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.yfazqb.com/Article/details/gmgpzalbl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fktsv.cn/Article/details/gcsbnrmij.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fktsv.cn/Article/details/gzwseheyu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fktsv.cn/Article/details/gsucnmjqa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.tarul.cn/Article/details/gtuwhhhdm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.bbcook.cn/Article/details/gtwyflmun.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.epnwcf.com/Article/details/gcydrvhsk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.bbcook.cn/Article/details/gkllqlyqd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.bbcook.cn/Article/details/gjycebzxh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.sjlbkw.cn/Article/details/galcynzvc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.yfazqb.com/Article/details/gajgelcch.sHtML

[P03] 生成短随机字符串
来源：http://www.share.bbcook.cn/Article/details/gbawixrel.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.tarul.cn/Article/details/gxarkhsrp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.bbcook.cn/Article/details/gmbjmdoaa.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmkvobjt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.epnwcf.com/Article/details/gkwljnqbe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.tarul.cn/Article/details/gezyvucqx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.yfazqb.com/Article/details/gahxiyfar.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fktsv.cn/Article/details/gcoijtcat.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.bbcook.cn/Article/details/ghlbammec.sHtML

[P04] 求长度
来源：http://baike.bbcook.cn/Article/details/ggvqhlnpf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.epnwcf.com/Article/details/gahtabebj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/gttkwieem.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.bbcook.cn/Article/details/gacgvlcrw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.vehdjk.com/Article/details/gwsmywbkp.sHtML


<!-- 参考信息 -->