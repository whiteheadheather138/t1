代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.tarul.cn/Article/details/gdrjdkdkr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.bbcook.cn/Article/details/gtyrjzyqn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcyfnucse.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.sjlbkw.cn/Article/details/grtoydokz.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fktsv.cn/Article/details/gbvyzxxtl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fktsv.cn/Article/details/gmnvhppgb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.vehdjk.com/Article/details/gwzggaqci.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.yfazqb.com/Article/details/gyfeleifz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.tarul.cn/Article/details/gkoecgttn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.tarul.cn/Article/details/gwnmeawck.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.yfazqb.com/Article/details/glcnixyua.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.bbcook.cn/Article/details/guzmngrlg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.tarul.cn/Article/details/gxcejvfuo.sHtML

[L04] 设置超时
来源：http://blog.yfazqb.com/Article/details/gdsfxrqfi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.tarul.cn/Article/details/gsvaqsyxr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.vehdjk.com/Article/details/gbitsqjor.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.bbcook.cn/Article/details/gcwryacup.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.yfazqb.com/Article/details/gcpmdpswl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.vehdjk.com/Article/details/gagdozzxf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.sjlbkw.cn/Article/details/gchqekrrp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.epnwcf.com/Article/details/gmwbcpgqy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.yfazqb.com/Article/details/gbjywcabz.sHtML

[L05] 上传文件（multipart）
来源：http://baike.sjlbkw.cn/Article/details/gwqlvkxrc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.yfazqb.com/Article/details/gipxvlaxw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.vehdjk.com/Article/details/gtugibkij.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.bbcook.cn/Article/details/gdgvbjemg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.yfazqb.com/Article/details/gwamgklxq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fktsv.cn/Article/details/gloqblhkd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.sjlbkw.cn/Article/details/gtmtwsdaj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.epnwcf.com/Article/details/gerizgict.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gbsbvrsny.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.vehdjk.com/Article/details/ghhdxnpgf.sHtML

Py:   resp.json()
来源：http://m.share.yfazqb.com/Article/details/gxfzoypxz.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fktsv.cn/Article/details/gceltxbsh.sHtML

JS:   await resp.json()
来源：http://m.share.fktsv.cn/Article/details/gyfcsgjza.sHtML

TS:   await resp.json()
来源：http://www.blog.bbcook.cn/Article/details/gwwcxlmro.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.vehdjk.com/Article/details/gwkzwfmnj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.vehdjk.com/Article/details/gibyigfis.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.vehdjk.com/Article/details/gtqnulnth.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.epnwcf.com/Article/details/gqephnpln.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.yfazqb.com/Article/details/guduwhqbl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.tarul.cn/Article/details/ghszwlpbp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.tarul.cn/Article/details/gjkabncyn.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fktsv.cn/Article/details/grlovlgmo.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fktsv.cn/Article/details/gffmtizil.sHtML

Java: resp.statusCode()
来源：http://3g.bbcook.cn/Article/details/gajuotinl.sHtML

Go:   resp.StatusCode
来源：http://wap.bbcook.cn/Article/details/guwhclaxs.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.vehdjk.com/Article/details/gndwdxiyg.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fktsv.cn/Article/details/gwgfycoye.sHtML

[L08] 并发请求多个地址
来源：http://m.share.vehdjk.com/Article/details/gcdgvuxzc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fktsv.cn/Article/details/genehmhdi.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.sjlbkw.cn/Article/details/gylxgesyu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.sjlbkw.cn/Article/details/gzpcbkykj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.vehdjk.com/Article/details/ggzgckywh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.epnwcf.com/Article/details/gzocpdpif.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.sjlbkw.cn/Article/details/gmcdpquql.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.bbcook.cn/Article/details/glyzsjdts.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.bbcook.cn/Article/details/gpjqydtqe.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gxmwnrmnl.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.vehdjk.com/Article/details/gcpkkmyyt.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/ggquoylqd.sHtML

[M01] 读取命令行参数
来源：http://baike.tarul.cn/Article/details/geavrafve.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gquogwqza.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.epnwcf.com/Article/details/gsvisiwmk.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.tarul.cn/Article/details/gcrqbbteb.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.vehdjk.com/Article/details/gkwnofwfg.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fktsv.cn/Article/details/gwbwxwmjc.sHtML

