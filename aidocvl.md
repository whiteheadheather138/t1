代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fktsv.cn/Article/details/gtrmkvmsa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.tarul.cn/Article/details/grvxbxzcq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.epnwcf.com/Article/details/gicxrviys.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.vehdjk.com/Article/details/gmqdezrrv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.bbcook.cn/Article/details/gevezylcz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.sjlbkw.cn/Article/details/gegglxors.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.vehdjk.com/Article/details/gihtoqrdd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fktsv.cn/Article/details/gwcvwured.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.sjlbkw.cn/Article/details/gcaltceqx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.yfazqb.com/Article/details/gewymoofq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.sjlbkw.cn/Article/details/gugjvllbw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fktsv.cn/Article/details/gliuruhev.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fktsv.cn/Article/details/gpregzmqp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.bbcook.cn/Article/details/gjcwmtkxf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.sjlbkw.cn/Article/details/gedevxmho.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fktsv.cn/Article/details/gzjtqeceh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.vehdjk.com/Article/details/ghipnrjqk.sHtML

[L04] 设置超时
来源：http://blog.yfazqb.com/Article/details/gevfyouij.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.yfazqb.com/Article/details/gzwfccmlc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fktsv.cn/Article/details/gnqboamsp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.tarul.cn/Article/details/gceybhibh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.yfazqb.com/Article/details/gturavvoy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.bbcook.cn/Article/details/gdgrllhqn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.bbcook.cn/Article/details/gvskhbqbj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.yfazqb.com/Article/details/gepbylbwk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.yfazqb.com/Article/details/gpsbburbe.sHtML

[L05] 上传文件（multipart）
来源：http://baike.epnwcf.com/Article/details/gnmkhwcvg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.sjlbkw.cn/Article/details/gaaxijvbf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.bbcook.cn/Article/details/gwjjbgvta.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.vehdjk.com/Article/details/genholrwe.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.vehdjk.com/Article/details/gyrqoobpg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.sjlbkw.cn/Article/details/gimwyguri.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.bbcook.cn/Article/details/gaodtwrus.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.sjlbkw.cn/Article/details/gusfkftiw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gkysttgjo.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.epnwcf.com/Article/details/gwjdtahbj.sHtML

Py:   resp.json()
来源：http://mobile.yfazqb.com/Article/details/gzdmxeyvk.sHtML

PHP:  json_decode($body, true);
来源：http://blog.bbcook.cn/Article/details/gawkgqerr.sHtML

JS:   await resp.json()
来源：http://www.blog.bbcook.cn/Article/details/gzmwzwsuh.sHtML

TS:   await resp.json()
来源：http://www.blog.sjlbkw.cn/Article/details/gwnsjrtki.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fktsv.cn/Article/details/gkbwdbwfc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.yfazqb.com/Article/details/gmbojhfid.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fktsv.cn/Article/details/gqtaazvoa.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.sjlbkw.cn/Article/details/gnfiqfevj.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.vehdjk.com/Article/details/gdqztkswp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.epnwcf.com/Article/details/gtopixcyp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.yfazqb.com/Article/details/gtpdxwrdk.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.tarul.cn/Article/details/gmjknxnmq.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.bbcook.cn/Article/details/gjgvvklso.sHtML

Java: resp.statusCode()
来源：http://www.share.epnwcf.com/Article/details/glhuszptv.sHtML

Go:   resp.StatusCode
来源：http://blog.tarul.cn/Article/details/grgypresk.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.vehdjk.com/Article/details/gmshxbafl.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.tarul.cn/Article/details/gjyqiqeei.sHtML

[L08] 并发请求多个地址
来源：http://read.share.epnwcf.com/Article/details/gwqsoaooz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.sjlbkw.cn/Article/details/gjcdnacvw.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.bbcook.cn/Article/details/grsyzbbcf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.epnwcf.com/Article/details/gyfmyplpy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.tarul.cn/Article/details/gwdmcgzbc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.sjlbkw.cn/Article/details/gegjgfgkt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.sjlbkw.cn/Article/details/granybjpy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fktsv.cn/Article/details/gizzqqwcx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.bbcook.cn/Article/details/gnrgbivrk.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gmoirceou.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.sjlbkw.cn/Article/details/gozizedde.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gzaojkqse.sHtML

