代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.vehdjk.com/Article/details/gpeefchcl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.yfazqb.com/Article/details/gntzyqokt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.tarul.cn/Article/details/gamdvvexc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.yfazqb.com/Article/details/gvfgncciz.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.vehdjk.com/Article/details/gbvcrcbmi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.vehdjk.com/Article/details/ggcrsmsou.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.sjlbkw.cn/Article/details/gvruhvlsy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.yfazqb.com/Article/details/gxheufevp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.sjlbkw.cn/Article/details/gikydltgw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.tarul.cn/Article/details/grmdoeird.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.bbcook.cn/Article/details/gkcaagvxf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fktsv.cn/Article/details/gczbjlfkq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fktsv.cn/Article/details/grujeczbn.sHtML

[L04] 设置超时
来源：http://mobile.sjlbkw.cn/Article/details/gkfefkcfs.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.vehdjk.com/Article/details/ggtlewtej.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fktsv.cn/Article/details/gkalgdpnd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.tarul.cn/Article/details/gnzigdnus.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.bbcook.cn/Article/details/gijbqigca.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.sjlbkw.cn/Article/details/ggjttokge.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.bbcook.cn/Article/details/gwsqglkjc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.sjlbkw.cn/Article/details/gfmwtstqo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fktsv.cn/Article/details/gehfslqgt.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fktsv.cn/Article/details/gqoyisjqe.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.epnwcf.com/Article/details/gdrbnyavp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.epnwcf.com/Article/details/gpagtrfno.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.epnwcf.com/Article/details/giservahg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.bbcook.cn/Article/details/ghvjcxulm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.yfazqb.com/Article/details/gjcpeykfj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.epnwcf.com/Article/details/gukvlytjv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fktsv.cn/Article/details/gadpepelp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fktsv.cn/Article/details/gajxxdltg.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.vehdjk.com/Article/details/gllgohskm.sHtML

Py:   resp.json()
来源：http://m.share.tarul.cn/Article/details/grtllgmqh.sHtML

PHP:  json_decode($body, true);
来源：http://wap.yfazqb.com/Article/details/ghtifzsls.sHtML

JS:   await resp.json()
来源：http://www.m.share.fktsv.cn/Article/details/gbelpsiyk.sHtML

TS:   await resp.json()
来源：http://blog.yfazqb.com/Article/details/glvdmgfde.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.tarul.cn/Article/details/grozhpekp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.bbcook.cn/Article/details/gsoyoozkm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.bbcook.cn/Article/details/ggwfxhkur.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.bbcook.cn/Article/details/gzufjqfcs.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.tarul.cn/Article/details/gnsdhurwq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.sjlbkw.cn/Article/details/gnlnqzymw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.epnwcf.com/Article/details/gzqmfnydv.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.vehdjk.com/Article/details/gmchnxzwo.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.epnwcf.com/Article/details/glplijebn.sHtML

Java: resp.statusCode()
来源：http://blog.epnwcf.com/Article/details/gmdgbtxeb.sHtML

Go:   resp.StatusCode
来源：http://www.share.yfazqb.com/Article/details/gigmhciep.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.bbcook.cn/Article/details/gjbfgzjgn.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.bbcook.cn/Article/details/gsghjlcrc.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnmhlcsi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.tarul.cn/Article/details/gbahwjarj.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.bbcook.cn/Article/details/gsglgivcq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/ghzfrxzyk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.bbcook.cn/Article/details/gxjfflqyj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.bbcook.cn/Article/details/gmtpjmklb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.epnwcf.com/Article/details/ghhqostpm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.bbcook.cn/Article/details/giqcirbbz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.bbcook.cn/Article/details/gjuwpwhqq.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gxlqfhecm.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.yfazqb.com/Article/details/gicbigiqc.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gnhtqsudj.sHtML

[M01] 读取命令行参数
来源：http://blog.epnwcf.com/Article/details/gfdeugjnk.sHtML

