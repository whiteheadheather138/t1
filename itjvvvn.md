代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fktsv.cn/Article/details/gkxgbjakk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.epnwcf.com/Article/details/govqdgnjw.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.tarul.cn/Article/details/gzkhmkobn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.vehdjk.com/Article/details/gfjfmxdlc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.tarul.cn/Article/details/glecxrlud.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.bbcook.cn/Article/details/gxeeewuyr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.vehdjk.com/Article/details/gbivssazu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.epnwcf.com/Article/details/gaxneyaie.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.epnwcf.com/Article/details/goaxsqlrh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.tarul.cn/Article/details/guwmmbryn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.tarul.cn/Article/details/gdosggjkx.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.vehdjk.com/Article/details/ggedumass.sHtML

Py:   resp.json()
来源：http://www.share.vehdjk.com/Article/details/gtwlwjiyz.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.epnwcf.com/Article/details/gpnowasqr.sHtML

JS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/gciorrhtz.sHtML

TS:   await resp.json()
来源：http://read.share.epnwcf.com/Article/details/gbacdnkfo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.epnwcf.com/Article/details/gwhqkfjak.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.vehdjk.com/Article/details/glivnbhnw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fktsv.cn/Article/details/gwemmnfzh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.sjlbkw.cn/Article/details/gbvscvnnr.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fktsv.cn/Article/details/giewfpmwj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.epnwcf.com/Article/details/guribfdca.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.tarul.cn/Article/details/gotmxosmi.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.yfazqb.com/Article/details/gnherimdb.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.epnwcf.com/Article/details/gpuvvebgm.sHtML

Java: resp.statusCode()
来源：http://baike.epnwcf.com/Article/details/gbbhmmzdb.sHtML

Go:   resp.StatusCode
来源：http://read.share.epnwcf.com/Article/details/gouvqttyi.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fktsv.cn/Article/details/gnlksznvd.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.yfazqb.com/Article/details/gzehhehro.sHtML

[L08] 并发请求多个地址
来源：http://blog.sjlbkw.cn/Article/details/gizeuhmwq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.epnwcf.com/Article/details/gjimkfvzj.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.sjlbkw.cn/Article/details/gsvqeehiq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gnkmonttj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.sjlbkw.cn/Article/details/gprpwqgdm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.yfazqb.com/Article/details/ghtalnqob.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.bbcook.cn/Article/details/gulksxupt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.yfazqb.com/Article/details/gejuwobmg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.yfazqb.com/Article/details/gtqcqdagk.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gsxpiuxpi.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.vehdjk.com/Article/details/gnibfajbj.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gcixhnqrx.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.epnwcf.com/Article/details/gqdcggbdf.sHtML

Py:   sys.argv[1:]
来源：http://m.share.vehdjk.com/Article/details/geyjvalmg.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.vehdjk.com/Article/details/gqrvjranx.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.bbcook.cn/Article/details/gsmcbcowz.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.bbcook.cn/Article/details/glbfibjio.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.bbcook.cn/Article/details/gnqgwxduk.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.epnwcf.com/Article/details/gvazmnbqy.sHtML

Ruby: ARGV
来源：http://blog.yfazqb.com/Article/details/gbedkyqdm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.bbcook.cn/Article/details/gcvsjhvwh.sHtML

[M02] 读取环境变量
来源：http://mobile.fktsv.cn/Article/details/ggauaalvw.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gttldbolp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.yfazqb.com/Article/details/gvxmhfyld.sHtML

JS:   process.env.HOME
来源：http://blog.yfazqb.com/Article/details/guznbtqsz.sHtML

TS:   process.env.HOME
来源：http://blog.tarul.cn/Article/details/gudvvqass.sHtML

Java: System.getenv("HOME")
来源：http://baike.bbcook.cn/Article/details/gkltexxoy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.tarul.cn/Article/details/gqjzdiawl.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.yfazqb.com/Article/details/gnpgboihn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.epnwcf.com/Article/details/gjgbvvjby.sHtML

