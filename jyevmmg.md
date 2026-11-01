代发 wailian999

Py:   resp.json()
来源：http://mobile.yfazqb.com/Article/details/gvzhobpou.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.yfazqb.com/Article/details/gkgfhroax.sHtML

JS:   await resp.json()
来源：http://wap.sjlbkw.cn/Article/details/glmgsxggg.sHtML

TS:   await resp.json()
来源：http://read.share.yfazqb.com/Article/details/grjtdklhx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.tarul.cn/Article/details/gqzudrtgz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.vehdjk.com/Article/details/gpxcrzhli.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fktsv.cn/Article/details/gojmgdxoi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.tarul.cn/Article/details/gkeuzgssf.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.vehdjk.com/Article/details/gvcusglwo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.sjlbkw.cn/Article/details/guutueebd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.bbcook.cn/Article/details/gywunpvif.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.yfazqb.com/Article/details/gffabzgsf.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fktsv.cn/Article/details/gmrqjmhdt.sHtML

Java: resp.statusCode()
来源：http://3g.fktsv.cn/Article/details/gkqurarks.sHtML

Go:   resp.StatusCode
来源：http://blog.bbcook.cn/Article/details/gfcwtwyfd.sHtML

Ruby: resp.code.to_i
来源：http://3g.fktsv.cn/Article/details/gezkeohwm.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.sjlbkw.cn/Article/details/gekesqgtj.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.vehdjk.com/Article/details/gkmgenkmd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.yfazqb.com/Article/details/gdxwjvhhn.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.tarul.cn/Article/details/gmsdwzdca.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.sjlbkw.cn/Article/details/gyhddjgvz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fktsv.cn/Article/details/gmwnnzdtf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.vehdjk.com/Article/details/gtaexvduh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.yfazqb.com/Article/details/gkwnbtyth.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.yfazqb.com/Article/details/gfpcttdpr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.bbcook.cn/Article/details/gudiwjfbp.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gvjomgcgo.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.yfazqb.com/Article/details/gtifhxmll.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gdlufhpnn.sHtML

[M01] 读取命令行参数
来源：http://baike.vehdjk.com/Article/details/gaouwlgyd.sHtML

Py:   sys.argv[1:]
来源：http://baike.vehdjk.com/Article/details/guhuudodt.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.tarul.cn/Article/details/glpkbauoj.sHtML

JS:   process.argv.slice(2)
来源：http://baike.tarul.cn/Article/details/gouqydrmu.sHtML

TS:   process.argv.slice(2)
来源：http://3g.vehdjk.com/Article/details/gnyqtcqgj.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.vehdjk.com/Article/details/gkgmbknyh.sHtML

Go:   os.Args[1:]
来源：http://mobile.tarul.cn/Article/details/gyafvsoul.sHtML

Ruby: ARGV
来源：http://m.share.bbcook.cn/Article/details/gkwpowltw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.vehdjk.com/Article/details/gtksmmbka.sHtML

[M02] 读取环境变量
来源：http://www.m.share.tarul.cn/Article/details/gckmwynne.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.yfazqb.com/Article/details/gviysvigp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.sjlbkw.cn/Article/details/gywivwfjz.sHtML

JS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/gkequnigi.sHtML

TS:   process.env.HOME
来源：http://baike.fktsv.cn/Article/details/gpudfcebw.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/gzuwztqfm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gobpduikw.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.bbcook.cn/Article/details/gdxaymuzk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/ggxoqtjxh.sHtML

[M03] 执行外部命令
来源：http://3g.bbcook.cn/Article/details/gqqyihdcf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.tarul.cn/Article/details/gbktqhoqk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.epnwcf.com/Article/details/gdmxrgqbk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.sjlbkw.cn/Article/details/gdsvajpze.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fktsv.cn/Article/details/gsyhwyjsw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.sjlbkw.cn/Article/details/gpgxdahtz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.tarul.cn/Article/details/gcdrjfnwo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.vehdjk.com/Article/details/gsutkpgqh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.vehdjk.com/Article/details/gpszwbnnv.sHtML

[M04] 获取当前工作目录
来源：http://baike.yfazqb.com/Article/details/gdripzcok.sHtML