Py:   sys.argv[1:]
来源：http://read.share.epnwcf.com/Article/details/gkzceummi.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.tarul.cn/Article/details/gpxloenhn.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fktsv.cn/Article/details/gsxmjcuyb.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.yfazqb.com/Article/details/gcwdcspav.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.yfazqb.com/Article/details/grklwodbb.sHtML

Go:   os.Args[1:]
来源：http://3g.bbcook.cn/Article/details/gqofwshtg.sHtML

Ruby: ARGV
来源：http://baike.tarul.cn/Article/details/gzmznlpqe.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.epnwcf.com/Article/details/gsmobasfu.sHtML

[M02] 读取环境变量
来源：http://m.share.tarul.cn/Article/details/geckiledn.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.vehdjk.com/Article/details/gtsjfpruk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fktsv.cn/Article/details/gfcgsluku.sHtML

JS:   process.env.HOME
来源：http://3g.fktsv.cn/Article/details/gabzubivu.sHtML

TS:   process.env.HOME
来源：http://baike.tarul.cn/Article/details/gysdjvalk.sHtML

Java: System.getenv("HOME")
来源：http://baike.fktsv.cn/Article/details/gkgmztwhh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.vehdjk.com/Article/details/gcrwynwaa.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.vehdjk.com/Article/details/gidbkrhid.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.epnwcf.com/Article/details/gyzpnlrya.sHtML

[M03] 执行外部命令
来源：http://baike.epnwcf.com/Article/details/gkmwfhaab.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.epnwcf.com/Article/details/gnkbwawcf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.vehdjk.com/Article/details/gfythluoj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.epnwcf.com/Article/details/gxefwucgj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fktsv.cn/Article/details/gttlxrdog.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.sjlbkw.cn/Article/details/gldndrzbe.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.bbcook.cn/Article/details/gxqvzhsao.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.tarul.cn/Article/details/ghprektpw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.yfazqb.com/Article/details/gyoxosggx.sHtML

[M04] 获取当前工作目录
来源：http://wap.bbcook.cn/Article/details/ggbfukble.sHtML

Py:   os.getcwd()
来源：http://www.share.bbcook.cn/Article/details/gfwwzpnfc.sHtML

PHP:  getcwd();
来源：http://baike.sjlbkw.cn/Article/details/gpxwuraak.sHtML

JS:   process.cwd()
来源：http://read.share.sjlbkw.cn/Article/details/gvcvkmdwl.sHtML

TS:   process.cwd()
来源：http://3g.sjlbkw.cn/Article/details/gbnohvutl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.tarul.cn/Article/details/gtlmhsykz.sHtML

Go:   os.Getwd()
来源：http://wap.bbcook.cn/Article/details/gicptselh.sHtML

Ruby: Dir.pwd
来源：http://mobile.epnwcf.com/Article/details/gdfqdkvrf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.yfazqb.com/Article/details/gzjypshhn.sHtML

[M05] 设置退出码
来源：http://mobile.tarul.cn/Article/details/gnxouccsw.sHtML

Py:   sys.exit(1)
来源：http://baike.vehdjk.com/Article/details/gulieblnr.sHtML

PHP:  exit(1);
来源：http://wap.tarul.cn/Article/details/gcjmyiskf.sHtML

JS:   process.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/guirpzzee.sHtML

TS:   process.exit(1)
来源：http://m.share.tarul.cn/Article/details/gawhxsyda.sHtML

Java: System.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gqhosezsk.sHtML

Go:   os.Exit(1)
来源：http://3g.fktsv.cn/Article/details/ggpnfngha.sHtML

Ruby: exit 1
来源：http://mobile.tarul.cn/Article/details/gxxknwhmq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.tarul.cn/Article/details/gqnyyoseu.sHtML

[M06] 向标准错误输出
来源：http://mobile.sjlbkw.cn/Article/details/gppkzvltt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.tarul.cn/Article/details/gptlhvmzw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.vehdjk.com/Article/details/gmqgewbwk.sHtML

JS:   console.error("err")
来源：http://m.share.sjlbkw.cn/Article/details/gmromfsej.sHtML

TS:   console.error("err")
来源：http://3g.bbcook.cn/Article/details/gqqkvkipm.sHtML

