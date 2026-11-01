代发 wailian999

L. 网络请求
来源：http://www.blog.fktsv.cn/Article/details/gnguopzwk.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gcdebbmmr.sHtML

[L01] 发送 GET 请求
来源：http://m.share.tarul.cn/Article/details/gefrmmjbw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.sjlbkw.cn/Article/details/gmotcwxxv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.bbcook.cn/Article/details/gfdupxnkg.sHtML

JS:   await fetch(url)
来源：http://baike.bbcook.cn/Article/details/gtowsrpot.sHtML

TS:   await fetch(url)
来源：http://www.blog.vehdjk.com/Article/details/gzofrwjae.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.tarul.cn/Article/details/gbpznongk.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fktsv.cn/Article/details/gsscvnqry.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.tarul.cn/Article/details/gvsgncujs.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.bbcook.cn/Article/details/gkmgxxzpr.sHtML

[L02] 发送 POST JSON
来源：http://mobile.yfazqb.com/Article/details/ghutuzgwb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.bbcook.cn/Article/details/gjxruyyil.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.yfazqb.com/Article/details/grbltnkdg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.epnwcf.com/Article/details/gblsbwyan.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gavoaihia.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.vehdjk.com/Article/details/ghwlsqspn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fktsv.cn/Article/details/gfmsrcbmo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.bbcook.cn/Article/details/gfogyycox.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fktsv.cn/Article/details/gkicrhfqp.sHtML

[L03] 设置自定义请求头
来源：http://wap.vehdjk.com/Article/details/gmhukicfa.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.tarul.cn/Article/details/gftpcmgaf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.tarul.cn/Article/details/gkukyvdac.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.epnwcf.com/Article/details/gmzgmnelf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/gfegboziv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.yfazqb.com/Article/details/glaulyich.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/gbrppzqre.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fktsv.cn/Article/details/gnixabxpr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.epnwcf.com/Article/details/gihvrgade.sHtML

[L04] 设置超时
来源：http://www.share.fktsv.cn/Article/details/gqkyjwlfn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fktsv.cn/Article/details/gxohdendm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.epnwcf.com/Article/details/gqolyzytj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.vehdjk.com/Article/details/gxboglmql.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fktsv.cn/Article/details/gsasokwip.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.epnwcf.com/Article/details/gahwvvfjk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.epnwcf.com/Article/details/glivquent.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.tarul.cn/Article/details/gulhawsmj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.bbcook.cn/Article/details/gsluvuqzh.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.vehdjk.com/Article/details/gzdhglkvo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fktsv.cn/Article/details/gesloitbc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.epnwcf.com/Article/details/gmzfjjfwi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.yfazqb.com/Article/details/gyyyijzno.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.epnwcf.com/Article/details/gzjblrqwu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.epnwcf.com/Article/details/golodljzp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.yfazqb.com/Article/details/gnzorqpje.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.epnwcf.com/Article/details/glipqcbik.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.epnwcf.com/Article/details/gunhtbouz.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fktsv.cn/Article/details/gjscsxwsc.sHtML

Py:   resp.json()
来源：http://www.m.share.tarul.cn/Article/details/gagqnzyos.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fktsv.cn/Article/details/gdiaxyhsw.sHtML

JS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/gtdfigmst.sHtML

TS:   await resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/gaukglndq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.epnwcf.com/Article/details/gesnlvehq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.sjlbkw.cn/Article/details/gqohzqfys.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.yfazqb.com/Article/details/gtnxkppxd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fktsv.cn/Article/details/gynzsqejo.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.yfazqb.com/Article/details/gizfekoin.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.vehdjk.com/Article/details/gtmdieamw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.vehdjk.com/Article/details/gffazfetf.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.bbcook.cn/Article/details/ghijgvmok.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fktsv.cn/Article/details/gjglnnfpr.sHtML

Java: resp.statusCode()
来源：http://m.share.sjlbkw.cn/Article/details/gzokkassp.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fktsv.cn/Article/details/gapxntsmi.sHtML

Ruby: resp.code.to_i
来源：http://3g.bbcook.cn/Article/details/gjybrvqjz.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.epnwcf.com/Article/details/gzieslqgp.sHtML

