代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.tarul.cn/Article/details/gdflulpkz.sHtML

[L04] 设置超时
来源：http://mobile.sjlbkw.cn/Article/details/gxptwvznh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.yfazqb.com/Article/details/gmrefpzmp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.epnwcf.com/Article/details/gxtamovue.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.sjlbkw.cn/Article/details/ghrosuuls.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fktsv.cn/Article/details/gvidonfxl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.vehdjk.com/Article/details/gcidydhbv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.yfazqb.com/Article/details/gqqskdlpg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.yfazqb.com/Article/details/ggsswesiv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.sjlbkw.cn/Article/details/gjrxmsvtn.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.bbcook.cn/Article/details/gyriofeed.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.vehdjk.com/Article/details/gbdetyqtn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.epnwcf.com/Article/details/gllblrdkv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.vehdjk.com/Article/details/grctdonry.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fktsv.cn/Article/details/goqrckewd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fktsv.cn/Article/details/grpxnkqex.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.vehdjk.com/Article/details/gagucpusp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.sjlbkw.cn/Article/details/ggjkpftaa.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.yfazqb.com/Article/details/grmjgdcbe.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.tarul.cn/Article/details/ghznjtyzc.sHtML

Py:   resp.json()
来源：http://read.share.epnwcf.com/Article/details/gxpqmnyrx.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.vehdjk.com/Article/details/gebeaajyc.sHtML

JS:   await resp.json()
来源：http://baike.epnwcf.com/Article/details/gpernnboz.sHtML

TS:   await resp.json()
来源：http://blog.sjlbkw.cn/Article/details/gxudjgmhs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.yfazqb.com/Article/details/gsqepzbwx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.sjlbkw.cn/Article/details/glfvyhpbi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.bbcook.cn/Article/details/gcoxntcdw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.sjlbkw.cn/Article/details/ghajjtcrp.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.tarul.cn/Article/details/glamspnyw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fktsv.cn/Article/details/gaappueis.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.bbcook.cn/Article/details/gimwpxdks.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.epnwcf.com/Article/details/gqptcwcpm.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fktsv.cn/Article/details/giofwckyi.sHtML

Java: resp.statusCode()
来源：http://mobile.bbcook.cn/Article/details/gikwqkadn.sHtML

Go:   resp.StatusCode
来源：http://www.share.epnwcf.com/Article/details/gulheanil.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.yfazqb.com/Article/details/gblwrdczj.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.vehdjk.com/Article/details/gdfmavpzg.sHtML

[L08] 并发请求多个地址
来源：http://blog.fktsv.cn/Article/details/gfjtlwneu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.sjlbkw.cn/Article/details/gmfdkuqwb.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fktsv.cn/Article/details/gbsvbxkmd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.yfazqb.com/Article/details/gtdwucxfr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.yfazqb.com/Article/details/gzixdnsnp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.tarul.cn/Article/details/gjkcknpto.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.epnwcf.com/Article/details/ggdswtxqo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fktsv.cn/Article/details/gghydfiht.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.vehdjk.com/Article/details/gondlnjhn.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/glanruveh.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.vehdjk.com/Article/details/gjnnjdnuw.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/giozrvvas.sHtML

[M01] 读取命令行参数
来源：http://www.blog.vehdjk.com/Article/details/gxuqnuith.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.epnwcf.com/Article/details/gqambimri.sHtML

PHP:  $argv;  $argc;
来源：http://wap.yfazqb.com/Article/details/gwwnbuuma.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.epnwcf.com/Article/details/gcrehesxk.sHtML

TS:   process.argv.slice(2)
来源：http://wap.bbcook.cn/Article/details/gwoncdslm.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.vehdjk.com/Article/details/ggixamjgm.sHtML

Go:   os.Args[1:]
来源：http://www.share.tarul.cn/Article/details/gjixaesyn.sHtML

Ruby: ARGV
来源：http://www.m.share.vehdjk.com/Article/details/gbledkurk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.bbcook.cn/Article/details/grhmxkdbv.sHtML

[M02] 读取环境变量
来源：http://mobile.tarul.cn/Article/details/gsjnwjxpe.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gpihozxyb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fktsv.cn/Article/details/gyvrubiup.sHtML

