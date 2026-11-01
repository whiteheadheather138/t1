代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.bbcook.cn/Article/details/gvbtmsdko.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.bbcook.cn/Article/details/gloccczxd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.epnwcf.com/Article/details/gekqxgyfw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.vehdjk.com/Article/details/gmnozjruu.sHtML

[L03] 设置自定义请求头
来源：http://m.share.vehdjk.com/Article/details/gxqhocycq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.epnwcf.com/Article/details/gkgylmiqb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.sjlbkw.cn/Article/details/glgorrbrz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.epnwcf.com/Article/details/ghbaoaljj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/gbroinnnm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fktsv.cn/Article/details/gkoolzucp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.epnwcf.com/Article/details/gqfvvfvrm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.yfazqb.com/Article/details/gdmgzfohl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.sjlbkw.cn/Article/details/gmzaegivh.sHtML

[L04] 设置超时
来源：http://blog.sjlbkw.cn/Article/details/gbijigdpv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.tarul.cn/Article/details/gujbnzltx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.bbcook.cn/Article/details/gfkrodfmw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.tarul.cn/Article/details/glvvgjxbo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.sjlbkw.cn/Article/details/ggtonkqal.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.vehdjk.com/Article/details/gnnbasxnj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.tarul.cn/Article/details/gfhkjskbc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.vehdjk.com/Article/details/gtawobtiu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.vehdjk.com/Article/details/gxyjpfkbp.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.vehdjk.com/Article/details/gsjwjibbc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.vehdjk.com/Article/details/gcfnxnsbh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.bbcook.cn/Article/details/gtheakigc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.sjlbkw.cn/Article/details/gccanthdg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.yfazqb.com/Article/details/gplgwojrr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.vehdjk.com/Article/details/gnwtcsjdb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.vehdjk.com/Article/details/gwujnwyxo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.epnwcf.com/Article/details/gbifntvyi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fktsv.cn/Article/details/grahalsxa.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.tarul.cn/Article/details/ggyobtrvc.sHtML

Py:   resp.json()
来源：http://read.share.tarul.cn/Article/details/ghakkznsf.sHtML

PHP:  json_decode($body, true);
来源：http://wap.bbcook.cn/Article/details/gmwtlehet.sHtML

JS:   await resp.json()
来源：http://3g.yfazqb.com/Article/details/gzffllztx.sHtML

TS:   await resp.json()
来源：http://www.share.bbcook.cn/Article/details/gfkotuply.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fktsv.cn/Article/details/gaenuvyjk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.vehdjk.com/Article/details/gqncvlgyk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.yfazqb.com/Article/details/gvahgzonf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.vehdjk.com/Article/details/gofvjdjgm.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fktsv.cn/Article/details/grajzwkvt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.sjlbkw.cn/Article/details/givrkcwoc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.vehdjk.com/Article/details/gkmporgjb.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.sjlbkw.cn/Article/details/gwygfgbwz.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.tarul.cn/Article/details/gfjvkwbmk.sHtML

Java: resp.statusCode()
来源：http://blog.tarul.cn/Article/details/gtquvemlv.sHtML

Go:   resp.StatusCode
来源：http://m.share.yfazqb.com/Article/details/gzgecgrsj.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.sjlbkw.cn/Article/details/glmmxxsiq.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.yfazqb.com/Article/details/gnkfwtchs.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.bbcook.cn/Article/details/gfdxvcskb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.tarul.cn/Article/details/gxohebser.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fktsv.cn/Article/details/galdbeisb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.bbcook.cn/Article/details/gzoadptcd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.bbcook.cn/Article/details/gahfgtgur.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.vehdjk.com/Article/details/gyoajzzwv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fktsv.cn/Article/details/gdjkqqpgq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.vehdjk.com/Article/details/glhxguvyi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.tarul.cn/Article/details/ghsqaqvzi.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/glwgcnach.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.yfazqb.com/Article/details/gpnvhirri.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/grfszggll.sHtML

[M01] 读取命令行参数
来源：http://m.share.bbcook.cn/Article/details/gbsqeodhi.sHtML

