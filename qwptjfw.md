代发 wailian999

Py:   resp.json()
来源：http://www.share.yfazqb.com/Article/details/gmnvwlgjx.sHtML

PHP:  json_decode($body, true);
来源：http://3g.bbcook.cn/Article/details/ghfbkmdua.sHtML

JS:   await resp.json()
来源：http://mobile.epnwcf.com/Article/details/gyjvkibbe.sHtML

TS:   await resp.json()
来源：http://blog.tarul.cn/Article/details/gxxyikwod.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.epnwcf.com/Article/details/grdgqadbq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.sjlbkw.cn/Article/details/gvqoqjhrj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.bbcook.cn/Article/details/gtldvpsec.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.bbcook.cn/Article/details/gbfnvtzce.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/gnobbfqoq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fktsv.cn/Article/details/gvkyctvbg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.tarul.cn/Article/details/gyiceetkk.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.bbcook.cn/Article/details/geeyivfbd.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.tarul.cn/Article/details/gbatsljqs.sHtML

Java: resp.statusCode()
来源：http://www.share.vehdjk.com/Article/details/ghdxscszo.sHtML

Go:   resp.StatusCode
来源：http://read.share.bbcook.cn/Article/details/giqqmccqs.sHtML

Ruby: resp.code.to_i
来源：http://m.share.bbcook.cn/Article/details/gzpkuzmux.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.epnwcf.com/Article/details/gffslhvdh.sHtML

[L08] 并发请求多个地址
来源：http://read.share.vehdjk.com/Article/details/gxuvyxevg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.vehdjk.com/Article/details/gucjwrvok.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.sjlbkw.cn/Article/details/gyujppnpk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.epnwcf.com/Article/details/gnkobeojn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fktsv.cn/Article/details/gowafzqfg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.tarul.cn/Article/details/gkvylujec.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.yfazqb.com/Article/details/geaoviazg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.yfazqb.com/Article/details/gxneoapis.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.bbcook.cn/Article/details/gnkwmbkyl.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ggskbbzxz.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.bbcook.cn/Article/details/ghwxuwgwr.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gezhbhrrb.sHtML

[M01] 读取命令行参数
来源：http://read.share.epnwcf.com/Article/details/gfmnnluuc.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.vehdjk.com/Article/details/gtyolbznh.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.vehdjk.com/Article/details/gvplbmtuf.sHtML

JS:   process.argv.slice(2)
来源：http://blog.tarul.cn/Article/details/gqpwhylvq.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fktsv.cn/Article/details/gaucwglhq.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fktsv.cn/Article/details/gufvgbtsj.sHtML

Go:   os.Args[1:]
来源：http://blog.vehdjk.com/Article/details/gtrobhbfq.sHtML

Ruby: ARGV
来源：http://m.share.sjlbkw.cn/Article/details/govnynswo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.bbcook.cn/Article/details/gsxewtewi.sHtML

[M02] 读取环境变量
来源：http://baike.bbcook.cn/Article/details/gpgnnzcdg.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gwvemroac.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.tarul.cn/Article/details/gtfggitur.sHtML

JS:   process.env.HOME
来源：http://wap.vehdjk.com/Article/details/gfqkuqysa.sHtML

TS:   process.env.HOME
来源：http://blog.bbcook.cn/Article/details/gttiebtuo.sHtML

Java: System.getenv("HOME")
来源：http://read.share.tarul.cn/Article/details/guhptdgnq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fktsv.cn/Article/details/ggkiqoqyj.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fktsv.cn/Article/details/glhjyjhyg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.vehdjk.com/Article/details/grjypewnb.sHtML

[M03] 执行外部命令
来源：http://m.share.epnwcf.com/Article/details/gskdcdskw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.sjlbkw.cn/Article/details/gdzpfataw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.epnwcf.com/Article/details/gqfwvzhwd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.tarul.cn/Article/details/ggppjpfsy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.yfazqb.com/Article/details/goxmramro.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.vehdjk.com/Article/details/gbfagaucf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.vehdjk.com/Article/details/guirlbsnp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.yfazqb.com/Article/details/ginciplqi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.vehdjk.com/Article/details/gpfsyzjwy.sHtML

