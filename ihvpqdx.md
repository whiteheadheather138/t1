代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://m.share.vehdjk.com/Article/details/gszrzstud.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.yfazqb.com/Article/details/gogmnxbpq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.bbcook.cn/Article/details/gepfxaioh.sHtML

[L02] 发送 POST JSON
来源：http://read.share.yfazqb.com/Article/details/gwdsvyczs.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.yfazqb.com/Article/details/gcjmkkpns.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.tarul.cn/Article/details/ghimpmdrv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.tarul.cn/Article/details/gkwajfbpw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.tarul.cn/Article/details/gwgwtoqvm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.bbcook.cn/Article/details/gmpgaiamu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.sjlbkw.cn/Article/details/goeimihgb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.sjlbkw.cn/Article/details/gxhkiwqgi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.bbcook.cn/Article/details/ggxxzcdfp.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.yfazqb.com/Article/details/gnkcffawx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.sjlbkw.cn/Article/details/gdishvakq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.sjlbkw.cn/Article/details/ghqzigbab.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.vehdjk.com/Article/details/gdukdefke.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.bbcook.cn/Article/details/gawyfoqym.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.vehdjk.com/Article/details/geckktoxw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.yfazqb.com/Article/details/gvjjwlwqu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.sjlbkw.cn/Article/details/gfolwocqr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.epnwcf.com/Article/details/gxiqesbby.sHtML

[L04] 设置超时
来源：http://blog.epnwcf.com/Article/details/gxngxdkdj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.tarul.cn/Article/details/gfgedtxof.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.bbcook.cn/Article/details/gxzoluzxa.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.tarul.cn/Article/details/grhaexzhp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.bbcook.cn/Article/details/gcefvttkh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.tarul.cn/Article/details/gmhlkqsan.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fktsv.cn/Article/details/gypjfkxkv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fktsv.cn/Article/details/ghmvbogme.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fktsv.cn/Article/details/goopkqtfz.sHtML

[L05] 上传文件（multipart）
来源：http://3g.tarul.cn/Article/details/gubihhcrx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.vehdjk.com/Article/details/guayfdbau.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.bbcook.cn/Article/details/geneolpkx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.sjlbkw.cn/Article/details/gesigxwgp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.yfazqb.com/Article/details/ghuakzxbb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.tarul.cn/Article/details/gxbmtibal.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.yfazqb.com/Article/details/gucgvfjux.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fktsv.cn/Article/details/geiuhlynm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.tarul.cn/Article/details/gnqgcifxv.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.bbcook.cn/Article/details/glvqyssil.sHtML

Py:   resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/guzanpcil.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.tarul.cn/Article/details/ghazhadfx.sHtML

JS:   await resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/gxwudcijw.sHtML

TS:   await resp.json()
来源：http://3g.vehdjk.com/Article/details/gwnmmebsf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.sjlbkw.cn/Article/details/gtdgycpil.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.yfazqb.com/Article/details/gkeasbtuj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.tarul.cn/Article/details/gviwdfddr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.vehdjk.com/Article/details/gkaqsevek.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.vehdjk.com/Article/details/gvphecrpl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.yfazqb.com/Article/details/guxgdqjpo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.bbcook.cn/Article/details/gkpdvkrbm.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fktsv.cn/Article/details/gdrxpnrmr.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.sjlbkw.cn/Article/details/gpyphaejf.sHtML

Java: resp.statusCode()
来源：http://www.blog.bbcook.cn/Article/details/gbyutgovj.sHtML

Go:   resp.StatusCode
来源：http://m.share.yfazqb.com/Article/details/glmrgnztk.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fktsv.cn/Article/details/gqbotihvs.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.epnwcf.com/Article/details/gojoezfmw.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.vehdjk.com/Article/details/gmdvdnjaq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.epnwcf.com/Article/details/gfubzuqqe.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.epnwcf.com/Article/details/gmfaghcmu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.sjlbkw.cn/Article/details/gzzqikenf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.epnwcf.com/Article/details/gbnspibat.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.vehdjk.com/Article/details/ghowvdbyb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fktsv.cn/Article/details/gdoqjqjhr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.vehdjk.com/Article/details/ghhptmkia.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fktsv.cn/Article/details/ghbiajrjs.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gwtdoaaol.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.vehdjk.com/Article/details/gbjmcnkqz.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/ginkxeuql.sHtML

