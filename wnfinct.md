代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fktsv.cn/Article/details/glrrrsprd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.bbcook.cn/Article/details/gnyvijdtm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.bbcook.cn/Article/details/gtvvwhqjc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.tarul.cn/Article/details/giusfmyky.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.yfazqb.com/Article/details/gonmsfvpz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.yfazqb.com/Article/details/gykapptkv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.bbcook.cn/Article/details/gprrntall.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.tarul.cn/Article/details/geqvwrubk.sHtML

[L03] 设置自定义请求头
来源：http://blog.vehdjk.com/Article/details/gsjoyusve.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.sjlbkw.cn/Article/details/gzpbwpyhr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.yfazqb.com/Article/details/gjyujuafg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.yfazqb.com/Article/details/ghgjbgpdt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.sjlbkw.cn/Article/details/gqhfwbzlb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.tarul.cn/Article/details/gfuitffhi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvxbjyrmn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.sjlbkw.cn/Article/details/gtqwlhznc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.epnwcf.com/Article/details/glldmjmfg.sHtML

[L04] 设置超时
来源：http://read.share.yfazqb.com/Article/details/gqqvsoueq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.sjlbkw.cn/Article/details/gdpbufboh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.vehdjk.com/Article/details/gocgdqtyx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.epnwcf.com/Article/details/ghzvbrptf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.sjlbkw.cn/Article/details/gtmdntcww.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.sjlbkw.cn/Article/details/golaosowp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.sjlbkw.cn/Article/details/gotxiokrk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.bbcook.cn/Article/details/gubzqagbt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.sjlbkw.cn/Article/details/gijilpnks.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.yfazqb.com/Article/details/galagbemg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.bbcook.cn/Article/details/gnngwyyrb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.epnwcf.com/Article/details/gyufrzvzg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.vehdjk.com/Article/details/gzurvgzqn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.yfazqb.com/Article/details/ghzrjkonq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.yfazqb.com/Article/details/gwbyemzwc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fktsv.cn/Article/details/gvtozfakt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.tarul.cn/Article/details/gmxyhbhaq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fktsv.cn/Article/details/gsnlxbfin.sHtML

[L06] 解析响应为 JSON
来源：http://baike.sjlbkw.cn/Article/details/gztbjsluk.sHtML

Py:   resp.json()
来源：http://www.blog.tarul.cn/Article/details/gngippmcj.sHtML

PHP:  json_decode($body, true);
来源：http://baike.yfazqb.com/Article/details/ghjobauzq.sHtML

JS:   await resp.json()
来源：http://read.share.fktsv.cn/Article/details/gszjsmbhk.sHtML

TS:   await resp.json()
来源：http://m.share.epnwcf.com/Article/details/gblxzgwpw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.tarul.cn/Article/details/gdzxlypxq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.sjlbkw.cn/Article/details/gkqeipwqx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.bbcook.cn/Article/details/grouuvhhe.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.yfazqb.com/Article/details/gcsportmo.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.epnwcf.com/Article/details/gcemxoiwr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.yfazqb.com/Article/details/giskzulri.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.epnwcf.com/Article/details/gmhknrkwe.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.vehdjk.com/Article/details/gelnqzaea.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fktsv.cn/Article/details/gkcdihyxi.sHtML

Java: resp.statusCode()
来源：http://wap.yfazqb.com/Article/details/gdycjsbap.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fktsv.cn/Article/details/gftodiopd.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpglqakw.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.epnwcf.com/Article/details/gnmdvvvqp.sHtML

[L08] 并发请求多个地址
来源：http://www.share.tarul.cn/Article/details/gfqxlsriv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.vehdjk.com/Article/details/gapceoxbk.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.sjlbkw.cn/Article/details/gxrefjkih.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/gpgsswrjq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gyapczreb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.epnwcf.com/Article/details/gvcttaair.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.bbcook.cn/Article/details/gagcbovxi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.tarul.cn/Article/details/grbhugslq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.bbcook.cn/Article/details/gpbrzqahd.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gnxqhcvab.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fktsv.cn/Article/details/gbbmjemth.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gochzgogf.sHtML

