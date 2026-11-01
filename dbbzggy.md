代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.sjlbkw.cn/Article/details/grwzoqfhw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.sjlbkw.cn/Article/details/gdzvfshin.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.bbcook.cn/Article/details/gwiedeeil.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fktsv.cn/Article/details/ghbvxhpfr.sHtML

Py:   resp.json()
来源：http://mobile.vehdjk.com/Article/details/gbtbjxfot.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.bbcook.cn/Article/details/gzwmcwqin.sHtML

JS:   await resp.json()
来源：http://mobile.tarul.cn/Article/details/gqjjihynz.sHtML

TS:   await resp.json()
来源：http://read.share.yfazqb.com/Article/details/gennwvfis.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.bbcook.cn/Article/details/gejxtqzzh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.sjlbkw.cn/Article/details/gbprapgcz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fktsv.cn/Article/details/gspavqncx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.bbcook.cn/Article/details/grzsgpoto.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.yfazqb.com/Article/details/gzbwunpsk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.epnwcf.com/Article/details/gwncnejtk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.sjlbkw.cn/Article/details/guygzdesy.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.vehdjk.com/Article/details/gqlvqwspb.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.yfazqb.com/Article/details/gwdnqemlt.sHtML

Java: resp.statusCode()
来源：http://blog.tarul.cn/Article/details/glpyramap.sHtML

Go:   resp.StatusCode
来源：http://www.blog.epnwcf.com/Article/details/gywigqkyy.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.epnwcf.com/Article/details/gpkcqkfcd.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.epnwcf.com/Article/details/geapvgbub.sHtML

[L08] 并发请求多个地址
来源：http://blog.bbcook.cn/Article/details/goeqxjdhj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.epnwcf.com/Article/details/gvfyirxnv.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.epnwcf.com/Article/details/gshfogyro.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.tarul.cn/Article/details/gtkquubxl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gbrzmoudj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.yfazqb.com/Article/details/grjulurwk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.sjlbkw.cn/Article/details/gwdhkqftu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.yfazqb.com/Article/details/gezxiywyr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.bbcook.cn/Article/details/gxwfpcvas.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gupeiskzc.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fktsv.cn/Article/details/gpozimvyg.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gklnbdsrg.sHtML

[M01] 读取命令行参数
来源：http://mobile.tarul.cn/Article/details/gjuxjonnl.sHtML

Py:   sys.argv[1:]
来源：http://3g.fktsv.cn/Article/details/gvplajjgc.sHtML

PHP:  $argv;  $argc;
来源：http://wap.vehdjk.com/Article/details/gadevdqnv.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fktsv.cn/Article/details/gmlezcadu.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.yfazqb.com/Article/details/ggevftmyx.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.yfazqb.com/Article/details/gotcgpwal.sHtML

Go:   os.Args[1:]
来源：http://baike.yfazqb.com/Article/details/geeszfxoi.sHtML

Ruby: ARGV
来源：http://mobile.bbcook.cn/Article/details/gszqvmwuc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.vehdjk.com/Article/details/gnluhnhmv.sHtML

[M02] 读取环境变量
来源：http://read.share.yfazqb.com/Article/details/ghuhpuppf.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.tarul.cn/Article/details/gnoosnpux.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.yfazqb.com/Article/details/gebmmqihc.sHtML

JS:   process.env.HOME
来源：http://m.share.fktsv.cn/Article/details/ghuhmpxes.sHtML

TS:   process.env.HOME
来源：http://baike.sjlbkw.cn/Article/details/gratjehir.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fktsv.cn/Article/details/gpryydjdw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fktsv.cn/Article/details/gqtyatwyo.sHtML

Ruby: ENV["HOME"]
来源：http://blog.tarul.cn/Article/details/ghheyxmxi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gngcrewwc.sHtML

[M03] 执行外部命令
来源：http://www.share.epnwcf.com/Article/details/gjxlggrth.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.sjlbkw.cn/Article/details/gcfejhwca.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.sjlbkw.cn/Article/details/glnzfjnsg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.bbcook.cn/Article/details/ghkknxlmp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.yfazqb.com/Article/details/gyamfuxms.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.vehdjk.com/Article/details/gmyessfus.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fktsv.cn/Article/details/gcmupmytb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fktsv.cn/Article/details/gqqxqdedt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.yfazqb.com/Article/details/ghhwdylns.sHtML

