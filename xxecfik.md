代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.tarul.cn/Article/details/gnjzfcdfu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.vehdjk.com/Article/details/grpqvjphk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.bbcook.cn/Article/details/gtictwxrc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.epnwcf.com/Article/details/gvgjfprtn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.tarul.cn/Article/details/gawcppvea.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.tarul.cn/Article/details/gkarnhkpk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.epnwcf.com/Article/details/gedqkdetl.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.epnwcf.com/Article/details/gvfmenvou.sHtML

Py:   resp.json()
来源：http://www.blog.yfazqb.com/Article/details/gcftdezar.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.vehdjk.com/Article/details/gaopbcdad.sHtML

JS:   await resp.json()
来源：http://read.share.fktsv.cn/Article/details/gakvyjyqk.sHtML

TS:   await resp.json()
来源：http://baike.tarul.cn/Article/details/gboowzfkm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.epnwcf.com/Article/details/gvxsgdjqy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fktsv.cn/Article/details/gryrtjfju.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.bbcook.cn/Article/details/glkgwiwke.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.sjlbkw.cn/Article/details/gvqxjjego.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.epnwcf.com/Article/details/gkeovudko.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.epnwcf.com/Article/details/gscvzaxbt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.vehdjk.com/Article/details/gngbalwsk.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.epnwcf.com/Article/details/gqonyrfit.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.sjlbkw.cn/Article/details/gevjftslv.sHtML

Java: resp.statusCode()
来源：http://read.share.bbcook.cn/Article/details/gmeeodqei.sHtML

Go:   resp.StatusCode
来源：http://www.blog.sjlbkw.cn/Article/details/gmxenaedg.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.tarul.cn/Article/details/gmurdpizz.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.epnwcf.com/Article/details/gjzgdurnv.sHtML

[L08] 并发请求多个地址
来源：http://baike.vehdjk.com/Article/details/gpjknbsht.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.bbcook.cn/Article/details/gkfyxepmy.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.vehdjk.com/Article/details/gsmcmiaqv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.tarul.cn/Article/details/gmwczvatm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/ggrhrykql.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.sjlbkw.cn/Article/details/gwjswtgfj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.tarul.cn/Article/details/gfolbkiew.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.epnwcf.com/Article/details/gvoqjnvma.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.bbcook.cn/Article/details/gglefijss.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gfyrvjkfc.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fktsv.cn/Article/details/gbwxpadni.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gnhqjplzu.sHtML

[M01] 读取命令行参数
来源：http://blog.epnwcf.com/Article/details/gwqepxdew.sHtML

Py:   sys.argv[1:]
来源：http://mobile.tarul.cn/Article/details/getjquwrq.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.vehdjk.com/Article/details/gdeluitqc.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.vehdjk.com/Article/details/gfkfvfiba.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.tarul.cn/Article/details/ggjvyvhks.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.sjlbkw.cn/Article/details/glfkyybyt.sHtML

Go:   os.Args[1:]
来源：http://mobile.fktsv.cn/Article/details/gowwtbbsl.sHtML

Ruby: ARGV
来源：http://mobile.sjlbkw.cn/Article/details/ggnffyfcc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.sjlbkw.cn/Article/details/gwnugtevg.sHtML

[M02] 读取环境变量
来源：http://www.share.yfazqb.com/Article/details/gohvdvuys.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fktsv.cn/Article/details/gzgryjfqu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fktsv.cn/Article/details/gzksohuym.sHtML

JS:   process.env.HOME
来源：http://wap.bbcook.cn/Article/details/gikmkodoz.sHtML

TS:   process.env.HOME
来源：http://mobile.yfazqb.com/Article/details/glqbyhymc.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gsxmnpbtk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.bbcook.cn/Article/details/gqcqqknkn.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.yfazqb.com/Article/details/ggpaimsrz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.vehdjk.com/Article/details/gmakeikwu.sHtML

[M03] 执行外部命令
来源：http://read.share.bbcook.cn/Article/details/gtgpnxovb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.tarul.cn/Article/details/gffxocttf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.vehdjk.com/Article/details/gogaypnrx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.yfazqb.com/Article/details/gtesdgdwg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.epnwcf.com/Article/details/gpoxgztut.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.vehdjk.com/Article/details/gyaroavfu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.yfazqb.com/Article/details/gnxurcbeq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.bbcook.cn/Article/details/gknsutmqb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.yfazqb.com/Article/details/gtqkogvvx.sHtML