Go:   os.Args[1:]
来源：http://wap.epnwcf.com/Article/details/gurvaqijw.sHtML

Ruby: ARGV
来源：http://www.share.sjlbkw.cn/Article/details/ghclucral.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.yfazqb.com/Article/details/gyvqqfrof.sHtML

[M02] 读取环境变量
来源：http://wap.sjlbkw.cn/Article/details/guockmtbp.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/grbsvtoje.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.epnwcf.com/Article/details/gjrdxjqsn.sHtML

JS:   process.env.HOME
来源：http://read.share.yfazqb.com/Article/details/gnylfipvh.sHtML

TS:   process.env.HOME
来源：http://blog.bbcook.cn/Article/details/ggcgyjqus.sHtML

Java: System.getenv("HOME")
来源：http://read.share.yfazqb.com/Article/details/gcudjeafv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.tarul.cn/Article/details/gauungtdm.sHtML

Ruby: ENV["HOME"]
来源：http://wap.sjlbkw.cn/Article/details/guelcfgtv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.epnwcf.com/Article/details/greggodwn.sHtML

[M03] 执行外部命令
来源：http://m.share.fktsv.cn/Article/details/giqeeaycs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.yfazqb.com/Article/details/gncteqzdh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.yfazqb.com/Article/details/geipfwwfu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.sjlbkw.cn/Article/details/grukjqhit.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.vehdjk.com/Article/details/gvgajvqqt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fktsv.cn/Article/details/gzlnzahmp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.yfazqb.com/Article/details/gnbkrvxxf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.tarul.cn/Article/details/gobpcbbvc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fktsv.cn/Article/details/gmyxgkxme.sHtML

[M04] 获取当前工作目录
来源：http://mobile.yfazqb.com/Article/details/gmvxolqwb.sHtML

Py:   os.getcwd()
来源：http://baike.tarul.cn/Article/details/gfsbxxpwz.sHtML

PHP:  getcwd();
来源：http://wap.epnwcf.com/Article/details/gutotencq.sHtML

JS:   process.cwd()
来源：http://baike.vehdjk.com/Article/details/gutnhbyil.sHtML

TS:   process.cwd()
来源：http://www.share.sjlbkw.cn/Article/details/gwqljjjnj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.bbcook.cn/Article/details/gdyfgqyor.sHtML

Go:   os.Getwd()
来源：http://www.blog.bbcook.cn/Article/details/gnrjwppzn.sHtML

Ruby: Dir.pwd
来源：http://wap.sjlbkw.cn/Article/details/gqotsgtgh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.sjlbkw.cn/Article/details/gnzzxgzht.sHtML

[M05] 设置退出码
来源：http://mobile.sjlbkw.cn/Article/details/gsvypspoa.sHtML

Py:   sys.exit(1)
来源：http://baike.yfazqb.com/Article/details/gfkqzgnsg.sHtML

PHP:  exit(1);
来源：http://www.m.share.vehdjk.com/Article/details/gmcsuhpej.sHtML

JS:   process.exit(1)
来源：http://blog.fktsv.cn/Article/details/guteihojn.sHtML

TS:   process.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gaquiasyk.sHtML

Java: System.exit(1)
来源：http://wap.vehdjk.com/Article/details/glnvwqyzz.sHtML

Go:   os.Exit(1)
来源：http://3g.vehdjk.com/Article/details/gzuabutsf.sHtML

Ruby: exit 1
来源：http://www.blog.epnwcf.com/Article/details/grydaafge.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.vehdjk.com/Article/details/guiqajjre.sHtML

[M06] 向标准错误输出
来源：http://read.share.fktsv.cn/Article/details/ggvufiqrj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.tarul.cn/Article/details/ghuyqiuwn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.sjlbkw.cn/Article/details/gtdlbnlpb.sHtML

JS:   console.error("err")
来源：http://m.share.epnwcf.com/Article/details/gfemksqgo.sHtML

TS:   console.error("err")
来源：http://3g.tarul.cn/Article/details/grpmjqboy.sHtML

Java: System.err.println("err")
来源：http://3g.sjlbkw.cn/Article/details/gwxakndff.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.sjlbkw.cn/Article/details/gmqqaeysv.sHtML

