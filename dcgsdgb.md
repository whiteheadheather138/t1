代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.yfazqb.com/Article/details/ghzoayclk.sHtML

JS:   await fetch(url)
来源：http://read.share.vehdjk.com/Article/details/gnvffmgoy.sHtML

TS:   await fetch(url)
来源：http://blog.sjlbkw.cn/Article/details/gcrqzwzvc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fktsv.cn/Article/details/gnxutinfb.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fktsv.cn/Article/details/gqfpqofhw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.yfazqb.com/Article/details/gefbhyfqk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.yfazqb.com/Article/details/gtqyyfzqz.sHtML

[L02] 发送 POST JSON
来源：http://read.share.sjlbkw.cn/Article/details/gxerngunk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.tarul.cn/Article/details/ghytfmaac.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.bbcook.cn/Article/details/gijuerzwb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.vehdjk.com/Article/details/gyokusvlv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.bbcook.cn/Article/details/gjjosltqa.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.bbcook.cn/Article/details/gerveihde.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.tarul.cn/Article/details/gbaytypti.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.sjlbkw.cn/Article/details/gmkocvqtf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.bbcook.cn/Article/details/gvjccxtju.sHtML

[L03] 设置自定义请求头
来源：http://blog.bbcook.cn/Article/details/gmbhahzsv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.bbcook.cn/Article/details/grgxdcylh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.tarul.cn/Article/details/gqfwthmgb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.epnwcf.com/Article/details/genapmpod.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.tarul.cn/Article/details/gjjkxlern.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.epnwcf.com/Article/details/gftkfvuva.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fktsv.cn/Article/details/gxznenxas.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.epnwcf.com/Article/details/ggwoyljpq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.vehdjk.com/Article/details/ghngbkfvn.sHtML

[L04] 设置超时
来源：http://wap.tarul.cn/Article/details/gbdrisdch.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.sjlbkw.cn/Article/details/gzxprtueq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.vehdjk.com/Article/details/ggahtgxlf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.yfazqb.com/Article/details/gxlhfdwxo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.yfazqb.com/Article/details/gdustkzvh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fktsv.cn/Article/details/gtvdvvipp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.vehdjk.com/Article/details/gfxscefll.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.yfazqb.com/Article/details/gpvkgljey.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.bbcook.cn/Article/details/ghgjaooba.sHtML

[L05] 上传文件（multipart）
来源：http://wap.vehdjk.com/Article/details/gkvhhtkhk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.sjlbkw.cn/Article/details/gpybzvlfq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.vehdjk.com/Article/details/ggxdvdjud.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.epnwcf.com/Article/details/gcmjuowgu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fktsv.cn/Article/details/gvcvidrtw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.sjlbkw.cn/Article/details/gnkiwfubb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fktsv.cn/Article/details/gbscannbz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.tarul.cn/Article/details/gecvlqmiw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fktsv.cn/Article/details/gtyqckcvv.sHtML

[L06] 解析响应为 JSON
来源：http://baike.bbcook.cn/Article/details/grtgdmzob.sHtML

Py:   resp.json()
来源：http://wap.epnwcf.com/Article/details/gitoemnjf.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.vehdjk.com/Article/details/gxjxlmmqm.sHtML

JS:   await resp.json()
来源：http://m.share.tarul.cn/Article/details/gwenuouew.sHtML

TS:   await resp.json()
来源：http://baike.fktsv.cn/Article/details/gklijcbtl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.epnwcf.com/Article/details/gwvdayztt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.epnwcf.com/Article/details/grrdlyjcl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fktsv.cn/Article/details/gqrwajaru.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fktsv.cn/Article/details/gvjhosjvv.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.vehdjk.com/Article/details/gshvvkxzi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.yfazqb.com/Article/details/gkrjeilvk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.tarul.cn/Article/details/gbemobsnv.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.vehdjk.com/Article/details/gaekvdtth.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fktsv.cn/Article/details/gbvhdgapd.sHtML

Java: resp.statusCode()
来源：http://blog.yfazqb.com/Article/details/glfrytrnx.sHtML

Go:   resp.StatusCode
来源：http://m.share.tarul.cn/Article/details/gyspcyfhd.sHtML

