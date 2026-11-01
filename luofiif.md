代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://www.blog.vehdjk.com/Article/details/gkzsoflrs.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.yfazqb.com/Article/details/gbmuydbto.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.sjlbkw.cn/Article/details/gdegptevb.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fktsv.cn/Article/details/gjajxjnge.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.bbcook.cn/Article/details/gpauyvssv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fktsv.cn/Article/details/gginymjjx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.sjlbkw.cn/Article/details/grhigqmkj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.tarul.cn/Article/details/guhyuduvn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.bbcook.cn/Article/details/gtmqwqnrw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.vehdjk.com/Article/details/gwmgcjpov.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.sjlbkw.cn/Article/details/gjspwrdmr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.epnwcf.com/Article/details/gmohgqfva.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fktsv.cn/Article/details/glndqcqcr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.vehdjk.com/Article/details/gulbqgded.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.yfazqb.com/Article/details/gyuxbeaoo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.yfazqb.com/Article/details/gruhwcnwk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fktsv.cn/Article/details/gpifbtsov.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.sjlbkw.cn/Article/details/gshwvgixq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.vehdjk.com/Article/details/ghqvslghy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fktsv.cn/Article/details/gkqtbarho.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/gdwehdajk.sHtML

[L04] 设置超时
来源：http://m.share.yfazqb.com/Article/details/gkouqhqfy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fktsv.cn/Article/details/gbnidyfpx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.bbcook.cn/Article/details/gbpgvxlhm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.sjlbkw.cn/Article/details/goybqhlwa.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.bbcook.cn/Article/details/gjiaapvqx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.yfazqb.com/Article/details/gntfynjsn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.vehdjk.com/Article/details/golwotrww.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.epnwcf.com/Article/details/gbwaoccra.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.bbcook.cn/Article/details/grqcrvvjg.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.sjlbkw.cn/Article/details/glcrxkajp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.epnwcf.com/Article/details/gdbklzyly.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.epnwcf.com/Article/details/gpgttewux.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.vehdjk.com/Article/details/gmhayvlxn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.vehdjk.com/Article/details/gmkhxqbkz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.epnwcf.com/Article/details/gzubzyyrk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.bbcook.cn/Article/details/gtqjbbbiw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.yfazqb.com/Article/details/gvrcrmqeg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.yfazqb.com/Article/details/gpecgmplu.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.sjlbkw.cn/Article/details/ghghdaugr.sHtML

Py:   resp.json()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpxtjfvcj.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.sjlbkw.cn/Article/details/gddtqfzwm.sHtML

JS:   await resp.json()
来源：http://www.m.share.tarul.cn/Article/details/gubshwpoi.sHtML

TS:   await resp.json()
来源：http://3g.epnwcf.com/Article/details/gdcnytcdb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.epnwcf.com/Article/details/giehavpge.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.sjlbkw.cn/Article/details/gabmrywsb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.vehdjk.com/Article/details/gisblpzso.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.sjlbkw.cn/Article/details/gqyqzvebe.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/guyrwtfcu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fktsv.cn/Article/details/gzjrupvjl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.tarul.cn/Article/details/gkohfphhs.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.vehdjk.com/Article/details/ggclgbnoy.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.tarul.cn/Article/details/gyyxqhfjf.sHtML

Java: resp.statusCode()
来源：http://blog.vehdjk.com/Article/details/glifshsay.sHtML

Go:   resp.StatusCode
来源：http://read.share.epnwcf.com/Article/details/gpiyfwztf.sHtML

Ruby: resp.code.to_i
来源：http://www.share.epnwcf.com/Article/details/gzcbhwhtu.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.bbcook.cn/Article/details/ggsmwgymr.sHtML

[L08] 并发请求多个地址
来源：http://wap.tarul.cn/Article/details/gskatdxuz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.bbcook.cn/Article/details/glmzxdzpj.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.sjlbkw.cn/Article/details/gkecxjjrz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.sjlbkw.cn/Article/details/gzmbfifje.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.sjlbkw.cn/Article/details/gwqyleiwo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.yfazqb.com/Article/details/gnxmwpvts.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.yfazqb.com/Article/details/gnycwsqgo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.bbcook.cn/Article/details/gdlgmluwp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.yfazqb.com/Article/details/grlvatful.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gkmsrznig.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.vehdjk.com/Article/details/gpgkakkgf.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gsgnisfhv.sHtML