[M04] 获取当前工作目录
来源：http://blog.fktsv.cn/Article/details/gqrtqhkat.sHtML

Py:   os.getcwd()
来源：http://www.share.epnwcf.com/Article/details/gxgugomco.sHtML

PHP:  getcwd();
来源：http://m.share.bbcook.cn/Article/details/gzegwexmy.sHtML

JS:   process.cwd()
来源：http://wap.yfazqb.com/Article/details/greczbmcb.sHtML

TS:   process.cwd()
来源：http://wap.yfazqb.com/Article/details/gagapqasr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fktsv.cn/Article/details/gldjwmzbu.sHtML

Go:   os.Getwd()
来源：http://mobile.tarul.cn/Article/details/gkbqnmjkk.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjbhkxkh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.yfazqb.com/Article/details/gmybctzji.sHtML

[M05] 设置退出码
来源：http://m.share.vehdjk.com/Article/details/gtixzdjmx.sHtML

Py:   sys.exit(1)
来源：http://www.share.bbcook.cn/Article/details/gepzxwimc.sHtML

PHP:  exit(1);
来源：http://read.share.bbcook.cn/Article/details/gctbgbxwn.sHtML

JS:   process.exit(1)
来源：http://www.share.epnwcf.com/Article/details/glseyrszw.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/galpsbpmc.sHtML

Java: System.exit(1)
来源：http://wap.epnwcf.com/Article/details/gxqjbtzuh.sHtML

Go:   os.Exit(1)
来源：http://www.share.vehdjk.com/Article/details/gonpcosrq.sHtML

Ruby: exit 1
来源：http://3g.fktsv.cn/Article/details/gxezwvmfz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.sjlbkw.cn/Article/details/gfguimzan.sHtML

[M06] 向标准错误输出
来源：http://blog.bbcook.cn/Article/details/gsgtcqgyk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.epnwcf.com/Article/details/gahldvrkt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.yfazqb.com/Article/details/ginndbkui.sHtML

JS:   console.error("err")
来源：http://read.share.tarul.cn/Article/details/glyatetpj.sHtML

