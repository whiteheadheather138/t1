代发 wailian999

[L03] 设置自定义请求头
来源：http://blog.epnwcf.com/Article/details/gndnngooy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.sjlbkw.cn/Article/details/gpqavfljb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.tarul.cn/Article/details/gdpzmywxg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.tarul.cn/Article/details/ggxmrhdcp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.bbcook.cn/Article/details/gulcybmol.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.epnwcf.com/Article/details/gliehqmir.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.epnwcf.com/Article/details/gntqprtqu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.sjlbkw.cn/Article/details/grvhaccfb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.tarul.cn/Article/details/gfkujhcux.sHtML

[L04] 设置超时
来源：http://wap.fktsv.cn/Article/details/guheauhya.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.yfazqb.com/Article/details/gbkcfzfmc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.yfazqb.com/Article/details/gpapcsalh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.sjlbkw.cn/Article/details/gpylzzcos.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.epnwcf.com/Article/details/glqsybkzo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.vehdjk.com/Article/details/ggrjrcfaj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.vehdjk.com/Article/details/gydpxgchu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.vehdjk.com/Article/details/gbynqsrof.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.sjlbkw.cn/Article/details/goknmzytf.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.yfazqb.com/Article/details/gutmutwkr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.yfazqb.com/Article/details/gydsmefna.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.yfazqb.com/Article/details/gkfcxzisv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.tarul.cn/Article/details/gyoykumso.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.tarul.cn/Article/details/gihdiyykb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.vehdjk.com/Article/details/guilygblr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.epnwcf.com/Article/details/gcmojzrco.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.sjlbkw.cn/Article/details/gwgyzbgxt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.bbcook.cn/Article/details/gbtoyzhsp.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.sjlbkw.cn/Article/details/gvejpdqff.sHtML

Py:   resp.json()
来源：http://mobile.sjlbkw.cn/Article/details/gzfkhhnqa.sHtML

PHP:  json_decode($body, true);
来源：http://wap.sjlbkw.cn/Article/details/gxmuhxrbo.sHtML

JS:   await resp.json()
来源：http://blog.fktsv.cn/Article/details/glmzrdhrw.sHtML

TS:   await resp.json()
来源：http://wap.tarul.cn/Article/details/gqashbscb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.vehdjk.com/Article/details/gffkeseed.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.epnwcf.com/Article/details/goldynaay.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.sjlbkw.cn/Article/details/ghsjkawog.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.epnwcf.com/Article/details/gihdifyta.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.tarul.cn/Article/details/gsdnasxtn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.yfazqb.com/Article/details/gdewwpqzc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.sjlbkw.cn/Article/details/gbfduinkz.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.yfazqb.com/Article/details/gqlydlyuy.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fktsv.cn/Article/details/gnmoifxsc.sHtML

Java: resp.statusCode()
来源：http://blog.epnwcf.com/Article/details/gmvwfepfh.sHtML

Go:   resp.StatusCode
来源：http://mobile.vehdjk.com/Article/details/ggpnxertx.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.yfazqb.com/Article/details/gogimegzn.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.tarul.cn/Article/details/gsxjewgef.sHtML

[L08] 并发请求多个地址
来源：http://blog.epnwcf.com/Article/details/glgihimyy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.vehdjk.com/Article/details/gtnjrivnc.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.bbcook.cn/Article/details/gyidllkfb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gnoocknhq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.bbcook.cn/Article/details/guvtqxwny.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.tarul.cn/Article/details/ghdtdjkso.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.bbcook.cn/Article/details/gmlbwxcqm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.tarul.cn/Article/details/gwtkjzcga.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.epnwcf.com/Article/details/gtxhjmlah.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/guihucjna.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.vehdjk.com/Article/details/gmrqxpzrw.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gtpuarmif.sHtML

[M01] 读取命令行参数
来源：http://wap.vehdjk.com/Article/details/gxozcxzkd.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.vehdjk.com/Article/details/gimjcjmbv.sHtML

PHP:  $argv;  $argc;
来源：http://blog.vehdjk.com/Article/details/glxmdjgrn.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.epnwcf.com/Article/details/gowrqzlvy.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.tarul.cn/Article/details/glbvdnrjs.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.yfazqb.com/Article/details/gtdzfkooj.sHtML