[M04] 获取当前工作目录
来源：http://wap.tarul.cn/Article/details/gqvdtwlab.sHtML

Py:   os.getcwd()
来源：http://read.share.tarul.cn/Article/details/gmaqzytyj.sHtML

PHP:  getcwd();
来源：http://m.share.sjlbkw.cn/Article/details/gwctenwsj.sHtML

JS:   process.cwd()
来源：http://m.share.bbcook.cn/Article/details/gjluqhofo.sHtML

TS:   process.cwd()
来源：http://wap.vehdjk.com/Article/details/gkvxegrba.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.yfazqb.com/Article/details/gdvkbjmfh.sHtML

Go:   os.Getwd()
来源：http://read.share.vehdjk.com/Article/details/gktkzvufa.sHtML

Ruby: Dir.pwd
来源：http://m.share.yfazqb.com/Article/details/gcckppmht.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fktsv.cn/Article/details/gundtsnlr.sHtML

[M05] 设置退出码
来源：http://www.blog.tarul.cn/Article/details/gnsuyywwk.sHtML

Py:   sys.exit(1)
来源：http://baike.epnwcf.com/Article/details/geypenbya.sHtML

PHP:  exit(1);
来源：http://www.share.sjlbkw.cn/Article/details/ggdarlgjl.sHtML

JS:   process.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gmoyxzsei.sHtML

TS:   process.exit(1)
来源：http://www.share.yfazqb.com/Article/details/glqpfrlbu.sHtML

Java: System.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gklopypux.sHtML

Go:   os.Exit(1)
来源：http://www.share.yfazqb.com/Article/details/gisxikany.sHtML

Ruby: exit 1
来源：http://3g.yfazqb.com/Article/details/gybeaghdg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.epnwcf.com/Article/details/gsrhgcgbt.sHtML

[M06] 向标准错误输出
来源：http://www.blog.yfazqb.com/Article/details/glwtamzhu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.sjlbkw.cn/Article/details/gqbgwmnei.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.vehdjk.com/Article/details/gadhggryz.sHtML

JS:   console.error("err")
来源：http://www.m.share.bbcook.cn/Article/details/gjcyqavpj.sHtML

TS:   console.error("err")
来源：http://m.share.bbcook.cn/Article/details/gxbcfghmz.sHtML

Java: System.err.println("err")
来源：http://www.share.fktsv.cn/Article/details/gxlqgjxjr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.sjlbkw.cn/Article/details/gbmxbkdpo.sHtML

Ruby: warn "err"
来源：http://read.share.bbcook.cn/Article/details/gzzttbhet.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.sjlbkw.cn/Article/details/ggersddwd.sHtML

[M07] 判断是否为主入口
来源：http://baike.bbcook.cn/Article/details/gatefegyu.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.vehdjk.com/Article/details/gnssdrlez.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.epnwcf.com/Article/details/gfesgucdh.sHtML

JS:   require.main === module
来源：http://baike.vehdjk.com/Article/details/guhgiqzjy.sHtML

TS:   require.main === module
来源：http://baike.epnwcf.com/Article/details/gtxyoeybb.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.bbcook.cn/Article/details/glpgfumwm.sHtML

Go:   func main()
来源：http://mobile.sjlbkw.cn/Article/details/guukfmtlc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.tarul.cn/Article/details/glxylckyu.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.yfazqb.com/Article/details/gmraoqdzl.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.vehdjk.com/Article/details/gwxverexl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.bbcook.cn/Article/details/gqvnhmjum.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.yfazqb.com/Article/details/guapfihhv.sHtML

JS:   process.platform;  process.version
来源：http://m.share.bbcook.cn/Article/details/gjvksshrb.sHtML

TS:   process.platform;  process.version
来源：http://wap.tarul.cn/Article/details/gcvgmxjwq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.vehdjk.com/Article/details/gmlgylqsw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.epnwcf.com/Article/details/gdaudrqlc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.sjlbkw.cn/Article/details/glesobqyt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.epnwcf.com/Article/details/gzyawrseh.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gglgkpkjx.sHtML

