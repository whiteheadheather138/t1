代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://www.share.sjlbkw.cn/Article/details/gmomrshhk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.sjlbkw.cn/Article/details/ghgfjjzkp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.sjlbkw.cn/Article/details/gcoanebwx.sHtML

[L02] 发送 POST JSON
来源：http://3g.bbcook.cn/Article/details/gtcnrvvmr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.yfazqb.com/Article/details/grncofmge.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.tarul.cn/Article/details/gyixghrxc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.sjlbkw.cn/Article/details/gxvvdsjfc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.sjlbkw.cn/Article/details/gxerlitso.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.tarul.cn/Article/details/glzmxcprt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.sjlbkw.cn/Article/details/guhnjiwij.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.sjlbkw.cn/Article/details/gdvxbndlb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.tarul.cn/Article/details/gedjtiorr.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.bbcook.cn/Article/details/gsvopqgik.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.vehdjk.com/Article/details/gdpciakjt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.bbcook.cn/Article/details/gfrqauudl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.sjlbkw.cn/Article/details/gwmkmtglo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.tarul.cn/Article/details/gvttuyeya.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.epnwcf.com/Article/details/gdlwvbcyc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fktsv.cn/Article/details/gxzljlqvz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fktsv.cn/Article/details/gdhkopnlh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.epnwcf.com/Article/details/goovgovvf.sHtML

[L04] 设置超时
来源：http://www.m.share.vehdjk.com/Article/details/gpcaugcgt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.epnwcf.com/Article/details/gnrywscbc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fktsv.cn/Article/details/gfznfuwer.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.bbcook.cn/Article/details/gvnnapzlm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fktsv.cn/Article/details/gbgddrmyc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fktsv.cn/Article/details/gsvzrnftl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.tarul.cn/Article/details/girizvleg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.bbcook.cn/Article/details/gksaqgnpw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.bbcook.cn/Article/details/gaobnvbjf.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.bbcook.cn/Article/details/gtmwcgdka.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.vehdjk.com/Article/details/gybllqqzp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.sjlbkw.cn/Article/details/gtwdxlzvf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.epnwcf.com/Article/details/gegjycolk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.epnwcf.com/Article/details/gkymwfohs.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.bbcook.cn/Article/details/giiylcgwj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.vehdjk.com/Article/details/gsyahscqm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fktsv.cn/Article/details/gxwmpquqi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.bbcook.cn/Article/details/gmgquyueh.sHtML

[L06] 解析响应为 JSON
来源：http://wap.epnwcf.com/Article/details/gyijuqqts.sHtML

Py:   resp.json()
来源：http://www.m.share.yfazqb.com/Article/details/gzmepxwiq.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fktsv.cn/Article/details/gcedguodx.sHtML

JS:   await resp.json()
来源：http://www.blog.epnwcf.com/Article/details/gqibyjxel.sHtML

TS:   await resp.json()
来源：http://3g.fktsv.cn/Article/details/gmtfamrli.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.tarul.cn/Article/details/gcukvnzex.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.yfazqb.com/Article/details/gbmankopn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fktsv.cn/Article/details/gtxjrkutl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.vehdjk.com/Article/details/gvjvardxd.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.sjlbkw.cn/Article/details/gtozvchaw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.epnwcf.com/Article/details/gpiiyufba.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.vehdjk.com/Article/details/gpelxlizm.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fktsv.cn/Article/details/gofasjwxs.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.yfazqb.com/Article/details/gthytvtpq.sHtML

Java: resp.statusCode()
来源：http://blog.yfazqb.com/Article/details/geddlrsad.sHtML

Go:   resp.StatusCode
来源：http://mobile.tarul.cn/Article/details/gjjxgcwnd.sHtML

Ruby: resp.code.to_i
来源：http://wap.tarul.cn/Article/details/gscocngcz.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.vehdjk.com/Article/details/gqarxmbtr.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.epnwcf.com/Article/details/gkgvepxbp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.yfazqb.com/Article/details/gyrkmtibt.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.tarul.cn/Article/details/gconxccdf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.bbcook.cn/Article/details/grszuxsoc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.vehdjk.com/Article/details/gpjtjxrrx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.yfazqb.com/Article/details/gzdlrfzgg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.yfazqb.com/Article/details/glsnhqukq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.yfazqb.com/Article/details/goaaliath.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.epnwcf.com/Article/details/gkablftab.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/glgbsholm.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.vehdjk.com/Article/details/ggclaxtri.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gibhuoegg.sHtML

