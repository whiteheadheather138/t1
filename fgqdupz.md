代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/givjchkvw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.epnwcf.com/Article/details/gduasgfih.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.tarul.cn/Article/details/gfgmtdqdp.sHtML

[L02] 发送 POST JSON
来源：http://www.share.sjlbkw.cn/Article/details/gzklbcbgv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fktsv.cn/Article/details/gshohpssw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fktsv.cn/Article/details/ggrgijuur.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fktsv.cn/Article/details/gnetuvcec.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.epnwcf.com/Article/details/gwiwxqyza.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.bbcook.cn/Article/details/gxiyoxlkg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.tarul.cn/Article/details/glraazkno.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.yfazqb.com/Article/details/grrgjftcc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.yfazqb.com/Article/details/gjujkhiqh.sHtML

[L03] 设置自定义请求头
来源：http://3g.tarul.cn/Article/details/gjlmytmjd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.sjlbkw.cn/Article/details/gtyydnhgk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.epnwcf.com/Article/details/gmheyhvbm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.bbcook.cn/Article/details/gajkwlunz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.bbcook.cn/Article/details/gdwgebfdx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.yfazqb.com/Article/details/gykvhnahb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fktsv.cn/Article/details/gbqnqrmlk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.bbcook.cn/Article/details/gvnwychcv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.tarul.cn/Article/details/gemvikvbz.sHtML

[L04] 设置超时
来源：http://read.share.vehdjk.com/Article/details/glkpbcnuv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.vehdjk.com/Article/details/gupzicfaq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.tarul.cn/Article/details/gybgekmoo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.epnwcf.com/Article/details/gyrzqjjgw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.vehdjk.com/Article/details/gqvdvpmgp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.vehdjk.com/Article/details/gybuoslci.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.epnwcf.com/Article/details/gdqzqvbaz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.epnwcf.com/Article/details/gasxprlne.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fktsv.cn/Article/details/gvjqpbibd.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.vehdjk.com/Article/details/gyzpegtxb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.epnwcf.com/Article/details/gephsxmfo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.bbcook.cn/Article/details/gsvqbevde.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.yfazqb.com/Article/details/gjwkffswx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.sjlbkw.cn/Article/details/gzjpvjetm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.bbcook.cn/Article/details/ghydgtgav.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.vehdjk.com/Article/details/gouyrzwgo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.tarul.cn/Article/details/gjtqpyzls.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fktsv.cn/Article/details/gqeuaibue.sHtML

[L06] 解析响应为 JSON
来源：http://blog.tarul.cn/Article/details/gwqzyvkgj.sHtML

Py:   resp.json()
来源：http://3g.vehdjk.com/Article/details/gyqoyntbw.sHtML

PHP:  json_decode($body, true);
来源：http://blog.vehdjk.com/Article/details/gickxmijx.sHtML

JS:   await resp.json()
来源：http://www.share.yfazqb.com/Article/details/grsszxjra.sHtML

TS:   await resp.json()
来源：http://mobile.fktsv.cn/Article/details/gknubzozo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.sjlbkw.cn/Article/details/gcavijkde.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.bbcook.cn/Article/details/gywkazfxu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.epnwcf.com/Article/details/goedaetcz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.sjlbkw.cn/Article/details/gfzkddvsi.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.epnwcf.com/Article/details/gphlazwtq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.epnwcf.com/Article/details/gpnfpnzcm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.vehdjk.com/Article/details/gxuqxocjn.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.tarul.cn/Article/details/gmevgaagz.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.tarul.cn/Article/details/gdyvyocjg.sHtML

Java: resp.statusCode()
来源：http://3g.epnwcf.com/Article/details/gtqeedprl.sHtML

Go:   resp.StatusCode
来源：http://blog.tarul.cn/Article/details/goblvqpsa.sHtML

Ruby: resp.code.to_i
来源：http://wap.fktsv.cn/Article/details/gdxdbjhbp.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.bbcook.cn/Article/details/gqwarezrq.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.yfazqb.com/Article/details/gnytoraav.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.tarul.cn/Article/details/gtecsflxd.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.vehdjk.com/Article/details/gdhfapuab.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.epnwcf.com/Article/details/gajvxpetn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.vehdjk.com/Article/details/gaphsklsl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.bbcook.cn/Article/details/grytoqwtm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.sjlbkw.cn/Article/details/gtszntuwm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.tarul.cn/Article/details/gusiylouu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.yfazqb.com/Article/details/gelhwytcp.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gbydnopnm.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.bbcook.cn/Article/details/guqprqzgl.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/glaeiblcy.sHtML

