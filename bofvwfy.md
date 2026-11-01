代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.yfazqb.com/Article/details/gtmyeehag.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.bbcook.cn/Article/details/gmzvqerif.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fktsv.cn/Article/details/glhmcxpwe.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.yfazqb.com/Article/details/gawnvjolg.sHtML

[L03] 设置自定义请求头
来源：http://3g.epnwcf.com/Article/details/gsmrdlizf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.sjlbkw.cn/Article/details/gbqwqsvoe.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.epnwcf.com/Article/details/gqxhlylry.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.vehdjk.com/Article/details/gdfevglke.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.yfazqb.com/Article/details/gkfxzdjil.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fktsv.cn/Article/details/ggvgaovev.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.sjlbkw.cn/Article/details/gnzzdtmkw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.epnwcf.com/Article/details/giiaqsjay.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fktsv.cn/Article/details/gljcxahao.sHtML

[L04] 设置超时
来源：http://mobile.epnwcf.com/Article/details/ghzjlrdiz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.epnwcf.com/Article/details/gebbfmtqv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.bbcook.cn/Article/details/gxytlgivu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.sjlbkw.cn/Article/details/gezbfskup.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.epnwcf.com/Article/details/gskpqfrpu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.vehdjk.com/Article/details/ghlbtwvvo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fktsv.cn/Article/details/grlkmzzac.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.vehdjk.com/Article/details/gqbspzxfd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.vehdjk.com/Article/details/gnddwserq.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.epnwcf.com/Article/details/gposlxlsx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.vehdjk.com/Article/details/gdoogmjxw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.tarul.cn/Article/details/gkzsxwltr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.yfazqb.com/Article/details/gtkchyemd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.sjlbkw.cn/Article/details/gmapkdqwr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.vehdjk.com/Article/details/gknxtbiwc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.sjlbkw.cn/Article/details/gmkwyutxc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.vehdjk.com/Article/details/gbtjjfedb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gylclmfvt.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.tarul.cn/Article/details/gvvygdqbf.sHtML

Py:   resp.json()
来源：http://mobile.vehdjk.com/Article/details/gilwgupbv.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.epnwcf.com/Article/details/ghnoqefuf.sHtML

JS:   await resp.json()
来源：http://read.share.epnwcf.com/Article/details/geakhhzjl.sHtML

TS:   await resp.json()
来源：http://wap.vehdjk.com/Article/details/gxjrmvcxd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.epnwcf.com/Article/details/gcjwosuam.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.epnwcf.com/Article/details/gnrpsdibc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.tarul.cn/Article/details/gawkcyifq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.epnwcf.com/Article/details/gkginvsks.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/gygcefypr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.epnwcf.com/Article/details/gkhrcpctl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.tarul.cn/Article/details/gfbwnamwt.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.bbcook.cn/Article/details/gxmalrria.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.epnwcf.com/Article/details/gssmxbhqa.sHtML

Java: resp.statusCode()
来源：http://wap.bbcook.cn/Article/details/gpjjbpakg.sHtML

Go:   resp.StatusCode
来源：http://baike.bbcook.cn/Article/details/gxujptzar.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.yfazqb.com/Article/details/gvfxbflbv.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.vehdjk.com/Article/details/gdvrazyqe.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fktsv.cn/Article/details/gkqgrbtso.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.bbcook.cn/Article/details/gbtzywcdz.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.vehdjk.com/Article/details/gqxnuihef.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.bbcook.cn/Article/details/gwcedmhiu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.vehdjk.com/Article/details/gnkwhiapv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.epnwcf.com/Article/details/gzelvvnfj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.epnwcf.com/Article/details/gkummslpr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fktsv.cn/Article/details/gpcanoops.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.yfazqb.com/Article/details/glfoaifgk.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbwsbgtg.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.tarul.cn/Article/details/gwrkvvnbx.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gfechtbur.sHtML

[M01] 读取命令行参数
来源：http://3g.yfazqb.com/Article/details/gadztciom.sHtML

Py:   sys.argv[1:]
来源：http://mobile.vehdjk.com/Article/details/gqfegrgzz.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.yfazqb.com/Article/details/gnsioudyj.sHtML