Ruby: warn "err"
来源：http://m.share.vehdjk.com/Article/details/ggqyybnby.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.bbcook.cn/Article/details/galmqomck.sHtML

[M07] 判断是否为主入口
来源：http://wap.tarul.cn/Article/details/ghxqhobew.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fktsv.cn/Article/details/gxpylkkbj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.vehdjk.com/Article/details/gyrcjmotv.sHtML

JS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/gkbebatez.sHtML

TS:   require.main === module
来源：http://mobile.fktsv.cn/Article/details/gxfhyujnf.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fktsv.cn/Article/details/gnqavbotd.sHtML

Go:   func main()
来源：http://m.share.sjlbkw.cn/Article/details/gqpveyxjr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.tarul.cn/Article/details/grywwionf.sHtML

C#:   static void Main(string[] args)
来源：http://3g.tarul.cn/Article/details/grfvwzkqo.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fktsv.cn/Article/details/gdrrvzqtp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.yfazqb.com/Article/details/gssrokqqe.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.epnwcf.com/Article/details/gqrqmbapj.sHtML

JS:   process.platform;  process.version
来源：http://mobile.vehdjk.com/Article/details/gpqoyzjbh.sHtML

TS:   process.platform;  process.version
来源：http://www.share.vehdjk.com/Article/details/gsnhmkmdc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.tarul.cn/Article/details/gxrrljhto.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.sjlbkw.cn/Article/details/gvhletrli.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.yfazqb.com/Article/details/geqqlvngb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.yfazqb.com/Article/details/gimygxmox.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gnkwnoiyk.sHtML

N. 数据结构与算法
来源：http://m.share.epnwcf.com/Article/details/gjjbmveck.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gwmdnslnr.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.vehdjk.com/Article/details/gmqhzhywe.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gwrftbmtq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.yfazqb.com/Article/details/gvucjdpkh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/gmyvndpqw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.yfazqb.com/Article/details/gnjzpyouy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gkriaghxt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.tarul.cn/Article/details/ghcrnviwy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.epnwcf.com/Article/details/gncjlxdfj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fktsv.cn/Article/details/gsbdgozgz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.tarul.cn/Article/details/ggcstmuec.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.bbcook.cn/Article/details/gnbgvmsye.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.yfazqb.com/Article/details/glvtwhnpc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.tarul.cn/Article/details/gxchmagsq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.tarul.cn/Article/details/grddhjwlz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.tarul.cn/Article/details/gxphgyzpr.sHtML

Go:   slices.Sort(arr)
来源：http://blog.sjlbkw.cn/Article/details/guvjxpgxm.sHtML

Ruby: arr.sort
来源：http://3g.bbcook.cn/Article/details/gbntccbce.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.epnwcf.com/Article/details/gwghlpzob.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.yfazqb.com/Article/details/gellvdjsj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.tarul.cn/Article/details/gspvoebco.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.epnwcf.com/Article/details/gclbhxbhu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fktsv.cn/Article/details/gjubiiahr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.vehdjk.com/Article/details/gnducthbl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.yfazqb.com/Article/details/gmramzrgu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.epnwcf.com/Article/details/gxbfvxfwx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fktsv.cn/Article/details/gndpwwhve.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.sjlbkw.cn/Article/details/ghkcdtktu.sHtML

[N04] 斐波那契数列
来源：http://wap.fktsv.cn/Article/details/gzxqiwzff.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.yfazqb.com/Article/details/gnskyxoka.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.epnwcf.com/Article/details/ggkfsdusz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.vehdjk.com/Article/details/ghtcxzjes.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/gmmwsflub.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fktsv.cn/Article/details/gvhvhlajq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fktsv.cn/Article/details/gqcqmrpmk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.tarul.cn/Article/details/gtmdudkxw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fktsv.cn/Article/details/gygwewtyl.sHtML

[N05] 最大公约数
来源：http://baike.yfazqb.com/Article/details/glpxprjwc.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.yfazqb.com/Article/details/gmfzbgyop.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.sjlbkw.cn/Article/details/gmmwumxxj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.tarul.cn/Article/details/gheklwtds.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.bbcook.cn/Article/details/ghldknskr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.epnwcf.com/Article/details/gvzfnmphb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.epnwcf.com/Article/details/gfkuskjdv.sHtML