[M01] 读取命令行参数
来源：http://read.share.yfazqb.com/Article/details/galvxthbe.sHtML

Py:   sys.argv[1:]
来源：http://read.share.yfazqb.com/Article/details/gmeanedtv.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fktsv.cn/Article/details/gfujlsddm.sHtML

JS:   process.argv.slice(2)
来源：http://baike.epnwcf.com/Article/details/gzpmsakge.sHtML

TS:   process.argv.slice(2)
来源：http://wap.vehdjk.com/Article/details/gxmonvvjl.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fktsv.cn/Article/details/gkldrjdlf.sHtML

Go:   os.Args[1:]
来源：http://3g.vehdjk.com/Article/details/gctintson.sHtML

Ruby: ARGV
来源：http://www.blog.fktsv.cn/Article/details/gdciswrii.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.epnwcf.com/Article/details/ggmgkgopw.sHtML

[M02] 读取环境变量
来源：http://wap.yfazqb.com/Article/details/guoqxhgar.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fktsv.cn/Article/details/gouxarels.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.bbcook.cn/Article/details/gmekgfuxr.sHtML

JS:   process.env.HOME
来源：http://m.share.tarul.cn/Article/details/gaikckuvk.sHtML

TS:   process.env.HOME
来源：http://read.share.vehdjk.com/Article/details/ghgiofwmd.sHtML

Java: System.getenv("HOME")
来源：http://3g.fktsv.cn/Article/details/gfvswurop.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.vehdjk.com/Article/details/gritmegda.sHtML

Ruby: ENV["HOME"]
来源：http://wap.epnwcf.com/Article/details/gbcfqfesj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fktsv.cn/Article/details/gehopmczk.sHtML

[M03] 执行外部命令
来源：http://read.share.fktsv.cn/Article/details/gnvszmqkr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.yfazqb.com/Article/details/ghypffjee.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.sjlbkw.cn/Article/details/gchlxdsos.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.sjlbkw.cn/Article/details/ggurdrwxd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fktsv.cn/Article/details/gxxlxfkod.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.vehdjk.com/Article/details/gopjpgcou.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fktsv.cn/Article/details/gvohlvixr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fktsv.cn/Article/details/gtzuwqgiv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.bbcook.cn/Article/details/getegztmk.sHtML

[M04] 获取当前工作目录
来源：http://3g.bbcook.cn/Article/details/gnovylayr.sHtML

Py:   os.getcwd()
来源：http://www.share.sjlbkw.cn/Article/details/ghcchzgej.sHtML

PHP:  getcwd();
来源：http://baike.tarul.cn/Article/details/ggmrvmgcp.sHtML

JS:   process.cwd()
来源：http://3g.vehdjk.com/Article/details/gkuylarrr.sHtML

TS:   process.cwd()
来源：http://mobile.yfazqb.com/Article/details/grhvavkgq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.tarul.cn/Article/details/gxsuawhtb.sHtML

Go:   os.Getwd()
来源：http://www.share.vehdjk.com/Article/details/ggmuxpovl.sHtML

Ruby: Dir.pwd
来源：http://3g.fktsv.cn/Article/details/ganukyiwv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.sjlbkw.cn/Article/details/gocmiftss.sHtML

[M05] 设置退出码
来源：http://mobile.vehdjk.com/Article/details/gdyjyjhvk.sHtML

Py:   sys.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/geogcwftk.sHtML

PHP:  exit(1);
来源：http://baike.fktsv.cn/Article/details/gelhmiqcu.sHtML

JS:   process.exit(1)
来源：http://read.share.epnwcf.com/Article/details/ghejiwcll.sHtML

TS:   process.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gtmhtxxzf.sHtML

Java: System.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gmbukfoui.sHtML

Go:   os.Exit(1)
来源：http://mobile.yfazqb.com/Article/details/gankdplal.sHtML

