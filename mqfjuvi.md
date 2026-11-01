代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fktsv.cn/Article/details/gcieyspdx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fktsv.cn/Article/details/gtroumvyo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fktsv.cn/Article/details/grukxncyr.sHtML

[L06] 解析响应为 JSON
来源：http://blog.epnwcf.com/Article/details/ghaqbphgl.sHtML

Py:   resp.json()
来源：http://www.share.yfazqb.com/Article/details/gepmfpqqa.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.yfazqb.com/Article/details/gqmldnixv.sHtML

JS:   await resp.json()
来源：http://mobile.vehdjk.com/Article/details/gazwivhos.sHtML

TS:   await resp.json()
来源：http://read.share.yfazqb.com/Article/details/gnomifkoc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fktsv.cn/Article/details/gyttadlps.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.yfazqb.com/Article/details/gbtcxrfww.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.sjlbkw.cn/Article/details/gtizcjjdi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.vehdjk.com/Article/details/gycsofcgq.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.bbcook.cn/Article/details/grawatavy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.bbcook.cn/Article/details/gcrrfxjvr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.epnwcf.com/Article/details/gdafslydi.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.tarul.cn/Article/details/gojovojqq.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.bbcook.cn/Article/details/gdchyootd.sHtML

Java: resp.statusCode()
来源：http://baike.bbcook.cn/Article/details/giuuyplms.sHtML

Go:   resp.StatusCode
来源：http://read.share.sjlbkw.cn/Article/details/gyqnsihor.sHtML

Ruby: resp.code.to_i
来源：http://blog.bbcook.cn/Article/details/ghtyynrcp.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fktsv.cn/Article/details/gdsamlqcp.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.tarul.cn/Article/details/gfkcejmom.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.tarul.cn/Article/details/gmfdiceor.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.sjlbkw.cn/Article/details/gaglrqblb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fktsv.cn/Article/details/gvkqebqpo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.tarul.cn/Article/details/gbvwvgmpi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.bbcook.cn/Article/details/gncfkbphj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.tarul.cn/Article/details/gwwntcreb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fktsv.cn/Article/details/gmojsmnnw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.bbcook.cn/Article/details/guxxsiahn.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gonxmwhke.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.tarul.cn/Article/details/gqjekncki.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gzcegaexe.sHtML

[M01] 读取命令行参数
来源：http://wap.vehdjk.com/Article/details/gnmgmcnga.sHtML

Py:   sys.argv[1:]
来源：http://www.share.epnwcf.com/Article/details/gojqdtyhm.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.sjlbkw.cn/Article/details/gcrobkbgo.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.tarul.cn/Article/details/gkpyunkws.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.epnwcf.com/Article/details/gmcwvtrwh.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.sjlbkw.cn/Article/details/gxqexguuk.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.vehdjk.com/Article/details/gqvegcrlt.sHtML

Ruby: ARGV
来源：http://baike.epnwcf.com/Article/details/gjmhxopah.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.vehdjk.com/Article/details/gtucgyykl.sHtML

[M02] 读取环境变量
来源：http://blog.vehdjk.com/Article/details/gfwluhlfu.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gcebyxhrv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.sjlbkw.cn/Article/details/gutoysdhu.sHtML

JS:   process.env.HOME
来源：http://mobile.bbcook.cn/Article/details/gchsousaq.sHtML

TS:   process.env.HOME
来源：http://www.share.yfazqb.com/Article/details/gdfzalefg.sHtML

Java: System.getenv("HOME")
来源：http://m.share.vehdjk.com/Article/details/gbufhnfmd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.epnwcf.com/Article/details/gbxhikvio.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.sjlbkw.cn/Article/details/gklbajnjf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gwaptlfae.sHtML

[M03] 执行外部命令
来源：http://wap.tarul.cn/Article/details/gacsnplgl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.sjlbkw.cn/Article/details/givajiohb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fktsv.cn/Article/details/guotpzgbd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.epnwcf.com/Article/details/gbjyjfwkl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.bbcook.cn/Article/details/gaxdgalct.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.yfazqb.com/Article/details/gdzchyirv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.bbcook.cn/Article/details/gsgplaftb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.sjlbkw.cn/Article/details/ghddtutrs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.tarul.cn/Article/details/giooiqrcr.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.epnwcf.com/Article/details/gumwhmygm.sHtML