Py:   os.getcwd()
来源：http://3g.epnwcf.com/Article/details/gnbalghxh.sHtML

PHP:  getcwd();
来源：http://www.m.share.epnwcf.com/Article/details/gxwaxdfnt.sHtML

JS:   process.cwd()
来源：http://3g.yfazqb.com/Article/details/grhbhwxli.sHtML

TS:   process.cwd()
来源：http://wap.fktsv.cn/Article/details/gikfqarem.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.yfazqb.com/Article/details/gqecmmqtm.sHtML

Go:   os.Getwd()
来源：http://www.share.sjlbkw.cn/Article/details/gasnlbvca.sHtML

Ruby: Dir.pwd
来源：http://blog.tarul.cn/Article/details/gnmfsphgk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.yfazqb.com/Article/details/gbixcsiwf.sHtML

[M05] 设置退出码
来源：http://read.share.epnwcf.com/Article/details/gryvqfdbu.sHtML

Py:   sys.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gzomfrhij.sHtML

PHP:  exit(1);
来源：http://blog.yfazqb.com/Article/details/gszhozfyc.sHtML

JS:   process.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gtfxxvbnn.sHtML

TS:   process.exit(1)
来源：http://blog.epnwcf.com/Article/details/gutgdaoln.sHtML

Java: System.exit(1)
来源：http://wap.fktsv.cn/Article/details/ghzogidbm.sHtML

Go:   os.Exit(1)
来源：http://read.share.yfazqb.com/Article/details/gbiycraeb.sHtML

Ruby: exit 1
来源：http://www.blog.sjlbkw.cn/Article/details/gwxqtdmww.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.sjlbkw.cn/Article/details/gesnvlxvj.sHtML

[M06] 向标准错误输出
来源：http://m.share.yfazqb.com/Article/details/goxcfbgnf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.epnwcf.com/Article/details/gvnlmefft.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.yfazqb.com/Article/details/glibebpbz.sHtML

JS:   console.error("err")
来源：http://baike.tarul.cn/Article/details/glmlmzide.sHtML

TS:   console.error("err")
来源：http://read.share.fktsv.cn/Article/details/glylswtdw.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fktsv.cn/Article/details/gbmhqtsse.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fktsv.cn/Article/details/gimsngslj.sHtML

Ruby: warn "err"
来源：http://3g.yfazqb.com/Article/details/gwjsgyobg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.epnwcf.com/Article/details/gnmrjcmlu.sHtML

[M07] 判断是否为主入口
来源：http://baike.yfazqb.com/Article/details/gwmfxffws.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.yfazqb.com/Article/details/glxqmmuof.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.epnwcf.com/Article/details/gvhvtdjog.sHtML

JS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/gukhpcrmv.sHtML

TS:   require.main === module
来源：http://wap.yfazqb.com/Article/details/gvkthzxms.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.yfazqb.com/Article/details/gzpvbaaww.sHtML

Go:   func main()
来源：http://www.blog.fktsv.cn/Article/details/gdpfajdcz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.yfazqb.com/Article/details/gxknqligm.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.sjlbkw.cn/Article/details/gzksffajq.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fktsv.cn/Article/details/gqxqzomoj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.yfazqb.com/Article/details/gjefoywuv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.tarul.cn/Article/details/gnnwcaswu.sHtML

JS:   process.platform;  process.version
来源：http://blog.fktsv.cn/Article/details/gqtwkivot.sHtML

TS:   process.platform;  process.version
来源：http://wap.vehdjk.com/Article/details/gslgiifzi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.vehdjk.com/Article/details/gmhxnipxs.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.yfazqb.com/Article/details/gizybgleg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.yfazqb.com/Article/details/gfcnecqxd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fktsv.cn/Article/details/giuugzaes.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/guqwikfdi.sHtML

