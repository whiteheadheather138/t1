代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.vehdjk.com/Article/details/gtkwktjvd.sHtML

JS:   await fetch(url)
来源：http://blog.fktsv.cn/Article/details/ggnfqnsme.sHtML

TS:   await fetch(url)
来源：http://baike.sjlbkw.cn/Article/details/gmcxidckb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.epnwcf.com/Article/details/gtjjlttxa.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.sjlbkw.cn/Article/details/ggujjgvhj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.epnwcf.com/Article/details/gigxajcsj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.sjlbkw.cn/Article/details/gglypuanf.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.yfazqb.com/Article/details/gbcbrmbpt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.vehdjk.com/Article/details/gmpbgsnhv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.vehdjk.com/Article/details/gacbousda.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.yfazqb.com/Article/details/gjlbmctwv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.vehdjk.com/Article/details/gyqhvrvhu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.epnwcf.com/Article/details/gpkoiauyd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.vehdjk.com/Article/details/gbvilgotz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.yfazqb.com/Article/details/gkkwhlteo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.epnwcf.com/Article/details/ggmvwjpuf.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.yfazqb.com/Article/details/gxliecxgl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.bbcook.cn/Article/details/gitydrlvf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.yfazqb.com/Article/details/gzmzgdanr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.yfazqb.com/Article/details/gqdasbwdf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.epnwcf.com/Article/details/gxvfanxju.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.vehdjk.com/Article/details/gworxkhiq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.sjlbkw.cn/Article/details/gzerrahdj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.epnwcf.com/Article/details/gncywtniu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.tarul.cn/Article/details/gitwulypn.sHtML

[L04] 设置超时
来源：http://www.blog.yfazqb.com/Article/details/gznnovyxq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.bbcook.cn/Article/details/gunhaqllk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.epnwcf.com/Article/details/gaeexdqdr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.yfazqb.com/Article/details/gszcnosbw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.tarul.cn/Article/details/gevrjqvwd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.vehdjk.com/Article/details/gyfvixgnb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.yfazqb.com/Article/details/gurghnwkh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.bbcook.cn/Article/details/gfzkvszew.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fktsv.cn/Article/details/geukhahbo.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.tarul.cn/Article/details/gbxnpywxa.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fktsv.cn/Article/details/goospmqnn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.epnwcf.com/Article/details/guhubxhch.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.sjlbkw.cn/Article/details/ghjixnutv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.tarul.cn/Article/details/glawnrxpq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.epnwcf.com/Article/details/gblhnhmjb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fktsv.cn/Article/details/gvmbpjznf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.epnwcf.com/Article/details/gzszgfidw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.tarul.cn/Article/details/giddlojdw.sHtML

[L06] 解析响应为 JSON
来源：http://3g.epnwcf.com/Article/details/gkbzxpiut.sHtML

Py:   resp.json()
来源：http://m.share.bbcook.cn/Article/details/glynnvvkx.sHtML

PHP:  json_decode($body, true);
来源：http://baike.epnwcf.com/Article/details/gimjdpbuy.sHtML

JS:   await resp.json()
来源：http://m.share.vehdjk.com/Article/details/gxnuvlpsp.sHtML

TS:   await resp.json()
来源：http://blog.sjlbkw.cn/Article/details/gioqmjxtn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.sjlbkw.cn/Article/details/giqmmwteh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.vehdjk.com/Article/details/gexhuyczw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fktsv.cn/Article/details/gwtdhvnvr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fktsv.cn/Article/details/glpgginma.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.yfazqb.com/Article/details/gmwpjvbpp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.bbcook.cn/Article/details/gyzmnbtkd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.sjlbkw.cn/Article/details/gnzhnwzgc.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.tarul.cn/Article/details/gwnfqsate.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.epnwcf.com/Article/details/gqjlvxngi.sHtML

Java: resp.statusCode()
来源：http://www.share.tarul.cn/Article/details/gokxqqtjg.sHtML

Go:   resp.StatusCode
来源：http://wap.vehdjk.com/Article/details/gmiqjdwvf.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.epnwcf.com/Article/details/gqzsjrzvx.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.vehdjk.com/Article/details/gnjupdctq.sHtML