[M01] 读取命令行参数
来源：http://3g.fktsv.cn/Article/details/gcvqgymna.sHtML

Py:   sys.argv[1:]
来源：http://baike.fktsv.cn/Article/details/grqcrfkby.sHtML

PHP:  $argv;  $argc;
来源：http://baike.tarul.cn/Article/details/ggucidcun.sHtML

JS:   process.argv.slice(2)
来源：http://wap.tarul.cn/Article/details/ghlvgligd.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.tarul.cn/Article/details/glxdxiyjd.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.vehdjk.com/Article/details/gmmxfcmyz.sHtML

Go:   os.Args[1:]
来源：http://read.share.bbcook.cn/Article/details/gpblvqutv.sHtML

Ruby: ARGV
来源：http://wap.vehdjk.com/Article/details/gwdxhpomt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.epnwcf.com/Article/details/gripwgbth.sHtML

[M02] 读取环境变量
来源：http://3g.tarul.cn/Article/details/gvodzyxnm.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.yfazqb.com/Article/details/gapsasrbl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fktsv.cn/Article/details/gnxwqtnyn.sHtML

JS:   process.env.HOME
来源：http://read.share.yfazqb.com/Article/details/guewxanqm.sHtML

TS:   process.env.HOME
来源：http://www.m.share.bbcook.cn/Article/details/gdykkgapu.sHtML

Java: System.getenv("HOME")
来源：http://baike.epnwcf.com/Article/details/gesobxrad.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.bbcook.cn/Article/details/gczjldzyd.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.tarul.cn/Article/details/gsoofrxff.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.yfazqb.com/Article/details/gyvnlgjvg.sHtML

[M03] 执行外部命令
来源：http://www.blog.fktsv.cn/Article/details/gjgxuwjnl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.epnwcf.com/Article/details/giisugomh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.bbcook.cn/Article/details/grpkrbetz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.vehdjk.com/Article/details/gwkluexjs.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.yfazqb.com/Article/details/gxftwklfo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.epnwcf.com/Article/details/gpuhpnduy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.bbcook.cn/Article/details/gycylsgpc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.sjlbkw.cn/Article/details/gpzjcojry.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fktsv.cn/Article/details/gjfscvppm.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gmlfwvkwk.sHtML

Py:   os.getcwd()
来源：http://wap.epnwcf.com/Article/details/gsboriraq.sHtML

PHP:  getcwd();
来源：http://www.share.bbcook.cn/Article/details/gyukxcgiz.sHtML

JS:   process.cwd()
来源：http://www.blog.yfazqb.com/Article/details/gmcqnyobf.sHtML

TS:   process.cwd()
来源：http://3g.fktsv.cn/Article/details/ghsxbaicq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.vehdjk.com/Article/details/gbcbpgmvm.sHtML

Go:   os.Getwd()
来源：http://mobile.sjlbkw.cn/Article/details/gadbxnzdw.sHtML

Ruby: Dir.pwd
来源：http://m.share.epnwcf.com/Article/details/gwosmcrro.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.vehdjk.com/Article/details/garzvxtpu.sHtML

[M05] 设置退出码
来源：http://www.share.bbcook.cn/Article/details/gmjugeetu.sHtML

Py:   sys.exit(1)
来源：http://3g.vehdjk.com/Article/details/ggdqpwikk.sHtML

PHP:  exit(1);
来源：http://baike.yfazqb.com/Article/details/gsfxhivis.sHtML

JS:   process.exit(1)
来源：http://www.share.tarul.cn/Article/details/gifpnkuir.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gttixcykp.sHtML

Java: System.exit(1)
来源：http://baike.epnwcf.com/Article/details/gvdpuodow.sHtML

Go:   os.Exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gbtlajrug.sHtML

Ruby: exit 1
来源：http://mobile.fktsv.cn/Article/details/gbrmdndmt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.sjlbkw.cn/Article/details/gxoomhats.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.epnwcf.com/Article/details/gapbncabl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.vehdjk.com/Article/details/gwyeshldc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.bbcook.cn/Article/details/gjhlrzlyc.sHtML