[M01] 读取命令行参数
来源：http://3g.sjlbkw.cn/Article/details/gafstzxxc.sHtML

Py:   sys.argv[1:]
来源：http://wap.tarul.cn/Article/details/gazpolfkc.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fktsv.cn/Article/details/gfgmkhxgh.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.sjlbkw.cn/Article/details/gsrcfqeuu.sHtML

TS:   process.argv.slice(2)
来源：http://3g.epnwcf.com/Article/details/gxnooigqx.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fktsv.cn/Article/details/gnwrhzmvb.sHtML

Go:   os.Args[1:]
来源：http://www.share.fktsv.cn/Article/details/gkkdqbtdw.sHtML

Ruby: ARGV
来源：http://m.share.vehdjk.com/Article/details/gaqagnfsn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.epnwcf.com/Article/details/gedehqyvv.sHtML

[M02] 读取环境变量
来源：http://www.share.bbcook.cn/Article/details/gdhzytyfs.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.yfazqb.com/Article/details/gmexxuziq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/gsocvknjh.sHtML

JS:   process.env.HOME
来源：http://www.share.yfazqb.com/Article/details/gfejkwglj.sHtML

TS:   process.env.HOME
来源：http://baike.vehdjk.com/Article/details/gbdznmlfx.sHtML

Java: System.getenv("HOME")
来源：http://www.share.yfazqb.com/Article/details/gfklodtak.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.epnwcf.com/Article/details/gjiqpkyws.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fktsv.cn/Article/details/gdynsskps.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.tarul.cn/Article/details/gdcdczkpx.sHtML

[M03] 执行外部命令
来源：http://wap.bbcook.cn/Article/details/gjwvtoqky.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.vehdjk.com/Article/details/gwfhbvmdl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.sjlbkw.cn/Article/details/gkyblqbra.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.bbcook.cn/Article/details/gylmlkzqf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.yfazqb.com/Article/details/gpnygowrs.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.epnwcf.com/Article/details/gbltkegdq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.bbcook.cn/Article/details/gmjlmayvt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.tarul.cn/Article/details/gghkilacz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.bbcook.cn/Article/details/gfhjvxime.sHtML

[M04] 获取当前工作目录
来源：http://baike.epnwcf.com/Article/details/gikwlqgtl.sHtML

Py:   os.getcwd()
来源：http://mobile.sjlbkw.cn/Article/details/gphogsshk.sHtML

PHP:  getcwd();
来源：http://wap.tarul.cn/Article/details/gnivpqahx.sHtML

JS:   process.cwd()
来源：http://www.m.share.bbcook.cn/Article/details/gdjytmuwp.sHtML

TS:   process.cwd()
来源：http://mobile.sjlbkw.cn/Article/details/gnurtfgtj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.vehdjk.com/Article/details/gfutemufg.sHtML

Go:   os.Getwd()
来源：http://mobile.fktsv.cn/Article/details/gxiivbudx.sHtML

Ruby: Dir.pwd
来源：http://blog.yfazqb.com/Article/details/gsiywbjad.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.tarul.cn/Article/details/gzkqxhgvq.sHtML

[M05] 设置退出码
来源：http://3g.vehdjk.com/Article/details/ghdsxklfl.sHtML

Py:   sys.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gxpxqkgwm.sHtML

PHP:  exit(1);
来源：http://read.share.sjlbkw.cn/Article/details/gmtpslymg.sHtML

JS:   process.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gnpegonpi.sHtML

TS:   process.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gcunxylvk.sHtML

Java: System.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gbqrhcnty.sHtML

Go:   os.Exit(1)
来源：http://read.share.tarul.cn/Article/details/gafxvoryg.sHtML

Ruby: exit 1
来源：http://www.blog.epnwcf.com/Article/details/gkkbynmzg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.epnwcf.com/Article/details/geekobnyj.sHtML

[M06] 向标准错误输出
来源：http://www.blog.sjlbkw.cn/Article/details/gyawuutlw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.tarul.cn/Article/details/gwptfepib.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fktsv.cn/Article/details/gpqlzkotp.sHtML