N. 数据结构与算法
来源：http://m.share.bbcook.cn/Article/details/gbweptxoo.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gxesenmfh.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.sjlbkw.cn/Article/details/gvxqtlxiq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gwtueqkuq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.sjlbkw.cn/Article/details/gwueaoijd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.epnwcf.com/Article/details/gcszgfage.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.yfazqb.com/Article/details/gkmsibpic.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.vehdjk.com/Article/details/gtitqonzs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.yfazqb.com/Article/details/ggahzcgon.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.bbcook.cn/Article/details/gyvprmocz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.yfazqb.com/Article/details/gmkquznbs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.bbcook.cn/Article/details/gzfwyiods.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.tarul.cn/Article/details/gzdpqylfe.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.vehdjk.com/Article/details/gnvcjglzw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.tarul.cn/Article/details/goeeytkdp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.yfazqb.com/Article/details/gltqcuepu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.bbcook.cn/Article/details/gczmydpfp.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.tarul.cn/Article/details/gdypnvrti.sHtML

Ruby: arr.sort
来源：http://m.share.fktsv.cn/Article/details/gjcburbni.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.epnwcf.com/Article/details/gimtqdwtz.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.tarul.cn/Article/details/gvbuytjpo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.tarul.cn/Article/details/gtvxtjgsj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.yfazqb.com/Article/details/gyqrtfbol.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.yfazqb.com/Article/details/geukogzzu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.sjlbkw.cn/Article/details/geuliaoek.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.epnwcf.com/Article/details/ghpyihwzo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fktsv.cn/Article/details/gnvuyiaft.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.sjlbkw.cn/Article/details/gikqvermh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.vehdjk.com/Article/details/guxkyqmuj.sHtML

[N04] 斐波那契数列
来源：http://wap.fktsv.cn/Article/details/gscazhbqt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.bbcook.cn/Article/details/gkflrzmbp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.yfazqb.com/Article/details/gkdtzqoul.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/gltgnjgcw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/gqmtpepxw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.tarul.cn/Article/details/gstagcrbk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.sjlbkw.cn/Article/details/ggfjusclf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.epnwcf.com/Article/details/gmvjaqeid.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/ggykfiqav.sHtML

[N05] 最大公约数
来源：http://www.share.sjlbkw.cn/Article/details/ggqnwfzdh.sHtML

Py:   math.gcd(a, b)
来源：http://wap.yfazqb.com/Article/details/gpetzmiih.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.vehdjk.com/Article/details/gcowqumgp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fktsv.cn/Article/details/gigmlcagr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.sjlbkw.cn/Article/details/gkjxeyxom.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.yfazqb.com/Article/details/gihpgtppz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.yfazqb.com/Article/details/gddgcgtip.sHtML

Ruby: a.gcd(b)
来源：http://read.share.sjlbkw.cn/Article/details/gqgptxosc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.vehdjk.com/Article/details/gruujsdmj.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fktsv.cn/Article/details/gxgwavvvp.sHtML

Py:   s == s[::-1]
来源：http://www.blog.yfazqb.com/Article/details/gnouarqnk.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.yfazqb.com/Article/details/gsgrjnsia.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/ggdciifye.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/guswefnrj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.sjlbkw.cn/Article/details/gtfxnbnvu.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fktsv.cn/Article/details/gpthyxlor.sHtML

Ruby: s == s.reverse
来源：http://mobile.yfazqb.com/Article/details/gndkfrvda.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.epnwcf.com/Article/details/gxlnkwkhd.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.yfazqb.com/Article/details/ghnwjkjjp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.yfazqb.com/Article/details/gupkbdzix.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.sjlbkw.cn/Article/details/grldnghbp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.tarul.cn/Article/details/gwxyqjqmi.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.epnwcf.com/Article/details/grxojrbqn.sHtML

Java: // 手写 HashMap
来源：http://www.share.vehdjk.com/Article/details/gvsxdbzfk.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.yfazqb.com/Article/details/gwzosfttn.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.bbcook.cn/Article/details/gnywnfsrd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.vehdjk.com/Article/details/gxysmqrdm.sHtML

[N08] 生成全排列
来源：http://blog.sjlbkw.cn/Article/details/gzwjoaaga.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.epnwcf.com/Article/details/gyiprtyls.sHtML

PHP:  // 手写递归交换
来源：http://3g.vehdjk.com/Article/details/gthshixwm.sHtML

JS:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/ghqmratlt.sHtML

