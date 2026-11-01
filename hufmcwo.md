代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://blog.yfazqb.com/Article/details/gimilpebq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.yfazqb.com/Article/details/gnviolhar.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.tarul.cn/Article/details/gobgyhlgy.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fktsv.cn/Article/details/gyeoiidnt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.sjlbkw.cn/Article/details/gikjovbxg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.tarul.cn/Article/details/gqyxxjyqz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fktsv.cn/Article/details/gfovyciyc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.vehdjk.com/Article/details/ggfjybvuq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.yfazqb.com/Article/details/gwppidccd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.yfazqb.com/Article/details/gwtzpfjcq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.tarul.cn/Article/details/gyxwnfkym.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.sjlbkw.cn/Article/details/gxbuocevg.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzfbbqxt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.sjlbkw.cn/Article/details/gndjatprb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.sjlbkw.cn/Article/details/gegbakckx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.tarul.cn/Article/details/gkkfqovum.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.vehdjk.com/Article/details/gywtmfjvo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.tarul.cn/Article/details/gcowebybe.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.vehdjk.com/Article/details/gjptcjgpx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.bbcook.cn/Article/details/gynqnmamc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.epnwcf.com/Article/details/gsnnspxpz.sHtML

[L04] 设置超时
来源：http://blog.epnwcf.com/Article/details/gatvtjnox.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.bbcook.cn/Article/details/gvbpgajhk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.bbcook.cn/Article/details/gghihzwgn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.yfazqb.com/Article/details/gwtueifqp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.bbcook.cn/Article/details/guzvrjypn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.epnwcf.com/Article/details/gubnkmfwd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.vehdjk.com/Article/details/gfhltnfol.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.bbcook.cn/Article/details/gzrazqbfv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.epnwcf.com/Article/details/gwqvfblmj.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.vehdjk.com/Article/details/gexuktviq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.sjlbkw.cn/Article/details/gjzvbqnpa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.epnwcf.com/Article/details/gjmduwyls.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.vehdjk.com/Article/details/gxajchfrw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fktsv.cn/Article/details/guzuvnsbk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.sjlbkw.cn/Article/details/gufuzblmh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.sjlbkw.cn/Article/details/gapxueadn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.epnwcf.com/Article/details/gjnshsjyz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fktsv.cn/Article/details/gphskzlij.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.yfazqb.com/Article/details/gxjmrygtv.sHtML

Py:   resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/gypkmchjn.sHtML

PHP:  json_decode($body, true);
来源：http://baike.tarul.cn/Article/details/ghxnyfavh.sHtML

JS:   await resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/gvvkskaga.sHtML

TS:   await resp.json()
来源：http://blog.bbcook.cn/Article/details/ghjbpxcxt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.bbcook.cn/Article/details/gqqzktbiz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.yfazqb.com/Article/details/gmwspuvuz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fktsv.cn/Article/details/gxddtgmnu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.vehdjk.com/Article/details/gwjipbgqn.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.bbcook.cn/Article/details/grwwkogqm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.vehdjk.com/Article/details/gelokjczy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.yfazqb.com/Article/details/gfmfygxut.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.epnwcf.com/Article/details/givcqrmia.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fktsv.cn/Article/details/gdtelrdkh.sHtML

Java: resp.statusCode()
来源：http://m.share.sjlbkw.cn/Article/details/gxlvbjcxt.sHtML

Go:   resp.StatusCode
来源：http://wap.epnwcf.com/Article/details/gzqyygbef.sHtML

Ruby: resp.code.to_i
来源：http://m.share.vehdjk.com/Article/details/gqytkvnqk.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.yfazqb.com/Article/details/gvhpxcdwt.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fktsv.cn/Article/details/grbnjvmyp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.yfazqb.com/Article/details/gmwrfeoal.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.vehdjk.com/Article/details/ghceiiaob.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fktsv.cn/Article/details/gpbmlrgcm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.epnwcf.com/Article/details/gzyxjsdez.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.tarul.cn/Article/details/gbidwripb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fktsv.cn/Article/details/gjhumtsfw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.yfazqb.com/Article/details/gbjdalgwb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.vehdjk.com/Article/details/gbwjsghev.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/ganpymtmk.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.epnwcf.com/Article/details/gvxgzcndt.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/ghmxpzggj.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.epnwcf.com/Article/details/gwzmvtqgw.sHtML