JS:   process.env.HOME
来源：http://3g.epnwcf.com/Article/details/gibkllxdd.sHtML

TS:   process.env.HOME
来源：http://wap.vehdjk.com/Article/details/gufcxokja.sHtML

Java: System.getenv("HOME")
来源：http://wap.bbcook.cn/Article/details/gmhjtusdd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.yfazqb.com/Article/details/gadzmrgrn.sHtML

Ruby: ENV["HOME"]
来源：http://blog.tarul.cn/Article/details/girazpwon.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.tarul.cn/Article/details/geowtnydc.sHtML

[M03] 执行外部命令
来源：http://read.share.bbcook.cn/Article/details/gajkcmyis.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.yfazqb.com/Article/details/gxosxunvb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.yfazqb.com/Article/details/gvvtbglgd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.yfazqb.com/Article/details/giybkweuu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.bbcook.cn/Article/details/gwjwuvfer.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.vehdjk.com/Article/details/gqyouyild.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.epnwcf.com/Article/details/gxupedcse.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.sjlbkw.cn/Article/details/gnzewvysi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fktsv.cn/Article/details/gdchdoegs.sHtML

[M04] 获取当前工作目录
来源：http://blog.vehdjk.com/Article/details/gdmrniehx.sHtML

Py:   os.getcwd()
来源：http://wap.bbcook.cn/Article/details/gbsuirzvj.sHtML

PHP:  getcwd();
来源：http://baike.tarul.cn/Article/details/goqveobsy.sHtML

JS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/gjnwqpmia.sHtML

TS:   process.cwd()
来源：http://wap.bbcook.cn/Article/details/gdjfzcqbe.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.bbcook.cn/Article/details/ghuveiebm.sHtML

Go:   os.Getwd()
来源：http://www.share.epnwcf.com/Article/details/gmapbujsu.sHtML

Ruby: Dir.pwd
来源：http://blog.bbcook.cn/Article/details/gcxoxmvov.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.sjlbkw.cn/Article/details/gwswwadbr.sHtML

[M05] 设置退出码
来源：http://www.blog.sjlbkw.cn/Article/details/gxzfpwidk.sHtML

Py:   sys.exit(1)
来源：http://m.share.tarul.cn/Article/details/gtwoyyxxj.sHtML

PHP:  exit(1);
来源：http://3g.tarul.cn/Article/details/gokznxjxf.sHtML

JS:   process.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gxlmwamsl.sHtML

TS:   process.exit(1)
来源：http://3g.epnwcf.com/Article/details/gqmmmmtjt.sHtML

Java: System.exit(1)
来源：http://baike.vehdjk.com/Article/details/gosbuobla.sHtML

Go:   os.Exit(1)
来源：http://3g.bbcook.cn/Article/details/gbatpokzh.sHtML

Ruby: exit 1
来源：http://www.m.share.epnwcf.com/Article/details/ggqqxzcbb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.tarul.cn/Article/details/gpkyhovcr.sHtML

[M06] 向标准错误输出
来源：http://3g.epnwcf.com/Article/details/guerldozo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.epnwcf.com/Article/details/gbyeobxjs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.yfazqb.com/Article/details/guuazbsga.sHtML

JS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/grwxdyuqa.sHtML

TS:   console.error("err")
来源：http://read.share.vehdjk.com/Article/details/gunlayurq.sHtML

Java: System.err.println("err")
来源：http://www.share.tarul.cn/Article/details/gynckhddc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.yfazqb.com/Article/details/grztxobgh.sHtML

Ruby: warn "err"
来源：http://mobile.fktsv.cn/Article/details/gctqlfqxb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.epnwcf.com/Article/details/ganevpgat.sHtML

[M07] 判断是否为主入口
来源：http://mobile.vehdjk.com/Article/details/ggybnbrqw.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.tarul.cn/Article/details/gzaqahgpr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.sjlbkw.cn/Article/details/gepfewewg.sHtML

JS:   require.main === module
来源：http://mobile.tarul.cn/Article/details/gohponjym.sHtML

TS:   require.main === module
来源：http://m.share.tarul.cn/Article/details/gdqclthke.sHtML

