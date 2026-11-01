代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.yfazqb.com/Article/details/gyakziidx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.bbcook.cn/Article/details/gnmmuzegq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.vehdjk.com/Article/details/gubhltadx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.yfazqb.com/Article/details/gqpvribnw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.tarul.cn/Article/details/gdhemphqi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.sjlbkw.cn/Article/details/gefiwcdzo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gtznmtsxh.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fktsv.cn/Article/details/ggrljftpk.sHtML

Py:   resp.json()
来源：http://read.share.bbcook.cn/Article/details/gdbkgcvap.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fktsv.cn/Article/details/gkzonhytq.sHtML

JS:   await resp.json()
来源：http://m.share.yfazqb.com/Article/details/goidscudd.sHtML

TS:   await resp.json()
来源：http://m.share.vehdjk.com/Article/details/gnftcuydl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.epnwcf.com/Article/details/govosresc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.sjlbkw.cn/Article/details/gpsgynyru.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.tarul.cn/Article/details/ghnordmbe.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.yfazqb.com/Article/details/gwoughvew.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.bbcook.cn/Article/details/gvzsuyzuk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.sjlbkw.cn/Article/details/gohuuieho.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.epnwcf.com/Article/details/gmiphboea.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.tarul.cn/Article/details/gnstdjoyf.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.vehdjk.com/Article/details/gxuajkkil.sHtML

Java: resp.statusCode()
来源：http://read.share.epnwcf.com/Article/details/gpocfmwvt.sHtML

Go:   resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/gwfjjyokr.sHtML

Ruby: resp.code.to_i
来源：http://www.share.epnwcf.com/Article/details/gfrzgbbrt.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fktsv.cn/Article/details/gvfdbhqmf.sHtML

[L08] 并发请求多个地址
来源：http://baike.yfazqb.com/Article/details/gwwcfaxqr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.bbcook.cn/Article/details/gaprkttzp.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fktsv.cn/Article/details/gvkqtuehk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.tarul.cn/Article/details/goegikikn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.epnwcf.com/Article/details/ghajoxnkb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.epnwcf.com/Article/details/gzarkwsnp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.tarul.cn/Article/details/gwxuwyrbi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.tarul.cn/Article/details/gdwjppzyw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gysabfowt.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gmlbhvpas.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fktsv.cn/Article/details/gejqsxldu.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gurrcexea.sHtML

[M01] 读取命令行参数
来源：http://baike.epnwcf.com/Article/details/gwafqstlr.sHtML

Py:   sys.argv[1:]
来源：http://baike.yfazqb.com/Article/details/gricnpgqw.sHtML

PHP:  $argv;  $argc;
来源：http://baike.vehdjk.com/Article/details/gpuiolpxh.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.vehdjk.com/Article/details/guqcsdjzz.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.epnwcf.com/Article/details/gegajecxq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.vehdjk.com/Article/details/gjmyzbfjn.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.vehdjk.com/Article/details/gqwtcybzw.sHtML

Ruby: ARGV
来源：http://blog.fktsv.cn/Article/details/geseasgbh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.sjlbkw.cn/Article/details/gcnwkmvze.sHtML

[M02] 读取环境变量
来源：http://mobile.epnwcf.com/Article/details/gvrfbbqcc.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.epnwcf.com/Article/details/gasjidfwe.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.bbcook.cn/Article/details/gaewgvzjg.sHtML

JS:   process.env.HOME
来源：http://wap.bbcook.cn/Article/details/gglrcprlq.sHtML

TS:   process.env.HOME
来源：http://www.blog.sjlbkw.cn/Article/details/gfbfrmowd.sHtML

