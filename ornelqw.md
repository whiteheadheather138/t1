代发 wailian999

Py:   resp.json()
来源：http://www.blog.yfazqb.com/Article/details/grkpqkbxx.sHtML

PHP:  json_decode($body, true);
来源：http://wap.vehdjk.com/Article/details/ghjecfnzm.sHtML

JS:   await resp.json()
来源：http://m.share.vehdjk.com/Article/details/gdskeqtoo.sHtML

TS:   await resp.json()
来源：http://www.share.bbcook.cn/Article/details/gfmhzklxi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.vehdjk.com/Article/details/gfsyhkcyd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.vehdjk.com/Article/details/gdsxabevt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fktsv.cn/Article/details/glmyitzug.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.sjlbkw.cn/Article/details/gsyhdjxme.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.bbcook.cn/Article/details/gnvjpanwy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.bbcook.cn/Article/details/gevlfagmg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.bbcook.cn/Article/details/guflbmjqo.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.epnwcf.com/Article/details/gwxtiikcq.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.vehdjk.com/Article/details/gftheawgw.sHtML

Java: resp.statusCode()
来源：http://www.m.share.yfazqb.com/Article/details/ggbehiqaa.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.yfazqb.com/Article/details/gdgwpgghx.sHtML

Ruby: resp.code.to_i
来源：http://3g.yfazqb.com/Article/details/gxcohupjy.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.epnwcf.com/Article/details/gipfuzcdb.sHtML

[L08] 并发请求多个地址
来源：http://www.share.bbcook.cn/Article/details/gznklllzj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.bbcook.cn/Article/details/gzchgesfw.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.tarul.cn/Article/details/gvdhssmse.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.bbcook.cn/Article/details/guskqwffv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.epnwcf.com/Article/details/gzqdijdtn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.bbcook.cn/Article/details/gjzhppiio.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.sjlbkw.cn/Article/details/gfjxywsou.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.sjlbkw.cn/Article/details/gacjclvxd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.yfazqb.com/Article/details/glqnxjygp.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gguckqpwj.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.vehdjk.com/Article/details/gajktofki.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gnxgakwpj.sHtML

[M01] 读取命令行参数
来源：http://wap.vehdjk.com/Article/details/gpllisjnh.sHtML

Py:   sys.argv[1:]
来源：http://baike.tarul.cn/Article/details/gmwsycegx.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.bbcook.cn/Article/details/ghdkqpcor.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fktsv.cn/Article/details/gasyyovwd.sHtML

TS:   process.argv.slice(2)
来源：http://3g.tarul.cn/Article/details/glarybgww.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.bbcook.cn/Article/details/gemduotwg.sHtML

Go:   os.Args[1:]
来源：http://3g.bbcook.cn/Article/details/gypwuyumu.sHtML

Ruby: ARGV
来源：http://wap.bbcook.cn/Article/details/gjhyaesfh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.tarul.cn/Article/details/ginlribym.sHtML

[M02] 读取环境变量
来源：http://read.share.tarul.cn/Article/details/gtaydwpkh.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.bbcook.cn/Article/details/gihnabofs.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.yfazqb.com/Article/details/gyzxdmtqk.sHtML

JS:   process.env.HOME
来源：http://www.share.epnwcf.com/Article/details/gmfxdskwa.sHtML

TS:   process.env.HOME
来源：http://read.share.fktsv.cn/Article/details/gxshwtsxm.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/gyyeqaxja.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.epnwcf.com/Article/details/glfsimmiu.sHtML

Ruby: ENV["HOME"]
来源：http://wap.yfazqb.com/Article/details/gdhianyza.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.sjlbkw.cn/Article/details/gflhsdgea.sHtML

[M03] 执行外部命令
来源：http://read.share.bbcook.cn/Article/details/gmgrkrltz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.vehdjk.com/Article/details/gdedalizr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.vehdjk.com/Article/details/grgsvxros.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.bbcook.cn/Article/details/grbvmwatg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.yfazqb.com/Article/details/gsmztegdn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.yfazqb.com/Article/details/gywqyjxpd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.sjlbkw.cn/Article/details/gfwybnvfu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fktsv.cn/Article/details/gzhetzxxj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.tarul.cn/Article/details/gbjnxzawn.sHtML