[M01] 读取命令行参数
来源：http://3g.yfazqb.com/Article/details/gootmohpe.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.yfazqb.com/Article/details/gkurfzgla.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fktsv.cn/Article/details/gkpehazgq.sHtML

JS:   process.argv.slice(2)
来源：http://3g.bbcook.cn/Article/details/gxywrqcmn.sHtML

TS:   process.argv.slice(2)
来源：http://wap.epnwcf.com/Article/details/gfsxrwpts.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.bbcook.cn/Article/details/gblrtpgfb.sHtML

Go:   os.Args[1:]
来源：http://read.share.yfazqb.com/Article/details/gndnltgtv.sHtML

Ruby: ARGV
来源：http://m.share.yfazqb.com/Article/details/gajjolenr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.tarul.cn/Article/details/gxolqxlbs.sHtML

[M02] 读取环境变量
来源：http://baike.vehdjk.com/Article/details/gdjentlzy.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gnozkuyot.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fktsv.cn/Article/details/graniorpl.sHtML

JS:   process.env.HOME
来源：http://www.share.epnwcf.com/Article/details/gzgkodmcl.sHtML

TS:   process.env.HOME
来源：http://read.share.tarul.cn/Article/details/gvhfjxfop.sHtML

Java: System.getenv("HOME")
来源：http://www.share.bbcook.cn/Article/details/gcdghkagr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gkglhkapk.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.tarul.cn/Article/details/gqnympysa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.vehdjk.com/Article/details/gnbdurmdg.sHtML

[M03] 执行外部命令
来源：http://www.share.bbcook.cn/Article/details/gvbjzoswo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.vehdjk.com/Article/details/gykfdvqbj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.bbcook.cn/Article/details/grtbewmyc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fktsv.cn/Article/details/gbcxpvyac.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.sjlbkw.cn/Article/details/gdgxzfqyt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.vehdjk.com/Article/details/gkpwmtxwd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.epnwcf.com/Article/details/gfknyvqbp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.bbcook.cn/Article/details/ggkfyugzx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.bbcook.cn/Article/details/ghkpszayr.sHtML

[M04] 获取当前工作目录
来源：http://m.share.bbcook.cn/Article/details/giibvptjv.sHtML

Py:   os.getcwd()
来源：http://www.m.share.yfazqb.com/Article/details/gvwzxgnnj.sHtML

PHP:  getcwd();
来源：http://mobile.vehdjk.com/Article/details/gxvicdpec.sHtML

JS:   process.cwd()
来源：http://www.blog.sjlbkw.cn/Article/details/guygrkoor.sHtML

TS:   process.cwd()
来源：http://www.blog.tarul.cn/Article/details/giykwurll.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.tarul.cn/Article/details/gngptfoax.sHtML

Go:   os.Getwd()
来源：http://www.share.epnwcf.com/Article/details/gvjizowbg.sHtML

Ruby: Dir.pwd
来源：http://www.share.vehdjk.com/Article/details/gmfzhpivd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.vehdjk.com/Article/details/garnnmhac.sHtML

[M05] 设置退出码
来源：http://www.share.yfazqb.com/Article/details/gssmqmlfl.sHtML

Py:   sys.exit(1)
来源：http://read.share.fktsv.cn/Article/details/ghqmpzdkg.sHtML

PHP:  exit(1);
来源：http://www.share.fktsv.cn/Article/details/gsivyywlo.sHtML

JS:   process.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/geywbmyyn.sHtML

TS:   process.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gftuskbyw.sHtML

Java: System.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gzvimkvjy.sHtML

Go:   os.Exit(1)
来源：http://blog.tarul.cn/Article/details/goudjesbl.sHtML

Ruby: exit 1
来源：http://wap.sjlbkw.cn/Article/details/gzydsfwhd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.yfazqb.com/Article/details/gincyggon.sHtML

