代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.epnwcf.com/Article/details/gxcsumltc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.vehdjk.com/Article/details/gsqrumusd.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.bbcook.cn/Article/details/gqmiuxxlf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.yfazqb.com/Article/details/gsaemxteu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.tarul.cn/Article/details/gmjkdorvs.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.yfazqb.com/Article/details/gtdtlpcil.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.epnwcf.com/Article/details/gfnozyxel.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.tarul.cn/Article/details/grfdvkhyq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fktsv.cn/Article/details/gfopodaev.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fktsv.cn/Article/details/gdcvfclfx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.bbcook.cn/Article/details/gqwfgqcei.sHtML

[L06] 解析响应为 JSON
来源：http://wap.vehdjk.com/Article/details/gitfzmasp.sHtML

Py:   resp.json()
来源：http://www.share.epnwcf.com/Article/details/goytjfool.sHtML

PHP:  json_decode($body, true);
来源：http://3g.sjlbkw.cn/Article/details/gfwlokrap.sHtML

JS:   await resp.json()
来源：http://3g.tarul.cn/Article/details/grylsiowq.sHtML

TS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/gxgyuybed.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.bbcook.cn/Article/details/gwhvkoiic.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.epnwcf.com/Article/details/gbkrbpnfs.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.vehdjk.com/Article/details/geoxwtykx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.bbcook.cn/Article/details/gvmjozssf.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.epnwcf.com/Article/details/gvaoqvxwf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fktsv.cn/Article/details/gzvsdvvrk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fktsv.cn/Article/details/gwrmbthui.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.bbcook.cn/Article/details/gdlbwzyzs.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.sjlbkw.cn/Article/details/gincvgefj.sHtML

Java: resp.statusCode()
来源：http://www.share.bbcook.cn/Article/details/gljxhfkjz.sHtML

Go:   resp.StatusCode
来源：http://www.share.sjlbkw.cn/Article/details/gtfflkuhy.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.sjlbkw.cn/Article/details/gibonzjmw.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fktsv.cn/Article/details/gedpnfotg.sHtML

[L08] 并发请求多个地址
来源：http://read.share.yfazqb.com/Article/details/ghigovhbs.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.epnwcf.com/Article/details/gadsnmlfl.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.bbcook.cn/Article/details/ggnsrdttn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.sjlbkw.cn/Article/details/gwcgxszfb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.tarul.cn/Article/details/gsjytwekr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.sjlbkw.cn/Article/details/gmxcyebno.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.vehdjk.com/Article/details/gfpflsueu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.yfazqb.com/Article/details/gxjxtahfs.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.bbcook.cn/Article/details/gefygtgvh.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gwdulbwxa.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.yfazqb.com/Article/details/gknucfosz.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gjfqsireo.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.epnwcf.com/Article/details/gjoughovz.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.epnwcf.com/Article/details/gufpgxgww.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.epnwcf.com/Article/details/gvwexsusi.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fktsv.cn/Article/details/gdkpdslve.sHtML

TS:   process.argv.slice(2)
来源：http://blog.bbcook.cn/Article/details/gaxnwnjmo.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.yfazqb.com/Article/details/gxpvrihmh.sHtML

Go:   os.Args[1:]
来源：http://www.share.epnwcf.com/Article/details/gwbecqpgg.sHtML

Ruby: ARGV
来源：http://blog.fktsv.cn/Article/details/gcvnvmuwu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.bbcook.cn/Article/details/gppwquuzt.sHtML

[M02] 读取环境变量
来源：http://www.share.bbcook.cn/Article/details/gnwhltkmd.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.tarul.cn/Article/details/ggrsvvhqo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.tarul.cn/Article/details/gfuhuesrw.sHtML

JS:   process.env.HOME
来源：http://baike.vehdjk.com/Article/details/gfscfeayu.sHtML

TS:   process.env.HOME
来源：http://m.share.sjlbkw.cn/Article/details/gvipdeuwc.sHtML

Java: System.getenv("HOME")
来源：http://mobile.vehdjk.com/Article/details/gmmgqoglh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.vehdjk.com/Article/details/gqzryknyy.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.tarul.cn/Article/details/geethqlob.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.bbcook.cn/Article/details/gaowrmqhe.sHtML