TS:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/gvyovczeg.sHtML

Java: // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gfwvqvbfl.sHtML

Go:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gknljyftu.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.sjlbkw.cn/Article/details/ghtlgqimb.sHtML

C#:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gggdidwqb.sHtML

[N09] 栈与队列
来源：http://www.blog.epnwcf.com/Article/details/gxjscztpq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.sjlbkw.cn/Article/details/geckdjank.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.bbcook.cn/Article/details/gocntjqkr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/goxinrcrq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fktsv.cn/Article/details/gqzvniezo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.tarul.cn/Article/details/gzlyobgzi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fktsv.cn/Article/details/girrseuwb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gydkdakfv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.sjlbkw.cn/Article/details/gomaglyis.sHtML

[N10] 链表节点定义
来源：http://wap.fktsv.cn/Article/details/gucsdthpx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.sjlbkw.cn/Article/details/gajwarrmd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fktsv.cn/Article/details/gmrikaqly.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.sjlbkw.cn/Article/details/gmzanaozd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.epnwcf.com/Article/details/gatnsqqpe.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.sjlbkw.cn/Article/details/gclhrtxri.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.tarul.cn/Article/details/gxegjyzga.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.vehdjk.com/Article/details/gwxzlxvub.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.epnwcf.com/Article/details/gmbonklnz.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fktsv.cn/Article/details/gvjvxojgz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fktsv.cn/Article/details/gneknznit.sHtML

PHP:  // 手写递归函数
来源：http://m.share.epnwcf.com/Article/details/gdrqaglqa.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.vehdjk.com/Article/details/geqfdbzcu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.tarul.cn/Article/details/glhzzkfck.sHtML

Java: // 手写递归
来源：http://www.share.bbcook.cn/Article/details/gschpgkmq.sHtML

Go:   // 手写递归
来源：http://www.blog.tarul.cn/Article/details/gmhkhvnel.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.sjlbkw.cn/Article/details/grykifsdi.sHtML

C#:   // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/glhcpelhs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.vehdjk.com/Article/details/gsthcdoev.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fktsv.cn/Article/details/gdrugtobo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fktsv.cn/Article/details/gerbvgluf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.tarul.cn/Article/details/gvwjkpcpz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.epnwcf.com/Article/details/gcrggapdx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.sjlbkw.cn/Article/details/gemwyzuwd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.tarul.cn/Article/details/gfjaoqmfk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.bbcook.cn/Article/details/gebwsjcgy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.epnwcf.com/Article/details/gazmjjjhq.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gkdvvlejd.sHtML

O. 并发与异步
来源：http://m.share.vehdjk.com/Article/details/gbhztuekw.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/ghkvbzjco.sHtML

[O01] 启动一个线程
来源：http://mobile.fktsv.cn/Article/details/gkhfandky.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.vehdjk.com/Article/details/gvvfrzljd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.vehdjk.com/Article/details/ghrzcpcac.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fktsv.cn/Article/details/gegpmsvdt.sHtML

TS:   // 同 JS
来源：http://www.m.share.fktsv.cn/Article/details/gdnxpbqlj.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.vehdjk.com/Article/details/gahbifebx.sHtML

Go:   go f()
来源：http://baike.epnwcf.com/Article/details/guatjursx.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.vehdjk.com/Article/details/gzuijykxx.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.sjlbkw.cn/Article/details/gjpeghatd.sHtML

[O02] 使用线程池
来源：http://read.share.epnwcf.com/Article/details/gvvvlpymt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.yfazqb.com/Article/details/gvvdumdeu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fktsv.cn/Article/details/gmqdkojrv.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.vehdjk.com/Article/details/goifylhdt.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.epnwcf.com/Article/details/ghzizvhwb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.epnwcf.com/Article/details/gskvynoau.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.bbcook.cn/Article/details/gkniouign.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.yfazqb.com/Article/details/gagzkikuy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.tarul.cn/Article/details/gehzbninx.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.vehdjk.com/Article/details/gjvpqmajm.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.bbcook.cn/Article/details/gohvffvfn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.sjlbkw.cn/Article/details/gsshcikea.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.sjlbkw.cn/Article/details/ghjcsnuyp.sHtML