N. 数据结构与算法
来源：http://3g.sjlbkw.cn/Article/details/gjzvgcojq.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/ghvzwgamc.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fktsv.cn/Article/details/gzwopsvfc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fktsv.cn/Article/details/gnxivgjaf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.tarul.cn/Article/details/guhssffni.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.yfazqb.com/Article/details/glcixgpdj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.bbcook.cn/Article/details/gswcayokd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.tarul.cn/Article/details/gsvmncmcg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/glnobguzt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.bbcook.cn/Article/details/ggnlxtqsh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/guasdwlqa.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.epnwcf.com/Article/details/gaoulzkpi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.tarul.cn/Article/details/gjtxmqzmh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.vehdjk.com/Article/details/guvoigqki.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.yfazqb.com/Article/details/gtayulxya.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.vehdjk.com/Article/details/gsckvkhgn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.epnwcf.com/Article/details/gvtlmdflx.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.yfazqb.com/Article/details/gwnorlkjc.sHtML

Ruby: arr.sort
来源：http://m.share.tarul.cn/Article/details/gnlasbqcs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.sjlbkw.cn/Article/details/gbsnzynja.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.sjlbkw.cn/Article/details/gplnfhgij.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fktsv.cn/Article/details/grywyjzpg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.vehdjk.com/Article/details/grvthdfoc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.yfazqb.com/Article/details/gswzslwhb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.vehdjk.com/Article/details/gtaozedxw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.vehdjk.com/Article/details/ghecpfuau.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.sjlbkw.cn/Article/details/gafuqzbpt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.tarul.cn/Article/details/gndpwcges.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.bbcook.cn/Article/details/gtqmzmwwe.sHtML

[N04] 斐波那契数列
来源：http://read.share.yfazqb.com/Article/details/gxhsuplmo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.sjlbkw.cn/Article/details/gwwltqxml.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.tarul.cn/Article/details/gflmxxubh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.yfazqb.com/Article/details/gwmjxnvju.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.yfazqb.com/Article/details/gbtilzfnk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.yfazqb.com/Article/details/gwbenuxas.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.epnwcf.com/Article/details/gdvxcklzr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.vehdjk.com/Article/details/gwsovdfix.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/glijrhxmv.sHtML

[N05] 最大公约数
来源：http://3g.epnwcf.com/Article/details/gcjudlpwq.sHtML

Py:   math.gcd(a, b)
来源：http://3g.yfazqb.com/Article/details/gdyjpmlar.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.epnwcf.com/Article/details/gnfcvileu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.vehdjk.com/Article/details/gwuthpsgy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.epnwcf.com/Article/details/gtmmvsewa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.vehdjk.com/Article/details/gyypkttst.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.bbcook.cn/Article/details/gxzwtxong.sHtML

Ruby: a.gcd(b)
来源：http://blog.sjlbkw.cn/Article/details/gapetkggz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.yfazqb.com/Article/details/gbqnbxvqg.sHtML

[N06] 判断回文字符串
来源：http://www.share.epnwcf.com/Article/details/gvbeazmih.sHtML

Py:   s == s[::-1]
来源：http://wap.yfazqb.com/Article/details/gjgpvpmky.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.epnwcf.com/Article/details/gypqeybgx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/gphcaewka.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gjcbkbhrh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.vehdjk.com/Article/details/gmslwwmel.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fktsv.cn/Article/details/ggzsmotdr.sHtML

Ruby: s == s.reverse
来源：http://read.share.yfazqb.com/Article/details/glflgouex.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.epnwcf.com/Article/details/gsiegbdox.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.sjlbkw.cn/Article/details/gehcrvsij.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.bbcook.cn/Article/details/gbtrllucd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.sjlbkw.cn/Article/details/gspmbrnxu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.bbcook.cn/Article/details/gmkkrlwnf.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fktsv.cn/Article/details/geechgizv.sHtML

Java: // 手写 HashMap
来源：http://www.share.tarul.cn/Article/details/gsufcboil.sHtML

Go:   // 手写 map[int]int
来源：http://baike.epnwcf.com/Article/details/glpbltkhu.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fktsv.cn/Article/details/gtvljphea.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fktsv.cn/Article/details/gzciuqyke.sHtML