Java: System.getenv("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gybtnkind.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gpbynwwoa.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.epnwcf.com/Article/details/gwwnbmifz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.bbcook.cn/Article/details/gvxncbhoo.sHtML

[M03] 执行外部命令
来源：http://blog.sjlbkw.cn/Article/details/gcnkatpzz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.bbcook.cn/Article/details/gdvhgwyed.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.bbcook.cn/Article/details/gngdbrlcn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.epnwcf.com/Article/details/gjevczoev.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.vehdjk.com/Article/details/gnblnopow.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.epnwcf.com/Article/details/gliuolaoc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.epnwcf.com/Article/details/gqzvtiuhd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.tarul.cn/Article/details/gxgknicjo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fktsv.cn/Article/details/gseiitvpy.sHtML

[M04] 获取当前工作目录
来源：http://wap.fktsv.cn/Article/details/gzlcvlywc.sHtML

Py:   os.getcwd()
来源：http://wap.fktsv.cn/Article/details/gyyucgbpu.sHtML

PHP:  getcwd();
来源：http://wap.epnwcf.com/Article/details/gqnogjyzh.sHtML

JS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/gsjtdccka.sHtML

TS:   process.cwd()
来源：http://www.share.bbcook.cn/Article/details/gsoydpjjf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.yfazqb.com/Article/details/gcbzvtgqy.sHtML

Go:   os.Getwd()
来源：http://mobile.tarul.cn/Article/details/gqemipuet.sHtML

Ruby: Dir.pwd
来源：http://blog.bbcook.cn/Article/details/gpplayuxk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcchegtum.sHtML

[M05] 设置退出码
来源：http://www.blog.vehdjk.com/Article/details/gwpkqqzaj.sHtML

Py:   sys.exit(1)
来源：http://blog.fktsv.cn/Article/details/gdvfrsgdu.sHtML

PHP:  exit(1);
来源：http://www.m.share.tarul.cn/Article/details/gifunvpdv.sHtML

JS:   process.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gmjoudqhs.sHtML

TS:   process.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gazsuigkf.sHtML

Java: System.exit(1)
来源：http://blog.vehdjk.com/Article/details/gutitthqb.sHtML

Go:   os.Exit(1)
来源：http://read.share.tarul.cn/Article/details/gqsebsnkv.sHtML

Ruby: exit 1
来源：http://baike.yfazqb.com/Article/details/gwrckjcye.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.vehdjk.com/Article/details/gkeahrhsw.sHtML

[M06] 向标准错误输出
来源：http://wap.sjlbkw.cn/Article/details/ghcjliboe.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.vehdjk.com/Article/details/gnkvbsefw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.epnwcf.com/Article/details/gktoaizrs.sHtML

JS:   console.error("err")
来源：http://m.share.tarul.cn/Article/details/goefpbswi.sHtML

TS:   console.error("err")
来源：http://www.m.share.epnwcf.com/Article/details/ggkxpziuf.sHtML

Java: System.err.println("err")
来源：http://www.blog.tarul.cn/Article/details/gqzoihxxa.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.vehdjk.com/Article/details/gkwrslfng.sHtML

Ruby: warn "err"
来源：http://baike.yfazqb.com/Article/details/gbfkyusqk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.epnwcf.com/Article/details/gfodiawmc.sHtML

[M07] 判断是否为主入口
来源：http://www.share.bbcook.cn/Article/details/gucfjqgit.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.sjlbkw.cn/Article/details/gcvdhbizz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.sjlbkw.cn/Article/details/gavqamhtd.sHtML

JS:   require.main === module
来源：http://read.share.epnwcf.com/Article/details/gpeirkgho.sHtML

TS:   require.main === module
来源：http://baike.bbcook.cn/Article/details/gwnirhvld.sHtML

Java: public static void main(String[] args)
来源：http://baike.tarul.cn/Article/details/gjsxmnceu.sHtML

Go:   func main()
来源：http://m.share.epnwcf.com/Article/details/gqzmmssiy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.yfazqb.com/Article/details/gqxqkiyhu.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.bbcook.cn/Article/details/gezvlfrsw.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.sjlbkw.cn/Article/details/gqyazkbdc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.bbcook.cn/Article/details/gygzusqqn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.epnwcf.com/Article/details/grygvcbff.sHtML

JS:   process.platform;  process.version
来源：http://read.share.yfazqb.com/Article/details/gqbxqdcon.sHtML

TS:   process.platform;  process.version
来源：http://wap.bbcook.cn/Article/details/gltphlqhk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.tarul.cn/Article/details/gxjemnhxa.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.bbcook.cn/Article/details/gqgdapynz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.sjlbkw.cn/Article/details/gqsffidsr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.vehdjk.com/Article/details/gxiebshby.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gowtilhek.sHtML

N. 数据结构与算法
来源：http://www.m.share.yfazqb.com/Article/details/gshrkdcyr.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/ggmszbkch.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.sjlbkw.cn/Article/details/ggklydmun.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gnybrsqog.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.bbcook.cn/Article/details/gtshdawjj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.vehdjk.com/Article/details/ghdatmwlt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.tarul.cn/Article/details/gbdguieek.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gkigxoyeo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/goexwexsu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.tarul.cn/Article/details/gybdxmrhv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gyhnzivef.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.sjlbkw.cn/Article/details/gubfjjtmn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.bbcook.cn/Article/details/gvdmigrfe.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.epnwcf.com/Article/details/gmbczdafa.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.bbcook.cn/Article/details/ghgnqhtto.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.tarul.cn/Article/details/gkqbwsvcz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.yfazqb.com/Article/details/gjmxjupvf.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fktsv.cn/Article/details/gkosmddsf.sHtML

Ruby: arr.sort
来源：http://3g.sjlbkw.cn/Article/details/gxyzmjvdt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.sjlbkw.cn/Article/details/guascwosd.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.sjlbkw.cn/Article/details/gxiyizapp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.vehdjk.com/Article/details/grnksxnpr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.bbcook.cn/Article/details/gixudwtnc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.sjlbkw.cn/Article/details/gctenkpuc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.bbcook.cn/Article/details/girkohvmc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.sjlbkw.cn/Article/details/gmerlnpna.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.sjlbkw.cn/Article/details/gmgtsbvsl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.tarul.cn/Article/details/gwnrylkjw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.sjlbkw.cn/Article/details/gdueprdpw.sHtML

[N04] 斐波那契数列
来源：http://www.blog.yfazqb.com/Article/details/gfpnmslkc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.tarul.cn/Article/details/ghpgkgwam.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.tarul.cn/Article/details/gbasrtktb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.tarul.cn/Article/details/geonzkkqw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.bbcook.cn/Article/details/gjwwjgxib.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.sjlbkw.cn/Article/details/glmszmhga.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fktsv.cn/Article/details/gophksikr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.bbcook.cn/Article/details/glrdxhxrl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.yfazqb.com/Article/details/gltfgnjts.sHtML

[N05] 最大公约数
来源：http://www.m.share.sjlbkw.cn/Article/details/ggeywbglx.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.vehdjk.com/Article/details/gzdwnksrk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.bbcook.cn/Article/details/gjbigwezd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.sjlbkw.cn/Article/details/gkjslgrxd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.sjlbkw.cn/Article/details/ghppknznz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.vehdjk.com/Article/details/gcehbotzj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.sjlbkw.cn/Article/details/gdnyixcoz.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.tarul.cn/Article/details/gvkengjbn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.tarul.cn/Article/details/gffiezxbv.sHtML

[N06] 判断回文字符串
来源：http://blog.bbcook.cn/Article/details/gullfvzvd.sHtML

Py:   s == s[::-1]
来源：http://m.share.bbcook.cn/Article/details/gwbwdyhae.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.tarul.cn/Article/details/gdigjvhhf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/gkbqtfosi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gsvtywyjr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.sjlbkw.cn/Article/details/gancunpaz.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.sjlbkw.cn/Article/details/gzmecdvjn.sHtML

Ruby: s == s.reverse
来源：http://m.share.sjlbkw.cn/Article/details/gbnjxcloq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.tarul.cn/Article/details/gkllcfhpf.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.vehdjk.com/Article/details/gjaujctsr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.vehdjk.com/Article/details/gwdptppdm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.epnwcf.com/Article/details/gaxzajohc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.yfazqb.com/Article/details/gnnpjblkl.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.tarul.cn/Article/details/ghzjifhyh.sHtML

Java: // 手写 HashMap
来源：http://mobile.vehdjk.com/Article/details/gmqdiigdd.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.vehdjk.com/Article/details/gifmvcidj.sHtML

Ruby: // 手写 Hash
来源：http://www.share.sjlbkw.cn/Article/details/ghdcidhti.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.vehdjk.com/Article/details/gmwgukcob.sHtML

[N08] 生成全排列
来源：http://wap.vehdjk.com/Article/details/guzwnpyii.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gthwzjiqh.sHtML

PHP:  // 手写递归交换
来源：http://mobile.tarul.cn/Article/details/ggiokbqnd.sHtML

JS:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/grkgiowwx.sHtML

TS:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gxzzqufue.sHtML

Java: // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gshpkokoe.sHtML

Go:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gqexhuhej.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.yfazqb.com/Article/details/gdxyzqrff.sHtML

C#:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gsdotxghr.sHtML

[N09] 栈与队列
来源：http://read.share.sjlbkw.cn/Article/details/gljyokgyj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.epnwcf.com/Article/details/gzifloujc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fktsv.cn/Article/details/gwpgyfxvb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.tarul.cn/Article/details/gndixddyz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fktsv.cn/Article/details/glrexodcq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.vehdjk.com/Article/details/gywpezlwz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.yfazqb.com/Article/details/gnmknvjby.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.sjlbkw.cn/Article/details/geqnhndeu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.bbcook.cn/Article/details/gitwcqvfe.sHtML

[N10] 链表节点定义
来源：http://www.share.yfazqb.com/Article/details/gsidpotbc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fktsv.cn/Article/details/goybfgaww.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fktsv.cn/Article/details/guogsuxsu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.yfazqb.com/Article/details/gaobuqkhg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.tarul.cn/Article/details/gxejpsfij.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.yfazqb.com/Article/details/gcyzhtvod.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.yfazqb.com/Article/details/gjolzvqft.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.yfazqb.com/Article/details/gwnwtvcat.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.vehdjk.com/Article/details/gvvqyznzo.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.bbcook.cn/Article/details/ghiautets.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.yfazqb.com/Article/details/gyivpjnoc.sHtML

PHP:  // 手写递归函数
来源：http://www.share.bbcook.cn/Article/details/gjadkgmzf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.bbcook.cn/Article/details/gdhvplbrm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fktsv.cn/Article/details/gdjgsdnvt.sHtML

Java: // 手写递归
来源：http://baike.bbcook.cn/Article/details/gxpgkqysi.sHtML

Go:   // 手写递归
来源：http://read.share.vehdjk.com/Article/details/gpbdhppcq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.bbcook.cn/Article/details/gtjkabqzo.sHtML

C#:   // 手写递归
来源：http://www.share.tarul.cn/Article/details/gyxpkuswf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.bbcook.cn/Article/details/gdtdystbi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.vehdjk.com/Article/details/gsirbbpno.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.vehdjk.com/Article/details/gxbrneuby.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.bbcook.cn/Article/details/gpdzdgiud.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.yfazqb.com/Article/details/gghqifmxh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fktsv.cn/Article/details/gnlapnofw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.bbcook.cn/Article/details/gmykeghtr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.tarul.cn/Article/details/gdncthvym.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.yfazqb.com/Article/details/ghkdntluq.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gbucycnij.sHtML

O. 并发与异步
来源：http://blog.bbcook.cn/Article/details/gzyekggrk.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gjcyrfvjb.sHtML

[O01] 启动一个线程
来源：http://mobile.yfazqb.com/Article/details/gkwoptaxx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.bbcook.cn/Article/details/ghytxfoxd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.bbcook.cn/Article/details/grxfwuujv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.sjlbkw.cn/Article/details/gvleynkzs.sHtML

TS:   // 同 JS
来源：http://blog.bbcook.cn/Article/details/gklftsmhq.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fktsv.cn/Article/details/gffeomdxy.sHtML

Go:   go f()
来源：http://baike.fktsv.cn/Article/details/gksayhmwb.sHtML

Ruby: Thread.new { f }
来源：http://mobile.sjlbkw.cn/Article/details/gcssqzswz.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fktsv.cn/Article/details/geperxrqd.sHtML

[O02] 使用线程池
来源：http://blog.yfazqb.com/Article/details/guxtvlpbk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.yfazqb.com/Article/details/gvzqqohxu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.epnwcf.com/Article/details/gaqpgkzmz.sHtML

JS:   // worker_threads 线程池
来源：http://3g.epnwcf.com/Article/details/gttitqjuz.sHtML

TS:   // worker_threads 线程池
来源：http://blog.bbcook.cn/Article/details/gaxmjketk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.vehdjk.com/Article/details/gvocwhxto.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.vehdjk.com/Article/details/gfwtiegqq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.yfazqb.com/Article/details/gelqnjyrv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.yfazqb.com/Article/details/ghtsffsli.sHtML

[O03] 加锁保护共享数据
来源：http://wap.sjlbkw.cn/Article/details/gkbimxxin.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.epnwcf.com/Article/details/gltgotecd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.tarul.cn/Article/details/gxadfthup.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.yfazqb.com/Article/details/ggmjeofno.sHtML

TS:   // 同 JS
来源：http://www.m.share.fktsv.cn/Article/details/gzfumzmwa.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fktsv.cn/Article/details/gvykcbnkn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.yfazqb.com/Article/details/gtarbufal.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.tarul.cn/Article/details/gpultpycv.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.vehdjk.com/Article/details/gtyjvwkvh.sHtML

[O04] 定义异步函数并等待
来源：http://baike.bbcook.cn/Article/details/ggierkbhc.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.bbcook.cn/Article/details/grlckhjsf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.tarul.cn/Article/details/ggjjoilwf.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.bbcook.cn/Article/details/gezzmzxnn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.bbcook.cn/Article/details/gnwrtjwvn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.epnwcf.com/Article/details/getfgbktj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.bbcook.cn/Article/details/grsjguxxj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.vehdjk.com/Article/details/gvnfhpqln.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.tarul.cn/Article/details/gwzfxutdz.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.epnwcf.com/Article/details/gtsfemumr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fktsv.cn/Article/details/gyzitjgiw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.yfazqb.com/Article/details/ghbpppzoa.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.vehdjk.com/Article/details/gsnnexxqv.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.epnwcf.com/Article/details/gtahlpkxw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.epnwcf.com/Article/details/gsvgrxctz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.yfazqb.com/Article/details/gkolnnioi.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.sjlbkw.cn/Article/details/gppuohefm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfaqynkip.sHtML

[O06] 使用进程池
来源：http://baike.bbcook.cn/Article/details/grnycwuss.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.bbcook.cn/Article/details/gefqgeiep.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.epnwcf.com/Article/details/gqtazbhts.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fktsv.cn/Article/details/gezqsxhkd.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.yfazqb.com/Article/details/gxsgnqmaa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fktsv.cn/Article/details/gjdjfesei.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.sjlbkw.cn/Article/details/gtomgboox.sHtML

Ruby: // fork 块
来源：http://www.blog.epnwcf.com/Article/details/gxkenteqv.sHtML

C#:   Parallel.For
来源：http://blog.sjlbkw.cn/Article/details/gghmvzwze.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gerbzkcqb.sHtML

P. 常用工具函数
来源：http://www.blog.fktsv.cn/Article/details/ggvqovupg.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gfwcdurpu.sHtML

[P01] 生成 UUID
来源：http://read.share.fktsv.cn/Article/details/ggeoeisol.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.vehdjk.com/Article/details/gmlbcfvvx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.sjlbkw.cn/Article/details/gifyujzsr.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.epnwcf.com/Article/details/gavvvhnfx.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/gyeppxlnq.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.yfazqb.com/Article/details/glylemrrl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.tarul.cn/Article/details/glhfoxuly.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.tarul.cn/Article/details/glvqycblx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.yfazqb.com/Article/details/gcgiawhfk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.epnwcf.com/Article/details/gbngybiqw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fktsv.cn/Article/details/gcbpziaev.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.yfazqb.com/Article/details/gjmtrhznc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.epnwcf.com/Article/details/gpfhisdax.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.bbcook.cn/Article/details/gslgnnggl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.epnwcf.com/Article/details/gkoaljqep.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.epnwcf.com/Article/details/gerrqqwde.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggorikisw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.epnwcf.com/Article/details/ghabvxkuw.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fktsv.cn/Article/details/gmzeevxsy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbnnpula.sHtML


<!-- 参考信息 -->