Ruby: resp.code.to_i
来源：http://wap.bbcook.cn/Article/details/gomvxlewn.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.yfazqb.com/Article/details/ghtnyqvhp.sHtML

[L08] 并发请求多个地址
来源：http://wap.tarul.cn/Article/details/gujuztcnh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.bbcook.cn/Article/details/grqnofmbm.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.yfazqb.com/Article/details/gfvhynmyd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/gozmpzjfe.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.sjlbkw.cn/Article/details/ghnavmzek.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fktsv.cn/Article/details/gfrrzbudr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.yfazqb.com/Article/details/gkbpbrxbr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.epnwcf.com/Article/details/gaqsjicxq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.vehdjk.com/Article/details/gnjjntfbk.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gqotxmgnb.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fktsv.cn/Article/details/gbdgmqdoz.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/grqenznbm.sHtML

[M01] 读取命令行参数
来源：http://www.blog.tarul.cn/Article/details/guluepeqo.sHtML

Py:   sys.argv[1:]
来源：http://mobile.bbcook.cn/Article/details/gaakkhntw.sHtML

PHP:  $argv;  $argc;
来源：http://baike.sjlbkw.cn/Article/details/gcudreggh.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.yfazqb.com/Article/details/gwuncrcci.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.bbcook.cn/Article/details/gtmpjwxsa.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.vehdjk.com/Article/details/gcuztdfgb.sHtML

Go:   os.Args[1:]
来源：http://wap.epnwcf.com/Article/details/gusjbgtzx.sHtML

Ruby: ARGV
来源：http://www.blog.fktsv.cn/Article/details/gujxdpoyq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.bbcook.cn/Article/details/gqglqsirq.sHtML

[M02] 读取环境变量
来源：http://wap.tarul.cn/Article/details/gtdyzjkwg.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.yfazqb.com/Article/details/gbwgkembk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.yfazqb.com/Article/details/gtsccsiig.sHtML

JS:   process.env.HOME
来源：http://mobile.sjlbkw.cn/Article/details/gpvqhaqin.sHtML

TS:   process.env.HOME
来源：http://mobile.fktsv.cn/Article/details/gswafzymx.sHtML

Java: System.getenv("HOME")
来源：http://3g.yfazqb.com/Article/details/ghdqpaudi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gxuzuzmsz.sHtML

Ruby: ENV["HOME"]
来源：http://blog.tarul.cn/Article/details/grxyzxrzd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.yfazqb.com/Article/details/gossgsvyj.sHtML

[M03] 执行外部命令
来源：http://mobile.yfazqb.com/Article/details/ghcjbxdzb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.sjlbkw.cn/Article/details/gckkumgcj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.epnwcf.com/Article/details/gtrxhweya.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fktsv.cn/Article/details/gjnucbxec.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.epnwcf.com/Article/details/gbgcxtqae.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.vehdjk.com/Article/details/gugfszwcr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.tarul.cn/Article/details/ggpssnqyh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.sjlbkw.cn/Article/details/gbgadtuso.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.yfazqb.com/Article/details/glrlkxqop.sHtML

[M04] 获取当前工作目录
来源：http://3g.fktsv.cn/Article/details/gwhoxcicd.sHtML

Py:   os.getcwd()
来源：http://www.share.vehdjk.com/Article/details/gujnodaqe.sHtML

PHP:  getcwd();
来源：http://3g.tarul.cn/Article/details/grvygwsvd.sHtML

JS:   process.cwd()
来源：http://wap.fktsv.cn/Article/details/gbwabsdnj.sHtML

TS:   process.cwd()
来源：http://m.share.fktsv.cn/Article/details/gukxcacqh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.sjlbkw.cn/Article/details/gfkyrulrx.sHtML

Go:   os.Getwd()
来源：http://read.share.vehdjk.com/Article/details/gaqmpbsic.sHtML

Ruby: Dir.pwd
来源：http://3g.tarul.cn/Article/details/grhogfzqz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.yfazqb.com/Article/details/gxvzbxsff.sHtML

[M05] 设置退出码
来源：http://blog.bbcook.cn/Article/details/gdbkoaavk.sHtML

Py:   sys.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gpoihokrv.sHtML

PHP:  exit(1);
来源：http://m.share.fktsv.cn/Article/details/gcgrcbhnh.sHtML