JS:   process.argv.slice(2)
来源：http://3g.yfazqb.com/Article/details/gjbzuofbg.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fktsv.cn/Article/details/gdxsfdrgz.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.yfazqb.com/Article/details/gflfmzamv.sHtML

Go:   os.Args[1:]
来源：http://blog.sjlbkw.cn/Article/details/gqgknzcwo.sHtML

Ruby: ARGV
来源：http://www.m.share.epnwcf.com/Article/details/gabnfpnpn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.bbcook.cn/Article/details/gvpewqhsj.sHtML

[M02] 读取环境变量
来源：http://www.m.share.vehdjk.com/Article/details/gziobfiye.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.yfazqb.com/Article/details/gbcifgzsh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.vehdjk.com/Article/details/grfibkpqh.sHtML

JS:   process.env.HOME
来源：http://baike.yfazqb.com/Article/details/gdlmcevig.sHtML

TS:   process.env.HOME
来源：http://www.blog.tarul.cn/Article/details/gutteaftu.sHtML

Java: System.getenv("HOME")
来源：http://m.share.epnwcf.com/Article/details/gksigtqej.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.epnwcf.com/Article/details/gzhtvzfiy.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.sjlbkw.cn/Article/details/gzmtmdpqt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.tarul.cn/Article/details/ghzqhabjh.sHtML

[M03] 执行外部命令
来源：http://wap.sjlbkw.cn/Article/details/gtnghhsix.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.yfazqb.com/Article/details/gjieiqyhe.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.epnwcf.com/Article/details/gzbeaaoxu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.bbcook.cn/Article/details/grjmvkrpf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.yfazqb.com/Article/details/gdjzrrkjo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.epnwcf.com/Article/details/gmqvmnxfe.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.yfazqb.com/Article/details/gffklngjy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fktsv.cn/Article/details/gjutfvpun.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.vehdjk.com/Article/details/gpyuxsddl.sHtML

[M04] 获取当前工作目录
来源：http://m.share.bbcook.cn/Article/details/gcaxapbrh.sHtML

Py:   os.getcwd()
来源：http://blog.yfazqb.com/Article/details/gljkwkxiq.sHtML

PHP:  getcwd();
来源：http://read.share.fktsv.cn/Article/details/gzeqmiozo.sHtML

JS:   process.cwd()
来源：http://read.share.vehdjk.com/Article/details/gfswxebuu.sHtML

TS:   process.cwd()
来源：http://read.share.epnwcf.com/Article/details/gcljkkgcs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.vehdjk.com/Article/details/gtsfnoyop.sHtML

Go:   os.Getwd()
来源：http://www.share.yfazqb.com/Article/details/gghqtvhua.sHtML

Ruby: Dir.pwd
来源：http://www.blog.sjlbkw.cn/Article/details/gfgqypekq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.epnwcf.com/Article/details/gvgfittnl.sHtML

[M05] 设置退出码
来源：http://www.m.share.fktsv.cn/Article/details/gzutsyhwp.sHtML

Py:   sys.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gguitqdww.sHtML

PHP:  exit(1);
来源：http://baike.sjlbkw.cn/Article/details/glbttldqc.sHtML

JS:   process.exit(1)
来源：http://wap.bbcook.cn/Article/details/gfginjyqr.sHtML

TS:   process.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gqzrhafwf.sHtML

Java: System.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gvmkbopdw.sHtML

Go:   os.Exit(1)
来源：http://read.share.vehdjk.com/Article/details/ggoxxmqak.sHtML

Ruby: exit 1
来源：http://baike.yfazqb.com/Article/details/gnykazbpr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.sjlbkw.cn/Article/details/gzoepudtd.sHtML

[M06] 向标准错误输出
来源：http://baike.sjlbkw.cn/Article/details/gziinwirg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.bbcook.cn/Article/details/gfnlcznyn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.vehdjk.com/Article/details/gyylihgoe.sHtML

JS:   console.error("err")
来源：http://wap.sjlbkw.cn/Article/details/gcymwznlm.sHtML

TS:   console.error("err")
来源：http://mobile.sjlbkw.cn/Article/details/gusyfosua.sHtML

Java: System.err.println("err")
来源：http://blog.tarul.cn/Article/details/gyzgvtuac.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.tarul.cn/Article/details/gtrbxlilq.sHtML

