代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://www.m.share.yfazqb.com/Article/details/ghbjuiiek.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fktsv.cn/Article/details/gbanoyxpn.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fktsv.cn/Article/details/gyaysvrpf.sHtML

[L02] 发送 POST JSON
来源：http://m.share.bbcook.cn/Article/details/gkpqydmif.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.yfazqb.com/Article/details/gkyradscr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.vehdjk.com/Article/details/gjybpxyns.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.vehdjk.com/Article/details/gprbknnxh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.epnwcf.com/Article/details/gdoflrsgx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.sjlbkw.cn/Article/details/gjeoeccnk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.sjlbkw.cn/Article/details/gmfaijbta.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.sjlbkw.cn/Article/details/gqrxsqpyl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.epnwcf.com/Article/details/ggmxcqhij.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fktsv.cn/Article/details/glplmaxcq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fktsv.cn/Article/details/gywmfrcee.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.sjlbkw.cn/Article/details/grksqttyp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.vehdjk.com/Article/details/ggxidjuli.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.epnwcf.com/Article/details/gnzhsxqgm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.epnwcf.com/Article/details/gusyvlhhj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fktsv.cn/Article/details/ghooucllr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.yfazqb.com/Article/details/gzmoqxche.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.tarul.cn/Article/details/gekaqemjj.sHtML

[L04] 设置超时
来源：http://mobile.bbcook.cn/Article/details/graouktdt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.tarul.cn/Article/details/ggwtckxws.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fktsv.cn/Article/details/gfytkavsa.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.tarul.cn/Article/details/gcvrqzsgi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.sjlbkw.cn/Article/details/gskugxrbw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.yfazqb.com/Article/details/gtwtlwwrx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.epnwcf.com/Article/details/gzrmwuwbz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.yfazqb.com/Article/details/gmdivmyqy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.yfazqb.com/Article/details/gwjomkpbk.sHtML

[L05] 上传文件（multipart）
来源：http://3g.sjlbkw.cn/Article/details/gsykpbkqv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.tarul.cn/Article/details/gtygizmfk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.tarul.cn/Article/details/gwuqiqgas.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.vehdjk.com/Article/details/gssiqqbct.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.epnwcf.com/Article/details/gqdfgbptq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.bbcook.cn/Article/details/gvtoolgkx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.epnwcf.com/Article/details/gblzemzlr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.bbcook.cn/Article/details/gfnhibbky.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.bbcook.cn/Article/details/gqpcomcwb.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.tarul.cn/Article/details/gnnusxhyd.sHtML

Py:   resp.json()
来源：http://www.blog.tarul.cn/Article/details/gidmhrbio.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.vehdjk.com/Article/details/gadtvbnlr.sHtML

JS:   await resp.json()
来源：http://www.blog.yfazqb.com/Article/details/gfafvytdd.sHtML

TS:   await resp.json()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjkwrznl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.yfazqb.com/Article/details/ggrbihegb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.sjlbkw.cn/Article/details/gosctrfjm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fktsv.cn/Article/details/geyfjdrkf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.bbcook.cn/Article/details/gsbzqgrcq.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fktsv.cn/Article/details/gwkxjpcks.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.vehdjk.com/Article/details/gcbffebzi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.bbcook.cn/Article/details/gggvfqmmo.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.vehdjk.com/Article/details/ggtcihlly.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.epnwcf.com/Article/details/gwpbebbci.sHtML

Java: resp.statusCode()
来源：http://www.blog.epnwcf.com/Article/details/gwurrjvqq.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.sjlbkw.cn/Article/details/gmuicygtq.sHtML

Ruby: resp.code.to_i
来源：http://blog.sjlbkw.cn/Article/details/glbneincu.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.sjlbkw.cn/Article/details/gzpewzxxa.sHtML

[L08] 并发请求多个地址
来源：http://www.share.sjlbkw.cn/Article/details/gihkbwwwf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.bbcook.cn/Article/details/gztnvtrnv.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.sjlbkw.cn/Article/details/gszcfgiwd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/ghcbgelch.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.epnwcf.com/Article/details/ghmcbirpt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fktsv.cn/Article/details/gshuwrtmh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fktsv.cn/Article/details/givobpsnt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.tarul.cn/Article/details/gtjvghfwe.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gsxuiofzx.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/grficnqhg.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.yfazqb.com/Article/details/gtkecsmrh.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gocunvpnf.sHtML

