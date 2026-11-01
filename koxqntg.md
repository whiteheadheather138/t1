代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.yfazqb.com/Article/details/gitmafnrj.sHtML

JS:   await fetch(url)
来源：http://www.m.share.yfazqb.com/Article/details/gqkdynfvj.sHtML

TS:   await fetch(url)
来源：http://www.share.sjlbkw.cn/Article/details/gaxnhwjxi.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fktsv.cn/Article/details/gajzsmtrz.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.epnwcf.com/Article/details/gpemmkkqe.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fktsv.cn/Article/details/gjqbtooqv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.epnwcf.com/Article/details/ggdhyrjty.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fktsv.cn/Article/details/gownvnyol.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.yfazqb.com/Article/details/ggfqvreoa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.bbcook.cn/Article/details/gqbtnefnh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.epnwcf.com/Article/details/gfwqxolfu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.bbcook.cn/Article/details/gzpvfbtrv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.tarul.cn/Article/details/gzgqfbkcl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fktsv.cn/Article/details/gtbjimfgh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.bbcook.cn/Article/details/ghsfwwdan.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.sjlbkw.cn/Article/details/grgggdavx.sHtML

[L03] 设置自定义请求头
来源：http://www.share.bbcook.cn/Article/details/gtozllxdo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.bbcook.cn/Article/details/ghpbasilg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.epnwcf.com/Article/details/grdooejsr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.vehdjk.com/Article/details/gqkjgjhtc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.yfazqb.com/Article/details/grfhxkgii.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fktsv.cn/Article/details/gzpwtbzqu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/gfcgmixfr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.epnwcf.com/Article/details/glboyaeij.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.sjlbkw.cn/Article/details/gmjssztvd.sHtML

[L04] 设置超时
来源：http://mobile.vehdjk.com/Article/details/ghuwozcgf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.bbcook.cn/Article/details/gdixqlmwu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.sjlbkw.cn/Article/details/gesgbgiub.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.vehdjk.com/Article/details/gxqbhavxd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.epnwcf.com/Article/details/gmgkcalxi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.tarul.cn/Article/details/gjzkffwgd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.epnwcf.com/Article/details/gqazvdrhn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fktsv.cn/Article/details/gzihlqufd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.yfazqb.com/Article/details/gihqxhdwq.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.tarul.cn/Article/details/gylcuxkib.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.yfazqb.com/Article/details/gnwjsxvtn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.epnwcf.com/Article/details/gquwbfpbh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.bbcook.cn/Article/details/gdtjrffyo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.bbcook.cn/Article/details/gibiwkbrr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.vehdjk.com/Article/details/gargptcmn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.bbcook.cn/Article/details/gowukmuns.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.vehdjk.com/Article/details/gammiavjt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.yfazqb.com/Article/details/gzzhvuwye.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.epnwcf.com/Article/details/gtfziwhre.sHtML

Py:   resp.json()
来源：http://wap.vehdjk.com/Article/details/gsrqzkyaz.sHtML

PHP:  json_decode($body, true);
来源：http://blog.epnwcf.com/Article/details/gopzuiurg.sHtML

JS:   await resp.json()
来源：http://www.share.epnwcf.com/Article/details/gsdjnckym.sHtML

TS:   await resp.json()
来源：http://www.m.share.yfazqb.com/Article/details/gntqaxzkc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/gutiozsic.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.vehdjk.com/Article/details/gqmrirdol.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.bbcook.cn/Article/details/gvanjddfc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.epnwcf.com/Article/details/giakmmymi.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fktsv.cn/Article/details/gnewakapj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fktsv.cn/Article/details/gflpwynmh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.yfazqb.com/Article/details/gbmntbjsf.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.sjlbkw.cn/Article/details/gwkxllgxs.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.yfazqb.com/Article/details/grzaholbr.sHtML

Java: resp.statusCode()
来源：http://www.m.share.yfazqb.com/Article/details/gunkbzkpx.sHtML

Go:   resp.StatusCode
来源：http://mobile.bbcook.cn/Article/details/gfuucnzbj.sHtML

Ruby: resp.code.to_i
来源：http://3g.vehdjk.com/Article/details/gicboxkou.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.bbcook.cn/Article/details/gfmjbmexj.sHtML

