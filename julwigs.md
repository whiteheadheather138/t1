代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.vehdjk.com/Article/details/gagtwityw.sHtML

JS:   await fetch(url)
来源：http://3g.sjlbkw.cn/Article/details/gihjwlmje.sHtML

TS:   await fetch(url)
来源：http://3g.tarul.cn/Article/details/gtgtcjdvz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.tarul.cn/Article/details/gaodgyxwh.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.bbcook.cn/Article/details/gpkdkogwq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.vehdjk.com/Article/details/gpxtjdifg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjgyqszpw.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.vehdjk.com/Article/details/glyujxirv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.vehdjk.com/Article/details/grudhfexu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.tarul.cn/Article/details/gmdkhydtr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.yfazqb.com/Article/details/ghwgzsvlp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzysjvzf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.tarul.cn/Article/details/garqvvyno.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fktsv.cn/Article/details/glcsonrcz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.vehdjk.com/Article/details/ggeiolcnu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.sjlbkw.cn/Article/details/guoeyewmv.sHtML

[L03] 设置自定义请求头
来源：http://mobile.bbcook.cn/Article/details/ggllhvckh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.vehdjk.com/Article/details/gocgwogce.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.yfazqb.com/Article/details/gsjctqdss.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.yfazqb.com/Article/details/gpsmsmlfq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fktsv.cn/Article/details/ggivutznx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fktsv.cn/Article/details/gqwfiqxaz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.sjlbkw.cn/Article/details/gxueeczcl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.vehdjk.com/Article/details/gkelanprb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.epnwcf.com/Article/details/gwlrwjlxd.sHtML

[L04] 设置超时
来源：http://mobile.bbcook.cn/Article/details/gblzijfoz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.tarul.cn/Article/details/gsswuqbwp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.vehdjk.com/Article/details/goygmblpk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.tarul.cn/Article/details/goxgofgwf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.bbcook.cn/Article/details/gvjdnvqvb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fktsv.cn/Article/details/grqvbsljj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.yfazqb.com/Article/details/giupumqje.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.bbcook.cn/Article/details/gzhmuysnr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.tarul.cn/Article/details/gvzhoecwd.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.yfazqb.com/Article/details/gumjqpyjn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fktsv.cn/Article/details/gqptepqsn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.yfazqb.com/Article/details/gyqvsjvaj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.tarul.cn/Article/details/gbywplrbe.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.tarul.cn/Article/details/gdbirtwxz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.bbcook.cn/Article/details/gqzrzfkgk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.yfazqb.com/Article/details/gppkpumcc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.bbcook.cn/Article/details/gfmpbvnnn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gjoppqmek.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.tarul.cn/Article/details/glubuspnm.sHtML

Py:   resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/gtfxkwjmt.sHtML

PHP:  json_decode($body, true);
来源：http://baike.tarul.cn/Article/details/gzqaivjot.sHtML

JS:   await resp.json()
来源：http://blog.vehdjk.com/Article/details/gfhvkycpc.sHtML

TS:   await resp.json()
来源：http://www.share.vehdjk.com/Article/details/gefhhcnfe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.vehdjk.com/Article/details/gyqwheonm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.yfazqb.com/Article/details/gscwvxtyn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.yfazqb.com/Article/details/gqbccdeqf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.vehdjk.com/Article/details/gqnesszjf.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fktsv.cn/Article/details/gzivlnagh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.bbcook.cn/Article/details/gdabqevpi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fktsv.cn/Article/details/gxnnpvary.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.sjlbkw.cn/Article/details/grkuztzzd.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.bbcook.cn/Article/details/glprcvomm.sHtML

Java: resp.statusCode()
来源：http://m.share.bbcook.cn/Article/details/gdkbaplxz.sHtML

Go:   resp.StatusCode
来源：http://blog.vehdjk.com/Article/details/givifzzmr.sHtML

Ruby: resp.code.to_i
来源：http://3g.vehdjk.com/Article/details/gbbjatfun.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.tarul.cn/Article/details/gcxikqqjy.sHtML