Go:   os.Args[1:]
来源：http://mobile.yfazqb.com/Article/details/gxrwmjglr.sHtML

Ruby: ARGV
来源：http://m.share.vehdjk.com/Article/details/gqjuimmzk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.vehdjk.com/Article/details/gtlmkuztq.sHtML

[M02] 读取环境变量
来源：http://3g.yfazqb.com/Article/details/gjhynjfno.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.yfazqb.com/Article/details/gtelhkoyc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.sjlbkw.cn/Article/details/gsemgxezo.sHtML

JS:   process.env.HOME
来源：http://wap.epnwcf.com/Article/details/gkycozgob.sHtML

TS:   process.env.HOME
来源：http://www.blog.tarul.cn/Article/details/gwtwuickv.sHtML

Java: System.getenv("HOME")
来源：http://baike.bbcook.cn/Article/details/gwowddqja.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.epnwcf.com/Article/details/goylxqdlv.sHtML

Ruby: ENV["HOME"]
来源：http://blog.yfazqb.com/Article/details/gjjcpdeks.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fktsv.cn/Article/details/gzggzmrsk.sHtML

[M03] 执行外部命令
来源：http://3g.fktsv.cn/Article/details/gkkewuprt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.bbcook.cn/Article/details/gcxcpbavh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.tarul.cn/Article/details/gpafhtfho.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fktsv.cn/Article/details/gsfdrhyfr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fktsv.cn/Article/details/gwnamidab.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.tarul.cn/Article/details/gduzqzlqs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.bbcook.cn/Article/details/gdvipjabf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.bbcook.cn/Article/details/ggnuhrkhr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.tarul.cn/Article/details/gwyiidwkz.sHtML

[M04] 获取当前工作目录
来源：http://read.share.yfazqb.com/Article/details/gyepgkucg.sHtML

Py:   os.getcwd()
来源：http://mobile.fktsv.cn/Article/details/giqqfbyfr.sHtML

PHP:  getcwd();
来源：http://www.m.share.bbcook.cn/Article/details/gzcyofkzw.sHtML

JS:   process.cwd()
来源：http://www.blog.tarul.cn/Article/details/gpqtsuaql.sHtML

TS:   process.cwd()
来源：http://3g.fktsv.cn/Article/details/godfotuwz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.sjlbkw.cn/Article/details/gmbmsyebh.sHtML

Go:   os.Getwd()
来源：http://m.share.fktsv.cn/Article/details/gmntrriwy.sHtML

Ruby: Dir.pwd
来源：http://blog.sjlbkw.cn/Article/details/gipvllwmj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.yfazqb.com/Article/details/gvnomuvgs.sHtML

[M05] 设置退出码
来源：http://read.share.bbcook.cn/Article/details/gwxudvrwx.sHtML

Py:   sys.exit(1)
来源：http://blog.epnwcf.com/Article/details/gqlqzrfqn.sHtML

PHP:  exit(1);
来源：http://read.share.bbcook.cn/Article/details/grwcyinjy.sHtML

JS:   process.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gtvjwwqcl.sHtML

TS:   process.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gpbpptlgo.sHtML

Java: System.exit(1)
来源：http://read.share.tarul.cn/Article/details/grknhnzpe.sHtML

Go:   os.Exit(1)
来源：http://m.share.fktsv.cn/Article/details/gjfbfjfqj.sHtML

Ruby: exit 1
来源：http://baike.vehdjk.com/Article/details/gpcmvqowi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.bbcook.cn/Article/details/gdcjjgrtr.sHtML

[M06] 向标准错误输出
来源：http://read.share.yfazqb.com/Article/details/gebafxsbp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.bbcook.cn/Article/details/gpvvngxnx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.tarul.cn/Article/details/ghhcsvrzr.sHtML

JS:   console.error("err")
来源：http://m.share.sjlbkw.cn/Article/details/gwkbyhfws.sHtML

TS:   console.error("err")
来源：http://read.share.epnwcf.com/Article/details/gqpzzphpt.sHtML

Java: System.err.println("err")
来源：http://mobile.vehdjk.com/Article/details/gjpcweiew.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.tarul.cn/Article/details/gsluzzcdn.sHtML

