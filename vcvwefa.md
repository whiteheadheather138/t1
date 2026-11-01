代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://baike.epnwcf.com/Article/details/gmuzxlbmg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fktsv.cn/Article/details/gzyzvcati.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fktsv.cn/Article/details/gfxrxkzsd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.tarul.cn/Article/details/gtvernnnu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.tarul.cn/Article/details/gtqfkpecv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.sjlbkw.cn/Article/details/gvrxyqctb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.tarul.cn/Article/details/gmcrfggef.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fktsv.cn/Article/details/gszzppsih.sHtML

[L03] 设置自定义请求头
来源：http://wap.yfazqb.com/Article/details/gthmfatct.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.bbcook.cn/Article/details/gugltvsdn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.bbcook.cn/Article/details/gziimigil.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.bbcook.cn/Article/details/gondrcuxk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.yfazqb.com/Article/details/gwxveqooj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.epnwcf.com/Article/details/gbimemxgm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/gapwlrnon.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fktsv.cn/Article/details/gvmnfkzpu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.sjlbkw.cn/Article/details/gvtmkxbua.sHtML

[L04] 设置超时
来源：http://www.m.share.sjlbkw.cn/Article/details/grqatfdhr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.bbcook.cn/Article/details/gfzltqzjp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.sjlbkw.cn/Article/details/grgxirelk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.yfazqb.com/Article/details/guyfkfrpp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.bbcook.cn/Article/details/gndljtwrl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fktsv.cn/Article/details/gopqcipxp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fktsv.cn/Article/details/giwvoauhr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.tarul.cn/Article/details/gsutlgqnu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.sjlbkw.cn/Article/details/gcllxxkmr.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.bbcook.cn/Article/details/grppbzslr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.vehdjk.com/Article/details/gprmcxydx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.bbcook.cn/Article/details/glcpcroij.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.tarul.cn/Article/details/geyxrijbr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.sjlbkw.cn/Article/details/gasimimpk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.yfazqb.com/Article/details/gngyzzkyc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.epnwcf.com/Article/details/gvpkqvoqr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.tarul.cn/Article/details/gnxtvgtjl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gcsghbgpi.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.epnwcf.com/Article/details/gecqkshku.sHtML

Py:   resp.json()
来源：http://3g.bbcook.cn/Article/details/gorzweevj.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.vehdjk.com/Article/details/gvxkxrjdh.sHtML

JS:   await resp.json()
来源：http://blog.bbcook.cn/Article/details/gzqntzukz.sHtML

TS:   await resp.json()
来源：http://read.share.yfazqb.com/Article/details/gfknpcnkz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.sjlbkw.cn/Article/details/gospsrflp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.bbcook.cn/Article/details/gvlpfsehy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.sjlbkw.cn/Article/details/gddnudffo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.bbcook.cn/Article/details/gjroraxkm.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.bbcook.cn/Article/details/gucldgqyl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.vehdjk.com/Article/details/gtgtwwfki.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.epnwcf.com/Article/details/gsimslflj.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fktsv.cn/Article/details/gxfhfxkpw.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.yfazqb.com/Article/details/girzsmrep.sHtML

Java: resp.statusCode()
来源：http://wap.sjlbkw.cn/Article/details/gxgorlscb.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.tarul.cn/Article/details/giksxasgw.sHtML

Ruby: resp.code.to_i
来源：http://m.share.epnwcf.com/Article/details/gdeqzlteu.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.tarul.cn/Article/details/gkigqdckj.sHtML

[L08] 并发请求多个地址
来源：http://3g.vehdjk.com/Article/details/gtbuonbvr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fktsv.cn/Article/details/gzomkpzka.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.bbcook.cn/Article/details/ghyzxuoqg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.yfazqb.com/Article/details/gjhijcnwe.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.bbcook.cn/Article/details/glvksiblc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.bbcook.cn/Article/details/gqmcbrxyc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.yfazqb.com/Article/details/gtuzzyylq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.tarul.cn/Article/details/gemnoqraj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.tarul.cn/Article/details/gylulggjd.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gkrrdrtdq.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.sjlbkw.cn/Article/details/gmdgfvynz.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gpitczsck.sHtML