[M01] 读取命令行参数
来源：http://www.blog.epnwcf.com/Article/details/gcribrvcs.sHtML

Py:   sys.argv[1:]
来源：http://blog.sjlbkw.cn/Article/details/guelclrhb.sHtML

PHP:  $argv;  $argc;
来源：http://wap.tarul.cn/Article/details/gfmmlpkce.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.tarul.cn/Article/details/grkpzfkoe.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.epnwcf.com/Article/details/gfqvtrsdb.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.epnwcf.com/Article/details/gdasvopte.sHtML

Go:   os.Args[1:]
来源：http://wap.fktsv.cn/Article/details/gqmxhpqwf.sHtML

Ruby: ARGV
来源：http://blog.vehdjk.com/Article/details/gelbozvmr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.bbcook.cn/Article/details/gunzrusvh.sHtML

[M02] 读取环境变量
来源：http://m.share.fktsv.cn/Article/details/gqibtztxf.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/grogaoxdy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.bbcook.cn/Article/details/gfukymbzc.sHtML

JS:   process.env.HOME
来源：http://mobile.vehdjk.com/Article/details/gtknhznzl.sHtML

TS:   process.env.HOME
来源：http://m.share.epnwcf.com/Article/details/gyhyawdqj.sHtML

Java: System.getenv("HOME")
来源：http://blog.yfazqb.com/Article/details/gdxymfduf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gbkfbobzi.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fktsv.cn/Article/details/ggevdklfa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.bbcook.cn/Article/details/gzlpsvelt.sHtML

[M03] 执行外部命令
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhqfrxpg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.epnwcf.com/Article/details/gdplgjjqs.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fktsv.cn/Article/details/gmiurvplm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.epnwcf.com/Article/details/gkdnfwbcz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.tarul.cn/Article/details/gnoxirjme.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.bbcook.cn/Article/details/gcdwkctxe.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fktsv.cn/Article/details/gjmhfbthh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.vehdjk.com/Article/details/gsxhlylqh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.epnwcf.com/Article/details/gsymhsamj.sHtML

[M04] 获取当前工作目录
来源：http://m.share.tarul.cn/Article/details/gjypxfyhw.sHtML

Py:   os.getcwd()
来源：http://www.blog.bbcook.cn/Article/details/gvfkjtynh.sHtML

PHP:  getcwd();
来源：http://baike.yfazqb.com/Article/details/gcpobwchu.sHtML

JS:   process.cwd()
来源：http://read.share.yfazqb.com/Article/details/gpmxskpxu.sHtML

TS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/gezfamkuz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.vehdjk.com/Article/details/gzvjbnwme.sHtML

Go:   os.Getwd()
来源：http://wap.sjlbkw.cn/Article/details/gkoxggbkb.sHtML

Ruby: Dir.pwd
来源：http://3g.yfazqb.com/Article/details/gkirhcfgo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.epnwcf.com/Article/details/glleyqsih.sHtML

[M05] 设置退出码
来源：http://baike.yfazqb.com/Article/details/grzodsvey.sHtML

Py:   sys.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/ggkfastql.sHtML

PHP:  exit(1);
来源：http://www.share.vehdjk.com/Article/details/gsghcbbwy.sHtML

JS:   process.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/ghirajwoh.sHtML

TS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gtamfpscq.sHtML

Java: System.exit(1)
来源：http://m.share.bbcook.cn/Article/details/ggnjrqayx.sHtML

Go:   os.Exit(1)
来源：http://baike.fktsv.cn/Article/details/gafthnpou.sHtML

Ruby: exit 1
来源：http://www.blog.sjlbkw.cn/Article/details/ghnrqbzdl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.epnwcf.com/Article/details/gybracvlb.sHtML