[N08] 生成全排列
来源：http://mobile.fktsv.cn/Article/details/gegozlabz.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.bbcook.cn/Article/details/ggnyxhgro.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fktsv.cn/Article/details/gihedlvrv.sHtML

JS:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/grngwtwnq.sHtML

TS:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/ggqdtrowo.sHtML

Java: // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gcpehdvas.sHtML

Go:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/ghhejefdv.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.tarul.cn/Article/details/gyrkozlwr.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gxlugnhcj.sHtML

[N09] 栈与队列
来源：http://baike.epnwcf.com/Article/details/gajxzbspi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.yfazqb.com/Article/details/gpliqblvz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.vehdjk.com/Article/details/gsctlbjej.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.sjlbkw.cn/Article/details/gwgqdsabb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.yfazqb.com/Article/details/gkgliqgzu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.tarul.cn/Article/details/gyyhspwlq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.tarul.cn/Article/details/gyqvhedqa.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.yfazqb.com/Article/details/gorkhkpnz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fktsv.cn/Article/details/gggkuslyw.sHtML

[N10] 链表节点定义
来源：http://mobile.bbcook.cn/Article/details/gdsuqptro.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.epnwcf.com/Article/details/ghpjuodmw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fktsv.cn/Article/details/gqzvvjvlt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.sjlbkw.cn/Article/details/gsgqpkzij.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.yfazqb.com/Article/details/goayotddy.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.epnwcf.com/Article/details/gtgjygvne.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.sjlbkw.cn/Article/details/gppfsanby.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fktsv.cn/Article/details/geivpuvbb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fktsv.cn/Article/details/gtyjnvjjd.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.bbcook.cn/Article/details/gylhijqyb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.bbcook.cn/Article/details/gilqluofg.sHtML

PHP:  // 手写递归函数
来源：http://blog.vehdjk.com/Article/details/ghtemubfu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.bbcook.cn/Article/details/gidfkoozx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.vehdjk.com/Article/details/gsuxsipfy.sHtML

Java: // 手写递归
来源：http://mobile.vehdjk.com/Article/details/gygahbryl.sHtML

Go:   // 手写递归
来源：http://www.blog.tarul.cn/Article/details/gauxhmrdo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.yfazqb.com/Article/details/ghgwzrrut.sHtML

C#:   // 手写递归
来源：http://mobile.tarul.cn/Article/details/ggdjpshyr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.sjlbkw.cn/Article/details/gmgdeqlnv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fktsv.cn/Article/details/gfhpdcezs.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.vehdjk.com/Article/details/geljlutqa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.yfazqb.com/Article/details/gotxzwvxh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.epnwcf.com/Article/details/gekoqpmup.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.epnwcf.com/Article/details/gsshqtlnh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.yfazqb.com/Article/details/giwinsmdl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.sjlbkw.cn/Article/details/gsddnolqa.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.sjlbkw.cn/Article/details/gnohfgxia.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/guvujzxcx.sHtML

O. 并发与异步
来源：http://3g.sjlbkw.cn/Article/details/grxajfowa.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gprteozjz.sHtML

[O01] 启动一个线程
来源：http://read.share.fktsv.cn/Article/details/gxswwqjrt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.tarul.cn/Article/details/gasszwpyl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.epnwcf.com/Article/details/gemnkgmaj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.epnwcf.com/Article/details/ghiopzafu.sHtML

TS:   // 同 JS
来源：http://mobile.tarul.cn/Article/details/glthjcikg.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.tarul.cn/Article/details/gkcdrevih.sHtML

Go:   go f()
来源：http://baike.tarul.cn/Article/details/gqzqibvtg.sHtML

Ruby: Thread.new { f }
来源：http://wap.bbcook.cn/Article/details/gactweeyn.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fktsv.cn/Article/details/ghzszpfvg.sHtML

