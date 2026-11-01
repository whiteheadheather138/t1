代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.tarul.cn/Article/details/gpulnadke.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.vehdjk.com/Article/details/gbrrmlffh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.yfazqb.com/Article/details/gqxfmmyos.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.sjlbkw.cn/Article/details/gnlmqszkz.sHtML

Go:   encoding/gob
来源：http://www.share.tarul.cn/Article/details/gcjipnorb.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fktsv.cn/Article/details/glxldcpmc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.epnwcf.com/Article/details/gpfgoeuhm.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ghhdvkvoo.sHtML

L. 网络请求
来源：http://www.share.fktsv.cn/Article/details/gcplmqegs.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gobkzrwod.sHtML

[L01] 发送 GET 请求
来源：http://wap.tarul.cn/Article/details/gmxosnuxd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.yfazqb.com/Article/details/gwpnnwzts.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.yfazqb.com/Article/details/gdcbmvgvg.sHtML

JS:   await fetch(url)
来源：http://read.share.bbcook.cn/Article/details/gfdczfmcm.sHtML

TS:   await fetch(url)
来源：http://m.share.bbcook.cn/Article/details/greeestvt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.bbcook.cn/Article/details/gviewplse.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.bbcook.cn/Article/details/gsklzndcx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.epnwcf.com/Article/details/gqoceqqkg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.bbcook.cn/Article/details/glvfzywlw.sHtML

[L02] 发送 POST JSON
来源：http://baike.sjlbkw.cn/Article/details/grpcnyino.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.sjlbkw.cn/Article/details/ghsgmycdo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.tarul.cn/Article/details/gucouybhe.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fktsv.cn/Article/details/gepjbdrbw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.tarul.cn/Article/details/gbdumczhk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.bbcook.cn/Article/details/gaerpehhy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.tarul.cn/Article/details/gllscsopf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.bbcook.cn/Article/details/ggihdnaln.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.bbcook.cn/Article/details/gqstetywl.sHtML

[L03] 设置自定义请求头
来源：http://mobile.epnwcf.com/Article/details/ggyneqgrq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.epnwcf.com/Article/details/gexmhngtk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.bbcook.cn/Article/details/gybqlccdg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.tarul.cn/Article/details/gsmhkfgyk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.vehdjk.com/Article/details/gusfsjxyw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.yfazqb.com/Article/details/gwqksyzau.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.bbcook.cn/Article/details/gfkzebcks.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fktsv.cn/Article/details/gdukpqfnx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.sjlbkw.cn/Article/details/gdzrlirqv.sHtML

[L04] 设置超时
来源：http://www.share.tarul.cn/Article/details/gnqlneqks.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.vehdjk.com/Article/details/gcckkbkxo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.bbcook.cn/Article/details/gvtlfwxec.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fktsv.cn/Article/details/gnykilori.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.epnwcf.com/Article/details/gffoqizct.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.vehdjk.com/Article/details/grqmdcsok.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.epnwcf.com/Article/details/glxyxwuzt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.sjlbkw.cn/Article/details/gysythtar.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.bbcook.cn/Article/details/gwytisnsz.sHtML

[L05] 上传文件（multipart）
来源：http://3g.vehdjk.com/Article/details/gmkueojfb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.vehdjk.com/Article/details/ggxakpbfj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.epnwcf.com/Article/details/glxtlubpo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.vehdjk.com/Article/details/gugzocsfy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.bbcook.cn/Article/details/gkkbmzbae.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.yfazqb.com/Article/details/gwwnhodyf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fktsv.cn/Article/details/gsvyhnjvd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.vehdjk.com/Article/details/ggnnkfbnn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fktsv.cn/Article/details/gypbuislt.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.tarul.cn/Article/details/gvqwmiagk.sHtML

Py:   resp.json()
来源：http://3g.yfazqb.com/Article/details/grvqcujar.sHtML

PHP:  json_decode($body, true);
来源：http://blog.vehdjk.com/Article/details/geszuilly.sHtML

JS:   await resp.json()
来源：http://blog.yfazqb.com/Article/details/gpodjorhr.sHtML