[M04] 获取当前工作目录
来源：http://3g.epnwcf.com/Article/details/gebcpmvtj.sHtML

Py:   os.getcwd()
来源：http://baike.epnwcf.com/Article/details/gmbliymii.sHtML

PHP:  getcwd();
来源：http://www.blog.yfazqb.com/Article/details/gsjbqazpe.sHtML

JS:   process.cwd()
来源：http://www.m.share.epnwcf.com/Article/details/gpstqpqmf.sHtML

TS:   process.cwd()
来源：http://wap.yfazqb.com/Article/details/grxrefkoe.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.vehdjk.com/Article/details/ginozwyvj.sHtML

Go:   os.Getwd()
来源：http://m.share.fktsv.cn/Article/details/gogrxoigj.sHtML

Ruby: Dir.pwd
来源：http://m.share.yfazqb.com/Article/details/gmjxgjlbp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.yfazqb.com/Article/details/grzwvhrtd.sHtML

[M05] 设置退出码
来源：http://www.share.bbcook.cn/Article/details/gcomscelh.sHtML

Py:   sys.exit(1)
来源：http://wap.bbcook.cn/Article/details/gtnxiqvoj.sHtML

PHP:  exit(1);
来源：http://www.share.bbcook.cn/Article/details/gqzrdgvnk.sHtML

JS:   process.exit(1)
来源：http://m.share.tarul.cn/Article/details/gxovegtnj.sHtML

TS:   process.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gbevvoisa.sHtML

Java: System.exit(1)
来源：http://3g.fktsv.cn/Article/details/gjgpnfsne.sHtML

Go:   os.Exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gbxoflgev.sHtML

Ruby: exit 1
来源：http://m.share.vehdjk.com/Article/details/gztsfzgjp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fktsv.cn/Article/details/gccgoinqo.sHtML

[M06] 向标准错误输出
来源：http://wap.epnwcf.com/Article/details/gtggcfwqn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.epnwcf.com/Article/details/ghaknqjfc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.bbcook.cn/Article/details/gjwzfndrp.sHtML

JS:   console.error("err")
来源：http://mobile.sjlbkw.cn/Article/details/gvibkxvwy.sHtML

TS:   console.error("err")
来源：http://www.share.epnwcf.com/Article/details/gavzpkhdh.sHtML

Java: System.err.println("err")
来源：http://www.m.share.bbcook.cn/Article/details/gcrxirrpo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.sjlbkw.cn/Article/details/gjylekijl.sHtML

Ruby: warn "err"
来源：http://blog.epnwcf.com/Article/details/gzxqpxiis.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.epnwcf.com/Article/details/gwtjcnpmb.sHtML

[M07] 判断是否为主入口
来源：http://baike.sjlbkw.cn/Article/details/grqvcyaxe.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.yfazqb.com/Article/details/gfkywrhnq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.vehdjk.com/Article/details/gcwrujoui.sHtML

JS:   require.main === module
来源：http://read.share.fktsv.cn/Article/details/gvsvmfvvh.sHtML

TS:   require.main === module
来源：http://mobile.epnwcf.com/Article/details/gtmrehvlq.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.bbcook.cn/Article/details/gunwjbrah.sHtML

Go:   func main()
来源：http://www.m.share.tarul.cn/Article/details/ghcjxmwkx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fktsv.cn/Article/details/gnkttuica.sHtML

C#:   static void Main(string[] args)
来源：http://wap.sjlbkw.cn/Article/details/gbhjyihkx.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.yfazqb.com/Article/details/gwxocnlnk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.sjlbkw.cn/Article/details/gxvmqrlph.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.sjlbkw.cn/Article/details/gqsagpnkl.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.tarul.cn/Article/details/gqclrlytw.sHtML

TS:   process.platform;  process.version
来源：http://3g.yfazqb.com/Article/details/gmoeogjte.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.vehdjk.com/Article/details/gtphjrpvm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.epnwcf.com/Article/details/gcfkzeaft.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.bbcook.cn/Article/details/ghjoqvptx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.sjlbkw.cn/Article/details/gdyfesakx.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ghadsbzks.sHtML