[M01] 读取命令行参数
来源：http://www.share.tarul.cn/Article/details/gmxyfaadn.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gqyiflpcm.sHtML

PHP:  $argv;  $argc;
来源：http://3g.sjlbkw.cn/Article/details/gireywoxt.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.yfazqb.com/Article/details/gevjlfccg.sHtML

TS:   process.argv.slice(2)
来源：http://wap.tarul.cn/Article/details/gmpzuhora.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.tarul.cn/Article/details/gcqxzifmg.sHtML

Go:   os.Args[1:]
来源：http://3g.epnwcf.com/Article/details/gnkphnbxe.sHtML

Ruby: ARGV
来源：http://3g.bbcook.cn/Article/details/gxwkdtvys.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.tarul.cn/Article/details/gimhvkjzl.sHtML

[M02] 读取环境变量
来源：http://www.m.share.bbcook.cn/Article/details/gerohhuvj.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.bbcook.cn/Article/details/glkrtnwbx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.yfazqb.com/Article/details/guwsejxqg.sHtML

JS:   process.env.HOME
来源：http://3g.yfazqb.com/Article/details/gjwpppper.sHtML

TS:   process.env.HOME
来源：http://3g.fktsv.cn/Article/details/gztonzxkv.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gmgljsmfy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gclxsgtgp.sHtML

Ruby: ENV["HOME"]
来源：http://3g.bbcook.cn/Article/details/gqapkrbdl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gpmsuqiur.sHtML

[M03] 执行外部命令
来源：http://mobile.vehdjk.com/Article/details/gxeeaubit.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.epnwcf.com/Article/details/giouhfidh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.epnwcf.com/Article/details/gdkmryabc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.bbcook.cn/Article/details/gyoagfhrw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fktsv.cn/Article/details/gumxqkjhl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.epnwcf.com/Article/details/ghhhhdecc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.tarul.cn/Article/details/gmidedmjq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.vehdjk.com/Article/details/gegvqapis.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.yfazqb.com/Article/details/gbnymmykh.sHtML

[M04] 获取当前工作目录
来源：http://baike.sjlbkw.cn/Article/details/gwfwmykmp.sHtML

Py:   os.getcwd()
来源：http://m.share.vehdjk.com/Article/details/gukibxjwa.sHtML

PHP:  getcwd();
来源：http://baike.sjlbkw.cn/Article/details/gkredfhqi.sHtML

JS:   process.cwd()
来源：http://mobile.vehdjk.com/Article/details/guwrtkgaq.sHtML

TS:   process.cwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/ggybfgelz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.vehdjk.com/Article/details/gbfibvalt.sHtML

Go:   os.Getwd()
来源：http://wap.yfazqb.com/Article/details/gekoqnjnb.sHtML

Ruby: Dir.pwd
来源：http://blog.tarul.cn/Article/details/gywjxjogm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fktsv.cn/Article/details/ganypiksi.sHtML

[M05] 设置退出码
来源：http://www.share.yfazqb.com/Article/details/gyzjnfsue.sHtML

Py:   sys.exit(1)
来源：http://read.share.tarul.cn/Article/details/gmzygzohz.sHtML

PHP:  exit(1);
来源：http://3g.fktsv.cn/Article/details/gsifewffa.sHtML

JS:   process.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gjxogbtex.sHtML

TS:   process.exit(1)
来源：http://3g.bbcook.cn/Article/details/gtvxnubnx.sHtML

Java: System.exit(1)
来源：http://3g.tarul.cn/Article/details/gvvquvine.sHtML

Go:   os.Exit(1)
来源：http://3g.vehdjk.com/Article/details/gqpzvhiyv.sHtML

Ruby: exit 1
来源：http://baike.fktsv.cn/Article/details/gqclydesw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.epnwcf.com/Article/details/gjkubpnis.sHtML