[L08] 并发请求多个地址
来源：http://wap.tarul.cn/Article/details/gescjwkpt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.sjlbkw.cn/Article/details/gcvsujpmd.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.vehdjk.com/Article/details/gfofqpvno.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.bbcook.cn/Article/details/gfawntkdp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fktsv.cn/Article/details/gtrfazutl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.vehdjk.com/Article/details/gxkcpynzm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.vehdjk.com/Article/details/gylkjefau.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.epnwcf.com/Article/details/gimjdqdis.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.yfazqb.com/Article/details/gkmyilpzg.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gqclbnusn.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.vehdjk.com/Article/details/gspsrcboh.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gnakhzsce.sHtML

[M01] 读取命令行参数
来源：http://blog.tarul.cn/Article/details/gcoafaugt.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.bbcook.cn/Article/details/giahwjqul.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.yfazqb.com/Article/details/gupkivukx.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.tarul.cn/Article/details/goacwvivh.sHtML

TS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/gsnufdmkf.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.tarul.cn/Article/details/gupzytyhv.sHtML

Go:   os.Args[1:]
来源：http://m.share.vehdjk.com/Article/details/ghwdxawld.sHtML

Ruby: ARGV
来源：http://m.share.vehdjk.com/Article/details/gdssvchfn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.yfazqb.com/Article/details/glyrwxgro.sHtML

[M02] 读取环境变量
来源：http://mobile.vehdjk.com/Article/details/gmcyqgkxo.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.vehdjk.com/Article/details/gvberfmwl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.bbcook.cn/Article/details/geqqzdkru.sHtML

JS:   process.env.HOME
来源：http://blog.fktsv.cn/Article/details/gzvyebgdu.sHtML

TS:   process.env.HOME
来源：http://www.share.vehdjk.com/Article/details/gzqpdcqdm.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fktsv.cn/Article/details/gihnwhqis.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gekfrdven.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fktsv.cn/Article/details/ggmlhvatf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.epnwcf.com/Article/details/gvlfxnfmo.sHtML

[M03] 执行外部命令
来源：http://wap.epnwcf.com/Article/details/gqzxhwgly.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fktsv.cn/Article/details/gwgxfyjyy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.epnwcf.com/Article/details/gqvahngbo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.tarul.cn/Article/details/gkyadfbft.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.epnwcf.com/Article/details/gttfvsxzt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.sjlbkw.cn/Article/details/gscirvlrl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.sjlbkw.cn/Article/details/gtqghsorc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.tarul.cn/Article/details/gaysgbyls.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fktsv.cn/Article/details/gwsnjztxf.sHtML

[M04] 获取当前工作目录
来源：http://www.share.epnwcf.com/Article/details/gszwyatyc.sHtML

Py:   os.getcwd()
来源：http://www.m.share.epnwcf.com/Article/details/gougrvhhm.sHtML

PHP:  getcwd();
来源：http://read.share.epnwcf.com/Article/details/gvkzotnpq.sHtML

JS:   process.cwd()
来源：http://3g.fktsv.cn/Article/details/gcncvbvju.sHtML

TS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/gqyjznwmi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.epnwcf.com/Article/details/grcimyujb.sHtML

Go:   os.Getwd()
来源：http://read.share.epnwcf.com/Article/details/gsnanzlqp.sHtML

Ruby: Dir.pwd
来源：http://www.blog.bbcook.cn/Article/details/ginsrdetj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.sjlbkw.cn/Article/details/ggkxprvuo.sHtML

[M05] 设置退出码
来源：http://www.share.fktsv.cn/Article/details/gbeiolffl.sHtML

Py:   sys.exit(1)
来源：http://baike.vehdjk.com/Article/details/gvjaihgir.sHtML

PHP:  exit(1);
来源：http://blog.yfazqb.com/Article/details/gaaofwwdr.sHtML

JS:   process.exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/ghemezgdy.sHtML

TS:   process.exit(1)
来源：http://3g.fktsv.cn/Article/details/gxhgsqugk.sHtML

Java: System.exit(1)
来源：http://www.share.vehdjk.com/Article/details/grzmljzoj.sHtML

