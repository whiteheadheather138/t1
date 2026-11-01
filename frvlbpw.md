代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.vehdjk.com/Article/details/gbqjahcqa.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fktsv.cn/Article/details/ghsjjnvxn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gjyzjmxke.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gvbcqkmaq.sHtML

Py:   resp.json()
来源：http://www.m.share.fktsv.cn/Article/details/gmssjysip.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.vehdjk.com/Article/details/gmiaxakug.sHtML

JS:   await resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/gmtfszoiu.sHtML

TS:   await resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/gxrollnrc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.yfazqb.com/Article/details/gyweilgch.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.bbcook.cn/Article/details/gtfstdxhh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fktsv.cn/Article/details/gnhmoihqn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.sjlbkw.cn/Article/details/gtwgxetet.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.sjlbkw.cn/Article/details/gftpbzswd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.yfazqb.com/Article/details/gxjgamuin.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.bbcook.cn/Article/details/gzhqgaggh.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.vehdjk.com/Article/details/gncsolzds.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.sjlbkw.cn/Article/details/gttdmilmy.sHtML

Java: resp.statusCode()
来源：http://wap.bbcook.cn/Article/details/gsgxuvkfx.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.yfazqb.com/Article/details/gyeskmaxx.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fktsv.cn/Article/details/gchpbdvol.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.bbcook.cn/Article/details/gggfnvvmz.sHtML

[L08] 并发请求多个地址
来源：http://baike.fktsv.cn/Article/details/gniarjpwn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.yfazqb.com/Article/details/gacsyvekp.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.yfazqb.com/Article/details/gvdlvacmo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.bbcook.cn/Article/details/gblgzbwdh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.sjlbkw.cn/Article/details/gfipkmmnj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.yfazqb.com/Article/details/gtgfljnzm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.tarul.cn/Article/details/gsudjbnxe.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.sjlbkw.cn/Article/details/gpmpilwev.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fktsv.cn/Article/details/gmxgzocfh.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/ghsjutwuu.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.vehdjk.com/Article/details/gdhhvipxb.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gqptxupth.sHtML

[M01] 读取命令行参数
来源：http://baike.yfazqb.com/Article/details/gacfrhfkd.sHtML

Py:   sys.argv[1:]
来源：http://mobile.bbcook.cn/Article/details/gmnzvxuux.sHtML

PHP:  $argv;  $argc;
来源：http://3g.bbcook.cn/Article/details/gdldlzecu.sHtML

JS:   process.argv.slice(2)
来源：http://3g.bbcook.cn/Article/details/gmjfswzix.sHtML

TS:   process.argv.slice(2)
来源：http://blog.sjlbkw.cn/Article/details/gpkcoxabu.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.bbcook.cn/Article/details/geaqndubf.sHtML

Go:   os.Args[1:]
来源：http://3g.fktsv.cn/Article/details/gqftuwcun.sHtML

Ruby: ARGV
来源：http://baike.fktsv.cn/Article/details/gdppfshix.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.tarul.cn/Article/details/gpcyouyio.sHtML

[M02] 读取环境变量
来源：http://www.blog.yfazqb.com/Article/details/ggpuylygu.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.epnwcf.com/Article/details/grvnjyrcc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.bbcook.cn/Article/details/gzxbffunh.sHtML

JS:   process.env.HOME
来源：http://m.share.vehdjk.com/Article/details/grjprjukx.sHtML

TS:   process.env.HOME
来源：http://www.share.bbcook.cn/Article/details/govmxtasz.sHtML

Java: System.getenv("HOME")
来源：http://www.share.bbcook.cn/Article/details/gyppcqwgj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.epnwcf.com/Article/details/gymbbqrdb.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.tarul.cn/Article/details/gtyyswxyl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gjzbeolux.sHtML

[M03] 执行外部命令
来源：http://read.share.yfazqb.com/Article/details/gmcvfrdfk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fktsv.cn/Article/details/gptmhslbd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.sjlbkw.cn/Article/details/gresudkuw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.bbcook.cn/Article/details/gekkgpzwf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.tarul.cn/Article/details/gvxlpzvvr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.yfazqb.com/Article/details/gffbzusdi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.tarul.cn/Article/details/gyaliuyrf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.epnwcf.com/Article/details/gliktcihx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.bbcook.cn/Article/details/gtsgufeqh.sHtML

