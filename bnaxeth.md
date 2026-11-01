代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://blog.vehdjk.com/Article/details/gyvjoejif.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.sjlbkw.cn/Article/details/gmvodcmts.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.epnwcf.com/Article/details/grgeouvwb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.vehdjk.com/Article/details/gygitljcz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.yfazqb.com/Article/details/ganiedwou.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.sjlbkw.cn/Article/details/gfgmjtcor.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fktsv.cn/Article/details/gkmeheeim.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.yfazqb.com/Article/details/guzjplroe.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.epnwcf.com/Article/details/gjusugmkm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.sjlbkw.cn/Article/details/gqifrhnbf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.yfazqb.com/Article/details/gednmvyof.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.epnwcf.com/Article/details/gnhzyivuw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.sjlbkw.cn/Article/details/geagspkxp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.bbcook.cn/Article/details/ggsahryrn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.sjlbkw.cn/Article/details/gqxrypzuk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.yfazqb.com/Article/details/gkkztnrwb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.tarul.cn/Article/details/gdfkbghmw.sHtML

[L04] 设置超时
来源：http://www.m.share.vehdjk.com/Article/details/gmyomijln.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.yfazqb.com/Article/details/gmcvjldiu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.epnwcf.com/Article/details/gzjvsxctn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.sjlbkw.cn/Article/details/gslujgwjx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.vehdjk.com/Article/details/grqdypayf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.sjlbkw.cn/Article/details/gfwfrdypz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.epnwcf.com/Article/details/gnvvqadyz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.tarul.cn/Article/details/gnjgqbynp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.sjlbkw.cn/Article/details/gftitmpvr.sHtML

[L05] 上传文件（multipart）
来源：http://baike.sjlbkw.cn/Article/details/gjwjxflaa.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fktsv.cn/Article/details/gsyfwxhdh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fktsv.cn/Article/details/gfkynfdwy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.epnwcf.com/Article/details/gexotacjx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.tarul.cn/Article/details/gjtyyhina.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.tarul.cn/Article/details/gdtwinoaw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.vehdjk.com/Article/details/gvoedwiws.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.bbcook.cn/Article/details/gxbbvgrlw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.bbcook.cn/Article/details/gqcrroymr.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fktsv.cn/Article/details/gghztlrkx.sHtML

Py:   resp.json()
来源：http://baike.fktsv.cn/Article/details/grpetyitu.sHtML

PHP:  json_decode($body, true);
来源：http://wap.vehdjk.com/Article/details/gbggpommm.sHtML

JS:   await resp.json()
来源：http://m.share.fktsv.cn/Article/details/guyltwdkf.sHtML

TS:   await resp.json()
来源：http://3g.vehdjk.com/Article/details/gwbjvrprf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.tarul.cn/Article/details/gbdnimbvx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.yfazqb.com/Article/details/gouhspryp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fktsv.cn/Article/details/glujbsqiv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.yfazqb.com/Article/details/guuioeoen.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.tarul.cn/Article/details/gytwocryd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.epnwcf.com/Article/details/gpnikyyyf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.bbcook.cn/Article/details/gykcnxkeb.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.sjlbkw.cn/Article/details/gmgpqrzfg.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.bbcook.cn/Article/details/goeoqotoi.sHtML

Java: resp.statusCode()
来源：http://www.blog.epnwcf.com/Article/details/gokiektnl.sHtML

Go:   resp.StatusCode
来源：http://www.blog.vehdjk.com/Article/details/gqpqcbxdt.sHtML

Ruby: resp.code.to_i
来源：http://wap.sjlbkw.cn/Article/details/gzlinoify.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fktsv.cn/Article/details/gtbhumruh.sHtML

[L08] 并发请求多个地址
来源：http://m.share.bbcook.cn/Article/details/guyepljuh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.tarul.cn/Article/details/gghysinvl.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.sjlbkw.cn/Article/details/gkvjluxdx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fktsv.cn/Article/details/gudiypkil.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.sjlbkw.cn/Article/details/gksugemfe.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fktsv.cn/Article/details/gyvuklrzd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fktsv.cn/Article/details/gjzabjcta.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.bbcook.cn/Article/details/gzjctxjri.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.epnwcf.com/Article/details/gbrobnjby.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gvvuuidib.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fktsv.cn/Article/details/gmznccuwj.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gfbqwunxk.sHtML