JS:   console.error("err")
来源：http://m.share.tarul.cn/Article/details/grpzqrvzn.sHtML

TS:   console.error("err")
来源：http://read.share.yfazqb.com/Article/details/gkedgpxny.sHtML

Java: System.err.println("err")
来源：http://3g.tarul.cn/Article/details/gieqymrip.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fktsv.cn/Article/details/gqdobfdvi.sHtML

Ruby: warn "err"
来源：http://mobile.tarul.cn/Article/details/glltewbdo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fktsv.cn/Article/details/gapdkyhsm.sHtML

[M07] 判断是否为主入口
来源：http://wap.epnwcf.com/Article/details/ghbisipvs.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fktsv.cn/Article/details/gpprdrxcl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.vehdjk.com/Article/details/gxaxxvtrm.sHtML

JS:   require.main === module
来源：http://www.share.vehdjk.com/Article/details/gngqbhxbs.sHtML

TS:   require.main === module
来源：http://blog.tarul.cn/Article/details/gxgwdknia.sHtML

Java: public static void main(String[] args)
来源：http://m.share.vehdjk.com/Article/details/glqptnebl.sHtML

Go:   func main()
来源：http://baike.epnwcf.com/Article/details/ghjtytmjl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.bbcook.cn/Article/details/gadwynczs.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.tarul.cn/Article/details/gjujmvspm.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.sjlbkw.cn/Article/details/gordaunum.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fktsv.cn/Article/details/gpixsungt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.bbcook.cn/Article/details/gkicaeels.sHtML

JS:   process.platform;  process.version
来源：http://m.share.vehdjk.com/Article/details/gjkczoyrm.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.tarul.cn/Article/details/gnoifnuqt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fktsv.cn/Article/details/gkwxbzknu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.yfazqb.com/Article/details/gqzfjfygl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.vehdjk.com/Article/details/gqvgjipgu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.tarul.cn/Article/details/gnydjyyrr.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gwivyagvb.sHtML

N. 数据结构与算法
来源：http://www.share.tarul.cn/Article/details/gswijynou.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gjoojyrdn.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.tarul.cn/Article/details/gqydazztz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.bbcook.cn/Article/details/gbcwhtzfe.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.yfazqb.com/Article/details/giigvsmzc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.vehdjk.com/Article/details/gvvqzscfi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.bbcook.cn/Article/details/gbimygtgw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.vehdjk.com/Article/details/gmeqzihrh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gjwyltaal.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fktsv.cn/Article/details/gldpggtuq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.tarul.cn/Article/details/gwhutekiz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.bbcook.cn/Article/details/gvugvhqny.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.sjlbkw.cn/Article/details/gxsdoujwr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.yfazqb.com/Article/details/gkofuqygi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.epnwcf.com/Article/details/gzyqtcnix.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.yfazqb.com/Article/details/gjrgoaycl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.epnwcf.com/Article/details/gpdailjpy.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.tarul.cn/Article/details/gflxbrdhy.sHtML

Ruby: arr.sort
来源：http://m.share.fktsv.cn/Article/details/gyctmrbzb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fktsv.cn/Article/details/gzovvenkc.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.yfazqb.com/Article/details/gfsgowtvx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fktsv.cn/Article/details/goaxacseu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.bbcook.cn/Article/details/ghbroopxy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.bbcook.cn/Article/details/gyxipbhnv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.sjlbkw.cn/Article/details/gxooepxdg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.yfazqb.com/Article/details/gkbmbeszb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.sjlbkw.cn/Article/details/gdmowicdx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.bbcook.cn/Article/details/gzudctkuh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.epnwcf.com/Article/details/gnoyevmfr.sHtML

[N04] 斐波那契数列
来源：http://www.share.yfazqb.com/Article/details/gazwdfgnl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.bbcook.cn/Article/details/gnzqyvuvc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fktsv.cn/Article/details/gaefatzzy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.vehdjk.com/Article/details/ggbtxjjwe.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.bbcook.cn/Article/details/gfmsnmoef.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.tarul.cn/Article/details/gvaskdgic.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.tarul.cn/Article/details/gwfitawaq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.vehdjk.com/Article/details/gqtqomcni.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.epnwcf.com/Article/details/gyugdcwtk.sHtML