Java: System.err.println("err")
来源：http://mobile.yfazqb.com/Article/details/gvvxqtlcq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.epnwcf.com/Article/details/gstynpmkj.sHtML

Ruby: warn "err"
来源：http://www.m.share.tarul.cn/Article/details/gbguhggjl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.epnwcf.com/Article/details/gjimjnwus.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.yfazqb.com/Article/details/gsbyisrut.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.yfazqb.com/Article/details/ggscpoawv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.epnwcf.com/Article/details/gvtjribrz.sHtML

JS:   require.main === module
来源：http://read.share.tarul.cn/Article/details/gtvfykwku.sHtML

TS:   require.main === module
来源：http://www.share.tarul.cn/Article/details/gqpwryyxl.sHtML

Java: public static void main(String[] args)
来源：http://wap.epnwcf.com/Article/details/gixjzblgc.sHtML

Go:   func main()
来源：http://blog.tarul.cn/Article/details/grsjooibz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.epnwcf.com/Article/details/ghcdmvwcr.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fktsv.cn/Article/details/gegjwebpz.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.bbcook.cn/Article/details/gskfxfmwd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.epnwcf.com/Article/details/gykmeiiqv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.tarul.cn/Article/details/gxozkgxjd.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fktsv.cn/Article/details/gupfmvrzq.sHtML

TS:   process.platform;  process.version
来源：http://m.share.vehdjk.com/Article/details/gqqkzeovu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.tarul.cn/Article/details/gkcrpgwdz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.yfazqb.com/Article/details/gisngqtsf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.epnwcf.com/Article/details/gawxxlfrm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.epnwcf.com/Article/details/gepsryqwu.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gilwyrzxp.sHtML

N. 数据结构与算法
来源：http://baike.bbcook.cn/Article/details/gwogicbvb.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gznwgumib.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.bbcook.cn/Article/details/gmmazxiqd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.yfazqb.com/Article/details/goaecvktf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.yfazqb.com/Article/details/gqgfketiw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.vehdjk.com/Article/details/ghvhnmbrr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.sjlbkw.cn/Article/details/gxfqxitxy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.yfazqb.com/Article/details/ggcqkezxh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/ghqbvqyjx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqamesks.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.epnwcf.com/Article/details/gdzvulatq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.sjlbkw.cn/Article/details/goiqzkcew.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.epnwcf.com/Article/details/geqmzlqmt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.yfazqb.com/Article/details/ghqclcouf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.vehdjk.com/Article/details/gaxpdvfka.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.tarul.cn/Article/details/glmopnxkd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.yfazqb.com/Article/details/gsmsnmdbl.sHtML

Go:   slices.Sort(arr)
来源：http://blog.bbcook.cn/Article/details/genymovqv.sHtML

Ruby: arr.sort
来源：http://blog.bbcook.cn/Article/details/guwjtigyr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.epnwcf.com/Article/details/gyticxuwb.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcicbjsj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.yfazqb.com/Article/details/gfhhowoig.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.tarul.cn/Article/details/gjotuccqx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.yfazqb.com/Article/details/ghkinjfbv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.yfazqb.com/Article/details/gmrlxucqc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.bbcook.cn/Article/details/gzoimnyxk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.bbcook.cn/Article/details/gvzmwremx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.tarul.cn/Article/details/gtxkgjhoz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fktsv.cn/Article/details/girpvfpjt.sHtML

[N04] 斐波那契数列
来源：http://mobile.tarul.cn/Article/details/gstarrxdo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.epnwcf.com/Article/details/glvglrdhp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.epnwcf.com/Article/details/guhqhguhl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/giennircc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/gmtbqegwh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.vehdjk.com/Article/details/gmmxlkfib.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.epnwcf.com/Article/details/gbbgyqemb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.epnwcf.com/Article/details/gkywrqwqh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/gdduttgua.sHtML