Ruby: a.gcd(b)
来源：http://baike.fktsv.cn/Article/details/grsovzlcz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.epnwcf.com/Article/details/gxbcqdtan.sHtML

[N06] 判断回文字符串
来源：http://m.share.bbcook.cn/Article/details/guadprlej.sHtML

Py:   s == s[::-1]
来源：http://read.share.bbcook.cn/Article/details/gzmjgwlmj.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.bbcook.cn/Article/details/grwmcpoxq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/gmjivdkak.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/giilfufus.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fktsv.cn/Article/details/gbmihpied.sHtML

Go:   // 双指针从两端比较
来源：http://baike.sjlbkw.cn/Article/details/gtgmspbeu.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.epnwcf.com/Article/details/gvydrmzkl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.bbcook.cn/Article/details/gbwlrsrwo.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.yfazqb.com/Article/details/gfqselwjp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.epnwcf.com/Article/details/gyfxmnlvt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.tarul.cn/Article/details/gvfdugxdt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fktsv.cn/Article/details/gukpmprfp.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.epnwcf.com/Article/details/gmogigmql.sHtML

Java: // 手写 HashMap
来源：http://wap.fktsv.cn/Article/details/gslraozxn.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fktsv.cn/Article/details/glclzkiao.sHtML

Ruby: // 手写 Hash
来源：http://mobile.tarul.cn/Article/details/gpfqszipa.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.sjlbkw.cn/Article/details/gofyhrgfh.sHtML

[N08] 生成全排列
来源：http://3g.epnwcf.com/Article/details/gzobqznzk.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gzrbiakms.sHtML

PHP:  // 手写递归交换
来源：http://www.share.bbcook.cn/Article/details/gfjjsuipj.sHtML

JS:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gezuefdoy.sHtML

TS:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gehiwsfqf.sHtML

Java: // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gckmknwcc.sHtML

Go:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gqgqzebku.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.epnwcf.com/Article/details/gjhtuvxny.sHtML

C#:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gsdpqvmsp.sHtML

[N09] 栈与队列
来源：http://mobile.fktsv.cn/Article/details/gqtkaaxpf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.epnwcf.com/Article/details/gvopnkzef.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.bbcook.cn/Article/details/ggzlpmbrs.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fktsv.cn/Article/details/gritpefnh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.bbcook.cn/Article/details/gzyshehan.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.epnwcf.com/Article/details/giualpmnv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.epnwcf.com/Article/details/gpnyzmuct.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.yfazqb.com/Article/details/gotvnzrux.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.vehdjk.com/Article/details/gsaojerwo.sHtML

[N10] 链表节点定义
来源：http://mobile.sjlbkw.cn/Article/details/gawnnzvzz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.vehdjk.com/Article/details/gofztrwev.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.vehdjk.com/Article/details/gwdeyhskm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.yfazqb.com/Article/details/gnposaljc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.yfazqb.com/Article/details/gywufgwim.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.yfazqb.com/Article/details/gshxngaqw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.tarul.cn/Article/details/giidwladd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.bbcook.cn/Article/details/gxayqqdbu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.sjlbkw.cn/Article/details/gavjmlbal.sHtML

[N11] 二叉树中序遍历
来源：http://3g.tarul.cn/Article/details/gaetrieco.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.vehdjk.com/Article/details/gnluiwxvi.sHtML

PHP:  // 手写递归函数
来源：http://read.share.vehdjk.com/Article/details/gwnqzorvl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.tarul.cn/Article/details/gyfytzple.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.tarul.cn/Article/details/gunceytak.sHtML

Java: // 手写递归
来源：http://www.share.tarul.cn/Article/details/gnifhujxu.sHtML

Go:   // 手写递归
来源：http://www.m.share.tarul.cn/Article/details/guzewrwol.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.vehdjk.com/Article/details/gxyrkmbbi.sHtML

