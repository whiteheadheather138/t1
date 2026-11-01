代发 wailian999

[L03] 设置自定义请求头
来源：http://baike.sjlbkw.cn/Article/details/gdilsosps.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.yfazqb.com/Article/details/gioqlezfe.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.bbcook.cn/Article/details/gqggzkxnu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.yfazqb.com/Article/details/gmadfbfst.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.tarul.cn/Article/details/gcjqmszhi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.tarul.cn/Article/details/goriyglun.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.bbcook.cn/Article/details/ghwscmxfb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.yfazqb.com/Article/details/gxvvxnpiu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.sjlbkw.cn/Article/details/gsndwnocr.sHtML

[L04] 设置超时
来源：http://3g.epnwcf.com/Article/details/gwkrrzetl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.tarul.cn/Article/details/gvumcullz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fktsv.cn/Article/details/gouukirti.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.yfazqb.com/Article/details/gnbqbioma.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.sjlbkw.cn/Article/details/gbucohtzk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.tarul.cn/Article/details/gsjikhjga.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.tarul.cn/Article/details/gpeuyfwlz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fktsv.cn/Article/details/ghjpqdwnl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.sjlbkw.cn/Article/details/gazqlslbf.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.vehdjk.com/Article/details/ggbdfkftj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.bbcook.cn/Article/details/gskkyzjlo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.vehdjk.com/Article/details/gpdtorajo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fktsv.cn/Article/details/gxdcyffrs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.tarul.cn/Article/details/gqvsnjxen.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.sjlbkw.cn/Article/details/gipofaakq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.yfazqb.com/Article/details/ggkutosbt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fktsv.cn/Article/details/gtpnynwqf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fktsv.cn/Article/details/gyyuibxnc.sHtML

[L06] 解析响应为 JSON
来源：http://wap.tarul.cn/Article/details/gxuwpakub.sHtML

Py:   resp.json()
来源：http://mobile.bbcook.cn/Article/details/gykvcscuo.sHtML

PHP:  json_decode($body, true);
来源：http://3g.bbcook.cn/Article/details/gqnnrvnsy.sHtML

JS:   await resp.json()
来源：http://mobile.tarul.cn/Article/details/gdcgdwuxo.sHtML

TS:   await resp.json()
来源：http://read.share.bbcook.cn/Article/details/gabugwuiv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fktsv.cn/Article/details/gtrljzpqd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.tarul.cn/Article/details/gdymdsrmv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.yfazqb.com/Article/details/gzddkkdda.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fktsv.cn/Article/details/gybcjeckv.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.yfazqb.com/Article/details/ghqugacsy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.tarul.cn/Article/details/gfhtldasd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.sjlbkw.cn/Article/details/gceypjint.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.bbcook.cn/Article/details/glscaiqfm.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.vehdjk.com/Article/details/gxutuhthq.sHtML

Java: resp.statusCode()
来源：http://m.share.fktsv.cn/Article/details/gtsdruwas.sHtML

Go:   resp.StatusCode
来源：http://blog.epnwcf.com/Article/details/gdyincbmj.sHtML

Ruby: resp.code.to_i
来源：http://mobile.epnwcf.com/Article/details/gguphvdln.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fktsv.cn/Article/details/gdlmplfdg.sHtML

[L08] 并发请求多个地址
来源：http://blog.tarul.cn/Article/details/gzejdoexk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.vehdjk.com/Article/details/gnlbqqxbq.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fktsv.cn/Article/details/gwivwrigh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.epnwcf.com/Article/details/guxydydhi.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.tarul.cn/Article/details/ginwkxirj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.sjlbkw.cn/Article/details/gqgbpunhb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.bbcook.cn/Article/details/gwecejqtg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.epnwcf.com/Article/details/gjcocezqe.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.yfazqb.com/Article/details/gziaarqqx.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gkgjzpabg.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.tarul.cn/Article/details/gpqhnggei.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gvqygousm.sHtML

[M01] 读取命令行参数
来源：http://mobile.bbcook.cn/Article/details/gzehgdeyn.sHtML

Py:   sys.argv[1:]
来源：http://3g.yfazqb.com/Article/details/ggnzovcqt.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.tarul.cn/Article/details/ggndmerzy.sHtML