TS:   console.error("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqcagiszm.sHtML

Java: System.err.println("err")
来源：http://www.blog.epnwcf.com/Article/details/gwpfbbeaq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.bbcook.cn/Article/details/gpbrwtukc.sHtML

Ruby: warn "err"
来源：http://www.blog.bbcook.cn/Article/details/gqklahqyd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.epnwcf.com/Article/details/gsyzneovh.sHtML

[M07] 判断是否为主入口
来源：http://3g.yfazqb.com/Article/details/gsiqdyqij.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fktsv.cn/Article/details/gczasdrpo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fktsv.cn/Article/details/gceqyvask.sHtML

JS:   require.main === module
来源：http://m.share.vehdjk.com/Article/details/gujlbulbo.sHtML

TS:   require.main === module
来源：http://read.share.epnwcf.com/Article/details/ghqouzebo.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdgrtmeke.sHtML

Go:   func main()
来源：http://read.share.epnwcf.com/Article/details/gcmsdefng.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.epnwcf.com/Article/details/gzulpkfys.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.yfazqb.com/Article/details/ggyjupatf.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.tarul.cn/Article/details/gcuhbrkor.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fktsv.cn/Article/details/gjrdngoiu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.yfazqb.com/Article/details/gowqbujps.sHtML

JS:   process.platform;  process.version
来源：http://m.share.epnwcf.com/Article/details/gxspvuksx.sHtML

TS:   process.platform;  process.version
来源：http://m.share.sjlbkw.cn/Article/details/geydremai.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fktsv.cn/Article/details/grvqdtmna.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.bbcook.cn/Article/details/gziazeusz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.tarul.cn/Article/details/gddnzcflg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.epnwcf.com/Article/details/ghtzaqjfd.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/glurhlbdw.sHtML

N. 数据结构与算法
来源：http://mobile.bbcook.cn/Article/details/gwbxuaaef.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gcufgkngo.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.sjlbkw.cn/Article/details/gstbxdcbu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gwrznocyr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fktsv.cn/Article/details/goccpshrp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/gsgfiknpw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.sjlbkw.cn/Article/details/ghxmgjjrb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gyryaqfrc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gicvkjtnf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.epnwcf.com/Article/details/gahuqnfdi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.tarul.cn/Article/details/gqqjdfcjc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.yfazqb.com/Article/details/gpevnawji.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.vehdjk.com/Article/details/gwgwrozou.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.tarul.cn/Article/details/ggofremzj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/gysdubijb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.sjlbkw.cn/Article/details/goqrdmcyl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.bbcook.cn/Article/details/ginclfriv.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gstguppda.sHtML

Ruby: arr.sort
来源：http://www.blog.sjlbkw.cn/Article/details/glokdwztc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.sjlbkw.cn/Article/details/grnagbosy.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.tarul.cn/Article/details/gcybakpul.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.tarul.cn/Article/details/gdexdrbrn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fktsv.cn/Article/details/gahwedbad.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.vehdjk.com/Article/details/gsauplgzr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.tarul.cn/Article/details/gjtwddwrf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.bbcook.cn/Article/details/glbwszity.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.sjlbkw.cn/Article/details/gbyqmvcgv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.epnwcf.com/Article/details/gsbeinfzf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.yfazqb.com/Article/details/gyvvrapbx.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fktsv.cn/Article/details/gvvirxvvw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.tarul.cn/Article/details/ghydykpqi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.yfazqb.com/Article/details/giohcddid.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/gwnjfxrsb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/gowoovptl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.yfazqb.com/Article/details/guyaenbpc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.vehdjk.com/Article/details/glglhtzdc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.bbcook.cn/Article/details/gyzxrvqhw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gltkyyblw.sHtML

[N05] 最大公约数
来源：http://www.share.fktsv.cn/Article/details/gbsbzzlfy.sHtML

Py:   math.gcd(a, b)
来源：http://blog.yfazqb.com/Article/details/gxgzxeeyr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.tarul.cn/Article/details/gfulkcpks.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.yfazqb.com/Article/details/gkdidpaoj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.sjlbkw.cn/Article/details/gqkmhqrle.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.vehdjk.com/Article/details/gyyzrnpsh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.yfazqb.com/Article/details/gnaocezao.sHtML

Ruby: a.gcd(b)
来源：http://baike.yfazqb.com/Article/details/gdwszazml.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.yfazqb.com/Article/details/gmitztxbo.sHtML

[N06] 判断回文字符串
来源：http://3g.yfazqb.com/Article/details/gbllzljbj.sHtML

Py:   s == s[::-1]
来源：http://wap.yfazqb.com/Article/details/gozaeqsbq.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.yfazqb.com/Article/details/guzuznmgd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/gmbhqhzjr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/gkeftzobl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.epnwcf.com/Article/details/gxsumkach.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.sjlbkw.cn/Article/details/gxlftwexu.sHtML

Ruby: s == s.reverse
来源：http://blog.fktsv.cn/Article/details/gxncffwdb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.sjlbkw.cn/Article/details/gdgsyazab.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fktsv.cn/Article/details/gujzqoile.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.tarul.cn/Article/details/gwubgbtti.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.yfazqb.com/Article/details/gysohwklt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.tarul.cn/Article/details/gshyrfmxp.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.epnwcf.com/Article/details/grgoazqru.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.sjlbkw.cn/Article/details/gikwadazq.sHtML

Go:   // 手写 map[int]int
来源：http://wap.vehdjk.com/Article/details/gjwohdjke.sHtML

Ruby: // 手写 Hash
来源：http://wap.vehdjk.com/Article/details/glkoefhbc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.sjlbkw.cn/Article/details/gdnjniual.sHtML

[N08] 生成全排列
来源：http://m.share.bbcook.cn/Article/details/gufgvxzbs.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.vehdjk.com/Article/details/gterkfqre.sHtML

PHP:  // 手写递归交换
来源：http://m.share.bbcook.cn/Article/details/gruraklbl.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gyhpybzpk.sHtML

TS:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/ggoubegas.sHtML

Java: // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gszpfknzj.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gfcokctre.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.epnwcf.com/Article/details/gmzbiazxc.sHtML

C#:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gilisueuy.sHtML

[N09] 栈与队列
来源：http://blog.bbcook.cn/Article/details/gqqmxjkdh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.yfazqb.com/Article/details/gecvfqmaw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/godqzusiw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.tarul.cn/Article/details/gxqeepkxh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.bbcook.cn/Article/details/gxuirnrxd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.bbcook.cn/Article/details/gleuauigz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.vehdjk.com/Article/details/gmvbjqcnu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.tarul.cn/Article/details/gkwsaatgt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fktsv.cn/Article/details/garrzrncu.sHtML

[N10] 链表节点定义
来源：http://baike.vehdjk.com/Article/details/goavsylcf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.tarul.cn/Article/details/gcqdpxwdl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.epnwcf.com/Article/details/gewbbwnui.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.sjlbkw.cn/Article/details/gkaaxotch.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.vehdjk.com/Article/details/gmvjvkvkx.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.vehdjk.com/Article/details/gailppawd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.sjlbkw.cn/Article/details/gdavoiyiv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.bbcook.cn/Article/details/gryvghvbc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.bbcook.cn/Article/details/gukpajmny.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.tarul.cn/Article/details/gklduyyvu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.sjlbkw.cn/Article/details/gjjnbqfve.sHtML

PHP:  // 手写递归函数
来源：http://mobile.epnwcf.com/Article/details/gjgdgkwar.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.sjlbkw.cn/Article/details/ggtrrvkgb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.vehdjk.com/Article/details/gruhdznof.sHtML

Java: // 手写递归
来源：http://blog.vehdjk.com/Article/details/gtkwspuyt.sHtML

Go:   // 手写递归
来源：http://3g.vehdjk.com/Article/details/gomppygbb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fktsv.cn/Article/details/gghrhrzjh.sHtML

C#:   // 手写递归
来源：http://www.blog.vehdjk.com/Article/details/gnfmjhimw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.tarul.cn/Article/details/gyjqzlhix.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.sjlbkw.cn/Article/details/gbsrafmdc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.bbcook.cn/Article/details/glvvjhkrt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.yfazqb.com/Article/details/gpbylwoib.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.yfazqb.com/Article/details/gmpeocfev.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fktsv.cn/Article/details/gsignvdvm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fktsv.cn/Article/details/gnefzmblp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.bbcook.cn/Article/details/gbpwaqxkc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.yfazqb.com/Article/details/gxugpqbda.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gyqihkjyz.sHtML

O. 并发与异步
来源：http://m.share.tarul.cn/Article/details/ghqfdaibn.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gnwblrwrh.sHtML

[O01] 启动一个线程
来源：http://read.share.yfazqb.com/Article/details/gascpgegb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.tarul.cn/Article/details/gxjquomhp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.epnwcf.com/Article/details/gxfpthvqv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhgecyoo.sHtML

TS:   // 同 JS
来源：http://www.m.share.tarul.cn/Article/details/gucekztgw.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.vehdjk.com/Article/details/gsbwiklmm.sHtML

Go:   go f()
来源：http://m.share.yfazqb.com/Article/details/gzddjrpwe.sHtML

Ruby: Thread.new { f }
来源：http://mobile.bbcook.cn/Article/details/gabgumayz.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.yfazqb.com/Article/details/gyuxbucwa.sHtML

[O02] 使用线程池
来源：http://m.share.fktsv.cn/Article/details/ggrorsxuk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.sjlbkw.cn/Article/details/gsijnxxoy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.yfazqb.com/Article/details/glicoaoai.sHtML

JS:   // worker_threads 线程池
来源：http://blog.yfazqb.com/Article/details/gkhphjxyh.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.tarul.cn/Article/details/gctqjnlki.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.yfazqb.com/Article/details/gbkxggukj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.yfazqb.com/Article/details/grjiatlea.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.sjlbkw.cn/Article/details/gfalrtstt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.yfazqb.com/Article/details/gimkctjhc.sHtML

[O03] 加锁保护共享数据
来源：http://blog.epnwcf.com/Article/details/gniulcueg.sHtML

Py:   with lock: shared += 1
来源：http://baike.bbcook.cn/Article/details/gusjorzhm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fktsv.cn/Article/details/gunxexjfr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.yfazqb.com/Article/details/gagcfkkbx.sHtML

TS:   // 同 JS
来源：http://www.blog.yfazqb.com/Article/details/gfcvdovar.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fktsv.cn/Article/details/ginpheczw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.yfazqb.com/Article/details/gqqkybjxm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.epnwcf.com/Article/details/gevvzumbi.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.vehdjk.com/Article/details/gmdzeovoc.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fktsv.cn/Article/details/gzhkmolqv.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.tarul.cn/Article/details/gtprnjrft.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.epnwcf.com/Article/details/gejwqmjsn.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.sjlbkw.cn/Article/details/geciehvnh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.yfazqb.com/Article/details/gyacgyawk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.sjlbkw.cn/Article/details/gjurnlwpy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.tarul.cn/Article/details/ghxegpyog.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fktsv.cn/Article/details/gjmmdscoz.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.tarul.cn/Article/details/giqteqjdn.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.bbcook.cn/Article/details/gpbogdmkh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.tarul.cn/Article/details/gfkqqozxg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.bbcook.cn/Article/details/gbqiocuhd.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.epnwcf.com/Article/details/gbbzjwzjk.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.epnwcf.com/Article/details/ghnoktfor.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.yfazqb.com/Article/details/gtpxugblj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.bbcook.cn/Article/details/gttvmdgjt.sHtML

Ruby: threads.map(&:join)
来源：http://baike.yfazqb.com/Article/details/gjzelcnhs.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.epnwcf.com/Article/details/guwbkhznd.sHtML

[O06] 使用进程池
来源：http://www.m.share.fktsv.cn/Article/details/ggzybzljy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fktsv.cn/Article/details/gzasqivzx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.vehdjk.com/Article/details/gzqongysu.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.epnwcf.com/Article/details/gsxgazcrd.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.bbcook.cn/Article/details/gxbxrufwm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fktsv.cn/Article/details/geudzebpk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.bbcook.cn/Article/details/guefiwksz.sHtML

Ruby: // fork 块
来源：http://blog.epnwcf.com/Article/details/gxaljshih.sHtML

C#:   Parallel.For
来源：http://m.share.sjlbkw.cn/Article/details/gsnbaiwgj.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/grpcgwepn.sHtML

P. 常用工具函数
来源：http://www.blog.sjlbkw.cn/Article/details/govnqhirv.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gvzzdstpb.sHtML

[P01] 生成 UUID
来源：http://www.blog.fktsv.cn/Article/details/gdhyzzrep.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.vehdjk.com/Article/details/gsotvlpxo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fktsv.cn/Article/details/gksxoavny.sHtML

JS:   crypto.randomUUID()
来源：http://3g.bbcook.cn/Article/details/gvxeuqdog.sHtML

TS:   crypto.randomUUID()
来源：http://wap.sjlbkw.cn/Article/details/gkqmruyrn.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fktsv.cn/Article/details/gndnmfxnx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/gyyxjzpll.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.vehdjk.com/Article/details/gbuzsmcvp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.tarul.cn/Article/details/gtduvxkbp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.bbcook.cn/Article/details/glllxqtkm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.vehdjk.com/Article/details/gmahofqfy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.yfazqb.com/Article/details/gasazpetd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.bbcook.cn/Article/details/ghupuvrmr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.yfazqb.com/Article/details/gaqohnvgi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/gmajwvxlj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fktsv.cn/Article/details/gmngkacvj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fktsv.cn/Article/details/giqduohuy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.bbcook.cn/Article/details/gjgqpktws.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.tarul.cn/Article/details/gqvjcncku.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhggxofc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.sjlbkw.cn/Article/details/guusoktwf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.tarul.cn/Article/details/gilhxamzg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.yfazqb.com/Article/details/gaacmllrx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.epnwcf.com/Article/details/gdhgjhclj.sHtML


<!-- 参考信息 -->