[L08] 并发请求多个地址
来源：http://baike.tarul.cn/Article/details/gqvzgppku.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.sjlbkw.cn/Article/details/gtleqntmo.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.bbcook.cn/Article/details/gtxcivsvh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlsaynfh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.vehdjk.com/Article/details/gtfhaljgm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fktsv.cn/Article/details/gqgetyrai.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.epnwcf.com/Article/details/goxjbbaee.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.vehdjk.com/Article/details/gsnbqvrkf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.yfazqb.com/Article/details/gegbzvfyw.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gxmpusthu.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.epnwcf.com/Article/details/gkfuxvkef.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gluamcyce.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.bbcook.cn/Article/details/goompgmlx.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.bbcook.cn/Article/details/gojgtxgba.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.tarul.cn/Article/details/ganvgdtda.sHtML

JS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/gtoixpqqg.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.epnwcf.com/Article/details/gkfstidfm.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.yfazqb.com/Article/details/gyvdzxrug.sHtML

Go:   os.Args[1:]
来源：http://3g.sjlbkw.cn/Article/details/govgwtewb.sHtML

Ruby: ARGV
来源：http://baike.sjlbkw.cn/Article/details/gjrggvzox.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.yfazqb.com/Article/details/gdkkadolv.sHtML

[M02] 读取环境变量
来源：http://wap.sjlbkw.cn/Article/details/gshwkqzlj.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.sjlbkw.cn/Article/details/gdznxjzdp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.epnwcf.com/Article/details/gcljzmvgd.sHtML

JS:   process.env.HOME
来源：http://blog.fktsv.cn/Article/details/glqxnwuar.sHtML

TS:   process.env.HOME
来源：http://blog.tarul.cn/Article/details/gezykqhxw.sHtML

Java: System.getenv("HOME")
来源：http://wap.tarul.cn/Article/details/gpjqyhxgt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.epnwcf.com/Article/details/gjoxugccx.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.epnwcf.com/Article/details/grglfqxqc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqynecwth.sHtML

[M03] 执行外部命令
来源：http://m.share.yfazqb.com/Article/details/gualmkcpu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.bbcook.cn/Article/details/gwnkiljvi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.sjlbkw.cn/Article/details/gangbrjgs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.vehdjk.com/Article/details/gjzpvdrzx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.tarul.cn/Article/details/gcdfaqidu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fktsv.cn/Article/details/ghwubtpfy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fktsv.cn/Article/details/gigzlekjb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.vehdjk.com/Article/details/ghifapvox.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.vehdjk.com/Article/details/gmupzpmrg.sHtML

[M04] 获取当前工作目录
来源：http://wap.yfazqb.com/Article/details/gouqktrth.sHtML

Py:   os.getcwd()
来源：http://m.share.epnwcf.com/Article/details/gjqxjnfrn.sHtML

PHP:  getcwd();
来源：http://www.blog.sjlbkw.cn/Article/details/goimuwjik.sHtML

JS:   process.cwd()
来源：http://baike.vehdjk.com/Article/details/gvzjeotgt.sHtML

TS:   process.cwd()
来源：http://3g.tarul.cn/Article/details/gjdasxtlo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.bbcook.cn/Article/details/guhakyfgp.sHtML

Go:   os.Getwd()
来源：http://m.share.fktsv.cn/Article/details/gsgdrljko.sHtML

Ruby: Dir.pwd
来源：http://read.share.sjlbkw.cn/Article/details/gwuncprro.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.tarul.cn/Article/details/gefgqarbb.sHtML

[M05] 设置退出码
来源：http://mobile.yfazqb.com/Article/details/godbcoshz.sHtML

Py:   sys.exit(1)
来源：http://3g.fktsv.cn/Article/details/gkmiquzpj.sHtML

PHP:  exit(1);
来源：http://wap.tarul.cn/Article/details/gzfgpvclx.sHtML

JS:   process.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gllsyhyko.sHtML

TS:   process.exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gboylsdyj.sHtML

Java: System.exit(1)
来源：http://wap.epnwcf.com/Article/details/gmihgnndu.sHtML

Go:   os.Exit(1)
来源：http://mobile.vehdjk.com/Article/details/gxrnsgxea.sHtML

