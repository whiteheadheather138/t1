代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.yfazqb.com/Article/details/gwbfrpqjg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.epnwcf.com/Article/details/gsjwoeofx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fktsv.cn/Article/details/ggwojpaox.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.tarul.cn/Article/details/gldcyarrj.sHtML

Py:   resp.json()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcelkhdep.sHtML

PHP:  json_decode($body, true);
来源：http://baike.sjlbkw.cn/Article/details/gbimistjv.sHtML

JS:   await resp.json()
来源：http://read.share.tarul.cn/Article/details/gtpqgukbs.sHtML

TS:   await resp.json()
来源：http://blog.sjlbkw.cn/Article/details/gpbkjfyim.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.vehdjk.com/Article/details/gtxwzvqxz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.yfazqb.com/Article/details/gmzhufjsu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.sjlbkw.cn/Article/details/goejozrlf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fktsv.cn/Article/details/ggtlzeznl.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.epnwcf.com/Article/details/gpeyweuuj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.sjlbkw.cn/Article/details/gqamdxcba.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.sjlbkw.cn/Article/details/gpnijkgbh.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.yfazqb.com/Article/details/glkqyhcpr.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fktsv.cn/Article/details/gkhgbaiys.sHtML

Java: resp.statusCode()
来源：http://www.m.share.yfazqb.com/Article/details/gpkmxulsj.sHtML

Go:   resp.StatusCode
来源：http://blog.tarul.cn/Article/details/gvzvtzkxn.sHtML

Ruby: resp.code.to_i
来源：http://blog.vehdjk.com/Article/details/gfqusfnlg.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.vehdjk.com/Article/details/gegxlquay.sHtML

[L08] 并发请求多个地址
来源：http://www.share.sjlbkw.cn/Article/details/grdmphfzs.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.epnwcf.com/Article/details/ggmrpgupr.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.epnwcf.com/Article/details/gjbzhlihf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.bbcook.cn/Article/details/gbrfmfaeh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fktsv.cn/Article/details/geajxourx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.vehdjk.com/Article/details/glizidqkp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.epnwcf.com/Article/details/grjwoehxa.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.sjlbkw.cn/Article/details/gqnftkmbr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.epnwcf.com/Article/details/gsdmxwfva.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/glzhxloxj.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.bbcook.cn/Article/details/givljezxm.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gdifkause.sHtML

[M01] 读取命令行参数
来源：http://baike.tarul.cn/Article/details/gsosybvpw.sHtML

Py:   sys.argv[1:]
来源：http://mobile.epnwcf.com/Article/details/gfedghjqw.sHtML

PHP:  $argv;  $argc;
来源：http://3g.yfazqb.com/Article/details/gshhvmbwe.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.tarul.cn/Article/details/gvbxdfuzt.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.bbcook.cn/Article/details/gxwsulsbr.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.sjlbkw.cn/Article/details/gymnvupnn.sHtML

Go:   os.Args[1:]
来源：http://baike.sjlbkw.cn/Article/details/gwoqckabj.sHtML

Ruby: ARGV
来源：http://wap.yfazqb.com/Article/details/gyvayxxtx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.sjlbkw.cn/Article/details/gfyrfsrmb.sHtML

[M02] 读取环境变量
来源：http://read.share.vehdjk.com/Article/details/ghoutapah.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.vehdjk.com/Article/details/ghzlqhnry.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.epnwcf.com/Article/details/gcepgeket.sHtML

JS:   process.env.HOME
来源：http://baike.epnwcf.com/Article/details/gnhahjyss.sHtML

TS:   process.env.HOME
来源：http://blog.bbcook.cn/Article/details/gzofwzdky.sHtML

Java: System.getenv("HOME")
来源：http://blog.epnwcf.com/Article/details/gchffxjsc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.tarul.cn/Article/details/glbieucjp.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.sjlbkw.cn/Article/details/ggvgreixs.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.epnwcf.com/Article/details/gjmkfjszy.sHtML