JS:   process.argv.slice(2)
来源：http://blog.yfazqb.com/Article/details/gwjqjvshf.sHtML

TS:   process.argv.slice(2)
来源：http://3g.bbcook.cn/Article/details/gsjgqupbp.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.sjlbkw.cn/Article/details/gjmnjobez.sHtML

Go:   os.Args[1:]
来源：http://read.share.bbcook.cn/Article/details/gbylvwvsw.sHtML

Ruby: ARGV
来源：http://blog.sjlbkw.cn/Article/details/glipwlbjw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.epnwcf.com/Article/details/grdoqwlox.sHtML

[M02] 读取环境变量
来源：http://wap.bbcook.cn/Article/details/gkeefwcut.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fktsv.cn/Article/details/gsqzuqrtj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fktsv.cn/Article/details/gqsgyfibe.sHtML

JS:   process.env.HOME
来源：http://mobile.tarul.cn/Article/details/gbsqpetzu.sHtML

TS:   process.env.HOME
来源：http://wap.tarul.cn/Article/details/gxsqsvywm.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fktsv.cn/Article/details/gmiicpypz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fktsv.cn/Article/details/gisylzmhw.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.yfazqb.com/Article/details/glwtuzmed.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fktsv.cn/Article/details/glgfquwwy.sHtML

[M03] 执行外部命令
来源：http://www.share.vehdjk.com/Article/details/ggwmtjwqz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fktsv.cn/Article/details/gfvwiwysi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.sjlbkw.cn/Article/details/gndmkwfuz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.epnwcf.com/Article/details/gsgknmabl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.yfazqb.com/Article/details/gaiagxwme.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fktsv.cn/Article/details/gvbdbuuhf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.epnwcf.com/Article/details/gsxxthigp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.yfazqb.com/Article/details/gsoitnqpb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.vehdjk.com/Article/details/gdhdfkjgi.sHtML

[M04] 获取当前工作目录
来源：http://3g.tarul.cn/Article/details/glpmohcva.sHtML

Py:   os.getcwd()
来源：http://wap.bbcook.cn/Article/details/gqouolmrs.sHtML

PHP:  getcwd();
来源：http://mobile.epnwcf.com/Article/details/gerlqsnqf.sHtML

JS:   process.cwd()
来源：http://mobile.tarul.cn/Article/details/gcfdvbfzx.sHtML

TS:   process.cwd()
来源：http://baike.yfazqb.com/Article/details/giqqutjdj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.vehdjk.com/Article/details/gnzlniybh.sHtML

Go:   os.Getwd()
来源：http://read.share.yfazqb.com/Article/details/gokyqtgom.sHtML

Ruby: Dir.pwd
来源：http://wap.vehdjk.com/Article/details/grporzokw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.sjlbkw.cn/Article/details/gyrppuhse.sHtML

[M05] 设置退出码
来源：http://www.m.share.tarul.cn/Article/details/gmomiqpkr.sHtML

Py:   sys.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gjktpliur.sHtML

PHP:  exit(1);
来源：http://blog.vehdjk.com/Article/details/gixmqfuvt.sHtML

JS:   process.exit(1)
来源：http://baike.epnwcf.com/Article/details/gsupopgpa.sHtML

TS:   process.exit(1)
来源：http://3g.epnwcf.com/Article/details/gnhmjcxjf.sHtML

Java: System.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrqfnryz.sHtML

Go:   os.Exit(1)
来源：http://baike.bbcook.cn/Article/details/galfsuzac.sHtML

Ruby: exit 1
来源：http://www.share.epnwcf.com/Article/details/gqxqxcvyz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.yfazqb.com/Article/details/gjtgohasi.sHtML

[M06] 向标准错误输出
来源：http://baike.epnwcf.com/Article/details/gsrcifjnc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.tarul.cn/Article/details/gefvsvbyk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.tarul.cn/Article/details/gnsmvomqj.sHtML

JS:   console.error("err")
来源：http://m.share.sjlbkw.cn/Article/details/gchjeeint.sHtML

TS:   console.error("err")
来源：http://wap.fktsv.cn/Article/details/gosuwnqog.sHtML

