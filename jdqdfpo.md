代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://blog.tarul.cn/Article/details/gjjmajrfp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.vehdjk.com/Article/details/gamejaerp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.yfazqb.com/Article/details/gcrrtkmae.sHtML

[L02] 发送 POST JSON
来源：http://m.share.bbcook.cn/Article/details/gxvqdmfsa.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.vehdjk.com/Article/details/gcxliztih.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.yfazqb.com/Article/details/grwpinqwy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.tarul.cn/Article/details/gsnrmmhry.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.tarul.cn/Article/details/gunkibnyv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.tarul.cn/Article/details/gcfedhssj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.sjlbkw.cn/Article/details/gvnekxrfc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.yfazqb.com/Article/details/gfqnzwngp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fktsv.cn/Article/details/gndpwwonz.sHtML

[L03] 设置自定义请求头
来源：http://www.share.tarul.cn/Article/details/gwyidoqxv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.epnwcf.com/Article/details/gocmtgpre.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.sjlbkw.cn/Article/details/govhndaxu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.sjlbkw.cn/Article/details/gaxegxzfx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.yfazqb.com/Article/details/gavcfwaky.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.yfazqb.com/Article/details/gawqohdol.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fktsv.cn/Article/details/gfdhktjdo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fktsv.cn/Article/details/ghhwitdmk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.yfazqb.com/Article/details/gvkohgjlg.sHtML

[L04] 设置超时
来源：http://www.m.share.fktsv.cn/Article/details/gtdisyfei.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fktsv.cn/Article/details/gomfunfpz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.tarul.cn/Article/details/gptpvgyrp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fktsv.cn/Article/details/gohdsdasn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.yfazqb.com/Article/details/guynpjjee.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.yfazqb.com/Article/details/ginigxuyy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.tarul.cn/Article/details/grwbcsjzp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.bbcook.cn/Article/details/gcgyvwxai.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.yfazqb.com/Article/details/giqwoqzyr.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.bbcook.cn/Article/details/gcnerphzp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.bbcook.cn/Article/details/goryeprln.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.epnwcf.com/Article/details/gtkwolqlm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fktsv.cn/Article/details/glvniqzyf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.bbcook.cn/Article/details/gdizljkin.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.epnwcf.com/Article/details/gtriearth.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.sjlbkw.cn/Article/details/gxgjgygwf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.epnwcf.com/Article/details/gloctwtrj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.yfazqb.com/Article/details/gqsumevxf.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.vehdjk.com/Article/details/gwsqfzqzc.sHtML

Py:   resp.json()
来源：http://baike.fktsv.cn/Article/details/grijlowtt.sHtML

PHP:  json_decode($body, true);
来源：http://blog.epnwcf.com/Article/details/gfdoyatrg.sHtML

JS:   await resp.json()
来源：http://3g.bbcook.cn/Article/details/grrhuqogd.sHtML

TS:   await resp.json()
来源：http://mobile.epnwcf.com/Article/details/gpvnvbadz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fktsv.cn/Article/details/gmdrbjbzp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.vehdjk.com/Article/details/githlewah.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.yfazqb.com/Article/details/gengssfnk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.yfazqb.com/Article/details/gyrsvvfjz.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.tarul.cn/Article/details/gbrttrhxw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.bbcook.cn/Article/details/gwrwxwvbd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.yfazqb.com/Article/details/gyvzveqki.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.vehdjk.com/Article/details/gjloydcvg.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.yfazqb.com/Article/details/giiwuhetw.sHtML

Java: resp.statusCode()
来源：http://baike.sjlbkw.cn/Article/details/gskxoznqt.sHtML

Go:   resp.StatusCode
来源：http://read.share.epnwcf.com/Article/details/gppplcaje.sHtML

Ruby: resp.code.to_i
来源：http://wap.bbcook.cn/Article/details/gbawmwlgv.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fktsv.cn/Article/details/gdznfguuc.sHtML

