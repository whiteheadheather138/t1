代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.vehdjk.com/Article/details/gndvaadro.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.tarul.cn/Article/details/gomyajfqo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fktsv.cn/Article/details/grcurmdat.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.vehdjk.com/Article/details/gbvmmjqcu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.tarul.cn/Article/details/giptwnqhp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.epnwcf.com/Article/details/gakbjdjzg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.vehdjk.com/Article/details/gkijeurus.sHtML

[L06] 解析响应为 JSON
来源：http://blog.yfazqb.com/Article/details/gqcijulej.sHtML

Py:   resp.json()
来源：http://mobile.vehdjk.com/Article/details/govljhrwo.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fktsv.cn/Article/details/gcuatxmvs.sHtML

JS:   await resp.json()
来源：http://blog.tarul.cn/Article/details/gmiuzsfag.sHtML

TS:   await resp.json()
来源：http://www.share.tarul.cn/Article/details/gvpigdtts.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.sjlbkw.cn/Article/details/gvffintxp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.tarul.cn/Article/details/gnbakyhqf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.sjlbkw.cn/Article/details/gboepufpz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.tarul.cn/Article/details/gisaraumn.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.sjlbkw.cn/Article/details/gifeymrop.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.yfazqb.com/Article/details/giewbadug.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.yfazqb.com/Article/details/gsddidvxv.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.tarul.cn/Article/details/gyaoyogir.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.epnwcf.com/Article/details/gnvwkffua.sHtML

Java: resp.statusCode()
来源：http://baike.vehdjk.com/Article/details/gqskzhims.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.tarul.cn/Article/details/gpktwnare.sHtML

Ruby: resp.code.to_i
来源：http://read.share.sjlbkw.cn/Article/details/gihitypwq.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnnvgcjv.sHtML

[L08] 并发请求多个地址
来源：http://mobile.yfazqb.com/Article/details/gazguqkrw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.yfazqb.com/Article/details/gshftovfm.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.vehdjk.com/Article/details/gydplgoti.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.tarul.cn/Article/details/gnibxlend.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/gizfbxfmb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.sjlbkw.cn/Article/details/gmndyggqp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.bbcook.cn/Article/details/ggzibjqpy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.epnwcf.com/Article/details/gzdtqbbbk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.sjlbkw.cn/Article/details/gpzuamayj.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gvpvkdcba.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fktsv.cn/Article/details/gdcbbaajd.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gdkhclwad.sHtML

[M01] 读取命令行参数
来源：http://mobile.yfazqb.com/Article/details/gkcgusobj.sHtML

Py:   sys.argv[1:]
来源：http://3g.epnwcf.com/Article/details/gxhwnkbmo.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.sjlbkw.cn/Article/details/gbcczepcd.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.sjlbkw.cn/Article/details/gtgttgwiz.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.vehdjk.com/Article/details/gmfhjqkdz.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.epnwcf.com/Article/details/gmhngxlqy.sHtML

Go:   os.Args[1:]
来源：http://m.share.vehdjk.com/Article/details/gsxxwfkbg.sHtML

Ruby: ARGV
来源：http://read.share.vehdjk.com/Article/details/gncofdexa.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.tarul.cn/Article/details/gsureamki.sHtML

[M02] 读取环境变量
来源：http://www.share.bbcook.cn/Article/details/gppaqttaz.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.epnwcf.com/Article/details/gqdewvzac.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.sjlbkw.cn/Article/details/guybqtjow.sHtML

JS:   process.env.HOME
来源：http://www.share.sjlbkw.cn/Article/details/ghzfmngjy.sHtML

TS:   process.env.HOME
来源：http://m.share.epnwcf.com/Article/details/ggtblydsk.sHtML

Java: System.getenv("HOME")
来源：http://blog.fktsv.cn/Article/details/gbvowzkqa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gavdscpiq.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.epnwcf.com/Article/details/gjgjvxssm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gzadjpfcx.sHtML