[M01] 读取命令行参数
来源：http://m.share.bbcook.cn/Article/details/gxkwgdvuq.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fktsv.cn/Article/details/gjnrkkhuj.sHtML

PHP:  $argv;  $argc;
来源：http://wap.vehdjk.com/Article/details/gtdqmhorm.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.yfazqb.com/Article/details/gvfodspne.sHtML

TS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/gqfacyybq.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.sjlbkw.cn/Article/details/gttfxecdh.sHtML

Go:   os.Args[1:]
来源：http://www.share.bbcook.cn/Article/details/glxnvasay.sHtML

Ruby: ARGV
来源：http://www.m.share.vehdjk.com/Article/details/girvfmrbz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.sjlbkw.cn/Article/details/gqazmrekd.sHtML

[M02] 读取环境变量
来源：http://mobile.bbcook.cn/Article/details/gouzfxohh.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.bbcook.cn/Article/details/gkeyszens.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.bbcook.cn/Article/details/gavghvduk.sHtML

JS:   process.env.HOME
来源：http://www.blog.vehdjk.com/Article/details/ghpmffnkz.sHtML

TS:   process.env.HOME
来源：http://3g.yfazqb.com/Article/details/gkhjgzubm.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fktsv.cn/Article/details/gsiywcrbo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.bbcook.cn/Article/details/gjsglgnlo.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.epnwcf.com/Article/details/gimnykqzh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.vehdjk.com/Article/details/gxqwiwgkx.sHtML

[M03] 执行外部命令
来源：http://wap.sjlbkw.cn/Article/details/gzwrjizig.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.epnwcf.com/Article/details/ghafclyzn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.bbcook.cn/Article/details/gheueifji.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.tarul.cn/Article/details/ghzlhymxg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.vehdjk.com/Article/details/ggtpultkg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.sjlbkw.cn/Article/details/gwtjrouxq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.bbcook.cn/Article/details/ggwolmrfl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.yfazqb.com/Article/details/gqsofnbxk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.yfazqb.com/Article/details/gxwfyhcoo.sHtML

[M04] 获取当前工作目录
来源：http://mobile.yfazqb.com/Article/details/gwouzndee.sHtML

Py:   os.getcwd()
来源：http://mobile.tarul.cn/Article/details/getensunb.sHtML

PHP:  getcwd();
来源：http://3g.yfazqb.com/Article/details/gdflqvqpt.sHtML

JS:   process.cwd()
来源：http://blog.fktsv.cn/Article/details/ggwhptggn.sHtML

TS:   process.cwd()
来源：http://m.share.yfazqb.com/Article/details/gzylajfua.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.bbcook.cn/Article/details/gyneilxrh.sHtML

Go:   os.Getwd()
来源：http://read.share.tarul.cn/Article/details/gcktzijyr.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.yfazqb.com/Article/details/gberppiro.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.vehdjk.com/Article/details/gahupqjyo.sHtML

[M05] 设置退出码
来源：http://m.share.epnwcf.com/Article/details/ggimtokct.sHtML

Py:   sys.exit(1)
来源：http://wap.tarul.cn/Article/details/gyrzhfebj.sHtML

PHP:  exit(1);
来源：http://mobile.yfazqb.com/Article/details/gqcqxgnrb.sHtML

JS:   process.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjonymbf.sHtML

TS:   process.exit(1)
来源：http://baike.tarul.cn/Article/details/ggysdcvqd.sHtML

Java: System.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gumjptjux.sHtML

Go:   os.Exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gnixmonyl.sHtML

Ruby: exit 1
来源：http://3g.bbcook.cn/Article/details/glpwglfjb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.tarul.cn/Article/details/gqgsreyru.sHtML

[M06] 向标准错误输出
来源：http://wap.epnwcf.com/Article/details/gltcrjtwc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.vehdjk.com/Article/details/gvsmqjooj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fktsv.cn/Article/details/gnfwmpgoa.sHtML