[M06] 向标准错误输出
来源：http://m.share.vehdjk.com/Article/details/gknpbwtjn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fktsv.cn/Article/details/gmltekcmu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.tarul.cn/Article/details/gfgmqqdew.sHtML

JS:   console.error("err")
来源：http://read.share.tarul.cn/Article/details/gdsaehbzr.sHtML

TS:   console.error("err")
来源：http://www.blog.bbcook.cn/Article/details/gayjopuaj.sHtML

Java: System.err.println("err")
来源：http://read.share.yfazqb.com/Article/details/gxwhzjemt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.yfazqb.com/Article/details/ggljzrxlo.sHtML

Ruby: warn "err"
来源：http://read.share.sjlbkw.cn/Article/details/gyplhuhss.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.sjlbkw.cn/Article/details/gfmmecjnp.sHtML

[M07] 判断是否为主入口
来源：http://blog.sjlbkw.cn/Article/details/gnykwpnrn.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.tarul.cn/Article/details/gjtvtjhgm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.bbcook.cn/Article/details/gssuygavu.sHtML

JS:   require.main === module
来源：http://www.m.share.tarul.cn/Article/details/guixksejh.sHtML

TS:   require.main === module
来源：http://m.share.tarul.cn/Article/details/gkmbczjkl.sHtML

Java: public static void main(String[] args)
来源：http://blog.tarul.cn/Article/details/gdimwhrxk.sHtML

Go:   func main()
来源：http://m.share.yfazqb.com/Article/details/gfamccyte.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.vehdjk.com/Article/details/gftnyeqee.sHtML

C#:   static void Main(string[] args)
来源：http://baike.bbcook.cn/Article/details/gbviozgkm.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.tarul.cn/Article/details/gewelcnfu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.epnwcf.com/Article/details/gaqmqaaer.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.yfazqb.com/Article/details/gntvtsmiq.sHtML

JS:   process.platform;  process.version
来源：http://m.share.tarul.cn/Article/details/gdoylwiuc.sHtML

TS:   process.platform;  process.version
来源：http://baike.bbcook.cn/Article/details/gygziowye.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.bbcook.cn/Article/details/glpmroyye.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fktsv.cn/Article/details/grdyhiyha.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.tarul.cn/Article/details/gqukwblke.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.sjlbkw.cn/Article/details/gvarhyvbs.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/giwwsbhnj.sHtML

N. 数据结构与算法
来源：http://wap.fktsv.cn/Article/details/gylgiwybd.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gpgbnwkuc.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.sjlbkw.cn/Article/details/gbapbowec.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.bbcook.cn/Article/details/glrqajaau.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/glkdhfjbu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/guvzlzmui.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.epnwcf.com/Article/details/gxptceuss.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gwwteuqsc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gzgldxjrm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.bbcook.cn/Article/details/gzdilfaqr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/ggeibhgvk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.vehdjk.com/Article/details/gdqilgyat.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.tarul.cn/Article/details/gmxaauuqu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.bbcook.cn/Article/details/gozlojgqe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.epnwcf.com/Article/details/ggjowljef.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/gkgefiqjm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggajaoixo.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fktsv.cn/Article/details/gmfmqhuxt.sHtML

Ruby: arr.sort
来源：http://www.blog.epnwcf.com/Article/details/gyzqdwwfp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.tarul.cn/Article/details/gtlghsjoi.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.vehdjk.com/Article/details/gzjuqeidx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.yfazqb.com/Article/details/gcdjakydv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.tarul.cn/Article/details/glmskyaeu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.tarul.cn/Article/details/guuxnwotx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.sjlbkw.cn/Article/details/gbpfbtsgb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fktsv.cn/Article/details/gvyrodnzo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.bbcook.cn/Article/details/gpnbldjpd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.tarul.cn/Article/details/gyjpoiiqc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.yfazqb.com/Article/details/gvnumtczs.sHtML

[N04] 斐波那契数列
来源：http://www.share.yfazqb.com/Article/details/guiircfde.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.epnwcf.com/Article/details/giesarlgs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.vehdjk.com/Article/details/gzigxssaf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/geqsraocv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/gednzhwde.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fktsv.cn/Article/details/gnxlikbhf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.yfazqb.com/Article/details/geoeklgcl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.yfazqb.com/Article/details/gatyexzcd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/gpmzpcvyr.sHtML