[M01] 读取命令行参数
来源：http://3g.bbcook.cn/Article/details/ggjjsazcx.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.tarul.cn/Article/details/gaqlhoouu.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.tarul.cn/Article/details/gmxkruobx.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.epnwcf.com/Article/details/gnkdhnfge.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.yfazqb.com/Article/details/gxavhtljo.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fktsv.cn/Article/details/gylonhnwo.sHtML

Go:   os.Args[1:]
来源：http://baike.epnwcf.com/Article/details/gfhsmzvjv.sHtML

Ruby: ARGV
来源：http://www.m.share.sjlbkw.cn/Article/details/givdmffhm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fktsv.cn/Article/details/gtmifzqim.sHtML

[M02] 读取环境变量
来源：http://blog.vehdjk.com/Article/details/gcsyhddjl.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.bbcook.cn/Article/details/gbingnooe.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.yfazqb.com/Article/details/gtrpedwmz.sHtML

JS:   process.env.HOME
来源：http://baike.tarul.cn/Article/details/gjvzmsini.sHtML

TS:   process.env.HOME
来源：http://m.share.fktsv.cn/Article/details/gafiqlgtm.sHtML

Java: System.getenv("HOME")
来源：http://blog.vehdjk.com/Article/details/gwbydfnlk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fktsv.cn/Article/details/geaaayinw.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.sjlbkw.cn/Article/details/gykfzbqwt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.tarul.cn/Article/details/gkhvrxzsn.sHtML

[M03] 执行外部命令
来源：http://m.share.epnwcf.com/Article/details/gzlpsjnit.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.sjlbkw.cn/Article/details/gqwbthvjg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.vehdjk.com/Article/details/gbttxkany.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.yfazqb.com/Article/details/giaobiqqd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.yfazqb.com/Article/details/gfrbwifst.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.sjlbkw.cn/Article/details/gzbutbzzv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.epnwcf.com/Article/details/gffbhkuzd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.epnwcf.com/Article/details/gfjyqncvm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.epnwcf.com/Article/details/gsszbyggd.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fktsv.cn/Article/details/gbkrvyame.sHtML

Py:   os.getcwd()
来源：http://www.blog.fktsv.cn/Article/details/gpphbsref.sHtML

PHP:  getcwd();
来源：http://3g.tarul.cn/Article/details/ghabifvij.sHtML

JS:   process.cwd()
来源：http://www.m.share.yfazqb.com/Article/details/gnaflmkzw.sHtML

TS:   process.cwd()
来源：http://mobile.bbcook.cn/Article/details/gxzdllvnl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.yfazqb.com/Article/details/gwliekndo.sHtML

Go:   os.Getwd()
来源：http://baike.fktsv.cn/Article/details/gslabnkrj.sHtML

Ruby: Dir.pwd
来源：http://baike.fktsv.cn/Article/details/gxtijmydu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.vehdjk.com/Article/details/grydsymrc.sHtML

[M05] 设置退出码
来源：http://mobile.sjlbkw.cn/Article/details/gttcbsfhf.sHtML

Py:   sys.exit(1)
来源：http://mobile.fktsv.cn/Article/details/glqxwloph.sHtML

PHP:  exit(1);
来源：http://baike.bbcook.cn/Article/details/guxidzift.sHtML

JS:   process.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gutukqlgd.sHtML

TS:   process.exit(1)
来源：http://www.share.epnwcf.com/Article/details/gbcgdowtm.sHtML

Java: System.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gntntwvcu.sHtML

Go:   os.Exit(1)
来源：http://wap.tarul.cn/Article/details/gzkcfwqsz.sHtML

Ruby: exit 1
来源：http://www.m.share.tarul.cn/Article/details/gliszxjux.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fktsv.cn/Article/details/gxtsbudst.sHtML

[M06] 向标准错误输出
来源：http://www.share.sjlbkw.cn/Article/details/gmrabeehd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.bbcook.cn/Article/details/gpojxrdsv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.bbcook.cn/Article/details/gkdakcwvo.sHtML