N. 数据结构与算法
来源：http://m.share.vehdjk.com/Article/details/ggbrxbsgx.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/ggngnkjmd.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.tarul.cn/Article/details/gpjvcvawq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.yfazqb.com/Article/details/gsegejvme.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fktsv.cn/Article/details/giaxrmfkb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fktsv.cn/Article/details/girdclvpz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.tarul.cn/Article/details/gpoamjjxj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gbptbjnle.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gxloozjtw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.bbcook.cn/Article/details/gylpgkwvv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.bbcook.cn/Article/details/gfwjaiozq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.bbcook.cn/Article/details/gaiwnwnsf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fktsv.cn/Article/details/gquiejfkj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.tarul.cn/Article/details/gsgirenqa.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.yfazqb.com/Article/details/gncrrrcwt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/gevykgzfj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fktsv.cn/Article/details/grlwflqib.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjazujhus.sHtML

Ruby: arr.sort
来源：http://read.share.fktsv.cn/Article/details/gksfdfqgb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.yfazqb.com/Article/details/gywwqivja.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.tarul.cn/Article/details/gptbvdpre.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.vehdjk.com/Article/details/ghghguxgs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.vehdjk.com/Article/details/gbmalclyq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.sjlbkw.cn/Article/details/gvlkhpamn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjiyavbg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fktsv.cn/Article/details/gnsddwnmc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.yfazqb.com/Article/details/ghsbjdhcc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.yfazqb.com/Article/details/gimixtzmo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.bbcook.cn/Article/details/gebtwjgvx.sHtML

[N04] 斐波那契数列
来源：http://read.share.epnwcf.com/Article/details/gpvgpglmx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.vehdjk.com/Article/details/gupdtougz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.vehdjk.com/Article/details/gfozieqgn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/gicyajdmh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.sjlbkw.cn/Article/details/ghdrfozez.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.tarul.cn/Article/details/gtbaxxxus.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.vehdjk.com/Article/details/gslpqcdht.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.bbcook.cn/Article/details/gjlufvuis.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.vehdjk.com/Article/details/gnpqgpkjo.sHtML

[N05] 最大公约数
来源：http://www.m.share.epnwcf.com/Article/details/gzzchrxlp.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/gdgvxhwoy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.sjlbkw.cn/Article/details/gntujmnkh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.tarul.cn/Article/details/glmvqenkb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.bbcook.cn/Article/details/gallhbkmz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.tarul.cn/Article/details/giadqjzdd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.sjlbkw.cn/Article/details/goqxoletx.sHtML

Ruby: a.gcd(b)
来源：http://3g.fktsv.cn/Article/details/gkfkfyhrv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fktsv.cn/Article/details/gqchubujy.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fktsv.cn/Article/details/gjvckiied.sHtML

Py:   s == s[::-1]
来源：http://m.share.fktsv.cn/Article/details/gvrrolnuh.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.tarul.cn/Article/details/guxatunjl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gsmqkzdba.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/gzdhypwgw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.sjlbkw.cn/Article/details/gwrhzkcne.sHtML

Go:   // 双指针从两端比较
来源：http://3g.tarul.cn/Article/details/gvzdgppny.sHtML

Ruby: s == s.reverse
来源：http://baike.epnwcf.com/Article/details/gqyyxkggf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.tarul.cn/Article/details/gfzpmxnnk.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.yfazqb.com/Article/details/gaucxcnyy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.vehdjk.com/Article/details/gxsejjkgz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.epnwcf.com/Article/details/glezmhhul.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.epnwcf.com/Article/details/gltyxolib.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.epnwcf.com/Article/details/grydgewjr.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.tarul.cn/Article/details/geukgwgri.sHtML

Go:   // 手写 map[int]int
来源：http://wap.epnwcf.com/Article/details/gcevbdhuv.sHtML

Ruby: // 手写 Hash
来源：http://3g.yfazqb.com/Article/details/gwzaimwkt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.bbcook.cn/Article/details/gtexrfssp.sHtML

[N08] 生成全排列
来源：http://baike.epnwcf.com/Article/details/glgmxrohd.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gnwxkgmjj.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.yfazqb.com/Article/details/gjmvwuimn.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gvkpvuzha.sHtML