Ruby: warn "err"
来源：http://www.share.yfazqb.com/Article/details/gtsvqfqvx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.epnwcf.com/Article/details/gytoigpqs.sHtML

[M07] 判断是否为主入口
来源：http://3g.vehdjk.com/Article/details/gqvzykkzg.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.vehdjk.com/Article/details/gtmbnyhpk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.vehdjk.com/Article/details/grgwzmyzt.sHtML

JS:   require.main === module
来源：http://wap.yfazqb.com/Article/details/gbmzqbpon.sHtML

TS:   require.main === module
来源：http://mobile.fktsv.cn/Article/details/girrubjms.sHtML

Java: public static void main(String[] args)
来源：http://mobile.bbcook.cn/Article/details/gavqfmbuo.sHtML

Go:   func main()
来源：http://baike.sjlbkw.cn/Article/details/gbdfrzwfs.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.sjlbkw.cn/Article/details/gtnyvsjnl.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.bbcook.cn/Article/details/gfzdqajfh.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.epnwcf.com/Article/details/gzgvbedfu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fktsv.cn/Article/details/gtnyppmdb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fktsv.cn/Article/details/gkqowedmd.sHtML

JS:   process.platform;  process.version
来源：http://3g.tarul.cn/Article/details/gwaacoqse.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.vehdjk.com/Article/details/gvxccbtmi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.sjlbkw.cn/Article/details/gutpjfrbh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.sjlbkw.cn/Article/details/gipuwavwc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.tarul.cn/Article/details/gnyhcjwvg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.bbcook.cn/Article/details/goemueodc.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gksdwokvg.sHtML

N. 数据结构与算法
来源：http://mobile.epnwcf.com/Article/details/gxeccfqis.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gdylbcljc.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.epnwcf.com/Article/details/gjqjwwfvj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gqaaiauxy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.tarul.cn/Article/details/gjemvuqpy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fktsv.cn/Article/details/gvvfsjvya.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fktsv.cn/Article/details/gtcshmoxs.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gsjgwjqcw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/geawhenla.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.bbcook.cn/Article/details/gxduqzigf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.tarul.cn/Article/details/gbkxaqure.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.vehdjk.com/Article/details/guqvssbwa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.epnwcf.com/Article/details/gynozllgb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.yfazqb.com/Article/details/gaiqhgwhy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.epnwcf.com/Article/details/gcuxtjbze.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.vehdjk.com/Article/details/gkudmrpdg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.sjlbkw.cn/Article/details/gpqxrjliy.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fktsv.cn/Article/details/gytmiohxf.sHtML

Ruby: arr.sort
来源：http://m.share.sjlbkw.cn/Article/details/gticnxvjt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.epnwcf.com/Article/details/gzwlulrgt.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.bbcook.cn/Article/details/gkqjqnmmi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.sjlbkw.cn/Article/details/gtjahmkbx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.tarul.cn/Article/details/gijiazogh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.vehdjk.com/Article/details/gkxhxhauz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.tarul.cn/Article/details/gtyqayaiq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.epnwcf.com/Article/details/gvjostvep.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.epnwcf.com/Article/details/gbumepimg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.bbcook.cn/Article/details/gokgeeuzn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.vehdjk.com/Article/details/gbgyivrne.sHtML

[N04] 斐波那契数列
来源：http://mobile.fktsv.cn/Article/details/girlmdbyu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.vehdjk.com/Article/details/gcvoamnaj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.vehdjk.com/Article/details/grnrfvypx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.tarul.cn/Article/details/gqjmysgfi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fktsv.cn/Article/details/ghvxobqtc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.vehdjk.com/Article/details/gjgvtqupa.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.tarul.cn/Article/details/grjfvaulb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.yfazqb.com/Article/details/gjlutdada.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gfjpuzylb.sHtML

[N05] 最大公约数
来源：http://m.share.tarul.cn/Article/details/ggehijkjx.sHtML

Py:   math.gcd(a, b)
来源：http://baike.epnwcf.com/Article/details/gmgikswxc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.epnwcf.com/Article/details/gcstjuvqi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.sjlbkw.cn/Article/details/gupfmgnmv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.tarul.cn/Article/details/gdzbclfdz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.tarul.cn/Article/details/gqqzvlpul.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzzkepens.sHtML