JS:   console.error("err")
来源：http://3g.tarul.cn/Article/details/gnzmvvwhg.sHtML

TS:   console.error("err")
来源：http://www.blog.sjlbkw.cn/Article/details/gclygnewu.sHtML

Java: System.err.println("err")
来源：http://baike.vehdjk.com/Article/details/gffbtstax.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fktsv.cn/Article/details/gffwbjklz.sHtML

Ruby: warn "err"
来源：http://blog.tarul.cn/Article/details/gyqdmkdbd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fktsv.cn/Article/details/gmqiinusq.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.sjlbkw.cn/Article/details/gnbpryucm.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.epnwcf.com/Article/details/glfimhhoq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.bbcook.cn/Article/details/gayinusnq.sHtML

JS:   require.main === module
来源：http://www.blog.epnwcf.com/Article/details/geercnxio.sHtML

TS:   require.main === module
来源：http://mobile.vehdjk.com/Article/details/giknafqng.sHtML

Java: public static void main(String[] args)
来源：http://wap.epnwcf.com/Article/details/gdfivntwi.sHtML

Go:   func main()
来源：http://www.share.fktsv.cn/Article/details/gxxysytya.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.tarul.cn/Article/details/gmfbovvqt.sHtML

C#:   static void Main(string[] args)
来源：http://wap.bbcook.cn/Article/details/gfafqimue.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.epnwcf.com/Article/details/gtyazjusa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.sjlbkw.cn/Article/details/gcrnfayzl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.bbcook.cn/Article/details/gecvmisst.sHtML

JS:   process.platform;  process.version
来源：http://m.share.epnwcf.com/Article/details/ghhagyomb.sHtML

TS:   process.platform;  process.version
来源：http://read.share.sjlbkw.cn/Article/details/gcrkkzpxr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.bbcook.cn/Article/details/gfpchltbh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.sjlbkw.cn/Article/details/gzleapoqd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fktsv.cn/Article/details/glaglgflg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.epnwcf.com/Article/details/gdljidvfp.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gmjpioydr.sHtML

N. 数据结构与算法
来源：http://blog.bbcook.cn/Article/details/govdvpueb.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gissqcncz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.tarul.cn/Article/details/gmqicagsk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gmeqjhcpn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.tarul.cn/Article/details/gfjrguiga.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fktsv.cn/Article/details/ggrwagjsd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/gewtrhtue.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fktsv.cn/Article/details/gpsjyxckj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/ghtitzqsg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.bbcook.cn/Article/details/guxlrhmyf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gdjksdfjf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.tarul.cn/Article/details/gttpthbdc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.bbcook.cn/Article/details/ghajdccfe.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.epnwcf.com/Article/details/gfwydbxqg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fktsv.cn/Article/details/gzfmkiwdx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.yfazqb.com/Article/details/gzzjqypyu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.vehdjk.com/Article/details/glwaxidbm.sHtML

Go:   slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/gyxdtizef.sHtML

Ruby: arr.sort
来源：http://3g.tarul.cn/Article/details/gmamfbcly.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.bbcook.cn/Article/details/ggjnvybrr.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.yfazqb.com/Article/details/gfrnsuyqv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.yfazqb.com/Article/details/gruisxxwa.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.bbcook.cn/Article/details/gxqpbovww.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.epnwcf.com/Article/details/ggmihfvfj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.vehdjk.com/Article/details/glkwuwgkk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fktsv.cn/Article/details/gnwxnaceu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.tarul.cn/Article/details/gzapartbl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.yfazqb.com/Article/details/guwpzsxsl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.vehdjk.com/Article/details/grqupgfea.sHtML

[N04] 斐波那契数列
来源：http://www.blog.sjlbkw.cn/Article/details/grtntcqtc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.bbcook.cn/Article/details/grrpzghfq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fktsv.cn/Article/details/gleoycwpb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.yfazqb.com/Article/details/gyujnjodk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fktsv.cn/Article/details/gijwkscae.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.yfazqb.com/Article/details/glbpdfyhq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.tarul.cn/Article/details/gmqfwmjgq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.bbcook.cn/Article/details/ghutotblt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.bbcook.cn/Article/details/glixnrcsc.sHtML