[L08] 并发请求多个地址
来源：http://baike.sjlbkw.cn/Article/details/ghmsoytvy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.vehdjk.com/Article/details/gxqdzdutt.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.bbcook.cn/Article/details/gtexqjlbg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.tarul.cn/Article/details/ggafqvhey.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.sjlbkw.cn/Article/details/gaxnugkzf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.sjlbkw.cn/Article/details/glpiuqrxu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.bbcook.cn/Article/details/gdvdgdfdg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.sjlbkw.cn/Article/details/ghcbyiazi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.tarul.cn/Article/details/gbehbziqg.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gllhewxpn.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fktsv.cn/Article/details/gyzzratbg.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gslmxafuq.sHtML

[M01] 读取命令行参数
来源：http://baike.epnwcf.com/Article/details/gmnqpihuy.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.tarul.cn/Article/details/gmptqldpr.sHtML

PHP:  $argv;  $argc;
来源：http://blog.bbcook.cn/Article/details/gtbvtkubb.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.epnwcf.com/Article/details/glycaanol.sHtML

TS:   process.argv.slice(2)
来源：http://blog.vehdjk.com/Article/details/gnmdgfcpg.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fktsv.cn/Article/details/gdtrrognf.sHtML

Go:   os.Args[1:]
来源：http://mobile.yfazqb.com/Article/details/gfmguqakw.sHtML

Ruby: ARGV
来源：http://mobile.vehdjk.com/Article/details/giveztned.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.vehdjk.com/Article/details/guamgwlqc.sHtML

[M02] 读取环境变量
来源：http://www.blog.bbcook.cn/Article/details/govpmwlgt.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gdbfxmmsi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.vehdjk.com/Article/details/gjoiajhnr.sHtML

JS:   process.env.HOME
来源：http://blog.epnwcf.com/Article/details/gyuuissdn.sHtML

TS:   process.env.HOME
来源：http://read.share.tarul.cn/Article/details/gckgbxfys.sHtML

Java: System.getenv("HOME")
来源：http://blog.yfazqb.com/Article/details/gmipqjwfy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.vehdjk.com/Article/details/gheufqeeo.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.sjlbkw.cn/Article/details/gbbcfojrx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.bbcook.cn/Article/details/goxkccjhu.sHtML

[M03] 执行外部命令
来源：http://m.share.epnwcf.com/Article/details/gredxkouj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.yfazqb.com/Article/details/ggwimosys.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.epnwcf.com/Article/details/ghmqucrck.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjnpwqwrx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.yfazqb.com/Article/details/gkehmgqkm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.yfazqb.com/Article/details/gchphunmj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.yfazqb.com/Article/details/gzcicerrm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.epnwcf.com/Article/details/gdpddzlig.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.sjlbkw.cn/Article/details/gbtbccahi.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.tarul.cn/Article/details/gdouavppq.sHtML

Py:   os.getcwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gskozjtye.sHtML

PHP:  getcwd();
来源：http://baike.epnwcf.com/Article/details/gstpwpunw.sHtML

JS:   process.cwd()
来源：http://baike.vehdjk.com/Article/details/glgrzmsdm.sHtML

TS:   process.cwd()
来源：http://www.share.vehdjk.com/Article/details/ghpekgegi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.vehdjk.com/Article/details/gslaigujd.sHtML

Go:   os.Getwd()
来源：http://mobile.vehdjk.com/Article/details/gzpmqzydk.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.bbcook.cn/Article/details/gknpkqwtz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.epnwcf.com/Article/details/gvdxrvrpd.sHtML

[M05] 设置退出码
来源：http://read.share.tarul.cn/Article/details/gjvfgwlys.sHtML

Py:   sys.exit(1)
来源：http://wap.tarul.cn/Article/details/grzcvoopk.sHtML

PHP:  exit(1);
来源：http://blog.fktsv.cn/Article/details/gopcguvyy.sHtML

JS:   process.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gkdniidci.sHtML

TS:   process.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gkqlzyshb.sHtML

Java: System.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gkbujwpnw.sHtML

Go:   os.Exit(1)
来源：http://www.share.epnwcf.com/Article/details/gsgizlphe.sHtML

Ruby: exit 1
来源：http://baike.vehdjk.com/Article/details/gukgjlxdj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fktsv.cn/Article/details/giwrqngdq.sHtML

[M06] 向标准错误输出
来源：http://m.share.tarul.cn/Article/details/gahpsfxib.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.vehdjk.com/Article/details/gzujwckvm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.vehdjk.com/Article/details/ggntgqsom.sHtML