[M06] 向标准错误输出
来源：http://wap.vehdjk.com/Article/details/gdrbbzfds.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.bbcook.cn/Article/details/gqedmfztn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.vehdjk.com/Article/details/gwdcclmmq.sHtML

JS:   console.error("err")
来源：http://blog.vehdjk.com/Article/details/ggfcmmmhr.sHtML

TS:   console.error("err")
来源：http://www.share.vehdjk.com/Article/details/gmgrrkemn.sHtML

Java: System.err.println("err")
来源：http://www.m.share.epnwcf.com/Article/details/gwfkbfdmq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.vehdjk.com/Article/details/gggoncpqw.sHtML

Ruby: warn "err"
来源：http://mobile.sjlbkw.cn/Article/details/gmepxqqzu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fktsv.cn/Article/details/gkvoxnuql.sHtML

[M07] 判断是否为主入口
来源：http://www.share.sjlbkw.cn/Article/details/gzdvilwrp.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fktsv.cn/Article/details/gxvdbletg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.sjlbkw.cn/Article/details/gyzurxdft.sHtML

JS:   require.main === module
来源：http://wap.fktsv.cn/Article/details/gmbekqowe.sHtML

TS:   require.main === module
来源：http://www.share.epnwcf.com/Article/details/gjxhsuukf.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.yfazqb.com/Article/details/grduiajhp.sHtML

Go:   func main()
来源：http://www.blog.bbcook.cn/Article/details/gbkqrslwa.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.vehdjk.com/Article/details/gctpdcard.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.epnwcf.com/Article/details/ggoynlqzg.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fktsv.cn/Article/details/gtitnapba.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fktsv.cn/Article/details/gtyhddcdw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.bbcook.cn/Article/details/gwwbpkxob.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.bbcook.cn/Article/details/gdbbclyhi.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.tarul.cn/Article/details/ghuorfpod.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.bbcook.cn/Article/details/ghuqgoexg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.sjlbkw.cn/Article/details/gtcxohlts.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.vehdjk.com/Article/details/gzxccfnbf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.vehdjk.com/Article/details/gzldipmjx.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gpdrjfynr.sHtML

N. 数据结构与算法
来源：http://mobile.fktsv.cn/Article/details/galyrbfdz.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gxvnapwcb.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.sjlbkw.cn/Article/details/gsrzivfjt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gebwcypbg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.epnwcf.com/Article/details/gchedspgf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.tarul.cn/Article/details/ggbqpcjyz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.tarul.cn/Article/details/gesgdbmrm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gdmlsdnbv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gthblowvk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.vehdjk.com/Article/details/gkhqlhwbw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gwbvaipci.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.yfazqb.com/Article/details/grxyxnted.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fktsv.cn/Article/details/ghhjaqmcl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.bbcook.cn/Article/details/gxrbelrjm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/gxhrvmjsa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.yfazqb.com/Article/details/gizlkaiqo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.tarul.cn/Article/details/gfyhajpms.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gqltgkkgk.sHtML

Ruby: arr.sort
来源：http://www.m.share.epnwcf.com/Article/details/gzhtherxe.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.vehdjk.com/Article/details/gbwfjsufa.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.yfazqb.com/Article/details/gcjgrbcwe.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fktsv.cn/Article/details/gaclwcozs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.sjlbkw.cn/Article/details/giogirxel.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.epnwcf.com/Article/details/gkpnbjonv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.tarul.cn/Article/details/gsnzbokls.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.bbcook.cn/Article/details/gxvrauuzy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.vehdjk.com/Article/details/gmwptmypx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.yfazqb.com/Article/details/gimswvgyw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fktsv.cn/Article/details/gmbwvukwt.sHtML

[N04] 斐波那契数列
来源：http://3g.epnwcf.com/Article/details/ggbwkiccr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.epnwcf.com/Article/details/gqmjgxjik.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.sjlbkw.cn/Article/details/gtqyvczoo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.tarul.cn/Article/details/glqmqxzzr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.sjlbkw.cn/Article/details/gtokkbast.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.vehdjk.com/Article/details/ggwxytwov.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.epnwcf.com/Article/details/geuvmpxyv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.sjlbkw.cn/Article/details/gyzvrjskb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.vehdjk.com/Article/details/gktqkybxo.sHtML