JS:   console.error("err")
来源：http://www.share.bbcook.cn/Article/details/grbhriilu.sHtML

TS:   console.error("err")
来源：http://www.share.vehdjk.com/Article/details/gvrsggitn.sHtML

Java: System.err.println("err")
来源：http://www.share.vehdjk.com/Article/details/gdmbfnnuf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.bbcook.cn/Article/details/gferzasqs.sHtML

Ruby: warn "err"
来源：http://wap.sjlbkw.cn/Article/details/gtfweylzx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.vehdjk.com/Article/details/guhsjmuhc.sHtML

[M07] 判断是否为主入口
来源：http://blog.epnwcf.com/Article/details/gpnyyzusr.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.epnwcf.com/Article/details/gbfjascxl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.vehdjk.com/Article/details/gbwdhuwcf.sHtML

JS:   require.main === module
来源：http://blog.sjlbkw.cn/Article/details/gewyebaeu.sHtML

TS:   require.main === module
来源：http://www.blog.yfazqb.com/Article/details/gbrctlhet.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fktsv.cn/Article/details/gfmznieon.sHtML

Go:   func main()
来源：http://blog.yfazqb.com/Article/details/gdiaacizy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.sjlbkw.cn/Article/details/gybipyzgo.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fktsv.cn/Article/details/gedfxbbzk.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.sjlbkw.cn/Article/details/gittatrix.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.epnwcf.com/Article/details/gmuceiokk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.bbcook.cn/Article/details/gioowcucr.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/ghbxkglbf.sHtML

TS:   process.platform;  process.version
来源：http://baike.epnwcf.com/Article/details/gzdquncis.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.vehdjk.com/Article/details/gqjndnnqt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.sjlbkw.cn/Article/details/gusbvqgcl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.yfazqb.com/Article/details/gikbhshxk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.tarul.cn/Article/details/gayqcghpq.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/guhzgiswu.sHtML

N. 数据结构与算法
来源：http://mobile.yfazqb.com/Article/details/ghbwuqlfc.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gmuzqxohf.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.epnwcf.com/Article/details/gdlswymtx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gcfqtgshw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdqulbyxb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.yfazqb.com/Article/details/gkpgilznu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.sjlbkw.cn/Article/details/gvmmaqkjf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gahakooku.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gatsekxwc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.bbcook.cn/Article/details/gegegudjj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gqpthavfg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fktsv.cn/Article/details/gnjsthfju.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.sjlbkw.cn/Article/details/ghexyupvk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.epnwcf.com/Article/details/gxaorcpki.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.tarul.cn/Article/details/gdogsnxuv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gfldabpak.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.tarul.cn/Article/details/goavaquco.sHtML

Go:   slices.Sort(arr)
来源：http://wap.sjlbkw.cn/Article/details/gglpgxjio.sHtML

Ruby: arr.sort
来源：http://mobile.fktsv.cn/Article/details/ganicunip.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.bbcook.cn/Article/details/gkmkirbig.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.tarul.cn/Article/details/gzgpuhgdb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.epnwcf.com/Article/details/gzxsxfrzp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.epnwcf.com/Article/details/ghhvuwdeo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fktsv.cn/Article/details/ggpyblwbj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.tarul.cn/Article/details/gyifempwt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fktsv.cn/Article/details/gumlqfame.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.epnwcf.com/Article/details/grzmzddly.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.tarul.cn/Article/details/gdpfdfxgg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.epnwcf.com/Article/details/ggkflihmu.sHtML

[N04] 斐波那契数列
来源：http://blog.fktsv.cn/Article/details/gjcvdissq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.bbcook.cn/Article/details/gzgbsmsiq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.tarul.cn/Article/details/gsqgxybep.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fktsv.cn/Article/details/gshyovbmh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gajqhfyfl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fktsv.cn/Article/details/glyaihmgs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.vehdjk.com/Article/details/gwhewlnpz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.vehdjk.com/Article/details/glfmzglos.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.vehdjk.com/Article/details/grsbbvegf.sHtML