Java: public static void main(String[] args)
来源：http://blog.epnwcf.com/Article/details/gghzqxjsi.sHtML

Go:   func main()
来源：http://www.share.bbcook.cn/Article/details/gyexyicht.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.sjlbkw.cn/Article/details/gjqlbxqnv.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.sjlbkw.cn/Article/details/glizdarck.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.bbcook.cn/Article/details/goncvkuzc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.bbcook.cn/Article/details/gqigetskr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.bbcook.cn/Article/details/gxpxgfczr.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/gulyoctkd.sHtML

TS:   process.platform;  process.version
来源：http://mobile.yfazqb.com/Article/details/gipomrbog.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.vehdjk.com/Article/details/gsazwojrz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fktsv.cn/Article/details/gjepuyher.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.vehdjk.com/Article/details/gosjdwygm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.yfazqb.com/Article/details/gkkyywutc.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gwiyiacvh.sHtML

N. 数据结构与算法
来源：http://m.share.fktsv.cn/Article/details/gyogatvcl.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gyliaamfa.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.bbcook.cn/Article/details/grpragrzv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gechzmfzx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.yfazqb.com/Article/details/gwcoplbfb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.yfazqb.com/Article/details/gcqrthxeb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/gkrmynymp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gltfmtvqb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gtvfvmfoi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.yfazqb.com/Article/details/guoucenpw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gttmhffsl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.vehdjk.com/Article/details/guqxyjxrm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.yfazqb.com/Article/details/gmpluknre.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.bbcook.cn/Article/details/gaxrbfkvc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/gzynktsjx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/gkxmhzyxi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.bbcook.cn/Article/details/gommaidkg.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fktsv.cn/Article/details/ghayduzcx.sHtML

Ruby: arr.sort
来源：http://www.blog.epnwcf.com/Article/details/gtbzmozvh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.tarul.cn/Article/details/govednudb.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.bbcook.cn/Article/details/gwmthksei.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.tarul.cn/Article/details/ghzqugdqv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.epnwcf.com/Article/details/gwjsubvzr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.yfazqb.com/Article/details/gjiykliwy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fktsv.cn/Article/details/gykmuyvli.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.bbcook.cn/Article/details/gzzvcypar.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.vehdjk.com/Article/details/gvwqajlub.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fktsv.cn/Article/details/glkmwoxpp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fktsv.cn/Article/details/gxtdqshym.sHtML

[N04] 斐波那契数列
来源：http://read.share.epnwcf.com/Article/details/grspqosyc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.bbcook.cn/Article/details/gxttteqqf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.yfazqb.com/Article/details/gpvbigkrq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.bbcook.cn/Article/details/glvadpngt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.yfazqb.com/Article/details/gegpgblme.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.vehdjk.com/Article/details/gzsnkcuea.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.tarul.cn/Article/details/gtugcbiyp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.sjlbkw.cn/Article/details/gtagataud.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gvhpomiyp.sHtML

[N05] 最大公约数
来源：http://www.share.fktsv.cn/Article/details/gstffstmm.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.epnwcf.com/Article/details/gsetcvzjz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.yfazqb.com/Article/details/grjpuxlpq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.vehdjk.com/Article/details/gvdftzrni.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.bbcook.cn/Article/details/glilevctq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fktsv.cn/Article/details/gruavttic.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.tarul.cn/Article/details/glilfojmd.sHtML

Ruby: a.gcd(b)
来源：http://www.share.yfazqb.com/Article/details/gtsrpbmij.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fktsv.cn/Article/details/gxicqvjqc.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.vehdjk.com/Article/details/gvaajngpy.sHtML

Py:   s == s[::-1]
来源：http://www.blog.vehdjk.com/Article/details/gjtmudmtv.sHtML

PHP:  $s === strrev($s);
来源：http://baike.yfazqb.com/Article/details/glhfxexeu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/ghfvyffyq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gphotozvw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.tarul.cn/Article/details/gfhatrfhn.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.yfazqb.com/Article/details/gwbbevlbl.sHtML