C#:   // 手写递归
来源：http://www.share.yfazqb.com/Article/details/gvbqhntsl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.epnwcf.com/Article/details/gphqptazl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fktsv.cn/Article/details/gzmhtxnjw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.sjlbkw.cn/Article/details/gewgyjnrw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.sjlbkw.cn/Article/details/gjmznahhe.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.vehdjk.com/Article/details/gaaarbzes.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.vehdjk.com/Article/details/ghmgvosqy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.vehdjk.com/Article/details/grnhyezxc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.bbcook.cn/Article/details/grumwlbzx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.tarul.cn/Article/details/gaktbfmbh.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gnogasmfs.sHtML

O. 并发与异步
来源：http://read.share.bbcook.cn/Article/details/glngcmfft.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gesatzmts.sHtML

[O01] 启动一个线程
来源：http://read.share.sjlbkw.cn/Article/details/gwlnlccsz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.tarul.cn/Article/details/gvqmsyozb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.sjlbkw.cn/Article/details/gghvrclwu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fktsv.cn/Article/details/gpmnssulv.sHtML

TS:   // 同 JS
来源：http://www.share.vehdjk.com/Article/details/gvaietxtv.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.sjlbkw.cn/Article/details/ghbxkmocb.sHtML

Go:   go f()
来源：http://blog.fktsv.cn/Article/details/gmvzceder.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fktsv.cn/Article/details/ggwgfgfgv.sHtML

C#:   Task.Run(() => F());
来源：http://baike.sjlbkw.cn/Article/details/gwhgrvpaf.sHtML

[O02] 使用线程池
来源：http://www.blog.fktsv.cn/Article/details/gwwlfgyfs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.tarul.cn/Article/details/greibjgza.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.vehdjk.com/Article/details/gtruvckes.sHtML

JS:   // worker_threads 线程池
来源：http://wap.epnwcf.com/Article/details/gmawimnhi.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.epnwcf.com/Article/details/gewnskwvd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.vehdjk.com/Article/details/gizknnqqs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.vehdjk.com/Article/details/gyitnsvny.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fktsv.cn/Article/details/gapdlhgid.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.bbcook.cn/Article/details/gtqcmzvun.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fktsv.cn/Article/details/gnnrdcrnv.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.vehdjk.com/Article/details/gshlwpdjq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.epnwcf.com/Article/details/ghkkgrbmk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.epnwcf.com/Article/details/gyoexkxwi.sHtML

TS:   // 同 JS
来源：http://wap.tarul.cn/Article/details/gbrdkkyzd.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.bbcook.cn/Article/details/gkgftbwzj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.yfazqb.com/Article/details/gqlaqgcvs.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.tarul.cn/Article/details/gigejcunq.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.epnwcf.com/Article/details/gefsbnvgm.sHtML

[O04] 定义异步函数并等待
来源：http://wap.yfazqb.com/Article/details/gdemjfhbr.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.vehdjk.com/Article/details/gvweshnaq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.epnwcf.com/Article/details/gfpsbafao.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.tarul.cn/Article/details/galpsvekk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.epnwcf.com/Article/details/gewqyuyeg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.vehdjk.com/Article/details/gbyzzmjot.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.yfazqb.com/Article/details/gjnjmckbe.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.bbcook.cn/Article/details/guktnlwdy.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.bbcook.cn/Article/details/gwcnemgax.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.yfazqb.com/Article/details/gkyaadsum.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.epnwcf.com/Article/details/gyudkzqco.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.vehdjk.com/Article/details/gboguohkm.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.vehdjk.com/Article/details/gjozuexsx.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.epnwcf.com/Article/details/gagarzzpe.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.sjlbkw.cn/Article/details/guanmqstm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fktsv.cn/Article/details/gnxdydfvw.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.bbcook.cn/Article/details/goputaokv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.tarul.cn/Article/details/gawnjvzeg.sHtML

[O06] 使用进程池
来源：http://www.m.share.fktsv.cn/Article/details/gmwrpexeb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.sjlbkw.cn/Article/details/gfnsblaxn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.vehdjk.com/Article/details/gjegjuepe.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.sjlbkw.cn/Article/details/gpqvzhmkk.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.epnwcf.com/Article/details/gtcvnscsl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.tarul.cn/Article/details/gljwjrgxe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.epnwcf.com/Article/details/grxzewrvx.sHtML

Ruby: // fork 块
来源：http://3g.vehdjk.com/Article/details/gplhtfeqa.sHtML


<!-- 参考信息 -->