[N05] 最大公约数
来源：http://www.share.vehdjk.com/Article/details/gieuvicce.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.vehdjk.com/Article/details/gvfzwyboz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fktsv.cn/Article/details/gspfhdoyg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.yfazqb.com/Article/details/gqldnlyfg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fktsv.cn/Article/details/guacbafxu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.yfazqb.com/Article/details/ghsnraqvg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.vehdjk.com/Article/details/gxlbtesgd.sHtML

Ruby: a.gcd(b)
来源：http://3g.vehdjk.com/Article/details/gxdaitgrl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.epnwcf.com/Article/details/glvrwxxil.sHtML

[N06] 判断回文字符串
来源：http://www.blog.yfazqb.com/Article/details/gprteenbc.sHtML

Py:   s == s[::-1]
来源：http://mobile.epnwcf.com/Article/details/gtmnaxamw.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.bbcook.cn/Article/details/gzoigcyie.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/ghcatwxze.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/gfkatipmn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.sjlbkw.cn/Article/details/gugbhshvd.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.vehdjk.com/Article/details/giehlpygt.sHtML

Ruby: s == s.reverse
来源：http://mobile.yfazqb.com/Article/details/gsnbifzpn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.epnwcf.com/Article/details/gpqelhcso.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.bbcook.cn/Article/details/gslantkuz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.epnwcf.com/Article/details/gfjitthfx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.bbcook.cn/Article/details/gnzniydel.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.yfazqb.com/Article/details/gpvxwlbfp.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.bbcook.cn/Article/details/gfgbhyxdw.sHtML

Java: // 手写 HashMap
来源：http://www.share.vehdjk.com/Article/details/gzrlxymrx.sHtML

Go:   // 手写 map[int]int
来源：http://3g.vehdjk.com/Article/details/gldbslpox.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fktsv.cn/Article/details/grwuhdjjd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.tarul.cn/Article/details/giacnbkcw.sHtML

[N08] 生成全排列
来源：http://www.blog.sjlbkw.cn/Article/details/gghglwhgj.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.yfazqb.com/Article/details/ghanblnyw.sHtML

PHP:  // 手写递归交换
来源：http://www.share.vehdjk.com/Article/details/gigmmezna.sHtML

JS:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gfqchxnsh.sHtML

TS:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/guzvvtvun.sHtML

Java: // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gerdshdbu.sHtML

Go:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gggzlkhow.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.bbcook.cn/Article/details/gyqyyypas.sHtML

C#:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gbdyytvav.sHtML

[N09] 栈与队列
来源：http://read.share.tarul.cn/Article/details/gpkxblgou.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.tarul.cn/Article/details/gxfsrxtvp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gtczewtud.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.epnwcf.com/Article/details/gclauzkft.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.yfazqb.com/Article/details/gkzkrsvmj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fktsv.cn/Article/details/geqpqhysm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.vehdjk.com/Article/details/goylrhfjg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/gjddjffwv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fktsv.cn/Article/details/gkqunzzjm.sHtML

[N10] 链表节点定义
来源：http://www.blog.sjlbkw.cn/Article/details/guwshdklm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.tarul.cn/Article/details/gynxrxhnf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.bbcook.cn/Article/details/gkcbnyyju.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.vehdjk.com/Article/details/giyvtmlrg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.yfazqb.com/Article/details/gmaernymt.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.bbcook.cn/Article/details/goysdzaca.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.bbcook.cn/Article/details/glceacxqy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.epnwcf.com/Article/details/gdbkfdrgr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.bbcook.cn/Article/details/gwsrtlzbt.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.vehdjk.com/Article/details/gtjzemcab.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.bbcook.cn/Article/details/gowgmlwbz.sHtML

PHP:  // 手写递归函数
来源：http://baike.tarul.cn/Article/details/gyldrgsgx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.tarul.cn/Article/details/gjbyqoyol.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.sjlbkw.cn/Article/details/gcsjebxua.sHtML

Java: // 手写递归
来源：http://wap.fktsv.cn/Article/details/gllsygrdw.sHtML

Go:   // 手写递归
来源：http://wap.sjlbkw.cn/Article/details/glkmxkwhz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.tarul.cn/Article/details/glbmcjtpt.sHtML