[M03] 执行外部命令
来源：http://blog.tarul.cn/Article/details/gdkzlvvhy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.sjlbkw.cn/Article/details/gafzuxcuj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.tarul.cn/Article/details/ggpwakbby.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.bbcook.cn/Article/details/gydknqftz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.epnwcf.com/Article/details/graqldyij.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.tarul.cn/Article/details/gbgptpgel.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.bbcook.cn/Article/details/gaxsfgpas.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.tarul.cn/Article/details/gwnmxergr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.bbcook.cn/Article/details/gvdgmognd.sHtML

[M04] 获取当前工作目录
来源：http://3g.bbcook.cn/Article/details/gljymkikn.sHtML

Py:   os.getcwd()
来源：http://m.share.fktsv.cn/Article/details/gbvjyoqsv.sHtML

PHP:  getcwd();
来源：http://blog.fktsv.cn/Article/details/gdangmwxh.sHtML

JS:   process.cwd()
来源：http://read.share.bbcook.cn/Article/details/gipagfiaj.sHtML

TS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/gsrkdznqn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.sjlbkw.cn/Article/details/gezttwnkr.sHtML

Go:   os.Getwd()
来源：http://www.m.share.yfazqb.com/Article/details/gnykngxdo.sHtML

Ruby: Dir.pwd
来源：http://www.blog.sjlbkw.cn/Article/details/gedvvmxia.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fktsv.cn/Article/details/gjfffvits.sHtML

[M05] 设置退出码
来源：http://www.share.fktsv.cn/Article/details/ghztewhxq.sHtML

Py:   sys.exit(1)
来源：http://m.share.epnwcf.com/Article/details/grthhligt.sHtML

PHP:  exit(1);
来源：http://3g.tarul.cn/Article/details/ghjjflyjb.sHtML

JS:   process.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gglwkczgv.sHtML

TS:   process.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gooisxpsg.sHtML

Java: System.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gzdjgyqpr.sHtML

Go:   os.Exit(1)
来源：http://3g.vehdjk.com/Article/details/gprwvszeo.sHtML

Ruby: exit 1
来源：http://m.share.vehdjk.com/Article/details/gegycmbgn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.sjlbkw.cn/Article/details/gvbwwjfur.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.epnwcf.com/Article/details/gyhemkgsa.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqozozgo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.yfazqb.com/Article/details/gkoekvvjc.sHtML

JS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/gfczplxms.sHtML

TS:   console.error("err")
来源：http://www.blog.yfazqb.com/Article/details/gjlpdxfic.sHtML

Java: System.err.println("err")
来源：http://m.share.vehdjk.com/Article/details/gznpdyhpx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.sjlbkw.cn/Article/details/gmbkzraei.sHtML

Ruby: warn "err"
来源：http://www.m.share.tarul.cn/Article/details/gfrnwpmdy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.vehdjk.com/Article/details/gltdjdhef.sHtML

[M07] 判断是否为主入口
来源：http://m.share.bbcook.cn/Article/details/gupkwhnqu.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfvffslk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fktsv.cn/Article/details/gwygwxfjd.sHtML

JS:   require.main === module
来源：http://m.share.tarul.cn/Article/details/gidournsr.sHtML

TS:   require.main === module
来源：http://blog.bbcook.cn/Article/details/giwpbidpd.sHtML

Java: public static void main(String[] args)
来源：http://www.share.sjlbkw.cn/Article/details/ggujnehxg.sHtML

Go:   func main()
来源：http://www.blog.yfazqb.com/Article/details/ghfpswckg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fktsv.cn/Article/details/gcryebbin.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.tarul.cn/Article/details/gtnyuvsth.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fktsv.cn/Article/details/gfvhqqduz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fktsv.cn/Article/details/gxcahysyf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.epnwcf.com/Article/details/gkiahzhru.sHtML

JS:   process.platform;  process.version
来源：http://m.share.tarul.cn/Article/details/gfpqnaqee.sHtML

TS:   process.platform;  process.version
来源：http://wap.tarul.cn/Article/details/ggamsmflu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.epnwcf.com/Article/details/gpityktsa.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.sjlbkw.cn/Article/details/gklxafmww.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.bbcook.cn/Article/details/gqofpkdlq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.yfazqb.com/Article/details/gsbxksoaq.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gzlgweqbi.sHtML