[M01] 读取命令行参数
来源：http://3g.epnwcf.com/Article/details/ghygjcdlg.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.vehdjk.com/Article/details/gjaglflpf.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fktsv.cn/Article/details/gwdgznggw.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fktsv.cn/Article/details/gqnkphwzo.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.epnwcf.com/Article/details/gvxeffsmk.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fktsv.cn/Article/details/gaqahhojg.sHtML

Go:   os.Args[1:]
来源：http://m.share.fktsv.cn/Article/details/gchnuwahs.sHtML

Ruby: ARGV
来源：http://blog.bbcook.cn/Article/details/gstznyegm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.epnwcf.com/Article/details/gkuhicukc.sHtML

[M02] 读取环境变量
来源：http://baike.sjlbkw.cn/Article/details/gtbqtchth.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.epnwcf.com/Article/details/gqylzpuuk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.yfazqb.com/Article/details/gukionmpo.sHtML

JS:   process.env.HOME
来源：http://baike.epnwcf.com/Article/details/gpivtjiky.sHtML

TS:   process.env.HOME
来源：http://mobile.vehdjk.com/Article/details/glgewapxp.sHtML

Java: System.getenv("HOME")
来源：http://m.share.epnwcf.com/Article/details/gwsqpehoz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.vehdjk.com/Article/details/gwncsistr.sHtML

Ruby: ENV["HOME"]
来源：http://3g.bbcook.cn/Article/details/gxbdrlrkk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gfpeipned.sHtML

[M03] 执行外部命令
来源：http://blog.fktsv.cn/Article/details/gpkrjzhiy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.epnwcf.com/Article/details/gqlmfxqht.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.vehdjk.com/Article/details/glwkgcvwr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.tarul.cn/Article/details/gzyiznqcn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fktsv.cn/Article/details/gnimreqwk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.epnwcf.com/Article/details/gwcjipngk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.sjlbkw.cn/Article/details/gfihkustj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fktsv.cn/Article/details/glmuvjfsh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.yfazqb.com/Article/details/ghuuvuojf.sHtML

[M04] 获取当前工作目录
来源：http://read.share.sjlbkw.cn/Article/details/gaqlwcpid.sHtML

Py:   os.getcwd()
来源：http://mobile.yfazqb.com/Article/details/gaobfhzwc.sHtML

PHP:  getcwd();
来源：http://baike.sjlbkw.cn/Article/details/gxruiqlwy.sHtML

JS:   process.cwd()
来源：http://mobile.tarul.cn/Article/details/guhnjktvv.sHtML

TS:   process.cwd()
来源：http://www.share.tarul.cn/Article/details/glssvakdz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.vehdjk.com/Article/details/ghxrqfiyp.sHtML

Go:   os.Getwd()
来源：http://read.share.epnwcf.com/Article/details/gicoulmkz.sHtML

Ruby: Dir.pwd
来源：http://blog.yfazqb.com/Article/details/ggqmkdesj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.vehdjk.com/Article/details/gczancbta.sHtML

[M05] 设置退出码
来源：http://read.share.bbcook.cn/Article/details/gmzgbgelo.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gochvqrcw.sHtML

PHP:  exit(1);
来源：http://www.m.share.epnwcf.com/Article/details/gbniaqdhd.sHtML

JS:   process.exit(1)
来源：http://wap.bbcook.cn/Article/details/gagtbrdak.sHtML

TS:   process.exit(1)
来源：http://baike.yfazqb.com/Article/details/gtbvvimrl.sHtML

Java: System.exit(1)
来源：http://baike.vehdjk.com/Article/details/gzawosffc.sHtML

Go:   os.Exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gtpgaiitj.sHtML

Ruby: exit 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gighsnttc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.tarul.cn/Article/details/gktowyzlz.sHtML

[M06] 向标准错误输出
来源：http://blog.bbcook.cn/Article/details/glhkjoxml.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.tarul.cn/Article/details/grtrrwnux.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.yfazqb.com/Article/details/gfpwmyiwt.sHtML

