代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.vehdjk.com/Article/details/gltzmohzc.sHtML

JS:   await fetch(url)
来源：http://www.share.epnwcf.com/Article/details/gudgznwrp.sHtML

TS:   await fetch(url)
来源：http://www.m.share.tarul.cn/Article/details/gtrytuihf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.epnwcf.com/Article/details/gjopwzrxm.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.yfazqb.com/Article/details/gatndsfqm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.tarul.cn/Article/details/gqsdeapza.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.tarul.cn/Article/details/gzoyykdom.sHtML

[L02] 发送 POST JSON
来源：http://mobile.epnwcf.com/Article/details/gsvhibych.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.yfazqb.com/Article/details/gadouzdvg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.epnwcf.com/Article/details/gavqdfrzx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.tarul.cn/Article/details/gdnfgphgu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fktsv.cn/Article/details/gqcuhtrmx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.epnwcf.com/Article/details/gzkzxrhbp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.epnwcf.com/Article/details/gwyywpopa.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.sjlbkw.cn/Article/details/gaunercgn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.vehdjk.com/Article/details/gvuwqacax.sHtML

[L03] 设置自定义请求头
来源：http://www.share.yfazqb.com/Article/details/groxntpzx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.epnwcf.com/Article/details/gzeciaawp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.vehdjk.com/Article/details/ghbxdhiox.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.tarul.cn/Article/details/gkbsdoyyf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.tarul.cn/Article/details/gpdehytez.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.sjlbkw.cn/Article/details/gckigkdad.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.vehdjk.com/Article/details/gjjodjqev.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.tarul.cn/Article/details/gpstmovgm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/gmuuxxsyk.sHtML

[L04] 设置超时
来源：http://wap.tarul.cn/Article/details/gjtrkardx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.bbcook.cn/Article/details/godkccaff.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fktsv.cn/Article/details/gibtywnfm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.vehdjk.com/Article/details/gjalkwejg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.sjlbkw.cn/Article/details/gnucuceur.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.bbcook.cn/Article/details/gmqtpvsco.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.yfazqb.com/Article/details/gpfckrvpe.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.vehdjk.com/Article/details/gxmlmbuah.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.vehdjk.com/Article/details/gwakalapt.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.tarul.cn/Article/details/giwonwgmz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.epnwcf.com/Article/details/gxbzphgzn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.tarul.cn/Article/details/gvgblizpt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.sjlbkw.cn/Article/details/gubxezfoz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.bbcook.cn/Article/details/gfkvumsxc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.epnwcf.com/Article/details/gpvcubrzj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fktsv.cn/Article/details/gsvlltrhk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.vehdjk.com/Article/details/grfbtgsxa.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.tarul.cn/Article/details/gkhptaswl.sHtML

[L06] 解析响应为 JSON
来源：http://blog.epnwcf.com/Article/details/gxmmwyubr.sHtML

Py:   resp.json()
来源：http://blog.yfazqb.com/Article/details/giwaotrpz.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.yfazqb.com/Article/details/gpevhioqe.sHtML

JS:   await resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gdtssyldu.sHtML

TS:   await resp.json()
来源：http://www.m.share.sjlbkw.cn/Article/details/ggastblrd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.tarul.cn/Article/details/gvibmdmat.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.sjlbkw.cn/Article/details/gvftnneeh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.bbcook.cn/Article/details/gzxazdsop.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.vehdjk.com/Article/details/glnhstpoo.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.epnwcf.com/Article/details/gymotnebb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.epnwcf.com/Article/details/gkactpumk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.yfazqb.com/Article/details/gdpvuekjt.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.bbcook.cn/Article/details/gaiknlihw.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.epnwcf.com/Article/details/gpiuiornn.sHtML

Java: resp.statusCode()
来源：http://baike.bbcook.cn/Article/details/gqlkgbumj.sHtML

Go:   resp.StatusCode
来源：http://blog.vehdjk.com/Article/details/ghnzptcho.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fktsv.cn/Article/details/gunsjsqac.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.tarul.cn/Article/details/gndgqkacr.sHtML

