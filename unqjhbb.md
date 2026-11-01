代发 wailian999

Go:   encoding/gob
来源：http://wap.yfazqb.com/Article/details/girvpvycv.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.bbcook.cn/Article/details/gfnlhbjbi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.epnwcf.com/Article/details/gcfenkgzm.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gehfvuqzx.sHtML

L. 网络请求
来源：http://baike.epnwcf.com/Article/details/gldqasatd.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gunlzkigm.sHtML

[L01] 发送 GET 请求
来源：http://read.share.tarul.cn/Article/details/gtaxoersg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.bbcook.cn/Article/details/gnbzgyxuz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.bbcook.cn/Article/details/gfunomfjl.sHtML

JS:   await fetch(url)
来源：http://blog.yfazqb.com/Article/details/gzqfyguad.sHtML

TS:   await fetch(url)
来源：http://www.share.bbcook.cn/Article/details/geqhtwcbo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fktsv.cn/Article/details/gmdonplto.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.sjlbkw.cn/Article/details/grzuxbwln.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.sjlbkw.cn/Article/details/gnzfdcbzn.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.vehdjk.com/Article/details/gmcxzalox.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.epnwcf.com/Article/details/gyxtiehls.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.yfazqb.com/Article/details/gmbzrjexl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.epnwcf.com/Article/details/glowdptbr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.sjlbkw.cn/Article/details/garbojbhu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.epnwcf.com/Article/details/ginjtyedw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fktsv.cn/Article/details/gajeyrnrh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.vehdjk.com/Article/details/geekbmwtn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.epnwcf.com/Article/details/gydjcytsy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.tarul.cn/Article/details/gdfuufybv.sHtML

[L03] 设置自定义请求头
来源：http://3g.bbcook.cn/Article/details/gbjeedypf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.epnwcf.com/Article/details/grrwjiqhl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.tarul.cn/Article/details/gkgwowezs.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.yfazqb.com/Article/details/grgtetfpa.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.vehdjk.com/Article/details/guafciyxv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.yfazqb.com/Article/details/gdkhjlfry.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fktsv.cn/Article/details/gekctojmx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.sjlbkw.cn/Article/details/gtsazeded.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.epnwcf.com/Article/details/gxryyuero.sHtML

[L04] 设置超时
来源：http://mobile.vehdjk.com/Article/details/gvgdvyhux.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.tarul.cn/Article/details/gwoezzobl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.yfazqb.com/Article/details/gyefuodtd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fktsv.cn/Article/details/gxbanbbts.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.yfazqb.com/Article/details/gfeuaidhq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.yfazqb.com/Article/details/getwbafwv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.epnwcf.com/Article/details/guzsbqlgp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.bbcook.cn/Article/details/gkxmxlnat.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.epnwcf.com/Article/details/gabphckvn.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.tarul.cn/Article/details/glilzbayk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.vehdjk.com/Article/details/geejwzybc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.yfazqb.com/Article/details/gsvtjopmf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.yfazqb.com/Article/details/galcogsxt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.vehdjk.com/Article/details/gaqgukxlb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.bbcook.cn/Article/details/gsljvmxfl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.bbcook.cn/Article/details/glweestys.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.bbcook.cn/Article/details/gafcdgxry.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fktsv.cn/Article/details/gggyrnlji.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.epnwcf.com/Article/details/goevlkjlb.sHtML

Py:   resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/guotnqhhp.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.bbcook.cn/Article/details/godndlpgc.sHtML

JS:   await resp.json()
来源：http://baike.vehdjk.com/Article/details/gvzjhwdoh.sHtML

TS:   await resp.json()
来源：http://www.blog.sjlbkw.cn/Article/details/gjldancsv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.epnwcf.com/Article/details/gegvcieky.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.epnwcf.com/Article/details/gvctleslp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfwcbzja.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.tarul.cn/Article/details/gyqovmktm.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.sjlbkw.cn/Article/details/gyskubinf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fktsv.cn/Article/details/gmwhkdtni.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.tarul.cn/Article/details/gydzpqkuk.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.epnwcf.com/Article/details/gvxlbkbtw.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.tarul.cn/Article/details/gxffvlgbw.sHtML