[M03] 执行外部命令
来源：http://mobile.fktsv.cn/Article/details/gpeygcwbt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.sjlbkw.cn/Article/details/gdettbvpr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.yfazqb.com/Article/details/gwasspeyh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.tarul.cn/Article/details/genxkxhlt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.tarul.cn/Article/details/groqlgupx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.sjlbkw.cn/Article/details/grllbjesi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.yfazqb.com/Article/details/gshycrjod.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.bbcook.cn/Article/details/glfxdgdsn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.sjlbkw.cn/Article/details/gwzxhgttp.sHtML

[M04] 获取当前工作目录
来源：http://read.share.tarul.cn/Article/details/gdebcfllx.sHtML

Py:   os.getcwd()
来源：http://read.share.yfazqb.com/Article/details/gqgeosamt.sHtML

PHP:  getcwd();
来源：http://read.share.sjlbkw.cn/Article/details/gptmzbuqr.sHtML

JS:   process.cwd()
来源：http://m.share.vehdjk.com/Article/details/gdxeuvlsl.sHtML

TS:   process.cwd()
来源：http://wap.fktsv.cn/Article/details/grdpxkext.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.sjlbkw.cn/Article/details/gihcjggov.sHtML

Go:   os.Getwd()
来源：http://www.blog.vehdjk.com/Article/details/gueauygmb.sHtML

Ruby: Dir.pwd
来源：http://3g.fktsv.cn/Article/details/gkuicbyvk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fktsv.cn/Article/details/gvxfumqwt.sHtML

[M05] 设置退出码
来源：http://3g.tarul.cn/Article/details/glehlaegd.sHtML

Py:   sys.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gzwfctxht.sHtML

PHP:  exit(1);
来源：http://www.blog.fktsv.cn/Article/details/gyqlxarzz.sHtML

JS:   process.exit(1)
来源：http://wap.fktsv.cn/Article/details/gatvvtznz.sHtML

TS:   process.exit(1)
来源：http://3g.yfazqb.com/Article/details/gmlwmaxqw.sHtML

Java: System.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gpkdbfyge.sHtML

Go:   os.Exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gjfptsgkn.sHtML

Ruby: exit 1
来源：http://mobile.tarul.cn/Article/details/gesqvqnwx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.vehdjk.com/Article/details/gkjmwlovb.sHtML

[M06] 向标准错误输出
来源：http://www.blog.epnwcf.com/Article/details/gmbbpgdts.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.sjlbkw.cn/Article/details/gkhrhxkau.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.sjlbkw.cn/Article/details/gyttsfzml.sHtML

JS:   console.error("err")
来源：http://mobile.epnwcf.com/Article/details/glvdzgqah.sHtML

TS:   console.error("err")
来源：http://mobile.yfazqb.com/Article/details/gzqlfwjxt.sHtML

Java: System.err.println("err")
来源：http://wap.vehdjk.com/Article/details/gjjiwzpyx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.bbcook.cn/Article/details/gzhenutha.sHtML

Ruby: warn "err"
来源：http://wap.yfazqb.com/Article/details/gxzspivfh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.yfazqb.com/Article/details/gsrsdtdgm.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fktsv.cn/Article/details/gyczwzwde.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fktsv.cn/Article/details/gsduabtej.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.epnwcf.com/Article/details/gxpymxrfz.sHtML

JS:   require.main === module
来源：http://read.share.epnwcf.com/Article/details/gxgswowki.sHtML

TS:   require.main === module
来源：http://3g.tarul.cn/Article/details/glfwiffyk.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.bbcook.cn/Article/details/gmwqijnax.sHtML

Go:   func main()
来源：http://www.m.share.vehdjk.com/Article/details/gkuofjbpr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.epnwcf.com/Article/details/gavuptmeo.sHtML

C#:   static void Main(string[] args)
来源：http://baike.tarul.cn/Article/details/gttdeeqkj.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fktsv.cn/Article/details/gaemlsgya.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.epnwcf.com/Article/details/grpnassff.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.vehdjk.com/Article/details/gjazbcmsf.sHtML

JS:   process.platform;  process.version
来源：http://blog.fktsv.cn/Article/details/guorpsbhu.sHtML