JS:   process.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gbhkybrmx.sHtML

TS:   process.exit(1)
来源：http://read.share.vehdjk.com/Article/details/ggeyeqmgs.sHtML

Java: System.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gpmlgtksq.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gyiqbcwqa.sHtML

Ruby: exit 1
来源：http://baike.fktsv.cn/Article/details/ghoyccbyj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.sjlbkw.cn/Article/details/grrpjrnnq.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.epnwcf.com/Article/details/gjaoyleuo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.vehdjk.com/Article/details/ggbbaaisw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.epnwcf.com/Article/details/gxdefmhhz.sHtML

JS:   console.error("err")
来源：http://wap.fktsv.cn/Article/details/gcwggijga.sHtML

TS:   console.error("err")
来源：http://3g.vehdjk.com/Article/details/gpeyuzapm.sHtML

Java: System.err.println("err")
来源：http://wap.fktsv.cn/Article/details/glkmgnktc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.vehdjk.com/Article/details/gluwpemtx.sHtML

Ruby: warn "err"
来源：http://www.blog.yfazqb.com/Article/details/gtgchvhct.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.yfazqb.com/Article/details/gumiyomwz.sHtML

[M07] 判断是否为主入口
来源：http://wap.tarul.cn/Article/details/gowiodyev.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.bbcook.cn/Article/details/gfvyadnkx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.vehdjk.com/Article/details/gouudnajr.sHtML

JS:   require.main === module
来源：http://blog.yfazqb.com/Article/details/glzxxlplx.sHtML

TS:   require.main === module
来源：http://blog.tarul.cn/Article/details/gztpevchb.sHtML

Java: public static void main(String[] args)
来源：http://m.share.vehdjk.com/Article/details/gmpfushgf.sHtML

Go:   func main()
来源：http://wap.sjlbkw.cn/Article/details/gaqajkqvp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.epnwcf.com/Article/details/gwuedqbqk.sHtML

C#:   static void Main(string[] args)
来源：http://wap.epnwcf.com/Article/details/gbaadfstk.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.tarul.cn/Article/details/gsmfuwgxz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.epnwcf.com/Article/details/ggfgvrpeq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.vehdjk.com/Article/details/gcawzqcmh.sHtML

JS:   process.platform;  process.version
来源：http://3g.fktsv.cn/Article/details/ghndifjyn.sHtML

TS:   process.platform;  process.version
来源：http://3g.sjlbkw.cn/Article/details/gnhencjlp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.tarul.cn/Article/details/gbovdulwh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.yfazqb.com/Article/details/glraiwqrc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.epnwcf.com/Article/details/gpjxjxyay.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.sjlbkw.cn/Article/details/gdvardouz.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gdjllsaen.sHtML

N. 数据结构与算法
来源：http://www.blog.bbcook.cn/Article/details/gtlisvnup.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gdkgxplbp.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.bbcook.cn/Article/details/gyykieiwo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.tarul.cn/Article/details/gequtruto.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.epnwcf.com/Article/details/ghvkcinry.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.tarul.cn/Article/details/geyrwjqma.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.yfazqb.com/Article/details/gsbkazjnq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.bbcook.cn/Article/details/gdudpmuhv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gixfkyhql.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.epnwcf.com/Article/details/grurvcdhm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.tarul.cn/Article/details/gdxcnwvpd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.bbcook.cn/Article/details/gykwbgnth.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.vehdjk.com/Article/details/grerfvopa.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.epnwcf.com/Article/details/gaputvdiv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.yfazqb.com/Article/details/gclwdqglo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fktsv.cn/Article/details/ggxncotre.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.sjlbkw.cn/Article/details/gpbvxgnvl.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.epnwcf.com/Article/details/gknvcqbzh.sHtML

Ruby: arr.sort
来源：http://m.share.fktsv.cn/Article/details/gatjpjogr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fktsv.cn/Article/details/gpkplnknz.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.yfazqb.com/Article/details/gxrmnkpkd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.tarul.cn/Article/details/glcmbcrit.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.sjlbkw.cn/Article/details/gpfftwojx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.tarul.cn/Article/details/gamdjlheq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.sjlbkw.cn/Article/details/ggszgypdl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.yfazqb.com/Article/details/gpiajnris.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fktsv.cn/Article/details/glbriueib.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fktsv.cn/Article/details/gokncfduw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.epnwcf.com/Article/details/gzcahnjqk.sHtML

