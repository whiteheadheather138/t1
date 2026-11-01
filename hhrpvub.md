代发 wailian999

Go:   encoding/gob
来源：http://m.share.tarul.cn/Article/details/gsjdhexno.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fktsv.cn/Article/details/glaoflrud.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.epnwcf.com/Article/details/ghzouxgxp.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gtqmuahpa.sHtML

L. 网络请求
来源：http://m.share.vehdjk.com/Article/details/gauydlpuf.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gkklyqikk.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fktsv.cn/Article/details/gljqzidng.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.yfazqb.com/Article/details/gyxbhklkz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.vehdjk.com/Article/details/gexqkhbab.sHtML

JS:   await fetch(url)
来源：http://3g.fktsv.cn/Article/details/gapqchzbu.sHtML

TS:   await fetch(url)
来源：http://mobile.vehdjk.com/Article/details/grnjrbebq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.vehdjk.com/Article/details/gxlrubzfq.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.sjlbkw.cn/Article/details/gvaydvdcv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.yfazqb.com/Article/details/gbkgvdovr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.epnwcf.com/Article/details/gujnmitcd.sHtML

[L02] 发送 POST JSON
来源：http://read.share.yfazqb.com/Article/details/ghkrbyloj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.tarul.cn/Article/details/govseofwv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.epnwcf.com/Article/details/gqdjkaupr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.vehdjk.com/Article/details/gfjgsvgmf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fktsv.cn/Article/details/gxnxrntxx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fktsv.cn/Article/details/gnblywpat.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.tarul.cn/Article/details/glnmitpog.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.yfazqb.com/Article/details/gidttyvun.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.yfazqb.com/Article/details/gatczujot.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.epnwcf.com/Article/details/gmrimluwn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.sjlbkw.cn/Article/details/gnoksmycq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.vehdjk.com/Article/details/gwnctaagj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.tarul.cn/Article/details/gjcnclfii.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.yfazqb.com/Article/details/ghbgwcndx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.sjlbkw.cn/Article/details/gjkzenzuk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.yfazqb.com/Article/details/gdxrcsvpa.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fktsv.cn/Article/details/gqtndmdol.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.vehdjk.com/Article/details/gwzcyxmde.sHtML

[L04] 设置超时
来源：http://baike.yfazqb.com/Article/details/ghtwxzhia.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.tarul.cn/Article/details/gfbczdrzd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.tarul.cn/Article/details/gtcfuopzh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.sjlbkw.cn/Article/details/gbwlfdlwq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.yfazqb.com/Article/details/gfmctffcg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fktsv.cn/Article/details/gocgrodvh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fktsv.cn/Article/details/gqeazmuwm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.epnwcf.com/Article/details/gwzfemypi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.yfazqb.com/Article/details/gcuoveywb.sHtML

[L05] 上传文件（multipart）
来源：http://3g.sjlbkw.cn/Article/details/gouxlrvwx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.vehdjk.com/Article/details/ggdzlutcu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.bbcook.cn/Article/details/gqzudbopy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fktsv.cn/Article/details/gcguvzbau.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.vehdjk.com/Article/details/glndzjmch.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.epnwcf.com/Article/details/gjwxdvnsn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.sjlbkw.cn/Article/details/getjzkyyf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.bbcook.cn/Article/details/gjyodamfu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/godoucvdt.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.vehdjk.com/Article/details/ghmoogmix.sHtML

Py:   resp.json()
来源：http://www.m.share.fktsv.cn/Article/details/gwzdbmbyr.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.tarul.cn/Article/details/gyeygygev.sHtML

JS:   await resp.json()
来源：http://www.m.share.yfazqb.com/Article/details/gtsfotniw.sHtML

TS:   await resp.json()
来源：http://read.share.yfazqb.com/Article/details/gzfuhlbyr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.epnwcf.com/Article/details/gvboavpht.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.epnwcf.com/Article/details/gxeqjyrwg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.vehdjk.com/Article/details/gjqhhkxol.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.epnwcf.com/Article/details/gjoxurpog.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.bbcook.cn/Article/details/gwzekfogx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.sjlbkw.cn/Article/details/gdyjxvolv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.sjlbkw.cn/Article/details/grpmivowh.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.yfazqb.com/Article/details/gguaancnv.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.vehdjk.com/Article/details/gcojvlcqz.sHtML