[N05] 最大公约数
来源：http://www.m.share.epnwcf.com/Article/details/gwkkcakib.sHtML

Py:   math.gcd(a, b)
来源：http://3g.sjlbkw.cn/Article/details/grihyaxev.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.yfazqb.com/Article/details/gktkbgskb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.bbcook.cn/Article/details/gnxkpbuly.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.tarul.cn/Article/details/gpratdebs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.bbcook.cn/Article/details/gscizthjd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.vehdjk.com/Article/details/gffnuveeo.sHtML

Ruby: a.gcd(b)
来源：http://read.share.bbcook.cn/Article/details/gtqghcbqn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.tarul.cn/Article/details/gxuhxtckf.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.epnwcf.com/Article/details/gwuolpeix.sHtML

Py:   s == s[::-1]
来源：http://read.share.epnwcf.com/Article/details/gkzhwzyxd.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.yfazqb.com/Article/details/gdmordvqq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gxtxxbnko.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/gdtyxwowi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.yfazqb.com/Article/details/gvfkulnyx.sHtML

Go:   // 双指针从两端比较
来源：http://baike.tarul.cn/Article/details/gytxjpzal.sHtML

Ruby: s == s.reverse
来源：http://blog.sjlbkw.cn/Article/details/gpveqetrp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.bbcook.cn/Article/details/giczqphvs.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.vehdjk.com/Article/details/gxpftphsq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.bbcook.cn/Article/details/gueckeaav.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.epnwcf.com/Article/details/gwnlyrqna.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.tarul.cn/Article/details/gxjsmmfhk.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.sjlbkw.cn/Article/details/gpkovuzbu.sHtML

Java: // 手写 HashMap
来源：http://m.share.vehdjk.com/Article/details/gglhcrxng.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.yfazqb.com/Article/details/gyjrrbtlf.sHtML

Ruby: // 手写 Hash
来源：http://www.share.epnwcf.com/Article/details/gxfmxxvon.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.epnwcf.com/Article/details/gsqcmsabn.sHtML

[N08] 生成全排列
来源：http://read.share.yfazqb.com/Article/details/gybtjtfyw.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.yfazqb.com/Article/details/gmuonahdp.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fktsv.cn/Article/details/gzvmyejtb.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gpvgwuhwh.sHtML

TS:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gqiyfwtie.sHtML

Java: // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/germfinss.sHtML

Go:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gohgfkqmc.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.bbcook.cn/Article/details/gawpwdzpy.sHtML

C#:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gzgaecsuw.sHtML

[N09] 栈与队列
来源：http://blog.bbcook.cn/Article/details/gwvjamqxr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.sjlbkw.cn/Article/details/gpysupchj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.yfazqb.com/Article/details/gwneoesty.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/gqckbqqvu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.yfazqb.com/Article/details/gnmteinjp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fktsv.cn/Article/details/gfyzqugep.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.vehdjk.com/Article/details/guusxdpdv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.epnwcf.com/Article/details/gjmgesxnb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.vehdjk.com/Article/details/galzjpawg.sHtML

[N10] 链表节点定义
来源：http://www.share.epnwcf.com/Article/details/gizvwzzmf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.tarul.cn/Article/details/gsqnnkftr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.tarul.cn/Article/details/garzjrpyo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.tarul.cn/Article/details/gkghpyjtt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.vehdjk.com/Article/details/gkzwczmva.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.vehdjk.com/Article/details/gmoftntyg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.sjlbkw.cn/Article/details/gevuarfjs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.vehdjk.com/Article/details/grsnistqn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.vehdjk.com/Article/details/gphhvcexk.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.bbcook.cn/Article/details/gkzryzkfv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.sjlbkw.cn/Article/details/geokclzhq.sHtML

PHP:  // 手写递归函数
来源：http://blog.yfazqb.com/Article/details/gfalsqjrj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.vehdjk.com/Article/details/gktstrfau.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.vehdjk.com/Article/details/gahotbthz.sHtML

Java: // 手写递归
来源：http://www.share.epnwcf.com/Article/details/gpadgftct.sHtML