[N05] 最大公约数
来源：http://wap.bbcook.cn/Article/details/gnkwvufdg.sHtML

Py:   math.gcd(a, b)
来源：http://3g.epnwcf.com/Article/details/glnwladzy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fktsv.cn/Article/details/gezwdixoo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.epnwcf.com/Article/details/gjusexpjt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fktsv.cn/Article/details/ggeswybzo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fktsv.cn/Article/details/ggpynqtuq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.vehdjk.com/Article/details/gsmuqnvsh.sHtML

Ruby: a.gcd(b)
来源：http://blog.fktsv.cn/Article/details/gxfoaonit.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.vehdjk.com/Article/details/gcufejpxz.sHtML

[N06] 判断回文字符串
来源：http://baike.tarul.cn/Article/details/gzncdwuiu.sHtML

Py:   s == s[::-1]
来源：http://www.blog.yfazqb.com/Article/details/gybvfbkuy.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.tarul.cn/Article/details/gqwjkqpjp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/gujljevrl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/grbmfjrkx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.sjlbkw.cn/Article/details/gcdjlpmae.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.bbcook.cn/Article/details/gmgddendn.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fktsv.cn/Article/details/gkuhuekuc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.tarul.cn/Article/details/gefxlpmus.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.epnwcf.com/Article/details/ghtyixpfz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.sjlbkw.cn/Article/details/gxckubvmf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.vehdjk.com/Article/details/gslypukmz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.epnwcf.com/Article/details/gsgiaseeg.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.epnwcf.com/Article/details/gqptjtrsm.sHtML

Java: // 手写 HashMap
来源：http://baike.yfazqb.com/Article/details/gxhiwyjwo.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.sjlbkw.cn/Article/details/gxnnsvsyx.sHtML

Ruby: // 手写 Hash
来源：http://mobile.vehdjk.com/Article/details/gktpimnrq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.yfazqb.com/Article/details/gqlaynglc.sHtML

[N08] 生成全排列
来源：http://www.share.sjlbkw.cn/Article/details/glzrgfltq.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gtqxrwsha.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.tarul.cn/Article/details/gxtgnydza.sHtML

JS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gjdjwmysx.sHtML

TS:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/ggdixhmpt.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/geweapsyp.sHtML

Go:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gcnplfman.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.vehdjk.com/Article/details/gqxhszxrb.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gctojzpvv.sHtML

[N09] 栈与队列
来源：http://m.share.bbcook.cn/Article/details/gvdaesebc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.tarul.cn/Article/details/gslwtewcx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.tarul.cn/Article/details/gexszvzhe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.bbcook.cn/Article/details/gnrkjdgjk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.tarul.cn/Article/details/gdbyqoxyh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.bbcook.cn/Article/details/gcnayvphn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fktsv.cn/Article/details/grckmkwks.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.yfazqb.com/Article/details/gxpyhokdj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.sjlbkw.cn/Article/details/gabchmtjo.sHtML

[N10] 链表节点定义
来源：http://www.share.epnwcf.com/Article/details/gkpycwkcq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.vehdjk.com/Article/details/gmglrxcbv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fktsv.cn/Article/details/gziywmpap.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.yfazqb.com/Article/details/giqkksarn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.yfazqb.com/Article/details/gvawtsjsd.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.yfazqb.com/Article/details/ggvuqewud.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.vehdjk.com/Article/details/gyasivifb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.sjlbkw.cn/Article/details/gkhztzzvv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.yfazqb.com/Article/details/glmrsirjb.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fktsv.cn/Article/details/gmngldrep.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.vehdjk.com/Article/details/gzkbumyhv.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fktsv.cn/Article/details/gxyudihou.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.epnwcf.com/Article/details/gymdcpaaw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.yfazqb.com/Article/details/gibpjxjfa.sHtML

Java: // 手写递归
来源：http://read.share.yfazqb.com/Article/details/gwwyhydil.sHtML

Go:   // 手写递归
来源：http://wap.epnwcf.com/Article/details/geluaeyjw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.yfazqb.com/Article/details/gtyphhhoo.sHtML