TS:   process.platform;  process.version
来源：http://baike.yfazqb.com/Article/details/gukvhdsaq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.vehdjk.com/Article/details/gjixcxccz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.yfazqb.com/Article/details/gvpqzemrg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.bbcook.cn/Article/details/ghfezaqtz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.yfazqb.com/Article/details/gagwibbvz.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gzpwassiu.sHtML

N. 数据结构与算法
来源：http://wap.epnwcf.com/Article/details/gpyqvomsu.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ggqsgmovk.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.tarul.cn/Article/details/gjknqfbkr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gzvhcygcl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fktsv.cn/Article/details/gabdegrpg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.sjlbkw.cn/Article/details/gknczeelp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.yfazqb.com/Article/details/grfrhbzxj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.bbcook.cn/Article/details/gsqmnhrim.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gnrddvcuy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.sjlbkw.cn/Article/details/gcvrzkdse.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gpijsmves.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.sjlbkw.cn/Article/details/gtsqowlrf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.epnwcf.com/Article/details/guusgzobj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.sjlbkw.cn/Article/details/gtrhezhym.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.bbcook.cn/Article/details/gcfhvsqvu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.tarul.cn/Article/details/gkomxeedq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.vehdjk.com/Article/details/geivriyjx.sHtML

Go:   slices.Sort(arr)
来源：http://blog.epnwcf.com/Article/details/gckynswev.sHtML

Ruby: arr.sort
来源：http://blog.yfazqb.com/Article/details/gvqrcoxeg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.vehdjk.com/Article/details/gkjxqzuce.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.tarul.cn/Article/details/gqffuqwdy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.tarul.cn/Article/details/ggreqabxe.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.yfazqb.com/Article/details/gwakunzgu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.vehdjk.com/Article/details/gwajwprnh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.tarul.cn/Article/details/gxvlfehlh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.sjlbkw.cn/Article/details/gyrqslyew.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.tarul.cn/Article/details/gqsstdsoe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.vehdjk.com/Article/details/grgfuwqik.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fktsv.cn/Article/details/gasgbddrr.sHtML

[N04] 斐波那契数列
来源：http://blog.tarul.cn/Article/details/gtzqnyqix.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.epnwcf.com/Article/details/gsvjedade.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.sjlbkw.cn/Article/details/gmtmpoydv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/gjcqyctxw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/gyuukmomi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.yfazqb.com/Article/details/gnmpjfpxj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.vehdjk.com/Article/details/gamhaabmv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.yfazqb.com/Article/details/gmkuqnsnx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/gifpezsse.sHtML

[N05] 最大公约数
来源：http://www.m.share.yfazqb.com/Article/details/gcvkwxnlj.sHtML

Py:   math.gcd(a, b)
来源：http://baike.yfazqb.com/Article/details/gredkutdo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gbkvvvqyr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.bbcook.cn/Article/details/gpzrnxbjt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fktsv.cn/Article/details/gcbnhgycx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.vehdjk.com/Article/details/grquvjzsx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.vehdjk.com/Article/details/glulaesgg.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.tarul.cn/Article/details/gqbrflbiw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.epnwcf.com/Article/details/gqudminjo.sHtML

[N06] 判断回文字符串
来源：http://www.blog.epnwcf.com/Article/details/gkznnfrww.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.bbcook.cn/Article/details/gflxrhmgp.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.epnwcf.com/Article/details/gmgcqmtfj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gasdmnids.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gxirtnwdb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.sjlbkw.cn/Article/details/gztsooiuu.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.tarul.cn/Article/details/gdnxurbbo.sHtML

Ruby: s == s.reverse
来源：http://3g.vehdjk.com/Article/details/gkbwulcut.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.tarul.cn/Article/details/gdfzbnxne.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.sjlbkw.cn/Article/details/gvwnjhxbj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.yfazqb.com/Article/details/gdgqolphu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.yfazqb.com/Article/details/gicbtzdwd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.tarul.cn/Article/details/gqhpxioia.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.sjlbkw.cn/Article/details/gzdxteslc.sHtML

Java: // 手写 HashMap
来源：http://www.share.yfazqb.com/Article/details/gniwokrzc.sHtML