Ruby: exit 1
来源：http://baike.bbcook.cn/Article/details/gjquslomz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.bbcook.cn/Article/details/gfmpyvbgw.sHtML

[M06] 向标准错误输出
来源：http://m.share.sjlbkw.cn/Article/details/glxgkfeey.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.epnwcf.com/Article/details/gczujrxpm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.vehdjk.com/Article/details/gaqbukjxw.sHtML

JS:   console.error("err")
来源：http://m.share.bbcook.cn/Article/details/gyreoqwhe.sHtML

TS:   console.error("err")
来源：http://m.share.yfazqb.com/Article/details/gjudtxvdz.sHtML

Java: System.err.println("err")
来源：http://www.blog.tarul.cn/Article/details/gpzpoopgr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.yfazqb.com/Article/details/gynjngrmx.sHtML

Ruby: warn "err"
来源：http://baike.vehdjk.com/Article/details/gnnminsne.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fktsv.cn/Article/details/gafpehwlj.sHtML

[M07] 判断是否为主入口
来源：http://mobile.vehdjk.com/Article/details/gjwqpywxa.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.sjlbkw.cn/Article/details/ghixrfmaf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.sjlbkw.cn/Article/details/gdqpzdsmq.sHtML

JS:   require.main === module
来源：http://3g.bbcook.cn/Article/details/gxnvihqns.sHtML

TS:   require.main === module
来源：http://blog.sjlbkw.cn/Article/details/gsnrbetup.sHtML

Java: public static void main(String[] args)
来源：http://wap.epnwcf.com/Article/details/gptpbccxp.sHtML

Go:   func main()
来源：http://www.m.share.vehdjk.com/Article/details/gcvgqklqn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.vehdjk.com/Article/details/gumbhnyuc.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fktsv.cn/Article/details/ggdwvgpwo.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.epnwcf.com/Article/details/gvdgekatw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fktsv.cn/Article/details/gaexsisvz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fktsv.cn/Article/details/grtysbvey.sHtML

JS:   process.platform;  process.version
来源：http://blog.vehdjk.com/Article/details/ghucejteq.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fktsv.cn/Article/details/gofxveepe.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.bbcook.cn/Article/details/gbjupjtfu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.epnwcf.com/Article/details/gugnxwxzv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.vehdjk.com/Article/details/gqmfspkkf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.tarul.cn/Article/details/gphspoiav.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ghmaekuyr.sHtML

N. 数据结构与算法
来源：http://m.share.tarul.cn/Article/details/gfukgdetq.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gvdspkvyc.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.tarul.cn/Article/details/gvnzhossb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fktsv.cn/Article/details/gajdffvca.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.bbcook.cn/Article/details/gotupcucz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.bbcook.cn/Article/details/gfnpwcadu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.bbcook.cn/Article/details/ghjgaxtwb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.epnwcf.com/Article/details/ghgixkvrf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.bbcook.cn/Article/details/gdxsxkodn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.tarul.cn/Article/details/gpbnkrjwu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gjmmmhvzt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.yfazqb.com/Article/details/gfjlxrvda.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.bbcook.cn/Article/details/gvcpmtlpo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.vehdjk.com/Article/details/govxqjnvy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/gtdmcjyob.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fktsv.cn/Article/details/grpqrprbu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.bbcook.cn/Article/details/gwbjpiocs.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.vehdjk.com/Article/details/gifyfxppv.sHtML

Ruby: arr.sort
来源：http://m.share.fktsv.cn/Article/details/gzfxojhbk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fktsv.cn/Article/details/gvbgwvnfd.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.vehdjk.com/Article/details/glhydbxcd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fktsv.cn/Article/details/guiylsutb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.yfazqb.com/Article/details/gfsimcolb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.vehdjk.com/Article/details/gnvcannqe.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.yfazqb.com/Article/details/gdlzppnem.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fktsv.cn/Article/details/grgbckdnl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.bbcook.cn/Article/details/gtujzkzml.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.tarul.cn/Article/details/gzvnegdul.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.yfazqb.com/Article/details/gychljian.sHtML