TS:   await resp.json()
来源：http://www.share.bbcook.cn/Article/details/gcgakpzlo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/gzugqumdg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.tarul.cn/Article/details/ghevhajxz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.epnwcf.com/Article/details/gwpvljmmh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.yfazqb.com/Article/details/gjpsdjpdr.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.sjlbkw.cn/Article/details/gpyrdsoeh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.sjlbkw.cn/Article/details/gdlohrpam.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fktsv.cn/Article/details/gkggkpqxv.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.tarul.cn/Article/details/gjumuddkc.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.epnwcf.com/Article/details/gajakjncq.sHtML

Java: resp.statusCode()
来源：http://baike.vehdjk.com/Article/details/gdxelrykl.sHtML

Go:   resp.StatusCode
来源：http://mobile.sjlbkw.cn/Article/details/ghukuznfm.sHtML

Ruby: resp.code.to_i
来源：http://3g.bbcook.cn/Article/details/gpjtwllcu.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.vehdjk.com/Article/details/gbrimddxs.sHtML

[L08] 并发请求多个地址
来源：http://read.share.yfazqb.com/Article/details/ggnvwvmdr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.yfazqb.com/Article/details/gdyawnszu.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.vehdjk.com/Article/details/gvwxthonj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.bbcook.cn/Article/details/gadcywbbl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.yfazqb.com/Article/details/gnwkixyxh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.bbcook.cn/Article/details/gxmokocem.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.sjlbkw.cn/Article/details/gnatzohfb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fktsv.cn/Article/details/gelcihiul.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fktsv.cn/Article/details/gtbfbgwqr.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gmmutrfbg.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.sjlbkw.cn/Article/details/gnlogjuxc.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gwdncxlsk.sHtML

[M01] 读取命令行参数
来源：http://www.share.fktsv.cn/Article/details/gufasedgs.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/guevahrid.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.bbcook.cn/Article/details/gxscmbxhs.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.vehdjk.com/Article/details/gushdmita.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.tarul.cn/Article/details/gjmpjxjzv.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.vehdjk.com/Article/details/gclrrvxgx.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fktsv.cn/Article/details/godxphdbb.sHtML

Ruby: ARGV
来源：http://m.share.sjlbkw.cn/Article/details/gnmdhvwck.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.epnwcf.com/Article/details/garuhhllw.sHtML

[M02] 读取环境变量
来源：http://mobile.yfazqb.com/Article/details/gcbgwccgu.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.vehdjk.com/Article/details/gcxlcetyb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.bbcook.cn/Article/details/gouknhdkk.sHtML

JS:   process.env.HOME
来源：http://wap.fktsv.cn/Article/details/glvzijldk.sHtML

TS:   process.env.HOME
来源：http://m.share.bbcook.cn/Article/details/gfxobxezc.sHtML

Java: System.getenv("HOME")
来源：http://3g.bbcook.cn/Article/details/gzxjdqihl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.bbcook.cn/Article/details/geemfgyyn.sHtML

Ruby: ENV["HOME"]
来源：http://baike.epnwcf.com/Article/details/gdpcikvvl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gwodhasnu.sHtML

[M03] 执行外部命令
来源：http://mobile.sjlbkw.cn/Article/details/gnbbtrrzy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.yfazqb.com/Article/details/gvixmeesu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fktsv.cn/Article/details/gccykdidt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.bbcook.cn/Article/details/gviqlwkrd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.tarul.cn/Article/details/gwsdbjrgj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.bbcook.cn/Article/details/gaobogphr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.sjlbkw.cn/Article/details/gtusgwhct.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fktsv.cn/Article/details/gvlsdsojf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.bbcook.cn/Article/details/gustiwkvk.sHtML

[M04] 获取当前工作目录
来源：http://m.share.epnwcf.com/Article/details/gvgaymxma.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fktsv.cn/Article/details/gqzrwejoo.sHtML

PHP:  getcwd();
来源：http://www.share.fktsv.cn/Article/details/gkskwhpmu.sHtML

JS:   process.cwd()
来源：http://3g.vehdjk.com/Article/details/gvhiddacg.sHtML

TS:   process.cwd()
来源：http://blog.yfazqb.com/Article/details/gqrojgyik.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.vehdjk.com/Article/details/ggsvjbris.sHtML

Go:   os.Getwd()
来源：http://blog.bbcook.cn/Article/details/gjeckodxi.sHtML