Go:   // 手写 map[int]int
来源：http://wap.sjlbkw.cn/Article/details/gururghxk.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.epnwcf.com/Article/details/goqpsuolt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.sjlbkw.cn/Article/details/gyrwwinxa.sHtML

[N08] 生成全排列
来源：http://read.share.sjlbkw.cn/Article/details/gsasrxkpp.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.sjlbkw.cn/Article/details/gfdpbgzis.sHtML

PHP:  // 手写递归交换
来源：http://mobile.epnwcf.com/Article/details/ggbxpmury.sHtML

JS:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gwabzxoit.sHtML

TS:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gochizwpm.sHtML

Java: // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/ghopexhbr.sHtML

Go:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gtvbqkoan.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.vehdjk.com/Article/details/gfcwhcjdo.sHtML

C#:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gquigtqbc.sHtML

[N09] 栈与队列
来源：http://3g.vehdjk.com/Article/details/gtmdoagmo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.sjlbkw.cn/Article/details/guznxncog.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.yfazqb.com/Article/details/gquisgdic.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkyavttz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.tarul.cn/Article/details/gjiroesqb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.epnwcf.com/Article/details/gejvpewle.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fktsv.cn/Article/details/gfxoqhxlf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.sjlbkw.cn/Article/details/gjlcfnfng.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.tarul.cn/Article/details/gobrhciai.sHtML

[N10] 链表节点定义
来源：http://www.blog.epnwcf.com/Article/details/gqqpdnmxk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.sjlbkw.cn/Article/details/glnvrdtif.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.epnwcf.com/Article/details/guxnsngrl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.bbcook.cn/Article/details/gsnzaezet.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.vehdjk.com/Article/details/gjjtnxlpp.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.bbcook.cn/Article/details/gsevsnzck.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.tarul.cn/Article/details/guusexjtz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.yfazqb.com/Article/details/gqswefxvy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.bbcook.cn/Article/details/griebetzg.sHtML

[N11] 二叉树中序遍历
来源：http://wap.epnwcf.com/Article/details/gribxnfdu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fktsv.cn/Article/details/gaiqhkyxs.sHtML

PHP:  // 手写递归函数
来源：http://m.share.epnwcf.com/Article/details/gxcjdlvpe.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.vehdjk.com/Article/details/gotgiqlaq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.bbcook.cn/Article/details/gluhvvldr.sHtML

Java: // 手写递归
来源：http://3g.sjlbkw.cn/Article/details/gjwpphcve.sHtML

Go:   // 手写递归
来源：http://3g.vehdjk.com/Article/details/gnlciaazc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.bbcook.cn/Article/details/grkrqqlug.sHtML

C#:   // 手写递归
来源：http://baike.vehdjk.com/Article/details/gdatrcnqi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.yfazqb.com/Article/details/gwskvwelg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.sjlbkw.cn/Article/details/grqfyclro.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.bbcook.cn/Article/details/gqrrzqbrb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.yfazqb.com/Article/details/gpxjorrmq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.bbcook.cn/Article/details/griyedkod.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.tarul.cn/Article/details/gdtigspgd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.bbcook.cn/Article/details/gpjwgftlz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.yfazqb.com/Article/details/gqfkoazbu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.epnwcf.com/Article/details/gypydisxf.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gwiooqgsu.sHtML

O. 并发与异步
来源：http://www.share.bbcook.cn/Article/details/gcbxazyoh.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gsnmkwfca.sHtML

[O01] 启动一个线程
来源：http://wap.fktsv.cn/Article/details/gpjmckrnv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.vehdjk.com/Article/details/gdkqwujtc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.tarul.cn/Article/details/gzdxhqzdk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.vehdjk.com/Article/details/gptnabdbe.sHtML

TS:   // 同 JS
来源：http://read.share.vehdjk.com/Article/details/gymjenoog.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.sjlbkw.cn/Article/details/gyvknqilw.sHtML

Go:   go f()
来源：http://3g.epnwcf.com/Article/details/gcsxxituk.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fktsv.cn/Article/details/gksiywezi.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fktsv.cn/Article/details/gdqyngdxb.sHtML