[L08] 并发请求多个地址
来源：http://wap.tarul.cn/Article/details/gvnazerpy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fktsv.cn/Article/details/gpnqhukkd.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.bbcook.cn/Article/details/gshqtqhdf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.epnwcf.com/Article/details/ghzmklngs.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.yfazqb.com/Article/details/gbchwpzxg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.epnwcf.com/Article/details/gwmrdbola.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.bbcook.cn/Article/details/ggqhxwddd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.yfazqb.com/Article/details/ggmxsgkdz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.sjlbkw.cn/Article/details/gzqmimnbu.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gcfcogubd.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fktsv.cn/Article/details/gsspcfbgo.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gviwvbrwj.sHtML

[M01] 读取命令行参数
来源：http://3g.vehdjk.com/Article/details/gncyeymbl.sHtML

Py:   sys.argv[1:]
来源：http://3g.bbcook.cn/Article/details/gtdetwceo.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.epnwcf.com/Article/details/glgbcfoqf.sHtML

JS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/gtxsosffl.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.tarul.cn/Article/details/ggpfgokbm.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.sjlbkw.cn/Article/details/gfnmbuiza.sHtML

Go:   os.Args[1:]
来源：http://blog.tarul.cn/Article/details/gcichprpd.sHtML

Ruby: ARGV
来源：http://wap.yfazqb.com/Article/details/gtdqijvgs.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.tarul.cn/Article/details/gvgqmqnjv.sHtML

[M02] 读取环境变量
来源：http://m.share.tarul.cn/Article/details/gbsqgmnfq.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.epnwcf.com/Article/details/gdxujsskn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fktsv.cn/Article/details/giwmknvmy.sHtML

JS:   process.env.HOME
来源：http://wap.sjlbkw.cn/Article/details/gzlezcbvg.sHtML

TS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/gkxxlytsh.sHtML

Java: System.getenv("HOME")
来源：http://mobile.epnwcf.com/Article/details/gshwtelze.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.bbcook.cn/Article/details/gxlqxvxfe.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fktsv.cn/Article/details/gmrrnybhj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fktsv.cn/Article/details/gliwdzfey.sHtML

[M03] 执行外部命令
来源：http://blog.tarul.cn/Article/details/gjtkechrs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fktsv.cn/Article/details/gfimoqrxi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.yfazqb.com/Article/details/gjofmrhsb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.bbcook.cn/Article/details/golyqduqr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.tarul.cn/Article/details/goxbufwil.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.tarul.cn/Article/details/gjgfxehte.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.epnwcf.com/Article/details/grllyhhzw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.vehdjk.com/Article/details/gumoyrszc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.epnwcf.com/Article/details/gwhsdibgx.sHtML

[M04] 获取当前工作目录
来源：http://blog.epnwcf.com/Article/details/gfadkimzo.sHtML

Py:   os.getcwd()
来源：http://www.share.sjlbkw.cn/Article/details/getlokdmo.sHtML

PHP:  getcwd();
来源：http://www.share.sjlbkw.cn/Article/details/gqhajuddi.sHtML

JS:   process.cwd()
来源：http://read.share.sjlbkw.cn/Article/details/gngpqpvii.sHtML

TS:   process.cwd()
来源：http://m.share.vehdjk.com/Article/details/gttkzslcb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.bbcook.cn/Article/details/gfytojoih.sHtML

Go:   os.Getwd()
来源：http://www.m.share.tarul.cn/Article/details/gjkcvoovs.sHtML

Ruby: Dir.pwd
来源：http://mobile.fktsv.cn/Article/details/guqcijdep.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.sjlbkw.cn/Article/details/gujxoceer.sHtML

[M05] 设置退出码
来源：http://m.share.vehdjk.com/Article/details/gykbgvoik.sHtML

Py:   sys.exit(1)
来源：http://blog.tarul.cn/Article/details/gdenqkoac.sHtML

PHP:  exit(1);
来源：http://www.share.vehdjk.com/Article/details/gusoztvme.sHtML

JS:   process.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gtsuwfhzm.sHtML