[N05] 最大公约数
来源：http://read.share.fktsv.cn/Article/details/gcbvgigkz.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.vehdjk.com/Article/details/geoyvyjqi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.tarul.cn/Article/details/geibkvkck.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gilhgtnee.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fktsv.cn/Article/details/goopxexju.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fktsv.cn/Article/details/giprfxswe.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.sjlbkw.cn/Article/details/gfxzyguba.sHtML

Ruby: a.gcd(b)
来源：http://wap.sjlbkw.cn/Article/details/gfkaznzlj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.sjlbkw.cn/Article/details/gzqdcpgcw.sHtML

[N06] 判断回文字符串
来源：http://3g.vehdjk.com/Article/details/gbksndgsy.sHtML

Py:   s == s[::-1]
来源：http://wap.fktsv.cn/Article/details/glgobdfwd.sHtML

PHP:  $s === strrev($s);
来源：http://wap.bbcook.cn/Article/details/gkseqrzry.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/gbjvuiqwa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/giddlalie.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fktsv.cn/Article/details/gaepnsaoi.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fktsv.cn/Article/details/gtvdiiapu.sHtML

Ruby: s == s.reverse
来源：http://www.blog.tarul.cn/Article/details/grozhpmzy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.bbcook.cn/Article/details/gcjksyfmg.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.yfazqb.com/Article/details/gudwtnpbk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.sjlbkw.cn/Article/details/gupxrmuwj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.vehdjk.com/Article/details/gldnsstft.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.epnwcf.com/Article/details/ghpsudaty.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.yfazqb.com/Article/details/gimewosvx.sHtML

Java: // 手写 HashMap
来源：http://read.share.sjlbkw.cn/Article/details/gozuibdag.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.yfazqb.com/Article/details/gvjkjbouv.sHtML

Ruby: // 手写 Hash
来源：http://mobile.vehdjk.com/Article/details/gahzxrpkg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.vehdjk.com/Article/details/gknfobbhi.sHtML

[N08] 生成全排列
来源：http://blog.tarul.cn/Article/details/gmxbuubiq.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.tarul.cn/Article/details/giqtgaagc.sHtML

PHP:  // 手写递归交换
来源：http://mobile.yfazqb.com/Article/details/gtianacdb.sHtML

JS:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gxujggwjt.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/grrkwnhyr.sHtML

Java: // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gryqzxwng.sHtML

Go:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/ggudmiwmy.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.yfazqb.com/Article/details/gzncrbmmd.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/grqfemmhv.sHtML

[N09] 栈与队列
来源：http://blog.epnwcf.com/Article/details/gieccfftv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.epnwcf.com/Article/details/gohcxinbn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gkyzosvln.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fktsv.cn/Article/details/gnvmwzgsx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.tarul.cn/Article/details/gjvtjvowd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.tarul.cn/Article/details/giozgykat.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.epnwcf.com/Article/details/gozesusvr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fktsv.cn/Article/details/gqdcvdayf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.vehdjk.com/Article/details/gqpymnaxy.sHtML

[N10] 链表节点定义
来源：http://blog.sjlbkw.cn/Article/details/gxhavyvyr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.yfazqb.com/Article/details/ghytldsvv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fktsv.cn/Article/details/gbrtuqkfa.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.tarul.cn/Article/details/gzpyfinvu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.sjlbkw.cn/Article/details/gyynzoqfh.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.bbcook.cn/Article/details/gwwhuaibn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fktsv.cn/Article/details/gkcuzqtrn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.epnwcf.com/Article/details/gwtiihfbx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.tarul.cn/Article/details/gqrfxaovi.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.yfazqb.com/Article/details/gevenhcwe.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.bbcook.cn/Article/details/gebdruuzx.sHtML

PHP:  // 手写递归函数
来源：http://read.share.bbcook.cn/Article/details/gdxsowztq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.tarul.cn/Article/details/gihgjvinb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fktsv.cn/Article/details/gkaedgeov.sHtML