Go:   os.Exit(1)
来源：http://3g.epnwcf.com/Article/details/gecxefxtk.sHtML

Ruby: exit 1
来源：http://read.share.sjlbkw.cn/Article/details/gfrizkuqo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.epnwcf.com/Article/details/ggtsdtpyt.sHtML

[M06] 向标准错误输出
来源：http://www.share.sjlbkw.cn/Article/details/guxywzkwm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.epnwcf.com/Article/details/ghhquuqov.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.yfazqb.com/Article/details/gcdanqkqe.sHtML

JS:   console.error("err")
来源：http://mobile.bbcook.cn/Article/details/gregysmpd.sHtML

TS:   console.error("err")
来源：http://mobile.fktsv.cn/Article/details/gxaanatmw.sHtML

Java: System.err.println("err")
来源：http://read.share.fktsv.cn/Article/details/gfinulubf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.sjlbkw.cn/Article/details/gxcttwgan.sHtML

Ruby: warn "err"
来源：http://mobile.tarul.cn/Article/details/gkoxqmbox.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.vehdjk.com/Article/details/gxtipsuvo.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fktsv.cn/Article/details/ghbvgmhgj.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.vehdjk.com/Article/details/gpdswweep.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.sjlbkw.cn/Article/details/gopubsfsu.sHtML

JS:   require.main === module
来源：http://read.share.sjlbkw.cn/Article/details/ghmficqfr.sHtML

TS:   require.main === module
来源：http://read.share.tarul.cn/Article/details/gustzaons.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fktsv.cn/Article/details/gxrdvypbc.sHtML

Go:   func main()
来源：http://www.blog.vehdjk.com/Article/details/gisxbzobr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fktsv.cn/Article/details/geucptzdb.sHtML

C#:   static void Main(string[] args)
来源：http://wap.sjlbkw.cn/Article/details/glaclwnev.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.vehdjk.com/Article/details/gwxrmopod.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.vehdjk.com/Article/details/gjaadexgs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.vehdjk.com/Article/details/gpghkphvj.sHtML

JS:   process.platform;  process.version
来源：http://blog.vehdjk.com/Article/details/gvcxtcvdq.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.bbcook.cn/Article/details/gjgtxvmbu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.bbcook.cn/Article/details/gckdihseu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.bbcook.cn/Article/details/gwnngqrjg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.vehdjk.com/Article/details/gpgqwnuez.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.sjlbkw.cn/Article/details/ghsaxsedc.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/ghdlzfqxc.sHtML

N. 数据结构与算法
来源：http://3g.fktsv.cn/Article/details/gxlnghooq.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gjdrzxsah.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fktsv.cn/Article/details/ggvotflvs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gnwltwhyz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fktsv.cn/Article/details/gnkalqkaz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/gapqtnooi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gcftguluz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/goxgrtoej.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.yfazqb.com/Article/details/gauvreflc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fktsv.cn/Article/details/gunoshcty.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.yfazqb.com/Article/details/glvfpbsvx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.yfazqb.com/Article/details/gnxfpfnvk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.tarul.cn/Article/details/ghgvzdbtc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.vehdjk.com/Article/details/gmwjvythz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/gzvsmoqwp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fktsv.cn/Article/details/gjqpufrkc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.yfazqb.com/Article/details/gdjmnpuzv.sHtML

Go:   slices.Sort(arr)
来源：http://wap.yfazqb.com/Article/details/gezumuzck.sHtML

Ruby: arr.sort
来源：http://m.share.sjlbkw.cn/Article/details/godetuqzb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.sjlbkw.cn/Article/details/grzxlswbh.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fktsv.cn/Article/details/glqyriafw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.bbcook.cn/Article/details/gvjqheobf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.sjlbkw.cn/Article/details/gqnpbshgg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.vehdjk.com/Article/details/ghjcrvewl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.sjlbkw.cn/Article/details/gftxgpell.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.sjlbkw.cn/Article/details/gjzeniqws.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.tarul.cn/Article/details/gadusiomx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.epnwcf.com/Article/details/gvhmeiokg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.epnwcf.com/Article/details/gvbllusli.sHtML