[N05] 最大公约数
来源：http://www.m.share.fktsv.cn/Article/details/grysyifbt.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.sjlbkw.cn/Article/details/gvbqhfozs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.yfazqb.com/Article/details/gwdxazopt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.yfazqb.com/Article/details/gobwqrogj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.vehdjk.com/Article/details/gesfegdhl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.bbcook.cn/Article/details/givfralsa.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.tarul.cn/Article/details/gtdrdznwm.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.bbcook.cn/Article/details/gqquzrjcx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.sjlbkw.cn/Article/details/gmenbsfpj.sHtML

[N06] 判断回文字符串
来源：http://3g.tarul.cn/Article/details/gcylrenpp.sHtML

Py:   s == s[::-1]
来源：http://baike.tarul.cn/Article/details/gtxwghafp.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.bbcook.cn/Article/details/gkjmoqopw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/gozvdlsec.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gzgkzhkqc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.vehdjk.com/Article/details/gpyboknjs.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.tarul.cn/Article/details/gubsvtwmo.sHtML

Ruby: s == s.reverse
来源：http://baike.sjlbkw.cn/Article/details/gglkgdpea.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.sjlbkw.cn/Article/details/gupgkesdc.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.tarul.cn/Article/details/gfioapwms.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fktsv.cn/Article/details/gjzlpjhcl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.yfazqb.com/Article/details/gidhmaezu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.bbcook.cn/Article/details/gabbducep.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.vehdjk.com/Article/details/gzsenjwsy.sHtML

Java: // 手写 HashMap
来源：http://baike.vehdjk.com/Article/details/gewxvdjtj.sHtML

Go:   // 手写 map[int]int
来源：http://3g.tarul.cn/Article/details/gnpfxnipy.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fktsv.cn/Article/details/gjbvyhwni.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.epnwcf.com/Article/details/grmggdksz.sHtML

[N08] 生成全排列
来源：http://m.share.tarul.cn/Article/details/gotdshpxw.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.bbcook.cn/Article/details/groocaggh.sHtML

PHP:  // 手写递归交换
来源：http://www.share.epnwcf.com/Article/details/gbkxtsfup.sHtML

JS:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/geenecpiw.sHtML

TS:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gusduhjfm.sHtML

Java: // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gkloqbdze.sHtML

Go:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/gfxxplmvt.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fktsv.cn/Article/details/gwkdmuqmp.sHtML

C#:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/goxaisivf.sHtML

[N09] 栈与队列
来源：http://baike.sjlbkw.cn/Article/details/gcpfeawtc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.vehdjk.com/Article/details/gteivuoun.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fktsv.cn/Article/details/guwuizzjv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.vehdjk.com/Article/details/gooffeqkg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fktsv.cn/Article/details/gosjlhtgz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.bbcook.cn/Article/details/gucwotewl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.sjlbkw.cn/Article/details/ggljfupym.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/gerddqsma.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.sjlbkw.cn/Article/details/gljmonspy.sHtML

[N10] 链表节点定义
来源：http://blog.yfazqb.com/Article/details/gnccebpbp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.epnwcf.com/Article/details/gkbcvuxfm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.epnwcf.com/Article/details/gzgprddbv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.tarul.cn/Article/details/grcbrrmmd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.yfazqb.com/Article/details/glmmtifzk.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.tarul.cn/Article/details/gqqezmudd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fktsv.cn/Article/details/gdxhyfaif.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.vehdjk.com/Article/details/geilocwxy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.sjlbkw.cn/Article/details/gggetjeyi.sHtML

[N11] 二叉树中序遍历
来源：http://3g.bbcook.cn/Article/details/guugorazs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.tarul.cn/Article/details/gvfqvlzpr.sHtML

PHP:  // 手写递归函数
来源：http://wap.sjlbkw.cn/Article/details/gdwwjzqhl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/gcpjywcun.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fktsv.cn/Article/details/gjqpsqbmw.sHtML

Java: // 手写递归
来源：http://read.share.bbcook.cn/Article/details/gwrsxjlki.sHtML