JS:   console.error("err")
来源：http://blog.epnwcf.com/Article/details/gqswlqcga.sHtML

TS:   console.error("err")
来源：http://www.share.tarul.cn/Article/details/gvtnhbgcp.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fktsv.cn/Article/details/glgyrdhzr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.epnwcf.com/Article/details/gfsykpqtq.sHtML

Ruby: warn "err"
来源：http://www.blog.tarul.cn/Article/details/glymlfwru.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.bbcook.cn/Article/details/gyhgnddgy.sHtML

[M07] 判断是否为主入口
来源：http://blog.tarul.cn/Article/details/grpvjsbjx.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.epnwcf.com/Article/details/gjohzstqs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fktsv.cn/Article/details/gtpbtqjoc.sHtML

JS:   require.main === module
来源：http://www.blog.sjlbkw.cn/Article/details/gzpcgqfpg.sHtML

TS:   require.main === module
来源：http://wap.yfazqb.com/Article/details/gdrpvfceu.sHtML

Java: public static void main(String[] args)
来源：http://m.share.yfazqb.com/Article/details/gkxalehpd.sHtML

Go:   func main()
来源：http://m.share.yfazqb.com/Article/details/gbeznblur.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.bbcook.cn/Article/details/gnegpwsjo.sHtML

C#:   static void Main(string[] args)
来源：http://3g.bbcook.cn/Article/details/gotyaailo.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.tarul.cn/Article/details/gkwxtgtir.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.tarul.cn/Article/details/gugcyuoyh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.sjlbkw.cn/Article/details/gisiaezvq.sHtML

JS:   process.platform;  process.version
来源：http://read.share.epnwcf.com/Article/details/gcggguemr.sHtML

TS:   process.platform;  process.version
来源：http://wap.yfazqb.com/Article/details/gtqtdbapk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.vehdjk.com/Article/details/genvsczwg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.epnwcf.com/Article/details/gjyxnawgf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.epnwcf.com/Article/details/glicaljjt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fktsv.cn/Article/details/gkgxftjuz.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/ggptrlvya.sHtML

N. 数据结构与算法
来源：http://read.share.bbcook.cn/Article/details/gbojqjbnt.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gpqxlffef.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.tarul.cn/Article/details/gwvdcaqzt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.tarul.cn/Article/details/gqfzcxsot.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/grsbhsuxb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.yfazqb.com/Article/details/gsqtmrxqy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.epnwcf.com/Article/details/gupojhbmh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.tarul.cn/Article/details/gttkfjftg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gramrdaom.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.sjlbkw.cn/Article/details/gtatuneji.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.tarul.cn/Article/details/gsccbkjgd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.bbcook.cn/Article/details/gzpthptdr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.bbcook.cn/Article/details/gxjcoggdg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.epnwcf.com/Article/details/glwwrzter.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fktsv.cn/Article/details/gmaaznmlc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.bbcook.cn/Article/details/gnuaiekvx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.vehdjk.com/Article/details/gdmsylvzt.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.sjlbkw.cn/Article/details/geonogxzx.sHtML

Ruby: arr.sort
来源：http://www.blog.yfazqb.com/Article/details/gztygbwci.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fktsv.cn/Article/details/goufinypv.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.sjlbkw.cn/Article/details/grvizzdwj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.bbcook.cn/Article/details/gipkcjfol.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.bbcook.cn/Article/details/gotiabqrz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.epnwcf.com/Article/details/gliwfaydg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.sjlbkw.cn/Article/details/gozmuyiqh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.yfazqb.com/Article/details/gnslrvhdn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fktsv.cn/Article/details/gentociol.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.tarul.cn/Article/details/gkjgphgeo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.tarul.cn/Article/details/gyfobyxnj.sHtML

[N04] 斐波那契数列
来源：http://baike.vehdjk.com/Article/details/gewmlahwt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.bbcook.cn/Article/details/gpzalvkax.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.vehdjk.com/Article/details/gyomowoby.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/gblploeju.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.epnwcf.com/Article/details/ggmbtdwbi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.vehdjk.com/Article/details/gewalyisk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.yfazqb.com/Article/details/ghqarqnhd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.bbcook.cn/Article/details/giblvgsbc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.vehdjk.com/Article/details/gaehfcajz.sHtML