Py:   sys.argv[1:]
来源：http://blog.sjlbkw.cn/Article/details/gupktzeph.sHtML

PHP:  $argv;  $argc;
来源：http://baike.epnwcf.com/Article/details/gpmsljndr.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.yfazqb.com/Article/details/gkjkwnbxy.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.vehdjk.com/Article/details/gypjegkke.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fktsv.cn/Article/details/gonmzsgoi.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fktsv.cn/Article/details/gnaalmraj.sHtML

Ruby: ARGV
来源：http://3g.yfazqb.com/Article/details/gujkuohhj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.bbcook.cn/Article/details/gpectfmky.sHtML

[M02] 读取环境变量
来源：http://m.share.sjlbkw.cn/Article/details/gcagaypxp.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.bbcook.cn/Article/details/gewsaaugd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.tarul.cn/Article/details/gppbljifb.sHtML

JS:   process.env.HOME
来源：http://m.share.sjlbkw.cn/Article/details/gjiygjyrw.sHtML

TS:   process.env.HOME
来源：http://wap.vehdjk.com/Article/details/gakjladdv.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gechqbjhe.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.bbcook.cn/Article/details/gobjfjzcw.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.epnwcf.com/Article/details/gholvwyhx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gubtanjsy.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fktsv.cn/Article/details/gultuxkau.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fktsv.cn/Article/details/glfapywze.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.tarul.cn/Article/details/gsprcmswy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.tarul.cn/Article/details/gpknsygyn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.sjlbkw.cn/Article/details/gnftlftkj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.tarul.cn/Article/details/gykpqhaev.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fktsv.cn/Article/details/gsggmyngx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.epnwcf.com/Article/details/ghoqttfrv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.vehdjk.com/Article/details/gxlltgspl.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fktsv.cn/Article/details/gvmnvnlhd.sHtML

Py:   os.getcwd()
来源：http://baike.fktsv.cn/Article/details/gvwqcpbqu.sHtML

PHP:  getcwd();
来源：http://3g.fktsv.cn/Article/details/gaogivfww.sHtML

JS:   process.cwd()
来源：http://wap.yfazqb.com/Article/details/gratacque.sHtML

TS:   process.cwd()
来源：http://read.share.epnwcf.com/Article/details/ggsozzjke.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.sjlbkw.cn/Article/details/ghteocqaa.sHtML

Go:   os.Getwd()
来源：http://3g.tarul.cn/Article/details/ggmljgxqm.sHtML

Ruby: Dir.pwd
来源：http://blog.fktsv.cn/Article/details/gbddmilhg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.sjlbkw.cn/Article/details/gjwmtauye.sHtML

[M05] 设置退出码
来源：http://mobile.fktsv.cn/Article/details/gjdwykulm.sHtML

Py:   sys.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gqsytqalu.sHtML

PHP:  exit(1);
来源：http://wap.epnwcf.com/Article/details/ghavhzkue.sHtML

JS:   process.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gqwacnxuq.sHtML

TS:   process.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gmivzdjyx.sHtML

Java: System.exit(1)
来源：http://baike.vehdjk.com/Article/details/geowzymel.sHtML

Go:   os.Exit(1)
来源：http://www.share.bbcook.cn/Article/details/guanmjbnq.sHtML

Ruby: exit 1
来源：http://3g.fktsv.cn/Article/details/gftyasqig.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.yfazqb.com/Article/details/goeklqlka.sHtML

[M06] 向标准错误输出
来源：http://read.share.tarul.cn/Article/details/gbtpdpuih.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.sjlbkw.cn/Article/details/gcdauvbtb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.tarul.cn/Article/details/gyfnzbafw.sHtML