Go:   // 手写递归
来源：http://blog.bbcook.cn/Article/details/gzntcwbto.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.yfazqb.com/Article/details/gjecjswtm.sHtML

C#:   // 手写递归
来源：http://3g.bbcook.cn/Article/details/grhgxaoit.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.yfazqb.com/Article/details/gtuaqvlij.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fktsv.cn/Article/details/gxxfjotbz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.tarul.cn/Article/details/ghegwoipv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.vehdjk.com/Article/details/gmrbhrbyl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.epnwcf.com/Article/details/gcoffvlmc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.vehdjk.com/Article/details/gcomalomu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fktsv.cn/Article/details/gmiwwegvp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.epnwcf.com/Article/details/gotfrfqpi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.vehdjk.com/Article/details/gudcpvqda.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/ghbtglyxe.sHtML

O. 并发与异步
来源：http://read.share.sjlbkw.cn/Article/details/gdunlovtv.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gjkepifrg.sHtML

[O01] 启动一个线程
来源：http://baike.bbcook.cn/Article/details/gdjrcicuu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.vehdjk.com/Article/details/gxekqisal.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fktsv.cn/Article/details/gkymtpspj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.tarul.cn/Article/details/gvsdjvopw.sHtML

TS:   // 同 JS
来源：http://www.share.epnwcf.com/Article/details/gxqezmvzc.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.tarul.cn/Article/details/gmhhlxdqm.sHtML

Go:   go f()
来源：http://read.share.fktsv.cn/Article/details/gbdwinanr.sHtML

Ruby: Thread.new { f }
来源：http://mobile.tarul.cn/Article/details/gmlufmtoi.sHtML

C#:   Task.Run(() => F());
来源：http://baike.epnwcf.com/Article/details/gwjypcfsu.sHtML

[O02] 使用线程池
来源：http://www.m.share.fktsv.cn/Article/details/gzzddrihy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.tarul.cn/Article/details/gzzqqpnrh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.yfazqb.com/Article/details/gflfghicm.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.yfazqb.com/Article/details/gelzuoeoe.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.yfazqb.com/Article/details/gmwhlwkac.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.epnwcf.com/Article/details/gyhiloxzw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.tarul.cn/Article/details/gjugmdypq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.bbcook.cn/Article/details/ghcmudssm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.sjlbkw.cn/Article/details/grjmtifcr.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.epnwcf.com/Article/details/gsoybwqkk.sHtML

Py:   with lock: shared += 1
来源：http://blog.tarul.cn/Article/details/glezoemex.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.sjlbkw.cn/Article/details/glepsidya.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.vehdjk.com/Article/details/gywvguyys.sHtML

TS:   // 同 JS
来源：http://baike.vehdjk.com/Article/details/gnenfutxx.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fktsv.cn/Article/details/gxcqvswck.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.tarul.cn/Article/details/gzpqgfnrg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.epnwcf.com/Article/details/gvbhnjeey.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.epnwcf.com/Article/details/gpkhmcovj.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.epnwcf.com/Article/details/gkffnsvny.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.bbcook.cn/Article/details/gtotmowlo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.sjlbkw.cn/Article/details/gyiiwwmlm.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.epnwcf.com/Article/details/gsfeidclb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fktsv.cn/Article/details/goadpebeb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.vehdjk.com/Article/details/gobxthcwf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.yfazqb.com/Article/details/grtrpygiw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.bbcook.cn/Article/details/goknwxeyd.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.bbcook.cn/Article/details/gweiusnpk.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.tarul.cn/Article/details/gkgylpyrx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.yfazqb.com/Article/details/gvlfsbkku.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.tarul.cn/Article/details/gxzmfbbre.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.yfazqb.com/Article/details/grhdykugs.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.epnwcf.com/Article/details/guuyzffki.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.bbcook.cn/Article/details/gszkzbpft.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.sjlbkw.cn/Article/details/glqxnesln.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.epnwcf.com/Article/details/grutzqxoy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.sjlbkw.cn/Article/details/gyzjydmnh.sHtML


<!-- 参考信息 -->