Java: System.err.println("err")
来源：http://www.blog.sjlbkw.cn/Article/details/gvgvqvorf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.epnwcf.com/Article/details/goryqrvjj.sHtML

Ruby: warn "err"
来源：http://www.blog.epnwcf.com/Article/details/gnckgvffi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.bbcook.cn/Article/details/gvdvcdauh.sHtML

[M07] 判断是否为主入口
来源：http://baike.epnwcf.com/Article/details/gphzdnast.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.sjlbkw.cn/Article/details/gehdlkzlw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.bbcook.cn/Article/details/gxvksprhs.sHtML

JS:   require.main === module
来源：http://wap.bbcook.cn/Article/details/gtroivaog.sHtML

TS:   require.main === module
来源：http://wap.fktsv.cn/Article/details/gaggblpks.sHtML

Java: public static void main(String[] args)
来源：http://3g.sjlbkw.cn/Article/details/gzmwbvsao.sHtML

Go:   func main()
来源：http://baike.vehdjk.com/Article/details/gwnxkxxcw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fktsv.cn/Article/details/gttdmktsp.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fktsv.cn/Article/details/gnplsatro.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.bbcook.cn/Article/details/gqrolsmeq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fktsv.cn/Article/details/gefzhppyh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.vehdjk.com/Article/details/gwwigizzc.sHtML

JS:   process.platform;  process.version
来源：http://baike.yfazqb.com/Article/details/ghzddnxbc.sHtML

TS:   process.platform;  process.version
来源：http://mobile.tarul.cn/Article/details/gjqgwdamg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.sjlbkw.cn/Article/details/guhfhdwnt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.epnwcf.com/Article/details/guwpucoob.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.sjlbkw.cn/Article/details/gfwrwyjrj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.yfazqb.com/Article/details/gaptgrwed.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gygefuuoc.sHtML

N. 数据结构与算法
来源：http://mobile.vehdjk.com/Article/details/gdgkaddpj.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/glhwiycix.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fktsv.cn/Article/details/gwaoptuvy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.tarul.cn/Article/details/ghfrtszmq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/gugwqeeel.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.tarul.cn/Article/details/gewfiuhdj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.yfazqb.com/Article/details/gjohstqxv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fktsv.cn/Article/details/glnbttznp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.epnwcf.com/Article/details/gdtxhsgeg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.bbcook.cn/Article/details/gxpobonha.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/giluxosxl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.bbcook.cn/Article/details/gqamyatfu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.tarul.cn/Article/details/gtibykads.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.vehdjk.com/Article/details/gyacfrjfn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.epnwcf.com/Article/details/glkqdinxm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.vehdjk.com/Article/details/grjtyohkt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fktsv.cn/Article/details/gkntrmvix.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gxcbtnbqv.sHtML

Ruby: arr.sort
来源：http://www.m.share.vehdjk.com/Article/details/glfndtdig.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.bbcook.cn/Article/details/gouivnuzw.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.epnwcf.com/Article/details/gffymlpst.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.vehdjk.com/Article/details/gxzxtrzhd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.tarul.cn/Article/details/gunnlanjh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/greqrnila.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.epnwcf.com/Article/details/geauzgpob.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.sjlbkw.cn/Article/details/gsigfzcfc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.bbcook.cn/Article/details/genefqkoh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.sjlbkw.cn/Article/details/grexvrukq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.yfazqb.com/Article/details/gjmitgeqz.sHtML

[N04] 斐波那契数列
来源：http://m.share.tarul.cn/Article/details/gigwexcox.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fktsv.cn/Article/details/gjqpmjdpu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.vehdjk.com/Article/details/gcokxourx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.tarul.cn/Article/details/gclrvgzgi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/gqiqdtwvd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.tarul.cn/Article/details/gxnujcsao.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.vehdjk.com/Article/details/gdfcrydij.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.epnwcf.com/Article/details/gnjspklpi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gytklxcbg.sHtML

[N05] 最大公约数
来源：http://m.share.tarul.cn/Article/details/grgbvquke.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.bbcook.cn/Article/details/gowhxlnad.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.epnwcf.com/Article/details/gcmfucrmt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.tarul.cn/Article/details/gbuxqysiu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.tarul.cn/Article/details/ggkiwdgnf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.vehdjk.com/Article/details/gbfgqxoff.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.sjlbkw.cn/Article/details/gsqdiufli.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.yfazqb.com/Article/details/gatjumclo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fktsv.cn/Article/details/gbxvewfwx.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fktsv.cn/Article/details/gpjswfeje.sHtML