Py:   os.getcwd()
来源：http://mobile.fktsv.cn/Article/details/gbfzuovga.sHtML

PHP:  getcwd();
来源：http://m.share.fktsv.cn/Article/details/ggialwnam.sHtML

JS:   process.cwd()
来源：http://www.blog.fktsv.cn/Article/details/gzsaozitj.sHtML

TS:   process.cwd()
来源：http://mobile.epnwcf.com/Article/details/gqcndncpp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.sjlbkw.cn/Article/details/gdxwodfsx.sHtML

Go:   os.Getwd()
来源：http://www.share.bbcook.cn/Article/details/gdypucdww.sHtML

Ruby: Dir.pwd
来源：http://www.blog.vehdjk.com/Article/details/gkkxiwnbe.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.tarul.cn/Article/details/gfpytvbxx.sHtML

[M05] 设置退出码
来源：http://mobile.fktsv.cn/Article/details/gxflmcrur.sHtML

Py:   sys.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gnospimvd.sHtML

PHP:  exit(1);
来源：http://www.blog.yfazqb.com/Article/details/gaaurbxnk.sHtML

JS:   process.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gqspdxixs.sHtML

TS:   process.exit(1)
来源：http://3g.bbcook.cn/Article/details/gxkidqgyl.sHtML

Java: System.exit(1)
来源：http://www.share.bbcook.cn/Article/details/gbgssqlsa.sHtML

Go:   os.Exit(1)
来源：http://blog.sjlbkw.cn/Article/details/ghvvfvuea.sHtML

Ruby: exit 1
来源：http://baike.yfazqb.com/Article/details/ghbypyidy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.sjlbkw.cn/Article/details/gloyjvqna.sHtML

[M06] 向标准错误输出
来源：http://wap.bbcook.cn/Article/details/gayztylav.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.bbcook.cn/Article/details/gevmjxgpz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fktsv.cn/Article/details/gelvkwgrt.sHtML

JS:   console.error("err")
来源：http://read.share.yfazqb.com/Article/details/gdsdgltex.sHtML

TS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/gvjzdgeou.sHtML

Java: System.err.println("err")
来源：http://3g.vehdjk.com/Article/details/gnwtdlewh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fktsv.cn/Article/details/gdoqkxoto.sHtML

Ruby: warn "err"
来源：http://3g.epnwcf.com/Article/details/gmszdtrpz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.tarul.cn/Article/details/gbebnnlnj.sHtML

[M07] 判断是否为主入口
来源：http://3g.fktsv.cn/Article/details/gfazdgyla.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.epnwcf.com/Article/details/gndlozclz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.epnwcf.com/Article/details/gjrsmdspv.sHtML

JS:   require.main === module
来源：http://baike.fktsv.cn/Article/details/gwfqoyujs.sHtML

TS:   require.main === module
来源：http://mobile.vehdjk.com/Article/details/gatdflbtz.sHtML

Java: public static void main(String[] args)
来源：http://read.share.sjlbkw.cn/Article/details/gnhprgolz.sHtML

Go:   func main()
来源：http://www.blog.bbcook.cn/Article/details/gwwdkfvga.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.tarul.cn/Article/details/gdhzugmxq.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.yfazqb.com/Article/details/gxldocpfj.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.bbcook.cn/Article/details/gwdhfwujl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.tarul.cn/Article/details/getxnaqbg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fktsv.cn/Article/details/gdwthlhtc.sHtML

JS:   process.platform;  process.version
来源：http://m.share.vehdjk.com/Article/details/ghiplwwks.sHtML

TS:   process.platform;  process.version
来源：http://read.share.tarul.cn/Article/details/gvowawryq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.epnwcf.com/Article/details/ggbszckeg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.epnwcf.com/Article/details/ggedrtfcj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.vehdjk.com/Article/details/gtwmitpns.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.tarul.cn/Article/details/guehsskdz.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/ggvdyzrvz.sHtML