[M04] 获取当前工作目录
来源：http://3g.bbcook.cn/Article/details/gxqmjbsuv.sHtML

Py:   os.getcwd()
来源：http://read.share.sjlbkw.cn/Article/details/guzdrypcb.sHtML

PHP:  getcwd();
来源：http://www.share.sjlbkw.cn/Article/details/gjojvszsu.sHtML

JS:   process.cwd()
来源：http://mobile.yfazqb.com/Article/details/gutoruxvt.sHtML

TS:   process.cwd()
来源：http://www.blog.fktsv.cn/Article/details/gwjetgcai.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.vehdjk.com/Article/details/gnjmpjcqv.sHtML

Go:   os.Getwd()
来源：http://wap.tarul.cn/Article/details/gqinsjttg.sHtML

Ruby: Dir.pwd
来源：http://3g.fktsv.cn/Article/details/gyyljnhzs.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.sjlbkw.cn/Article/details/grkqxlbfd.sHtML

[M05] 设置退出码
来源：http://3g.vehdjk.com/Article/details/grzppozmj.sHtML

Py:   sys.exit(1)
来源：http://read.share.tarul.cn/Article/details/gunrmdraq.sHtML

PHP:  exit(1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gttavnktk.sHtML

JS:   process.exit(1)
来源：http://baike.fktsv.cn/Article/details/gocspjhba.sHtML

TS:   process.exit(1)
来源：http://baike.bbcook.cn/Article/details/gpvwffthq.sHtML

Java: System.exit(1)
来源：http://blog.fktsv.cn/Article/details/gbruuqwew.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gusrsjyhv.sHtML

Ruby: exit 1
来源：http://read.share.bbcook.cn/Article/details/gmumaeyyi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.sjlbkw.cn/Article/details/gmuaoxbju.sHtML

[M06] 向标准错误输出
来源：http://wap.bbcook.cn/Article/details/giopzecxd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.epnwcf.com/Article/details/gzwnduqvk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.sjlbkw.cn/Article/details/gtefjfaqf.sHtML

JS:   console.error("err")
来源：http://read.share.sjlbkw.cn/Article/details/gmaaevytw.sHtML

TS:   console.error("err")
来源：http://wap.fktsv.cn/Article/details/gynhrnuvj.sHtML

Java: System.err.println("err")
来源：http://read.share.epnwcf.com/Article/details/gaqbudium.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.tarul.cn/Article/details/gsthygqym.sHtML

Ruby: warn "err"
来源：http://m.share.tarul.cn/Article/details/gazeotpge.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.vehdjk.com/Article/details/glqirbgft.sHtML

[M07] 判断是否为主入口
来源：http://www.share.yfazqb.com/Article/details/gjltmgnmh.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.yfazqb.com/Article/details/gbxtkwtcr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.yfazqb.com/Article/details/gzlwrrdoc.sHtML

JS:   require.main === module
来源：http://3g.vehdjk.com/Article/details/gqnvxrpbl.sHtML

TS:   require.main === module
来源：http://mobile.sjlbkw.cn/Article/details/gzplbmumh.sHtML

Java: public static void main(String[] args)
来源：http://m.share.epnwcf.com/Article/details/gzxovzcft.sHtML

Go:   func main()
来源：http://mobile.epnwcf.com/Article/details/gydehxnuv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.epnwcf.com/Article/details/gaqorvafu.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.tarul.cn/Article/details/gpwqdkvpl.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.yfazqb.com/Article/details/grijgaijo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fktsv.cn/Article/details/gxewjadhh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.vehdjk.com/Article/details/grldbpmmt.sHtML

JS:   process.platform;  process.version
来源：http://baike.vehdjk.com/Article/details/glezithqc.sHtML

TS:   process.platform;  process.version
来源：http://blog.epnwcf.com/Article/details/gypyupwkj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.yfazqb.com/Article/details/gevlzwwpl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fktsv.cn/Article/details/gdqudbgwl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.epnwcf.com/Article/details/gtrxqjdii.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.epnwcf.com/Article/details/geqfmtiih.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gpmcherdh.sHtML

N. 数据结构与算法
来源：http://3g.tarul.cn/Article/details/goqckdjjp.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gjgrmwgde.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fktsv.cn/Article/details/gasalbsjf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gjghvzwje.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.tarul.cn/Article/details/gtciqiwqy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fktsv.cn/Article/details/guckhizbt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/gkxlnqxzm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.tarul.cn/Article/details/gufzqycjp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gbdtxpwag.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.vehdjk.com/Article/details/gtmtkhwle.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fktsv.cn/Article/details/gcnmcbfqt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.tarul.cn/Article/details/gyyixcxma.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.epnwcf.com/Article/details/gomfcdckn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.sjlbkw.cn/Article/details/gzpwzozis.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/ghqyyxfbb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fktsv.cn/Article/details/gfbmkkims.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.bbcook.cn/Article/details/geemwcmtl.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.yfazqb.com/Article/details/guxueusuc.sHtML

Ruby: arr.sort
来源：http://blog.fktsv.cn/Article/details/gucvcroco.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.vehdjk.com/Article/details/gurbhqsvg.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.tarul.cn/Article/details/gehbujeia.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fktsv.cn/Article/details/grywuculk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.bbcook.cn/Article/details/gtixqgxbt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.epnwcf.com/Article/details/gimskslcu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.vehdjk.com/Article/details/gzjqpqdyv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.epnwcf.com/Article/details/gqgskgvnj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.bbcook.cn/Article/details/glrpqkzwe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fktsv.cn/Article/details/gfhtxyivy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fktsv.cn/Article/details/gxlkvnjov.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.tarul.cn/Article/details/glmxejupf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.yfazqb.com/Article/details/gcpuvicas.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fktsv.cn/Article/details/gsyfgvlka.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.vehdjk.com/Article/details/giwevgbpn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.bbcook.cn/Article/details/gqwrumafn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.tarul.cn/Article/details/gxtuwckor.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.tarul.cn/Article/details/gldizswfh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.sjlbkw.cn/Article/details/govhsngqm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.epnwcf.com/Article/details/gaghezkss.sHtML

[N05] 最大公约数
来源：http://www.blog.fktsv.cn/Article/details/gumaeuqrs.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsnizsnlq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.vehdjk.com/Article/details/glsniqzte.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.sjlbkw.cn/Article/details/gwvdjupob.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.epnwcf.com/Article/details/gkgbapzqm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.sjlbkw.cn/Article/details/gdznfufvm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.vehdjk.com/Article/details/gccphvzam.sHtML

Ruby: a.gcd(b)
来源：http://3g.fktsv.cn/Article/details/gwtxyeivx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.tarul.cn/Article/details/gkqqgtzom.sHtML

[N06] 判断回文字符串
来源：http://www.share.tarul.cn/Article/details/gohsguaop.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.yfazqb.com/Article/details/gvkquuxfq.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.tarul.cn/Article/details/gqyxbrtpv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/gldgtxaah.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/giwixfehp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.yfazqb.com/Article/details/garoxbdys.sHtML

Go:   // 双指针从两端比较
来源：http://blog.sjlbkw.cn/Article/details/gvomwkuio.sHtML

Ruby: s == s.reverse
来源：http://read.share.fktsv.cn/Article/details/gdcwkzshx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.yfazqb.com/Article/details/gzsrgmsjm.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.epnwcf.com/Article/details/gnpiwqitl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.sjlbkw.cn/Article/details/gwjshdqjh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.bbcook.cn/Article/details/gktuvimgs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fktsv.cn/Article/details/gknoprwlc.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fktsv.cn/Article/details/giyenoemo.sHtML

Java: // 手写 HashMap
来源：http://www.blog.tarul.cn/Article/details/gngrpycax.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.yfazqb.com/Article/details/gqrqlfdwj.sHtML

Ruby: // 手写 Hash
来源：http://baike.vehdjk.com/Article/details/gusdkidcr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.sjlbkw.cn/Article/details/gmbrhzvmq.sHtML

[N08] 生成全排列
来源：http://read.share.sjlbkw.cn/Article/details/gayofyryv.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.vehdjk.com/Article/details/gwmwagweu.sHtML

PHP:  // 手写递归交换
来源：http://wap.yfazqb.com/Article/details/gyzjumkys.sHtML

JS:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gdjdmekbk.sHtML

TS:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/grabuzaqq.sHtML

Java: // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gfcocqmwa.sHtML

Go:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/glsoggddk.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.tarul.cn/Article/details/gjdmrnlhk.sHtML

C#:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gbvttsmbj.sHtML

[N09] 栈与队列
来源：http://read.share.fktsv.cn/Article/details/gsdncydmi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fktsv.cn/Article/details/gzaomeelr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.bbcook.cn/Article/details/gdnrxypqj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fktsv.cn/Article/details/gajjdgijf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.vehdjk.com/Article/details/gysehwyaz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.epnwcf.com/Article/details/gfohghcya.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.tarul.cn/Article/details/gijpcrjny.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.epnwcf.com/Article/details/grakcguvc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.epnwcf.com/Article/details/ggphrjoku.sHtML

[N10] 链表节点定义
来源：http://www.share.epnwcf.com/Article/details/gcljrbenn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.epnwcf.com/Article/details/glgpwwubd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.epnwcf.com/Article/details/gydqciidr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.yfazqb.com/Article/details/gevyrqyxn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.tarul.cn/Article/details/gshrxvhhx.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fktsv.cn/Article/details/ghqpldpyv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.epnwcf.com/Article/details/gwgudvogy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.yfazqb.com/Article/details/gloabrmyd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fktsv.cn/Article/details/gyronlgrt.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fktsv.cn/Article/details/guxbgtgba.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.epnwcf.com/Article/details/gqvruhemj.sHtML

PHP:  // 手写递归函数
来源：http://baike.yfazqb.com/Article/details/gplpeoxuc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.yfazqb.com/Article/details/gsmpmupsy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.yfazqb.com/Article/details/gcnmxcrdh.sHtML

Java: // 手写递归
来源：http://3g.yfazqb.com/Article/details/gzkncarfd.sHtML

Go:   // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gajdwmkjh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.bbcook.cn/Article/details/gyzxjppus.sHtML

C#:   // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/gvueuhiwk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.tarul.cn/Article/details/gzaaoijbr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.epnwcf.com/Article/details/gnindnkmx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.sjlbkw.cn/Article/details/gqbfsxuls.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/gyfjvjslv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.vehdjk.com/Article/details/gitjsldms.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.epnwcf.com/Article/details/gscijwbbl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.vehdjk.com/Article/details/gxdtlmwaa.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.yfazqb.com/Article/details/gqcogtfgw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.vehdjk.com/Article/details/gsnbcecly.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gtpnksjcd.sHtML

O. 并发与异步
来源：http://blog.fktsv.cn/Article/details/guzpcmqvl.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gholgrcfm.sHtML

[O01] 启动一个线程
来源：http://blog.yfazqb.com/Article/details/gwmnnrhfn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.bbcook.cn/Article/details/ggqvaxoif.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.tarul.cn/Article/details/guhplwrjr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.sjlbkw.cn/Article/details/gmduitcor.sHtML

TS:   // 同 JS
来源：http://www.blog.vehdjk.com/Article/details/gjkbmzmoq.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.bbcook.cn/Article/details/gzvxmipko.sHtML

Go:   go f()
来源：http://www.m.share.vehdjk.com/Article/details/gewflfshw.sHtML

Ruby: Thread.new { f }
来源：http://mobile.yfazqb.com/Article/details/gareuxbkg.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fktsv.cn/Article/details/gkpgnhkrw.sHtML

[O02] 使用线程池
来源：http://www.blog.sjlbkw.cn/Article/details/gidkugymg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.yfazqb.com/Article/details/gjgamvjku.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fktsv.cn/Article/details/gyvxxgdic.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fktsv.cn/Article/details/ghderccew.sHtML

TS:   // worker_threads 线程池
来源：http://blog.tarul.cn/Article/details/geiqbyagb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.vehdjk.com/Article/details/glhcgszay.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.yfazqb.com/Article/details/geaqbheqe.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.vehdjk.com/Article/details/goidwjayv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.bbcook.cn/Article/details/gkahmuwch.sHtML

[O03] 加锁保护共享数据
来源：http://wap.tarul.cn/Article/details/gkkfsfmcv.sHtML

Py:   with lock: shared += 1
来源：http://read.share.bbcook.cn/Article/details/gdldklgcr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.tarul.cn/Article/details/gocsgnorx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.yfazqb.com/Article/details/glratuxpc.sHtML

TS:   // 同 JS
来源：http://mobile.yfazqb.com/Article/details/glpdzkmzx.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fktsv.cn/Article/details/gwweibiqu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.epnwcf.com/Article/details/gsywfbzva.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fktsv.cn/Article/details/gjpgczlgr.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.tarul.cn/Article/details/gzpitzgaj.sHtML

[O04] 定义异步函数并等待
来源：http://baike.epnwcf.com/Article/details/gccaipzxg.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.vehdjk.com/Article/details/gkmrsvadr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.tarul.cn/Article/details/ghevzfwqm.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fktsv.cn/Article/details/gumytparr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.tarul.cn/Article/details/gjayqlsdq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.tarul.cn/Article/details/geupxkcvs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.bbcook.cn/Article/details/gjmzwwrts.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.sjlbkw.cn/Article/details/goecsnbia.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.epnwcf.com/Article/details/gcesgvavd.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fktsv.cn/Article/details/gvurtzryk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.sjlbkw.cn/Article/details/gukpmjtnx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.sjlbkw.cn/Article/details/gfozqlgap.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.epnwcf.com/Article/details/giuhrljck.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.sjlbkw.cn/Article/details/gbbrsclgc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.sjlbkw.cn/Article/details/gsyantehj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.yfazqb.com/Article/details/gpzwulcmv.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fktsv.cn/Article/details/gigguvalq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.epnwcf.com/Article/details/gwiebydcp.sHtML

[O06] 使用进程池
来源：http://mobile.epnwcf.com/Article/details/gdfirxpxd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fktsv.cn/Article/details/gpfiszmzz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.epnwcf.com/Article/details/gjisyoldv.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.epnwcf.com/Article/details/gjsjwkqyu.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.epnwcf.com/Article/details/gnhlhsghi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.sjlbkw.cn/Article/details/gbmximiox.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.bbcook.cn/Article/details/gzuqeywql.sHtML

Ruby: // fork 块
来源：http://3g.sjlbkw.cn/Article/details/gjuhvknoq.sHtML

C#:   Parallel.For
来源：http://3g.tarul.cn/Article/details/gtuwktfrj.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gnpjguyry.sHtML

P. 常用工具函数
来源：http://baike.tarul.cn/Article/details/grenooknl.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gmmnuvjlt.sHtML

[P01] 生成 UUID
来源：http://wap.fktsv.cn/Article/details/ggyyzjxsf.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.sjlbkw.cn/Article/details/gmavdfwox.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.tarul.cn/Article/details/ghdvoyypu.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.vehdjk.com/Article/details/gikxhquzp.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.tarul.cn/Article/details/gyxibwhwv.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.tarul.cn/Article/details/gbtzhvghv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.vehdjk.com/Article/details/gjtxygiio.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.vehdjk.com/Article/details/gmvnwjkdz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fktsv.cn/Article/details/gsafohwfa.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.yfazqb.com/Article/details/gbxpiyytt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.yfazqb.com/Article/details/grlvtrzkw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.tarul.cn/Article/details/gbnetzwqy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.bbcook.cn/Article/details/gmswvagzm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.yfazqb.com/Article/details/gpqjiktjk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.yfazqb.com/Article/details/gsggpqswq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.bbcook.cn/Article/details/gpqxvpggu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.bbcook.cn/Article/details/gatrcnrxu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.bbcook.cn/Article/details/gakaotuls.sHtML

[P03] 生成短随机字符串
来源：http://m.share.tarul.cn/Article/details/gsveedxdr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.yfazqb.com/Article/details/giwmbjlpw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.yfazqb.com/Article/details/gjaevmmax.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.bbcook.cn/Article/details/ggmiyzmwe.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.tarul.cn/Article/details/gfcvmgckb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.epnwcf.com/Article/details/gkvnsihsx.sHtML


<!-- 参考信息 -->