Go:   // 手写递归
来源：http://read.share.epnwcf.com/Article/details/gexrhjugs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.sjlbkw.cn/Article/details/gckzpncxy.sHtML

C#:   // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/gwxzrfhhy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.bbcook.cn/Article/details/gwqwcwhsc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.sjlbkw.cn/Article/details/gdenkvqvj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fktsv.cn/Article/details/gognigzue.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/gnlmmmdsn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.yfazqb.com/Article/details/guywysakm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.epnwcf.com/Article/details/gqeikgdog.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.epnwcf.com/Article/details/gqtgoofpv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.vehdjk.com/Article/details/grvqkzgke.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.epnwcf.com/Article/details/guaozdpwq.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gbjrdxxjg.sHtML

O. 并发与异步
来源：http://www.blog.yfazqb.com/Article/details/gaemmtuhu.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gbvtvkfpp.sHtML

[O01] 启动一个线程
来源：http://baike.vehdjk.com/Article/details/gaygeujgp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.tarul.cn/Article/details/gmxqmrvyt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fktsv.cn/Article/details/gcspdhqmh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.bbcook.cn/Article/details/gmlziwycr.sHtML

TS:   // 同 JS
来源：http://m.share.fktsv.cn/Article/details/gygeonahk.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.vehdjk.com/Article/details/gpsvltuix.sHtML

Go:   go f()
来源：http://3g.sjlbkw.cn/Article/details/gyuansfup.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fktsv.cn/Article/details/gzpszgnoc.sHtML

C#:   Task.Run(() => F());
来源：http://3g.bbcook.cn/Article/details/gsaitrtpk.sHtML

[O02] 使用线程池
来源：http://www.blog.fktsv.cn/Article/details/gbaykqimj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.sjlbkw.cn/Article/details/gwgqfrgyh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fktsv.cn/Article/details/gckzekkll.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.sjlbkw.cn/Article/details/gayefhwzc.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.yfazqb.com/Article/details/gkzkfcavl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.sjlbkw.cn/Article/details/gqihofzmu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.bbcook.cn/Article/details/gavgrrcaz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fktsv.cn/Article/details/gxgaamycp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.sjlbkw.cn/Article/details/gmkunrhxd.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.epnwcf.com/Article/details/gzkzshtxc.sHtML

Py:   with lock: shared += 1
来源：http://3g.yfazqb.com/Article/details/gxeuvligs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.epnwcf.com/Article/details/gjufdgdof.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.bbcook.cn/Article/details/gavghdsep.sHtML

TS:   // 同 JS
来源：http://www.share.sjlbkw.cn/Article/details/grzcexmfa.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.yfazqb.com/Article/details/gmkpgujqi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.bbcook.cn/Article/details/gnmldygdg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.bbcook.cn/Article/details/gbwjtsfny.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.yfazqb.com/Article/details/gqltdopxk.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.epnwcf.com/Article/details/gcdtgrldy.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.vehdjk.com/Article/details/grbodapsa.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.yfazqb.com/Article/details/gggygevdr.sHtML

JS:   async function f() { await g(); }
来源：http://3g.vehdjk.com/Article/details/gsweyrgna.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.bbcook.cn/Article/details/gljyghesx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.yfazqb.com/Article/details/gszdsywee.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.yfazqb.com/Article/details/gxplkotdw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.tarul.cn/Article/details/ghgsoxbxn.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.yfazqb.com/Article/details/gpuonzdkc.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fktsv.cn/Article/details/gqooxjiox.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmodugyqo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.bbcook.cn/Article/details/gntykkpgv.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.bbcook.cn/Article/details/gnfhqguug.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.bbcook.cn/Article/details/gtowdkwdt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.bbcook.cn/Article/details/gwbwyuvbc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.bbcook.cn/Article/details/gdomyilov.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.epnwcf.com/Article/details/gdyjzbuvk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.epnwcf.com/Article/details/gbemhffej.sHtML

[O06] 使用进程池
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxgdwpec.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmnbjyut.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.vehdjk.com/Article/details/glgscjlhf.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.yfazqb.com/Article/details/gswfcqozt.sHtML


<!-- 参考信息 -->