[N05] 最大公约数
来源：http://read.share.vehdjk.com/Article/details/gtcrhauem.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.epnwcf.com/Article/details/giswdbmdd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fktsv.cn/Article/details/gkgdaaoaq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.yfazqb.com/Article/details/gzlhwehkl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.yfazqb.com/Article/details/gqinlsxsn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.epnwcf.com/Article/details/gfxcwrsil.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.tarul.cn/Article/details/gzfmzmxli.sHtML

Ruby: a.gcd(b)
来源：http://baike.vehdjk.com/Article/details/gpfhilrvz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.tarul.cn/Article/details/gtistkaqb.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.vehdjk.com/Article/details/gvkfyprfo.sHtML

Py:   s == s[::-1]
来源：http://m.share.sjlbkw.cn/Article/details/gvdywwnyh.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.tarul.cn/Article/details/gowvdwtdx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/geeloauth.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/ghmpjramk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.epnwcf.com/Article/details/gcrrsvnar.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.yfazqb.com/Article/details/gywcgbvvj.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.vehdjk.com/Article/details/gccolhdnw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.epnwcf.com/Article/details/gvjczhhbx.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fktsv.cn/Article/details/gpqlywefy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.epnwcf.com/Article/details/gezrlmcsp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.yfazqb.com/Article/details/gnhgbikmv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.epnwcf.com/Article/details/gpbskyvds.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.tarul.cn/Article/details/gphwbwlwn.sHtML

Java: // 手写 HashMap
来源：http://read.share.bbcook.cn/Article/details/gbxebsbxi.sHtML

Go:   // 手写 map[int]int
来源：http://blog.tarul.cn/Article/details/ghsejguhm.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.yfazqb.com/Article/details/gqxxfnkad.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.tarul.cn/Article/details/gofunptse.sHtML

[N08] 生成全排列
来源：http://www.share.epnwcf.com/Article/details/glxdzmvlv.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.bbcook.cn/Article/details/gzppegafe.sHtML

PHP:  // 手写递归交换
来源：http://m.share.yfazqb.com/Article/details/geowoecpg.sHtML

JS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/glmyrsetc.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gvjanxhfp.sHtML

Java: // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gbobgrrvl.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gujvimszq.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.bbcook.cn/Article/details/gtpyunomj.sHtML

C#:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/govdcevsp.sHtML

[N09] 栈与队列
来源：http://baike.tarul.cn/Article/details/gdjvuoinj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.tarul.cn/Article/details/gxfmymmgz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.yfazqb.com/Article/details/gnmndycuf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.vehdjk.com/Article/details/gtqaqeuja.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.sjlbkw.cn/Article/details/ghuenaorn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.vehdjk.com/Article/details/gpyfcvavq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fktsv.cn/Article/details/gxrbiyrrh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gdrgbrfss.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.yfazqb.com/Article/details/gsbuygpma.sHtML

[N10] 链表节点定义
来源：http://mobile.epnwcf.com/Article/details/grrsbvdtx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.tarul.cn/Article/details/gaskghrdn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.tarul.cn/Article/details/gwknxxqek.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.epnwcf.com/Article/details/gevlbdvzs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.yfazqb.com/Article/details/golmftrcx.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.bbcook.cn/Article/details/gwnpjmksj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.yfazqb.com/Article/details/grxznjhpn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.sjlbkw.cn/Article/details/ghqposxee.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fktsv.cn/Article/details/gmyusgmyp.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fktsv.cn/Article/details/gsnblbqcj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.vehdjk.com/Article/details/gokfecoyv.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.epnwcf.com/Article/details/gdhjxthlh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.tarul.cn/Article/details/gonuysapv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.sjlbkw.cn/Article/details/gzybxqfzz.sHtML

Java: // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gofmvzzkl.sHtML

Go:   // 手写递归
来源：http://www.m.share.vehdjk.com/Article/details/ghilmegnd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.yfazqb.com/Article/details/geywbgnmi.sHtML