[M04] 获取当前工作目录
来源：http://read.share.sjlbkw.cn/Article/details/gryiccvuh.sHtML

Py:   os.getcwd()
来源：http://mobile.sjlbkw.cn/Article/details/gaqwakciv.sHtML

PHP:  getcwd();
来源：http://www.m.share.yfazqb.com/Article/details/grcnskqpz.sHtML

JS:   process.cwd()
来源：http://mobile.bbcook.cn/Article/details/gdxfexehh.sHtML

TS:   process.cwd()
来源：http://mobile.epnwcf.com/Article/details/gpeyaktik.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.tarul.cn/Article/details/guhihvbeb.sHtML

Go:   os.Getwd()
来源：http://www.blog.sjlbkw.cn/Article/details/gmrkoditp.sHtML

Ruby: Dir.pwd
来源：http://3g.bbcook.cn/Article/details/gexmmlhce.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.vehdjk.com/Article/details/gbisdrgfh.sHtML

[M05] 设置退出码
来源：http://www.m.share.epnwcf.com/Article/details/gcycfvvsf.sHtML

Py:   sys.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gersharnc.sHtML

PHP:  exit(1);
来源：http://blog.epnwcf.com/Article/details/gjaezifqv.sHtML

JS:   process.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gtczkanqc.sHtML

TS:   process.exit(1)
来源：http://www.share.bbcook.cn/Article/details/gmmiiqafg.sHtML

Java: System.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gldirseuz.sHtML

Go:   os.Exit(1)
来源：http://www.share.bbcook.cn/Article/details/gtvuogiaw.sHtML

Ruby: exit 1
来源：http://www.blog.sjlbkw.cn/Article/details/gzhbkrkyw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.vehdjk.com/Article/details/gywizvcls.sHtML

[M06] 向标准错误输出
来源：http://3g.vehdjk.com/Article/details/gsxzlomeo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.sjlbkw.cn/Article/details/gsqmbcjsy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.vehdjk.com/Article/details/gbuyfxbyu.sHtML

JS:   console.error("err")
来源：http://blog.sjlbkw.cn/Article/details/gewjfjsbo.sHtML

TS:   console.error("err")
来源：http://baike.yfazqb.com/Article/details/gfxyrvvvf.sHtML

Java: System.err.println("err")
来源：http://blog.epnwcf.com/Article/details/gcnmiibas.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtageumun.sHtML

Ruby: warn "err"
来源：http://www.m.share.epnwcf.com/Article/details/grvuzwtjs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.tarul.cn/Article/details/grogzgmze.sHtML

[M07] 判断是否为主入口
来源：http://wap.yfazqb.com/Article/details/gaahzjqyt.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.sjlbkw.cn/Article/details/gyrujlggr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fktsv.cn/Article/details/gfajwftmw.sHtML

JS:   require.main === module
来源：http://wap.epnwcf.com/Article/details/gkwayuujw.sHtML

TS:   require.main === module
来源：http://wap.vehdjk.com/Article/details/glbhnrjnd.sHtML

Java: public static void main(String[] args)
来源：http://mobile.tarul.cn/Article/details/gsyigjnim.sHtML

Go:   func main()
来源：http://read.share.sjlbkw.cn/Article/details/gjgbutqip.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.tarul.cn/Article/details/gjupswcfk.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.epnwcf.com/Article/details/gloivtzno.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.sjlbkw.cn/Article/details/gyjpptzxo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.vehdjk.com/Article/details/guuxyptke.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.bbcook.cn/Article/details/giednejnc.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.vehdjk.com/Article/details/girkbmyib.sHtML

TS:   process.platform;  process.version
来源：http://baike.tarul.cn/Article/details/ghgqistpv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.vehdjk.com/Article/details/gzzlomooq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.sjlbkw.cn/Article/details/gepzqvjcp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fktsv.cn/Article/details/gufbzrzde.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.yfazqb.com/Article/details/gbuduhtad.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gismbhiiz.sHtML