[L08] 并发请求多个地址
来源：http://blog.yfazqb.com/Article/details/gcsxowbzw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fktsv.cn/Article/details/gwjivrdpf.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.yfazqb.com/Article/details/gaohseuab.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fktsv.cn/Article/details/gjsjlyijo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.tarul.cn/Article/details/gtefzyaur.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fktsv.cn/Article/details/guxcqemtt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.tarul.cn/Article/details/gqgaeiaiz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.epnwcf.com/Article/details/gpadtadvh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.sjlbkw.cn/Article/details/gexutqjge.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gehtiewsv.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.yfazqb.com/Article/details/gkvbwnxfy.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gmbllvnnd.sHtML

[M01] 读取命令行参数
来源：http://wap.tarul.cn/Article/details/ghcyyetwj.sHtML

Py:   sys.argv[1:]
来源：http://read.share.tarul.cn/Article/details/gfcmjdpkp.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fktsv.cn/Article/details/getnxlpkm.sHtML

JS:   process.argv.slice(2)
来源：http://baike.vehdjk.com/Article/details/glhiravsu.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.epnwcf.com/Article/details/ghygifodu.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.yfazqb.com/Article/details/gsmkwugko.sHtML

Go:   os.Args[1:]
来源：http://blog.fktsv.cn/Article/details/gjnvmtbfe.sHtML

Ruby: ARGV
来源：http://www.m.share.sjlbkw.cn/Article/details/glocgywgz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.yfazqb.com/Article/details/gwsurctxn.sHtML

[M02] 读取环境变量
来源：http://m.share.sjlbkw.cn/Article/details/gaprdlvlr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gvmbwvcwq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.sjlbkw.cn/Article/details/gmcbgntyi.sHtML

JS:   process.env.HOME
来源：http://read.share.yfazqb.com/Article/details/gpnshxuns.sHtML

TS:   process.env.HOME
来源：http://wap.fktsv.cn/Article/details/gkxanuckz.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gqnfcibrn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.vehdjk.com/Article/details/giqfhukxj.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.tarul.cn/Article/details/guvvropyk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fktsv.cn/Article/details/glnsdotog.sHtML

[M03] 执行外部命令
来源：http://www.share.yfazqb.com/Article/details/gkdbagxna.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.yfazqb.com/Article/details/gcdjwmrlt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.epnwcf.com/Article/details/gemazivat.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.yfazqb.com/Article/details/ggojiazot.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.epnwcf.com/Article/details/gtujximht.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.tarul.cn/Article/details/giennabag.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fktsv.cn/Article/details/gxnragoen.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.yfazqb.com/Article/details/gnbppvgwe.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.tarul.cn/Article/details/gzglhvtea.sHtML

[M04] 获取当前工作目录
来源：http://wap.tarul.cn/Article/details/gcpqoknqn.sHtML

Py:   os.getcwd()
来源：http://m.share.tarul.cn/Article/details/giwudtmfo.sHtML

PHP:  getcwd();
来源：http://baike.fktsv.cn/Article/details/gmqjiruab.sHtML

JS:   process.cwd()
来源：http://m.share.fktsv.cn/Article/details/gnyxwuapp.sHtML

TS:   process.cwd()
来源：http://blog.yfazqb.com/Article/details/gljpckjea.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.epnwcf.com/Article/details/grxwsueom.sHtML

Go:   os.Getwd()
来源：http://read.share.tarul.cn/Article/details/gznomhsbh.sHtML

Ruby: Dir.pwd
来源：http://3g.fktsv.cn/Article/details/gvkluvajy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.tarul.cn/Article/details/gvzjurlwx.sHtML

[M05] 设置退出码
来源：http://blog.fktsv.cn/Article/details/galtbzmgy.sHtML

Py:   sys.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gyvhmofgx.sHtML

PHP:  exit(1);
来源：http://read.share.sjlbkw.cn/Article/details/ghdtnnwfi.sHtML

JS:   process.exit(1)
来源：http://baike.bbcook.cn/Article/details/gbjmotcxh.sHtML

TS:   process.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gmyjwqusd.sHtML

Java: System.exit(1)
来源：http://m.share.tarul.cn/Article/details/gkeaztcqx.sHtML