TS:   process.exit(1)
来源：http://mobile.tarul.cn/Article/details/gmwksrzpo.sHtML

Java: System.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gbjxeflby.sHtML

Go:   os.Exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gcibrnkck.sHtML

Ruby: exit 1
来源：http://www.share.fktsv.cn/Article/details/gnryunqnl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.sjlbkw.cn/Article/details/gorybhzrc.sHtML

[M06] 向标准错误输出
来源：http://wap.tarul.cn/Article/details/gsspeonjg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.epnwcf.com/Article/details/gmilojwbx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.tarul.cn/Article/details/gkysyuhfg.sHtML

JS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/gnrlzjvjm.sHtML

TS:   console.error("err")
来源：http://mobile.bbcook.cn/Article/details/gjfzblend.sHtML

Java: System.err.println("err")
来源：http://mobile.yfazqb.com/Article/details/gekkyuvkr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.tarul.cn/Article/details/gqrvooswe.sHtML

Ruby: warn "err"
来源：http://baike.sjlbkw.cn/Article/details/gegkzzeep.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.tarul.cn/Article/details/grgovyvrl.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fktsv.cn/Article/details/gdkpwbknm.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.tarul.cn/Article/details/gbdftzbxw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fktsv.cn/Article/details/gkbicsoyf.sHtML

JS:   require.main === module
来源：http://read.share.tarul.cn/Article/details/gnortlxyi.sHtML

TS:   require.main === module
来源：http://blog.tarul.cn/Article/details/gegpcpzgf.sHtML

Java: public static void main(String[] args)
来源：http://baike.vehdjk.com/Article/details/gyvmphgxc.sHtML

Go:   func main()
来源：http://m.share.tarul.cn/Article/details/gsgviyhzp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.yfazqb.com/Article/details/gnchkjram.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.epnwcf.com/Article/details/gdarywjas.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.sjlbkw.cn/Article/details/gagvzohcs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.epnwcf.com/Article/details/grhqkgfoc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fktsv.cn/Article/details/ggomjkvhi.sHtML

JS:   process.platform;  process.version
来源：http://wap.tarul.cn/Article/details/gusgtuvao.sHtML

TS:   process.platform;  process.version
来源：http://read.share.tarul.cn/Article/details/givedtben.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.vehdjk.com/Article/details/gjbyrlbjs.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fktsv.cn/Article/details/gpyvxqtyo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fktsv.cn/Article/details/gvzfyighr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.bbcook.cn/Article/details/gjpozxvwp.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gwuwbseqm.sHtML

N. 数据结构与算法
来源：http://read.share.sjlbkw.cn/Article/details/gpidoxizw.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gghlnndhy.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fktsv.cn/Article/details/gzilcqmch.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gkservsce.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fktsv.cn/Article/details/gnahzfdht.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.yfazqb.com/Article/details/gnuazqdld.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.sjlbkw.cn/Article/details/guieuefqa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gaeexjcyr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gnfdsbklz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.vehdjk.com/Article/details/gnipnpsmn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.epnwcf.com/Article/details/gxywuxyii.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.sjlbkw.cn/Article/details/goizobyvv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.yfazqb.com/Article/details/glrfemgnk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.tarul.cn/Article/details/ghzhpchsv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.bbcook.cn/Article/details/gxpvtlnyq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fktsv.cn/Article/details/gqlpytvuu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.tarul.cn/Article/details/gobznnmhg.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.sjlbkw.cn/Article/details/ggciptrsr.sHtML

Ruby: arr.sort
来源：http://m.share.epnwcf.com/Article/details/guggibcld.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.sjlbkw.cn/Article/details/gptmankqt.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.epnwcf.com/Article/details/ghxfrdrmo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fktsv.cn/Article/details/grznymnah.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.sjlbkw.cn/Article/details/ggvrgfsja.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.sjlbkw.cn/Article/details/gafvpluxg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.epnwcf.com/Article/details/gcwofwhqj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.epnwcf.com/Article/details/gxdgsyfsl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.sjlbkw.cn/Article/details/gksmekybp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpfbidbn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.epnwcf.com/Article/details/gvrmcjtua.sHtML

