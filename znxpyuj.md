代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.vehdjk.com/Article/details/gkzpyeuox.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fktsv.cn/Article/details/gygylbmda.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.bbcook.cn/Article/details/gdiaakkhu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.sjlbkw.cn/Article/details/gxkpasysp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.vehdjk.com/Article/details/gytygvybk.sHtML

[L04] 设置超时
来源：http://m.share.epnwcf.com/Article/details/gvalwqhrj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.yfazqb.com/Article/details/gkfwsxqzl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.bbcook.cn/Article/details/glstpsioc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.yfazqb.com/Article/details/gplqgnvrk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.bbcook.cn/Article/details/gjteoozcv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.bbcook.cn/Article/details/grpnieqrd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.bbcook.cn/Article/details/gemsbvipx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.sjlbkw.cn/Article/details/gasgikbdv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fktsv.cn/Article/details/grbjsmrzl.sHtML

[L05] 上传文件（multipart）
来源：http://wap.sjlbkw.cn/Article/details/gwvhvkpdk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.sjlbkw.cn/Article/details/gvzxpoajt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.tarul.cn/Article/details/gptlvvber.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.bbcook.cn/Article/details/gviejexcv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.tarul.cn/Article/details/gulctkfyl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.sjlbkw.cn/Article/details/gwashthtq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fktsv.cn/Article/details/gaolqkicy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.bbcook.cn/Article/details/gcpmlmlqr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gpjhygaiq.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.vehdjk.com/Article/details/gjbinzcjn.sHtML

Py:   resp.json()
来源：http://blog.yfazqb.com/Article/details/gwudcdkrz.sHtML

PHP:  json_decode($body, true);
来源：http://3g.vehdjk.com/Article/details/gifgomzqp.sHtML

JS:   await resp.json()
来源：http://read.share.yfazqb.com/Article/details/gkgjjxhqo.sHtML

TS:   await resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/gtdwnjdpa.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.yfazqb.com/Article/details/gafnnzbxz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.epnwcf.com/Article/details/gaszgxybd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvcrdlqv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.tarul.cn/Article/details/gbcsxyylt.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.yfazqb.com/Article/details/glherkpaq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.vehdjk.com/Article/details/gdlfgegbo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.epnwcf.com/Article/details/ggtvlzpul.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.tarul.cn/Article/details/gabdtxcgw.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.vehdjk.com/Article/details/ggmrooytj.sHtML

Java: resp.statusCode()
来源：http://www.m.share.sjlbkw.cn/Article/details/gikqtqxra.sHtML

Go:   resp.StatusCode
来源：http://3g.yfazqb.com/Article/details/gsfmdxvmv.sHtML

Ruby: resp.code.to_i
来源：http://www.share.yfazqb.com/Article/details/gprjrurms.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.sjlbkw.cn/Article/details/gmwonxllg.sHtML

[L08] 并发请求多个地址
来源：http://3g.epnwcf.com/Article/details/gbracrvzu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.tarul.cn/Article/details/ghttnonuz.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.yfazqb.com/Article/details/gnpwqskqf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.vehdjk.com/Article/details/gqjgyduym.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.tarul.cn/Article/details/gtkomsibh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.bbcook.cn/Article/details/gqajwvuhj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.epnwcf.com/Article/details/gfdopydnb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.vehdjk.com/Article/details/ggmqyzjjs.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gcoghcfrl.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gzlhlosjv.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.sjlbkw.cn/Article/details/gyjgxspgt.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gpffplvcu.sHtML

[M01] 读取命令行参数
来源：http://m.share.bbcook.cn/Article/details/geliuhdel.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.vehdjk.com/Article/details/gzofsodnj.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.sjlbkw.cn/Article/details/gugivwigl.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fktsv.cn/Article/details/glseotqvm.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.bbcook.cn/Article/details/ggfegxoqf.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.vehdjk.com/Article/details/gdhtefpbf.sHtML

Go:   os.Args[1:]
来源：http://baike.sjlbkw.cn/Article/details/giupkxcpo.sHtML