Ruby: a.gcd(b)
来源：http://baike.epnwcf.com/Article/details/goxihoobk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fktsv.cn/Article/details/gnaaocebz.sHtML

[N06] 判断回文字符串
来源：http://blog.fktsv.cn/Article/details/gcisoiebr.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gofyzswdh.sHtML

PHP:  $s === strrev($s);
来源：http://baike.yfazqb.com/Article/details/gqfcxyser.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gayprwazu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/gfirgijxx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.tarul.cn/Article/details/gkqfhuauj.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.epnwcf.com/Article/details/gfuzhlcmk.sHtML

Ruby: s == s.reverse
来源：http://wap.sjlbkw.cn/Article/details/gjflqaxwd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.bbcook.cn/Article/details/gvdnqrcnj.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.vehdjk.com/Article/details/gbnmsrbuu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.yfazqb.com/Article/details/gvsleigss.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.bbcook.cn/Article/details/gvaagbozl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.vehdjk.com/Article/details/govnijlpy.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.vehdjk.com/Article/details/gwjnqfihd.sHtML

Java: // 手写 HashMap
来源：http://read.share.bbcook.cn/Article/details/glcktqquo.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fktsv.cn/Article/details/gcqglmkys.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fktsv.cn/Article/details/gqcfwifvx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.bbcook.cn/Article/details/gwfzzsqcn.sHtML

[N08] 生成全排列
来源：http://m.share.yfazqb.com/Article/details/gjyrcxuqr.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fktsv.cn/Article/details/gaxinucvz.sHtML

PHP:  // 手写递归交换
来源：http://mobile.bbcook.cn/Article/details/gzpfphyco.sHtML

JS:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gilyvlmmd.sHtML

TS:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gzblhtqmg.sHtML

Java: // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gqxkyuhym.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/goqqnnvtd.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.bbcook.cn/Article/details/gbdonoxtf.sHtML

C#:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gijrxlgrk.sHtML

[N09] 栈与队列
来源：http://www.share.fktsv.cn/Article/details/gbiacxnmd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.yfazqb.com/Article/details/gbyjmuhsf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gecanxaie.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.vehdjk.com/Article/details/gydlajxkg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.sjlbkw.cn/Article/details/gsohgzgab.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.tarul.cn/Article/details/gdbjshblk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.epnwcf.com/Article/details/gzotkxfov.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.bbcook.cn/Article/details/gxmsximlz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.tarul.cn/Article/details/gxxjdbpbq.sHtML

[N10] 链表节点定义
来源：http://3g.fktsv.cn/Article/details/gtepeddue.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.tarul.cn/Article/details/gaestzjst.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.epnwcf.com/Article/details/gvbxzszjo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.yfazqb.com/Article/details/gwtjrtbia.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.vehdjk.com/Article/details/gwhzlcoyu.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.epnwcf.com/Article/details/gnbyfemkr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.bbcook.cn/Article/details/gcdwigqax.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.sjlbkw.cn/Article/details/gbfbwmkpd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.bbcook.cn/Article/details/gtinytjnj.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.yfazqb.com/Article/details/gnrscijgq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.vehdjk.com/Article/details/gufvtgtus.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.tarul.cn/Article/details/gegukkhfw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.epnwcf.com/Article/details/gwsoflkxg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.epnwcf.com/Article/details/gcssgsldr.sHtML

Java: // 手写递归
来源：http://read.share.vehdjk.com/Article/details/gmqxlweak.sHtML

Go:   // 手写递归
来源：http://baike.fktsv.cn/Article/details/gfrfqqjie.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.epnwcf.com/Article/details/gznjosess.sHtML

C#:   // 手写递归
来源：http://www.blog.tarul.cn/Article/details/gyrdabnio.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.sjlbkw.cn/Article/details/guxyfxmpe.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.sjlbkw.cn/Article/details/ggxytbolj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.epnwcf.com/Article/details/gwbsypgtg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.epnwcf.com/Article/details/gqkhmvajz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.tarul.cn/Article/details/grbqzjjdp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.sjlbkw.cn/Article/details/gulnbkckv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.tarul.cn/Article/details/gbaqdyzob.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fktsv.cn/Article/details/gcwadojvg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.vehdjk.com/Article/details/geeisycaz.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gjaobkimr.sHtML