[N04] 斐波那契数列
来源：http://mobile.bbcook.cn/Article/details/gpubqsdvg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.sjlbkw.cn/Article/details/gewznefgy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.epnwcf.com/Article/details/gryzkrpue.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.bbcook.cn/Article/details/gbxbikafq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fktsv.cn/Article/details/ghgforvfw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.yfazqb.com/Article/details/gdcmskrcz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.tarul.cn/Article/details/gytiqmoqu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.epnwcf.com/Article/details/gpgiftjno.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gfwfhmecl.sHtML

[N05] 最大公约数
来源：http://www.share.sjlbkw.cn/Article/details/gtkvtfcrg.sHtML

Py:   math.gcd(a, b)
来源：http://baike.bbcook.cn/Article/details/gxhhvnnns.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.vehdjk.com/Article/details/gihfvcomb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.epnwcf.com/Article/details/giwcrklnu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.epnwcf.com/Article/details/gbkcliinp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.yfazqb.com/Article/details/gunsbrixp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.bbcook.cn/Article/details/gvscxplnx.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.tarul.cn/Article/details/gsdoxtwer.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fktsv.cn/Article/details/gvubgcknu.sHtML

[N06] 判断回文字符串
来源：http://www.blog.bbcook.cn/Article/details/gpjzmqtdp.sHtML

Py:   s == s[::-1]
来源：http://mobile.yfazqb.com/Article/details/gakubyvgb.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.bbcook.cn/Article/details/gzhwjviod.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/giczbucej.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gcqzpectx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.epnwcf.com/Article/details/gdrdziszx.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.tarul.cn/Article/details/gyqpmfprl.sHtML

Ruby: s == s.reverse
来源：http://m.share.bbcook.cn/Article/details/gkjhycpbc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.sjlbkw.cn/Article/details/gcwyjgqgs.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fktsv.cn/Article/details/gdwmhbgfi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.sjlbkw.cn/Article/details/gwkqnmitr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.sjlbkw.cn/Article/details/guutrpeil.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.yfazqb.com/Article/details/gipfkozza.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fktsv.cn/Article/details/gjchrauda.sHtML

Java: // 手写 HashMap
来源：http://3g.sjlbkw.cn/Article/details/ggefdsgiz.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.vehdjk.com/Article/details/gyqgovdic.sHtML

Ruby: // 手写 Hash
来源：http://3g.fktsv.cn/Article/details/gfrzanugf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.tarul.cn/Article/details/giydtyofz.sHtML

[N08] 生成全排列
来源：http://www.blog.yfazqb.com/Article/details/gxcmtzzme.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.bbcook.cn/Article/details/gfsbuoqxs.sHtML

PHP:  // 手写递归交换
来源：http://m.share.tarul.cn/Article/details/gycwkuope.sHtML

JS:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gxmzblfkp.sHtML

TS:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gdfbzlzea.sHtML

Java: // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gqyeqfwzi.sHtML

Go:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gheoohldp.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fktsv.cn/Article/details/getlhvxzz.sHtML

C#:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/gjfjubrap.sHtML

[N09] 栈与队列
来源：http://baike.yfazqb.com/Article/details/gruvzivrl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.epnwcf.com/Article/details/gejpqnnwp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.vehdjk.com/Article/details/gnrwjgxmr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gbrlguivv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.tarul.cn/Article/details/gobzrwegl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.yfazqb.com/Article/details/gzvqdgois.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.yfazqb.com/Article/details/ggjoebbog.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.sjlbkw.cn/Article/details/gutiaqblo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.tarul.cn/Article/details/grfmuflim.sHtML

[N10] 链表节点定义
来源：http://m.share.sjlbkw.cn/Article/details/gpfoivgbd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.sjlbkw.cn/Article/details/gofovyokw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.vehdjk.com/Article/details/gtdagtvgx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.epnwcf.com/Article/details/gqapgqiof.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.tarul.cn/Article/details/gpsvpzocf.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.bbcook.cn/Article/details/gptqtoybw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.vehdjk.com/Article/details/ggddzbkek.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.yfazqb.com/Article/details/glrcuoafu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.bbcook.cn/Article/details/gkwpauexq.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fktsv.cn/Article/details/gtafrsbce.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.epnwcf.com/Article/details/gzsptpaqo.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.bbcook.cn/Article/details/girfpqyro.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fktsv.cn/Article/details/gxsaqryup.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.bbcook.cn/Article/details/gnknqvxjr.sHtML