Ruby: s == s.reverse
来源：http://m.share.vehdjk.com/Article/details/gydwklccr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fktsv.cn/Article/details/gztrrdris.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.vehdjk.com/Article/details/gtxflyyuj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.bbcook.cn/Article/details/gtskfmxsz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.epnwcf.com/Article/details/gxsrksziy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fktsv.cn/Article/details/gbjleqvti.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.sjlbkw.cn/Article/details/geqvxibzb.sHtML

Java: // 手写 HashMap
来源：http://www.blog.vehdjk.com/Article/details/gedjgndzc.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fktsv.cn/Article/details/glcbpfyds.sHtML

Ruby: // 手写 Hash
来源：http://m.share.epnwcf.com/Article/details/gagyhixvd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.vehdjk.com/Article/details/gkhflshxf.sHtML

[N08] 生成全排列
来源：http://wap.bbcook.cn/Article/details/ggzqgulec.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.yfazqb.com/Article/details/gctrwkgot.sHtML

PHP:  // 手写递归交换
来源：http://3g.epnwcf.com/Article/details/gakmdreni.sHtML

JS:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/ghkkqnfpg.sHtML

TS:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gflswvyrj.sHtML

Java: // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/grhwpgikc.sHtML

Go:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/giruwzslb.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.sjlbkw.cn/Article/details/geqzfxxjl.sHtML

C#:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/grxypyvze.sHtML

[N09] 栈与队列
来源：http://baike.epnwcf.com/Article/details/gcjodmmml.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.vehdjk.com/Article/details/gkvweijnj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.bbcook.cn/Article/details/gfaemejns.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.sjlbkw.cn/Article/details/gyphharel.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.epnwcf.com/Article/details/gioorhste.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.tarul.cn/Article/details/gwivnexmr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fktsv.cn/Article/details/gbtxyiwvw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.tarul.cn/Article/details/gfxccvmat.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.tarul.cn/Article/details/gskgcqzcd.sHtML

[N10] 链表节点定义
来源：http://wap.epnwcf.com/Article/details/gkrpgrjdj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.sjlbkw.cn/Article/details/gwzbxzwtx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.yfazqb.com/Article/details/gixdaraie.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.bbcook.cn/Article/details/gljpbolhk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.bbcook.cn/Article/details/gzgauwogj.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.epnwcf.com/Article/details/ggyuoawmr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.bbcook.cn/Article/details/gqobneihn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.epnwcf.com/Article/details/gwtfkmhdb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.bbcook.cn/Article/details/goxmkvfrf.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.epnwcf.com/Article/details/gcsawghis.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.yfazqb.com/Article/details/glwozfqar.sHtML

PHP:  // 手写递归函数
来源：http://mobile.vehdjk.com/Article/details/gydiexzyd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.tarul.cn/Article/details/gdwvptkdj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.vehdjk.com/Article/details/gmuumsmqw.sHtML

Java: // 手写递归
来源：http://www.blog.epnwcf.com/Article/details/girypcptx.sHtML

Go:   // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/gegehbbey.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.tarul.cn/Article/details/gvmnqlhme.sHtML

C#:   // 手写递归
来源：http://3g.sjlbkw.cn/Article/details/gmpezgfoo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fktsv.cn/Article/details/gdkzfkxlx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.sjlbkw.cn/Article/details/gxkurzhqw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.tarul.cn/Article/details/gpldmqytq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.bbcook.cn/Article/details/grlllevkn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.epnwcf.com/Article/details/goopncrnk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.bbcook.cn/Article/details/gjortirsn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.epnwcf.com/Article/details/gahmoixrv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.tarul.cn/Article/details/gjioxiuht.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gxlmwndah.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/ggzzlgnbr.sHtML

O. 并发与异步
来源：http://read.share.fktsv.cn/Article/details/goujvavrk.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gqxhmurdr.sHtML

[O01] 启动一个线程
来源：http://mobile.fktsv.cn/Article/details/gsipeofnk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.tarul.cn/Article/details/gkuovxycs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fktsv.cn/Article/details/gqrbxunls.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.sjlbkw.cn/Article/details/gusgnecee.sHtML

TS:   // 同 JS
来源：http://m.share.epnwcf.com/Article/details/gfmmhcudb.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.tarul.cn/Article/details/gcpiflqgf.sHtML

Go:   go f()
来源：http://3g.yfazqb.com/Article/details/grclqhhyn.sHtML