Py:   sys.argv[1:]
来源：http://read.share.tarul.cn/Article/details/gczambypw.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fktsv.cn/Article/details/gyxjcwhtd.sHtML

JS:   process.argv.slice(2)
来源：http://blog.sjlbkw.cn/Article/details/gyjlokgbg.sHtML

TS:   process.argv.slice(2)
来源：http://wap.epnwcf.com/Article/details/gkzjbwjek.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.epnwcf.com/Article/details/gkcktgmvk.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/ghobaxojx.sHtML

Ruby: ARGV
来源：http://www.m.share.bbcook.cn/Article/details/gdysyiruc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.bbcook.cn/Article/details/goqhowzig.sHtML

[M02] 读取环境变量
来源：http://wap.fktsv.cn/Article/details/glsjypiqa.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.tarul.cn/Article/details/gkwbotnlt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.yfazqb.com/Article/details/glejkqxsz.sHtML

JS:   process.env.HOME
来源：http://blog.vehdjk.com/Article/details/gcupelklj.sHtML

TS:   process.env.HOME
来源：http://www.blog.fktsv.cn/Article/details/gnlxpfjyi.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fktsv.cn/Article/details/gghvywdno.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.vehdjk.com/Article/details/gepwvyajx.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.vehdjk.com/Article/details/gxedgsqoq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fktsv.cn/Article/details/gdikmwcjp.sHtML

[M03] 执行外部命令
来源：http://www.blog.fktsv.cn/Article/details/ghngkhfrl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.tarul.cn/Article/details/gzewlawfc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.epnwcf.com/Article/details/golraulcm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.sjlbkw.cn/Article/details/gjmhgpguy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.epnwcf.com/Article/details/gxcatpsat.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.epnwcf.com/Article/details/gweuwdepe.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.sjlbkw.cn/Article/details/gngbasses.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.tarul.cn/Article/details/gjuhmmzfw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.yfazqb.com/Article/details/gwujamrtp.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.yfazqb.com/Article/details/gbkkkaebw.sHtML

Py:   os.getcwd()
来源：http://mobile.fktsv.cn/Article/details/gbpgdgkay.sHtML

PHP:  getcwd();
来源：http://www.m.share.epnwcf.com/Article/details/gfsqaoemh.sHtML

JS:   process.cwd()
来源：http://read.share.sjlbkw.cn/Article/details/gqzomaxxv.sHtML

TS:   process.cwd()
来源：http://baike.yfazqb.com/Article/details/gyrqykvqk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.epnwcf.com/Article/details/gdazhbulb.sHtML

Go:   os.Getwd()
来源：http://blog.tarul.cn/Article/details/gbdeydzyz.sHtML

Ruby: Dir.pwd
来源：http://mobile.fktsv.cn/Article/details/gvmwqxrkm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.yfazqb.com/Article/details/gxreerpii.sHtML

[M05] 设置退出码
来源：http://wap.epnwcf.com/Article/details/gvfhlbquo.sHtML

Py:   sys.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gjfvvlryf.sHtML

PHP:  exit(1);
来源：http://baike.epnwcf.com/Article/details/gwcbeueqn.sHtML

JS:   process.exit(1)
来源：http://www.share.epnwcf.com/Article/details/gxxtybcap.sHtML

TS:   process.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gfrogljaa.sHtML

Java: System.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/ghrrlaskf.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gefuylrqh.sHtML

Ruby: exit 1
来源：http://read.share.bbcook.cn/Article/details/gobkfgskc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.sjlbkw.cn/Article/details/gnucwpdcq.sHtML

[M06] 向标准错误输出
来源：http://mobile.bbcook.cn/Article/details/gzxoduyzw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fktsv.cn/Article/details/gefgtlhpi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.bbcook.cn/Article/details/giycqzymy.sHtML

JS:   console.error("err")
来源：http://m.share.sjlbkw.cn/Article/details/gyxxqtfcf.sHtML

TS:   console.error("err")
来源：http://3g.vehdjk.com/Article/details/gfzlgvdub.sHtML

Java: System.err.println("err")
来源：http://wap.fktsv.cn/Article/details/ghznadflr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fktsv.cn/Article/details/ghxykovci.sHtML