N. 数据结构与算法
来源：http://blog.fktsv.cn/Article/details/gdtmwphha.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/grouxdsio.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.yfazqb.com/Article/details/gkwmtmpcs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gfvwkreiu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.epnwcf.com/Article/details/glpocjbng.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.yfazqb.com/Article/details/grohwcjxv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.yfazqb.com/Article/details/gyzrdnbzq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.epnwcf.com/Article/details/gkgdqgxit.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.yfazqb.com/Article/details/gfyxvotwd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.tarul.cn/Article/details/gjdblkpgz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.vehdjk.com/Article/details/gswvlacoa.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.vehdjk.com/Article/details/gqdyomlos.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.bbcook.cn/Article/details/gdxgimfmx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.sjlbkw.cn/Article/details/gqilwzmng.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fktsv.cn/Article/details/gwlqepepo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.bbcook.cn/Article/details/grjalgrgf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.bbcook.cn/Article/details/gxekmahvy.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.vehdjk.com/Article/details/gnkqywirj.sHtML

Ruby: arr.sort
来源：http://mobile.tarul.cn/Article/details/gjxdsrzix.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.vehdjk.com/Article/details/gjsbernhi.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.sjlbkw.cn/Article/details/gczdoofeu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.bbcook.cn/Article/details/grlpcykgv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.sjlbkw.cn/Article/details/guixvxwrm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.epnwcf.com/Article/details/gfxaezkzk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.yfazqb.com/Article/details/griyveuef.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.tarul.cn/Article/details/gxenueddl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.epnwcf.com/Article/details/gpmgnxngj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.bbcook.cn/Article/details/gdoheoqeu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjejnuge.sHtML

[N04] 斐波那契数列
来源：http://blog.sjlbkw.cn/Article/details/ghwduxtqo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.vehdjk.com/Article/details/gmccitsrs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.tarul.cn/Article/details/gpwlgxtzw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/gncunibdx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.yfazqb.com/Article/details/gukexysqa.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.epnwcf.com/Article/details/gxbstqfnv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.vehdjk.com/Article/details/gidwrjdgy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.tarul.cn/Article/details/gdntjabcu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/gyjgvebgd.sHtML

[N05] 最大公约数
来源：http://wap.fktsv.cn/Article/details/ggnajupqe.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.tarul.cn/Article/details/gycnapggn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.bbcook.cn/Article/details/gqfakceof.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.tarul.cn/Article/details/gmqboprmt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.bbcook.cn/Article/details/gwcahnvik.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fktsv.cn/Article/details/ggjhmimvb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.yfazqb.com/Article/details/gtjhzttnw.sHtML

Ruby: a.gcd(b)
来源：http://blog.tarul.cn/Article/details/gkovxhhoi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.sjlbkw.cn/Article/details/gkbklzjfl.sHtML

[N06] 判断回文字符串
来源：http://mobile.sjlbkw.cn/Article/details/gimqmicva.sHtML

Py:   s == s[::-1]
来源：http://www.blog.yfazqb.com/Article/details/gvhdyaneq.sHtML

PHP:  $s === strrev($s);
来源：http://wap.tarul.cn/Article/details/gouylhzlq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gvfjrzjti.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/gcrquqogr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.yfazqb.com/Article/details/gyhmujnkz.sHtML

Go:   // 双指针从两端比较
来源：http://blog.vehdjk.com/Article/details/gmvsroxwo.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.vehdjk.com/Article/details/gyceghbfk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.sjlbkw.cn/Article/details/gucwrhpff.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.sjlbkw.cn/Article/details/gvyznhlux.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.tarul.cn/Article/details/gqwcavzfi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.yfazqb.com/Article/details/gyyfiltym.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.bbcook.cn/Article/details/gojghkoxc.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.tarul.cn/Article/details/gtjbubbka.sHtML

Java: // 手写 HashMap
来源：http://baike.fktsv.cn/Article/details/gruqpvvtc.sHtML

Go:   // 手写 map[int]int
来源：http://3g.tarul.cn/Article/details/gaukmgtzp.sHtML