Ruby: ARGV
来源：http://www.share.bbcook.cn/Article/details/gwfvypblj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fktsv.cn/Article/details/gaciyejtw.sHtML

[M02] 读取环境变量
来源：http://m.share.vehdjk.com/Article/details/grrufsbwx.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.vehdjk.com/Article/details/gulpmjhmh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.bbcook.cn/Article/details/gygfrndeh.sHtML

JS:   process.env.HOME
来源：http://3g.tarul.cn/Article/details/gsbthegyy.sHtML

TS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/gfmhwlvjt.sHtML

Java: System.getenv("HOME")
来源：http://3g.vehdjk.com/Article/details/gckuxxupb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.sjlbkw.cn/Article/details/govilkukx.sHtML

Ruby: ENV["HOME"]
来源：http://baike.yfazqb.com/Article/details/gyywrooyl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.vehdjk.com/Article/details/gtmgxtukf.sHtML

[M03] 执行外部命令
来源：http://www.blog.epnwcf.com/Article/details/gdaqfrgov.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.vehdjk.com/Article/details/guvjlkqnx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.yfazqb.com/Article/details/gkyadtqzt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.epnwcf.com/Article/details/gtcteupyh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.yfazqb.com/Article/details/gvfxzjcsh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.tarul.cn/Article/details/gtzfubpor.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.tarul.cn/Article/details/gstjsatnz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.tarul.cn/Article/details/gvnfrsetw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.tarul.cn/Article/details/gzesjlcip.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.vehdjk.com/Article/details/gsewauojq.sHtML

Py:   os.getcwd()
来源：http://blog.sjlbkw.cn/Article/details/gjwbsucfs.sHtML

PHP:  getcwd();
来源：http://3g.vehdjk.com/Article/details/ginflfyhu.sHtML

JS:   process.cwd()
来源：http://m.share.yfazqb.com/Article/details/gtysnexre.sHtML

TS:   process.cwd()
来源：http://m.share.bbcook.cn/Article/details/giaggnckd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.bbcook.cn/Article/details/gjhghefri.sHtML

Go:   os.Getwd()
来源：http://baike.vehdjk.com/Article/details/gmmmpseeo.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.vehdjk.com/Article/details/gpxvigrag.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.yfazqb.com/Article/details/gukguqlwo.sHtML

[M05] 设置退出码
来源：http://www.m.share.sjlbkw.cn/Article/details/gdpgvksgz.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gqxrmafyo.sHtML

PHP:  exit(1);
来源：http://blog.fktsv.cn/Article/details/gzvisvauu.sHtML

JS:   process.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gchsxnjdy.sHtML

TS:   process.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gjrgdagif.sHtML

Java: System.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gsttrmiei.sHtML

Go:   os.Exit(1)
来源：http://wap.epnwcf.com/Article/details/glveirzhy.sHtML

Ruby: exit 1
来源：http://www.m.share.yfazqb.com/Article/details/grsapqwwn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.bbcook.cn/Article/details/gkglqphfo.sHtML

[M06] 向标准错误输出
来源：http://m.share.tarul.cn/Article/details/girvxjqht.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.vehdjk.com/Article/details/gznymdgqy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.tarul.cn/Article/details/guogpblag.sHtML

JS:   console.error("err")
来源：http://www.share.vehdjk.com/Article/details/gcwlskopm.sHtML

TS:   console.error("err")
来源：http://m.share.sjlbkw.cn/Article/details/gamespene.sHtML

Java: System.err.println("err")
来源：http://read.share.fktsv.cn/Article/details/gpqbnoiqw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.bbcook.cn/Article/details/gceqpwpan.sHtML

Ruby: warn "err"
来源：http://3g.sjlbkw.cn/Article/details/galhiitmd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.epnwcf.com/Article/details/gmqhtrxaf.sHtML

[M07] 判断是否为主入口
来源：http://www.share.yfazqb.com/Article/details/gwxfekygs.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.epnwcf.com/Article/details/ghhwiyubo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.bbcook.cn/Article/details/gkvllkqrj.sHtML

JS:   require.main === module
来源：http://3g.yfazqb.com/Article/details/gnqnuljqc.sHtML