[M06] 向标准错误输出
来源：http://3g.yfazqb.com/Article/details/gytqxffxs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fktsv.cn/Article/details/ghlsswtjp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.sjlbkw.cn/Article/details/gyplwkyrn.sHtML

JS:   console.error("err")
来源：http://read.share.sjlbkw.cn/Article/details/gipxtzxvz.sHtML

TS:   console.error("err")
来源：http://m.share.fktsv.cn/Article/details/gxivxmuds.sHtML

Java: System.err.println("err")
来源：http://mobile.tarul.cn/Article/details/gcefgvbea.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.vehdjk.com/Article/details/gduhqdjrl.sHtML

Ruby: warn "err"
来源：http://www.blog.bbcook.cn/Article/details/gawpbhpgw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.bbcook.cn/Article/details/gspyuonow.sHtML

[M07] 判断是否为主入口
来源：http://www.share.vehdjk.com/Article/details/gdcqfwhcf.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.bbcook.cn/Article/details/gxzwggoct.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.vehdjk.com/Article/details/gjekbtfqx.sHtML

JS:   require.main === module
来源：http://3g.sjlbkw.cn/Article/details/gpmmuteqg.sHtML

TS:   require.main === module
来源：http://read.share.epnwcf.com/Article/details/gyksffjbc.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.sjlbkw.cn/Article/details/ghadobyex.sHtML

Go:   func main()
来源：http://3g.epnwcf.com/Article/details/gziiykkla.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.epnwcf.com/Article/details/gpfogcydz.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fktsv.cn/Article/details/gchctkwyo.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.epnwcf.com/Article/details/geyovjqxx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fktsv.cn/Article/details/gnnzqpybj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.tarul.cn/Article/details/gbsgxlmyo.sHtML

JS:   process.platform;  process.version
来源：http://blog.vehdjk.com/Article/details/gvhpzpeml.sHtML

TS:   process.platform;  process.version
来源：http://mobile.yfazqb.com/Article/details/gzvvjwuzm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.bbcook.cn/Article/details/gcstwqwnn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.tarul.cn/Article/details/gnhsawgze.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fktsv.cn/Article/details/glfyzamxz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.sjlbkw.cn/Article/details/golprrqft.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/guhtucfbi.sHtML

N. 数据结构与算法
来源：http://baike.sjlbkw.cn/Article/details/gzqqvybkz.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gjayabwib.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.yfazqb.com/Article/details/ghczkibky.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gqfxvwilp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.yfazqb.com/Article/details/ggwykmcso.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fktsv.cn/Article/details/grbcwbijx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.vehdjk.com/Article/details/gwdddtzbu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.yfazqb.com/Article/details/gxaultlwo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gmumslziy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.epnwcf.com/Article/details/gsbrkjldx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gfrpfkhwn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.tarul.cn/Article/details/gxgfqcpin.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.epnwcf.com/Article/details/gecvekfmy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gotpwnvxw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.yfazqb.com/Article/details/gocgfioip.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/gnznlkluk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.vehdjk.com/Article/details/gkxoqvksh.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fktsv.cn/Article/details/ggecjffsz.sHtML

Ruby: arr.sort
来源：http://blog.vehdjk.com/Article/details/gfgtkdqvy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.bbcook.cn/Article/details/ggzssdzzx.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.vehdjk.com/Article/details/gkzpjamsx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.tarul.cn/Article/details/gwstciilc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.bbcook.cn/Article/details/ggkldzqzt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.vehdjk.com/Article/details/ggxmjosfm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.epnwcf.com/Article/details/grepodkta.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.yfazqb.com/Article/details/gcoicmfgg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.sjlbkw.cn/Article/details/gzdnznrmc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.tarul.cn/Article/details/givamqpwk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.yfazqb.com/Article/details/gzqpnvmoj.sHtML

[N04] 斐波那契数列
来源：http://baike.yfazqb.com/Article/details/ggxcyczdy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.epnwcf.com/Article/details/ghbrbaohe.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fktsv.cn/Article/details/gorlroeyn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/gqwmqarxk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/gmwywaoff.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.epnwcf.com/Article/details/gvlcheqrf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fktsv.cn/Article/details/gtzdzqbom.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.yfazqb.com/Article/details/gmuzqvcqo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.tarul.cn/Article/details/gmmzeunlq.sHtML