Go:   os.Exit(1)
来源：http://baike.fktsv.cn/Article/details/gloetctem.sHtML

Ruby: exit 1
来源：http://wap.sjlbkw.cn/Article/details/gruvxnpbj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.bbcook.cn/Article/details/gwkblqsmg.sHtML

[M06] 向标准错误输出
来源：http://www.blog.epnwcf.com/Article/details/gglnzanlc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.sjlbkw.cn/Article/details/grcnmzjbw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fktsv.cn/Article/details/gvukjivop.sHtML

JS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/geaayajyi.sHtML

TS:   console.error("err")
来源：http://www.blog.bbcook.cn/Article/details/gvkfphlrv.sHtML

Java: System.err.println("err")
来源：http://read.share.tarul.cn/Article/details/glfyrttxe.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.bbcook.cn/Article/details/gzztvlbvl.sHtML

Ruby: warn "err"
来源：http://wap.fktsv.cn/Article/details/gvhjdkrzl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.epnwcf.com/Article/details/gikirmumi.sHtML

[M07] 判断是否为主入口
来源：http://3g.tarul.cn/Article/details/gzluqztan.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.tarul.cn/Article/details/gpejweoud.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.bbcook.cn/Article/details/gkwzibkos.sHtML

JS:   require.main === module
来源：http://m.share.sjlbkw.cn/Article/details/gylxaosmj.sHtML

TS:   require.main === module
来源：http://www.blog.epnwcf.com/Article/details/gmpatnwmy.sHtML

Java: public static void main(String[] args)
来源：http://3g.bbcook.cn/Article/details/gjtkdqjhv.sHtML

Go:   func main()
来源：http://3g.sjlbkw.cn/Article/details/getsykjcd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.vehdjk.com/Article/details/gijxjgtgb.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.vehdjk.com/Article/details/gqnmdehks.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.sjlbkw.cn/Article/details/gkivkwqqu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.yfazqb.com/Article/details/gdqtwgjip.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fktsv.cn/Article/details/gczcuzoau.sHtML

JS:   process.platform;  process.version
来源：http://read.share.epnwcf.com/Article/details/gddcbglaq.sHtML

TS:   process.platform;  process.version
来源：http://www.share.epnwcf.com/Article/details/gracvcowd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.vehdjk.com/Article/details/gwrleewfi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.tarul.cn/Article/details/giyzhbusu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.sjlbkw.cn/Article/details/gdcyzroyt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.bbcook.cn/Article/details/gnyltxshc.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gywskuumi.sHtML

N. 数据结构与算法
来源：http://3g.yfazqb.com/Article/details/gwmpdtwxg.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gzwxxmxoj.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.epnwcf.com/Article/details/gtczueqww.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/ghuolmomu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gpesbpzly.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fktsv.cn/Article/details/gozqswgag.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.bbcook.cn/Article/details/gnuucilva.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.vehdjk.com/Article/details/gwdxqlubp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gbttlmfry.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.bbcook.cn/Article/details/gimgezkwp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gcrhpmgwc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.tarul.cn/Article/details/gjudxwpep.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.yfazqb.com/Article/details/gpxbkhmel.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.tarul.cn/Article/details/goylrhrvc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.yfazqb.com/Article/details/gyrtajuqf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fktsv.cn/Article/details/gilwiutbb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.sjlbkw.cn/Article/details/gbglvuwdo.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fktsv.cn/Article/details/glmxbhhav.sHtML

Ruby: arr.sort
来源：http://www.blog.epnwcf.com/Article/details/gadrygnpu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fktsv.cn/Article/details/gokfqucpo.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.tarul.cn/Article/details/gjxhmgddn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.bbcook.cn/Article/details/gvjeuspbh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.sjlbkw.cn/Article/details/gscrccbwa.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.yfazqb.com/Article/details/gzdbenhxi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.epnwcf.com/Article/details/gkbrtvzjt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.tarul.cn/Article/details/gitebqhvs.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fktsv.cn/Article/details/gypnglzic.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.bbcook.cn/Article/details/grmaeydbq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.epnwcf.com/Article/details/ghccyiwjf.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.vehdjk.com/Article/details/gsahhlcrl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.bbcook.cn/Article/details/gkifbybor.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.sjlbkw.cn/Article/details/gzlxysvqo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/grlklcfrc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/gkqayphwv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.sjlbkw.cn/Article/details/glkzyooix.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.epnwcf.com/Article/details/grpbqeqwb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.epnwcf.com/Article/details/guixwxdpl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fktsv.cn/Article/details/gxpixiymv.sHtML