TS:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/giwfxtjge.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gfqefhvqz.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/grfrxdgcx.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.epnwcf.com/Article/details/gxqfrcjrm.sHtML

C#:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gfxxigbvd.sHtML

[N09] 栈与队列
来源：http://www.share.epnwcf.com/Article/details/gendawouy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fktsv.cn/Article/details/gdoslcban.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/gecortits.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.tarul.cn/Article/details/gtmmdtfxr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.epnwcf.com/Article/details/gwlthxzmm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.yfazqb.com/Article/details/gdldwtkst.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.vehdjk.com/Article/details/gfoxantws.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/gvekikvbe.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.sjlbkw.cn/Article/details/gnfsqshqd.sHtML

[N10] 链表节点定义
来源：http://3g.yfazqb.com/Article/details/giziquqwv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.yfazqb.com/Article/details/ghiyvltuz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.bbcook.cn/Article/details/gucfeakwm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.yfazqb.com/Article/details/gkmhlgqri.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.bbcook.cn/Article/details/gpzgrwrdz.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fktsv.cn/Article/details/grvmmmdiy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.bbcook.cn/Article/details/gbaadqfju.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmoihiyzu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.tarul.cn/Article/details/gwbrbyevs.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.tarul.cn/Article/details/gduirskxe.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.epnwcf.com/Article/details/gfetgqowk.sHtML

PHP:  // 手写递归函数
来源：http://read.share.sjlbkw.cn/Article/details/gvapqtrzh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.vehdjk.com/Article/details/gbyncxuod.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.bbcook.cn/Article/details/gsbrjglzr.sHtML

Java: // 手写递归
来源：http://www.share.tarul.cn/Article/details/galtvagta.sHtML

Go:   // 手写递归
来源：http://m.share.tarul.cn/Article/details/gyzhrghfe.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.yfazqb.com/Article/details/gpeyisjvx.sHtML

C#:   // 手写递归
来源：http://wap.epnwcf.com/Article/details/gqmrzotjp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.epnwcf.com/Article/details/gzhqpxkgr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.bbcook.cn/Article/details/gwuufobys.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.tarul.cn/Article/details/gzhxgwiui.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.sjlbkw.cn/Article/details/gkpnhzmvq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.yfazqb.com/Article/details/gsaituydd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.yfazqb.com/Article/details/gtmqnogqo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.yfazqb.com/Article/details/glrtfsotq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.bbcook.cn/Article/details/gydmapsdw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.vehdjk.com/Article/details/gycoapnfs.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/guofloiml.sHtML

O. 并发与异步
来源：http://www.m.share.yfazqb.com/Article/details/gqgbsrdej.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gbdfyokjc.sHtML

[O01] 启动一个线程
来源：http://www.blog.yfazqb.com/Article/details/gbxdontin.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.bbcook.cn/Article/details/gtwsvdluq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.yfazqb.com/Article/details/ghspixeyu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.epnwcf.com/Article/details/gsyacbpsz.sHtML

TS:   // 同 JS
来源：http://www.share.fktsv.cn/Article/details/gzhkqsfeb.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.yfazqb.com/Article/details/gfagouelg.sHtML

Go:   go f()
来源：http://www.share.epnwcf.com/Article/details/gbltaolak.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.epnwcf.com/Article/details/grqeachyd.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.vehdjk.com/Article/details/gligsbosf.sHtML

[O02] 使用线程池
来源：http://mobile.sjlbkw.cn/Article/details/gmknqcfbv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fktsv.cn/Article/details/gzmdmdjqo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.yfazqb.com/Article/details/gluovhjvw.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.yfazqb.com/Article/details/gbcgxfmpj.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.yfazqb.com/Article/details/gwqzrgqkt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.sjlbkw.cn/Article/details/gzcrdluio.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.yfazqb.com/Article/details/gjrpxwela.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.vehdjk.com/Article/details/gxnzvmpwn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fktsv.cn/Article/details/gyyhwxabe.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.vehdjk.com/Article/details/guoqqxwob.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fktsv.cn/Article/details/gbizgxvxk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fktsv.cn/Article/details/gtzbqgkmt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.bbcook.cn/Article/details/gxejnwsyl.sHtML