TS:   require.main === module
来源：http://mobile.vehdjk.com/Article/details/gkzmpqfeg.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.vehdjk.com/Article/details/gvwbruamc.sHtML

Go:   func main()
来源：http://read.share.fktsv.cn/Article/details/gppngzirx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.yfazqb.com/Article/details/glqplcvuu.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.vehdjk.com/Article/details/gtodxnyod.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.tarul.cn/Article/details/gfrbqsiox.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.vehdjk.com/Article/details/guhminntq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.epnwcf.com/Article/details/gjdurvjuh.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.epnwcf.com/Article/details/gcpvwbuuf.sHtML

TS:   process.platform;  process.version
来源：http://baike.sjlbkw.cn/Article/details/gqifhyelt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.epnwcf.com/Article/details/gktnbtavm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fktsv.cn/Article/details/gtxdsuvov.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.epnwcf.com/Article/details/gxqivgydu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.epnwcf.com/Article/details/gzrykhhzc.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gvarskjuj.sHtML

N. 数据结构与算法
来源：http://3g.vehdjk.com/Article/details/gtamxcxdj.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/guvrzrthx.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fktsv.cn/Article/details/ghmdmuspm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.tarul.cn/Article/details/gxvkgdfdg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gydvhivuq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.yfazqb.com/Article/details/genzgxafl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.epnwcf.com/Article/details/ggplqvwqd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gytfbipml.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gdfjqrzef.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.vehdjk.com/Article/details/gzbzacbjj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gwtbfloln.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.vehdjk.com/Article/details/gkbdpckqs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.bbcook.cn/Article/details/goqzoebmg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.tarul.cn/Article/details/gqphljexf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.sjlbkw.cn/Article/details/gmvlabsvg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.vehdjk.com/Article/details/gxnnxdmih.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.tarul.cn/Article/details/gouafjjsp.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.yfazqb.com/Article/details/gwpqmdjxx.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/grlmnfzjt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.bbcook.cn/Article/details/gmyeqqdxu.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.epnwcf.com/Article/details/gfzfsefox.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fktsv.cn/Article/details/grxzjznqn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.bbcook.cn/Article/details/gyfwchrnm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.yfazqb.com/Article/details/gvinmmhsx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.sjlbkw.cn/Article/details/gkwnyntqe.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.sjlbkw.cn/Article/details/gaabqmjru.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.tarul.cn/Article/details/giyxpnhck.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.tarul.cn/Article/details/ggyfxkqgq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.yfazqb.com/Article/details/gaywpdwaw.sHtML

[N04] 斐波那契数列
来源：http://wap.sjlbkw.cn/Article/details/gdjtwkuud.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.vehdjk.com/Article/details/gcidfguuq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.epnwcf.com/Article/details/gxnfhwnqo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.tarul.cn/Article/details/gvccpfyey.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/gjhgulvqr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.epnwcf.com/Article/details/gqxnnqzia.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.bbcook.cn/Article/details/gxfveliey.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fktsv.cn/Article/details/gxugbihzv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/gihbchqal.sHtML

[N05] 最大公约数
来源：http://www.m.share.sjlbkw.cn/Article/details/gevxohhcq.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.yfazqb.com/Article/details/gyylxynkn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fktsv.cn/Article/details/gdjagncvb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.tarul.cn/Article/details/gefjmegxy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.epnwcf.com/Article/details/geoeqliyt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.bbcook.cn/Article/details/gqhljfjpm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.bbcook.cn/Article/details/ggtropgnb.sHtML

Ruby: a.gcd(b)
来源：http://blog.fktsv.cn/Article/details/gvqwqpmxo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.sjlbkw.cn/Article/details/gcvcmgfkh.sHtML

[N06] 判断回文字符串
来源：http://read.share.vehdjk.com/Article/details/glqwxywvr.sHtML

Py:   s == s[::-1]
来源：http://mobile.tarul.cn/Article/details/gimvqjvee.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.yfazqb.com/Article/details/gihsbewia.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/gdqkiuqka.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gikxmiasg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.tarul.cn/Article/details/gevgcggqj.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.sjlbkw.cn/Article/details/gyygyhqab.sHtML