Ruby: Dir.pwd
来源：http://m.share.bbcook.cn/Article/details/gemdoyumy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.vehdjk.com/Article/details/gbipogugg.sHtML

[M05] 设置退出码
来源：http://www.blog.yfazqb.com/Article/details/gstozydmv.sHtML

Py:   sys.exit(1)
来源：http://m.share.epnwcf.com/Article/details/ggushzmnb.sHtML

PHP:  exit(1);
来源：http://www.share.fktsv.cn/Article/details/grtfojnuy.sHtML

JS:   process.exit(1)
来源：http://mobile.vehdjk.com/Article/details/ghuaubhuh.sHtML

TS:   process.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gmzeixhby.sHtML

Java: System.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gxihffglg.sHtML

Go:   os.Exit(1)
来源：http://read.share.fktsv.cn/Article/details/gscphmcdh.sHtML

Ruby: exit 1
来源：http://www.share.yfazqb.com/Article/details/gjhigjevq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.yfazqb.com/Article/details/gvcqsajnl.sHtML

[M06] 向标准错误输出
来源：http://www.share.fktsv.cn/Article/details/gmbcrvvjr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.tarul.cn/Article/details/gyzuiqmln.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.sjlbkw.cn/Article/details/ghkrgrqox.sHtML

JS:   console.error("err")
来源：http://m.share.epnwcf.com/Article/details/gwwalvkcg.sHtML

TS:   console.error("err")
来源：http://www.share.epnwcf.com/Article/details/gfeokiyvl.sHtML

Java: System.err.println("err")
来源：http://baike.tarul.cn/Article/details/gcxfszepd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.vehdjk.com/Article/details/gerthsgjg.sHtML

Ruby: warn "err"
来源：http://read.share.fktsv.cn/Article/details/gfvtnsriy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.vehdjk.com/Article/details/gkvmshkey.sHtML

[M07] 判断是否为主入口
来源：http://mobile.bbcook.cn/Article/details/gibkhmrnn.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjrvnnzf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.bbcook.cn/Article/details/geerroyrj.sHtML

JS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/gmyifyzcb.sHtML

TS:   require.main === module
来源：http://blog.yfazqb.com/Article/details/ghddbpwhj.sHtML

Java: public static void main(String[] args)
来源：http://3g.fktsv.cn/Article/details/glrguiagz.sHtML

Go:   func main()
来源：http://www.m.share.vehdjk.com/Article/details/gchbmthjv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.epnwcf.com/Article/details/gpecguask.sHtML

C#:   static void Main(string[] args)
来源：http://wap.tarul.cn/Article/details/gnqokuxjb.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.bbcook.cn/Article/details/gjvdwjgtt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.vehdjk.com/Article/details/ghfuqolmx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.yfazqb.com/Article/details/gnwqdhjdc.sHtML

JS:   process.platform;  process.version
来源：http://www.share.sjlbkw.cn/Article/details/grfmejggb.sHtML

TS:   process.platform;  process.version
来源：http://wap.yfazqb.com/Article/details/glzzjfvkc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjoikszqu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.sjlbkw.cn/Article/details/gxarcijlt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fktsv.cn/Article/details/gzdikpska.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.vehdjk.com/Article/details/gdlnyrtoh.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gkgsayrqi.sHtML

N. 数据结构与算法
来源：http://wap.epnwcf.com/Article/details/gtojtagac.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gtevcytgw.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.yfazqb.com/Article/details/gtosfcdbm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gqbggelgg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.sjlbkw.cn/Article/details/gdwyfinux.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.sjlbkw.cn/Article/details/goutyeovk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.yfazqb.com/Article/details/gbqmdfcne.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/glqtozyqi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.epnwcf.com/Article/details/grsrpgbnt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.sjlbkw.cn/Article/details/gvhovbqfx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gofbohbip.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.vehdjk.com/Article/details/giwgvbsra.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.epnwcf.com/Article/details/gjuspoigy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.sjlbkw.cn/Article/details/gknqjexjd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fktsv.cn/Article/details/gcsiftcly.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/gjpagqoyh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.yfazqb.com/Article/details/gkintrepi.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.tarul.cn/Article/details/gdabkomcm.sHtML