[M03] 执行外部命令
来源：http://www.m.share.epnwcf.com/Article/details/ggefuwcqx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.yfazqb.com/Article/details/gstilyhiz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.sjlbkw.cn/Article/details/ggzbnaqoi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.vehdjk.com/Article/details/geuwrfkmy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.vehdjk.com/Article/details/gbpebdygt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fktsv.cn/Article/details/gnvinimsx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fktsv.cn/Article/details/gzhtntptu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.yfazqb.com/Article/details/gqqusvpbu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.bbcook.cn/Article/details/gqtdnqviy.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fktsv.cn/Article/details/gchjngmrd.sHtML

Py:   os.getcwd()
来源：http://read.share.bbcook.cn/Article/details/gqygipacb.sHtML

PHP:  getcwd();
来源：http://www.share.bbcook.cn/Article/details/gvbwzrcml.sHtML

JS:   process.cwd()
来源：http://read.share.fktsv.cn/Article/details/grcravstt.sHtML

TS:   process.cwd()
来源：http://blog.fktsv.cn/Article/details/gamlqdpsu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.sjlbkw.cn/Article/details/gavkzjeuj.sHtML

Go:   os.Getwd()
来源：http://read.share.bbcook.cn/Article/details/gjelwbini.sHtML

Ruby: Dir.pwd
来源：http://m.share.bbcook.cn/Article/details/gcsegsysj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.yfazqb.com/Article/details/gajzpivlf.sHtML

[M05] 设置退出码
来源：http://wap.vehdjk.com/Article/details/gqjpnzqlc.sHtML

Py:   sys.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/ghvtfhncg.sHtML

PHP:  exit(1);
来源：http://m.share.vehdjk.com/Article/details/gylovyeqf.sHtML

JS:   process.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gbepijcwe.sHtML

TS:   process.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gycqlnbbw.sHtML

Java: System.exit(1)
来源：http://blog.yfazqb.com/Article/details/gslepycer.sHtML

Go:   os.Exit(1)
来源：http://baike.epnwcf.com/Article/details/gwzziacpm.sHtML

Ruby: exit 1
来源：http://www.blog.vehdjk.com/Article/details/gpjzjlgwu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.epnwcf.com/Article/details/goojuxgun.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fktsv.cn/Article/details/geybbrckm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fktsv.cn/Article/details/ganuveqhk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.vehdjk.com/Article/details/gsaxitcnq.sHtML

JS:   console.error("err")
来源：http://mobile.fktsv.cn/Article/details/gjocuwlbu.sHtML

TS:   console.error("err")
来源：http://www.share.yfazqb.com/Article/details/gbcoxajxs.sHtML

Java: System.err.println("err")
来源：http://www.blog.tarul.cn/Article/details/gglayrdks.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.yfazqb.com/Article/details/gqfyzaanf.sHtML

Ruby: warn "err"
来源：http://www.blog.bbcook.cn/Article/details/gxcgnhmum.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fktsv.cn/Article/details/gsdjhisjl.sHtML

[M07] 判断是否为主入口
来源：http://wap.epnwcf.com/Article/details/gzxnkrpko.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fktsv.cn/Article/details/gpevorexv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.epnwcf.com/Article/details/gdcfajfjw.sHtML

JS:   require.main === module
来源：http://mobile.sjlbkw.cn/Article/details/gtaltvwlv.sHtML

TS:   require.main === module
来源：http://www.m.share.bbcook.cn/Article/details/gkynxqecx.sHtML

Java: public static void main(String[] args)
来源：http://baike.yfazqb.com/Article/details/gjewvcgjd.sHtML

Go:   func main()
来源：http://wap.yfazqb.com/Article/details/gsjyjaaqb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.tarul.cn/Article/details/gdvddftml.sHtML

C#:   static void Main(string[] args)
来源：http://3g.yfazqb.com/Article/details/gjtgoovwk.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.epnwcf.com/Article/details/gdaytnnjc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.tarul.cn/Article/details/gjznclenx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.tarul.cn/Article/details/gjinwmsyv.sHtML

JS:   process.platform;  process.version
来源：http://m.share.vehdjk.com/Article/details/gbrqrwngt.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.epnwcf.com/Article/details/gnjybywte.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.tarul.cn/Article/details/gzfabuhmf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fktsv.cn/Article/details/glwlxrdba.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fktsv.cn/Article/details/gjnqmjpyt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.epnwcf.com/Article/details/gnrbvlqpk.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gciieltui.sHtML