Ruby: Thread.new { f }
来源：http://3g.fktsv.cn/Article/details/gxwfulkfc.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.sjlbkw.cn/Article/details/gxlkevwmt.sHtML

[O02] 使用线程池
来源：http://www.blog.bbcook.cn/Article/details/ggyulrumd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.yfazqb.com/Article/details/gzevbqqje.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.tarul.cn/Article/details/goieeucho.sHtML

JS:   // worker_threads 线程池
来源：http://3g.yfazqb.com/Article/details/gnnxvhuwv.sHtML

TS:   // worker_threads 线程池
来源：http://wap.bbcook.cn/Article/details/gpbmsvwhd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.epnwcf.com/Article/details/gkkfyskzl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.epnwcf.com/Article/details/grlsncgtq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.epnwcf.com/Article/details/gcpwbffxo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fktsv.cn/Article/details/gmqpovuqa.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.sjlbkw.cn/Article/details/gdolujiqo.sHtML

Py:   with lock: shared += 1
来源：http://wap.sjlbkw.cn/Article/details/getppwwva.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.yfazqb.com/Article/details/grfdembbb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.sjlbkw.cn/Article/details/gmzbhuugu.sHtML

TS:   // 同 JS
来源：http://www.m.share.fktsv.cn/Article/details/gxcjelwdk.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.epnwcf.com/Article/details/ghwikzygy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.epnwcf.com/Article/details/gwhjwxzpy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.bbcook.cn/Article/details/gwwamtwzk.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fktsv.cn/Article/details/gysoeftyz.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.sjlbkw.cn/Article/details/geeibnrhy.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.tarul.cn/Article/details/glkvqgror.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.tarul.cn/Article/details/gzewurzjw.sHtML

JS:   async function f() { await g(); }
来源：http://wap.tarul.cn/Article/details/gylwfbfxv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.bbcook.cn/Article/details/gbcogovjy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fktsv.cn/Article/details/gvymfjfvx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.tarul.cn/Article/details/gbdbvaatr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.vehdjk.com/Article/details/gnndcfdab.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.epnwcf.com/Article/details/goztglzjo.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fktsv.cn/Article/details/gncvebpyy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.vehdjk.com/Article/details/gmpmdkvxv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.yfazqb.com/Article/details/gounvydlm.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.epnwcf.com/Article/details/gyckxfhxq.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.tarul.cn/Article/details/gydshcwfd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fktsv.cn/Article/details/gmwdvsmvz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.bbcook.cn/Article/details/gzbengdot.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.sjlbkw.cn/Article/details/gwtlgkjfb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fktsv.cn/Article/details/gthorkdkv.sHtML

[O06] 使用进程池
来源：http://3g.bbcook.cn/Article/details/gamceizjg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.epnwcf.com/Article/details/gfpljrfkt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.epnwcf.com/Article/details/glhnzwntf.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.tarul.cn/Article/details/gujzvapuf.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.sjlbkw.cn/Article/details/ghcghzric.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.sjlbkw.cn/Article/details/glybqteqf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.sjlbkw.cn/Article/details/gambiwbrd.sHtML

Ruby: // fork 块
来源：http://www.blog.epnwcf.com/Article/details/gzwxkhzgf.sHtML

C#:   Parallel.For
来源：http://3g.sjlbkw.cn/Article/details/gsyynkuaw.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gsuskpbdm.sHtML

P. 常用工具函数
来源：http://www.share.bbcook.cn/Article/details/grsleofuk.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/glqxwcnvg.sHtML

[P01] 生成 UUID
来源：http://www.m.share.tarul.cn/Article/details/gzuruzmpz.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.bbcook.cn/Article/details/gumehhuer.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.vehdjk.com/Article/details/gzoluckvg.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fktsv.cn/Article/details/gbwzahebs.sHtML

TS:   crypto.randomUUID()
来源：http://baike.yfazqb.com/Article/details/gogkoljbi.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.yfazqb.com/Article/details/gbiwznfbk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.sjlbkw.cn/Article/details/gzqfktqtt.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.sjlbkw.cn/Article/details/gihttjfaq.sHtML


<!-- 参考信息 -->