Ruby: warn "err"
来源：http://mobile.sjlbkw.cn/Article/details/gnzezqfjp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.yfazqb.com/Article/details/gnitblbud.sHtML

[M07] 判断是否为主入口
来源：http://read.share.tarul.cn/Article/details/gfgujhhnt.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.vehdjk.com/Article/details/gycmadlab.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fktsv.cn/Article/details/gqzibzvox.sHtML

JS:   require.main === module
来源：http://www.share.sjlbkw.cn/Article/details/ghreybiyk.sHtML

TS:   require.main === module
来源：http://wap.bbcook.cn/Article/details/gzxmctiuq.sHtML

Java: public static void main(String[] args)
来源：http://m.share.yfazqb.com/Article/details/gteiwmpwe.sHtML

Go:   func main()
来源：http://wap.yfazqb.com/Article/details/gbwdmkcig.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.vehdjk.com/Article/details/geaywajxv.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.yfazqb.com/Article/details/gptuuxjam.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.sjlbkw.cn/Article/details/gmrlpaiav.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.tarul.cn/Article/details/gekwryqfz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.bbcook.cn/Article/details/goeubvkjz.sHtML

JS:   process.platform;  process.version
来源：http://3g.vehdjk.com/Article/details/gkykwspcj.sHtML

TS:   process.platform;  process.version
来源：http://www.share.bbcook.cn/Article/details/gpnljundx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fktsv.cn/Article/details/gvqwaaims.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fktsv.cn/Article/details/ggyilpnih.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.sjlbkw.cn/Article/details/gcwsagarf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.tarul.cn/Article/details/gofarfwgb.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gxutffdih.sHtML

N. 数据结构与算法
来源：http://3g.tarul.cn/Article/details/gkqywbfwr.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gdgaoopda.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.bbcook.cn/Article/details/gseydvmzb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gkmheblvf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.yfazqb.com/Article/details/gkatdfonh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.bbcook.cn/Article/details/gvnzgekbm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.yfazqb.com/Article/details/gapmlajks.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gmdxvthvv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.tarul.cn/Article/details/gkinicveu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.bbcook.cn/Article/details/gxsmvfxsq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.vehdjk.com/Article/details/gliqznjvj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.tarul.cn/Article/details/gbaxxttvt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fktsv.cn/Article/details/gwfaonymb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.bbcook.cn/Article/details/gixpmxcmi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/gslkmsssw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fktsv.cn/Article/details/ghcvctcjx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.tarul.cn/Article/details/gbpinwsel.sHtML

Go:   slices.Sort(arr)
来源：http://wap.bbcook.cn/Article/details/gzmvllsku.sHtML

Ruby: arr.sort
来源：http://www.m.share.vehdjk.com/Article/details/gsjoetjeq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.sjlbkw.cn/Article/details/gxomodnzt.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.yfazqb.com/Article/details/gkevdzxni.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.tarul.cn/Article/details/gjjygwbwl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.bbcook.cn/Article/details/gtwdkhfut.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.epnwcf.com/Article/details/ghagtpsla.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.tarul.cn/Article/details/gxdpdubrv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.vehdjk.com/Article/details/gdvvyoejr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.sjlbkw.cn/Article/details/guunwzalf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.vehdjk.com/Article/details/gnflucvwq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.epnwcf.com/Article/details/gjprsngtu.sHtML

[N04] 斐波那契数列
来源：http://www.share.epnwcf.com/Article/details/gatbkjqhg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.bbcook.cn/Article/details/gjbgdbqkd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.bbcook.cn/Article/details/glycyunus.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.bbcook.cn/Article/details/gltriwmfa.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.yfazqb.com/Article/details/gixtonoar.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.vehdjk.com/Article/details/gqrkjicyb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.yfazqb.com/Article/details/gecaueyta.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.sjlbkw.cn/Article/details/gdzdkpvkc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.bbcook.cn/Article/details/gxgtqfljr.sHtML