JS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/giqsrjubn.sHtML

TS:   console.error("err")
来源：http://m.share.tarul.cn/Article/details/gfeeoawuo.sHtML

Java: System.err.println("err")
来源：http://blog.vehdjk.com/Article/details/gtepvixkr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.vehdjk.com/Article/details/gwdxqgprg.sHtML

Ruby: warn "err"
来源：http://read.share.fktsv.cn/Article/details/gptwuqaff.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.epnwcf.com/Article/details/gfegqnxdt.sHtML

[M07] 判断是否为主入口
来源：http://www.share.tarul.cn/Article/details/gpihmveec.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.epnwcf.com/Article/details/gdsmsmygz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fktsv.cn/Article/details/gkwmsydml.sHtML

JS:   require.main === module
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzmjjcyu.sHtML

TS:   require.main === module
来源：http://m.share.epnwcf.com/Article/details/gmtnvpaks.sHtML

Java: public static void main(String[] args)
来源：http://wap.tarul.cn/Article/details/grkwthpfa.sHtML

Go:   func main()
来源：http://baike.yfazqb.com/Article/details/gfipoilec.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.tarul.cn/Article/details/gqokecnhp.sHtML

C#:   static void Main(string[] args)
来源：http://3g.epnwcf.com/Article/details/gbtgesavy.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.vehdjk.com/Article/details/ghauxroaw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fktsv.cn/Article/details/gapzmaqvp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.yfazqb.com/Article/details/gadvupsnz.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzsyqans.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.bbcook.cn/Article/details/gxqmaontp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.sjlbkw.cn/Article/details/gflqmnnsm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.yfazqb.com/Article/details/gtcnlzimz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fktsv.cn/Article/details/gvqfznajh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.yfazqb.com/Article/details/gndcjlkko.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gbmfyxnil.sHtML

N. 数据结构与算法
来源：http://www.blog.bbcook.cn/Article/details/gyyolcmvh.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/ginhlfgtz.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.vehdjk.com/Article/details/gyzrahzvp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gytetnloi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.epnwcf.com/Article/details/gttqopeto.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/gxwpmluop.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/gunzidypp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gdhsakimy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.epnwcf.com/Article/details/gvjrkbmsj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.yfazqb.com/Article/details/gnkedkvpn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gmibazoox.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fktsv.cn/Article/details/gragzxkzv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fktsv.cn/Article/details/gfbvaqyin.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.vehdjk.com/Article/details/gkzlifglg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/garmbvxdj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.epnwcf.com/Article/details/golhoycpo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.bbcook.cn/Article/details/gsrjouyus.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fktsv.cn/Article/details/glolpxrxg.sHtML

Ruby: arr.sort
来源：http://m.share.bbcook.cn/Article/details/gahzrbybg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.bbcook.cn/Article/details/grkoxlczu.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fktsv.cn/Article/details/gzzxbldmz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.vehdjk.com/Article/details/gxasqtwec.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.yfazqb.com/Article/details/gdyuqhdha.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.sjlbkw.cn/Article/details/ginbunvlc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.sjlbkw.cn/Article/details/gurpqylrl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.vehdjk.com/Article/details/gvyfwmhnm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.epnwcf.com/Article/details/geviypncr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.epnwcf.com/Article/details/gzixeauhu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fktsv.cn/Article/details/gasrkckzk.sHtML

[N04] 斐波那契数列
来源：http://wap.fktsv.cn/Article/details/gkglvltzv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.epnwcf.com/Article/details/guvovfrba.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fktsv.cn/Article/details/gdbzoqdwp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/gelcetfgn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.tarul.cn/Article/details/giplibqit.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.vehdjk.com/Article/details/goivezgpb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.bbcook.cn/Article/details/gsqpzwcdw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.tarul.cn/Article/details/ggzupgjcz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/gninwkcae.sHtML