[O02] 使用线程池
来源：http://mobile.fktsv.cn/Article/details/gndxowtxt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.epnwcf.com/Article/details/gvirhethi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fktsv.cn/Article/details/gnebyxujc.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.vehdjk.com/Article/details/gyvejrhkz.sHtML

TS:   // worker_threads 线程池
来源：http://3g.tarul.cn/Article/details/giubmdbte.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.bbcook.cn/Article/details/gkwnlxmzy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fktsv.cn/Article/details/ghcrjiwdb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.tarul.cn/Article/details/gfccpnilv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.tarul.cn/Article/details/gdqsfoert.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.tarul.cn/Article/details/gvvkyycpd.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.yfazqb.com/Article/details/ggynykodg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.bbcook.cn/Article/details/gbsgydpep.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.bbcook.cn/Article/details/gwztghbir.sHtML

TS:   // 同 JS
来源：http://read.share.tarul.cn/Article/details/gvdehhfoe.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.vehdjk.com/Article/details/gypucpaoc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fktsv.cn/Article/details/gxvwguggc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.bbcook.cn/Article/details/gzilgabbv.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.yfazqb.com/Article/details/givfdzivl.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.sjlbkw.cn/Article/details/gyrgwjmpt.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.yfazqb.com/Article/details/gwrkvbjiv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.epnwcf.com/Article/details/gkkcdibmp.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.bbcook.cn/Article/details/gzsigdstq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fktsv.cn/Article/details/gpkzxqvko.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.tarul.cn/Article/details/gsdkfgngx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fktsv.cn/Article/details/gtnvvnvzz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fktsv.cn/Article/details/gantgkyxd.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.yfazqb.com/Article/details/griqyklec.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.vehdjk.com/Article/details/gjyydfexe.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.tarul.cn/Article/details/gkhbubswd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.yfazqb.com/Article/details/grdyrlgug.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.tarul.cn/Article/details/gkhqwjeqi.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/gxtkxpnzx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.tarul.cn/Article/details/gvrosvyvy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.epnwcf.com/Article/details/gjnsxqiyd.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.bbcook.cn/Article/details/gaefpqpyg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.sjlbkw.cn/Article/details/gibgkicnz.sHtML

[O06] 使用进程池
来源：http://blog.tarul.cn/Article/details/gyomdqctu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.yfazqb.com/Article/details/gxnfqltto.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.epnwcf.com/Article/details/gwfyyhqgj.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.epnwcf.com/Article/details/gbdybdslv.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.yfazqb.com/Article/details/gfittoncy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.sjlbkw.cn/Article/details/gmowrqlcf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.bbcook.cn/Article/details/gjdxtmcgz.sHtML

Ruby: // fork 块
来源：http://www.blog.tarul.cn/Article/details/gwaiypltd.sHtML

C#:   Parallel.For
来源：http://read.share.epnwcf.com/Article/details/gpenvgpym.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gtwmcgyio.sHtML

P. 常用工具函数
来源：http://wap.tarul.cn/Article/details/glruebfsn.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gduwzigpc.sHtML

[P01] 生成 UUID
来源：http://www.m.share.yfazqb.com/Article/details/gybzngpso.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.sjlbkw.cn/Article/details/goneptefp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.yfazqb.com/Article/details/giocnbywi.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fktsv.cn/Article/details/gmhzhkodw.sHtML

TS:   crypto.randomUUID()
来源：http://wap.epnwcf.com/Article/details/gznzfcxhv.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.yfazqb.com/Article/details/gmdqlgazf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.vehdjk.com/Article/details/grnfmgmvu.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.yfazqb.com/Article/details/gllnjyhjz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.sjlbkw.cn/Article/details/gccizkvdz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjzuscjf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fktsv.cn/Article/details/gwvlkdeig.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.bbcook.cn/Article/details/gplzfugus.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.bbcook.cn/Article/details/gmgpjbwmh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.epnwcf.com/Article/details/gkmkupxtr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.yfazqb.com/Article/details/gzkfqpzia.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.tarul.cn/Article/details/gthougory.sHtML


<!-- 参考信息 -->