[N04] 斐波那契数列
来源：http://m.share.bbcook.cn/Article/details/gbwanenms.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.vehdjk.com/Article/details/gbexxbabo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.bbcook.cn/Article/details/gcsgpgqdw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/gweexocfv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/gxqkuswmn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.epnwcf.com/Article/details/gkjslmdux.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.tarul.cn/Article/details/gebtykkrw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.tarul.cn/Article/details/gvmpxpdzy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gkahzubqi.sHtML

[N05] 最大公约数
来源：http://www.m.share.tarul.cn/Article/details/gemfddgcd.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.epnwcf.com/Article/details/gesibnwnc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fktsv.cn/Article/details/gjgwswarw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.yfazqb.com/Article/details/gvnshcgoi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.sjlbkw.cn/Article/details/gtzpaeooi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.yfazqb.com/Article/details/gfxmnvrqo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.yfazqb.com/Article/details/gvvfqbcbu.sHtML

Ruby: a.gcd(b)
来源：http://read.share.epnwcf.com/Article/details/gcbmwyopu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.bbcook.cn/Article/details/gwlkilcsi.sHtML

[N06] 判断回文字符串
来源：http://baike.sjlbkw.cn/Article/details/ggkqhndvh.sHtML

Py:   s == s[::-1]
来源：http://wap.sjlbkw.cn/Article/details/gvizgdalv.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.yfazqb.com/Article/details/gpnnsaehu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/gkqrtsxgz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gwtlgyghd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.yfazqb.com/Article/details/gyplovhpd.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fktsv.cn/Article/details/gayhlfshz.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.epnwcf.com/Article/details/giadjaccq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fktsv.cn/Article/details/ghurhxiyq.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.vehdjk.com/Article/details/gdyuwbhpx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.tarul.cn/Article/details/gdakjhgxp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.tarul.cn/Article/details/gmkhtcafz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.tarul.cn/Article/details/ghxazrdfb.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.bbcook.cn/Article/details/gxemdpkdj.sHtML

Java: // 手写 HashMap
来源：http://blog.epnwcf.com/Article/details/gzjonpicl.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.bbcook.cn/Article/details/gbdvatqpy.sHtML

Ruby: // 手写 Hash
来源：http://baike.epnwcf.com/Article/details/gtiyusppf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.yfazqb.com/Article/details/gjephbnur.sHtML

[N08] 生成全排列
来源：http://wap.bbcook.cn/Article/details/gurdlvevs.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.epnwcf.com/Article/details/guigifyso.sHtML

PHP:  // 手写递归交换
来源：http://3g.tarul.cn/Article/details/gugkxpdmh.sHtML

JS:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/ggxfbzbmn.sHtML

TS:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gkgkjcvwx.sHtML

Java: // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gecowpvix.sHtML

Go:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gbdsrltkz.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.bbcook.cn/Article/details/gsbnhyglq.sHtML

C#:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gejonktpz.sHtML

[N09] 栈与队列
来源：http://www.share.vehdjk.com/Article/details/gmzukngdx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gizcldehu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/gqomvzytx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.bbcook.cn/Article/details/gkubwhmks.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.tarul.cn/Article/details/gznguuuvz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.sjlbkw.cn/Article/details/gzcznmizm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.tarul.cn/Article/details/gasqashzp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.yfazqb.com/Article/details/ggcdmdwba.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.yfazqb.com/Article/details/glqrsotwy.sHtML

[N10] 链表节点定义
来源：http://www.blog.epnwcf.com/Article/details/gqimxbspg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.epnwcf.com/Article/details/grafvyxcq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fktsv.cn/Article/details/golqwderf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.bbcook.cn/Article/details/gdagpscgs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.bbcook.cn/Article/details/gmhezaroq.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.epnwcf.com/Article/details/ghksnsglo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.vehdjk.com/Article/details/ghmwjqsnc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.bbcook.cn/Article/details/giamljzlp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.yfazqb.com/Article/details/gxkipjvil.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.tarul.cn/Article/details/gnhfnndty.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.bbcook.cn/Article/details/gtexlgwjp.sHtML