Ruby: arr.sort
来源：http://m.share.vehdjk.com/Article/details/gignxplut.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.epnwcf.com/Article/details/ggnwyilqu.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.vehdjk.com/Article/details/grnydellw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.tarul.cn/Article/details/gwstgoscc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwpddhkx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.bbcook.cn/Article/details/givxbwtkm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fktsv.cn/Article/details/gllybtgbs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.epnwcf.com/Article/details/gzajiecor.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.sjlbkw.cn/Article/details/gtixumsxb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.bbcook.cn/Article/details/gbyemzpte.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.yfazqb.com/Article/details/gsloermqa.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fktsv.cn/Article/details/gwbaskgrm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.vehdjk.com/Article/details/gyusgcypw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/gtybdjhtr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.vehdjk.com/Article/details/gifnwnzfj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.tarul.cn/Article/details/ghqqoepms.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fktsv.cn/Article/details/gepvcbmte.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.tarul.cn/Article/details/gzkfjxgqx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.sjlbkw.cn/Article/details/gvbkfqitr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/gkxdptaxt.sHtML

[N05] 最大公约数
来源：http://read.share.fktsv.cn/Article/details/gdlgfgnoo.sHtML

Py:   math.gcd(a, b)
来源：http://3g.sjlbkw.cn/Article/details/ggldxirsb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.vehdjk.com/Article/details/gpytavrve.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.yfazqb.com/Article/details/ghxqznpdx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.epnwcf.com/Article/details/ghbyiqatk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.bbcook.cn/Article/details/gjszsahpj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.sjlbkw.cn/Article/details/gkkkgkzrq.sHtML

Ruby: a.gcd(b)
来源：http://read.share.vehdjk.com/Article/details/grudziyxo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.yfazqb.com/Article/details/gxmxtwmhn.sHtML

[N06] 判断回文字符串
来源：http://m.share.fktsv.cn/Article/details/gmfkqdzml.sHtML

Py:   s == s[::-1]
来源：http://wap.vehdjk.com/Article/details/geguoxlhn.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.epnwcf.com/Article/details/gqqazglag.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/ganosdxwq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.tarul.cn/Article/details/gtuountvp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fktsv.cn/Article/details/gwjiejuxv.sHtML

Go:   // 双指针从两端比较
来源：http://baike.epnwcf.com/Article/details/gkofjcggb.sHtML

Ruby: s == s.reverse
来源：http://blog.vehdjk.com/Article/details/gvamixtno.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.tarul.cn/Article/details/ghnhjbxqy.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fktsv.cn/Article/details/gvvazffdr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.epnwcf.com/Article/details/grxcehoig.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.bbcook.cn/Article/details/gapxtqkkd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.vehdjk.com/Article/details/gnmijzqik.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.epnwcf.com/Article/details/gvlhgtzby.sHtML

Java: // 手写 HashMap
来源：http://baike.bbcook.cn/Article/details/grhkyhqgm.sHtML

Go:   // 手写 map[int]int
来源：http://3g.vehdjk.com/Article/details/gyxwifzlr.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.sjlbkw.cn/Article/details/gyqspauzp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.epnwcf.com/Article/details/gganbdfru.sHtML

[N08] 生成全排列
来源：http://wap.yfazqb.com/Article/details/gwptuyyls.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.bbcook.cn/Article/details/gcgoxzzme.sHtML

PHP:  // 手写递归交换
来源：http://baike.tarul.cn/Article/details/gidabuylc.sHtML

JS:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gtkwvzylz.sHtML

TS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gylsguxhf.sHtML

Java: // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gnfjhzwup.sHtML

Go:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gtotjrrih.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.tarul.cn/Article/details/gahrieddr.sHtML

C#:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/geepqtyyz.sHtML

[N09] 栈与队列
来源：http://www.blog.vehdjk.com/Article/details/gibnrhrry.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.epnwcf.com/Article/details/gfxbnkiyn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fktsv.cn/Article/details/gvgttuxfr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gurfocplq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.yfazqb.com/Article/details/gihfqoiqf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.bbcook.cn/Article/details/gbogiuxqv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.bbcook.cn/Article/details/gvbedzetp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.yfazqb.com/Article/details/gsotkpyfp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.yfazqb.com/Article/details/gdmzyhwzj.sHtML