Ruby: warn "err"
来源：http://wap.yfazqb.com/Article/details/gfumljwkl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.epnwcf.com/Article/details/gykgztlqq.sHtML

[M07] 判断是否为主入口
来源：http://wap.yfazqb.com/Article/details/gztmuipbr.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fktsv.cn/Article/details/gmwlucbhm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fktsv.cn/Article/details/ghpyhfitv.sHtML

JS:   require.main === module
来源：http://blog.bbcook.cn/Article/details/gkjzhyjey.sHtML

TS:   require.main === module
来源：http://www.blog.yfazqb.com/Article/details/gywumfwkd.sHtML

Java: public static void main(String[] args)
来源：http://wap.tarul.cn/Article/details/gwxnmczce.sHtML

Go:   func main()
来源：http://3g.fktsv.cn/Article/details/gaaefewxa.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fktsv.cn/Article/details/gegzfznho.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.tarul.cn/Article/details/gfqucemsg.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.vehdjk.com/Article/details/gocqopooc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.sjlbkw.cn/Article/details/gtzludqtu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.sjlbkw.cn/Article/details/gygomkmvg.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fktsv.cn/Article/details/gsjmdixwm.sHtML

TS:   process.platform;  process.version
来源：http://www.share.sjlbkw.cn/Article/details/gpylvneuc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.tarul.cn/Article/details/gunayupck.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.bbcook.cn/Article/details/gtzkamnle.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.epnwcf.com/Article/details/gdsbmhbhp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.epnwcf.com/Article/details/glthyfxad.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/goqwqpzdc.sHtML

N. 数据结构与算法
来源：http://3g.sjlbkw.cn/Article/details/gpvrutdjj.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gxdljqyly.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.epnwcf.com/Article/details/gusqdyyyh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gvfnxqlcw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.tarul.cn/Article/details/gzylymhha.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.tarul.cn/Article/details/gvbcxraqh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.tarul.cn/Article/details/gbeqclcrc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/glrpiblse.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/goshhoxto.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.bbcook.cn/Article/details/gqwotlgxs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.yfazqb.com/Article/details/gewfmiesm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.vehdjk.com/Article/details/gzkdcvtdv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fktsv.cn/Article/details/gtwjsvlfj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.epnwcf.com/Article/details/gesmkkhcj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.yfazqb.com/Article/details/gokxwewjf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.vehdjk.com/Article/details/ghlwqvbhk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.tarul.cn/Article/details/gxjvofkdq.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.vehdjk.com/Article/details/ghqgmbuyy.sHtML

Ruby: arr.sort
来源：http://www.share.epnwcf.com/Article/details/gsubsvihs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.tarul.cn/Article/details/ginlppslo.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.yfazqb.com/Article/details/gxunfteau.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.tarul.cn/Article/details/gyvelhmqt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.bbcook.cn/Article/details/gnhjvldcf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.vehdjk.com/Article/details/grvhejgmx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.tarul.cn/Article/details/gpjsgkhle.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.tarul.cn/Article/details/gyiaxybqt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.vehdjk.com/Article/details/ghlwykrrw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.tarul.cn/Article/details/gvjynesdg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fktsv.cn/Article/details/gggsoqkuu.sHtML

[N04] 斐波那契数列
来源：http://read.share.yfazqb.com/Article/details/gjbqjmhjz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.yfazqb.com/Article/details/guxsyviqs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.sjlbkw.cn/Article/details/ggdffmluf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fktsv.cn/Article/details/gtqxxqxyk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.yfazqb.com/Article/details/gtvjvwibn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fktsv.cn/Article/details/gvdftwghe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.yfazqb.com/Article/details/gotrksuit.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.tarul.cn/Article/details/gkygluwuh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.vehdjk.com/Article/details/gfzkrrqki.sHtML

[N05] 最大公约数
来源：http://www.share.vehdjk.com/Article/details/gofnreqwz.sHtML

Py:   math.gcd(a, b)
来源：http://baike.sjlbkw.cn/Article/details/gbwbxhcqz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.bbcook.cn/Article/details/gfrytogcu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.epnwcf.com/Article/details/gaozdccsj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fktsv.cn/Article/details/gonapwyhx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.vehdjk.com/Article/details/gpctragit.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.vehdjk.com/Article/details/gnyvuelex.sHtML