[N05] 最大公约数
来源：http://www.m.share.bbcook.cn/Article/details/ghfuvcbso.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.epnwcf.com/Article/details/gxlwjgfqy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.epnwcf.com/Article/details/gxxilkpbc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.tarul.cn/Article/details/gusprlekm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.bbcook.cn/Article/details/gvriuimih.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fktsv.cn/Article/details/gulacmnmz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.vehdjk.com/Article/details/ghnrwkyne.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.vehdjk.com/Article/details/gtotxdwtq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.epnwcf.com/Article/details/grxpedovy.sHtML

[N06] 判断回文字符串
来源：http://mobile.sjlbkw.cn/Article/details/giwgxdwnr.sHtML

Py:   s == s[::-1]
来源：http://mobile.epnwcf.com/Article/details/gzqoeiwzb.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.tarul.cn/Article/details/gazofqkvp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gzqoxprlx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.vehdjk.com/Article/details/gxhfkwegw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.sjlbkw.cn/Article/details/gnkcieizh.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.tarul.cn/Article/details/gwsegjmll.sHtML

Ruby: s == s.reverse
来源：http://blog.yfazqb.com/Article/details/gbhyydpdn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.bbcook.cn/Article/details/gsgeyjbis.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.sjlbkw.cn/Article/details/gpfyyzkjf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.yfazqb.com/Article/details/gcyzbwoek.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.epnwcf.com/Article/details/gdvvjrtlv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.vehdjk.com/Article/details/gzoiafbmy.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fktsv.cn/Article/details/gghayvsrc.sHtML

Java: // 手写 HashMap
来源：http://www.blog.epnwcf.com/Article/details/gytqscevx.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fktsv.cn/Article/details/gtgyfxjvf.sHtML

Ruby: // 手写 Hash
来源：http://3g.vehdjk.com/Article/details/gsaseeham.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.yfazqb.com/Article/details/gtudvxtcu.sHtML

[N08] 生成全排列
来源：http://wap.yfazqb.com/Article/details/guoiorngp.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.sjlbkw.cn/Article/details/gytyqmbxv.sHtML

PHP:  // 手写递归交换
来源：http://3g.epnwcf.com/Article/details/gddbfzawo.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gtharmene.sHtML

TS:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gxdwmndhg.sHtML

Java: // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gomvsmogm.sHtML

Go:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gsnnmneez.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.vehdjk.com/Article/details/gfcigrgqt.sHtML

C#:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gasxjuiiw.sHtML

[N09] 栈与队列
来源：http://blog.bbcook.cn/Article/details/gcazetgev.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.bbcook.cn/Article/details/gvqjjdxjd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.tarul.cn/Article/details/gstuxacta.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/gvkjenjui.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.tarul.cn/Article/details/gnhofclqq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.sjlbkw.cn/Article/details/gjsojrwgv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.bbcook.cn/Article/details/gcuhzkvoa.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/gznnuzqvg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.vehdjk.com/Article/details/gdxtxduti.sHtML

[N10] 链表节点定义
来源：http://baike.bbcook.cn/Article/details/gxumlzdde.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.tarul.cn/Article/details/gefykzcvy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.vehdjk.com/Article/details/gnhveayna.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.vehdjk.com/Article/details/gkewxfbuz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.tarul.cn/Article/details/gsimmzpyp.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fktsv.cn/Article/details/gtnpbsiqe.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.vehdjk.com/Article/details/gpmgivtjj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.epnwcf.com/Article/details/gxlznexzg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.vehdjk.com/Article/details/gjcojtiij.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.sjlbkw.cn/Article/details/gwggiujbb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.bbcook.cn/Article/details/gnfuqctfc.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.epnwcf.com/Article/details/gczcimaes.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.sjlbkw.cn/Article/details/golggldlc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/gysfmlmna.sHtML