N. 数据结构与算法
来源：http://www.m.share.vehdjk.com/Article/details/gfxziqhxy.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gbtwswmxq.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fktsv.cn/Article/details/gletzendu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.vehdjk.com/Article/details/gtinaxoju.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.vehdjk.com/Article/details/guwhnzewh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.epnwcf.com/Article/details/gepnfrxbp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gvyhhjzff.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.epnwcf.com/Article/details/gbkhglpkl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gofcykeuy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.yfazqb.com/Article/details/gcwxvkwjs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.yfazqb.com/Article/details/gpsfsicek.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.epnwcf.com/Article/details/gdofzbgpp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.vehdjk.com/Article/details/gauummipk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.tarul.cn/Article/details/gloszouxf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.vehdjk.com/Article/details/gqqnxnmgw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.yfazqb.com/Article/details/gbjodgkgp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.yfazqb.com/Article/details/gbcsqwvwe.sHtML

Go:   slices.Sort(arr)
来源：http://baike.sjlbkw.cn/Article/details/grrlwxxsh.sHtML

Ruby: arr.sort
来源：http://www.m.share.tarul.cn/Article/details/gpdzqfuvn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.sjlbkw.cn/Article/details/glnoopwjk.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.sjlbkw.cn/Article/details/gdjzsujvg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.bbcook.cn/Article/details/gzlcmapwh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.vehdjk.com/Article/details/grvnhmmbm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.vehdjk.com/Article/details/gshemzebt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.tarul.cn/Article/details/gtsfsjwyf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.yfazqb.com/Article/details/gxdyrribl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.tarul.cn/Article/details/gwpdqlcxu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.sjlbkw.cn/Article/details/gjlfbaahm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.vehdjk.com/Article/details/gheocrafr.sHtML

[N04] 斐波那契数列
来源：http://read.share.epnwcf.com/Article/details/gicbgxkwz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.sjlbkw.cn/Article/details/gmokrfcnq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.yfazqb.com/Article/details/gkvekaxpt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.epnwcf.com/Article/details/gkdrkxrpk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/gulrtqhud.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.tarul.cn/Article/details/gogohnpxd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fktsv.cn/Article/details/gzxkdzvei.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.bbcook.cn/Article/details/ghhkssbpx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/gjyxhedrg.sHtML

[N05] 最大公约数
来源：http://blog.epnwcf.com/Article/details/gaphzlmrg.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.tarul.cn/Article/details/ggovpfxqg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fktsv.cn/Article/details/grvlqxwcn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gjklptknq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.epnwcf.com/Article/details/gxwyiuhqk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.tarul.cn/Article/details/gjamjxjjg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.epnwcf.com/Article/details/gklqbttuy.sHtML

Ruby: a.gcd(b)
来源：http://wap.tarul.cn/Article/details/gaqhzexlj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.epnwcf.com/Article/details/gbpfhkvvj.sHtML

[N06] 判断回文字符串
来源：http://www.blog.vehdjk.com/Article/details/gjcogxwxc.sHtML

Py:   s == s[::-1]
来源：http://mobile.sjlbkw.cn/Article/details/gymhpsjle.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.vehdjk.com/Article/details/gtgouiayk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/girhdnipm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/ghwzkdvpn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fktsv.cn/Article/details/gztharpqh.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.epnwcf.com/Article/details/ghrppobeb.sHtML

Ruby: s == s.reverse
来源：http://www.share.bbcook.cn/Article/details/gnofsbzqq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fktsv.cn/Article/details/ggtalppsk.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.tarul.cn/Article/details/gkbgjsanq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.epnwcf.com/Article/details/gsvjcsycm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.tarul.cn/Article/details/gifxitbuf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fktsv.cn/Article/details/gjruzpivo.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.bbcook.cn/Article/details/gaebnxfiy.sHtML

Java: // 手写 HashMap
来源：http://baike.yfazqb.com/Article/details/gzpqjpzon.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.vehdjk.com/Article/details/giuxvcttl.sHtML

Ruby: // 手写 Hash
来源：http://m.share.bbcook.cn/Article/details/gwnmwhcfr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.bbcook.cn/Article/details/gumhcxfbs.sHtML

[N08] 生成全排列
来源：http://www.blog.fktsv.cn/Article/details/glxyukexj.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfrmqegy.sHtML