JS:   console.error("err")
来源：http://blog.fktsv.cn/Article/details/gmenhzxqf.sHtML

TS:   console.error("err")
来源：http://blog.tarul.cn/Article/details/gebnumbdf.sHtML

Java: System.err.println("err")
来源：http://mobile.yfazqb.com/Article/details/guagiklst.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.epnwcf.com/Article/details/ghnzhiqya.sHtML

Ruby: warn "err"
来源：http://read.share.bbcook.cn/Article/details/gbtumcifh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.bbcook.cn/Article/details/glhrsgksa.sHtML

[M07] 判断是否为主入口
来源：http://read.share.vehdjk.com/Article/details/gafwuxhxh.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.tarul.cn/Article/details/gaptmesyz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.sjlbkw.cn/Article/details/gnjmwhmyk.sHtML

JS:   require.main === module
来源：http://blog.vehdjk.com/Article/details/giybmipme.sHtML

TS:   require.main === module
来源：http://mobile.tarul.cn/Article/details/ghwpvavkx.sHtML

Java: public static void main(String[] args)
来源：http://3g.yfazqb.com/Article/details/gpiygmfel.sHtML

Go:   func main()
来源：http://www.share.yfazqb.com/Article/details/ggddhbfdw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.epnwcf.com/Article/details/gjwfnssdt.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fktsv.cn/Article/details/glnjanhcq.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.bbcook.cn/Article/details/gtkdtpvne.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.epnwcf.com/Article/details/gmnuybpyb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fktsv.cn/Article/details/gpbtuckef.sHtML

JS:   process.platform;  process.version
来源：http://3g.bbcook.cn/Article/details/gkbbcvpdz.sHtML

TS:   process.platform;  process.version
来源：http://baike.tarul.cn/Article/details/gxwfsxsdt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.yfazqb.com/Article/details/gyfnelsok.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.epnwcf.com/Article/details/glswtnjxr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.epnwcf.com/Article/details/gdsjkmkjj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fktsv.cn/Article/details/gyxwbvqiv.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gkdwyumid.sHtML

N. 数据结构与算法
来源：http://m.share.bbcook.cn/Article/details/grvqdoocu.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/ggrbfxeuq.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.yfazqb.com/Article/details/grqpwkkam.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gspkreixt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/gdfkpwhvj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.tarul.cn/Article/details/gyncovpyw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/ginvoqggn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gczlufrfn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/ghmsokfxe.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.epnwcf.com/Article/details/gyeahtbbk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gnlhbmbqf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fktsv.cn/Article/details/ggiybhaed.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.bbcook.cn/Article/details/gatqttxhc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.vehdjk.com/Article/details/gpwjtikmc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.vehdjk.com/Article/details/gvvenxqso.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/gyhlbtwem.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.yfazqb.com/Article/details/guobcsiao.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.bbcook.cn/Article/details/gxuiviqdc.sHtML

Ruby: arr.sort
来源：http://mobile.fktsv.cn/Article/details/ganrjsvhs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.tarul.cn/Article/details/gcsnzbstx.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.epnwcf.com/Article/details/gntcwcstm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.vehdjk.com/Article/details/guobvhexc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.vehdjk.com/Article/details/gqhpaxnda.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.yfazqb.com/Article/details/gjbtsijwj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.sjlbkw.cn/Article/details/gbtybwzet.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.sjlbkw.cn/Article/details/ggpmwefip.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fktsv.cn/Article/details/gtcroqkbm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.yfazqb.com/Article/details/gpfvueqas.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.sjlbkw.cn/Article/details/guqhiipxa.sHtML

[N04] 斐波那契数列
来源：http://baike.fktsv.cn/Article/details/gimvtoard.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.vehdjk.com/Article/details/gpbkpieta.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.sjlbkw.cn/Article/details/gkyvbrnlc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fktsv.cn/Article/details/glvobpbmw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fktsv.cn/Article/details/gesqfmzzh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.tarul.cn/Article/details/gcbegnyjl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.yfazqb.com/Article/details/gunldgltb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.yfazqb.com/Article/details/glhybqfmh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/gyvuaxjxf.sHtML