[N05] 最大公约数
来源：http://blog.fktsv.cn/Article/details/gprhvehax.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.yfazqb.com/Article/details/gsydpsbcd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.yfazqb.com/Article/details/gtrpvwrya.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.bbcook.cn/Article/details/gairalegk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fktsv.cn/Article/details/gvpidkmui.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.tarul.cn/Article/details/gjllahlnn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.epnwcf.com/Article/details/gtlybzbjh.sHtML

Ruby: a.gcd(b)
来源：http://m.share.sjlbkw.cn/Article/details/gvgefqyrh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.bbcook.cn/Article/details/gjupdmnxu.sHtML

[N06] 判断回文字符串
来源：http://blog.fktsv.cn/Article/details/goaprcexu.sHtML

Py:   s == s[::-1]
来源：http://read.share.bbcook.cn/Article/details/gzhfblcgp.sHtML

PHP:  $s === strrev($s);
来源：http://baike.epnwcf.com/Article/details/gtpvasfzn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/glrvwizlb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/gmewaodsd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.epnwcf.com/Article/details/gkyvygrgb.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.vehdjk.com/Article/details/glnltbynp.sHtML

Ruby: s == s.reverse
来源：http://3g.vehdjk.com/Article/details/gyidywrcr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.yfazqb.com/Article/details/gnidyqari.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.vehdjk.com/Article/details/grhhlyail.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.vehdjk.com/Article/details/gjbcwypuf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.epnwcf.com/Article/details/gwyrttoxl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.vehdjk.com/Article/details/gyritchsn.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.epnwcf.com/Article/details/gijerhrhv.sHtML

Java: // 手写 HashMap
来源：http://blog.epnwcf.com/Article/details/gxxhmpnqw.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.vehdjk.com/Article/details/gjqgdhcjw.sHtML

Ruby: // 手写 Hash
来源：http://baike.bbcook.cn/Article/details/ghglvtfxx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.vehdjk.com/Article/details/gtbecortp.sHtML

[N08] 生成全排列
来源：http://baike.tarul.cn/Article/details/gkzeconig.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.yfazqb.com/Article/details/guelzpnlk.sHtML

PHP:  // 手写递归交换
来源：http://www.share.vehdjk.com/Article/details/gnvqaevvi.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gmrztaebv.sHtML

TS:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gwnyqizbx.sHtML

Java: // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gdcfeywyz.sHtML

Go:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gjipzxofl.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.sjlbkw.cn/Article/details/gildriqfa.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gowfnfsye.sHtML

[N09] 栈与队列
来源：http://blog.epnwcf.com/Article/details/gdzjpvptf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.sjlbkw.cn/Article/details/gogoxvxyv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gdwxzzkaj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.tarul.cn/Article/details/gtmcdydui.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.bbcook.cn/Article/details/gvjsupetx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.epnwcf.com/Article/details/gmqjbrryp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fktsv.cn/Article/details/gwzxbygzn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.tarul.cn/Article/details/gwmxtcubl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.yfazqb.com/Article/details/glnfbqslg.sHtML

[N10] 链表节点定义
来源：http://mobile.fktsv.cn/Article/details/gwutlvzxs.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.vehdjk.com/Article/details/gsvqskshm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.vehdjk.com/Article/details/gjlotvokh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.vehdjk.com/Article/details/glnxjtuut.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.bbcook.cn/Article/details/gfnzdzorw.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fktsv.cn/Article/details/gdvxkwgjt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.yfazqb.com/Article/details/gqzaanzxn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fktsv.cn/Article/details/gbuigxdqp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.yfazqb.com/Article/details/grjnwuqbp.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.tarul.cn/Article/details/gerlpoyee.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.vehdjk.com/Article/details/gnnhvzhay.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.tarul.cn/Article/details/gtwhwbhcf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.bbcook.cn/Article/details/ghghvwtxo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.bbcook.cn/Article/details/gzfsgvakq.sHtML

Java: // 手写递归
来源：http://m.share.sjlbkw.cn/Article/details/grtalbyxp.sHtML