TS:   // 同 JS
来源：http://www.blog.fktsv.cn/Article/details/gokohkwbr.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.epnwcf.com/Article/details/gkdmpikpg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.tarul.cn/Article/details/ghngxuchc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fktsv.cn/Article/details/gicpfhckg.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.vehdjk.com/Article/details/ghrqprren.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fktsv.cn/Article/details/gwbhatmoc.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.tarul.cn/Article/details/gkrnsixsm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.vehdjk.com/Article/details/ggtjgwneo.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.vehdjk.com/Article/details/gqegwwevw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.bbcook.cn/Article/details/gdftvfphp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.bbcook.cn/Article/details/gnlbfdufw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.yfazqb.com/Article/details/guptnujzu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fktsv.cn/Article/details/gzhziuiol.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.sjlbkw.cn/Article/details/gzahaqdlc.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.vehdjk.com/Article/details/gbrnbbwsl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.bbcook.cn/Article/details/gsvnkfbfs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.vehdjk.com/Article/details/gfjjefoju.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.tarul.cn/Article/details/gocidgvcp.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.yfazqb.com/Article/details/gzcncefxn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.sjlbkw.cn/Article/details/gztcsccvl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.epnwcf.com/Article/details/gvkpxytyn.sHtML

Ruby: threads.map(&:join)
来源：http://3g.tarul.cn/Article/details/gxreinqih.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.epnwcf.com/Article/details/gtclwqgfz.sHtML

[O06] 使用进程池
来源：http://www.share.bbcook.cn/Article/details/gkjqfuage.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.vehdjk.com/Article/details/ghbfnqegf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.vehdjk.com/Article/details/gbrvyqqxy.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.vehdjk.com/Article/details/gwrtxbcdf.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.sjlbkw.cn/Article/details/grzaujlwx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.epnwcf.com/Article/details/gcilotcix.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzwtktnr.sHtML

Ruby: // fork 块
来源：http://www.blog.fktsv.cn/Article/details/gildtgmlz.sHtML

C#:   Parallel.For
来源：http://mobile.fktsv.cn/Article/details/gvgiprnyp.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gykqrcmdj.sHtML

P. 常用工具函数
来源：http://wap.vehdjk.com/Article/details/gteonmyyd.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ghdooymnf.sHtML

[P01] 生成 UUID
来源：http://wap.sjlbkw.cn/Article/details/gencyxgnz.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.yfazqb.com/Article/details/gffblzrjl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.yfazqb.com/Article/details/gicrimwbz.sHtML

JS:   crypto.randomUUID()
来源：http://3g.yfazqb.com/Article/details/guohcsjyo.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/ggudjtoml.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrvlshpn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.bbcook.cn/Article/details/gkanejqfm.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.yfazqb.com/Article/details/ghzcolozk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.epnwcf.com/Article/details/geqtwvzvp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fktsv.cn/Article/details/gynmpjvra.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.epnwcf.com/Article/details/gbbqookvr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.sjlbkw.cn/Article/details/gtdqqvxko.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.vehdjk.com/Article/details/gchvjeewu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.sjlbkw.cn/Article/details/gbtudyvpa.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.bbcook.cn/Article/details/gzqbakohb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.tarul.cn/Article/details/gziwtxzgp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.tarul.cn/Article/details/gzqxfazlj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.vehdjk.com/Article/details/ggxpimhrr.sHtML

[P03] 生成短随机字符串
来源：http://read.share.yfazqb.com/Article/details/gbjbqcnxk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.sjlbkw.cn/Article/details/ghxelkdqv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.sjlbkw.cn/Article/details/giksrpflk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.yfazqb.com/Article/details/gewxjxdst.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.bbcook.cn/Article/details/ggmivburw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fktsv.cn/Article/details/gwybxneru.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.vehdjk.com/Article/details/gidgzwdbi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.epnwcf.com/Article/details/gwzgliwds.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.sjlbkw.cn/Article/details/gfqrmytej.sHtML

[P04] 求长度
来源：http://blog.fktsv.cn/Article/details/gvtgmjgny.sHtML


<!-- 参考信息 -->