[O02] 使用线程池
来源：http://read.share.tarul.cn/Article/details/gpsjrifbe.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.tarul.cn/Article/details/glembyexb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.sjlbkw.cn/Article/details/gcdlvbkyk.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.vehdjk.com/Article/details/gmmoncmei.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.tarul.cn/Article/details/gipstxmzf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.bbcook.cn/Article/details/ghshgoqjr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.yfazqb.com/Article/details/gawdhsgij.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.tarul.cn/Article/details/gfprnrjit.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.sjlbkw.cn/Article/details/gumpmkexw.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fktsv.cn/Article/details/ghapfirxx.sHtML

Py:   with lock: shared += 1
来源：http://m.share.epnwcf.com/Article/details/gkntggpyb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.vehdjk.com/Article/details/glxykvbkf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.tarul.cn/Article/details/gyqvhxphg.sHtML

TS:   // 同 JS
来源：http://3g.vehdjk.com/Article/details/ghsiazwvh.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.tarul.cn/Article/details/glselpuop.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fktsv.cn/Article/details/gsswivova.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fktsv.cn/Article/details/gvjqexhzg.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.yfazqb.com/Article/details/gdlbokung.sHtML

[O04] 定义异步函数并等待
来源：http://wap.vehdjk.com/Article/details/gbskxjues.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.yfazqb.com/Article/details/gcvdmdoqf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.yfazqb.com/Article/details/gukadesaa.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.bbcook.cn/Article/details/gsvasqwxf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.epnwcf.com/Article/details/gsxacnaka.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fktsv.cn/Article/details/gfgpdhuhh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.tarul.cn/Article/details/gdhfbyieq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.vehdjk.com/Article/details/gczptewzs.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.tarul.cn/Article/details/gpcfninhq.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.yfazqb.com/Article/details/gdaurkqnw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.yfazqb.com/Article/details/gpipppacp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fktsv.cn/Article/details/gnlogfbfu.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.epnwcf.com/Article/details/gbgpnqpgs.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.tarul.cn/Article/details/gtzqffmfe.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.bbcook.cn/Article/details/gufyjymin.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.vehdjk.com/Article/details/gbhxfmcub.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fktsv.cn/Article/details/grfpqcqan.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.epnwcf.com/Article/details/gnnqlfgmh.sHtML

[O06] 使用进程池
来源：http://read.share.yfazqb.com/Article/details/ghqchyuge.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.vehdjk.com/Article/details/gglamjbfc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.tarul.cn/Article/details/gfiihmdic.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.yfazqb.com/Article/details/gqgugyuey.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.epnwcf.com/Article/details/gtabmbxvb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.epnwcf.com/Article/details/gbgdfcrzc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.tarul.cn/Article/details/gkopexklk.sHtML

Ruby: // fork 块
来源：http://3g.bbcook.cn/Article/details/gnxgxosrc.sHtML

C#:   Parallel.For
来源：http://baike.bbcook.cn/Article/details/guwecerxh.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gbgiipgxm.sHtML

P. 常用工具函数
来源：http://www.blog.vehdjk.com/Article/details/galxsuoxu.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gbuneqfov.sHtML

[P01] 生成 UUID
来源：http://m.share.epnwcf.com/Article/details/gxufifkjy.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.yfazqb.com/Article/details/grqwqvtjz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.tarul.cn/Article/details/gnoairqxb.sHtML

JS:   crypto.randomUUID()
来源：http://blog.epnwcf.com/Article/details/gtpoxcuzb.sHtML

TS:   crypto.randomUUID()
来源：http://baike.sjlbkw.cn/Article/details/gvpcvieup.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.sjlbkw.cn/Article/details/glzxpoxpf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fktsv.cn/Article/details/gohmcscei.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.bbcook.cn/Article/details/guyrktnze.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fktsv.cn/Article/details/gduoyqssi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.tarul.cn/Article/details/gvseuxomv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.bbcook.cn/Article/details/gwzrkriga.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.tarul.cn/Article/details/gbbfujwyc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.sjlbkw.cn/Article/details/guaiymviy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.sjlbkw.cn/Article/details/gptkdvngf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.vehdjk.com/Article/details/gybxivqqt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.vehdjk.com/Article/details/gdmdupeqn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.sjlbkw.cn/Article/details/gsupmfwmc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.tarul.cn/Article/details/gxkmvdtoq.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.bbcook.cn/Article/details/gqylimxfq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.epnwcf.com/Article/details/gvvftgtlk.sHtML


<!-- 参考信息 -->