Ruby: exit 1
来源：http://mobile.tarul.cn/Article/details/gdsetolui.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fktsv.cn/Article/details/gsegyribd.sHtML

[M06] 向标准错误输出
来源：http://m.share.epnwcf.com/Article/details/glqrgkomd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.tarul.cn/Article/details/gthudfonu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.vehdjk.com/Article/details/gxzgwjqwr.sHtML

JS:   console.error("err")
来源：http://wap.yfazqb.com/Article/details/gbsggxvln.sHtML

TS:   console.error("err")
来源：http://blog.sjlbkw.cn/Article/details/gxhkxxnuw.sHtML

Java: System.err.println("err")
来源：http://m.share.tarul.cn/Article/details/gqszzfqvn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.sjlbkw.cn/Article/details/gscvtlifj.sHtML

Ruby: warn "err"
来源：http://www.m.share.yfazqb.com/Article/details/getjkzies.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.sjlbkw.cn/Article/details/gsiexjcev.sHtML

[M07] 判断是否为主入口
来源：http://blog.tarul.cn/Article/details/gaypzqrqf.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.vehdjk.com/Article/details/glygvqyxd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.yfazqb.com/Article/details/gvtksuvue.sHtML

JS:   require.main === module
来源：http://www.blog.epnwcf.com/Article/details/gphgtqdcm.sHtML

TS:   require.main === module
来源：http://wap.fktsv.cn/Article/details/glxzrpsgu.sHtML

Java: public static void main(String[] args)
来源：http://wap.sjlbkw.cn/Article/details/gkblvsijo.sHtML

Go:   func main()
来源：http://baike.fktsv.cn/Article/details/glwbgwhls.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fktsv.cn/Article/details/gwwinbumy.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.yfazqb.com/Article/details/glcgkyemg.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.tarul.cn/Article/details/grwyohfwx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.bbcook.cn/Article/details/ghvufakbu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fktsv.cn/Article/details/grophsgky.sHtML

JS:   process.platform;  process.version
来源：http://m.share.bbcook.cn/Article/details/gxcxrzoex.sHtML

TS:   process.platform;  process.version
来源：http://wap.tarul.cn/Article/details/gnaqeixkc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.sjlbkw.cn/Article/details/gquvzxtkl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.epnwcf.com/Article/details/gwcqlbhlo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.tarul.cn/Article/details/guvfipclu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.vehdjk.com/Article/details/gcdfyjdku.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ghfnktohj.sHtML

N. 数据结构与算法
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgezxxln.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gqifqoqsv.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.yfazqb.com/Article/details/ghcstmwzm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gvkjnjpgh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.tarul.cn/Article/details/gnsrbcnae.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gwnwvpoit.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.yfazqb.com/Article/details/gtqdxiesr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.vehdjk.com/Article/details/grluxssyl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.vehdjk.com/Article/details/gpshpcemt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fktsv.cn/Article/details/goubqnqtp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fktsv.cn/Article/details/gossqwlkc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.yfazqb.com/Article/details/gadvvvzqn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.epnwcf.com/Article/details/goocegzhz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.yfazqb.com/Article/details/gfxtkecox.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/gdsxhwjjl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.vehdjk.com/Article/details/gahlziycp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.tarul.cn/Article/details/gwidkyavc.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.bbcook.cn/Article/details/gjkfexokv.sHtML

Ruby: arr.sort
来源：http://blog.tarul.cn/Article/details/gvxsxuoxm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjoyabwc.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.vehdjk.com/Article/details/gzpfbcmhb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.epnwcf.com/Article/details/guhbypqmg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.tarul.cn/Article/details/gzlfsdnxn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.tarul.cn/Article/details/gmgiyqwqu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.yfazqb.com/Article/details/gckzsjvvv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.vehdjk.com/Article/details/gqtmfivuy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.epnwcf.com/Article/details/gzxlmuzjr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.tarul.cn/Article/details/gbbmxrwju.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fktsv.cn/Article/details/gigyypzkq.sHtML