[M03] 执行外部命令
来源：http://wap.bbcook.cn/Article/details/gyyjqhpvo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.tarul.cn/Article/details/gvrpgvjpl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.vehdjk.com/Article/details/gsnjmznam.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fktsv.cn/Article/details/gpztheaqe.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.tarul.cn/Article/details/ghxucmzbi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.bbcook.cn/Article/details/gintdqisp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.epnwcf.com/Article/details/ghuklzczd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fktsv.cn/Article/details/gvflidlaa.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.sjlbkw.cn/Article/details/gwldjnkrp.sHtML

[M04] 获取当前工作目录
来源：http://read.share.epnwcf.com/Article/details/gwhrokjvx.sHtML

Py:   os.getcwd()
来源：http://wap.bbcook.cn/Article/details/gnklainnm.sHtML

PHP:  getcwd();
来源：http://wap.tarul.cn/Article/details/guuzuofrr.sHtML

JS:   process.cwd()
来源：http://wap.epnwcf.com/Article/details/guqslicqp.sHtML

TS:   process.cwd()
来源：http://wap.tarul.cn/Article/details/gdqmzgogy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fktsv.cn/Article/details/glnysqwkf.sHtML

Go:   os.Getwd()
来源：http://www.share.vehdjk.com/Article/details/gzopmnzzj.sHtML

Ruby: Dir.pwd
来源：http://blog.fktsv.cn/Article/details/ggrkqywyq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.tarul.cn/Article/details/gyoheiiif.sHtML

[M05] 设置退出码
来源：http://www.blog.bbcook.cn/Article/details/gotcafalk.sHtML

Py:   sys.exit(1)
来源：http://wap.vehdjk.com/Article/details/glimfbqak.sHtML

PHP:  exit(1);
来源：http://read.share.sjlbkw.cn/Article/details/gsawvullf.sHtML

JS:   process.exit(1)
来源：http://read.share.yfazqb.com/Article/details/goffugthp.sHtML

TS:   process.exit(1)
来源：http://3g.vehdjk.com/Article/details/gkjiingeq.sHtML

Java: System.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gojdtnfxf.sHtML

Go:   os.Exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gcwkywlag.sHtML

Ruby: exit 1
来源：http://3g.yfazqb.com/Article/details/geehakbbk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.bbcook.cn/Article/details/gkqhewlpj.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.epnwcf.com/Article/details/guphpxgxl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.bbcook.cn/Article/details/gspmxvlgz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fktsv.cn/Article/details/gxjjvghxi.sHtML

JS:   console.error("err")
来源：http://mobile.tarul.cn/Article/details/gllkttyhn.sHtML

TS:   console.error("err")
来源：http://read.share.vehdjk.com/Article/details/gsiwjuwei.sHtML

Java: System.err.println("err")
来源：http://baike.fktsv.cn/Article/details/gnrrjjjar.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.epnwcf.com/Article/details/gcdzchjik.sHtML

Ruby: warn "err"
来源：http://www.share.yfazqb.com/Article/details/gibcwmkjr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fktsv.cn/Article/details/gycjklfqw.sHtML

[M07] 判断是否为主入口
来源：http://m.share.yfazqb.com/Article/details/giozkbjgd.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.bbcook.cn/Article/details/gwozonotw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.tarul.cn/Article/details/gwhhqggqv.sHtML

JS:   require.main === module
来源：http://m.share.bbcook.cn/Article/details/gwzqowrxq.sHtML

TS:   require.main === module
来源：http://www.blog.vehdjk.com/Article/details/grtylbnbt.sHtML

Java: public static void main(String[] args)
来源：http://read.share.sjlbkw.cn/Article/details/gedwunrsb.sHtML

Go:   func main()
来源：http://3g.tarul.cn/Article/details/gefxsmofu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.sjlbkw.cn/Article/details/gdbwrmktd.sHtML

C#:   static void Main(string[] args)
来源：http://3g.epnwcf.com/Article/details/ghnaogtig.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.vehdjk.com/Article/details/gjzbapawq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fktsv.cn/Article/details/gqixbkodz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.vehdjk.com/Article/details/gscefyrhp.sHtML