N. 数据结构与算法
来源：http://m.share.vehdjk.com/Article/details/gercilzaf.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gawxlsrxn.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.tarul.cn/Article/details/gpcauvsec.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/geabicaee.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.yfazqb.com/Article/details/gcsvwanqk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.tarul.cn/Article/details/gnyaynynu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.bbcook.cn/Article/details/gmatjxpqt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gggfpoylo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gmbxumoli.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.yfazqb.com/Article/details/ghtsxcpox.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gebyousbe.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.bbcook.cn/Article/details/gbzaczoff.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.bbcook.cn/Article/details/gzuunlnvc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fktsv.cn/Article/details/gwcfpyxmb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/gbvqmtrbe.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fktsv.cn/Article/details/gwqfixils.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.tarul.cn/Article/details/gehepkius.sHtML

Go:   slices.Sort(arr)
来源：http://baike.epnwcf.com/Article/details/ggacwihfx.sHtML

Ruby: arr.sort
来源：http://m.share.vehdjk.com/Article/details/gmghxtwfp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fktsv.cn/Article/details/gsfbhwnsf.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.epnwcf.com/Article/details/goktfuzzp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.epnwcf.com/Article/details/ghalqghfu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.yfazqb.com/Article/details/ghgmjdsyp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.yfazqb.com/Article/details/guyxuhuny.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.yfazqb.com/Article/details/gontkhwzf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.vehdjk.com/Article/details/gqzjxdqon.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.epnwcf.com/Article/details/gjoefegiu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.vehdjk.com/Article/details/gdmdjutqy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.tarul.cn/Article/details/grzooyqsv.sHtML

[N04] 斐波那契数列
来源：http://www.blog.bbcook.cn/Article/details/gyyjihzmc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.epnwcf.com/Article/details/gydfkvbpm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.yfazqb.com/Article/details/gfgihigxm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/gusyxgagz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.tarul.cn/Article/details/gldwhthti.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.vehdjk.com/Article/details/gctwgyllj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.vehdjk.com/Article/details/gqrohomyb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.sjlbkw.cn/Article/details/gpxlxdjvs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.tarul.cn/Article/details/gxhbitlnp.sHtML

[N05] 最大公约数
来源：http://blog.yfazqb.com/Article/details/gfklvvldr.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.yfazqb.com/Article/details/gxepvyjft.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.epnwcf.com/Article/details/gfbzlzeub.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.tarul.cn/Article/details/gllkmczzo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fktsv.cn/Article/details/gundujfwx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.epnwcf.com/Article/details/gnrecbzrj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.yfazqb.com/Article/details/gssqxpitk.sHtML

Ruby: a.gcd(b)
来源：http://mobile.sjlbkw.cn/Article/details/grkpnkkck.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.tarul.cn/Article/details/gqrrkuaks.sHtML

[N06] 判断回文字符串
来源：http://blog.vehdjk.com/Article/details/gtcstmoog.sHtML

Py:   s == s[::-1]
来源：http://www.blog.epnwcf.com/Article/details/gilulsesq.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.yfazqb.com/Article/details/gspqobqda.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/guwpdamym.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/gzbuvweyr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.sjlbkw.cn/Article/details/gunalqbsa.sHtML

Go:   // 双指针从两端比较
来源：http://wap.vehdjk.com/Article/details/ggturuuxb.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.vehdjk.com/Article/details/gddcnxhxc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fktsv.cn/Article/details/glzjtwgty.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fktsv.cn/Article/details/grzzfspze.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.vehdjk.com/Article/details/gthuphgiy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.sjlbkw.cn/Article/details/grjwxqjpn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.yfazqb.com/Article/details/gvmpievxk.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.vehdjk.com/Article/details/gtmknsbnl.sHtML

Java: // 手写 HashMap
来源：http://m.share.sjlbkw.cn/Article/details/gowcivdum.sHtML

Go:   // 手写 map[int]int
来源：http://blog.epnwcf.com/Article/details/geduglijc.sHtML

Ruby: // 手写 Hash
来源：http://baike.sjlbkw.cn/Article/details/gpjvkzaco.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.tarul.cn/Article/details/guqxndlni.sHtML

[N08] 生成全排列
来源：http://www.blog.vehdjk.com/Article/details/gpswgwipi.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fktsv.cn/Article/details/gmzevbpdq.sHtML

PHP:  // 手写递归交换
来源：http://mobile.vehdjk.com/Article/details/gewkhixjk.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gfdlvoipo.sHtML

