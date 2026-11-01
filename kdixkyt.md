代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.sjlbkw.cn/Article/details/gxiacjnbc.sHtML

JS:   await fetch(url)
来源：http://baike.vehdjk.com/Article/details/gtkcxbrkz.sHtML

TS:   await fetch(url)
来源：http://3g.fktsv.cn/Article/details/gtbpnbnvn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.vehdjk.com/Article/details/ghvhlennk.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.epnwcf.com/Article/details/gyqrlmuzr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.epnwcf.com/Article/details/gdjfeirbd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.sjlbkw.cn/Article/details/gdruqmeus.sHtML

[L02] 发送 POST JSON
来源：http://m.share.sjlbkw.cn/Article/details/giarpqlvq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.sjlbkw.cn/Article/details/gxaqizxhq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.epnwcf.com/Article/details/gtqboeplh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.bbcook.cn/Article/details/gclzqjfjm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.sjlbkw.cn/Article/details/gdluesshj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.vehdjk.com/Article/details/gthmdohue.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.tarul.cn/Article/details/gadnpprhq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.vehdjk.com/Article/details/gnoqsgqez.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtjhytgs.sHtML

[L03] 设置自定义请求头
来源：http://m.share.vehdjk.com/Article/details/gjlvrliun.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.bbcook.cn/Article/details/ghejknkhq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.epnwcf.com/Article/details/gvzhdswkc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.vehdjk.com/Article/details/gepncftoz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.yfazqb.com/Article/details/ghmkdqzyq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.vehdjk.com/Article/details/gaghukzbo.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.bbcook.cn/Article/details/guqkgkoot.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.sjlbkw.cn/Article/details/ghmwcwmlb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.sjlbkw.cn/Article/details/gxxiebopd.sHtML

[L04] 设置超时
来源：http://m.share.fktsv.cn/Article/details/ggybehffm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.tarul.cn/Article/details/guilkmqbu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.sjlbkw.cn/Article/details/gucvgdoug.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.vehdjk.com/Article/details/gghcmbzud.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.sjlbkw.cn/Article/details/gatxddxti.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.bbcook.cn/Article/details/ghlsrrgkj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.bbcook.cn/Article/details/gwwbobzcr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.vehdjk.com/Article/details/gxugfgvix.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.yfazqb.com/Article/details/gidgxcdsb.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.tarul.cn/Article/details/gkutiujge.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.yfazqb.com/Article/details/gbydueltq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.yfazqb.com/Article/details/grequxdwr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.yfazqb.com/Article/details/gksvnrwwf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.sjlbkw.cn/Article/details/ghciesgta.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.sjlbkw.cn/Article/details/gpqlythjm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.vehdjk.com/Article/details/gixmurtqn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.tarul.cn/Article/details/gqqcrftxg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.vehdjk.com/Article/details/ghxhevhiz.sHtML

[L06] 解析响应为 JSON
来源：http://blog.sjlbkw.cn/Article/details/gttkjpdxf.sHtML

Py:   resp.json()
来源：http://blog.yfazqb.com/Article/details/gwqowoqbz.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.vehdjk.com/Article/details/glgmeybxp.sHtML

JS:   await resp.json()
来源：http://www.share.tarul.cn/Article/details/gqcizmxov.sHtML

TS:   await resp.json()
来源：http://read.share.yfazqb.com/Article/details/gwsyeaujl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.bbcook.cn/Article/details/gyyvbplue.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.epnwcf.com/Article/details/glkoyjczy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fktsv.cn/Article/details/guperpmkp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.vehdjk.com/Article/details/gzfyaysvy.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.bbcook.cn/Article/details/gxxxupqar.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fktsv.cn/Article/details/gsllybedr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.sjlbkw.cn/Article/details/gtztyphes.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.yfazqb.com/Article/details/gyqtiobwp.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.vehdjk.com/Article/details/glsvesfli.sHtML

Java: resp.statusCode()
来源：http://read.share.tarul.cn/Article/details/gaefsursk.sHtML

Go:   resp.StatusCode
来源：http://3g.vehdjk.com/Article/details/gsblmobvm.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fktsv.cn/Article/details/gwoaanakg.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fktsv.cn/Article/details/ggrgfjafp.sHtML