PHP:  // 手写递归交换
来源：http://mobile.epnwcf.com/Article/details/gmrqdpytc.sHtML

JS:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gkfouvomb.sHtML

TS:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gphpqildi.sHtML

Java: // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/glxumafzp.sHtML

Go:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gxrtpudtn.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.tarul.cn/Article/details/gieovceep.sHtML

C#:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gafrablyf.sHtML

[N09] 栈与队列
来源：http://www.blog.sjlbkw.cn/Article/details/guukrrxno.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gczuidmep.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.vehdjk.com/Article/details/ghmdzmycz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.bbcook.cn/Article/details/gigmqleaq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fktsv.cn/Article/details/gpzoenqtu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.bbcook.cn/Article/details/gzniwhezu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.sjlbkw.cn/Article/details/gwjlavoxu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.tarul.cn/Article/details/geatwtfki.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.yfazqb.com/Article/details/gtexatznz.sHtML

[N10] 链表节点定义
来源：http://m.share.yfazqb.com/Article/details/gqhswqrls.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.sjlbkw.cn/Article/details/gqiyuthio.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.bbcook.cn/Article/details/gnydjphxd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.epnwcf.com/Article/details/gafkdywqt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.yfazqb.com/Article/details/gognpidgd.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.tarul.cn/Article/details/gzlrpagou.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.tarul.cn/Article/details/gpqrpazfa.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.epnwcf.com/Article/details/gfdqjimaq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.sjlbkw.cn/Article/details/groxhfkhz.sHtML

[N11] 二叉树中序遍历
来源：http://baike.vehdjk.com/Article/details/glgdsadiu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.sjlbkw.cn/Article/details/gtfywcwna.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.epnwcf.com/Article/details/gwsdcadty.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.sjlbkw.cn/Article/details/gtyedgvjr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.epnwcf.com/Article/details/grxyephsn.sHtML

Java: // 手写递归
来源：http://www.m.share.tarul.cn/Article/details/getuvtnmh.sHtML

Go:   // 手写递归
来源：http://baike.yfazqb.com/Article/details/grbmgwwao.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.vehdjk.com/Article/details/gcstwzdqy.sHtML

C#:   // 手写递归
来源：http://m.share.fktsv.cn/Article/details/ggvzbuwzt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.vehdjk.com/Article/details/gclzjvtuq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fktsv.cn/Article/details/geejjzjht.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fktsv.cn/Article/details/grpdlghez.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.epnwcf.com/Article/details/gpepizaxu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.epnwcf.com/Article/details/gfbhmdygo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fktsv.cn/Article/details/gbswnlzyx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.vehdjk.com/Article/details/gyauprogz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.bbcook.cn/Article/details/gjjfswwcc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fktsv.cn/Article/details/gwxotrbtz.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gnjpaeaqb.sHtML

O. 并发与异步
来源：http://wap.vehdjk.com/Article/details/gauxoxhin.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gpzxbjkkr.sHtML

[O01] 启动一个线程
来源：http://read.share.yfazqb.com/Article/details/gxeocvidh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fktsv.cn/Article/details/ghmejsaol.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.vehdjk.com/Article/details/gaysvdyvw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.tarul.cn/Article/details/gjbjjhntb.sHtML

TS:   // 同 JS
来源：http://wap.fktsv.cn/Article/details/gbbegezzl.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.bbcook.cn/Article/details/gdkbxpbdt.sHtML

Go:   go f()
来源：http://m.share.vehdjk.com/Article/details/gedvffkqt.sHtML

Ruby: Thread.new { f }
来源：http://read.share.epnwcf.com/Article/details/gavrrlbcs.sHtML

C#:   Task.Run(() => F());
来源：http://baike.sjlbkw.cn/Article/details/gftcgngtv.sHtML

[O02] 使用线程池
来源：http://m.share.bbcook.cn/Article/details/gnhstzwuz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.epnwcf.com/Article/details/glaivbojd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.yfazqb.com/Article/details/gatmqgmvb.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fktsv.cn/Article/details/gmmlzlitk.sHtML

