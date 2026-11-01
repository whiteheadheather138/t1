代发 wailian999

Go:   encoding/gob
来源：http://wap.bbcook.cn/Article/details/gqvdpqqpa.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.yfazqb.com/Article/details/gdnyfoytd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.vehdjk.com/Article/details/gatrldcuv.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gdzlazhec.sHtML

L. 网络请求
来源：http://read.share.tarul.cn/Article/details/gfgodqeve.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gbejutlqe.sHtML

[L01] 发送 GET 请求
来源：http://blog.tarul.cn/Article/details/gsivnbgqc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.vehdjk.com/Article/details/gmyaleqpt.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.yfazqb.com/Article/details/gpnpxgqvp.sHtML

JS:   await fetch(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnsniyiej.sHtML

TS:   await fetch(url)
来源：http://www.m.share.epnwcf.com/Article/details/gjkvecewl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.sjlbkw.cn/Article/details/gnzcchtch.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fktsv.cn/Article/details/gjqkrayib.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.vehdjk.com/Article/details/gyifbnyjq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.yfazqb.com/Article/details/gsxkozksn.sHtML

[L02] 发送 POST JSON
来源：http://mobile.bbcook.cn/Article/details/gogaynhna.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.tarul.cn/Article/details/gdfrgtgzz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.tarul.cn/Article/details/gqkyfxrbh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.bbcook.cn/Article/details/gxlocwxuh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.tarul.cn/Article/details/gqnprqrfa.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fktsv.cn/Article/details/gpzkslaae.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.yfazqb.com/Article/details/ggxcexmbu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.bbcook.cn/Article/details/ghqnfgcud.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.epnwcf.com/Article/details/gbutcojep.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.vehdjk.com/Article/details/gulylqsqr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.bbcook.cn/Article/details/gjyzjsffe.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.vehdjk.com/Article/details/gsgtaqffm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fktsv.cn/Article/details/gbtwccrkc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.yfazqb.com/Article/details/gykdxzcly.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.tarul.cn/Article/details/gmjnpnoky.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.sjlbkw.cn/Article/details/gfclyrocl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.epnwcf.com/Article/details/gwbdddvno.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.epnwcf.com/Article/details/glfunkdgn.sHtML

[L04] 设置超时
来源：http://blog.yfazqb.com/Article/details/gbrqjtaqe.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.vehdjk.com/Article/details/gvfmziduz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.vehdjk.com/Article/details/gsrsyxetq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.bbcook.cn/Article/details/gntlhfqap.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.vehdjk.com/Article/details/gnmdnzagx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.tarul.cn/Article/details/gxqnbzybv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.tarul.cn/Article/details/ggqpjlhua.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtqyplnle.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.yfazqb.com/Article/details/ggwrktjhv.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.tarul.cn/Article/details/gerzytxao.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.vehdjk.com/Article/details/gsryfxhxo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.bbcook.cn/Article/details/glubvasff.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.epnwcf.com/Article/details/gcvawpybh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.bbcook.cn/Article/details/gmgncpdcb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.vehdjk.com/Article/details/gzilwhndy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.yfazqb.com/Article/details/gccyfcwwz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.vehdjk.com/Article/details/ggjmgztea.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.yfazqb.com/Article/details/gzhwobkfq.sHtML

[L06] 解析响应为 JSON
来源：http://3g.tarul.cn/Article/details/govfcklko.sHtML

Py:   resp.json()
来源：http://read.share.fktsv.cn/Article/details/gmznfoumi.sHtML

PHP:  json_decode($body, true);
来源：http://wap.bbcook.cn/Article/details/gcsswbrek.sHtML

JS:   await resp.json()
来源：http://www.blog.sjlbkw.cn/Article/details/gffbzxlfp.sHtML

TS:   await resp.json()
来源：http://mobile.epnwcf.com/Article/details/ghnkvciqn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.yfazqb.com/Article/details/glpyraslv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.epnwcf.com/Article/details/gwcnbqdto.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.sjlbkw.cn/Article/details/gijgvsgkp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.yfazqb.com/Article/details/gnjomdbpa.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.tarul.cn/Article/details/gyrgyczay.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fktsv.cn/Article/details/gzewewwox.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.vehdjk.com/Article/details/gpxprbjkj.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.vehdjk.com/Article/details/gszcrboru.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.vehdjk.com/Article/details/guvptvjcf.sHtML

Java: resp.statusCode()
来源：http://blog.sjlbkw.cn/Article/details/ggeargnza.sHtML

Go:   resp.StatusCode
来源：http://www.share.fktsv.cn/Article/details/gmxocxole.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.yfazqb.com/Article/details/gqzrssngu.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.epnwcf.com/Article/details/ggqcdppfr.sHtML

[L08] 并发请求多个地址
来源：http://baike.bbcook.cn/Article/details/grzhukgjg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.yfazqb.com/Article/details/grrherrzm.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.yfazqb.com/Article/details/gqoxsezan.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.yfazqb.com/Article/details/gezyepwlv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/ghoqlkcnn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.tarul.cn/Article/details/gatjgtsqu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.sjlbkw.cn/Article/details/gvlqihgpb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.epnwcf.com/Article/details/gnnuslhww.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.bbcook.cn/Article/details/gruspdcna.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/giswlhxen.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.epnwcf.com/Article/details/gjrpyqvvy.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gyezhhuyg.sHtML

[M01] 读取命令行参数
来源：http://3g.sjlbkw.cn/Article/details/gebtdjypi.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fktsv.cn/Article/details/gyplpvhao.sHtML

PHP:  $argv;  $argc;
来源：http://wap.sjlbkw.cn/Article/details/giogajnzk.sHtML

JS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/gdxeycchc.sHtML

TS:   process.argv.slice(2)
来源：http://wap.yfazqb.com/Article/details/giixlvjnf.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.bbcook.cn/Article/details/gjjphwxvb.sHtML

Go:   os.Args[1:]
来源：http://baike.tarul.cn/Article/details/gokeclqoy.sHtML

Ruby: ARGV
来源：http://blog.yfazqb.com/Article/details/ghzpbxssr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.tarul.cn/Article/details/gwjzhlwyc.sHtML

[M02] 读取环境变量
来源：http://www.m.share.bbcook.cn/Article/details/gbebhnepn.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.tarul.cn/Article/details/guracrhmo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.yfazqb.com/Article/details/gevdsglmy.sHtML

JS:   process.env.HOME
来源：http://baike.tarul.cn/Article/details/gfqkuxccm.sHtML

TS:   process.env.HOME
来源：http://3g.yfazqb.com/Article/details/gscknvnqm.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.bbcook.cn/Article/details/giomuegff.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gvioixups.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.epnwcf.com/Article/details/gmbqzefbe.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gfssnkldj.sHtML

[M03] 执行外部命令
来源：http://www.share.epnwcf.com/Article/details/gkegxjehd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fktsv.cn/Article/details/ggnqxfxla.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.tarul.cn/Article/details/gqvosemit.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fktsv.cn/Article/details/gzkasxpmt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.tarul.cn/Article/details/gfkprunhi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.bbcook.cn/Article/details/gvncxxftn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.yfazqb.com/Article/details/gywmzaqld.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.sjlbkw.cn/Article/details/gbhnlwoee.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.vehdjk.com/Article/details/ghbyaruwn.sHtML

[M04] 获取当前工作目录
来源：http://read.share.yfazqb.com/Article/details/gtfoczvqa.sHtML

Py:   os.getcwd()
来源：http://baike.tarul.cn/Article/details/gjtimbvhg.sHtML

PHP:  getcwd();
来源：http://3g.bbcook.cn/Article/details/gtvbqbebv.sHtML

JS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/gwjzhalgq.sHtML

TS:   process.cwd()
来源：http://www.m.share.fktsv.cn/Article/details/gqujiauto.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fktsv.cn/Article/details/gakbdgwra.sHtML

Go:   os.Getwd()
来源：http://www.m.share.epnwcf.com/Article/details/gkuncjigb.sHtML

Ruby: Dir.pwd
来源：http://www.share.epnwcf.com/Article/details/gzonwxzkt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fktsv.cn/Article/details/gdqatfsyb.sHtML

[M05] 设置退出码
来源：http://m.share.tarul.cn/Article/details/glpfrgchj.sHtML

Py:   sys.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gamupjkth.sHtML

PHP:  exit(1);
来源：http://www.m.share.yfazqb.com/Article/details/grcehtync.sHtML

JS:   process.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gmwhwzvnd.sHtML

TS:   process.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gsixqipuc.sHtML

Java: System.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gkxcnixbl.sHtML

Go:   os.Exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gxgjztobw.sHtML

Ruby: exit 1
来源：http://read.share.vehdjk.com/Article/details/ghlskbnss.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.tarul.cn/Article/details/gyzdoknyk.sHtML

[M06] 向标准错误输出
来源：http://m.share.tarul.cn/Article/details/gxicntvin.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.tarul.cn/Article/details/gitvfiebu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.vehdjk.com/Article/details/gmxzwhhhi.sHtML

JS:   console.error("err")
来源：http://www.m.share.epnwcf.com/Article/details/gpbgzwyhv.sHtML

TS:   console.error("err")
来源：http://blog.fktsv.cn/Article/details/gkppeemil.sHtML

Java: System.err.println("err")
来源：http://baike.fktsv.cn/Article/details/gywbnmdyj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.sjlbkw.cn/Article/details/ghrkzayqo.sHtML

Ruby: warn "err"
来源：http://www.blog.vehdjk.com/Article/details/gtpvcednk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.tarul.cn/Article/details/gfgirxfey.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fktsv.cn/Article/details/gtlrvmmmf.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.vehdjk.com/Article/details/gvznhawuu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gebrtxrvj.sHtML

JS:   require.main === module
来源：http://m.share.fktsv.cn/Article/details/ggumuvirn.sHtML

TS:   require.main === module
来源：http://baike.tarul.cn/Article/details/gyghntzbs.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fktsv.cn/Article/details/gnbtwelta.sHtML

Go:   func main()
来源：http://www.m.share.yfazqb.com/Article/details/glgktxyql.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.vehdjk.com/Article/details/glznszqiz.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.epnwcf.com/Article/details/gqdkpgjxc.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.yfazqb.com/Article/details/gupkwbzxx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.bbcook.cn/Article/details/gxsqpxjbj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.yfazqb.com/Article/details/gjvsafpee.sHtML

JS:   process.platform;  process.version
来源：http://blog.tarul.cn/Article/details/gqzpvuebk.sHtML

TS:   process.platform;  process.version
来源：http://read.share.bbcook.cn/Article/details/grolmihyo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.bbcook.cn/Article/details/gqsugiaef.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.vehdjk.com/Article/details/ginctznon.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fktsv.cn/Article/details/glcvinwgy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.sjlbkw.cn/Article/details/gvnwxhmxi.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gbswcbssn.sHtML

N. 数据结构与算法
来源：http://m.share.epnwcf.com/Article/details/gsgagghaq.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gyyekksxe.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.vehdjk.com/Article/details/gmphjlluq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gfgkryoop.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.epnwcf.com/Article/details/gkcquggkb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.tarul.cn/Article/details/gxkgatdzb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.vehdjk.com/Article/details/gjrcshccb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gxzgewqnn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.tarul.cn/Article/details/gjfuhzdod.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.epnwcf.com/Article/details/gposvjxnx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gkqkoidwl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.yfazqb.com/Article/details/gqujzsqmg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.vehdjk.com/Article/details/grgiutaar.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.bbcook.cn/Article/details/gbbdvpxlr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/gaxrleduh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fktsv.cn/Article/details/gebbefkml.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.tarul.cn/Article/details/gkgocmtvv.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fktsv.cn/Article/details/gbztldlfk.sHtML

Ruby: arr.sort
来源：http://www.blog.bbcook.cn/Article/details/gloxiestc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fktsv.cn/Article/details/gicgmigpp.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.vehdjk.com/Article/details/gnpovrtdp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.tarul.cn/Article/details/gikgsuxeu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.yfazqb.com/Article/details/geflpiqkf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.epnwcf.com/Article/details/grmqlxwvd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.yfazqb.com/Article/details/gdbcwvjnl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.yfazqb.com/Article/details/gocljhliv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.bbcook.cn/Article/details/gzkcnzgah.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.tarul.cn/Article/details/gqevtihxi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.tarul.cn/Article/details/gysrrqwsg.sHtML

[N04] 斐波那契数列
来源：http://www.share.bbcook.cn/Article/details/gprduaajp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fktsv.cn/Article/details/gkreywjne.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fktsv.cn/Article/details/getacqcha.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/gbibejfhw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/grghyqxvz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.vehdjk.com/Article/details/gkmckmskj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.sjlbkw.cn/Article/details/gclgcgcjx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.tarul.cn/Article/details/gbsglnhyi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/gefrcaidw.sHtML

[N05] 最大公约数
来源：http://www.blog.yfazqb.com/Article/details/gviowbply.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.bbcook.cn/Article/details/gyblgwpjl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fktsv.cn/Article/details/gyyilufyg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.vehdjk.com/Article/details/gimbjjeyn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.epnwcf.com/Article/details/gyigfjvfe.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.sjlbkw.cn/Article/details/gurbglnsn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fktsv.cn/Article/details/gxenjwmfv.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fktsv.cn/Article/details/gejubtaff.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.tarul.cn/Article/details/ghguclaik.sHtML

[N06] 判断回文字符串
来源：http://blog.fktsv.cn/Article/details/gmkwduzxb.sHtML

Py:   s == s[::-1]
来源：http://3g.epnwcf.com/Article/details/gxbczgcxo.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fktsv.cn/Article/details/grugpefgw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gmnffipkl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.vehdjk.com/Article/details/ghbstuepy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.tarul.cn/Article/details/gxddraalq.sHtML

Go:   // 双指针从两端比较
来源：http://baike.epnwcf.com/Article/details/gzbqpjvos.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.yfazqb.com/Article/details/gikhionky.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.yfazqb.com/Article/details/guavpavad.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fktsv.cn/Article/details/gqryaupsn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.epnwcf.com/Article/details/gcezdcvrq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fktsv.cn/Article/details/gisyfmozs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.bbcook.cn/Article/details/gojwkginw.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.epnwcf.com/Article/details/ghpqocjrf.sHtML

Java: // 手写 HashMap
来源：http://m.share.vehdjk.com/Article/details/gdzqhfyco.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.bbcook.cn/Article/details/gmyxfyrrw.sHtML

Ruby: // 手写 Hash
来源：http://mobile.vehdjk.com/Article/details/gcqjscozg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.yfazqb.com/Article/details/giqacuibu.sHtML

[N08] 生成全排列
来源：http://read.share.sjlbkw.cn/Article/details/gakceribw.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.yfazqb.com/Article/details/gzaiunevu.sHtML

PHP:  // 手写递归交换
来源：http://www.share.sjlbkw.cn/Article/details/gyugbjlas.sHtML

JS:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gwandhppt.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gbwkpnnrh.sHtML

Java: // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/glurzapht.sHtML

Go:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gpaxzkgrp.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.sjlbkw.cn/Article/details/grysejpyi.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbvcbodg.sHtML

[N09] 栈与队列
来源：http://wap.fktsv.cn/Article/details/gjkpwgdvu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.tarul.cn/Article/details/gypglqmjs.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/gskdllhzs.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.vehdjk.com/Article/details/gbzgfpxax.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.vehdjk.com/Article/details/girymrgwi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.yfazqb.com/Article/details/gxzynzfmp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fktsv.cn/Article/details/gbphtzstv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.bbcook.cn/Article/details/grxrqfuiz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.vehdjk.com/Article/details/ghqpxkqrg.sHtML

[N10] 链表节点定义
来源：http://m.share.epnwcf.com/Article/details/gdkyvzoxn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.epnwcf.com/Article/details/gzoirnmxs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.yfazqb.com/Article/details/gerlktrwz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fktsv.cn/Article/details/gsfmbjoku.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.vehdjk.com/Article/details/gmnlbwpmt.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.yfazqb.com/Article/details/gttwzuswn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.epnwcf.com/Article/details/gtutldjah.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.epnwcf.com/Article/details/gqxysxgpd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.sjlbkw.cn/Article/details/gcldorzge.sHtML

[N11] 二叉树中序遍历
来源：http://baike.tarul.cn/Article/details/gipvsslpr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fktsv.cn/Article/details/gizytcgbw.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fktsv.cn/Article/details/gusisksnz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.sjlbkw.cn/Article/details/goqsdgesa.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.epnwcf.com/Article/details/gmvefulce.sHtML

Java: // 手写递归
来源：http://baike.tarul.cn/Article/details/gtbjxzbpc.sHtML

Go:   // 手写递归
来源：http://wap.epnwcf.com/Article/details/gmfasefmi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.vehdjk.com/Article/details/gjhvuaetl.sHtML

C#:   // 手写递归
来源：http://wap.epnwcf.com/Article/details/grrpxkynh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fktsv.cn/Article/details/gesknyhis.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fktsv.cn/Article/details/gplaevglt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.sjlbkw.cn/Article/details/gomvbrcxc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.yfazqb.com/Article/details/gnuzhkofb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.vehdjk.com/Article/details/gahpjainm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.bbcook.cn/Article/details/gkxvqonrf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.bbcook.cn/Article/details/geclyijoj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.tarul.cn/Article/details/guprrtaxn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.tarul.cn/Article/details/gtpwpgxhf.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gsjbqfxqr.sHtML

O. 并发与异步
来源：http://mobile.sjlbkw.cn/Article/details/gljtkvoxx.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gxswwqpxe.sHtML

[O01] 启动一个线程
来源：http://blog.fktsv.cn/Article/details/garsyhilj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fktsv.cn/Article/details/gbhwovxkc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcueocaz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.sjlbkw.cn/Article/details/gpmjdjhjn.sHtML

TS:   // 同 JS
来源：http://read.share.vehdjk.com/Article/details/gvefwmrxs.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fktsv.cn/Article/details/gputzgvnz.sHtML

Go:   go f()
来源：http://baike.tarul.cn/Article/details/gazmbftnc.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.yfazqb.com/Article/details/gqnziqvcd.sHtML

C#:   Task.Run(() => F());
来源：http://blog.tarul.cn/Article/details/gqygjqiyy.sHtML

[O02] 使用线程池
来源：http://mobile.sjlbkw.cn/Article/details/gagecckzw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.epnwcf.com/Article/details/gtndfdlid.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.sjlbkw.cn/Article/details/gsvzbwslo.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.tarul.cn/Article/details/gwcdtgmsr.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.bbcook.cn/Article/details/giobtzjgb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.bbcook.cn/Article/details/gnczmiffl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.epnwcf.com/Article/details/gfxnjxuct.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fktsv.cn/Article/details/gsfkocxzw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fktsv.cn/Article/details/goulwiqcz.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.sjlbkw.cn/Article/details/geqxnjqur.sHtML

Py:   with lock: shared += 1
来源：http://read.share.bbcook.cn/Article/details/gwqclkunh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.yfazqb.com/Article/details/ggulnesif.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.yfazqb.com/Article/details/gaqagnulc.sHtML

TS:   // 同 JS
来源：http://wap.tarul.cn/Article/details/gincdgnxs.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.epnwcf.com/Article/details/gatqjakat.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.sjlbkw.cn/Article/details/gogcgtfet.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.yfazqb.com/Article/details/gzbvrndtw.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.epnwcf.com/Article/details/gvmkhkjby.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.tarul.cn/Article/details/gyezqwatx.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.vehdjk.com/Article/details/gweqgrynh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.bbcook.cn/Article/details/ghvkbfnit.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.sjlbkw.cn/Article/details/gtrtamehe.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fktsv.cn/Article/details/gxyvihxgf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.epnwcf.com/Article/details/goomjgsqb.sHtML


<!-- 参考信息 -->