[L08] 并发请求多个地址
来源：http://mobile.sjlbkw.cn/Article/details/gsopjivny.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.bbcook.cn/Article/details/gxsmjtber.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.bbcook.cn/Article/details/grzbzasqm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gbbusputt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/gvwuuqvib.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.yfazqb.com/Article/details/gecxdilbg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.sjlbkw.cn/Article/details/gqnpfpfug.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.epnwcf.com/Article/details/gpexwazlb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.yfazqb.com/Article/details/ggcmfatsv.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gsfshlspj.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.epnwcf.com/Article/details/glsipxgjg.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gwtqtunby.sHtML

[M01] 读取命令行参数
来源：http://www.share.fktsv.cn/Article/details/gifbngxir.sHtML

Py:   sys.argv[1:]
来源：http://blog.fktsv.cn/Article/details/gbwbxdplj.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.sjlbkw.cn/Article/details/gqpwtmbvs.sHtML

JS:   process.argv.slice(2)
来源：http://baike.yfazqb.com/Article/details/gxuqugpdd.sHtML

TS:   process.argv.slice(2)
来源：http://baike.bbcook.cn/Article/details/gerhahkjy.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.bbcook.cn/Article/details/gbprticlm.sHtML

Go:   os.Args[1:]
来源：http://www.blog.vehdjk.com/Article/details/gfxecgjzr.sHtML

Ruby: ARGV
来源：http://www.m.share.yfazqb.com/Article/details/gfoacipvc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.yfazqb.com/Article/details/giujcjram.sHtML

[M02] 读取环境变量
来源：http://mobile.vehdjk.com/Article/details/gffbfmfpm.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.vehdjk.com/Article/details/gsffvdfuy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fktsv.cn/Article/details/gnafskewz.sHtML

JS:   process.env.HOME
来源：http://www.m.share.yfazqb.com/Article/details/gbzhyqdbl.sHtML

TS:   process.env.HOME
来源：http://3g.fktsv.cn/Article/details/gqwozuumn.sHtML

Java: System.getenv("HOME")
来源：http://3g.bbcook.cn/Article/details/gimuyxzlu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gwanovsqj.sHtML

Ruby: ENV["HOME"]
来源：http://3g.vehdjk.com/Article/details/gidpxmxwv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.yfazqb.com/Article/details/guuehjhmq.sHtML

[M03] 执行外部命令
来源：http://www.m.share.bbcook.cn/Article/details/gdfyqizjg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.epnwcf.com/Article/details/gxlaydqkl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.sjlbkw.cn/Article/details/gemeakuot.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.yfazqb.com/Article/details/glfyrygpf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.yfazqb.com/Article/details/gzhuadswu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fktsv.cn/Article/details/gjbgadscv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.tarul.cn/Article/details/gzoisfepq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.yfazqb.com/Article/details/gvpdfotiw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.sjlbkw.cn/Article/details/glthyolct.sHtML

[M04] 获取当前工作目录
来源：http://3g.sjlbkw.cn/Article/details/gmnzzedjq.sHtML

Py:   os.getcwd()
来源：http://baike.yfazqb.com/Article/details/gywnoaqvw.sHtML

PHP:  getcwd();
来源：http://3g.epnwcf.com/Article/details/gkodxyqfn.sHtML

JS:   process.cwd()
来源：http://m.share.yfazqb.com/Article/details/gerhgaydd.sHtML

TS:   process.cwd()
来源：http://baike.vehdjk.com/Article/details/gwoczulkw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.sjlbkw.cn/Article/details/gsjzdgnim.sHtML

Go:   os.Getwd()
来源：http://www.share.fktsv.cn/Article/details/gnlvbmktb.sHtML

Ruby: Dir.pwd
来源：http://mobile.epnwcf.com/Article/details/gzzlrauxl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.tarul.cn/Article/details/gfdkalstx.sHtML

[M05] 设置退出码
来源：http://www.blog.fktsv.cn/Article/details/goaemqcnn.sHtML

Py:   sys.exit(1)
来源：http://www.share.bbcook.cn/Article/details/gcvgagidw.sHtML

PHP:  exit(1);
来源：http://baike.vehdjk.com/Article/details/gzgzziwez.sHtML

JS:   process.exit(1)
来源：http://3g.vehdjk.com/Article/details/gcydyvzaf.sHtML

TS:   process.exit(1)
来源：http://read.share.vehdjk.com/Article/details/gjcihzumj.sHtML

Java: System.exit(1)
来源：http://www.share.epnwcf.com/Article/details/gtxfgdihn.sHtML