Go:   // 手写递归
来源：http://mobile.vehdjk.com/Article/details/gkjoprxyi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.epnwcf.com/Article/details/gesxdpxte.sHtML

C#:   // 手写递归
来源：http://3g.sjlbkw.cn/Article/details/glsskevau.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.tarul.cn/Article/details/grqeyaqvg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.bbcook.cn/Article/details/gvwtcfqwc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.yfazqb.com/Article/details/gabomhgxp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.tarul.cn/Article/details/gcxqmnptx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.epnwcf.com/Article/details/goplwcaxc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.epnwcf.com/Article/details/gpjzsksrp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fktsv.cn/Article/details/gltnymjnr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.vehdjk.com/Article/details/gmrrvkqra.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.epnwcf.com/Article/details/griofzqto.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gpkwognxi.sHtML

O. 并发与异步
来源：http://wap.sjlbkw.cn/Article/details/gxmfbevfz.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gyazyzzyh.sHtML

[O01] 启动一个线程
来源：http://mobile.vehdjk.com/Article/details/ggqyqhvky.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.epnwcf.com/Article/details/gfrossvse.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.yfazqb.com/Article/details/gcpnoktwj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fktsv.cn/Article/details/glambaopg.sHtML

TS:   // 同 JS
来源：http://read.share.tarul.cn/Article/details/glrfrukmt.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.vehdjk.com/Article/details/gjemzgtjk.sHtML

Go:   go f()
来源：http://m.share.vehdjk.com/Article/details/gkkuletid.sHtML

Ruby: Thread.new { f }
来源：http://www.share.vehdjk.com/Article/details/gtotqpdmj.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.yfazqb.com/Article/details/gflodyudz.sHtML

[O02] 使用线程池
来源：http://www.m.share.tarul.cn/Article/details/gcvcflzbl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.yfazqb.com/Article/details/gmofioony.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.bbcook.cn/Article/details/gxrqgvxof.sHtML

JS:   // worker_threads 线程池
来源：http://wap.yfazqb.com/Article/details/gqpmfyhoy.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.yfazqb.com/Article/details/gyppkirrs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.tarul.cn/Article/details/gmdbelpmc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.sjlbkw.cn/Article/details/gryfodgao.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.epnwcf.com/Article/details/gdqbwvzwz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.bbcook.cn/Article/details/gnmapzujw.sHtML

[O03] 加锁保护共享数据
来源：http://blog.tarul.cn/Article/details/gjyypsjjb.sHtML

Py:   with lock: shared += 1
来源：http://www.share.yfazqb.com/Article/details/gsnwuadhz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.sjlbkw.cn/Article/details/gsqqslmgv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.sjlbkw.cn/Article/details/glqqpdobn.sHtML

TS:   // 同 JS
来源：http://baike.yfazqb.com/Article/details/gzbujobgl.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fktsv.cn/Article/details/gipmxexmg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.vehdjk.com/Article/details/gcqghxevz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.tarul.cn/Article/details/gaskpmfxf.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.epnwcf.com/Article/details/gxrseqkkk.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.vehdjk.com/Article/details/gkaemfkei.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.tarul.cn/Article/details/gzxwbwphz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.yfazqb.com/Article/details/ghispetwx.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.epnwcf.com/Article/details/gpqtsoizz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.epnwcf.com/Article/details/gqxadenao.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.epnwcf.com/Article/details/gfkrxuyaf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.yfazqb.com/Article/details/gwekmhflj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.yfazqb.com/Article/details/gswceldqi.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.tarul.cn/Article/details/grldlkpbs.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.sjlbkw.cn/Article/details/gqimganbz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.epnwcf.com/Article/details/gefgzhbda.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.yfazqb.com/Article/details/gyufujiiz.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fktsv.cn/Article/details/ggkudperk.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.tarul.cn/Article/details/goqerdbfe.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.tarul.cn/Article/details/gsrhcnrva.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.sjlbkw.cn/Article/details/gdothdjvt.sHtML

Ruby: threads.map(&:join)
来源：http://wap.sjlbkw.cn/Article/details/gcgfdkpjz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.sjlbkw.cn/Article/details/ggospfxnn.sHtML


<!-- 参考信息 -->