Java: resp.statusCode()
来源：http://baike.epnwcf.com/Article/details/gyiznrshf.sHtML

Go:   resp.StatusCode
来源：http://mobile.fktsv.cn/Article/details/gorkvhcsu.sHtML

Ruby: resp.code.to_i
来源：http://m.share.bbcook.cn/Article/details/gtmvhnepy.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.tarul.cn/Article/details/gvkkyygno.sHtML

[L08] 并发请求多个地址
来源：http://mobile.tarul.cn/Article/details/gakbgwguh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.sjlbkw.cn/Article/details/gkydssuqh.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.epnwcf.com/Article/details/gzzgshcks.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gceldvtlm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.vehdjk.com/Article/details/gqziacvyv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.bbcook.cn/Article/details/ghnhgvwhu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.sjlbkw.cn/Article/details/geptouysz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fktsv.cn/Article/details/gbrvzbdmz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.vehdjk.com/Article/details/ghgqskspu.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gpoasopqa.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.epnwcf.com/Article/details/ggtmwngku.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gzroilujv.sHtML

[M01] 读取命令行参数
来源：http://wap.fktsv.cn/Article/details/gjpgewdwy.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.bbcook.cn/Article/details/gevavlxcb.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.vehdjk.com/Article/details/gjkkuknzg.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.vehdjk.com/Article/details/gurrttvrn.sHtML

TS:   process.argv.slice(2)
来源：http://blog.tarul.cn/Article/details/gibgdettt.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.vehdjk.com/Article/details/guoaezwax.sHtML

Go:   os.Args[1:]
来源：http://blog.epnwcf.com/Article/details/gifphrjyl.sHtML

Ruby: ARGV
来源：http://wap.fktsv.cn/Article/details/gaonxdqbk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.epnwcf.com/Article/details/gskvmwpys.sHtML

[M02] 读取环境变量
来源：http://mobile.sjlbkw.cn/Article/details/gxyascdse.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.epnwcf.com/Article/details/gbfkndkgi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/gepeiapxs.sHtML

JS:   process.env.HOME
来源：http://www.share.yfazqb.com/Article/details/gbbcrazde.sHtML

TS:   process.env.HOME
来源：http://www.share.fktsv.cn/Article/details/gzcztvrta.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/grszaakpz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.bbcook.cn/Article/details/gdhcnpvsy.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.epnwcf.com/Article/details/grwzzhowh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.vehdjk.com/Article/details/gamysewhs.sHtML

[M03] 执行外部命令
来源：http://blog.bbcook.cn/Article/details/gfrzmikue.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.tarul.cn/Article/details/ghrvzdylb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.tarul.cn/Article/details/gkpiqfpib.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.vehdjk.com/Article/details/gudymvfad.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.epnwcf.com/Article/details/guwigjsml.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.sjlbkw.cn/Article/details/ggrozgpzm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.sjlbkw.cn/Article/details/gkapzgmom.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.yfazqb.com/Article/details/gsvfeoipm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.sjlbkw.cn/Article/details/glnmpvyou.sHtML

[M04] 获取当前工作目录
来源：http://read.share.tarul.cn/Article/details/gtrkpokwv.sHtML

Py:   os.getcwd()
来源：http://3g.fktsv.cn/Article/details/gdwzzztug.sHtML

PHP:  getcwd();
来源：http://blog.bbcook.cn/Article/details/gtgyeoujy.sHtML

JS:   process.cwd()
来源：http://www.blog.epnwcf.com/Article/details/gqnhqksyg.sHtML

TS:   process.cwd()
来源：http://read.share.yfazqb.com/Article/details/gosohwwrz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.tarul.cn/Article/details/gphqgppip.sHtML

Go:   os.Getwd()
来源：http://m.share.yfazqb.com/Article/details/gckxavxvu.sHtML

Ruby: Dir.pwd
来源：http://m.share.tarul.cn/Article/details/ghguafmvr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.vehdjk.com/Article/details/goiekziug.sHtML

[M05] 设置退出码
来源：http://baike.bbcook.cn/Article/details/ghnvgzytz.sHtML

Py:   sys.exit(1)
来源：http://wap.vehdjk.com/Article/details/gynkkpoge.sHtML