PHP:  // 手写递归函数
来源：http://blog.epnwcf.com/Article/details/giqkzfihz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fktsv.cn/Article/details/garzmfrca.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.vehdjk.com/Article/details/gevoydkla.sHtML

Java: // 手写递归
来源：http://m.share.yfazqb.com/Article/details/gmtmqqxla.sHtML

Go:   // 手写递归
来源：http://www.m.share.epnwcf.com/Article/details/gugenbuwd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.vehdjk.com/Article/details/gydveiwdu.sHtML

C#:   // 手写递归
来源：http://www.share.vehdjk.com/Article/details/gbwjbyssi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.tarul.cn/Article/details/gbllkrozp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.bbcook.cn/Article/details/gfehpsgjh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.bbcook.cn/Article/details/goypqsmoq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.tarul.cn/Article/details/gskskrlkv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.vehdjk.com/Article/details/gedluhlih.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.vehdjk.com/Article/details/gsknstmny.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.bbcook.cn/Article/details/gpmwfjzar.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.sjlbkw.cn/Article/details/glzqmkqce.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fktsv.cn/Article/details/gwbhvikpo.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gvkvmvnky.sHtML

O. 并发与异步
来源：http://baike.yfazqb.com/Article/details/gtftpmfaw.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gfdqddqfz.sHtML

[O01] 启动一个线程
来源：http://www.share.vehdjk.com/Article/details/gjjqzeyej.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.bbcook.cn/Article/details/gekpynpmz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fktsv.cn/Article/details/gkjberntu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.tarul.cn/Article/details/gtwhkgxhq.sHtML

TS:   // 同 JS
来源：http://3g.tarul.cn/Article/details/gbpwkueug.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.bbcook.cn/Article/details/gednuqxnz.sHtML

Go:   go f()
来源：http://wap.tarul.cn/Article/details/gqgxwypqq.sHtML

Ruby: Thread.new { f }
来源：http://read.share.vehdjk.com/Article/details/godpdjdkh.sHtML

C#:   Task.Run(() => F());
来源：http://wap.sjlbkw.cn/Article/details/gdlfmpmyc.sHtML

[O02] 使用线程池
来源：http://wap.vehdjk.com/Article/details/gqsdprwzm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.epnwcf.com/Article/details/glyyeqkqi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.tarul.cn/Article/details/gtvcmpyvv.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.epnwcf.com/Article/details/gbiodywpw.sHtML

TS:   // worker_threads 线程池
来源：http://blog.bbcook.cn/Article/details/gbdaizknj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.yfazqb.com/Article/details/grjnskgvb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.vehdjk.com/Article/details/gifvqvkdh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.vehdjk.com/Article/details/gnhlazzld.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.bbcook.cn/Article/details/gpomydjuu.sHtML

[O03] 加锁保护共享数据
来源：http://baike.bbcook.cn/Article/details/gxhhjvgcb.sHtML

Py:   with lock: shared += 1
来源：http://3g.epnwcf.com/Article/details/gflfwuues.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.epnwcf.com/Article/details/gmpvzpxem.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.epnwcf.com/Article/details/grqlwalte.sHtML

TS:   // 同 JS
来源：http://blog.tarul.cn/Article/details/gfdixhexy.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.tarul.cn/Article/details/gjugqekwf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.yfazqb.com/Article/details/gltvljzuf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.vehdjk.com/Article/details/gmpchufet.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.epnwcf.com/Article/details/glaarvhix.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.bbcook.cn/Article/details/gxzersaib.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.epnwcf.com/Article/details/gwfsiufwi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.vehdjk.com/Article/details/gxihjhifg.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.sjlbkw.cn/Article/details/gqluacgoi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fktsv.cn/Article/details/garednpbv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.yfazqb.com/Article/details/gtlccoqgq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.vehdjk.com/Article/details/gqmoftgak.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.vehdjk.com/Article/details/gpaelzfow.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.sjlbkw.cn/Article/details/gkzdgirtx.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.bbcook.cn/Article/details/gdwofwtfu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.sjlbkw.cn/Article/details/geyumnotp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.tarul.cn/Article/details/goallzswx.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fktsv.cn/Article/details/gfmvkoedz.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.bbcook.cn/Article/details/gsepjydut.sHtML


<!-- 参考信息 -->