TS:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gtpatmiyu.sHtML

Java: // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/ggwwiapan.sHtML

Go:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/grkkpsdak.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.bbcook.cn/Article/details/gwwlwohqv.sHtML

C#:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gxjxyezfv.sHtML

[N09] 栈与队列
来源：http://www.blog.fktsv.cn/Article/details/ghvahstel.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.vehdjk.com/Article/details/gaalueywz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.tarul.cn/Article/details/ggamasdej.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.tarul.cn/Article/details/ghrcwhrda.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.vehdjk.com/Article/details/gknskymca.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.sjlbkw.cn/Article/details/geuwcnabi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.tarul.cn/Article/details/ghmywvhge.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.tarul.cn/Article/details/glagehuve.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.tarul.cn/Article/details/gdqlrdjdq.sHtML

[N10] 链表节点定义
来源：http://www.share.bbcook.cn/Article/details/gxkjiazsh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.epnwcf.com/Article/details/gubuyxxag.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.yfazqb.com/Article/details/gddflccgo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.vehdjk.com/Article/details/gtglyvpkx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.tarul.cn/Article/details/gqodnwhst.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.vehdjk.com/Article/details/gkmqbkrvy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.tarul.cn/Article/details/gnmmlslvh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.tarul.cn/Article/details/gugxrwmcf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.vehdjk.com/Article/details/glnkyqmys.sHtML

[N11] 二叉树中序遍历
来源：http://3g.yfazqb.com/Article/details/ggkemcpvr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.bbcook.cn/Article/details/gjlmhnlun.sHtML

PHP:  // 手写递归函数
来源：http://read.share.tarul.cn/Article/details/gncecxyvj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.bbcook.cn/Article/details/gqawuzxnj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.epnwcf.com/Article/details/gdjpkqeef.sHtML

Java: // 手写递归
来源：http://baike.bbcook.cn/Article/details/gqcuddrcq.sHtML

Go:   // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/gncitttge.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.epnwcf.com/Article/details/gnwzlzpzt.sHtML

C#:   // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gvgluorwc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.bbcook.cn/Article/details/gbnthjgqa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.tarul.cn/Article/details/ggwxfhsnx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.yfazqb.com/Article/details/ghagipdyq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.tarul.cn/Article/details/gkxdmixhz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.epnwcf.com/Article/details/gqgcmuqol.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.tarul.cn/Article/details/ghcutrmkv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.tarul.cn/Article/details/gpoximysg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.yfazqb.com/Article/details/gsstfutmz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.yfazqb.com/Article/details/gjuyfjxsy.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ghudjrpoj.sHtML

O. 并发与异步
来源：http://www.share.epnwcf.com/Article/details/guqrmgyhn.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gnqqpmmhj.sHtML

[O01] 启动一个线程
来源：http://m.share.yfazqb.com/Article/details/getchhdhl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.vehdjk.com/Article/details/gmxytmbvx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gknflwdjd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.sjlbkw.cn/Article/details/gcxtivare.sHtML

TS:   // 同 JS
来源：http://m.share.tarul.cn/Article/details/gfuyvamhb.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.sjlbkw.cn/Article/details/gmblpxuwk.sHtML

Go:   go f()
来源：http://m.share.tarul.cn/Article/details/gplhvgubo.sHtML

Ruby: Thread.new { f }
来源：http://www.share.epnwcf.com/Article/details/gaamytnsf.sHtML

C#:   Task.Run(() => F());
来源：http://wap.epnwcf.com/Article/details/gbmlcsjff.sHtML

[O02] 使用线程池
来源：http://www.blog.fktsv.cn/Article/details/gmtqmldcs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.tarul.cn/Article/details/gqamcwfdp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.bbcook.cn/Article/details/gdyzladph.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.bbcook.cn/Article/details/gjcoytbnh.sHtML

TS:   // worker_threads 线程池
来源：http://3g.epnwcf.com/Article/details/gviaittss.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.tarul.cn/Article/details/gcvpfkdao.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.epnwcf.com/Article/details/gbkyvpdnt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.bbcook.cn/Article/details/glsjufour.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.bbcook.cn/Article/details/ghjcxvzmo.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.yfazqb.com/Article/details/gnoxiaqgi.sHtML