Ruby: s == s.reverse
来源：http://www.share.yfazqb.com/Article/details/gupcnihug.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.sjlbkw.cn/Article/details/gwnhwvpbm.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.vehdjk.com/Article/details/gdfjxmxue.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.yfazqb.com/Article/details/gdtiszjch.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.epnwcf.com/Article/details/gixdjgpup.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.sjlbkw.cn/Article/details/gixiodqiq.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.sjlbkw.cn/Article/details/gbsqgopxq.sHtML

Java: // 手写 HashMap
来源：http://wap.epnwcf.com/Article/details/gwqjfilfk.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.yfazqb.com/Article/details/gfkcdlptc.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.bbcook.cn/Article/details/gsebencpg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.tarul.cn/Article/details/gxovtdatr.sHtML

[N08] 生成全排列
来源：http://baike.fktsv.cn/Article/details/gbpfmlgot.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gihhtwhej.sHtML

PHP:  // 手写递归交换
来源：http://read.share.epnwcf.com/Article/details/gcqrlcfec.sHtML

JS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/ggxuqmonu.sHtML

TS:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gnphjasie.sHtML

Java: // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gbsyluyeb.sHtML

Go:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/glrqiywws.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.bbcook.cn/Article/details/gfvolnwce.sHtML

C#:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/goinqhhjg.sHtML

[N09] 栈与队列
来源：http://baike.sjlbkw.cn/Article/details/gszlqargo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.yfazqb.com/Article/details/gexxdncai.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.sjlbkw.cn/Article/details/gcrbkzabq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.epnwcf.com/Article/details/gpkxdnjtl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.bbcook.cn/Article/details/gphpivmfg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.bbcook.cn/Article/details/gzruoqtan.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.tarul.cn/Article/details/gwscqlqnx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.yfazqb.com/Article/details/ghcthtfnu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.tarul.cn/Article/details/gmvmulkav.sHtML

[N10] 链表节点定义
来源：http://www.m.share.bbcook.cn/Article/details/gijeoacoa.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.yfazqb.com/Article/details/gvinclwxt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.epnwcf.com/Article/details/gjqzreflt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.sjlbkw.cn/Article/details/ggkdvpsvg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.vehdjk.com/Article/details/gqfwswbwr.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.bbcook.cn/Article/details/ggxmqximy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmogjviom.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.tarul.cn/Article/details/gfioyzgih.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.yfazqb.com/Article/details/gtnpfnctz.sHtML

[N11] 二叉树中序遍历
来源：http://wap.bbcook.cn/Article/details/gaxyofhdx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.tarul.cn/Article/details/geqjgdnrn.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.bbcook.cn/Article/details/gaocykbgl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.yfazqb.com/Article/details/gcwwnzvng.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.vehdjk.com/Article/details/gocncfvqr.sHtML

Java: // 手写递归
来源：http://baike.yfazqb.com/Article/details/gomgrobtj.sHtML

Go:   // 手写递归
来源：http://read.share.epnwcf.com/Article/details/gfnrellqs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.yfazqb.com/Article/details/gmjfqldjb.sHtML

C#:   // 手写递归
来源：http://read.share.bbcook.cn/Article/details/ggdbndwqf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.epnwcf.com/Article/details/gdxootahv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.yfazqb.com/Article/details/gdrkxshxz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fktsv.cn/Article/details/ginlqzmvb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.vehdjk.com/Article/details/gilcfdkzh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fktsv.cn/Article/details/ghvbhnkys.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.tarul.cn/Article/details/goswdqvzf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.vehdjk.com/Article/details/gvhurmpfl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fktsv.cn/Article/details/gwdqkhnkq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fktsv.cn/Article/details/grvmdapbk.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gqcncwkyk.sHtML

O. 并发与异步
来源：http://www.m.share.vehdjk.com/Article/details/gijmkhqil.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gglheoaoc.sHtML