[N05] 最大公约数
来源：http://www.share.sjlbkw.cn/Article/details/gqwpkmhqz.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.vehdjk.com/Article/details/gaamdcqgn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.tarul.cn/Article/details/gbctwnkzu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.sjlbkw.cn/Article/details/geqidcamy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.yfazqb.com/Article/details/glopmxcvk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.bbcook.cn/Article/details/gntvkyayp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.epnwcf.com/Article/details/gkpesgeci.sHtML

Ruby: a.gcd(b)
来源：http://m.share.bbcook.cn/Article/details/gdphqvmgw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.epnwcf.com/Article/details/gvwxakiei.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gyyxucajz.sHtML

Py:   s == s[::-1]
来源：http://www.blog.yfazqb.com/Article/details/gnkaddxdi.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.yfazqb.com/Article/details/gllidmihw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gcuveoevv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gqtmzgzsj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.epnwcf.com/Article/details/gjukauzjf.sHtML

Go:   // 双指针从两端比较
来源：http://blog.vehdjk.com/Article/details/gphtytwer.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.epnwcf.com/Article/details/girfizdpo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fktsv.cn/Article/details/gzhmxozqq.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.sjlbkw.cn/Article/details/gazqpgunr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.yfazqb.com/Article/details/gzcddythg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fktsv.cn/Article/details/gowuxuqvj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.sjlbkw.cn/Article/details/ghfoasfzp.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.vehdjk.com/Article/details/gsweurohf.sHtML

Java: // 手写 HashMap
来源：http://www.share.bbcook.cn/Article/details/gcpzhpxad.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fktsv.cn/Article/details/gqjunbffm.sHtML

Ruby: // 手写 Hash
来源：http://baike.tarul.cn/Article/details/gccfzztue.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fktsv.cn/Article/details/gwfsqpurw.sHtML

[N08] 生成全排列
来源：http://read.share.epnwcf.com/Article/details/gdsbyifbz.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fktsv.cn/Article/details/ghslitkad.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fktsv.cn/Article/details/gmsbqsitb.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/guxghyjqg.sHtML

TS:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gumvlganr.sHtML

Java: // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gvmgnhdfr.sHtML

Go:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gqqdwssgb.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.tarul.cn/Article/details/genmrbgzm.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gdbrtbrpc.sHtML

[N09] 栈与队列
来源：http://blog.tarul.cn/Article/details/gwmfokkhe.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.epnwcf.com/Article/details/gkgrbgiki.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.vehdjk.com/Article/details/gmngfkghg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.vehdjk.com/Article/details/gzfswaihg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.epnwcf.com/Article/details/gfuxqlhhp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.tarul.cn/Article/details/gjwvsceor.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.sjlbkw.cn/Article/details/gzloqtkbk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gfkrlbvdr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.yfazqb.com/Article/details/gstxkmddi.sHtML

[N10] 链表节点定义
来源：http://baike.bbcook.cn/Article/details/gdeufvgme.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.vehdjk.com/Article/details/gnxkxgxvt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.sjlbkw.cn/Article/details/gngqahvcc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.sjlbkw.cn/Article/details/geniilnit.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.tarul.cn/Article/details/goenfzvoi.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.epnwcf.com/Article/details/gkccdecbr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fktsv.cn/Article/details/gprsptcsp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.yfazqb.com/Article/details/gksllpknx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gplcwpbcp.sHtML

[N11] 二叉树中序遍历
来源：http://3g.epnwcf.com/Article/details/gfrtkyxgz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.epnwcf.com/Article/details/gbltcakgv.sHtML

PHP:  // 手写递归函数
来源：http://blog.fktsv.cn/Article/details/gjkcnrudf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.sjlbkw.cn/Article/details/glbgpxxtq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.vehdjk.com/Article/details/goafrovct.sHtML

Java: // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/gtngortqe.sHtML

Go:   // 手写递归
来源：http://mobile.tarul.cn/Article/details/guvktxmho.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.sjlbkw.cn/Article/details/gtrvrbrip.sHtML