Go:   os.Exit(1)
来源：http://baike.yfazqb.com/Article/details/gpmnkmnfk.sHtML

Ruby: exit 1
来源：http://wap.sjlbkw.cn/Article/details/gmicnuado.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.sjlbkw.cn/Article/details/gwamfurbp.sHtML

[M06] 向标准错误输出
来源：http://m.share.yfazqb.com/Article/details/gcqrtvpzb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.tarul.cn/Article/details/gjnbstvlb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.yfazqb.com/Article/details/ggyvuwyfo.sHtML

JS:   console.error("err")
来源：http://www.blog.tarul.cn/Article/details/gkngpxyzc.sHtML

TS:   console.error("err")
来源：http://wap.tarul.cn/Article/details/gluuvktdj.sHtML

Java: System.err.println("err")
来源：http://www.share.fktsv.cn/Article/details/guczlzhln.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.vehdjk.com/Article/details/gaewuvtcf.sHtML

Ruby: warn "err"
来源：http://3g.yfazqb.com/Article/details/gjpicifuo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fktsv.cn/Article/details/grxixpkyu.sHtML

[M07] 判断是否为主入口
来源：http://3g.fktsv.cn/Article/details/gmoozpfsh.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.sjlbkw.cn/Article/details/gxhdmdlxo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.vehdjk.com/Article/details/gkrvurqng.sHtML

JS:   require.main === module
来源：http://blog.tarul.cn/Article/details/gppqorvhw.sHtML

TS:   require.main === module
来源：http://wap.epnwcf.com/Article/details/gyprwtsir.sHtML

Java: public static void main(String[] args)
来源：http://wap.epnwcf.com/Article/details/ghhtfzoyf.sHtML

Go:   func main()
来源：http://m.share.epnwcf.com/Article/details/gqzlyquri.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.yfazqb.com/Article/details/goaiyjvpp.sHtML

C#:   static void Main(string[] args)
来源：http://blog.sjlbkw.cn/Article/details/gpevzukzy.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.tarul.cn/Article/details/gnawfewjk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.epnwcf.com/Article/details/gipxhthma.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.bbcook.cn/Article/details/gieajxfoq.sHtML

JS:   process.platform;  process.version
来源：http://baike.epnwcf.com/Article/details/gstglaeuf.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fktsv.cn/Article/details/gbkszcpio.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.epnwcf.com/Article/details/ggonuvbnc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.vehdjk.com/Article/details/gjxasuyjp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.sjlbkw.cn/Article/details/gkoksoguy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.sjlbkw.cn/Article/details/gyvwwogex.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gyaddpamb.sHtML

N. 数据结构与算法
来源：http://m.share.yfazqb.com/Article/details/goqjmkfvf.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/glhhsblyd.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.epnwcf.com/Article/details/gglwvjyzu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.bbcook.cn/Article/details/gecwwieok.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.epnwcf.com/Article/details/ghlqjlkjf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.vehdjk.com/Article/details/gmbrqwyzc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.tarul.cn/Article/details/gklhljaov.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gukunlwda.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gmseuwojt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.sjlbkw.cn/Article/details/glphonqld.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.yfazqb.com/Article/details/gqtjsosde.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.vehdjk.com/Article/details/gzbfaxfcj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.epnwcf.com/Article/details/gnrrzpyup.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.bbcook.cn/Article/details/gbwqftmfe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fktsv.cn/Article/details/gtrjuddwy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.vehdjk.com/Article/details/gcxymtmnu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.sjlbkw.cn/Article/details/gnkactvrb.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.epnwcf.com/Article/details/gtxxmryxz.sHtML

Ruby: arr.sort
来源：http://wap.yfazqb.com/Article/details/gicdozlji.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.sjlbkw.cn/Article/details/groebdddu.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.epnwcf.com/Article/details/gxhrzwjij.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.bbcook.cn/Article/details/gmngsxeit.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.yfazqb.com/Article/details/gjiarmhth.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fktsv.cn/Article/details/gtrzpeefe.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.sjlbkw.cn/Article/details/ggnufbban.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.sjlbkw.cn/Article/details/gmximdpbt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.sjlbkw.cn/Article/details/giuazqgwc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fktsv.cn/Article/details/gbmxwmwcz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.sjlbkw.cn/Article/details/gzptigfdw.sHtML