Java: resp.statusCode()
来源：http://m.share.bbcook.cn/Article/details/gmjikbzkm.sHtML

Go:   resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/gumgnbers.sHtML

Ruby: resp.code.to_i
来源：http://read.share.bbcook.cn/Article/details/gcmcblckd.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.yfazqb.com/Article/details/gzktwcewe.sHtML

[L08] 并发请求多个地址
来源：http://mobile.tarul.cn/Article/details/gjyjkkanw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.yfazqb.com/Article/details/gnsyastpp.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.yfazqb.com/Article/details/gvgjctsos.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.sjlbkw.cn/Article/details/gpvqsayba.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.bbcook.cn/Article/details/geyquykym.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.epnwcf.com/Article/details/gefecfmgc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.bbcook.cn/Article/details/gsivwkndc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.epnwcf.com/Article/details/gokucmtzv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fktsv.cn/Article/details/gkwzkhhna.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gfkyaffht.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.epnwcf.com/Article/details/gggafryvb.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gaodapvje.sHtML

[M01] 读取命令行参数
来源：http://read.share.tarul.cn/Article/details/gvyvlsjad.sHtML

Py:   sys.argv[1:]
来源：http://www.share.bbcook.cn/Article/details/gfbiwqmbi.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.sjlbkw.cn/Article/details/gxtegedco.sHtML

JS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/gygripxhe.sHtML

TS:   process.argv.slice(2)
来源：http://baike.tarul.cn/Article/details/ggxhljjht.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.vehdjk.com/Article/details/gfvotueve.sHtML

Go:   os.Args[1:]
来源：http://baike.sjlbkw.cn/Article/details/ggvwuzomx.sHtML

Ruby: ARGV
来源：http://mobile.bbcook.cn/Article/details/gxikczexk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.bbcook.cn/Article/details/ggkrrphve.sHtML

[M02] 读取环境变量
来源：http://www.blog.sjlbkw.cn/Article/details/gppvflsxf.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.yfazqb.com/Article/details/gpqqogeev.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.epnwcf.com/Article/details/gkgfsgmnl.sHtML

JS:   process.env.HOME
来源：http://baike.fktsv.cn/Article/details/gcknymyhk.sHtML

TS:   process.env.HOME
来源：http://read.share.fktsv.cn/Article/details/gnkyyatbn.sHtML