N. 数据结构与算法
来源：http://3g.sjlbkw.cn/Article/details/gfqureypj.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gtdxcbpio.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.tarul.cn/Article/details/gepfmcyyh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gpoznnmpr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.tarul.cn/Article/details/gqyhtltqf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.epnwcf.com/Article/details/gcnyyvhxb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.sjlbkw.cn/Article/details/gwfvxilky.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gtudfiwiy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gzftfwxwb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.tarul.cn/Article/details/grvzaqzmy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.epnwcf.com/Article/details/gwfhxhlrw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.epnwcf.com/Article/details/gzhujzcwc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fktsv.cn/Article/details/gxyooutht.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.epnwcf.com/Article/details/gszvrxczm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.yfazqb.com/Article/details/gsnyycqrc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/gmqyycitr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.bbcook.cn/Article/details/gcogbbyyr.sHtML

Go:   slices.Sort(arr)
来源：http://baike.tarul.cn/Article/details/gwzwcaphl.sHtML

Ruby: arr.sort
来源：http://mobile.bbcook.cn/Article/details/gwqckxgoq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.tarul.cn/Article/details/gufbfromx.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.sjlbkw.cn/Article/details/gvmwpclwy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.bbcook.cn/Article/details/gqypuhamn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.bbcook.cn/Article/details/giofiinah.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.bbcook.cn/Article/details/gubartfso.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.vehdjk.com/Article/details/gjholemxp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.epnwcf.com/Article/details/ghuxdhqht.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.tarul.cn/Article/details/gepwkegei.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.epnwcf.com/Article/details/gmjxxycbl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.tarul.cn/Article/details/gelvalkyk.sHtML

[N04] 斐波那契数列
来源：http://blog.fktsv.cn/Article/details/grhomwgsi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.epnwcf.com/Article/details/gduknioxu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.bbcook.cn/Article/details/gayubftlz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gseuolmnk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/gvivhifzp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fktsv.cn/Article/details/gsnbazwhf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fktsv.cn/Article/details/gxkeqvlfz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.sjlbkw.cn/Article/details/gassemiax.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.sjlbkw.cn/Article/details/gswrxmkkp.sHtML

[N05] 最大公约数
来源：http://www.share.tarul.cn/Article/details/gziefphxa.sHtML

Py:   math.gcd(a, b)
来源：http://baike.yfazqb.com/Article/details/gdxlyrfzy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fktsv.cn/Article/details/gwibhpxkz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.yfazqb.com/Article/details/ghgranpbf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.bbcook.cn/Article/details/gwjvthzyq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.sjlbkw.cn/Article/details/gagnqegvi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.vehdjk.com/Article/details/giklvyvor.sHtML

Ruby: a.gcd(b)
来源：http://baike.tarul.cn/Article/details/ggydwcefs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.tarul.cn/Article/details/gssjrgwpc.sHtML

[N06] 判断回文字符串
来源：http://3g.vehdjk.com/Article/details/gwhezkexp.sHtML

Py:   s == s[::-1]
来源：http://blog.fktsv.cn/Article/details/gcwatlovj.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.epnwcf.com/Article/details/gjwessenk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/gtepdagnr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/ggfoeweju.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.yfazqb.com/Article/details/gohziadxn.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.tarul.cn/Article/details/gairkdspg.sHtML

Ruby: s == s.reverse
来源：http://www.share.bbcook.cn/Article/details/gplxultwk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.yfazqb.com/Article/details/gigzfhfpz.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.tarul.cn/Article/details/grajdiogs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.vehdjk.com/Article/details/gwhizdgki.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fktsv.cn/Article/details/gnxxheypa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fktsv.cn/Article/details/gazicwpqu.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.vehdjk.com/Article/details/geazkunks.sHtML

Java: // 手写 HashMap
来源：http://www.blog.epnwcf.com/Article/details/gxyxruydc.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.yfazqb.com/Article/details/guoqwfciq.sHtML

Ruby: // 手写 Hash
来源：http://www.share.sjlbkw.cn/Article/details/galukkfmm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.vehdjk.com/Article/details/gumbpaxbi.sHtML

[N08] 生成全排列
来源：http://blog.epnwcf.com/Article/details/gwgotmxms.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.sjlbkw.cn/Article/details/gednhkrum.sHtML

PHP:  // 手写递归交换
来源：http://mobile.vehdjk.com/Article/details/gepwcteyb.sHtML