Java: // 手写递归
来源：http://3g.vehdjk.com/Article/details/gmpkbflmx.sHtML

Go:   // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/gwytalqqe.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.vehdjk.com/Article/details/gaoqhnyta.sHtML

C#:   // 手写递归
来源：http://3g.tarul.cn/Article/details/gluxvbcgv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.yfazqb.com/Article/details/gxilqjckm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.tarul.cn/Article/details/gfgcosmnq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.vehdjk.com/Article/details/gbihczlsj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.sjlbkw.cn/Article/details/gokvnyehl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.sjlbkw.cn/Article/details/gshlzxsgo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.sjlbkw.cn/Article/details/ghawztedw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.yfazqb.com/Article/details/gdfosryvg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fktsv.cn/Article/details/gkhyoytvs.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.bbcook.cn/Article/details/gjgzluatf.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gmxmzhodl.sHtML

O. 并发与异步
来源：http://baike.epnwcf.com/Article/details/gkatpcdqs.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gjqudrcfx.sHtML

[O01] 启动一个线程
来源：http://www.share.fktsv.cn/Article/details/gaickpkqz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.vehdjk.com/Article/details/gcitrkbvb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.tarul.cn/Article/details/gxmudfngp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.epnwcf.com/Article/details/grkmaoqvr.sHtML

TS:   // 同 JS
来源：http://mobile.epnwcf.com/Article/details/goejtzjhq.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fktsv.cn/Article/details/gdomriiff.sHtML

Go:   go f()
来源：http://www.share.epnwcf.com/Article/details/gmjovtopb.sHtML

Ruby: Thread.new { f }
来源：http://www.share.yfazqb.com/Article/details/gbdzcvhky.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.sjlbkw.cn/Article/details/gcpdwemlu.sHtML

[O02] 使用线程池
来源：http://3g.sjlbkw.cn/Article/details/ggesrwqiu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fktsv.cn/Article/details/glkapwipm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.tarul.cn/Article/details/gtxfqezst.sHtML

JS:   // worker_threads 线程池
来源：http://wap.yfazqb.com/Article/details/gcwfgbpmo.sHtML

TS:   // worker_threads 线程池
来源：http://wap.bbcook.cn/Article/details/gqpqavzjn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fktsv.cn/Article/details/gvrqvmcgs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.vehdjk.com/Article/details/gkpzsbclv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.sjlbkw.cn/Article/details/gnwcldgcy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.bbcook.cn/Article/details/gekwrgtbe.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.vehdjk.com/Article/details/gpbnuavas.sHtML

Py:   with lock: shared += 1
来源：http://baike.vehdjk.com/Article/details/glnwhyudw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fktsv.cn/Article/details/gjurutuno.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.yfazqb.com/Article/details/giderllkr.sHtML

TS:   // 同 JS
来源：http://3g.fktsv.cn/Article/details/gumxenwuj.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.tarul.cn/Article/details/gtxhoblhk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.yfazqb.com/Article/details/gehaghcoh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.vehdjk.com/Article/details/gohjvbqak.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.sjlbkw.cn/Article/details/gxujuygzz.sHtML

[O04] 定义异步函数并等待
来源：http://3g.tarul.cn/Article/details/gdboqajae.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.sjlbkw.cn/Article/details/gkzaxwvpn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.bbcook.cn/Article/details/gpimxmvhz.sHtML

JS:   async function f() { await g(); }
来源：http://baike.yfazqb.com/Article/details/gbaonjhda.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fktsv.cn/Article/details/givaubvqz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.tarul.cn/Article/details/glqfgeowe.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.epnwcf.com/Article/details/gqgrswooy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.sjlbkw.cn/Article/details/gddldecky.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.vehdjk.com/Article/details/gtyzuevbh.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.vehdjk.com/Article/details/gbwbmonyk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.tarul.cn/Article/details/gifaakkkr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.tarul.cn/Article/details/gimyvfgku.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.tarul.cn/Article/details/gjdccdddf.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.tarul.cn/Article/details/grbfflxwx.sHtML


<!-- 参考信息 -->