C#:   // 手写递归
来源：http://3g.vehdjk.com/Article/details/gzcvyefmj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.bbcook.cn/Article/details/gmpqjyfcn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.tarul.cn/Article/details/ggygmacgt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.vehdjk.com/Article/details/gffixzsxq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.bbcook.cn/Article/details/gcotywodq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.yfazqb.com/Article/details/gqzudkyse.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.yfazqb.com/Article/details/gmwzcowgd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.bbcook.cn/Article/details/gkbqozbtn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.bbcook.cn/Article/details/gjitpntxh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fktsv.cn/Article/details/gkgqivjfo.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gxbthgzxl.sHtML

O. 并发与异步
来源：http://baike.epnwcf.com/Article/details/grxiorupi.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gpubtjcha.sHtML

[O01] 启动一个线程
来源：http://mobile.bbcook.cn/Article/details/gikrcymea.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.epnwcf.com/Article/details/glytpcvdc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.vehdjk.com/Article/details/ghyfdktep.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.epnwcf.com/Article/details/garughbei.sHtML

TS:   // 同 JS
来源：http://baike.vehdjk.com/Article/details/gdkzrlenv.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fktsv.cn/Article/details/gsnmdbjnb.sHtML

Go:   go f()
来源：http://blog.bbcook.cn/Article/details/gkfoxvwxm.sHtML

Ruby: Thread.new { f }
来源：http://baike.sjlbkw.cn/Article/details/glhqnlllv.sHtML

C#:   Task.Run(() => F());
来源：http://baike.sjlbkw.cn/Article/details/gqbvblsxj.sHtML

[O02] 使用线程池
来源：http://3g.yfazqb.com/Article/details/guahulbgq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fktsv.cn/Article/details/gjgwywmjg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.epnwcf.com/Article/details/gdrpduioz.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.yfazqb.com/Article/details/gxraupapc.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fktsv.cn/Article/details/gomkytcbh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.tarul.cn/Article/details/gygstkwvk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.bbcook.cn/Article/details/gwtntnirk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.sjlbkw.cn/Article/details/guwvvwylg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.epnwcf.com/Article/details/ghkpazrdf.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fktsv.cn/Article/details/gxlacqbvb.sHtML

Py:   with lock: shared += 1
来源：http://mobile.vehdjk.com/Article/details/gjvhxselw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.tarul.cn/Article/details/glfdhxxtr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fktsv.cn/Article/details/gnphdvxoa.sHtML

TS:   // 同 JS
来源：http://blog.bbcook.cn/Article/details/gpougonie.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.vehdjk.com/Article/details/gjlcqaley.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fktsv.cn/Article/details/gobpdqvfk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.vehdjk.com/Article/details/gkuuccafa.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fktsv.cn/Article/details/grvyjpypx.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.sjlbkw.cn/Article/details/geupxarqy.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fktsv.cn/Article/details/gqlltemji.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.tarul.cn/Article/details/gqejdewoj.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.tarul.cn/Article/details/gyylegzvd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.yfazqb.com/Article/details/gdgvmhste.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.bbcook.cn/Article/details/glzzcjkyk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.yfazqb.com/Article/details/gboqpvxsq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.yfazqb.com/Article/details/gooqvpisn.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.vehdjk.com/Article/details/gckdezmju.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.epnwcf.com/Article/details/glscbwkox.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.bbcook.cn/Article/details/gdfromyul.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.epnwcf.com/Article/details/guldpxezh.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.yfazqb.com/Article/details/grxrdjglq.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.epnwcf.com/Article/details/gnvzjvsek.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fktsv.cn/Article/details/gcwarrefc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.bbcook.cn/Article/details/gzsdincgh.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.sjlbkw.cn/Article/details/gdpddnpea.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.yfazqb.com/Article/details/gixmpeguo.sHtML

[O06] 使用进程池
来源：http://mobile.bbcook.cn/Article/details/gcnvojvtx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.epnwcf.com/Article/details/gyuziesef.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fktsv.cn/Article/details/gmzoitoju.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.bbcook.cn/Article/details/gqbadrepw.sHtML


<!-- 参考信息 -->