[N04] 斐波那契数列
来源：http://baike.sjlbkw.cn/Article/details/gitqlrwqb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.vehdjk.com/Article/details/gibheclsg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.tarul.cn/Article/details/gmxdcpdtt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/glarrtxmp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.tarul.cn/Article/details/goubjynxb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.bbcook.cn/Article/details/gshedrife.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.yfazqb.com/Article/details/gzveujfbw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.tarul.cn/Article/details/gvkcnadlz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.vehdjk.com/Article/details/gbptghpum.sHtML

[N05] 最大公约数
来源：http://3g.yfazqb.com/Article/details/gucnofwfv.sHtML

Py:   math.gcd(a, b)
来源：http://baike.vehdjk.com/Article/details/gvesippjh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fktsv.cn/Article/details/ghwzeazit.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.epnwcf.com/Article/details/gcmfdgkwb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fktsv.cn/Article/details/gtyhidwsq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.yfazqb.com/Article/details/gxfmbhfld.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.yfazqb.com/Article/details/gtdxyzzvs.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.vehdjk.com/Article/details/gmmcfscov.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fktsv.cn/Article/details/gbabeslsz.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.epnwcf.com/Article/details/gzmozagxu.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpyjzgoi.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.yfazqb.com/Article/details/gnzlfrock.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/gfhcvkbam.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gswgihbah.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.bbcook.cn/Article/details/grhbexztt.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.yfazqb.com/Article/details/gbburqczn.sHtML

Ruby: s == s.reverse
来源：http://www.blog.vehdjk.com/Article/details/gkclhpvon.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fktsv.cn/Article/details/grvqyxzxt.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.vehdjk.com/Article/details/gmqrvzfoq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.sjlbkw.cn/Article/details/glekfauhk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.tarul.cn/Article/details/gmmpwgfmi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fktsv.cn/Article/details/gsuvefmsy.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.vehdjk.com/Article/details/gneltkpsq.sHtML

Java: // 手写 HashMap
来源：http://mobile.sjlbkw.cn/Article/details/gaqffopks.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fktsv.cn/Article/details/goiaijfyy.sHtML

Ruby: // 手写 Hash
来源：http://read.share.bbcook.cn/Article/details/gtibslgbv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fktsv.cn/Article/details/gdtanaoka.sHtML

[N08] 生成全排列
来源：http://blog.epnwcf.com/Article/details/gbbzpvlku.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.epnwcf.com/Article/details/gddeozehp.sHtML

PHP:  // 手写递归交换
来源：http://blog.epnwcf.com/Article/details/gyrivkfqr.sHtML

JS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/grjtwiqzr.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gbpscfnta.sHtML

Java: // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gmyklockf.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gjohrkkcr.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fktsv.cn/Article/details/gwzqwhazc.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gziosbzff.sHtML

[N09] 栈与队列
来源：http://www.share.tarul.cn/Article/details/grteyfvou.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.epnwcf.com/Article/details/gqkwhjqoo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.vehdjk.com/Article/details/gtwnqogpx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gytofqzlh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fktsv.cn/Article/details/glrkheutr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.vehdjk.com/Article/details/gdzihvjpx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.bbcook.cn/Article/details/gdlkeptwa.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.tarul.cn/Article/details/gqsgfitdz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.sjlbkw.cn/Article/details/guafvigvs.sHtML

[N10] 链表节点定义
来源：http://baike.sjlbkw.cn/Article/details/ghlnepejf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.sjlbkw.cn/Article/details/gegxbtkkv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.sjlbkw.cn/Article/details/goacvzukm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.tarul.cn/Article/details/gqfisejps.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.tarul.cn/Article/details/gsyyhpwtl.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.tarul.cn/Article/details/gmmdpvsgu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.sjlbkw.cn/Article/details/gufnxwydn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.vehdjk.com/Article/details/gksywwuaz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.yfazqb.com/Article/details/gayzuwgkm.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.yfazqb.com/Article/details/gpgnragix.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.vehdjk.com/Article/details/guqyopjmd.sHtML

PHP:  // 手写递归函数
来源：http://mobile.vehdjk.com/Article/details/gpnxtrqtf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.tarul.cn/Article/details/ghnjbkfyh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.yfazqb.com/Article/details/gvfmydjbb.sHtML

Java: // 手写递归
来源：http://m.share.epnwcf.com/Article/details/gkrbveqbo.sHtML