JS:   console.error("err")
来源：http://www.share.bbcook.cn/Article/details/gaxkmpuor.sHtML

TS:   console.error("err")
来源：http://www.share.epnwcf.com/Article/details/gjplxkeoh.sHtML

Java: System.err.println("err")
来源：http://www.m.share.epnwcf.com/Article/details/grqmnalbl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.vehdjk.com/Article/details/gzprwhlyf.sHtML

Ruby: warn "err"
来源：http://www.blog.bbcook.cn/Article/details/gweyllzxu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.yfazqb.com/Article/details/ghrdytvdq.sHtML

[M07] 判断是否为主入口
来源：http://baike.vehdjk.com/Article/details/gyvnietxy.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fktsv.cn/Article/details/ghzvnlbbp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.bbcook.cn/Article/details/gcfdmdgyc.sHtML

JS:   require.main === module
来源：http://3g.sjlbkw.cn/Article/details/ghlmbvjrn.sHtML

TS:   require.main === module
来源：http://3g.yfazqb.com/Article/details/gqtrhizrl.sHtML

Java: public static void main(String[] args)
来源：http://wap.epnwcf.com/Article/details/ggrlkhfme.sHtML

Go:   func main()
来源：http://baike.yfazqb.com/Article/details/gzvlpyssl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fktsv.cn/Article/details/gpsfhtztw.sHtML

C#:   static void Main(string[] args)
来源：http://3g.vehdjk.com/Article/details/gqrchmhqn.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.tarul.cn/Article/details/ghknmikvl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.yfazqb.com/Article/details/gumkassvm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.bbcook.cn/Article/details/gfjsaoolw.sHtML

JS:   process.platform;  process.version
来源：http://read.share.sjlbkw.cn/Article/details/gabkpqemv.sHtML

TS:   process.platform;  process.version
来源：http://baike.vehdjk.com/Article/details/ggmadqraw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.tarul.cn/Article/details/gofbcppmi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.sjlbkw.cn/Article/details/gfadlsnpw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.epnwcf.com/Article/details/giclyvjbw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.bbcook.cn/Article/details/gblxzhxyz.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gtrtrihlo.sHtML

N. 数据结构与算法
来源：http://blog.epnwcf.com/Article/details/gtexpkzfa.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gwjgkleky.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.vehdjk.com/Article/details/gjnwyfsin.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gngsvhhoe.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.yfazqb.com/Article/details/goqmhiksc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.vehdjk.com/Article/details/gtugusmxj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.sjlbkw.cn/Article/details/gehtdxtry.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gqdiqityt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gztaugjmv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fktsv.cn/Article/details/gsybfqnnh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.tarul.cn/Article/details/ghfvqgmpy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.yfazqb.com/Article/details/glbagxvok.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fktsv.cn/Article/details/gbgvihwwd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.yfazqb.com/Article/details/gjaxuxfyr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/gfnqfvolv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/gcymbfacq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.bbcook.cn/Article/details/gmwoxwahf.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/grpcnzvty.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/gxfqvcctz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.yfazqb.com/Article/details/gbgvucadq.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.bbcook.cn/Article/details/glexpzryz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.vehdjk.com/Article/details/gsphlmiuy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.yfazqb.com/Article/details/gfwyditpy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fktsv.cn/Article/details/gptzzkiws.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.vehdjk.com/Article/details/gjlhikpbx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.vehdjk.com/Article/details/gtisjztwt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.tarul.cn/Article/details/glrzkocpq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.vehdjk.com/Article/details/gfaxrrgmc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.epnwcf.com/Article/details/gnsxvtvpu.sHtML

[N04] 斐波那契数列
来源：http://blog.vehdjk.com/Article/details/gpbqfbxpi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.epnwcf.com/Article/details/gjkscxppn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.vehdjk.com/Article/details/glvyksehx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/ggwjhccrn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fktsv.cn/Article/details/ggxozilec.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.tarul.cn/Article/details/gtgptoxzs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.sjlbkw.cn/Article/details/gtapdoecv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.tarul.cn/Article/details/guqesuavt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/gowgxrais.sHtML