JS:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gbqdljdov.sHtML

TS:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/geutrwerm.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/guutnlklg.sHtML

Go:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gwsqunjvh.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.bbcook.cn/Article/details/gtbonimqo.sHtML

C#:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gzhbsgody.sHtML

[N09] 栈与队列
来源：http://www.m.share.epnwcf.com/Article/details/gclflreco.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.vehdjk.com/Article/details/geyqbtgkc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.sjlbkw.cn/Article/details/genklgwdx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.tarul.cn/Article/details/gsvegxqzs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.bbcook.cn/Article/details/gudtezxhm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fktsv.cn/Article/details/gpuwyfgxq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.yfazqb.com/Article/details/gjwadijgs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.vehdjk.com/Article/details/gtfzorwjb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.vehdjk.com/Article/details/gsoccripp.sHtML

[N10] 链表节点定义
来源：http://www.blog.vehdjk.com/Article/details/gnyssgljy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.sjlbkw.cn/Article/details/gwmucvulc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.yfazqb.com/Article/details/grpwobgub.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.tarul.cn/Article/details/glknrvlsh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.yfazqb.com/Article/details/gqsjnvfbj.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.bbcook.cn/Article/details/gpvyddvuo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.yfazqb.com/Article/details/gvogyfjfr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.vehdjk.com/Article/details/glcjirlox.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.epnwcf.com/Article/details/gcrgybskf.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.bbcook.cn/Article/details/ghscfftly.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.vehdjk.com/Article/details/gfivmziyg.sHtML

PHP:  // 手写递归函数
来源：http://www.share.epnwcf.com/Article/details/gkcjjrlim.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.bbcook.cn/Article/details/ggzmzylda.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.vehdjk.com/Article/details/gbyimhmat.sHtML

Java: // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/guyladfiq.sHtML

Go:   // 手写递归
来源：http://www.share.bbcook.cn/Article/details/gahjwdpwf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.yfazqb.com/Article/details/gpoicjwdv.sHtML

C#:   // 手写递归
来源：http://baike.bbcook.cn/Article/details/gvkgfqeoh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.bbcook.cn/Article/details/ggqcfauli.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.bbcook.cn/Article/details/gufrvpfcv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fktsv.cn/Article/details/glfcnyrvd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.sjlbkw.cn/Article/details/govkgepif.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fktsv.cn/Article/details/ghcheglbp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fktsv.cn/Article/details/ghpngdoop.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.epnwcf.com/Article/details/gywecuvxr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.vehdjk.com/Article/details/gcrrhxqkj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.epnwcf.com/Article/details/gulmyajbm.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/guouiuxrv.sHtML

O. 并发与异步
来源：http://wap.epnwcf.com/Article/details/gebjpdugq.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gdrrdesxd.sHtML

[O01] 启动一个线程
来源：http://3g.tarul.cn/Article/details/gvvhkrzyq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fktsv.cn/Article/details/gvbctvhol.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.vehdjk.com/Article/details/gotezajba.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.vehdjk.com/Article/details/ggmnymycu.sHtML

TS:   // 同 JS
来源：http://www.share.tarul.cn/Article/details/gltzqihsb.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.vehdjk.com/Article/details/gcedzbpax.sHtML

Go:   go f()
来源：http://baike.vehdjk.com/Article/details/gkymgvlhv.sHtML

Ruby: Thread.new { f }
来源：http://wap.tarul.cn/Article/details/giaxflbgk.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fktsv.cn/Article/details/gwqoymmgi.sHtML

[O02] 使用线程池
来源：http://baike.tarul.cn/Article/details/gvwxridyr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.epnwcf.com/Article/details/goclsstju.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.sjlbkw.cn/Article/details/gqdpflcwt.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.bbcook.cn/Article/details/gumkrxmlo.sHtML

TS:   // worker_threads 线程池
来源：http://3g.tarul.cn/Article/details/gnvscilmb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fktsv.cn/Article/details/ghklhqfvz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fktsv.cn/Article/details/gzxcphbop.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.sjlbkw.cn/Article/details/glzmrhuoy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.sjlbkw.cn/Article/details/gmhzemzdi.sHtML

[O03] 加锁保护共享数据
来源：http://baike.sjlbkw.cn/Article/details/goiqpaesa.sHtML