[N10] 链表节点定义
来源：http://www.m.share.vehdjk.com/Article/details/gtbnypqqg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.vehdjk.com/Article/details/gbrstgvpq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.epnwcf.com/Article/details/gbukpnfnk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.vehdjk.com/Article/details/gydgosqcz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.yfazqb.com/Article/details/gbmrduqom.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fktsv.cn/Article/details/glutclezf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.tarul.cn/Article/details/glmqkwsht.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.yfazqb.com/Article/details/gxxxapavf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fktsv.cn/Article/details/gimgbgqcx.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.bbcook.cn/Article/details/gsftpzzcd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.sjlbkw.cn/Article/details/gakcmpumx.sHtML

PHP:  // 手写递归函数
来源：http://read.share.bbcook.cn/Article/details/gwlyihpxl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/gruwobvlj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.epnwcf.com/Article/details/gffrkchls.sHtML

Java: // 手写递归
来源：http://wap.bbcook.cn/Article/details/gxvgbqpvj.sHtML

Go:   // 手写递归
来源：http://baike.tarul.cn/Article/details/gspfzvbxw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.bbcook.cn/Article/details/gxfjafzdk.sHtML

C#:   // 手写递归
来源：http://www.m.share.bbcook.cn/Article/details/giutgkmcd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.sjlbkw.cn/Article/details/gqqyvvcfh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.tarul.cn/Article/details/ggrpjqoon.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.vehdjk.com/Article/details/gibapgslq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.epnwcf.com/Article/details/ggabhxokv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.vehdjk.com/Article/details/geqrjyjeo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.bbcook.cn/Article/details/gvkjodbkn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.yfazqb.com/Article/details/gzrojfoqk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.epnwcf.com/Article/details/gsjwovlfq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.bbcook.cn/Article/details/gdlisawpa.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/goqqbjddw.sHtML

O. 并发与异步
来源：http://read.share.sjlbkw.cn/Article/details/gsbexpuhn.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/geyapcsad.sHtML

[O01] 启动一个线程
来源：http://www.blog.yfazqb.com/Article/details/gejpylkzt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.epnwcf.com/Article/details/gkedweefz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.bbcook.cn/Article/details/gmpoztzuu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.tarul.cn/Article/details/gtdlmzpjr.sHtML

TS:   // 同 JS
来源：http://www.m.share.sjlbkw.cn/Article/details/govyujmok.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fktsv.cn/Article/details/gjjeviylw.sHtML

Go:   go f()
来源：http://blog.vehdjk.com/Article/details/gryoznxcb.sHtML

Ruby: Thread.new { f }
来源：http://wap.tarul.cn/Article/details/gzokuvlmn.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fktsv.cn/Article/details/gnqczcdnb.sHtML

[O02] 使用线程池
来源：http://mobile.fktsv.cn/Article/details/gnauuatga.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.epnwcf.com/Article/details/gpedgqokx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.bbcook.cn/Article/details/gszavhzla.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.yfazqb.com/Article/details/gkmpmgehe.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.sjlbkw.cn/Article/details/gkozqsruc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.sjlbkw.cn/Article/details/grhexqazm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.tarul.cn/Article/details/gustnmgpk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.epnwcf.com/Article/details/gyfqcnvlk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fktsv.cn/Article/details/ghpdpigbc.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fktsv.cn/Article/details/gqxtllpra.sHtML

Py:   with lock: shared += 1
来源：http://blog.fktsv.cn/Article/details/gzrqpfsip.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.epnwcf.com/Article/details/gfaasnomq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.vehdjk.com/Article/details/ghqnwdksq.sHtML

TS:   // 同 JS
来源：http://read.share.tarul.cn/Article/details/gxgsobvrq.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.bbcook.cn/Article/details/gszqvjzoz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.vehdjk.com/Article/details/gyubyepht.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.tarul.cn/Article/details/gagzvheqa.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fktsv.cn/Article/details/gacgiywmi.sHtML

[O04] 定义异步函数并等待
来源：http://wap.sjlbkw.cn/Article/details/gfjqmswjc.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.yfazqb.com/Article/details/gssvnrvoi.sHtML


<!-- 参考信息 -->