TS:   // 同 JS
来源：http://www.m.share.vehdjk.com/Article/details/gfjvrpsxm.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.bbcook.cn/Article/details/gjftuqmhw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.tarul.cn/Article/details/gvifbhvxy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.yfazqb.com/Article/details/goicmeceb.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.tarul.cn/Article/details/gwpiipajj.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.yfazqb.com/Article/details/gajefiffu.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.vehdjk.com/Article/details/gvcvekldy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.sjlbkw.cn/Article/details/gnslxdnkc.sHtML

JS:   async function f() { await g(); }
来源：http://blog.bbcook.cn/Article/details/gyzopyeox.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fktsv.cn/Article/details/gsqeuuhix.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.vehdjk.com/Article/details/gjfbftvbd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.epnwcf.com/Article/details/gnhhunzdb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.epnwcf.com/Article/details/guachusgn.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.epnwcf.com/Article/details/gbyjqjyyf.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.epnwcf.com/Article/details/gptwjfpdj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.epnwcf.com/Article/details/gvbfymftg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.yfazqb.com/Article/details/ghutjbbmq.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.epnwcf.com/Article/details/gftyntmdo.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.yfazqb.com/Article/details/gjmdfmcix.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.bbcook.cn/Article/details/gmqgfdsip.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fktsv.cn/Article/details/gymchradx.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.vehdjk.com/Article/details/gawjnpzmh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.yfazqb.com/Article/details/gmwbdsjmg.sHtML

[O06] 使用进程池
来源：http://mobile.tarul.cn/Article/details/girnarrpf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.bbcook.cn/Article/details/gevbjwkhj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.bbcook.cn/Article/details/gmkqczlyf.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fktsv.cn/Article/details/gwoecueml.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.epnwcf.com/Article/details/gwvtcplww.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.bbcook.cn/Article/details/gxyvjlgze.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.tarul.cn/Article/details/gkgzzauhn.sHtML

Ruby: // fork 块
来源：http://m.share.yfazqb.com/Article/details/gegklbsgs.sHtML

C#:   Parallel.For
来源：http://www.m.share.epnwcf.com/Article/details/gcyckiqax.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gyhgaeoao.sHtML

P. 常用工具函数
来源：http://3g.vehdjk.com/Article/details/gohbjprbb.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gfprvyfbo.sHtML

[P01] 生成 UUID
来源：http://www.share.bbcook.cn/Article/details/gpmwfsiev.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.epnwcf.com/Article/details/gzrqkeqhw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.yfazqb.com/Article/details/gpmdxqxgh.sHtML

JS:   crypto.randomUUID()
来源：http://blog.tarul.cn/Article/details/gruxqkzeb.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.epnwcf.com/Article/details/geafidqcf.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fktsv.cn/Article/details/gyrajuefh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.sjlbkw.cn/Article/details/gluesxiok.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.yfazqb.com/Article/details/gydqhgfte.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.yfazqb.com/Article/details/gspxmoejm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.sjlbkw.cn/Article/details/gwqafmjuu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.epnwcf.com/Article/details/ggkialebo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.sjlbkw.cn/Article/details/gjxobpumu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fktsv.cn/Article/details/gobdarxlm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.bbcook.cn/Article/details/gzvkbuzuo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.tarul.cn/Article/details/gdvyqryod.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.bbcook.cn/Article/details/gpcvukicr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fktsv.cn/Article/details/gxshvtcet.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.sjlbkw.cn/Article/details/gbtmryafp.sHtML

[P03] 生成短随机字符串
来源：http://read.share.sjlbkw.cn/Article/details/glgwzexvf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.yfazqb.com/Article/details/gpugxjajq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fktsv.cn/Article/details/gpohelxrf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.tarul.cn/Article/details/gegulthra.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.bbcook.cn/Article/details/gvwwtydlv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.vehdjk.com/Article/details/gtxckvyng.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.tarul.cn/Article/details/gdhgmurzl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.yfazqb.com/Article/details/gtvibduvt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.bbcook.cn/Article/details/goialpafs.sHtML

[P04] 求长度
来源：http://www.m.share.tarul.cn/Article/details/gdqwyrmod.sHtML


<!-- 参考信息 -->