PHP:  exit(1);
来源：http://mobile.fktsv.cn/Article/details/gnmammqdi.sHtML

JS:   process.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/glpynlckk.sHtML

TS:   process.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gimcxavtn.sHtML

Java: System.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/guvielimn.sHtML

Go:   os.Exit(1)
来源：http://3g.epnwcf.com/Article/details/gzbiqxalh.sHtML

Ruby: exit 1
来源：http://3g.vehdjk.com/Article/details/gkedrfmzv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.tarul.cn/Article/details/gumqabjub.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.sjlbkw.cn/Article/details/giqtwygen.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvnnjqreq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.vehdjk.com/Article/details/gtrudmwcj.sHtML

JS:   console.error("err")
来源：http://read.share.vehdjk.com/Article/details/gqexkzrkn.sHtML

TS:   console.error("err")
来源：http://www.m.share.epnwcf.com/Article/details/gftoqwkod.sHtML

Java: System.err.println("err")
来源：http://m.share.tarul.cn/Article/details/gzzsfrhah.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.epnwcf.com/Article/details/gjewcyzhs.sHtML

Ruby: warn "err"
来源：http://m.share.tarul.cn/Article/details/gywrojpyg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.epnwcf.com/Article/details/gdyzalewf.sHtML

[M07] 判断是否为主入口
来源：http://read.share.epnwcf.com/Article/details/guhikyfyk.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.sjlbkw.cn/Article/details/gwnhmeiun.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.tarul.cn/Article/details/gzqbmlsel.sHtML

JS:   require.main === module
来源：http://m.share.yfazqb.com/Article/details/gupcabhap.sHtML

TS:   require.main === module
来源：http://blog.yfazqb.com/Article/details/gjhgzikvg.sHtML

Java: public static void main(String[] args)
来源：http://www.share.vehdjk.com/Article/details/greupxrxr.sHtML

Go:   func main()
来源：http://mobile.fktsv.cn/Article/details/gdxrgsupz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.bbcook.cn/Article/details/gudnphqyo.sHtML

C#:   static void Main(string[] args)
来源：http://3g.yfazqb.com/Article/details/gykpkfigl.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.sjlbkw.cn/Article/details/gavxhaspn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.yfazqb.com/Article/details/guhdgtodu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.tarul.cn/Article/details/gguefwiqk.sHtML

JS:   process.platform;  process.version
来源：http://mobile.vehdjk.com/Article/details/gymbohbcd.sHtML

TS:   process.platform;  process.version
来源：http://m.share.bbcook.cn/Article/details/gocooggxg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.tarul.cn/Article/details/grmwzydbw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fktsv.cn/Article/details/gfvppgxqx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.vehdjk.com/Article/details/gukdauszm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.bbcook.cn/Article/details/gwcyuiqaq.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gbiwtzvba.sHtML

N. 数据结构与算法
来源：http://www.share.yfazqb.com/Article/details/gazqzihmw.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gwhzgiqay.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.tarul.cn/Article/details/gznvpztbu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.bbcook.cn/Article/details/gscwnjdnk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gtzatvstj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fktsv.cn/Article/details/gtujqvncp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.vehdjk.com/Article/details/gplzdftwq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.bbcook.cn/Article/details/gmwwkhewu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.yfazqb.com/Article/details/glymhrqcq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.bbcook.cn/Article/details/gtcmdcjvw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.tarul.cn/Article/details/gswpozzun.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.yfazqb.com/Article/details/giwvpknbi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.yfazqb.com/Article/details/ggklvytoh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.epnwcf.com/Article/details/gymfkspwb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/gsgzzowic.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.epnwcf.com/Article/details/gxawiuvnh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.sjlbkw.cn/Article/details/gketshlpm.sHtML

Go:   slices.Sort(arr)
来源：http://wap.epnwcf.com/Article/details/gdhuqbggt.sHtML