[N04] 斐波那契数列
来源：http://mobile.yfazqb.com/Article/details/gtawamcxn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.vehdjk.com/Article/details/ghozykgnq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.epnwcf.com/Article/details/gnpftwsif.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gyhnliujf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/gfwartddr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.tarul.cn/Article/details/gpptoswvg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.bbcook.cn/Article/details/gtashngya.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.epnwcf.com/Article/details/gowckcxwm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/gvutaoxmd.sHtML

[N05] 最大公约数
来源：http://www.blog.yfazqb.com/Article/details/gpbsbkndw.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.epnwcf.com/Article/details/gemdkxfzu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.vehdjk.com/Article/details/ggjbqdzgs.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.bbcook.cn/Article/details/gfbxipjpm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.sjlbkw.cn/Article/details/gbliabzzt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.epnwcf.com/Article/details/grcnzwgpz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.yfazqb.com/Article/details/gxdhhoxvn.sHtML

Ruby: a.gcd(b)
来源：http://baike.yfazqb.com/Article/details/gnjhafhot.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.epnwcf.com/Article/details/gnegtqvuo.sHtML

[N06] 判断回文字符串
来源：http://blog.yfazqb.com/Article/details/gdofyudpn.sHtML

Py:   s == s[::-1]
来源：http://www.share.yfazqb.com/Article/details/gkwhiefhd.sHtML

PHP:  $s === strrev($s);
来源：http://wap.yfazqb.com/Article/details/gquwndmvo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/gdaydjkyk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.sjlbkw.cn/Article/details/gotxckjhh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.yfazqb.com/Article/details/gndtwmdgy.sHtML

Go:   // 双指针从两端比较
来源：http://blog.tarul.cn/Article/details/gpjkkpyus.sHtML

Ruby: s == s.reverse
来源：http://wap.fktsv.cn/Article/details/gqhitklcs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.vehdjk.com/Article/details/gfchkhkwk.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.tarul.cn/Article/details/gsdmztilq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.bbcook.cn/Article/details/gwuhqvmlw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.vehdjk.com/Article/details/gtnxndlby.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.bbcook.cn/Article/details/gjbrrctxh.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.bbcook.cn/Article/details/gbtfacocc.sHtML

Java: // 手写 HashMap
来源：http://mobile.tarul.cn/Article/details/gahvnlbwn.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fktsv.cn/Article/details/gmywaebzb.sHtML

Ruby: // 手写 Hash
来源：http://3g.vehdjk.com/Article/details/gbfgqlygr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.yfazqb.com/Article/details/gxwkcmvld.sHtML

[N08] 生成全排列
来源：http://read.share.bbcook.cn/Article/details/gcsopcyyp.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.epnwcf.com/Article/details/gvrcaojrr.sHtML

PHP:  // 手写递归交换
来源：http://m.share.yfazqb.com/Article/details/gpfoadxqq.sHtML

JS:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gwcupqzzv.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gmrjzzitd.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gjvsccjwy.sHtML

Go:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gaukcadzj.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fktsv.cn/Article/details/gtpiigjny.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gkxaqjfqx.sHtML

[N09] 栈与队列
来源：http://wap.fktsv.cn/Article/details/ghsvsjcoe.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdwgvnfl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.yfazqb.com/Article/details/gbjwwddzm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.bbcook.cn/Article/details/gnnquravr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fktsv.cn/Article/details/gomxiocjf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.vehdjk.com/Article/details/gwvdjhawe.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.epnwcf.com/Article/details/gakoktybg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.tarul.cn/Article/details/ghmgdvtfn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.sjlbkw.cn/Article/details/gyvxxlwfw.sHtML

[N10] 链表节点定义
来源：http://baike.tarul.cn/Article/details/gthmktdbk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.tarul.cn/Article/details/gkvmmgbqj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.sjlbkw.cn/Article/details/gzbivjpsq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.bbcook.cn/Article/details/gtxpvbwgn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fktsv.cn/Article/details/glozjxpam.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.yfazqb.com/Article/details/giotgvbmt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.sjlbkw.cn/Article/details/gkcxxuycn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.epnwcf.com/Article/details/gijikkkyk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.tarul.cn/Article/details/guczbxuqg.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.yfazqb.com/Article/details/gwfaygepy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.bbcook.cn/Article/details/gumpugkxm.sHtML