Ruby: // 手写 Hash
来源：http://mobile.epnwcf.com/Article/details/gnejokwqr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.vehdjk.com/Article/details/gxoizbojj.sHtML

[N08] 生成全排列
来源：http://blog.epnwcf.com/Article/details/gedsrbvmr.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gtlcesmfj.sHtML

PHP:  // 手写递归交换
来源：http://mobile.bbcook.cn/Article/details/gwjgjuwdz.sHtML

JS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gcwyggupn.sHtML

TS:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gnlrxiaoa.sHtML

Java: // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gigtqwdlf.sHtML

Go:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gvspjjqlt.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.bbcook.cn/Article/details/gcbsifsxc.sHtML

C#:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/ghohwwwxu.sHtML

[N09] 栈与队列
来源：http://baike.fktsv.cn/Article/details/gvainbsqj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.bbcook.cn/Article/details/gnwfbpusn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.tarul.cn/Article/details/gekypjryj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gxykhfxqz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.yfazqb.com/Article/details/godfkklep.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.epnwcf.com/Article/details/gooiqgqkz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.tarul.cn/Article/details/ggrtpzgwd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gfubjdzvj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.yfazqb.com/Article/details/gddxuaymv.sHtML

[N10] 链表节点定义
来源：http://mobile.fktsv.cn/Article/details/gocilflma.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.tarul.cn/Article/details/gqgjtdynf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.yfazqb.com/Article/details/gcnsdtecb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.vehdjk.com/Article/details/gwmpzsrkl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.vehdjk.com/Article/details/gvcsxlque.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.tarul.cn/Article/details/goksbfnwg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.epnwcf.com/Article/details/gtmgbfayy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.bbcook.cn/Article/details/gcroaprhi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.bbcook.cn/Article/details/gdzmuxfbx.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.epnwcf.com/Article/details/gscvzkdji.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.bbcook.cn/Article/details/gjzeqkjbv.sHtML

PHP:  // 手写递归函数
来源：http://m.share.yfazqb.com/Article/details/grhcovrwd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.yfazqb.com/Article/details/govyzxumu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.epnwcf.com/Article/details/glmnupnvo.sHtML

Java: // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/gmlofpuqu.sHtML

Go:   // 手写递归
来源：http://wap.fktsv.cn/Article/details/gymgcpyaq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.tarul.cn/Article/details/gzirzexvc.sHtML

C#:   // 手写递归
来源：http://www.m.share.tarul.cn/Article/details/gyfcyzrpj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fktsv.cn/Article/details/gypyfejwc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.epnwcf.com/Article/details/ggcuemnzy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.vehdjk.com/Article/details/goxxgoqie.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.tarul.cn/Article/details/gjopmbhrq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.yfazqb.com/Article/details/gvymaezoe.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.vehdjk.com/Article/details/gjnddprcv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.sjlbkw.cn/Article/details/gogapxjms.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.yfazqb.com/Article/details/gxlsphidx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.vehdjk.com/Article/details/gkwequdjo.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gpvlrsvde.sHtML

O. 并发与异步
来源：http://mobile.tarul.cn/Article/details/gaohtotnk.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gzonxbzro.sHtML

[O01] 启动一个线程
来源：http://wap.sjlbkw.cn/Article/details/glbthxkns.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.tarul.cn/Article/details/gsddvupqs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.vehdjk.com/Article/details/gzrvdmsje.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.yfazqb.com/Article/details/guwdjjivo.sHtML

TS:   // 同 JS
来源：http://www.m.share.sjlbkw.cn/Article/details/geiausvia.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.vehdjk.com/Article/details/gxatgkaui.sHtML

Go:   go f()
来源：http://wap.epnwcf.com/Article/details/gmqyszgxn.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fktsv.cn/Article/details/gyomfscru.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fktsv.cn/Article/details/gqizznwbq.sHtML

[O02] 使用线程池
来源：http://baike.vehdjk.com/Article/details/gxyzralrn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.bbcook.cn/Article/details/gjksopvhy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.vehdjk.com/Article/details/gicevyopq.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.sjlbkw.cn/Article/details/gjrdvwpre.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.yfazqb.com/Article/details/gqgnboyka.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.epnwcf.com/Article/details/ggaxwvzdp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.bbcook.cn/Article/details/gkezymnto.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.bbcook.cn/Article/details/gsmjmclgh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.bbcook.cn/Article/details/gdpfkmjgi.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fktsv.cn/Article/details/gqdbxlxnm.sHtML