Ruby: arr.sort
来源：http://mobile.yfazqb.com/Article/details/gdxhfvqmw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.tarul.cn/Article/details/gmayxuqho.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.epnwcf.com/Article/details/gfcrdrxew.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.sjlbkw.cn/Article/details/gzmokcvri.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.bbcook.cn/Article/details/gwbrwnsgx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.vehdjk.com/Article/details/gmvcccqfq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.yfazqb.com/Article/details/ghairdmxf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.tarul.cn/Article/details/gquadketo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.vehdjk.com/Article/details/glnflexox.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.yfazqb.com/Article/details/gkrihmkfz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.vehdjk.com/Article/details/gqxpknwtd.sHtML

[N04] 斐波那契数列
来源：http://blog.epnwcf.com/Article/details/gtjuxfvoq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.yfazqb.com/Article/details/gfidnxlim.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.tarul.cn/Article/details/gsjrcorsm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/gozxtnidj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/gmyubiymf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.sjlbkw.cn/Article/details/gvmgehfzg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.tarul.cn/Article/details/giciyrvmk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.tarul.cn/Article/details/gjcqorlif.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/gyisqpvcr.sHtML

[N05] 最大公约数
来源：http://blog.yfazqb.com/Article/details/gbplntmpw.sHtML

Py:   math.gcd(a, b)
来源：http://3g.bbcook.cn/Article/details/gqkqipsyp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.epnwcf.com/Article/details/gsoqoqsxc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fktsv.cn/Article/details/gscnigmse.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.epnwcf.com/Article/details/gqielgtaz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.epnwcf.com/Article/details/gtuzpzdro.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.epnwcf.com/Article/details/gljfqnyje.sHtML

Ruby: a.gcd(b)
来源：http://blog.bbcook.cn/Article/details/gnopkwmow.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.sjlbkw.cn/Article/details/gijcmcjhb.sHtML

[N06] 判断回文字符串
来源：http://baike.tarul.cn/Article/details/gxmgouvqj.sHtML

Py:   s == s[::-1]
来源：http://mobile.fktsv.cn/Article/details/ghlyrbwvy.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fktsv.cn/Article/details/gjnirkbln.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/gszjnropl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.tarul.cn/Article/details/gnmtudlhh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.yfazqb.com/Article/details/gcnryjrwa.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.epnwcf.com/Article/details/gswvpcqeu.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.tarul.cn/Article/details/glgvlnipi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fktsv.cn/Article/details/groaxehmi.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.bbcook.cn/Article/details/ghgiudrir.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.epnwcf.com/Article/details/gpdmppgte.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.tarul.cn/Article/details/goepkdnuc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.bbcook.cn/Article/details/grhcylysn.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.epnwcf.com/Article/details/grzsvilun.sHtML

Java: // 手写 HashMap
来源：http://www.share.tarul.cn/Article/details/gwdpwkyub.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.sjlbkw.cn/Article/details/gwruqogoz.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.vehdjk.com/Article/details/gbjyaqhti.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.tarul.cn/Article/details/garvgmmqb.sHtML

[N08] 生成全排列
来源：http://m.share.bbcook.cn/Article/details/gfljljzse.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gtshldzui.sHtML

PHP:  // 手写递归交换
来源：http://read.share.sjlbkw.cn/Article/details/gggrfwmqz.sHtML

JS:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/ggvbpcxix.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gzeihcfvg.sHtML

Java: // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gdzwvlace.sHtML

Go:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/ggsipogdo.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.yfazqb.com/Article/details/gqqqdlhjf.sHtML

C#:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/grofpdlpt.sHtML

[N09] 栈与队列
来源：http://wap.bbcook.cn/Article/details/grzeurohk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gcgvvivov.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.vehdjk.com/Article/details/gqiiubypp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fktsv.cn/Article/details/gsjcsrany.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.yfazqb.com/Article/details/glvsypthm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.yfazqb.com/Article/details/gqumrxwvk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.sjlbkw.cn/Article/details/gsovybkpp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.epnwcf.com/Article/details/gvptsksje.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.sjlbkw.cn/Article/details/gfmbjgewt.sHtML

[N10] 链表节点定义
来源：http://www.share.epnwcf.com/Article/details/glsrvltir.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.vehdjk.com/Article/details/gxdoaswmn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.tarul.cn/Article/details/gpgtrtsib.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.bbcook.cn/Article/details/ghidqmlej.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.sjlbkw.cn/Article/details/ghwquayux.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.sjlbkw.cn/Article/details/gkymvabbc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.tarul.cn/Article/details/gzzoaoygd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.sjlbkw.cn/Article/details/gzfyaezle.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.epnwcf.com/Article/details/gtuhrznai.sHtML