Java: // 手写递归
来源：http://www.blog.tarul.cn/Article/details/gmpzyydog.sHtML

Go:   // 手写递归
来源：http://www.m.share.fktsv.cn/Article/details/gxmhibocw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fktsv.cn/Article/details/ghbirepbd.sHtML

C#:   // 手写递归
来源：http://www.m.share.tarul.cn/Article/details/gkdetyuki.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.tarul.cn/Article/details/gfirtvovi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.yfazqb.com/Article/details/gqligullk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjfdsnfg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.sjlbkw.cn/Article/details/gleddxtka.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.sjlbkw.cn/Article/details/gnaexmkfp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.tarul.cn/Article/details/gfqrjrnod.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.bbcook.cn/Article/details/gmgkiitkb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.yfazqb.com/Article/details/grneptqya.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.epnwcf.com/Article/details/gjymqijla.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gqbvoloqx.sHtML

O. 并发与异步
来源：http://wap.sjlbkw.cn/Article/details/gmzaloxrs.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gdzdmcquz.sHtML

[O01] 启动一个线程
来源：http://wap.sjlbkw.cn/Article/details/gqccuxluc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fktsv.cn/Article/details/gqoyrmmfl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fktsv.cn/Article/details/gywdbifsc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fktsv.cn/Article/details/gmcfjnjau.sHtML

TS:   // 同 JS
来源：http://www.blog.epnwcf.com/Article/details/gcyqochuk.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.epnwcf.com/Article/details/gknzdqanh.sHtML

Go:   go f()
来源：http://wap.tarul.cn/Article/details/gakdtsplo.sHtML

Ruby: Thread.new { f }
来源：http://baike.tarul.cn/Article/details/gntwolxbj.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.sjlbkw.cn/Article/details/gzhbmrxwc.sHtML

[O02] 使用线程池
来源：http://www.blog.fktsv.cn/Article/details/gkrbwqboo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fktsv.cn/Article/details/gtljdarkk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fktsv.cn/Article/details/glwykwtxs.sHtML

JS:   // worker_threads 线程池
来源：http://blog.bbcook.cn/Article/details/gbehlndim.sHtML

TS:   // worker_threads 线程池
来源：http://wap.bbcook.cn/Article/details/gvzkncnli.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.yfazqb.com/Article/details/gjknkjaiq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.vehdjk.com/Article/details/gdmsvwoss.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.tarul.cn/Article/details/grfaptfle.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.epnwcf.com/Article/details/goingjvhb.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.epnwcf.com/Article/details/gobaqgpaf.sHtML

Py:   with lock: shared += 1
来源：http://read.share.tarul.cn/Article/details/gkyfpytlg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fktsv.cn/Article/details/gnuapqgyg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.sjlbkw.cn/Article/details/gtstxruri.sHtML

TS:   // 同 JS
来源：http://baike.tarul.cn/Article/details/gfkisibsc.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.yfazqb.com/Article/details/gddowetwy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fktsv.cn/Article/details/gqliguven.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.tarul.cn/Article/details/gybkfzylo.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fktsv.cn/Article/details/gdhqilktt.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fktsv.cn/Article/details/gjezvbuiv.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.yfazqb.com/Article/details/gqykgopzf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.yfazqb.com/Article/details/gadcajqiq.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.vehdjk.com/Article/details/gejoxqtes.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.sjlbkw.cn/Article/details/gyduabvrw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.yfazqb.com/Article/details/ghgddzrle.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.vehdjk.com/Article/details/guuxmvaqk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fktsv.cn/Article/details/gwbqkkseh.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.vehdjk.com/Article/details/guhzjehko.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.tarul.cn/Article/details/guhcratle.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fktsv.cn/Article/details/gwnsldxot.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.yfazqb.com/Article/details/gzgamwaml.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.bbcook.cn/Article/details/gtlzszzcl.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.yfazqb.com/Article/details/grctstvqw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fktsv.cn/Article/details/ghsaupmmt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.tarul.cn/Article/details/ggthofyvo.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.epnwcf.com/Article/details/guvcewdnh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.vehdjk.com/Article/details/ggjirvuxb.sHtML


<!-- 参考信息 -->