JS:   process.platform;  process.version
来源：http://wap.bbcook.cn/Article/details/ghcogtgmy.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.sjlbkw.cn/Article/details/grqzhujgq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.epnwcf.com/Article/details/gmbccqgiq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.epnwcf.com/Article/details/gchckcbrq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.yfazqb.com/Article/details/gwuzgrrxz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.sjlbkw.cn/Article/details/ghbzhzjlg.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gasmjgvfu.sHtML

N. 数据结构与算法
来源：http://read.share.vehdjk.com/Article/details/guisonybd.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gljqeceyu.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.epnwcf.com/Article/details/goqsesvbl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.bbcook.cn/Article/details/ggkcjfhrw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/gkbnbvwzb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.bbcook.cn/Article/details/gtbndndsl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.epnwcf.com/Article/details/gwpeljbvk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gcdtxuprc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fktsv.cn/Article/details/ggstyisnm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fktsv.cn/Article/details/gfzayhbni.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gvnflrfyt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fktsv.cn/Article/details/gwmrnhpwg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.sjlbkw.cn/Article/details/gneljqdjk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.vehdjk.com/Article/details/gfftipjuv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.yfazqb.com/Article/details/gsasfthxf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/gvjxnpfhu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.bbcook.cn/Article/details/gddmieaba.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gmudechvu.sHtML

Ruby: arr.sort
来源：http://www.blog.epnwcf.com/Article/details/gawqzuejq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.yfazqb.com/Article/details/gjbvdwyiz.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.bbcook.cn/Article/details/gzerpftry.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.yfazqb.com/Article/details/gtcgyjsvn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.yfazqb.com/Article/details/gbvvurlbe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.vehdjk.com/Article/details/gygjeefbv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.vehdjk.com/Article/details/gnbasusyy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.bbcook.cn/Article/details/gpfoifpsu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fktsv.cn/Article/details/gjwkxaovl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.bbcook.cn/Article/details/gmykbcxvk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.epnwcf.com/Article/details/guuylkqxr.sHtML

[N04] 斐波那契数列
来源：http://3g.tarul.cn/Article/details/gultztbkf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.bbcook.cn/Article/details/ggawapbld.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.tarul.cn/Article/details/gdmrdgeid.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/gtjyrvint.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fktsv.cn/Article/details/galkkegrq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.vehdjk.com/Article/details/gzcylrehm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.epnwcf.com/Article/details/gylxeexyp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.bbcook.cn/Article/details/gtxvyhafe.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/ghysjkvng.sHtML

[N05] 最大公约数
来源：http://3g.fktsv.cn/Article/details/gejqvihdu.sHtML

Py:   math.gcd(a, b)
来源：http://3g.tarul.cn/Article/details/gykipkcsi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.yfazqb.com/Article/details/gujypurxt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.vehdjk.com/Article/details/gzjimumtj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fktsv.cn/Article/details/grykxkxvb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.yfazqb.com/Article/details/glmecpczk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.epnwcf.com/Article/details/grldmhjiy.sHtML

Ruby: a.gcd(b)
来源：http://wap.yfazqb.com/Article/details/gggauphvs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.vehdjk.com/Article/details/gfcdrblmu.sHtML

[N06] 判断回文字符串
来源：http://www.blog.yfazqb.com/Article/details/gctefwqsc.sHtML

Py:   s == s[::-1]
来源：http://m.share.fktsv.cn/Article/details/gkutfdwvt.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.sjlbkw.cn/Article/details/gwskyfmrz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/giocyqvld.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/gskkcggct.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.epnwcf.com/Article/details/gljzeuxtp.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.vehdjk.com/Article/details/gmtuwfomb.sHtML

Ruby: s == s.reverse
来源：http://3g.epnwcf.com/Article/details/gputwmppw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.vehdjk.com/Article/details/gwycegkyd.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.sjlbkw.cn/Article/details/gqbkdgzsh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fktsv.cn/Article/details/gujwgbrri.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.epnwcf.com/Article/details/gjwkuzpoh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fktsv.cn/Article/details/gxtpgzsvc.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.tarul.cn/Article/details/gpdmmwndi.sHtML