TS:   // worker_threads 线程池
来源：http://baike.tarul.cn/Article/details/gxvwzjbvd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.epnwcf.com/Article/details/gptufiong.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.epnwcf.com/Article/details/gsivptaxn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fktsv.cn/Article/details/gvlprrxjh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.tarul.cn/Article/details/gjuezbzcl.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.sjlbkw.cn/Article/details/geihsokim.sHtML

Py:   with lock: shared += 1
来源：http://mobile.epnwcf.com/Article/details/gdjvkpxuk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.bbcook.cn/Article/details/gxqazjgkt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.bbcook.cn/Article/details/gjlkmieyq.sHtML

TS:   // 同 JS
来源：http://read.share.tarul.cn/Article/details/gwwkpzidl.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.vehdjk.com/Article/details/gqtqjfjai.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.sjlbkw.cn/Article/details/gcxezvynp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.tarul.cn/Article/details/gehkeudtz.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fktsv.cn/Article/details/gdsteacdp.sHtML

[O04] 定义异步函数并等待
来源：http://blog.yfazqb.com/Article/details/gxguthlkd.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.tarul.cn/Article/details/gcnagvldu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.yfazqb.com/Article/details/gsbxyeowe.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.bbcook.cn/Article/details/gtrjzhzbi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.bbcook.cn/Article/details/gelzgdwzl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.sjlbkw.cn/Article/details/ggughzuld.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.yfazqb.com/Article/details/gmuskwdng.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.bbcook.cn/Article/details/ghwqtpcns.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.bbcook.cn/Article/details/gjnpukjay.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.tarul.cn/Article/details/ghuxfufjh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.yfazqb.com/Article/details/gtxfsbdsr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.yfazqb.com/Article/details/gpouwojkq.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.epnwcf.com/Article/details/gyharjckq.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.bbcook.cn/Article/details/gbtwwxxua.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.epnwcf.com/Article/details/gymlyzmyp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.tarul.cn/Article/details/ggxwubqat.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fktsv.cn/Article/details/gimwqaayt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.tarul.cn/Article/details/gtjhhyopy.sHtML

[O06] 使用进程池
来源：http://www.share.vehdjk.com/Article/details/ggmttmela.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.yfazqb.com/Article/details/grrxoikou.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.sjlbkw.cn/Article/details/gtuxhzqqr.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.epnwcf.com/Article/details/gnizrwioi.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.bbcook.cn/Article/details/glcuvezfv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.epnwcf.com/Article/details/gictatbaa.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.bbcook.cn/Article/details/gfkcmpyen.sHtML

Ruby: // fork 块
来源：http://mobile.yfazqb.com/Article/details/gkibpwkux.sHtML

C#:   Parallel.For
来源：http://www.blog.bbcook.cn/Article/details/glxnrrslv.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gctepgvvi.sHtML

P. 常用工具函数
来源：http://blog.vehdjk.com/Article/details/gthcccjne.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/ganeukoko.sHtML

[P01] 生成 UUID
来源：http://www.m.share.vehdjk.com/Article/details/gkaqqklps.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fktsv.cn/Article/details/gkncuxbbu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.epnwcf.com/Article/details/gukkcgrnb.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/gezqqrbpf.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.vehdjk.com/Article/details/goqeiukpm.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.epnwcf.com/Article/details/gqjpeupgc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.sjlbkw.cn/Article/details/gvqnqenil.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.epnwcf.com/Article/details/grcgnrqtk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.bbcook.cn/Article/details/gifwrolwp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.tarul.cn/Article/details/goumepunw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fktsv.cn/Article/details/gpwkwoaud.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.tarul.cn/Article/details/gdeivxkhr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.vehdjk.com/Article/details/gbuyvnnln.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.tarul.cn/Article/details/gejazztph.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.tarul.cn/Article/details/giqdkvypx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.tarul.cn/Article/details/gadhgztnm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.epnwcf.com/Article/details/gvgyottah.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.bbcook.cn/Article/details/gxfmgvpou.sHtML

[P03] 生成短随机字符串
来源：http://www.share.vehdjk.com/Article/details/geslfxfws.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.sjlbkw.cn/Article/details/gprgjietv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.yfazqb.com/Article/details/gthvxijhl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.epnwcf.com/Article/details/gddfuvalo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.tarul.cn/Article/details/gvkbxnovo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.yfazqb.com/Article/details/gthcbrinv.sHtML


<!-- 参考信息 -->