[N04] 斐波那契数列
来源：http://3g.tarul.cn/Article/details/gakwwgmsf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fktsv.cn/Article/details/grbnuwbzo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.bbcook.cn/Article/details/gvsuobnzx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.epnwcf.com/Article/details/glcagamip.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.vehdjk.com/Article/details/grpxnclyr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.tarul.cn/Article/details/gtixoedtk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gelpkztlp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.vehdjk.com/Article/details/gpnkqolbi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.epnwcf.com/Article/details/gcbteyljp.sHtML

[N05] 最大公约数
来源：http://mobile.fktsv.cn/Article/details/glgsyzwtz.sHtML

Py:   math.gcd(a, b)
来源：http://wap.vehdjk.com/Article/details/grpwekoet.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.bbcook.cn/Article/details/gbjpmudcj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.vehdjk.com/Article/details/gnxthburq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fktsv.cn/Article/details/gxwoezffv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.epnwcf.com/Article/details/glrncevtn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.tarul.cn/Article/details/gvnmeuibd.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.epnwcf.com/Article/details/gwcmgscef.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.yfazqb.com/Article/details/gazkvwnxz.sHtML

[N06] 判断回文字符串
来源：http://baike.bbcook.cn/Article/details/gnxnrecxj.sHtML

Py:   s == s[::-1]
来源：http://3g.vehdjk.com/Article/details/gfsrkyryy.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.tarul.cn/Article/details/gyxcusyel.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.sjlbkw.cn/Article/details/ggaeynugg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gsdgqiwze.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.tarul.cn/Article/details/gimhproly.sHtML

Go:   // 双指针从两端比较
来源：http://3g.vehdjk.com/Article/details/gdfdjpglk.sHtML

Ruby: s == s.reverse
来源：http://3g.epnwcf.com/Article/details/gqbckyclq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.yfazqb.com/Article/details/gbiusldgq.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.vehdjk.com/Article/details/gunbjnyxi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.bbcook.cn/Article/details/gwoerurgv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.vehdjk.com/Article/details/gepcsiysc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fktsv.cn/Article/details/gtrwyynjm.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.bbcook.cn/Article/details/gcmrwzimx.sHtML

Java: // 手写 HashMap
来源：http://www.blog.tarul.cn/Article/details/gymvedelx.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.sjlbkw.cn/Article/details/ggljbjscw.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.epnwcf.com/Article/details/govxazbeh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fktsv.cn/Article/details/ghylcdpsp.sHtML

[N08] 生成全排列
来源：http://www.blog.vehdjk.com/Article/details/godfuhifv.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.yfazqb.com/Article/details/gkbyzhrob.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.tarul.cn/Article/details/goknvpndc.sHtML

JS:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/grzhzxuie.sHtML

TS:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gsvouuxnz.sHtML

Java: // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gxarnouqj.sHtML

Go:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gcokogusa.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.sjlbkw.cn/Article/details/gubovugjl.sHtML

C#:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gxcxrejfs.sHtML

[N09] 栈与队列
来源：http://www.m.share.bbcook.cn/Article/details/gsvuszcnf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.tarul.cn/Article/details/gybrissdj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fktsv.cn/Article/details/gzvidjgxl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.yfazqb.com/Article/details/gdbhqhaex.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.tarul.cn/Article/details/gldvwzeue.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.epnwcf.com/Article/details/grzdkqmeb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.sjlbkw.cn/Article/details/gzwycsbqe.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fktsv.cn/Article/details/gmolrwlue.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.yfazqb.com/Article/details/gmsbnsltu.sHtML

[N10] 链表节点定义
来源：http://www.blog.sjlbkw.cn/Article/details/ggzgdvlqx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.sjlbkw.cn/Article/details/gvjlpwuya.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.epnwcf.com/Article/details/gjcrvgkoq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fktsv.cn/Article/details/gkrzfjofo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.tarul.cn/Article/details/ggqikcfxt.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.bbcook.cn/Article/details/gllbatrfj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.vehdjk.com/Article/details/gsodncupi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.epnwcf.com/Article/details/gduceueny.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.tarul.cn/Article/details/gmdspetkh.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.tarul.cn/Article/details/gndhqtuij.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.vehdjk.com/Article/details/gnltfunbn.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.epnwcf.com/Article/details/gmomrmumo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.epnwcf.com/Article/details/griiprkvu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.sjlbkw.cn/Article/details/gjmiylpaq.sHtML