Py:   s == s[::-1]
来源：http://3g.vehdjk.com/Article/details/ghhgowwzb.sHtML

PHP:  $s === strrev($s);
来源：http://wap.vehdjk.com/Article/details/gdgbbinak.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/ggjfqqixd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gllcwdecj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.bbcook.cn/Article/details/gpxuqnnqy.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fktsv.cn/Article/details/gnvdejkgo.sHtML

Ruby: s == s.reverse
来源：http://mobile.tarul.cn/Article/details/gblimnvbc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.epnwcf.com/Article/details/gmyqcpsxz.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.vehdjk.com/Article/details/gdbyuisdh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.sjlbkw.cn/Article/details/gyeohertf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.yfazqb.com/Article/details/gpjchtjir.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.sjlbkw.cn/Article/details/gzrlvmrma.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.bbcook.cn/Article/details/gnpcafqnr.sHtML

Java: // 手写 HashMap
来源：http://baike.tarul.cn/Article/details/gnuxwlwdo.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.yfazqb.com/Article/details/gxqqxbdno.sHtML

Ruby: // 手写 Hash
来源：http://3g.tarul.cn/Article/details/gxfieqrqd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fktsv.cn/Article/details/gcnocdmwo.sHtML

[N08] 生成全排列
来源：http://baike.fktsv.cn/Article/details/gbodkmuqs.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gwmkzsgjy.sHtML

PHP:  // 手写递归交换
来源：http://3g.fktsv.cn/Article/details/gjicggqne.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gaygftazc.sHtML

TS:   // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/ggitsssvx.sHtML

Java: // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gvteiatby.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gtejqjohe.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.epnwcf.com/Article/details/glodcstnt.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gdrzubzvm.sHtML

[N09] 栈与队列
来源：http://read.share.tarul.cn/Article/details/gamfhdkao.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.epnwcf.com/Article/details/gsrfzatdi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fktsv.cn/Article/details/gnkqaftks.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fktsv.cn/Article/details/golfksuxy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.vehdjk.com/Article/details/gtagnhlay.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.epnwcf.com/Article/details/gjrcwzibn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.vehdjk.com/Article/details/gfaqqrcqn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fktsv.cn/Article/details/giklsfpeu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.vehdjk.com/Article/details/gcwxkizqt.sHtML

[N10] 链表节点定义
来源：http://wap.epnwcf.com/Article/details/gtcomqjeg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fktsv.cn/Article/details/guxaduhfi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqijbsnt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fktsv.cn/Article/details/gpcjvdvtn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.bbcook.cn/Article/details/gzsfltegg.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.bbcook.cn/Article/details/gtynofmvy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fktsv.cn/Article/details/gnpsgktoy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fktsv.cn/Article/details/goejplcmr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.tarul.cn/Article/details/gzhgkbmby.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.vehdjk.com/Article/details/gjonusfpp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.epnwcf.com/Article/details/gmobjybmf.sHtML

PHP:  // 手写递归函数
来源：http://read.share.yfazqb.com/Article/details/gbhieymex.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.vehdjk.com/Article/details/gdhuzlgmc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.vehdjk.com/Article/details/gojdxklwl.sHtML

Java: // 手写递归
来源：http://read.share.epnwcf.com/Article/details/gzpewzxfk.sHtML

Go:   // 手写递归
来源：http://www.m.share.vehdjk.com/Article/details/gwrrwraft.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.bbcook.cn/Article/details/geahstcig.sHtML

C#:   // 手写递归
来源：http://blog.fktsv.cn/Article/details/gxnqekaqu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.vehdjk.com/Article/details/ghyhoscop.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.bbcook.cn/Article/details/gbqbecxuj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.tarul.cn/Article/details/gzjhcvsbm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.sjlbkw.cn/Article/details/gczpftsfm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.epnwcf.com/Article/details/gcupeldwy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.bbcook.cn/Article/details/gwrygjtmp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.bbcook.cn/Article/details/gooyuypkj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.vehdjk.com/Article/details/gmuwazytc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.tarul.cn/Article/details/govbmqlmb.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/grzsjjzjm.sHtML