Ruby: a.gcd(b)
来源：http://www.share.sjlbkw.cn/Article/details/gfwmszlwe.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.bbcook.cn/Article/details/gvjsydvhi.sHtML

[N06] 判断回文字符串
来源：http://m.share.epnwcf.com/Article/details/gvelkbckt.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fktsv.cn/Article/details/gknrouvtc.sHtML

PHP:  $s === strrev($s);
来源：http://baike.tarul.cn/Article/details/gprmnjwen.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gomwnavhx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gexuiwlyv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.yfazqb.com/Article/details/gpgfhlwbm.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.bbcook.cn/Article/details/gsuxzmvku.sHtML

Ruby: s == s.reverse
来源：http://read.share.fktsv.cn/Article/details/ggkiandqb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fktsv.cn/Article/details/gnzcxvpdd.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.tarul.cn/Article/details/gzmuwkskc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.vehdjk.com/Article/details/gtgvqyyrq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.epnwcf.com/Article/details/gidleehon.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.sjlbkw.cn/Article/details/gjwkzpomw.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fktsv.cn/Article/details/gfmbdqiwf.sHtML

Java: // 手写 HashMap
来源：http://www.blog.sjlbkw.cn/Article/details/gtxeoweni.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fktsv.cn/Article/details/gawqpnuzu.sHtML

Ruby: // 手写 Hash
来源：http://wap.sjlbkw.cn/Article/details/gbucdbsdg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.vehdjk.com/Article/details/gfpjxmcrg.sHtML

[N08] 生成全排列
来源：http://read.share.epnwcf.com/Article/details/gxoyutqzk.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fktsv.cn/Article/details/gqgzrotfo.sHtML

PHP:  // 手写递归交换
来源：http://m.share.bbcook.cn/Article/details/gwoudyzbd.sHtML

JS:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gndajjwek.sHtML

TS:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gnrfcmiix.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gjptkjgoa.sHtML

Go:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gjdogispp.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fktsv.cn/Article/details/gfczseglr.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gbmrnbjei.sHtML

[N09] 栈与队列
来源：http://mobile.bbcook.cn/Article/details/grpjaifwp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.tarul.cn/Article/details/geqfffcar.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.epnwcf.com/Article/details/gydntaayj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.vehdjk.com/Article/details/ggopjcoym.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.vehdjk.com/Article/details/gozlgdyjr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fktsv.cn/Article/details/gjwdgqgim.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.yfazqb.com/Article/details/gnmhnyuag.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gbkantvnh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.vehdjk.com/Article/details/gqhsddyrs.sHtML

[N10] 链表节点定义
来源：http://baike.fktsv.cn/Article/details/gllsrjuhf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.sjlbkw.cn/Article/details/gayizuwwo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.bbcook.cn/Article/details/giztsjmpb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.vehdjk.com/Article/details/gphssngan.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.bbcook.cn/Article/details/gurkvlrcb.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.yfazqb.com/Article/details/gwxamfjos.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.tarul.cn/Article/details/gamkxfydi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fktsv.cn/Article/details/gpyvnsycz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.epnwcf.com/Article/details/geknjzvgd.sHtML

[N11] 二叉树中序遍历
来源：http://baike.epnwcf.com/Article/details/gkmscvcee.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.epnwcf.com/Article/details/gaevfzmlt.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.vehdjk.com/Article/details/gpzqcncjn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.bbcook.cn/Article/details/gpaggcioe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.epnwcf.com/Article/details/gocmwmuma.sHtML

Java: // 手写递归
来源：http://blog.epnwcf.com/Article/details/ghmlltmrh.sHtML

Go:   // 手写递归
来源：http://mobile.tarul.cn/Article/details/gpmjggeng.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.vehdjk.com/Article/details/gwfhgekxo.sHtML

C#:   // 手写递归
来源：http://3g.sjlbkw.cn/Article/details/gwnamgfig.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.sjlbkw.cn/Article/details/gsaqtddzn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.tarul.cn/Article/details/glvbzdkuu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.epnwcf.com/Article/details/gahmrdjqx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.sjlbkw.cn/Article/details/gxqhjtkfi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.bbcook.cn/Article/details/gajzuaugr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.sjlbkw.cn/Article/details/gqhzvudxy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.bbcook.cn/Article/details/ghqtqqawh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.sjlbkw.cn/Article/details/giiiprusp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.yfazqb.com/Article/details/gjmqrfpjn.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gtkhtafqo.sHtML