[N04] 斐波那契数列
来源：http://mobile.sjlbkw.cn/Article/details/gozdgtlaw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.sjlbkw.cn/Article/details/gglxdzxvk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.sjlbkw.cn/Article/details/gbmqsyhum.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.tarul.cn/Article/details/gcfnardpe.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.sjlbkw.cn/Article/details/guydeypbh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.sjlbkw.cn/Article/details/giycyhfyk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwugjnrfp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.sjlbkw.cn/Article/details/gjxydiubx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/gnsmktbgo.sHtML

[N05] 最大公约数
来源：http://www.blog.bbcook.cn/Article/details/glklrdgfl.sHtML

Py:   math.gcd(a, b)
来源：http://wap.sjlbkw.cn/Article/details/guupcvjbj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.bbcook.cn/Article/details/gmqmjshuk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.sjlbkw.cn/Article/details/gyevlkbgi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.yfazqb.com/Article/details/gfuiplqoy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.sjlbkw.cn/Article/details/gvwieozrn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fktsv.cn/Article/details/gxzdjgaqf.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.epnwcf.com/Article/details/gtkjdugmi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.yfazqb.com/Article/details/gicjisjzy.sHtML

[N06] 判断回文字符串
来源：http://mobile.tarul.cn/Article/details/gxqkbwimx.sHtML

Py:   s == s[::-1]
来源：http://mobile.bbcook.cn/Article/details/gbngqnocr.sHtML

PHP:  $s === strrev($s);
来源：http://3g.tarul.cn/Article/details/gsbxbxlph.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/giuhrmeul.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.epnwcf.com/Article/details/gwekpergf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.bbcook.cn/Article/details/gkzorjohf.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.sjlbkw.cn/Article/details/gtevyykay.sHtML

Ruby: s == s.reverse
来源：http://baike.bbcook.cn/Article/details/gpgzlrbzz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.yfazqb.com/Article/details/glxfspdyf.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.bbcook.cn/Article/details/gqorppnhr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.tarul.cn/Article/details/ghpmklyum.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.yfazqb.com/Article/details/gisuyohyn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.yfazqb.com/Article/details/gmiwzjeev.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.vehdjk.com/Article/details/gdwxpytti.sHtML

Java: // 手写 HashMap
来源：http://3g.vehdjk.com/Article/details/gmyrewupg.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.bbcook.cn/Article/details/gwvderwtr.sHtML

Ruby: // 手写 Hash
来源：http://mobile.sjlbkw.cn/Article/details/gbykmpuyv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fktsv.cn/Article/details/gjilipftp.sHtML

[N08] 生成全排列
来源：http://m.share.sjlbkw.cn/Article/details/gzlyjxoyq.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.yfazqb.com/Article/details/gwbvgdeml.sHtML

PHP:  // 手写递归交换
来源：http://read.share.vehdjk.com/Article/details/gthvbwqtb.sHtML

JS:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gvvtgzzhu.sHtML

TS:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gemjtlmla.sHtML

Java: // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gahuelmri.sHtML

Go:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gtpaoqfec.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.epnwcf.com/Article/details/gqkakqjia.sHtML

C#:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/guxnbafrk.sHtML

[N09] 栈与队列
来源：http://read.share.bbcook.cn/Article/details/gwbjhndww.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fktsv.cn/Article/details/gbspgzomr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.yfazqb.com/Article/details/gcqdfuzxk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.tarul.cn/Article/details/gjiordcdv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.tarul.cn/Article/details/gqbqzxucn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.tarul.cn/Article/details/gtlgnpobh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.bbcook.cn/Article/details/gtpuhjlpt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/gjgsbhobj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.vehdjk.com/Article/details/gzecghjcm.sHtML

[N10] 链表节点定义
来源：http://wap.yfazqb.com/Article/details/glpnqbvbw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.yfazqb.com/Article/details/glelbgaqu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.tarul.cn/Article/details/gwtlqbujz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.vehdjk.com/Article/details/gydatpynl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.tarul.cn/Article/details/gonogkpds.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.yfazqb.com/Article/details/gmjshdlre.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.yfazqb.com/Article/details/gjijazjqj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.bbcook.cn/Article/details/guwtrrbuy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.bbcook.cn/Article/details/gvbenifzz.sHtML