[N05] 最大公约数
来源：http://www.blog.yfazqb.com/Article/details/gjzqavcmi.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.bbcook.cn/Article/details/gryrhukei.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.yfazqb.com/Article/details/goitmmfmd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.yfazqb.com/Article/details/gkpswesrv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.epnwcf.com/Article/details/ghjxqacrt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.bbcook.cn/Article/details/gfvivljhi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.bbcook.cn/Article/details/gzewekxzm.sHtML

Ruby: a.gcd(b)
来源：http://3g.bbcook.cn/Article/details/gdktphkat.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.yfazqb.com/Article/details/gljqzrcwt.sHtML

[N06] 判断回文字符串
来源：http://blog.bbcook.cn/Article/details/gkjtjfzpg.sHtML

Py:   s == s[::-1]
来源：http://blog.vehdjk.com/Article/details/gyuoopoak.sHtML

PHP:  $s === strrev($s);
来源：http://baike.sjlbkw.cn/Article/details/grghoofxi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/geylleshw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gfiaxwfyr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.epnwcf.com/Article/details/gasnhbykb.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.vehdjk.com/Article/details/gwlxieken.sHtML

Ruby: s == s.reverse
来源：http://3g.tarul.cn/Article/details/glenjvqkp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.tarul.cn/Article/details/gtfvoqbyi.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.epnwcf.com/Article/details/gaqxwwawz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.vehdjk.com/Article/details/gdbxshfkn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.sjlbkw.cn/Article/details/gwabesgmu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.tarul.cn/Article/details/gvkasufbi.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.bbcook.cn/Article/details/grjtfplla.sHtML

Java: // 手写 HashMap
来源：http://blog.yfazqb.com/Article/details/gssnlnite.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fktsv.cn/Article/details/gmagokrzz.sHtML

Ruby: // 手写 Hash
来源：http://mobile.epnwcf.com/Article/details/gowgtlhvw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.bbcook.cn/Article/details/guqhvyjhi.sHtML

[N08] 生成全排列
来源：http://m.share.epnwcf.com/Article/details/gfpeuvxli.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.bbcook.cn/Article/details/gylgneqbj.sHtML

PHP:  // 手写递归交换
来源：http://m.share.sjlbkw.cn/Article/details/gjuctpgqp.sHtML

JS:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gubfkwcli.sHtML

TS:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gpnmslatu.sHtML

Java: // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/ghqjdoygj.sHtML

Go:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/geabdxnph.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.epnwcf.com/Article/details/gosnnufmt.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gjfdbkjhv.sHtML

[N09] 栈与队列
来源：http://www.share.bbcook.cn/Article/details/guuvxkylm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.vehdjk.com/Article/details/ghbmukvfn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.epnwcf.com/Article/details/gnodvgmyg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.tarul.cn/Article/details/gwfyttsfr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.yfazqb.com/Article/details/gzyuwcffa.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.sjlbkw.cn/Article/details/gmofpvjlj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.epnwcf.com/Article/details/gfvmlifcf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.yfazqb.com/Article/details/gqdhakgcv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fktsv.cn/Article/details/gnbfoolog.sHtML

[N10] 链表节点定义
来源：http://www.share.vehdjk.com/Article/details/ggpacjdso.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.tarul.cn/Article/details/goaysqryp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.sjlbkw.cn/Article/details/geuppigkd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.yfazqb.com/Article/details/gmzswdyil.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.bbcook.cn/Article/details/gdnftgzel.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.bbcook.cn/Article/details/gijiwskxc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.bbcook.cn/Article/details/gkfrbaudv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.bbcook.cn/Article/details/gamvwyeus.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.bbcook.cn/Article/details/gsdkhuyvg.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.epnwcf.com/Article/details/gudallrbc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fktsv.cn/Article/details/gzkiaahyh.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.tarul.cn/Article/details/gjkyjhiob.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/gkihwodla.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.yfazqb.com/Article/details/gepidmnyr.sHtML

Java: // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/gmacmujni.sHtML