[L08] 并发请求多个地址
来源：http://mobile.vehdjk.com/Article/details/gbieqfmyq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.vehdjk.com/Article/details/gglmucdql.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.bbcook.cn/Article/details/gijzwkkea.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/gnwycdijz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fktsv.cn/Article/details/gonsydiph.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.yfazqb.com/Article/details/gvfnckoci.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fktsv.cn/Article/details/gmuuinmqr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.epnwcf.com/Article/details/gxwvowaam.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gkoxnhucy.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gmpvjfhbi.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.sjlbkw.cn/Article/details/gxoaqbcbt.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/grcsksezh.sHtML

[M01] 读取命令行参数
来源：http://m.share.vehdjk.com/Article/details/gfpuxgcwc.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.yfazqb.com/Article/details/gdatnyasx.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.bbcook.cn/Article/details/gjdqairbz.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.bbcook.cn/Article/details/gfozegkbn.sHtML

TS:   process.argv.slice(2)
来源：http://3g.epnwcf.com/Article/details/gcrndeyuz.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.bbcook.cn/Article/details/gdlzriqtp.sHtML

Go:   os.Args[1:]
来源：http://m.share.vehdjk.com/Article/details/gbwzsfqho.sHtML

Ruby: ARGV
来源：http://read.share.fktsv.cn/Article/details/gtbstzpoe.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.yfazqb.com/Article/details/ghmarqqlh.sHtML

[M02] 读取环境变量
来源：http://baike.sjlbkw.cn/Article/details/gxwxwpfja.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.yfazqb.com/Article/details/gyxzegybn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.vehdjk.com/Article/details/gvdwrdrtq.sHtML

JS:   process.env.HOME
来源：http://read.share.yfazqb.com/Article/details/gxyibpbsa.sHtML

TS:   process.env.HOME
来源：http://www.blog.yfazqb.com/Article/details/gddhffqig.sHtML