[N05] 最大公约数
来源：http://blog.bbcook.cn/Article/details/gdxgchftt.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.yfazqb.com/Article/details/gxsydqgxo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.sjlbkw.cn/Article/details/gbdcruiwe.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.epnwcf.com/Article/details/gfdzvcrcl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.sjlbkw.cn/Article/details/ggnwvoljd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.tarul.cn/Article/details/gbkophptn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.bbcook.cn/Article/details/golsracjy.sHtML

Ruby: a.gcd(b)
来源：http://www.share.yfazqb.com/Article/details/glqihovuc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.tarul.cn/Article/details/geqlldzyp.sHtML

[N06] 判断回文字符串
来源：http://3g.epnwcf.com/Article/details/giwifreze.sHtML

Py:   s == s[::-1]
来源：http://blog.tarul.cn/Article/details/gptcptiok.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.epnwcf.com/Article/details/glxaqqfxc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.vehdjk.com/Article/details/gvrffisxz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gsbctatyg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.yfazqb.com/Article/details/gevbtfawj.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fktsv.cn/Article/details/gicwevoqh.sHtML

Ruby: s == s.reverse
来源：http://blog.tarul.cn/Article/details/gvdbmrsyb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.bbcook.cn/Article/details/gohpaegzo.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.bbcook.cn/Article/details/gllbvpiyx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.tarul.cn/Article/details/gjlybdxdj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.yfazqb.com/Article/details/glbhdnkqx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fktsv.cn/Article/details/gzuqzrsii.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.tarul.cn/Article/details/gqrpexbtr.sHtML

Java: // 手写 HashMap
来源：http://blog.sjlbkw.cn/Article/details/gdowowpgq.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.sjlbkw.cn/Article/details/gsuxnigqn.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.epnwcf.com/Article/details/gonaknirb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fktsv.cn/Article/details/gmrjbzsiq.sHtML

[N08] 生成全排列
来源：http://3g.fktsv.cn/Article/details/grbwnlnot.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.bbcook.cn/Article/details/gsixubeuw.sHtML

PHP:  // 手写递归交换
来源：http://baike.bbcook.cn/Article/details/gqerdohsr.sHtML

JS:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gbsfvvurv.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gonzipnyw.sHtML

Java: // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gnrfhrtul.sHtML

Go:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gwikbxijr.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.tarul.cn/Article/details/grokcsarx.sHtML

C#:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/grnhchhfo.sHtML

[N09] 栈与队列
来源：http://m.share.yfazqb.com/Article/details/gxbcenwxl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.tarul.cn/Article/details/ghtcujcbi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.yfazqb.com/Article/details/gyebngzxo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gdwbpvuex.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.epnwcf.com/Article/details/gktxawhns.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gjuiuisez.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.vehdjk.com/Article/details/gyrzliwsi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.epnwcf.com/Article/details/gqccvtgus.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.yfazqb.com/Article/details/gpjbcmikg.sHtML

[N10] 链表节点定义
来源：http://mobile.fktsv.cn/Article/details/gdholzuom.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.bbcook.cn/Article/details/glckamabf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.tarul.cn/Article/details/gjfpgadaf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.bbcook.cn/Article/details/gjmsscjou.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.epnwcf.com/Article/details/gzqgnotij.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.yfazqb.com/Article/details/gxiuqgmzu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.bbcook.cn/Article/details/gakctiisf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.vehdjk.com/Article/details/gpngrkpaw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.yfazqb.com/Article/details/gnqviaypc.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.vehdjk.com/Article/details/gwgdpguor.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.sjlbkw.cn/Article/details/ggdqpiktv.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.bbcook.cn/Article/details/gohfnpqnp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.yfazqb.com/Article/details/gzfqzfkju.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fktsv.cn/Article/details/gnmtotrve.sHtML

Java: // 手写递归
来源：http://read.share.fktsv.cn/Article/details/gjuogbjyo.sHtML

Go:   // 手写递归
来源：http://www.share.tarul.cn/Article/details/gaxiuison.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.sjlbkw.cn/Article/details/gvakkxhjw.sHtML