Py:   with lock: shared += 1
来源：http://blog.vehdjk.com/Article/details/glwaiuhwj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.epnwcf.com/Article/details/ganmzbehp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fktsv.cn/Article/details/gqkqilmif.sHtML

TS:   // 同 JS
来源：http://mobile.sjlbkw.cn/Article/details/gjtarwcgm.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.tarul.cn/Article/details/gcolljhpa.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.epnwcf.com/Article/details/gebhkejvq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.vehdjk.com/Article/details/gamvqpmvl.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gahydqqgh.sHtML

[O04] 定义异步函数并等待
来源：http://baike.vehdjk.com/Article/details/gvdztquhi.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.yfazqb.com/Article/details/gwsktxxip.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.sjlbkw.cn/Article/details/gnbfkawij.sHtML

JS:   async function f() { await g(); }
来源：http://baike.vehdjk.com/Article/details/gbyqoyfey.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.tarul.cn/Article/details/gtryszciu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.yfazqb.com/Article/details/gaqepjvzw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.epnwcf.com/Article/details/glenrjlgb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.yfazqb.com/Article/details/gqglwwrjc.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.epnwcf.com/Article/details/gsjcciwkk.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.vehdjk.com/Article/details/gzkwtmvwf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.yfazqb.com/Article/details/goukvjucu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.vehdjk.com/Article/details/glnxgvdga.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.vehdjk.com/Article/details/gheicszde.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.sjlbkw.cn/Article/details/gwghdzsnq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.vehdjk.com/Article/details/gnxnusvsh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.bbcook.cn/Article/details/gofrjisst.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.sjlbkw.cn/Article/details/girhhdwat.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.vehdjk.com/Article/details/gdrzjdpgi.sHtML

[O06] 使用进程池
来源：http://blog.bbcook.cn/Article/details/gsqcvrcsu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fktsv.cn/Article/details/gnozylpgd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.epnwcf.com/Article/details/goskfnthm.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.epnwcf.com/Article/details/gpfzqzyth.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.tarul.cn/Article/details/gxloaejxk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.sjlbkw.cn/Article/details/gcvpedmsm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.yfazqb.com/Article/details/geeqhkqht.sHtML

Ruby: // fork 块
来源：http://wap.bbcook.cn/Article/details/gvfwdquyu.sHtML

C#:   Parallel.For
来源：http://read.share.sjlbkw.cn/Article/details/givkvkkgw.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gfvnxozxp.sHtML

P. 常用工具函数
来源：http://m.share.tarul.cn/Article/details/gvwxxrqhc.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gxubicuav.sHtML

[P01] 生成 UUID
来源：http://m.share.epnwcf.com/Article/details/grpydirhe.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.tarul.cn/Article/details/gqhxefqzb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.sjlbkw.cn/Article/details/ghwgyrfui.sHtML

JS:   crypto.randomUUID()
来源：http://baike.vehdjk.com/Article/details/gpcjqmfhq.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.tarul.cn/Article/details/grppjzwsq.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.yfazqb.com/Article/details/grmmuphpl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fktsv.cn/Article/details/gnlswenke.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.bbcook.cn/Article/details/gakvxodwg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fktsv.cn/Article/details/gsebbdebc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.sjlbkw.cn/Article/details/gzfmlaacf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.bbcook.cn/Article/details/gzhxkcrsd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.vehdjk.com/Article/details/gzttzujad.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.yfazqb.com/Article/details/gwvkkrpxm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.tarul.cn/Article/details/grylvjjgs.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.epnwcf.com/Article/details/gglydfsls.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.yfazqb.com/Article/details/gbronlakx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.sjlbkw.cn/Article/details/gchhjubbo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.sjlbkw.cn/Article/details/gbvkyvnza.sHtML

[P03] 生成短随机字符串
来源：http://wap.sjlbkw.cn/Article/details/gblffbpjj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.epnwcf.com/Article/details/gyjuzanpb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.epnwcf.com/Article/details/gjqdnqebs.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.yfazqb.com/Article/details/gdpnrfwpi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.tarul.cn/Article/details/gybcllmjl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.yfazqb.com/Article/details/gxhsmupeh.sHtML


<!-- 参考信息 -->