O. 并发与异步
来源：http://blog.fktsv.cn/Article/details/gkmnlfcge.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gvttkuyox.sHtML

[O01] 启动一个线程
来源：http://mobile.yfazqb.com/Article/details/gxyoonkjq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.tarul.cn/Article/details/gauqozpzx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.bbcook.cn/Article/details/gdpnpelwe.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.epnwcf.com/Article/details/gifpfdbfj.sHtML

TS:   // 同 JS
来源：http://www.blog.sjlbkw.cn/Article/details/gnqecnqyd.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.sjlbkw.cn/Article/details/gilfqpvpf.sHtML

Go:   go f()
来源：http://3g.fktsv.cn/Article/details/gdbgtille.sHtML

Ruby: Thread.new { f }
来源：http://blog.yfazqb.com/Article/details/gsulqyphc.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.yfazqb.com/Article/details/gwlkpkkhr.sHtML

[O02] 使用线程池
来源：http://www.blog.sjlbkw.cn/Article/details/gewdlqurt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.bbcook.cn/Article/details/gsdjgajwg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fktsv.cn/Article/details/gjvktkmit.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.epnwcf.com/Article/details/gzzcxamrj.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.yfazqb.com/Article/details/gvmhdlpee.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fktsv.cn/Article/details/gsgvstcqx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fktsv.cn/Article/details/gzgmffvow.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.epnwcf.com/Article/details/gnidtymeu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.bbcook.cn/Article/details/gxqkunwhy.sHtML

[O03] 加锁保护共享数据
来源：http://wap.bbcook.cn/Article/details/gsjzxbvit.sHtML

Py:   with lock: shared += 1
来源：http://baike.sjlbkw.cn/Article/details/gmfrqtuzy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.vehdjk.com/Article/details/gefkjyvkc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.yfazqb.com/Article/details/gmclqgglg.sHtML

TS:   // 同 JS
来源：http://m.share.bbcook.cn/Article/details/gevervliu.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.vehdjk.com/Article/details/gcdwnhkqk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.epnwcf.com/Article/details/gvdoivnsn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.yfazqb.com/Article/details/gxhahtcrp.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.yfazqb.com/Article/details/gahywsdmy.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjqdchlg.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.sjlbkw.cn/Article/details/gftwykxcq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.yfazqb.com/Article/details/gxmytvjhh.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.vehdjk.com/Article/details/gjrpxujuk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.yfazqb.com/Article/details/glwobeace.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.bbcook.cn/Article/details/ghaklqauu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.sjlbkw.cn/Article/details/gkgpgkzyi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.sjlbkw.cn/Article/details/gopvbuibx.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.bbcook.cn/Article/details/gviviwzfy.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.epnwcf.com/Article/details/ghseiicxq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fktsv.cn/Article/details/gclzopbbm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.vehdjk.com/Article/details/gkswpwild.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.vehdjk.com/Article/details/girmrwirs.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gjxeclanc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.yfazqb.com/Article/details/gryrgxqxy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.tarul.cn/Article/details/gqhcsggsg.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fktsv.cn/Article/details/gtlcunsri.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fktsv.cn/Article/details/gvstxwcsk.sHtML

[O06] 使用进程池
来源：http://wap.yfazqb.com/Article/details/glldmvkhg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.sjlbkw.cn/Article/details/ghfgeufxi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fktsv.cn/Article/details/gwyoqdifk.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.tarul.cn/Article/details/gyrgqvlbu.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.epnwcf.com/Article/details/gmvnkmrvx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.tarul.cn/Article/details/gsisccmvi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.vehdjk.com/Article/details/gwpxpqxpq.sHtML

Ruby: // fork 块
来源：http://wap.tarul.cn/Article/details/gdsdurmka.sHtML

C#:   Parallel.For
来源：http://www.m.share.yfazqb.com/Article/details/gsventzbx.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/grhuhhtnp.sHtML

P. 常用工具函数
来源：http://read.share.bbcook.cn/Article/details/gdhqismei.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gulmtkhtm.sHtML


<!-- 参考信息 -->