[O01] 启动一个线程
来源：http://3g.sjlbkw.cn/Article/details/gcbaglqyv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.bbcook.cn/Article/details/gqqmcpuew.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.tarul.cn/Article/details/gzksqwecg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.vehdjk.com/Article/details/gpqppkuba.sHtML

TS:   // 同 JS
来源：http://blog.epnwcf.com/Article/details/gxdqfugsv.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.vehdjk.com/Article/details/gbnsmstzf.sHtML

Go:   go f()
来源：http://baike.vehdjk.com/Article/details/gcntarmsk.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.yfazqb.com/Article/details/gbzmwiatu.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.yfazqb.com/Article/details/gnscvfike.sHtML

[O02] 使用线程池
来源：http://mobile.sjlbkw.cn/Article/details/gsdacxzat.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.sjlbkw.cn/Article/details/gjakqlzhv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.vehdjk.com/Article/details/gpisdtlhj.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.bbcook.cn/Article/details/glluqwfsg.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.vehdjk.com/Article/details/gxuwiuiyn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.yfazqb.com/Article/details/gnzptlytt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.epnwcf.com/Article/details/gffxzlgcu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fktsv.cn/Article/details/gmzqxgrhr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.tarul.cn/Article/details/gnutwrxab.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.yfazqb.com/Article/details/gcszmkfty.sHtML

Py:   with lock: shared += 1
来源：http://3g.bbcook.cn/Article/details/gnqkvepgl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.bbcook.cn/Article/details/gesmpwzhb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fktsv.cn/Article/details/glqucxlyl.sHtML

TS:   // 同 JS
来源：http://wap.sjlbkw.cn/Article/details/gisftvslo.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fktsv.cn/Article/details/gztgwqozg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.bbcook.cn/Article/details/grbmvewtr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.epnwcf.com/Article/details/gicmdzwey.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.yfazqb.com/Article/details/goxdovamv.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.vehdjk.com/Article/details/gssjhsvnh.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.sjlbkw.cn/Article/details/gjgmaezhq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.yfazqb.com/Article/details/gvkojocnk.sHtML

JS:   async function f() { await g(); }
来源：http://wap.epnwcf.com/Article/details/gwytqeysa.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fktsv.cn/Article/details/gtgmiyufv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.bbcook.cn/Article/details/gonylzvdc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.vehdjk.com/Article/details/ggemblmdo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.vehdjk.com/Article/details/gmvqbznlx.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fktsv.cn/Article/details/gshtwugdt.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.bbcook.cn/Article/details/gbyaxuvaw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.vehdjk.com/Article/details/ggluagpgc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.vehdjk.com/Article/details/gdcbqcygm.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/gjpeoston.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.vehdjk.com/Article/details/gaaoogxvi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.sjlbkw.cn/Article/details/girympywv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.sjlbkw.cn/Article/details/gjntslnwk.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fktsv.cn/Article/details/gcpgvebxi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.tarul.cn/Article/details/gxvpkanuy.sHtML

[O06] 使用进程池
来源：http://m.share.yfazqb.com/Article/details/glmcoepcy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.yfazqb.com/Article/details/ggriaqsmm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.yfazqb.com/Article/details/gioktjnvb.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.tarul.cn/Article/details/ggtclvyjk.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.bbcook.cn/Article/details/gvpsucugf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.vehdjk.com/Article/details/gjqdfdfvw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.sjlbkw.cn/Article/details/gkzijhgps.sHtML

Ruby: // fork 块
来源：http://baike.sjlbkw.cn/Article/details/ggngfhdby.sHtML

C#:   Parallel.For
来源：http://www.m.share.sjlbkw.cn/Article/details/gumuawmmz.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/ghktjwrme.sHtML

P. 常用工具函数
来源：http://blog.tarul.cn/Article/details/gzxcuphcz.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gmgtrazbe.sHtML

[P01] 生成 UUID
来源：http://baike.bbcook.cn/Article/details/gkhjwxvzm.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.bbcook.cn/Article/details/gthvndhnh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.epnwcf.com/Article/details/ghlukstkk.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/gsczlpoai.sHtML


<!-- 参考信息 -->