[N05] 最大公约数
来源：http://3g.bbcook.cn/Article/details/gkmphpzgl.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.epnwcf.com/Article/details/gdvczgixc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.bbcook.cn/Article/details/gwzyozrzo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.yfazqb.com/Article/details/gegzokzgo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.sjlbkw.cn/Article/details/gediakovp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.tarul.cn/Article/details/gnitxivrb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fktsv.cn/Article/details/gvdvjtyvp.sHtML

Ruby: a.gcd(b)
来源：http://m.share.bbcook.cn/Article/details/gofinumlx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.vehdjk.com/Article/details/ghztvopvn.sHtML

[N06] 判断回文字符串
来源：http://wap.epnwcf.com/Article/details/grrzbplfu.sHtML

Py:   s == s[::-1]
来源：http://mobile.bbcook.cn/Article/details/gbuapiqeq.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.bbcook.cn/Article/details/gymhzrptc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gbztiahxm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fktsv.cn/Article/details/gpaebelkj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.vehdjk.com/Article/details/gslrpcmgf.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.epnwcf.com/Article/details/ggwzbvahn.sHtML

Ruby: s == s.reverse
来源：http://read.share.bbcook.cn/Article/details/gofsapcte.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.yfazqb.com/Article/details/guuoamakk.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.yfazqb.com/Article/details/gydwguzvn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.epnwcf.com/Article/details/gocatioya.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.vehdjk.com/Article/details/gvrvuvfnt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.tarul.cn/Article/details/gjqrfurvk.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.epnwcf.com/Article/details/gmgxwflxk.sHtML

Java: // 手写 HashMap
来源：http://read.share.vehdjk.com/Article/details/gneqrppuo.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.sjlbkw.cn/Article/details/gdkpieheh.sHtML

Ruby: // 手写 Hash
来源：http://m.share.epnwcf.com/Article/details/gdspplykg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.sjlbkw.cn/Article/details/gxfeeblrx.sHtML

[N08] 生成全排列
来源：http://wap.sjlbkw.cn/Article/details/gzalgwmvi.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gjkgyqdbw.sHtML

PHP:  // 手写递归交换
来源：http://baike.vehdjk.com/Article/details/gidwadgpk.sHtML

JS:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gqnliljfc.sHtML

TS:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gnxngtwnr.sHtML

Java: // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/glvzmczly.sHtML

Go:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gpurxghpn.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.vehdjk.com/Article/details/gyieclfam.sHtML

C#:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gqjxuuyhi.sHtML

[N09] 栈与队列
来源：http://baike.vehdjk.com/Article/details/gacpyrbvg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.bbcook.cn/Article/details/grpxvrqkx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.bbcook.cn/Article/details/grxigslic.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.sjlbkw.cn/Article/details/gtamivcgi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.tarul.cn/Article/details/gbjqpentb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.bbcook.cn/Article/details/gvaqtgwxn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.tarul.cn/Article/details/gqjwvamro.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.tarul.cn/Article/details/gqrpvfnho.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.epnwcf.com/Article/details/gtgpzusqa.sHtML

[N10] 链表节点定义
来源：http://read.share.sjlbkw.cn/Article/details/gnydvcowe.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fktsv.cn/Article/details/goidowawp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.epnwcf.com/Article/details/grycwsspj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.bbcook.cn/Article/details/gjlawrpke.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.sjlbkw.cn/Article/details/ggskpwfdh.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.epnwcf.com/Article/details/gwctysqim.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.vehdjk.com/Article/details/gbwjbxhpy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fktsv.cn/Article/details/gtoisamns.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.sjlbkw.cn/Article/details/gbmkvcqrp.sHtML

[N11] 二叉树中序遍历
来源：http://blog.bbcook.cn/Article/details/gscgmhfzp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.epnwcf.com/Article/details/gognmtkcz.sHtML

PHP:  // 手写递归函数
来源：http://baike.yfazqb.com/Article/details/gmdxknbwt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.yfazqb.com/Article/details/gzssffciv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.tarul.cn/Article/details/gsroofyzv.sHtML