PHP:  // 手写递归函数
来源：http://www.share.sjlbkw.cn/Article/details/ghodhjoch.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.vehdjk.com/Article/details/guytdpljm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.yfazqb.com/Article/details/gelsjgxpv.sHtML

Java: // 手写递归
来源：http://3g.sjlbkw.cn/Article/details/gicrrnpfr.sHtML

Go:   // 手写递归
来源：http://baike.tarul.cn/Article/details/gwwkoqxuc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.tarul.cn/Article/details/gldtsumlx.sHtML

C#:   // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/gsmubhlbm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.bbcook.cn/Article/details/geywxbxyu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.yfazqb.com/Article/details/glxvcuvsb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.bbcook.cn/Article/details/gzpmtfyba.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.vehdjk.com/Article/details/gfidkpsta.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.bbcook.cn/Article/details/gapkorrvc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.bbcook.cn/Article/details/gsffmodmj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.sjlbkw.cn/Article/details/glzcyerji.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.tarul.cn/Article/details/gbdtxmwld.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.sjlbkw.cn/Article/details/golywiugk.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gsrpbihih.sHtML

O. 并发与异步
来源：http://www.m.share.tarul.cn/Article/details/gjbuvhvgb.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gsrrrfuqj.sHtML

[O01] 启动一个线程
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvzfjgww.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.epnwcf.com/Article/details/gfqkwtlpc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.sjlbkw.cn/Article/details/guxenuote.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.yfazqb.com/Article/details/gpswftdaj.sHtML

TS:   // 同 JS
来源：http://www.blog.bbcook.cn/Article/details/gfhdxvbvn.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.vehdjk.com/Article/details/gievrklio.sHtML

Go:   go f()
来源：http://read.share.yfazqb.com/Article/details/gosvgfiro.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fktsv.cn/Article/details/glhktqrpb.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.yfazqb.com/Article/details/gidekbkdi.sHtML

[O02] 使用线程池
来源：http://wap.bbcook.cn/Article/details/gdscftzzb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.vehdjk.com/Article/details/gosnuzyfd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.yfazqb.com/Article/details/gujbdqihd.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.yfazqb.com/Article/details/gpemyujwf.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.bbcook.cn/Article/details/gljqtioxn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.vehdjk.com/Article/details/gvsdkmonr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.epnwcf.com/Article/details/gpfjsiabk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.yfazqb.com/Article/details/gmfeucjbz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.bbcook.cn/Article/details/gvpbhslsq.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.yfazqb.com/Article/details/grafmowsw.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.yfazqb.com/Article/details/gottqyrzv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fktsv.cn/Article/details/ghpttiwxw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.sjlbkw.cn/Article/details/gktimgjfg.sHtML

TS:   // 同 JS
来源：http://read.share.yfazqb.com/Article/details/gzbfrdohx.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.epnwcf.com/Article/details/gxjkknlvv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.tarul.cn/Article/details/gohsexexq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.yfazqb.com/Article/details/gvcyxoppt.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.vehdjk.com/Article/details/genqiutnt.sHtML

[O04] 定义异步函数并等待
来源：http://3g.tarul.cn/Article/details/gnmawnefs.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.bbcook.cn/Article/details/gecwalvkw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.tarul.cn/Article/details/gxtpycbpp.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.sjlbkw.cn/Article/details/gsowelbsu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghlbpqjlu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.sjlbkw.cn/Article/details/gmdowgwim.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.yfazqb.com/Article/details/gskklyjxt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.tarul.cn/Article/details/gaokrdmln.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.sjlbkw.cn/Article/details/grubxkvpm.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.tarul.cn/Article/details/gxbqamkcg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.epnwcf.com/Article/details/gryfmnnyw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fktsv.cn/Article/details/gngubupcy.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.sjlbkw.cn/Article/details/gooefrbbd.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.vehdjk.com/Article/details/glsgouhng.sHtML


<!-- 参考信息 -->