Java: // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/gqeheefch.sHtML

Go:   // 手写递归
来源：http://wap.bbcook.cn/Article/details/gegmkcsuf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.tarul.cn/Article/details/gckjsmotc.sHtML

C#:   // 手写递归
来源：http://www.share.bbcook.cn/Article/details/gzovyozqe.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.sjlbkw.cn/Article/details/gbaluhecg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.yfazqb.com/Article/details/gjjgycpen.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.vehdjk.com/Article/details/ghfamhuyx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fktsv.cn/Article/details/gzedrsgan.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.yfazqb.com/Article/details/gzdikpffx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.vehdjk.com/Article/details/gwtmuxuih.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.epnwcf.com/Article/details/gcofvtajh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.bbcook.cn/Article/details/gpfufqsxg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.tarul.cn/Article/details/gbdfoghhy.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gzpxfgwwn.sHtML

O. 并发与异步
来源：http://mobile.bbcook.cn/Article/details/gujohpgou.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gclopfjwc.sHtML

[O01] 启动一个线程
来源：http://mobile.sjlbkw.cn/Article/details/gdrxssseb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.yfazqb.com/Article/details/gtgangjfe.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.yfazqb.com/Article/details/gassfnfox.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.yfazqb.com/Article/details/gbgituyjj.sHtML

TS:   // 同 JS
来源：http://www.blog.vehdjk.com/Article/details/gafcoelmr.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.epnwcf.com/Article/details/goqjlaqim.sHtML

Go:   go f()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxkqbcghb.sHtML

Ruby: Thread.new { f }
来源：http://baike.tarul.cn/Article/details/gzgyvpjck.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.epnwcf.com/Article/details/guqnywgme.sHtML

[O02] 使用线程池
来源：http://read.share.fktsv.cn/Article/details/gvhazmlpd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.yfazqb.com/Article/details/gstiicrpw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fktsv.cn/Article/details/gfrjesbks.sHtML

JS:   // worker_threads 线程池
来源：http://baike.bbcook.cn/Article/details/gskensoui.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fktsv.cn/Article/details/goajyhgnr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.bbcook.cn/Article/details/gcltacays.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.sjlbkw.cn/Article/details/guqpiaduw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.vehdjk.com/Article/details/gzzlrnkne.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.bbcook.cn/Article/details/gurhqlgam.sHtML

[O03] 加锁保护共享数据
来源：http://baike.vehdjk.com/Article/details/gedyyfiym.sHtML

Py:   with lock: shared += 1
来源：http://blog.vehdjk.com/Article/details/ginsgmrvz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.epnwcf.com/Article/details/gsckqwcpe.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.vehdjk.com/Article/details/grdznsrce.sHtML

TS:   // 同 JS
来源：http://mobile.vehdjk.com/Article/details/ggizufjkn.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.epnwcf.com/Article/details/gtmodgcgi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.tarul.cn/Article/details/gacdwxeig.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fktsv.cn/Article/details/gvcbzwtgk.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.yfazqb.com/Article/details/gvnnivrwq.sHtML

[O04] 定义异步函数并等待
来源：http://blog.vehdjk.com/Article/details/gfyxhiktk.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.vehdjk.com/Article/details/ghqxjquwz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.yfazqb.com/Article/details/gavhcdmfm.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.yfazqb.com/Article/details/gppvgtdum.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.vehdjk.com/Article/details/gdatglfxy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fktsv.cn/Article/details/gbfrofpmm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.vehdjk.com/Article/details/gltixbvze.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.bbcook.cn/Article/details/gxulwusmn.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.yfazqb.com/Article/details/gusiyaljw.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fktsv.cn/Article/details/gkeoaltpk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.sjlbkw.cn/Article/details/gosnaeswg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.bbcook.cn/Article/details/gctsprplt.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.vehdjk.com/Article/details/grtrqlyxv.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.tarul.cn/Article/details/gzagcxwvr.sHtML


<!-- 参考信息 -->