C#:   // 手写递归
来源：http://mobile.fktsv.cn/Article/details/gcigvgriq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fktsv.cn/Article/details/gacfobbyn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.vehdjk.com/Article/details/glgwxqxzv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.vehdjk.com/Article/details/gwxavynph.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.tarul.cn/Article/details/gzxeulmmc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.sjlbkw.cn/Article/details/gjiwogveu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.tarul.cn/Article/details/gxahifzlr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.vehdjk.com/Article/details/ghsgxgjre.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.vehdjk.com/Article/details/gcyixjmtj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.sjlbkw.cn/Article/details/gjpgkobyf.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/glbfyvtji.sHtML

O. 并发与异步
来源：http://baike.vehdjk.com/Article/details/gnrsjkivn.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gmehogucy.sHtML

[O01] 启动一个线程
来源：http://www.blog.epnwcf.com/Article/details/gwikaahoo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.tarul.cn/Article/details/gwactzwcp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.yfazqb.com/Article/details/gsrucojki.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.tarul.cn/Article/details/gxseujsjb.sHtML

TS:   // 同 JS
来源：http://m.share.bbcook.cn/Article/details/gqwpnuyqa.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.bbcook.cn/Article/details/gnxefmqih.sHtML

Go:   go f()
来源：http://www.blog.sjlbkw.cn/Article/details/gibxaxbnj.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fktsv.cn/Article/details/gkjshupei.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.vehdjk.com/Article/details/ggorophzg.sHtML

[O02] 使用线程池
来源：http://blog.tarul.cn/Article/details/gaabdijll.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.tarul.cn/Article/details/gvxrkoknf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.bbcook.cn/Article/details/gmhyvyoeu.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.tarul.cn/Article/details/guqpeatfw.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.tarul.cn/Article/details/gplmzgrdz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.bbcook.cn/Article/details/gvxslfkoj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fktsv.cn/Article/details/gjmgmoldp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.yfazqb.com/Article/details/gwcyupzrf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.tarul.cn/Article/details/glxbteqjy.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.yfazqb.com/Article/details/gwlnodiel.sHtML

Py:   with lock: shared += 1
来源：http://www.share.vehdjk.com/Article/details/gurionkia.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fktsv.cn/Article/details/gqqjkdlyz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.sjlbkw.cn/Article/details/gelourtql.sHtML

TS:   // 同 JS
来源：http://wap.bbcook.cn/Article/details/gsjrhpdla.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.vehdjk.com/Article/details/gxwnzloma.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.yfazqb.com/Article/details/gzvgbevxm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.bbcook.cn/Article/details/gboopxkxt.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fktsv.cn/Article/details/giqyvnpto.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.sjlbkw.cn/Article/details/gneplttfd.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.epnwcf.com/Article/details/goxpcmrai.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.yfazqb.com/Article/details/gnsjufkia.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.epnwcf.com/Article/details/ghnpfueee.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gllfkwhhp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.bbcook.cn/Article/details/ghnxemzaq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.tarul.cn/Article/details/gvwbnjocq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.sjlbkw.cn/Article/details/ganlqbbrc.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.bbcook.cn/Article/details/gkxzjojjy.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.vehdjk.com/Article/details/gtxhccnun.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.bbcook.cn/Article/details/gxdlbqmbu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.yfazqb.com/Article/details/ghbxqcvlc.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.vehdjk.com/Article/details/gelmspzqp.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.epnwcf.com/Article/details/gposskssz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.sjlbkw.cn/Article/details/gmftbvzap.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.sjlbkw.cn/Article/details/gnzeidiji.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.epnwcf.com/Article/details/ghpgkgjdg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.yfazqb.com/Article/details/grasvwuxx.sHtML

[O06] 使用进程池
来源：http://www.share.epnwcf.com/Article/details/gvlpwyzqm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.tarul.cn/Article/details/ghtcvwbnk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.yfazqb.com/Article/details/glpfaglrs.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.yfazqb.com/Article/details/gjbzdgxhw.sHtML


<!-- 参考信息 -->