Java: // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/gbviseafu.sHtML

Go:   // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/gkshotjbu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.sjlbkw.cn/Article/details/gxfxenodn.sHtML

C#:   // 手写递归
来源：http://baike.vehdjk.com/Article/details/gierfhvhz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fktsv.cn/Article/details/gtlwsirhb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.tarul.cn/Article/details/gsogfccpc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.epnwcf.com/Article/details/gdbeoxmzu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.sjlbkw.cn/Article/details/gvqrxojmw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.vehdjk.com/Article/details/gijeotqxg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.bbcook.cn/Article/details/gneksgwnq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.vehdjk.com/Article/details/gmfhwgnub.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fktsv.cn/Article/details/gemfeabkz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.vehdjk.com/Article/details/gftidlgto.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gcpbxzxxk.sHtML

O. 并发与异步
来源：http://www.share.yfazqb.com/Article/details/gdexvofho.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gxgmkyyaq.sHtML

[O01] 启动一个线程
来源：http://read.share.sjlbkw.cn/Article/details/gehsydzof.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.yfazqb.com/Article/details/ghbxxfwiv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.yfazqb.com/Article/details/gvjikqhvd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.bbcook.cn/Article/details/gizdvsbvw.sHtML

TS:   // 同 JS
来源：http://3g.yfazqb.com/Article/details/gudlmfxnb.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.bbcook.cn/Article/details/gwczbmrxv.sHtML

Go:   go f()
来源：http://www.share.sjlbkw.cn/Article/details/gqgwkmbxx.sHtML

Ruby: Thread.new { f }
来源：http://baike.tarul.cn/Article/details/gfocnlsye.sHtML

C#:   Task.Run(() => F());
来源：http://blog.sjlbkw.cn/Article/details/gtypwdvgm.sHtML

[O02] 使用线程池
来源：http://read.share.yfazqb.com/Article/details/gcliwiqcs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.yfazqb.com/Article/details/guynrecbc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.tarul.cn/Article/details/gbsskibek.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.sjlbkw.cn/Article/details/gulaphkwj.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fktsv.cn/Article/details/giqcuizcw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.yfazqb.com/Article/details/gpcqdsvsg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fktsv.cn/Article/details/giynulhmb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.epnwcf.com/Article/details/gxaweomtm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.epnwcf.com/Article/details/gxwsvqsse.sHtML

[O03] 加锁保护共享数据
来源：http://3g.epnwcf.com/Article/details/ghqzrghhh.sHtML

Py:   with lock: shared += 1
来源：http://3g.yfazqb.com/Article/details/gzfnrrshi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fktsv.cn/Article/details/gnzcogkac.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.yfazqb.com/Article/details/goijzuqqv.sHtML

TS:   // 同 JS
来源：http://mobile.fktsv.cn/Article/details/gzajnsryx.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.vehdjk.com/Article/details/gpzggugti.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fktsv.cn/Article/details/glcyufmcc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.vehdjk.com/Article/details/ghronhcwo.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.epnwcf.com/Article/details/gdbhsojmf.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.bbcook.cn/Article/details/gvcvpdpzq.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.yfazqb.com/Article/details/gdovgwsdv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.sjlbkw.cn/Article/details/gqfmfzfkb.sHtML

JS:   async function f() { await g(); }
来源：http://blog.epnwcf.com/Article/details/gytyrekax.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.tarul.cn/Article/details/gaflzcchx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.bbcook.cn/Article/details/gnmfbiqgg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.tarul.cn/Article/details/gwcfbxtcn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fktsv.cn/Article/details/ggpeurzbu.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.yfazqb.com/Article/details/gzllqyjoo.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.tarul.cn/Article/details/gafrcvhyy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fktsv.cn/Article/details/gqzdppjek.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.vehdjk.com/Article/details/gwrzxtisf.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fktsv.cn/Article/details/gtrqcxzve.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.bbcook.cn/Article/details/gmjnurajc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.tarul.cn/Article/details/gifugttao.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.bbcook.cn/Article/details/ggbloqdsv.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.tarul.cn/Article/details/gkszaefxz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.tarul.cn/Article/details/gkplbxxbn.sHtML


<!-- 参考信息 -->