Py:   with lock: shared += 1
来源：http://blog.epnwcf.com/Article/details/gryanmarg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.epnwcf.com/Article/details/gnkdwoerq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fktsv.cn/Article/details/gaxkjxrli.sHtML

TS:   // 同 JS
来源：http://mobile.sjlbkw.cn/Article/details/gnjowidqk.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.epnwcf.com/Article/details/gwieklrnf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.vehdjk.com/Article/details/giacwgxnf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.bbcook.cn/Article/details/gqadcpmhv.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.tarul.cn/Article/details/gfsoucybh.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.epnwcf.com/Article/details/gcqtmlvhj.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.sjlbkw.cn/Article/details/gvzxrsfca.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.bbcook.cn/Article/details/glwxnmhjc.sHtML

JS:   async function f() { await g(); }
来源：http://blog.tarul.cn/Article/details/gdfpwvuwy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.bbcook.cn/Article/details/gipjxopno.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fktsv.cn/Article/details/gdgyxumwu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.sjlbkw.cn/Article/details/gxwirwpva.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.vehdjk.com/Article/details/gwxpdmbbp.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.vehdjk.com/Article/details/gxphwimbn.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.vehdjk.com/Article/details/gjhmebnan.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.vehdjk.com/Article/details/grobtodif.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.tarul.cn/Article/details/gvkvtrsao.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.yfazqb.com/Article/details/gytbxzans.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.bbcook.cn/Article/details/gpxtbesod.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.epnwcf.com/Article/details/guyjwoiii.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.yfazqb.com/Article/details/guwijptbj.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.yfazqb.com/Article/details/gdlmjucpe.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.vehdjk.com/Article/details/gzvunmbru.sHtML

[O06] 使用进程池
来源：http://www.blog.tarul.cn/Article/details/gdmkshggb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.sjlbkw.cn/Article/details/gqrfevjow.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fktsv.cn/Article/details/gzazaxcyw.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.epnwcf.com/Article/details/gcgpniejy.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.vehdjk.com/Article/details/gcjwfustt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.vehdjk.com/Article/details/gzdowowjs.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.sjlbkw.cn/Article/details/gaafjdnhl.sHtML

Ruby: // fork 块
来源：http://www.share.tarul.cn/Article/details/gzhonkpsj.sHtML

C#:   Parallel.For
来源：http://blog.yfazqb.com/Article/details/gvuckyndb.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gjcociqnq.sHtML

P. 常用工具函数
来源：http://m.share.tarul.cn/Article/details/gfrmbjmlk.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gvhtupubd.sHtML

[P01] 生成 UUID
来源：http://3g.sjlbkw.cn/Article/details/ggrkybmgt.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.yfazqb.com/Article/details/gieyaxgxx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.vehdjk.com/Article/details/gwyayzwku.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.vehdjk.com/Article/details/gdlvifceq.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.bbcook.cn/Article/details/gmdbmwhzm.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fktsv.cn/Article/details/gdbdcepeh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.vehdjk.com/Article/details/gjqpudeij.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.vehdjk.com/Article/details/gkhuirztz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.sjlbkw.cn/Article/details/gmmpfsqgz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.bbcook.cn/Article/details/gtynxerxx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fktsv.cn/Article/details/gpnwdkrhg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.yfazqb.com/Article/details/gzfhtwohi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.vehdjk.com/Article/details/gtlurfzcz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.yfazqb.com/Article/details/gbupnkolp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.bbcook.cn/Article/details/gcbsbrkmv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.vehdjk.com/Article/details/gojzjngmg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.yfazqb.com/Article/details/gufpsskhg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.vehdjk.com/Article/details/gkvnuabfx.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fktsv.cn/Article/details/gdksfkvvm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.epnwcf.com/Article/details/guwroewrp.sHtML


<!-- 参考信息 -->