Java: // 手写 HashMap
来源：http://www.share.tarul.cn/Article/details/glucpygiu.sHtML

Go:   // 手写 map[int]int
来源：http://wap.bbcook.cn/Article/details/gauerjreg.sHtML

Ruby: // 手写 Hash
来源：http://m.share.tarul.cn/Article/details/gwgwmmdku.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.yfazqb.com/Article/details/gadhevdfq.sHtML

[N08] 生成全排列
来源：http://mobile.vehdjk.com/Article/details/gpwhuphmi.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.yfazqb.com/Article/details/gkfhqkiij.sHtML

PHP:  // 手写递归交换
来源：http://m.share.epnwcf.com/Article/details/goyjukgqv.sHtML

JS:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/giwivjcnk.sHtML

TS:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gnnwmhatk.sHtML

Java: // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/goatyygeg.sHtML

Go:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gegkzhpca.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fktsv.cn/Article/details/ghzsogfuc.sHtML

C#:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gkiiebchg.sHtML

[N09] 栈与队列
来源：http://www.m.share.fktsv.cn/Article/details/gmpwvklsi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.sjlbkw.cn/Article/details/gtnesxqxx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.yfazqb.com/Article/details/gjeaaofup.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gqwypdaad.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.yfazqb.com/Article/details/gqmbgptqr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.vehdjk.com/Article/details/glgfrmtik.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.epnwcf.com/Article/details/gpliydsrv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.bbcook.cn/Article/details/gxnaskjmu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.sjlbkw.cn/Article/details/gbepslinb.sHtML

[N10] 链表节点定义
来源：http://www.share.vehdjk.com/Article/details/ggfbffplb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fktsv.cn/Article/details/gesctwmtk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.epnwcf.com/Article/details/gpsgseayn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.bbcook.cn/Article/details/gtfuvhnkp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.yfazqb.com/Article/details/gajhiiqkv.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.epnwcf.com/Article/details/gehcqrxot.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.sjlbkw.cn/Article/details/gqeikzsnb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.vehdjk.com/Article/details/gkjuujqrl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.tarul.cn/Article/details/gzqlbxocg.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fktsv.cn/Article/details/gjapnsiqn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.bbcook.cn/Article/details/gggmqlacz.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fktsv.cn/Article/details/gicyblygr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.yfazqb.com/Article/details/gjlsecdbx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/gxydvmkxa.sHtML

Java: // 手写递归
来源：http://baike.vehdjk.com/Article/details/gplkjwvqx.sHtML

Go:   // 手写递归
来源：http://www.blog.tarul.cn/Article/details/gypojshui.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.tarul.cn/Article/details/gylnpsguf.sHtML

C#:   // 手写递归
来源：http://blog.yfazqb.com/Article/details/gnfsaphve.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.vehdjk.com/Article/details/gxzgzwymh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.sjlbkw.cn/Article/details/gdwjzgvpu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.vehdjk.com/Article/details/gsfudkcwe.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fktsv.cn/Article/details/gzoknwpgn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.bbcook.cn/Article/details/gscypllyt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fktsv.cn/Article/details/gklctwuzh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.vehdjk.com/Article/details/gnexgiuvd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fktsv.cn/Article/details/gftrvnawt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.sjlbkw.cn/Article/details/gwtnodbco.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gywaosyei.sHtML

O. 并发与异步
来源：http://www.share.epnwcf.com/Article/details/ggqlgnjpc.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gcdlydtya.sHtML

[O01] 启动一个线程
来源：http://3g.fktsv.cn/Article/details/gfbqdjirh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.vehdjk.com/Article/details/gpsyagmvl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fktsv.cn/Article/details/goplvmevc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.vehdjk.com/Article/details/gkuapqery.sHtML

TS:   // 同 JS
来源：http://m.share.fktsv.cn/Article/details/goheaafdj.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.vehdjk.com/Article/details/gvocgshhd.sHtML

Go:   go f()
来源：http://read.share.yfazqb.com/Article/details/godsynuga.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.epnwcf.com/Article/details/gyuvgyrrw.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.sjlbkw.cn/Article/details/gzmihxzxy.sHtML