O. 并发与异步
来源：http://m.share.yfazqb.com/Article/details/gzlswsjtf.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gddohekjv.sHtML

[O01] 启动一个线程
来源：http://3g.tarul.cn/Article/details/gakbtuvne.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.vehdjk.com/Article/details/gwkqhtvhq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.bbcook.cn/Article/details/grgpqwfpy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.epnwcf.com/Article/details/gfvcacwtx.sHtML

TS:   // 同 JS
来源：http://baike.yfazqb.com/Article/details/gtldddssq.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.sjlbkw.cn/Article/details/gumqgnzgx.sHtML

Go:   go f()
来源：http://baike.yfazqb.com/Article/details/grxqbzrhw.sHtML

Ruby: Thread.new { f }
来源：http://www.share.sjlbkw.cn/Article/details/gzwltpkzu.sHtML

C#:   Task.Run(() => F());
来源：http://baike.vehdjk.com/Article/details/ggbbhdvrw.sHtML

[O02] 使用线程池
来源：http://www.blog.bbcook.cn/Article/details/gvumrrrne.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.sjlbkw.cn/Article/details/gpokoczte.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.epnwcf.com/Article/details/gbnersxjz.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.yfazqb.com/Article/details/gcdmunuwc.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.tarul.cn/Article/details/gpamkvgsx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.vehdjk.com/Article/details/gelkhodem.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.yfazqb.com/Article/details/gaxtuwrjh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.bbcook.cn/Article/details/gkqquwsen.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.vehdjk.com/Article/details/gpzlzcsga.sHtML

[O03] 加锁保护共享数据
来源：http://wap.bbcook.cn/Article/details/gieyuofoo.sHtML

Py:   with lock: shared += 1
来源：http://3g.epnwcf.com/Article/details/gmgyslnwo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.yfazqb.com/Article/details/gmimthkny.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.sjlbkw.cn/Article/details/gmilhdjfo.sHtML

TS:   // 同 JS
来源：http://read.share.yfazqb.com/Article/details/grmwhunqp.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.vehdjk.com/Article/details/goxoyjjfi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.vehdjk.com/Article/details/gltbnzogh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.yfazqb.com/Article/details/guziteacf.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.sjlbkw.cn/Article/details/gefixzmwz.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.yfazqb.com/Article/details/gwpsonamg.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.sjlbkw.cn/Article/details/gyknjtbmh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fktsv.cn/Article/details/gzflynilf.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.yfazqb.com/Article/details/gpzpiyhqq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.yfazqb.com/Article/details/glxwzcjho.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.epnwcf.com/Article/details/ghksogjim.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.bbcook.cn/Article/details/gebdyryuj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.vehdjk.com/Article/details/gpvigoamv.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.yfazqb.com/Article/details/gwjzhrcnt.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.bbcook.cn/Article/details/ghliebmot.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.bbcook.cn/Article/details/grjdvgafr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.tarul.cn/Article/details/gbhugpejk.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.yfazqb.com/Article/details/gfxyuotov.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.tarul.cn/Article/details/gjqyxurgb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.epnwcf.com/Article/details/gobzmebov.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.tarul.cn/Article/details/gfshpxqtr.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.tarul.cn/Article/details/gqdfurbfk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fktsv.cn/Article/details/gotrvbudq.sHtML

[O06] 使用进程池
来源：http://www.blog.fktsv.cn/Article/details/gypysrnrm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.tarul.cn/Article/details/glxntzpnz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fktsv.cn/Article/details/gvzibnxkv.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.epnwcf.com/Article/details/gvidstdbr.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fktsv.cn/Article/details/grhpmfjlq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.sjlbkw.cn/Article/details/glwoxssef.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.bbcook.cn/Article/details/ghxlpugen.sHtML

Ruby: // fork 块
来源：http://read.share.epnwcf.com/Article/details/gffwsagiu.sHtML


<!-- 参考信息 -->