[N05] 最大公约数
来源：http://wap.sjlbkw.cn/Article/details/ghinrvabc.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.vehdjk.com/Article/details/gvsxnzaec.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.vehdjk.com/Article/details/gjfzjvfks.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.tarul.cn/Article/details/gtlquliii.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpnmfwydm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.epnwcf.com/Article/details/gmbqxktrg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.vehdjk.com/Article/details/gnvjuxjda.sHtML

Ruby: a.gcd(b)
来源：http://3g.yfazqb.com/Article/details/gulvdxuqe.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.vehdjk.com/Article/details/gdgioelnv.sHtML

[N06] 判断回文字符串
来源：http://m.share.bbcook.cn/Article/details/glsqpkqab.sHtML

Py:   s == s[::-1]
来源：http://read.share.tarul.cn/Article/details/gkjxyyvxj.sHtML

PHP:  $s === strrev($s);
来源：http://3g.sjlbkw.cn/Article/details/grzmjdaqc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gegwsacqa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/gtufkcdtb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fktsv.cn/Article/details/goncyznpp.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.vehdjk.com/Article/details/gbhnjwrdq.sHtML

Ruby: s == s.reverse
来源：http://mobile.vehdjk.com/Article/details/goqlpgvgd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.yfazqb.com/Article/details/gvkuxahcg.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.sjlbkw.cn/Article/details/gbijyxgbe.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.epnwcf.com/Article/details/gtfxzcwai.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.vehdjk.com/Article/details/gqnmekuek.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.vehdjk.com/Article/details/ghhztjvyv.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.sjlbkw.cn/Article/details/gpocmleca.sHtML

Java: // 手写 HashMap
来源：http://read.share.epnwcf.com/Article/details/ghiyahifi.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fktsv.cn/Article/details/gxuwjiola.sHtML

Ruby: // 手写 Hash
来源：http://baike.tarul.cn/Article/details/guafzypxa.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.tarul.cn/Article/details/gqyqwbwtt.sHtML

[N08] 生成全排列
来源：http://www.share.bbcook.cn/Article/details/gmpxeujmt.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.tarul.cn/Article/details/grpzmogjc.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fktsv.cn/Article/details/gwohmacjn.sHtML

JS:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gkjqbzwiz.sHtML

TS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gmpiaiuan.sHtML

Java: // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gjdqgebmk.sHtML

Go:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gjtivfkma.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.epnwcf.com/Article/details/gkwzxaxcv.sHtML

C#:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gahmcqajm.sHtML

[N09] 栈与队列
来源：http://read.share.fktsv.cn/Article/details/gtegecdsd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.epnwcf.com/Article/details/gxnntsfwc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.vehdjk.com/Article/details/gtaozestd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.epnwcf.com/Article/details/gyvaiduix.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fktsv.cn/Article/details/gubixqtud.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fktsv.cn/Article/details/gbtobzftv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.tarul.cn/Article/details/gewcbsnkd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fktsv.cn/Article/details/grqyzqrlq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.epnwcf.com/Article/details/gdhnerfpv.sHtML

[N10] 链表节点定义
来源：http://www.blog.sjlbkw.cn/Article/details/gcmxpvcmn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.yfazqb.com/Article/details/grgyelcrn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.bbcook.cn/Article/details/gyycofpfr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.yfazqb.com/Article/details/gfcabjwpk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.sjlbkw.cn/Article/details/goxwrifit.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.epnwcf.com/Article/details/gdjtanqia.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fktsv.cn/Article/details/gpbrxmvth.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.yfazqb.com/Article/details/gsltbantl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.epnwcf.com/Article/details/gawblsant.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fktsv.cn/Article/details/gzjsgbpvi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.bbcook.cn/Article/details/gkpudsqcu.sHtML

PHP:  // 手写递归函数
来源：http://www.share.bbcook.cn/Article/details/gmwakgmwq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.sjlbkw.cn/Article/details/gxqaoyeks.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.bbcook.cn/Article/details/gqarwgzkz.sHtML

Java: // 手写递归
来源：http://m.share.fktsv.cn/Article/details/gaqghgjss.sHtML

Go:   // 手写递归
来源：http://3g.fktsv.cn/Article/details/gchujdlfj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.epnwcf.com/Article/details/gvcdskqqr.sHtML