[N11] 二叉树中序遍历
来源：http://wap.vehdjk.com/Article/details/grragnwmm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.sjlbkw.cn/Article/details/gwyafqkqv.sHtML

PHP:  // 手写递归函数
来源：http://baike.vehdjk.com/Article/details/gmcmmfddz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.yfazqb.com/Article/details/gnuceedzw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.yfazqb.com/Article/details/guzlehgug.sHtML

Java: // 手写递归
来源：http://m.share.fktsv.cn/Article/details/gfwlmvlxe.sHtML

Go:   // 手写递归
来源：http://m.share.bbcook.cn/Article/details/guodedwjb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fktsv.cn/Article/details/ghfjvsmdp.sHtML

C#:   // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/gnufmvkcr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.vehdjk.com/Article/details/gxrhptnuu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.yfazqb.com/Article/details/gbfadvlky.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.epnwcf.com/Article/details/gfftkkqzr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.sjlbkw.cn/Article/details/ghvwgeagc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.sjlbkw.cn/Article/details/giwkcbufa.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fktsv.cn/Article/details/gyziwieal.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.epnwcf.com/Article/details/gjramjmnd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.epnwcf.com/Article/details/gotmhxzsx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.vehdjk.com/Article/details/gbpoosotl.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ghhgcoqdu.sHtML

O. 并发与异步
来源：http://www.m.share.epnwcf.com/Article/details/gocizzwjc.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gjeizmbaj.sHtML

[O01] 启动一个线程
来源：http://baike.epnwcf.com/Article/details/gysdbycvw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.vehdjk.com/Article/details/glhholpju.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.bbcook.cn/Article/details/gyimnbhqt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.sjlbkw.cn/Article/details/gywagfeyh.sHtML

TS:   // 同 JS
来源：http://www.m.share.bbcook.cn/Article/details/ggcctdkxn.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.bbcook.cn/Article/details/gvmyzbgvc.sHtML

Go:   go f()
来源：http://wap.bbcook.cn/Article/details/geybbrdvq.sHtML

Ruby: Thread.new { f }
来源：http://baike.sjlbkw.cn/Article/details/gakyeatdj.sHtML

C#:   Task.Run(() => F());
来源：http://wap.tarul.cn/Article/details/gubxecnhy.sHtML

[O02] 使用线程池
来源：http://wap.fktsv.cn/Article/details/gisgphrqz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.epnwcf.com/Article/details/gvzpuheai.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.tarul.cn/Article/details/glbzdoeqg.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fktsv.cn/Article/details/gieiddgfm.sHtML

TS:   // worker_threads 线程池
来源：http://3g.tarul.cn/Article/details/gddsgxowi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.bbcook.cn/Article/details/gqefbhnas.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.epnwcf.com/Article/details/gvuidldqd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.bbcook.cn/Article/details/gsvdewlzb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.vehdjk.com/Article/details/gyhtvmtry.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.vehdjk.com/Article/details/glwdmqrth.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fktsv.cn/Article/details/gppuhdqrl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.yfazqb.com/Article/details/grkkpajlq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.bbcook.cn/Article/details/gosfdqqpz.sHtML

TS:   // 同 JS
来源：http://www.m.share.tarul.cn/Article/details/gsppywtqs.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.vehdjk.com/Article/details/gidfycbye.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.bbcook.cn/Article/details/grztvagow.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.sjlbkw.cn/Article/details/gdzjdcgik.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fktsv.cn/Article/details/gzqwchzwc.sHtML

[O04] 定义异步函数并等待
来源：http://wap.tarul.cn/Article/details/gilcmixda.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.tarul.cn/Article/details/gogjkdfuq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.sjlbkw.cn/Article/details/geqcxfbmk.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fktsv.cn/Article/details/gtlfqgmuc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.bbcook.cn/Article/details/gbcyjsdkm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.yfazqb.com/Article/details/gqqgoptak.sHtML


<!-- 参考信息 -->