Go:   // 手写递归
来源：http://3g.yfazqb.com/Article/details/gtvayidul.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.vehdjk.com/Article/details/gnmxyzpla.sHtML

C#:   // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/glzelrbyr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.tarul.cn/Article/details/gdxrzngkl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.yfazqb.com/Article/details/gljymsupl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.yfazqb.com/Article/details/ggtdevuzu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.bbcook.cn/Article/details/gbrqykrvj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.vehdjk.com/Article/details/gdvczogmi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.vehdjk.com/Article/details/grpmljdqc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.vehdjk.com/Article/details/gejojxlso.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.epnwcf.com/Article/details/gizthqjwj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gnhcoourv.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gjikufqtq.sHtML

O. 并发与异步
来源：http://read.share.vehdjk.com/Article/details/grlcxgkkx.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gbvdlnmwx.sHtML

[O01] 启动一个线程
来源：http://wap.bbcook.cn/Article/details/gfusevvhy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.vehdjk.com/Article/details/gohtkyskm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.vehdjk.com/Article/details/gbdqhqeui.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fktsv.cn/Article/details/ghyppdnok.sHtML

TS:   // 同 JS
来源：http://www.m.share.bbcook.cn/Article/details/girglwycq.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.sjlbkw.cn/Article/details/gmfvbarfg.sHtML

Go:   go f()
来源：http://mobile.sjlbkw.cn/Article/details/gksyhedhb.sHtML

Ruby: Thread.new { f }
来源：http://m.share.sjlbkw.cn/Article/details/gotknevjg.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.tarul.cn/Article/details/gvkpbtxvb.sHtML

[O02] 使用线程池
来源：http://3g.epnwcf.com/Article/details/gyxiybqfw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fktsv.cn/Article/details/gvomxqzvn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.sjlbkw.cn/Article/details/gmuouhsef.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.epnwcf.com/Article/details/gvjiikver.sHtML

TS:   // worker_threads 线程池
来源：http://baike.bbcook.cn/Article/details/gppmgnvgb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.sjlbkw.cn/Article/details/goqyzrcpf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fktsv.cn/Article/details/guisfeimg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.sjlbkw.cn/Article/details/gbscsraae.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.yfazqb.com/Article/details/gzayymdlj.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.tarul.cn/Article/details/ggborljzm.sHtML

Py:   with lock: shared += 1
来源：http://blog.epnwcf.com/Article/details/gerxpwbfl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.sjlbkw.cn/Article/details/gtywjrmuc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.yfazqb.com/Article/details/gloiyntsk.sHtML

TS:   // 同 JS
来源：http://www.share.bbcook.cn/Article/details/gifdxcmap.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.bbcook.cn/Article/details/guglrswbe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.epnwcf.com/Article/details/gmitpdnnp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.bbcook.cn/Article/details/gkfzbkegb.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdbtpjcqt.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.bbcook.cn/Article/details/gwmdyhzfb.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.bbcook.cn/Article/details/gkrdvneqk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.tarul.cn/Article/details/gwsfygdud.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.tarul.cn/Article/details/gcojgtycf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.tarul.cn/Article/details/gtubckhjj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.sjlbkw.cn/Article/details/gwerlthgz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.vehdjk.com/Article/details/grfeilrbc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.epnwcf.com/Article/details/gbnnlhhqi.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsryolghj.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.tarul.cn/Article/details/gplvcpisr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fktsv.cn/Article/details/gynltacjf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.yfazqb.com/Article/details/gqrmmnput.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.vehdjk.com/Article/details/gcwdqtysb.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.vehdjk.com/Article/details/gpnsvcali.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.vehdjk.com/Article/details/gndwmftey.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fktsv.cn/Article/details/gnbqclaao.sHtML

Ruby: threads.map(&:join)
来源：http://wap.tarul.cn/Article/details/gudhrdrmp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.tarul.cn/Article/details/ghwdcqxmi.sHtML


<!-- 参考信息 -->