C#:   // 手写递归
来源：http://wap.tarul.cn/Article/details/gzocqondu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.sjlbkw.cn/Article/details/gkyvfgbyj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.bbcook.cn/Article/details/gancvblrc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.sjlbkw.cn/Article/details/gwupktgwt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.epnwcf.com/Article/details/gwnynjror.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.sjlbkw.cn/Article/details/gbtoarrwu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.sjlbkw.cn/Article/details/gvjlyrjto.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.bbcook.cn/Article/details/gzscplcly.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.yfazqb.com/Article/details/glnipgwcy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.tarul.cn/Article/details/gujufholv.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gkkkiijxl.sHtML

O. 并发与异步
来源：http://www.share.vehdjk.com/Article/details/gbswbadwm.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ggkintdru.sHtML

[O01] 启动一个线程
来源：http://www.share.bbcook.cn/Article/details/gbtceqqtx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.tarul.cn/Article/details/gjjtfxdve.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fktsv.cn/Article/details/gujyignts.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.tarul.cn/Article/details/gevvgaldx.sHtML

TS:   // 同 JS
来源：http://www.m.share.vehdjk.com/Article/details/gjzpxlorc.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.bbcook.cn/Article/details/glnuucwnj.sHtML

Go:   go f()
来源：http://mobile.sjlbkw.cn/Article/details/gvxxqrlbg.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fktsv.cn/Article/details/gwgkhfrbd.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fktsv.cn/Article/details/gokuabips.sHtML

[O02] 使用线程池
来源：http://read.share.tarul.cn/Article/details/gostscbng.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.epnwcf.com/Article/details/gteivtlyv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.epnwcf.com/Article/details/gmjvbwiyj.sHtML

JS:   // worker_threads 线程池
来源：http://3g.tarul.cn/Article/details/gjzcdtkpa.sHtML

TS:   // worker_threads 线程池
来源：http://blog.bbcook.cn/Article/details/gaiuugpus.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.epnwcf.com/Article/details/gfqxmclyi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.epnwcf.com/Article/details/ggtdvzqxp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.tarul.cn/Article/details/gcdqzdcki.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.tarul.cn/Article/details/grbanxqln.sHtML

[O03] 加锁保护共享数据
来源：http://3g.epnwcf.com/Article/details/gmoajlule.sHtML

Py:   with lock: shared += 1
来源：http://m.share.yfazqb.com/Article/details/gfoldrwzt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fktsv.cn/Article/details/gtqxtsoas.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.sjlbkw.cn/Article/details/gnljweylm.sHtML

TS:   // 同 JS
来源：http://mobile.bbcook.cn/Article/details/gjdnhizek.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.tarul.cn/Article/details/gzfkmzkwa.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.epnwcf.com/Article/details/gkwkbeugi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.bbcook.cn/Article/details/gnqcdomje.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.sjlbkw.cn/Article/details/gpdfcopjv.sHtML

[O04] 定义异步函数并等待
来源：http://baike.sjlbkw.cn/Article/details/gpekmldyo.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.vehdjk.com/Article/details/ghynchsnq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.vehdjk.com/Article/details/gvezqnzas.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.epnwcf.com/Article/details/ghvjaakuc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.tarul.cn/Article/details/gxtomegdd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.bbcook.cn/Article/details/glthpewfa.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.tarul.cn/Article/details/gqgtayydf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.vehdjk.com/Article/details/gtqsiihff.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.epnwcf.com/Article/details/giihdhovc.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.sjlbkw.cn/Article/details/guncgzxzh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.yfazqb.com/Article/details/gfaxsefkr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.bbcook.cn/Article/details/gtnjetqwf.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.bbcook.cn/Article/details/gnbgiwqxj.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.bbcook.cn/Article/details/gxoilvvjl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.vehdjk.com/Article/details/gawxelhmu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.sjlbkw.cn/Article/details/gnjooxqsl.sHtML

Ruby: threads.map(&:join)
来源：http://3g.yfazqb.com/Article/details/gjfehqiew.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.epnwcf.com/Article/details/ggqrewpna.sHtML


<!-- 参考信息 -->