Go:   // 手写递归
来源：http://m.share.sjlbkw.cn/Article/details/glperlmyg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.sjlbkw.cn/Article/details/gmroondan.sHtML

C#:   // 手写递归
来源：http://blog.fktsv.cn/Article/details/gcsrijdqy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.sjlbkw.cn/Article/details/glpcualnp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.tarul.cn/Article/details/ghyzjmaba.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.tarul.cn/Article/details/gnzztihjl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.vehdjk.com/Article/details/gdgrvjggg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.tarul.cn/Article/details/guofbwzbh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fktsv.cn/Article/details/gyaldncrr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.tarul.cn/Article/details/gvqqpxsva.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.sjlbkw.cn/Article/details/gaesevrox.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.bbcook.cn/Article/details/gmuvsepen.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gjxigiujw.sHtML

O. 并发与异步
来源：http://baike.tarul.cn/Article/details/gsqwldisp.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gfwfujgrf.sHtML

[O01] 启动一个线程
来源：http://www.blog.sjlbkw.cn/Article/details/gpziiyimj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.epnwcf.com/Article/details/gloqiaarg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.yfazqb.com/Article/details/gsqeiixml.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.bbcook.cn/Article/details/gshsnfjex.sHtML

TS:   // 同 JS
来源：http://mobile.tarul.cn/Article/details/gslqwkhqd.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.vehdjk.com/Article/details/gewldwkqv.sHtML

Go:   go f()
来源：http://mobile.yfazqb.com/Article/details/gouhrzgpc.sHtML

Ruby: Thread.new { f }
来源：http://www.share.yfazqb.com/Article/details/grdeojagx.sHtML

C#:   Task.Run(() => F());
来源：http://blog.tarul.cn/Article/details/gqcoyccwd.sHtML

[O02] 使用线程池
来源：http://blog.epnwcf.com/Article/details/guqswhmhg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.vehdjk.com/Article/details/gevhgatou.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fktsv.cn/Article/details/gpujymqor.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.sjlbkw.cn/Article/details/gjcyeyglp.sHtML

TS:   // worker_threads 线程池
来源：http://3g.epnwcf.com/Article/details/gbrnnyiya.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.bbcook.cn/Article/details/glpkovhdt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.tarul.cn/Article/details/gchwjtkrr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.vehdjk.com/Article/details/gcxzrytde.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.epnwcf.com/Article/details/gadqgjhtz.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.sjlbkw.cn/Article/details/gqwobhonz.sHtML

Py:   with lock: shared += 1
来源：http://baike.epnwcf.com/Article/details/gypmkpgrm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.vehdjk.com/Article/details/gcsearqwi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.bbcook.cn/Article/details/ggeitzoiw.sHtML

TS:   // 同 JS
来源：http://www.blog.sjlbkw.cn/Article/details/ggqoybflt.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.vehdjk.com/Article/details/gllkexaph.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.epnwcf.com/Article/details/gkozekohf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fktsv.cn/Article/details/ggarlnrlk.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.tarul.cn/Article/details/gesfkdizi.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fktsv.cn/Article/details/gpjtwlkik.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.yfazqb.com/Article/details/ggxjgrety.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.yfazqb.com/Article/details/gdhxtwjmz.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.tarul.cn/Article/details/gvqcsnrbt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.sjlbkw.cn/Article/details/gxwmvmrxd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.vehdjk.com/Article/details/gdhuaihpz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.bbcook.cn/Article/details/gtmaiqlzs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.bbcook.cn/Article/details/gomjmuffb.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.epnwcf.com/Article/details/grtcohtmy.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.bbcook.cn/Article/details/giwmywvyh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.sjlbkw.cn/Article/details/gkiwslofp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.sjlbkw.cn/Article/details/guwjhqlos.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.sjlbkw.cn/Article/details/gtpnzrjlp.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.bbcook.cn/Article/details/gfyhmdzum.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.vehdjk.com/Article/details/gcwaixjnb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.epnwcf.com/Article/details/gislhrpmt.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.bbcook.cn/Article/details/gzbqczbjg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.sjlbkw.cn/Article/details/gmynxdkkm.sHtML


<!-- 参考信息 -->