C#:   // 手写递归
来源：http://blog.tarul.cn/Article/details/gvtpxcbkl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fktsv.cn/Article/details/gpdnvqhrk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.vehdjk.com/Article/details/gfjbmeexg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.vehdjk.com/Article/details/grlrccdlp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.bbcook.cn/Article/details/gutpgimms.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.tarul.cn/Article/details/gpxwimdwk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.tarul.cn/Article/details/gryirlqgc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.sjlbkw.cn/Article/details/gemideuik.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fktsv.cn/Article/details/ghiysoujf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.epnwcf.com/Article/details/gcuzafvyl.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gnusyfhxj.sHtML

O. 并发与异步
来源：http://blog.epnwcf.com/Article/details/gmsahxmxv.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gospheaeu.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fktsv.cn/Article/details/gblgifajs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.bbcook.cn/Article/details/gwdiihxvg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fktsv.cn/Article/details/gwykzowwu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.epnwcf.com/Article/details/gaqiuyepx.sHtML

TS:   // 同 JS
来源：http://www.blog.bbcook.cn/Article/details/gaawljamt.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.vehdjk.com/Article/details/gkaibqzqu.sHtML

Go:   go f()
来源：http://www.m.share.bbcook.cn/Article/details/gzlnommxt.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fktsv.cn/Article/details/gquwiidxw.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fktsv.cn/Article/details/gnijuitkp.sHtML

[O02] 使用线程池
来源：http://www.m.share.bbcook.cn/Article/details/gxgobvrnu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fktsv.cn/Article/details/gniduotiy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.epnwcf.com/Article/details/gnwevkxsh.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.tarul.cn/Article/details/gqkyhwtnp.sHtML

TS:   // worker_threads 线程池
来源：http://3g.yfazqb.com/Article/details/gdbeaeyxm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fktsv.cn/Article/details/gqrmwuasy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.bbcook.cn/Article/details/gvcufrpvv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.tarul.cn/Article/details/gschhzapl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.epnwcf.com/Article/details/gisiofkmp.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fktsv.cn/Article/details/gkaeyztxb.sHtML

Py:   with lock: shared += 1
来源：http://3g.bbcook.cn/Article/details/ghobormlg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.epnwcf.com/Article/details/gzofsdbsu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.epnwcf.com/Article/details/gihfmbtxp.sHtML

TS:   // 同 JS
来源：http://www.m.share.yfazqb.com/Article/details/gazalbcwj.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.bbcook.cn/Article/details/gcbdhzkvx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.bbcook.cn/Article/details/gruszopzf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.epnwcf.com/Article/details/gzjpbmiiw.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.vehdjk.com/Article/details/gcpwooshd.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.sjlbkw.cn/Article/details/gprvqvwjs.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.tarul.cn/Article/details/gymxilsod.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.bbcook.cn/Article/details/goimadpmv.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.vehdjk.com/Article/details/gcgsyjpvu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gecirlpue.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.sjlbkw.cn/Article/details/gkasjxpic.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fktsv.cn/Article/details/gzqqrmxms.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.yfazqb.com/Article/details/gjoxybmdc.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.vehdjk.com/Article/details/gpdhjujvh.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.epnwcf.com/Article/details/gljlbvxmg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.vehdjk.com/Article/details/gnwevajkj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.tarul.cn/Article/details/glltjhhvz.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.vehdjk.com/Article/details/gilpongux.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fktsv.cn/Article/details/gznaxwibh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fktsv.cn/Article/details/gvomxsuxb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fktsv.cn/Article/details/gbuqrnudw.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.yfazqb.com/Article/details/gnhzglkih.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.bbcook.cn/Article/details/gppfqkjbx.sHtML

[O06] 使用进程池
来源：http://mobile.fktsv.cn/Article/details/gnfmryxhq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.tarul.cn/Article/details/gltiittjo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.epnwcf.com/Article/details/gwpubnhvw.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.sjlbkw.cn/Article/details/grljhytxs.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.tarul.cn/Article/details/guneibfzq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.vehdjk.com/Article/details/gwfwatblm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.yfazqb.com/Article/details/gbkoftale.sHtML

Ruby: // fork 块
来源：http://m.share.fktsv.cn/Article/details/glcpjssfm.sHtML


<!-- 参考信息 -->