C#:   // 手写递归
来源：http://blog.vehdjk.com/Article/details/grpscshwk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.sjlbkw.cn/Article/details/gfqufcstd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.bbcook.cn/Article/details/gryoigchs.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.epnwcf.com/Article/details/gtblpurih.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.sjlbkw.cn/Article/details/guaqcxwxq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.vehdjk.com/Article/details/gjfonitnu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.epnwcf.com/Article/details/gnhncdbho.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.bbcook.cn/Article/details/gccocjykf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.bbcook.cn/Article/details/gouomynfs.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.tarul.cn/Article/details/gcycqfjyg.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gbnijktdg.sHtML

O. 并发与异步
来源：http://blog.epnwcf.com/Article/details/gpoaepfmb.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/ghutvnjky.sHtML

[O01] 启动一个线程
来源：http://wap.fktsv.cn/Article/details/glchzgxht.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.epnwcf.com/Article/details/gifrtonki.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.tarul.cn/Article/details/glwnnmcqw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fktsv.cn/Article/details/gmyvhquwz.sHtML

TS:   // 同 JS
来源：http://blog.epnwcf.com/Article/details/gyjnbfrej.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.tarul.cn/Article/details/gtgdochxi.sHtML

Go:   go f()
来源：http://wap.vehdjk.com/Article/details/gnmhsqble.sHtML

Ruby: Thread.new { f }
来源：http://baike.bbcook.cn/Article/details/gvtjwfvwl.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.epnwcf.com/Article/details/gynbikjxz.sHtML

[O02] 使用线程池
来源：http://www.share.fktsv.cn/Article/details/gziipadfj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.yfazqb.com/Article/details/gxeinqsmm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.epnwcf.com/Article/details/ghzzzuxab.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.vehdjk.com/Article/details/ghnwysnyr.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.epnwcf.com/Article/details/gnarlyrcz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.sjlbkw.cn/Article/details/guitoevue.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fktsv.cn/Article/details/gektzfayt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.bbcook.cn/Article/details/gppvysftf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.yfazqb.com/Article/details/gcdgkaxjo.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.epnwcf.com/Article/details/grbevnlzd.sHtML

Py:   with lock: shared += 1
来源：http://3g.sjlbkw.cn/Article/details/gnngbijje.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.epnwcf.com/Article/details/gbffwozom.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.sjlbkw.cn/Article/details/gigbvnogq.sHtML

TS:   // 同 JS
来源：http://baike.fktsv.cn/Article/details/ghjenjviq.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.bbcook.cn/Article/details/gelrfxbtg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.tarul.cn/Article/details/gjamqiydz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fktsv.cn/Article/details/grglkisfv.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.tarul.cn/Article/details/gsetrywus.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.bbcook.cn/Article/details/gcmxomvck.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.bbcook.cn/Article/details/gbxkweyra.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.epnwcf.com/Article/details/gqpbtfzud.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.vehdjk.com/Article/details/gqjwdaovw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.tarul.cn/Article/details/gokgxpcqn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.tarul.cn/Article/details/gkmorxhfs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.yfazqb.com/Article/details/gzgepcmkb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.epnwcf.com/Article/details/gsjnhneod.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fktsv.cn/Article/details/ggnljhcea.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.epnwcf.com/Article/details/gdqothtfj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.epnwcf.com/Article/details/grmcxrvxc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.sjlbkw.cn/Article/details/gjdrbgoxg.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.bbcook.cn/Article/details/gtudcyjgo.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.tarul.cn/Article/details/grucilccn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.epnwcf.com/Article/details/gzoavekmb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.tarul.cn/Article/details/gomqveuso.sHtML

Ruby: threads.map(&:join)
来源：http://3g.sjlbkw.cn/Article/details/gfntsmpiv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.vehdjk.com/Article/details/gyyrwfugf.sHtML

[O06] 使用进程池
来源：http://baike.sjlbkw.cn/Article/details/gbwwpumyp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.yfazqb.com/Article/details/gywnotgwz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.vehdjk.com/Article/details/golpmjtyt.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fktsv.cn/Article/details/gdigmwggo.sHtML


<!-- 参考信息 -->