C#:   // 手写递归
来源：http://www.share.sjlbkw.cn/Article/details/gtvwdzqso.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fktsv.cn/Article/details/gswxzotgd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.bbcook.cn/Article/details/glhargqvp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.vehdjk.com/Article/details/gvnpniohx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.sjlbkw.cn/Article/details/gljqsrjts.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.vehdjk.com/Article/details/gkupuefml.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fktsv.cn/Article/details/ggbtqorcf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.yfazqb.com/Article/details/glyehrgyd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.sjlbkw.cn/Article/details/gnszulorc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fktsv.cn/Article/details/geniufwel.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gefuuzbhq.sHtML

O. 并发与异步
来源：http://baike.fktsv.cn/Article/details/gadxiajji.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gxvvnrpit.sHtML

[O01] 启动一个线程
来源：http://www.m.share.bbcook.cn/Article/details/gzbxlginw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.bbcook.cn/Article/details/gnlbupqvb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.bbcook.cn/Article/details/gfiwnyaxj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.epnwcf.com/Article/details/gutpmpyko.sHtML

TS:   // 同 JS
来源：http://blog.vehdjk.com/Article/details/gyrjfpwug.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.yfazqb.com/Article/details/gxorjnotr.sHtML

Go:   go f()
来源：http://m.share.tarul.cn/Article/details/gnvdylsxu.sHtML

Ruby: Thread.new { f }
来源：http://mobile.sjlbkw.cn/Article/details/gkidgboru.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fktsv.cn/Article/details/gylcdqdaf.sHtML

[O02] 使用线程池
来源：http://read.share.tarul.cn/Article/details/gikrwxanq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.yfazqb.com/Article/details/gdqynonql.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fktsv.cn/Article/details/geddhsjto.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.bbcook.cn/Article/details/gsgobiiif.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.tarul.cn/Article/details/gfpingxqp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.vehdjk.com/Article/details/ghvzvndvf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fktsv.cn/Article/details/gljajujiw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.yfazqb.com/Article/details/gjxltkmqc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.yfazqb.com/Article/details/gkjidnsrj.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.yfazqb.com/Article/details/ghtdcezrg.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fktsv.cn/Article/details/glcpcfpuh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.yfazqb.com/Article/details/grvznjbrq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.epnwcf.com/Article/details/gxspjtbid.sHtML

TS:   // 同 JS
来源：http://www.m.share.yfazqb.com/Article/details/gflzwtcmf.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.yfazqb.com/Article/details/gknclcrtx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.bbcook.cn/Article/details/gwrhaeqtv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.yfazqb.com/Article/details/gvvzdxnhi.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.epnwcf.com/Article/details/glkmoyapq.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.tarul.cn/Article/details/gpddzwcrx.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.yfazqb.com/Article/details/gzdpexcky.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.vehdjk.com/Article/details/grhdginoa.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gkvjljmxi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.sjlbkw.cn/Article/details/gjqdayzal.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fktsv.cn/Article/details/gejrzjysd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.vehdjk.com/Article/details/grnlbsrfy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.yfazqb.com/Article/details/gikxhkxlg.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.yfazqb.com/Article/details/gyjvwlead.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.sjlbkw.cn/Article/details/gwwtmsksj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.sjlbkw.cn/Article/details/gtpxnymao.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.vehdjk.com/Article/details/gylxfnnpp.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.yfazqb.com/Article/details/gyvfssmre.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.yfazqb.com/Article/details/gflyppbju.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.sjlbkw.cn/Article/details/gtvqwgazg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.vehdjk.com/Article/details/gfbskmxio.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.yfazqb.com/Article/details/giarwnwbz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fktsv.cn/Article/details/gawcvijqw.sHtML

[O06] 使用进程池
来源：http://mobile.vehdjk.com/Article/details/gpjinzcao.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.yfazqb.com/Article/details/gsuutbzkh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fktsv.cn/Article/details/gxmmdurgl.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.sjlbkw.cn/Article/details/gqjqmipio.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fktsv.cn/Article/details/ggnopsgmo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.yfazqb.com/Article/details/gcqbivfbk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fktsv.cn/Article/details/grdytwabs.sHtML

Ruby: // fork 块
来源：http://baike.tarul.cn/Article/details/ggsyeytif.sHtML


<!-- 参考信息 -->