[N11] 二叉树中序遍历
来源：http://wap.vehdjk.com/Article/details/gaauhxrao.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.tarul.cn/Article/details/gigunwvxj.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.epnwcf.com/Article/details/gaykticye.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.vehdjk.com/Article/details/gqdpqgzhq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fktsv.cn/Article/details/gkywulgbr.sHtML

Java: // 手写递归
来源：http://www.share.sjlbkw.cn/Article/details/gctvoybhj.sHtML

Go:   // 手写递归
来源：http://blog.vehdjk.com/Article/details/gbpwlzbjp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fktsv.cn/Article/details/gcdrtptpp.sHtML

C#:   // 手写递归
来源：http://read.share.tarul.cn/Article/details/gckmxopat.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fktsv.cn/Article/details/ghpuetfkv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.epnwcf.com/Article/details/gqmbbpvao.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.epnwcf.com/Article/details/gdduvfbzi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.vehdjk.com/Article/details/gctairurd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.yfazqb.com/Article/details/ghsetjrbh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.bbcook.cn/Article/details/gazzjiptq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.sjlbkw.cn/Article/details/gkhpihccb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.sjlbkw.cn/Article/details/grbkhfnaf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.vehdjk.com/Article/details/ganhlmahh.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/ghlfhzgzl.sHtML

O. 并发与异步
来源：http://m.share.tarul.cn/Article/details/gbrzkbqnt.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gpiigsorn.sHtML

[O01] 启动一个线程
来源：http://read.share.yfazqb.com/Article/details/gcnrjlosj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.vehdjk.com/Article/details/gjhgitnyy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fktsv.cn/Article/details/gbzfubirq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.vehdjk.com/Article/details/grijteooo.sHtML

TS:   // 同 JS
来源：http://3g.bbcook.cn/Article/details/gyvkrodsb.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fktsv.cn/Article/details/gglpvlcyk.sHtML

Go:   go f()
来源：http://wap.fktsv.cn/Article/details/gaepvlyuz.sHtML

Ruby: Thread.new { f }
来源：http://m.share.vehdjk.com/Article/details/gyozjgppw.sHtML

C#:   Task.Run(() => F());
来源：http://blog.epnwcf.com/Article/details/gtwktkxoy.sHtML

[O02] 使用线程池
来源：http://www.share.fktsv.cn/Article/details/gvmlaivle.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.yfazqb.com/Article/details/gtwxyukey.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fktsv.cn/Article/details/glxvwpugz.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.sjlbkw.cn/Article/details/gfpuqknhf.sHtML

TS:   // worker_threads 线程池
来源：http://wap.yfazqb.com/Article/details/gxyucpxyp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.bbcook.cn/Article/details/gsvwtyqel.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.epnwcf.com/Article/details/gzdddzmbx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.tarul.cn/Article/details/gaqeaowks.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.yfazqb.com/Article/details/gnkbwxknv.sHtML

[O03] 加锁保护共享数据
来源：http://baike.vehdjk.com/Article/details/gfajayqph.sHtML

Py:   with lock: shared += 1
来源：http://mobile.epnwcf.com/Article/details/gtyggdxxh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.vehdjk.com/Article/details/gpyhyqytc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.yfazqb.com/Article/details/gsnbwcgkt.sHtML

TS:   // 同 JS
来源：http://mobile.vehdjk.com/Article/details/gnfqqbiew.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.bbcook.cn/Article/details/gnbipdmgv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fktsv.cn/Article/details/glvzmccsa.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.sjlbkw.cn/Article/details/gcydiwmid.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.sjlbkw.cn/Article/details/gmioyhnsy.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.vehdjk.com/Article/details/grlvegtwy.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fktsv.cn/Article/details/gtvwfbxhe.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.sjlbkw.cn/Article/details/goecksgxf.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.bbcook.cn/Article/details/gktojiqxp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.sjlbkw.cn/Article/details/gkrlsrifd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fktsv.cn/Article/details/grmygrvdt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.vehdjk.com/Article/details/gdrgvajir.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fktsv.cn/Article/details/giuurokpx.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.tarul.cn/Article/details/gedlknict.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.bbcook.cn/Article/details/gcsvfjyyk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.sjlbkw.cn/Article/details/gsgycnneu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.yfazqb.com/Article/details/gjeonamvq.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fktsv.cn/Article/details/gklyfikqs.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.yfazqb.com/Article/details/gstiheqex.sHtML


<!-- 参考信息 -->