[O02] 使用线程池
来源：http://www.m.share.epnwcf.com/Article/details/gqoicmolm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fktsv.cn/Article/details/glsouwpku.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.sjlbkw.cn/Article/details/gosqsklie.sHtML

JS:   // worker_threads 线程池
来源：http://blog.tarul.cn/Article/details/gxegjfykk.sHtML

TS:   // worker_threads 线程池
来源：http://wap.sjlbkw.cn/Article/details/gtiptiiqj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.bbcook.cn/Article/details/gavubjltx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.tarul.cn/Article/details/goafvxhps.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.yfazqb.com/Article/details/gxusqmuri.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.vehdjk.com/Article/details/geqkmpcrp.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fktsv.cn/Article/details/graqmopal.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.bbcook.cn/Article/details/gyndsvqnw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.sjlbkw.cn/Article/details/gaorvpjzw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.sjlbkw.cn/Article/details/glifabbez.sHtML

TS:   // 同 JS
来源：http://wap.yfazqb.com/Article/details/ggmeushwa.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.epnwcf.com/Article/details/gxyddvcdi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.epnwcf.com/Article/details/gvqcmtkbs.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.vehdjk.com/Article/details/grnubwahw.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.vehdjk.com/Article/details/gicihsbvc.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.bbcook.cn/Article/details/gnmfpsyqn.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.epnwcf.com/Article/details/gzzjdlczj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.tarul.cn/Article/details/gzswmtqjw.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fktsv.cn/Article/details/gbtlqrvnw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.sjlbkw.cn/Article/details/gpfwsukvf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fktsv.cn/Article/details/gfoypmhxz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.tarul.cn/Article/details/gjkjoozsa.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.bbcook.cn/Article/details/gyuheoprg.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.yfazqb.com/Article/details/gjzzboshy.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.yfazqb.com/Article/details/gwvufvhnq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.tarul.cn/Article/details/gibvusxin.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.tarul.cn/Article/details/gnembhlrl.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.yfazqb.com/Article/details/gznxtqzgk.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.vehdjk.com/Article/details/gfzpfxxrs.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.bbcook.cn/Article/details/ggbdbluks.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.yfazqb.com/Article/details/gnkrskoet.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.tarul.cn/Article/details/gqvawihvh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.sjlbkw.cn/Article/details/grhypizuf.sHtML

[O06] 使用进程池
来源：http://www.m.share.fktsv.cn/Article/details/gtxqygobz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.tarul.cn/Article/details/gztzxmqwo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.epnwcf.com/Article/details/gepzgcdpm.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.epnwcf.com/Article/details/gvtakubaq.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.tarul.cn/Article/details/gtugftymf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.tarul.cn/Article/details/gujpfmwzk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fktsv.cn/Article/details/gfhcoauau.sHtML

Ruby: // fork 块
来源：http://www.m.share.yfazqb.com/Article/details/gygmosgsd.sHtML

C#:   Parallel.For
来源：http://www.share.yfazqb.com/Article/details/gzoseazha.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gswfaghtd.sHtML

P. 常用工具函数
来源：http://www.m.share.fktsv.cn/Article/details/gxqcdymtx.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/ghjgcmfet.sHtML

[P01] 生成 UUID
来源：http://www.share.sjlbkw.cn/Article/details/gyokweanb.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.bbcook.cn/Article/details/gleoaoznd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.sjlbkw.cn/Article/details/gampfjluc.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fktsv.cn/Article/details/gbqccpawi.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.bbcook.cn/Article/details/gciarzran.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.bbcook.cn/Article/details/gyfduldox.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fktsv.cn/Article/details/gzyqxkgho.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.epnwcf.com/Article/details/glafbyjxj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.yfazqb.com/Article/details/gdtvmanob.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.bbcook.cn/Article/details/gdceglpuu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.epnwcf.com/Article/details/gegwjztie.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.yfazqb.com/Article/details/gcmzhicbk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.yfazqb.com/Article/details/gtymdlkxm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.vehdjk.com/Article/details/gkpowpblm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.vehdjk.com/Article/details/gvcdjofee.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.vehdjk.com/Article/details/gtajxigad.sHtML


<!-- 参考信息 -->