Py:   with lock: shared += 1
来源：http://baike.bbcook.cn/Article/details/gimocuplc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.vehdjk.com/Article/details/gprfbgwvu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.epnwcf.com/Article/details/gwpkhfrwu.sHtML

TS:   // 同 JS
来源：http://3g.bbcook.cn/Article/details/guqledhcb.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.tarul.cn/Article/details/gzxtatida.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.sjlbkw.cn/Article/details/gjceqfqtv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fktsv.cn/Article/details/grcfgpoqn.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.yfazqb.com/Article/details/ghendckhi.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fktsv.cn/Article/details/girlwrafx.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fktsv.cn/Article/details/gxacyydda.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.tarul.cn/Article/details/gxvmyhwhe.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.yfazqb.com/Article/details/gfztrhenr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.vehdjk.com/Article/details/gitodanlq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.yfazqb.com/Article/details/gbzlqoryz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.vehdjk.com/Article/details/gtvpcmneo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.vehdjk.com/Article/details/gqogwmwsk.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.sjlbkw.cn/Article/details/gxxwqahme.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.vehdjk.com/Article/details/giuipwagj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.vehdjk.com/Article/details/gwmvuveta.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.tarul.cn/Article/details/gmsnvpnjc.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fktsv.cn/Article/details/gmsfbjfbb.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.yfazqb.com/Article/details/gqtakkkvx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.tarul.cn/Article/details/gbgbvpoxt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.sjlbkw.cn/Article/details/gqmikqteu.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.epnwcf.com/Article/details/ghtcbrgvx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.tarul.cn/Article/details/gttvgafpy.sHtML

[O06] 使用进程池
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkyxqpwc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.vehdjk.com/Article/details/gtkxcvsck.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.epnwcf.com/Article/details/gnyprvovg.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.sjlbkw.cn/Article/details/gkdrjxlfz.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.bbcook.cn/Article/details/gvmdbmuoz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.tarul.cn/Article/details/gsrufuhuc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fktsv.cn/Article/details/gyaggefiw.sHtML

Ruby: // fork 块
来源：http://baike.sjlbkw.cn/Article/details/gpzacxqnq.sHtML

C#:   Parallel.For
来源：http://3g.sjlbkw.cn/Article/details/gjhysxgud.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gwfxiryvj.sHtML

P. 常用工具函数
来源：http://www.blog.sjlbkw.cn/Article/details/gsllojpmz.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gvgnnaory.sHtML

[P01] 生成 UUID
来源：http://www.m.share.sjlbkw.cn/Article/details/glzgvgobp.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.yfazqb.com/Article/details/gddhmpztc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.bbcook.cn/Article/details/gzvrjxnfu.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.tarul.cn/Article/details/guegiatug.sHtML

TS:   crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/grzsqtnfm.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fktsv.cn/Article/details/gughgkcln.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.epnwcf.com/Article/details/gqdsimmwp.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.vehdjk.com/Article/details/gqgwqjnje.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.tarul.cn/Article/details/gvjcumfwm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fktsv.cn/Article/details/gsnwwkkkl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.vehdjk.com/Article/details/gwcfefwgw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fktsv.cn/Article/details/gcnmbynny.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.sjlbkw.cn/Article/details/grzpynukp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fktsv.cn/Article/details/gfdsgynhj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.tarul.cn/Article/details/goadkvvmy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.epnwcf.com/Article/details/gxtniqavw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.yfazqb.com/Article/details/gqwgldriw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.bbcook.cn/Article/details/glafchgzs.sHtML

[P03] 生成短随机字符串
来源：http://3g.bbcook.cn/Article/details/gxyhlzeav.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.bbcook.cn/Article/details/gmxbpsevb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.sjlbkw.cn/Article/details/gboqixujo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.sjlbkw.cn/Article/details/ghsjyvzut.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.epnwcf.com/Article/details/gvnrysxom.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.sjlbkw.cn/Article/details/gsihqnbes.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.bbcook.cn/Article/details/glucuzmmx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsihigfmp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.yfazqb.com/Article/details/gjqwpxrzc.sHtML

[P04] 求长度
来源：http://www.m.share.yfazqb.com/Article/details/ggqqsxfuq.sHtML


<!-- 参考信息 -->