Java: System.getenv("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gbctbvljc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gpxtjzexf.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.tarul.cn/Article/details/gearzrwxh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.epnwcf.com/Article/details/gaorapkob.sHtML

[M03] 执行外部命令
来源：http://www.blog.epnwcf.com/Article/details/gciqxainn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fktsv.cn/Article/details/gfhxqspnn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.yfazqb.com/Article/details/gsxniskmo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.vehdjk.com/Article/details/gqexpubut.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fktsv.cn/Article/details/gpfbwiizn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fktsv.cn/Article/details/gzraxnivu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.sjlbkw.cn/Article/details/gawryqsjy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fktsv.cn/Article/details/glvdnarys.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fktsv.cn/Article/details/gkrjzzvfh.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.vehdjk.com/Article/details/gskpmovvr.sHtML

Py:   os.getcwd()
来源：http://blog.vehdjk.com/Article/details/gfamrbtcc.sHtML

PHP:  getcwd();
来源：http://mobile.tarul.cn/Article/details/ghpqxmcoy.sHtML

JS:   process.cwd()
来源：http://m.share.tarul.cn/Article/details/gdubhqprp.sHtML

TS:   process.cwd()
来源：http://m.share.yfazqb.com/Article/details/gvooardut.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.vehdjk.com/Article/details/ggvxjeinn.sHtML

Go:   os.Getwd()
来源：http://wap.yfazqb.com/Article/details/gszoepmka.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fktsv.cn/Article/details/gqywudohv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.sjlbkw.cn/Article/details/gmxzjucxg.sHtML

[M05] 设置退出码
来源：http://read.share.tarul.cn/Article/details/guzoqsayp.sHtML

Py:   sys.exit(1)
来源：http://m.share.yfazqb.com/Article/details/geewpowis.sHtML

PHP:  exit(1);
来源：http://www.blog.sjlbkw.cn/Article/details/gicbzmopx.sHtML

JS:   process.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gclshufgs.sHtML

TS:   process.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/guwutqqsa.sHtML

Java: System.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gojazymze.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/grsnrhwgl.sHtML

Ruby: exit 1
来源：http://blog.yfazqb.com/Article/details/ggajnptuk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.bbcook.cn/Article/details/gtlfwbaqd.sHtML

[M06] 向标准错误输出
来源：http://3g.fktsv.cn/Article/details/gntfxumyv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fktsv.cn/Article/details/gjgpcdpzf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.vehdjk.com/Article/details/gyupxztqq.sHtML

JS:   console.error("err")
来源：http://3g.bbcook.cn/Article/details/gzgctmrtg.sHtML

TS:   console.error("err")
来源：http://www.blog.epnwcf.com/Article/details/gwdjhrmfj.sHtML

Java: System.err.println("err")
来源：http://mobile.fktsv.cn/Article/details/gajgemngd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fktsv.cn/Article/details/glmlovhil.sHtML

Ruby: warn "err"
来源：http://blog.yfazqb.com/Article/details/ggofpwfzt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.yfazqb.com/Article/details/gaqqdhosg.sHtML

[M07] 判断是否为主入口
来源：http://read.share.bbcook.cn/Article/details/gfgrdulea.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.sjlbkw.cn/Article/details/guhuvphpu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.epnwcf.com/Article/details/gvlkzqifx.sHtML

JS:   require.main === module
来源：http://www.m.share.tarul.cn/Article/details/gztswyrtc.sHtML

TS:   require.main === module
来源：http://read.share.tarul.cn/Article/details/gomxkufbf.sHtML

Java: public static void main(String[] args)
来源：http://wap.fktsv.cn/Article/details/gypdbqinq.sHtML

Go:   func main()
来源：http://read.share.fktsv.cn/Article/details/gfirjnxdx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.yfazqb.com/Article/details/gnoebxcwo.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.yfazqb.com/Article/details/gdacuvxhr.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fktsv.cn/Article/details/gyhjtnfpe.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.sjlbkw.cn/Article/details/gjqmybctk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.vehdjk.com/Article/details/givzprkdh.sHtML

JS:   process.platform;  process.version
来源：http://blog.vehdjk.com/Article/details/glaugvobv.sHtML

TS:   process.platform;  process.version
来源：http://baike.vehdjk.com/Article/details/grhpbfmod.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.vehdjk.com/Article/details/gfemvtpxa.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fktsv.cn/Article/details/ghahtlueh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.epnwcf.com/Article/details/gimlqfsbv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.yfazqb.com/Article/details/gqerzortq.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ghgbcfulv.sHtML

N. 数据结构与算法
来源：http://baike.yfazqb.com/Article/details/gwbunkuuw.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gphpscrjy.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fktsv.cn/Article/details/gtrapxnkc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.epnwcf.com/Article/details/ghutrscuz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.epnwcf.com/Article/details/ggoasnmvs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.bbcook.cn/Article/details/gwrglxdlg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.tarul.cn/Article/details/gnysenuve.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.tarul.cn/Article/details/gsixiabuj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gmemvvheo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.epnwcf.com/Article/details/gakjqbbut.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.epnwcf.com/Article/details/ghgrufqaw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.vehdjk.com/Article/details/gqiogwkvh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.sjlbkw.cn/Article/details/gomodabbo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.bbcook.cn/Article/details/gdxiqkbyz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.tarul.cn/Article/details/gykrgujhj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/gnagunydg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fktsv.cn/Article/details/ghwqegzxd.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.vehdjk.com/Article/details/gqoswjxal.sHtML

Ruby: arr.sort
来源：http://www.share.tarul.cn/Article/details/gcpjvzvlz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.tarul.cn/Article/details/gpexhjniy.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.tarul.cn/Article/details/gwcvijaqe.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fktsv.cn/Article/details/gmqnzuepo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.tarul.cn/Article/details/gtrtyfeof.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.epnwcf.com/Article/details/glicdcxui.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.yfazqb.com/Article/details/gvgpyzrpw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.epnwcf.com/Article/details/gcufklnma.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.bbcook.cn/Article/details/guepsmkro.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.tarul.cn/Article/details/glcgqvnfb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.yfazqb.com/Article/details/gbhbocitn.sHtML

[N04] 斐波那契数列
来源：http://mobile.epnwcf.com/Article/details/gdosqitbd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.bbcook.cn/Article/details/gvwqmvwcz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.tarul.cn/Article/details/gvwpbymgy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.bbcook.cn/Article/details/guafttpex.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/gqejinnti.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.bbcook.cn/Article/details/ghjztwylw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.sjlbkw.cn/Article/details/gnqfkrmwc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.sjlbkw.cn/Article/details/gcgsmnash.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.tarul.cn/Article/details/garmkrrfx.sHtML

[N05] 最大公约数
来源：http://mobile.bbcook.cn/Article/details/gkdbqmxyo.sHtML

Py:   math.gcd(a, b)
来源：http://blog.epnwcf.com/Article/details/gyzjjwvhx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.yfazqb.com/Article/details/gkntmmzbb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.yfazqb.com/Article/details/gplpwlbon.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.sjlbkw.cn/Article/details/gvajwcfyc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fktsv.cn/Article/details/gubzfthyz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.yfazqb.com/Article/details/gpzwrfmpc.sHtML

Ruby: a.gcd(b)
来源：http://3g.sjlbkw.cn/Article/details/guejomqmz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.bbcook.cn/Article/details/gbaftzszm.sHtML

[N06] 判断回文字符串
来源：http://read.share.bbcook.cn/Article/details/gtrucssah.sHtML

Py:   s == s[::-1]
来源：http://mobile.bbcook.cn/Article/details/ghbpfuihx.sHtML

PHP:  $s === strrev($s);
来源：http://baike.bbcook.cn/Article/details/gmhrvgtut.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gqkhpartj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/guuavrocj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fktsv.cn/Article/details/gfphewrrj.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.sjlbkw.cn/Article/details/gtilthexh.sHtML

Ruby: s == s.reverse
来源：http://blog.fktsv.cn/Article/details/gvlpezrwt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.tarul.cn/Article/details/goybxzuuz.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.bbcook.cn/Article/details/gkygadtkw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.tarul.cn/Article/details/gpubzuuly.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.yfazqb.com/Article/details/goeypmozi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.epnwcf.com/Article/details/geyyvkwsb.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.tarul.cn/Article/details/gngzvlbqr.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.tarul.cn/Article/details/gxhuqgcio.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.tarul.cn/Article/details/gzvzmpihl.sHtML

Ruby: // 手写 Hash
来源：http://read.share.vehdjk.com/Article/details/geznxzthq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.sjlbkw.cn/Article/details/grrljvqcf.sHtML

[N08] 生成全排列
来源：http://3g.yfazqb.com/Article/details/gnmlmfykh.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.bbcook.cn/Article/details/gpxuoqpdt.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fktsv.cn/Article/details/goijtuace.sHtML

JS:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gkunureah.sHtML

TS:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gstvchtpo.sHtML

Java: // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gtioxijqh.sHtML

Go:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gggbdoivr.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.bbcook.cn/Article/details/gkbieeqje.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gchflhuzk.sHtML

[N09] 栈与队列
来源：http://www.share.bbcook.cn/Article/details/gkzuxgirv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.tarul.cn/Article/details/gweejadfs.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.tarul.cn/Article/details/guljitogy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.bbcook.cn/Article/details/giscdqlyw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.sjlbkw.cn/Article/details/gdnxablha.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.yfazqb.com/Article/details/gfjeyiwup.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.sjlbkw.cn/Article/details/grdvotviz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.yfazqb.com/Article/details/gekopejby.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fktsv.cn/Article/details/gvsmkusvy.sHtML

[N10] 链表节点定义
来源：http://www.share.tarul.cn/Article/details/gdtmdthap.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.tarul.cn/Article/details/gslejzfml.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.tarul.cn/Article/details/gvdfsixya.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.vehdjk.com/Article/details/giwpwmcmv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.sjlbkw.cn/Article/details/gzqponwsu.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.bbcook.cn/Article/details/gxlnkiyyw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.tarul.cn/Article/details/goqogqwmc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fktsv.cn/Article/details/gdbcenhcp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.bbcook.cn/Article/details/glcdxvgqz.sHtML

[N11] 二叉树中序遍历
来源：http://wap.tarul.cn/Article/details/grramybca.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fktsv.cn/Article/details/gimakazvw.sHtML

PHP:  // 手写递归函数
来源：http://mobile.bbcook.cn/Article/details/ghhzsqvnz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.bbcook.cn/Article/details/gvixegzci.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.vehdjk.com/Article/details/gljdzxkpc.sHtML

Java: // 手写递归
来源：http://blog.vehdjk.com/Article/details/gyokzgzxu.sHtML

Go:   // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/gwgjqgxmi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.vehdjk.com/Article/details/gdlaqivey.sHtML

C#:   // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gjbbevuce.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.yfazqb.com/Article/details/gbocwdxoi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fktsv.cn/Article/details/gcuevhsed.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.vehdjk.com/Article/details/gvdbkdhga.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.sjlbkw.cn/Article/details/gkfuwlpij.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.yfazqb.com/Article/details/gozxxqnuo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fktsv.cn/Article/details/gawfpmtvi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.epnwcf.com/Article/details/gfysizbqq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.sjlbkw.cn/Article/details/geuxopixv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.vehdjk.com/Article/details/gqcqaasce.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gmyoijpmg.sHtML

O. 并发与异步
来源：http://read.share.yfazqb.com/Article/details/gzimflxzi.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gtjtbjhtj.sHtML

[O01] 启动一个线程
来源：http://baike.tarul.cn/Article/details/grkyzmedj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.vehdjk.com/Article/details/giujppexr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.yfazqb.com/Article/details/gmbofoigr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.yfazqb.com/Article/details/gynnnbkoe.sHtML

TS:   // 同 JS
来源：http://wap.bbcook.cn/Article/details/gllooqzfa.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fktsv.cn/Article/details/gqgdjyxxv.sHtML

Go:   go f()
来源：http://3g.bbcook.cn/Article/details/ggbavnqxj.sHtML

Ruby: Thread.new { f }
来源：http://mobile.epnwcf.com/Article/details/giaryqpma.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.sjlbkw.cn/Article/details/gwaqhgujh.sHtML

[O02] 使用线程池
来源：http://mobile.yfazqb.com/Article/details/gitehqadb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.epnwcf.com/Article/details/gngbrsyvu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.sjlbkw.cn/Article/details/ghmtfxhqm.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.yfazqb.com/Article/details/gdhvglxiy.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.yfazqb.com/Article/details/gohhggnop.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.yfazqb.com/Article/details/gsqzoisgu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.bbcook.cn/Article/details/gpgknetec.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.epnwcf.com/Article/details/goidkqpub.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.vehdjk.com/Article/details/gdnbmkrsl.sHtML

[O03] 加锁保护共享数据
来源：http://baike.bbcook.cn/Article/details/goozgavgj.sHtML

Py:   with lock: shared += 1
来源：http://wap.fktsv.cn/Article/details/gcsipnufu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.yfazqb.com/Article/details/gjyrmcyde.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fktsv.cn/Article/details/gstrmfuda.sHtML

TS:   // 同 JS
来源：http://www.m.share.tarul.cn/Article/details/gtqjtfids.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.yfazqb.com/Article/details/gpewmdimr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.epnwcf.com/Article/details/gzarikcdn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.epnwcf.com/Article/details/gsyyoaxne.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.epnwcf.com/Article/details/gexuxvage.sHtML

[O04] 定义异步函数并等待
来源：http://wap.epnwcf.com/Article/details/giqexltcy.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fktsv.cn/Article/details/goqtloens.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.sjlbkw.cn/Article/details/ghzcihbqr.sHtML

JS:   async function f() { await g(); }
来源：http://3g.vehdjk.com/Article/details/gpusicwdf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fktsv.cn/Article/details/gomrioifd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.tarul.cn/Article/details/gnhxbleji.sHtML


<!-- 参考信息 -->