Java: System.getenv("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gotcftsla.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.tarul.cn/Article/details/gynhovpiz.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.tarul.cn/Article/details/gbnrfziwg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gxhbiikva.sHtML

[M03] 执行外部命令
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbtmqxyi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.tarul.cn/Article/details/glapwwnyn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.yfazqb.com/Article/details/gywxcgasb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.vehdjk.com/Article/details/gpmqthobp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.yfazqb.com/Article/details/gdmpfceic.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.bbcook.cn/Article/details/gtxvxmrnd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.bbcook.cn/Article/details/gimhhtbuf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.vehdjk.com/Article/details/gpyntxykd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.yfazqb.com/Article/details/gqinnfjga.sHtML

[M04] 获取当前工作目录
来源：http://baike.sjlbkw.cn/Article/details/gixpunkav.sHtML

Py:   os.getcwd()
来源：http://www.blog.fktsv.cn/Article/details/ggycjttli.sHtML

PHP:  getcwd();
来源：http://www.m.share.yfazqb.com/Article/details/gztniiyun.sHtML

JS:   process.cwd()
来源：http://www.blog.fktsv.cn/Article/details/gfdsbebju.sHtML

TS:   process.cwd()
来源：http://blog.epnwcf.com/Article/details/glzgqpbbm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fktsv.cn/Article/details/glznpqumj.sHtML

Go:   os.Getwd()
来源：http://mobile.tarul.cn/Article/details/goeydgohf.sHtML

Ruby: Dir.pwd
来源：http://mobile.vehdjk.com/Article/details/gshrrjlta.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.bbcook.cn/Article/details/gfjkyxzgv.sHtML

[M05] 设置退出码
来源：http://www.share.vehdjk.com/Article/details/gstdvgkev.sHtML

Py:   sys.exit(1)
来源：http://baike.yfazqb.com/Article/details/gtaqeahdq.sHtML

PHP:  exit(1);
来源：http://3g.vehdjk.com/Article/details/gljfjyasr.sHtML

JS:   process.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gupvtcpsj.sHtML

TS:   process.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/guguvidtw.sHtML

Java: System.exit(1)
来源：http://baike.vehdjk.com/Article/details/gmgllpecf.sHtML

Go:   os.Exit(1)
来源：http://m.share.fktsv.cn/Article/details/gmsinoalf.sHtML

Ruby: exit 1
来源：http://wap.epnwcf.com/Article/details/ggiyrkhdo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.tarul.cn/Article/details/ghnbmznbo.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.epnwcf.com/Article/details/gyojevtbv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fktsv.cn/Article/details/giebutkqu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.epnwcf.com/Article/details/golygaolg.sHtML

JS:   console.error("err")
来源：http://wap.epnwcf.com/Article/details/gjhttzvzc.sHtML

TS:   console.error("err")
来源：http://www.m.share.yfazqb.com/Article/details/gzwatzdax.sHtML

Java: System.err.println("err")
来源：http://baike.epnwcf.com/Article/details/gyvyfgvnw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fktsv.cn/Article/details/gpjqgfbll.sHtML

Ruby: warn "err"
来源：http://www.share.epnwcf.com/Article/details/gvnweloag.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.yfazqb.com/Article/details/gtuukqoks.sHtML

[M07] 判断是否为主入口
来源：http://baike.bbcook.cn/Article/details/graktegek.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fktsv.cn/Article/details/gbbmjoown.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.tarul.cn/Article/details/givhrmbdn.sHtML

JS:   require.main === module
来源：http://mobile.yfazqb.com/Article/details/gdlgdswub.sHtML

TS:   require.main === module
来源：http://3g.epnwcf.com/Article/details/ggsbgfmma.sHtML

Java: public static void main(String[] args)
来源：http://wap.sjlbkw.cn/Article/details/gfovsmdlj.sHtML

Go:   func main()
来源：http://blog.fktsv.cn/Article/details/gndawlbdk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.sjlbkw.cn/Article/details/gopujiart.sHtML

C#:   static void Main(string[] args)
来源：http://baike.tarul.cn/Article/details/gxhvvrdth.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.epnwcf.com/Article/details/gmofudwnj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fktsv.cn/Article/details/gurmhqbpj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.sjlbkw.cn/Article/details/gptmbjeme.sHtML

JS:   process.platform;  process.version
来源：http://www.share.epnwcf.com/Article/details/gvrbeviwb.sHtML

TS:   process.platform;  process.version
来源：http://baike.tarul.cn/Article/details/glueynkok.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.vehdjk.com/Article/details/gvfaslmjw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.epnwcf.com/Article/details/guuvvlmkn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.sjlbkw.cn/Article/details/giqenzmsw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.tarul.cn/Article/details/gdmwipkrj.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gjvgdcqsq.sHtML

N. 数据结构与算法
来源：http://www.m.share.sjlbkw.cn/Article/details/gzsogfzqu.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gdokoqptj.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.bbcook.cn/Article/details/gvwrxwuus.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gwvdxxvek.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gcimglxch.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gukzgnkrx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gmkaetohq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gdccfbeij.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.tarul.cn/Article/details/gwooeftfa.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.bbcook.cn/Article/details/ggfizwobd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.epnwcf.com/Article/details/gxtsgevmh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.epnwcf.com/Article/details/gjlssjhhf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fktsv.cn/Article/details/gczsdkehq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.vehdjk.com/Article/details/gcgypyvzu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.bbcook.cn/Article/details/gosezactz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/ghulnxdry.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.epnwcf.com/Article/details/gifwevzoj.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.tarul.cn/Article/details/gbmfjzojr.sHtML

Ruby: arr.sort
来源：http://m.share.tarul.cn/Article/details/gqvfwwfbv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.yfazqb.com/Article/details/gwxzbvecf.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.vehdjk.com/Article/details/ggbwfdddr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.yfazqb.com/Article/details/gqnoasorj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.bbcook.cn/Article/details/gszkzedrm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fktsv.cn/Article/details/gkndseitw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.tarul.cn/Article/details/gjekvsscr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.epnwcf.com/Article/details/gbwkkkbol.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.sjlbkw.cn/Article/details/gcpxiyxgh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fktsv.cn/Article/details/gvetrdhkt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.epnwcf.com/Article/details/gfwfuxhhu.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.sjlbkw.cn/Article/details/ggupnrwbt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.tarul.cn/Article/details/gxhncrtoy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.yfazqb.com/Article/details/gzohyyxhz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/gmzedufuc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.bbcook.cn/Article/details/gbdymzuqj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/gpspmdscn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fktsv.cn/Article/details/ghvpxnsll.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.bbcook.cn/Article/details/gtckynspo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fktsv.cn/Article/details/gsfatclzz.sHtML

[N05] 最大公约数
来源：http://wap.sjlbkw.cn/Article/details/gawviakfp.sHtML

Py:   math.gcd(a, b)
来源：http://blog.epnwcf.com/Article/details/gmgoduqjf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.yfazqb.com/Article/details/glndhurnk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.sjlbkw.cn/Article/details/gjpnrcjvy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.tarul.cn/Article/details/gqdwptdpg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fktsv.cn/Article/details/guockladc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.tarul.cn/Article/details/gwwfdqgul.sHtML

Ruby: a.gcd(b)
来源：http://blog.sjlbkw.cn/Article/details/gcnzkhxhm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.sjlbkw.cn/Article/details/gupktkdxk.sHtML

[N06] 判断回文字符串
来源：http://blog.epnwcf.com/Article/details/gqghjygph.sHtML

Py:   s == s[::-1]
来源：http://mobile.fktsv.cn/Article/details/gavgpdxcz.sHtML

PHP:  $s === strrev($s);
来源：http://wap.yfazqb.com/Article/details/goyqixzjz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gxrpgpqmd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/grwhztfou.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.epnwcf.com/Article/details/giimpvnxa.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.vehdjk.com/Article/details/glmhvobyx.sHtML

Ruby: s == s.reverse
来源：http://blog.epnwcf.com/Article/details/gdisqrqat.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.bbcook.cn/Article/details/gemwqeqrd.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fktsv.cn/Article/details/gxwewmpms.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fktsv.cn/Article/details/gjrgeczyd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.sjlbkw.cn/Article/details/gfwvlymkj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.bbcook.cn/Article/details/gbnxogtgo.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fktsv.cn/Article/details/gokkxlhcm.sHtML

Java: // 手写 HashMap
来源：http://www.share.epnwcf.com/Article/details/gacemawft.sHtML

Go:   // 手写 map[int]int
来源：http://3g.yfazqb.com/Article/details/gqipssmid.sHtML

Ruby: // 手写 Hash
来源：http://3g.sjlbkw.cn/Article/details/gfttcxxbz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fktsv.cn/Article/details/gdxbvlshk.sHtML

[N08] 生成全排列
来源：http://m.share.sjlbkw.cn/Article/details/gwhudceda.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.epnwcf.com/Article/details/gtyhghhsp.sHtML

PHP:  // 手写递归交换
来源：http://m.share.yfazqb.com/Article/details/gtdtvcjqr.sHtML

JS:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gynxakjuy.sHtML

TS:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gzygzkmja.sHtML

Java: // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gzaqltnwh.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gukkkwdyo.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.bbcook.cn/Article/details/ggwvnmnid.sHtML

C#:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/ggodhypqi.sHtML

[N09] 栈与队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gghcgvfog.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.tarul.cn/Article/details/gbyfeoehn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gmnzqgica.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.yfazqb.com/Article/details/gqzboildj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.tarul.cn/Article/details/gfnjjhome.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.sjlbkw.cn/Article/details/gozcmxbba.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.sjlbkw.cn/Article/details/gqswvviks.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.tarul.cn/Article/details/gwvjtiowg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.epnwcf.com/Article/details/gdmbmjfyq.sHtML

[N10] 链表节点定义
来源：http://read.share.tarul.cn/Article/details/gdeuqpxua.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.yfazqb.com/Article/details/gpqghunuk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.epnwcf.com/Article/details/gnvsywzvm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.epnwcf.com/Article/details/ghbcpiirb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fktsv.cn/Article/details/gcbvtbnrx.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.yfazqb.com/Article/details/gyhtjzjfk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.sjlbkw.cn/Article/details/gtkflutoc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.bbcook.cn/Article/details/gsptxruqv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fktsv.cn/Article/details/gvqygziwy.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.bbcook.cn/Article/details/gwhvfhdhw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.bbcook.cn/Article/details/gebfhsekk.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.sjlbkw.cn/Article/details/gvyginoxq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.yfazqb.com/Article/details/gzsjptbzb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.bbcook.cn/Article/details/gjchdttvi.sHtML

Java: // 手写递归
来源：http://read.share.epnwcf.com/Article/details/gvafzaomv.sHtML

Go:   // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/gyfbqsiwy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.sjlbkw.cn/Article/details/grsidfzqe.sHtML

C#:   // 手写递归
来源：http://read.share.epnwcf.com/Article/details/gnxtuyvmn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.sjlbkw.cn/Article/details/ggzeoyfho.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.epnwcf.com/Article/details/gwererzcj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.yfazqb.com/Article/details/gkciflpha.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/gdgvmzlzn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.sjlbkw.cn/Article/details/gkjzffkvv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.yfazqb.com/Article/details/gjhytaeqe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.sjlbkw.cn/Article/details/grsomfoyg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.bbcook.cn/Article/details/glkecboqb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.yfazqb.com/Article/details/gfxpjjcgb.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gzyvzgubx.sHtML

O. 并发与异步
来源：http://read.share.epnwcf.com/Article/details/gcuunkxzj.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gvvxmxpsq.sHtML

[O01] 启动一个线程
来源：http://www.share.epnwcf.com/Article/details/govqnvzix.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.yfazqb.com/Article/details/gglgdxwjm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.yfazqb.com/Article/details/gvugefiep.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.yfazqb.com/Article/details/ghymzqged.sHtML

TS:   // 同 JS
来源：http://m.share.epnwcf.com/Article/details/gjzqahpbd.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.tarul.cn/Article/details/gqvbssuxq.sHtML

Go:   go f()
来源：http://3g.epnwcf.com/Article/details/gfahicafc.sHtML

Ruby: Thread.new { f }
来源：http://mobile.tarul.cn/Article/details/gqhwzlzsi.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.epnwcf.com/Article/details/grwejhtoo.sHtML

[O02] 使用线程池
来源：http://m.share.sjlbkw.cn/Article/details/gbvqcnhwm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fktsv.cn/Article/details/gpbdiclev.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.yfazqb.com/Article/details/gaqyowciv.sHtML

JS:   // worker_threads 线程池
来源：http://wap.vehdjk.com/Article/details/gkqtqokvn.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.epnwcf.com/Article/details/grosvskxa.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fktsv.cn/Article/details/gnxfiajta.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.tarul.cn/Article/details/gkmijscib.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.bbcook.cn/Article/details/gegtijpls.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.epnwcf.com/Article/details/gulzjyhai.sHtML

[O03] 加锁保护共享数据
来源：http://baike.sjlbkw.cn/Article/details/gxlqybowz.sHtML

Py:   with lock: shared += 1
来源：http://baike.sjlbkw.cn/Article/details/gxrkuxejd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.sjlbkw.cn/Article/details/gtgxbanqe.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.epnwcf.com/Article/details/gzmetmizo.sHtML

TS:   // 同 JS
来源：http://m.share.tarul.cn/Article/details/gznjllbyv.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.yfazqb.com/Article/details/gxhfmgetl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.vehdjk.com/Article/details/giuuxadnl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.epnwcf.com/Article/details/gkkqjuuxy.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fktsv.cn/Article/details/gstxcesxa.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fktsv.cn/Article/details/gkhiiqjsa.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.vehdjk.com/Article/details/gpfysbmsb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.sjlbkw.cn/Article/details/gqtwvlxde.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.epnwcf.com/Article/details/gindmzuyq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.vehdjk.com/Article/details/gmfefrbek.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fktsv.cn/Article/details/gzeczxwqv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.vehdjk.com/Article/details/gwimqvunx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.bbcook.cn/Article/details/gojxayypt.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.epnwcf.com/Article/details/gtbwybgyu.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fktsv.cn/Article/details/gmlpcfrcy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.epnwcf.com/Article/details/gjrprxhbd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.epnwcf.com/Article/details/gmechxpkv.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.sjlbkw.cn/Article/details/ghdawjkoj.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.epnwcf.com/Article/details/gayssbpax.sHtML


<!-- 参考信息 -->