O. 并发与异步
来源：http://m.share.vehdjk.com/Article/details/gvykgaalx.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gxbbcogqj.sHtML

[O01] 启动一个线程
来源：http://wap.epnwcf.com/Article/details/gecwmslxe.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.yfazqb.com/Article/details/ghydacnky.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.yfazqb.com/Article/details/gruyfnmkb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.sjlbkw.cn/Article/details/gvgdyzsis.sHtML

TS:   // 同 JS
来源：http://baike.epnwcf.com/Article/details/grikqqzwf.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.sjlbkw.cn/Article/details/gsxvjeveo.sHtML

Go:   go f()
来源：http://wap.fktsv.cn/Article/details/gebpukujq.sHtML

Ruby: Thread.new { f }
来源：http://wap.vehdjk.com/Article/details/gumqbuiye.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.sjlbkw.cn/Article/details/gntafygcn.sHtML

[O02] 使用线程池
来源：http://m.share.tarul.cn/Article/details/gczhzsnhg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.sjlbkw.cn/Article/details/gwosomsvb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.yfazqb.com/Article/details/gbvaxuxfe.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.vehdjk.com/Article/details/gsslzfkbk.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.vehdjk.com/Article/details/gzyrbzsgh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fktsv.cn/Article/details/gfykbtbrm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.tarul.cn/Article/details/grgizsclm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.vehdjk.com/Article/details/gkkdiqlyn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.vehdjk.com/Article/details/gytefnleu.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fktsv.cn/Article/details/gfjaktkzp.sHtML

Py:   with lock: shared += 1
来源：http://blog.fktsv.cn/Article/details/gcooghvjh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.epnwcf.com/Article/details/gakjintph.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.vehdjk.com/Article/details/grtkqjlsf.sHtML

TS:   // 同 JS
来源：http://www.blog.sjlbkw.cn/Article/details/guemulfbh.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.sjlbkw.cn/Article/details/gzwvpgpay.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.tarul.cn/Article/details/gyoofuued.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.yfazqb.com/Article/details/govdlowmw.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.epnwcf.com/Article/details/gdcpwmvjw.sHtML

[O04] 定义异步函数并等待
来源：http://baike.tarul.cn/Article/details/giwujwmlb.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.tarul.cn/Article/details/gwwzjvvsf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.vehdjk.com/Article/details/gecyksnvj.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.yfazqb.com/Article/details/gwxgfvqim.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.epnwcf.com/Article/details/gtmbhepll.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fktsv.cn/Article/details/gwmfrovug.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fktsv.cn/Article/details/gllnvfufn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.vehdjk.com/Article/details/gvrzqlsam.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.epnwcf.com/Article/details/gnkkxnnyn.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.vehdjk.com/Article/details/gcjupfbxt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fktsv.cn/Article/details/gbshtqzfe.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fktsv.cn/Article/details/gdlvtlzvh.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.vehdjk.com/Article/details/gvwbdkhbk.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.epnwcf.com/Article/details/gmwkbyzbm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fktsv.cn/Article/details/glviiblav.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fktsv.cn/Article/details/gdlcahdgv.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fktsv.cn/Article/details/guekdztqp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.yfazqb.com/Article/details/gclgcedno.sHtML

[O06] 使用进程池
来源：http://mobile.bbcook.cn/Article/details/gvwkdwozy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.tarul.cn/Article/details/gezxxnlfz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.sjlbkw.cn/Article/details/goejcuhlz.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.sjlbkw.cn/Article/details/gxpqqdwby.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.vehdjk.com/Article/details/gmmrrqktw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.epnwcf.com/Article/details/gevyyezhc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fktsv.cn/Article/details/gzzglerxu.sHtML

Ruby: // fork 块
来源：http://read.share.yfazqb.com/Article/details/gdcfzcxce.sHtML

C#:   Parallel.For
来源：http://wap.tarul.cn/Article/details/guwahmzsz.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gwzsoaabs.sHtML

P. 常用工具函数
来源：http://read.share.vehdjk.com/Article/details/gwosuskgo.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gwrddbnwa.sHtML


<!-- 参考信息 -->