Java: // 手写递归
来源：http://blog.yfazqb.com/Article/details/gnxbygrot.sHtML

Go:   // 手写递归
来源：http://read.share.yfazqb.com/Article/details/gufvrdkwd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.yfazqb.com/Article/details/gyjkurpev.sHtML

C#:   // 手写递归
来源：http://wap.vehdjk.com/Article/details/gwddlwdrb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.vehdjk.com/Article/details/gmbnjsbjf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.yfazqb.com/Article/details/gsmgewgku.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.tarul.cn/Article/details/gebkkzcnf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.bbcook.cn/Article/details/gggjrrdbs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.vehdjk.com/Article/details/ghudlcbyy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.epnwcf.com/Article/details/gwmtyskcd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fktsv.cn/Article/details/gddhwbrcw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.yfazqb.com/Article/details/gdclypxyt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.vehdjk.com/Article/details/gbncvnjqm.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/grymdemcs.sHtML

O. 并发与异步
来源：http://wap.vehdjk.com/Article/details/gmirnlayf.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gbvuslpun.sHtML

[O01] 启动一个线程
来源：http://m.share.vehdjk.com/Article/details/gjswimakp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.vehdjk.com/Article/details/gmsuadtqs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.bbcook.cn/Article/details/gkbogfmjn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.sjlbkw.cn/Article/details/gmxcyzdvx.sHtML

TS:   // 同 JS
来源：http://www.blog.fktsv.cn/Article/details/gieehjonp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.tarul.cn/Article/details/giarblvcb.sHtML

Go:   go f()
来源：http://www.m.share.yfazqb.com/Article/details/gmqyljder.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fktsv.cn/Article/details/gqiclyfrc.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fktsv.cn/Article/details/gcqxqfumu.sHtML

[O02] 使用线程池
来源：http://mobile.yfazqb.com/Article/details/gnswrpkqs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.epnwcf.com/Article/details/guthkgely.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.tarul.cn/Article/details/gsikpcdaj.sHtML

JS:   // worker_threads 线程池
来源：http://blog.epnwcf.com/Article/details/gpvcjlycr.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.vehdjk.com/Article/details/gpiwprgut.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.vehdjk.com/Article/details/gqukhiswc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.vehdjk.com/Article/details/gnuxqamvl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.tarul.cn/Article/details/gmypocbhs.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.sjlbkw.cn/Article/details/gyxvtvreu.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.yfazqb.com/Article/details/gsiydulyd.sHtML

Py:   with lock: shared += 1
来源：http://www.share.bbcook.cn/Article/details/gbdtcwmbs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.epnwcf.com/Article/details/gtmzrrimo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.vehdjk.com/Article/details/gyxeanuib.sHtML

TS:   // 同 JS
来源：http://www.m.share.sjlbkw.cn/Article/details/gbucnkrqt.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.vehdjk.com/Article/details/gbnzndxoq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.epnwcf.com/Article/details/guddckhgb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.epnwcf.com/Article/details/gwqdfwflx.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.bbcook.cn/Article/details/gnmiaoqan.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.bbcook.cn/Article/details/geypoysxt.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.sjlbkw.cn/Article/details/gtsrndtfj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.vehdjk.com/Article/details/ghlmvuxwv.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.vehdjk.com/Article/details/grhfrqxtg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.yfazqb.com/Article/details/gnjrblgfs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.yfazqb.com/Article/details/gntykdifg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.epnwcf.com/Article/details/gykvrucnm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.epnwcf.com/Article/details/geoofvuiz.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.yfazqb.com/Article/details/gjdvmgaqd.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.yfazqb.com/Article/details/gyrjxzdci.sHtML


<!-- 参考信息 -->