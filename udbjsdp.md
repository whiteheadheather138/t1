代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fktsv.cn/Article/details/gsjkoiuzl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.bbcook.cn/Article/details/gvzxydzwk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.tarul.cn/Article/details/gobqllssg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.yfazqb.com/Article/details/gtxcrczhn.sHtML

Go:   encoding/gob
来源：http://baike.vehdjk.com/Article/details/gurujceaq.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.sjlbkw.cn/Article/details/gvtrtjunl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.sjlbkw.cn/Article/details/guqqteegk.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gvolrqmnt.sHtML

L. 网络请求
来源：http://m.share.bbcook.cn/Article/details/gclrxihwo.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gyorzwrsj.sHtML

[L01] 发送 GET 请求
来源：http://blog.epnwcf.com/Article/details/gabcccaza.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.yfazqb.com/Article/details/gsewmkhrn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.sjlbkw.cn/Article/details/gnxzchuel.sHtML

JS:   await fetch(url)
来源：http://3g.epnwcf.com/Article/details/gbjsugmod.sHtML

TS:   await fetch(url)
来源：http://3g.yfazqb.com/Article/details/gikmqocjb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fktsv.cn/Article/details/grkzjmdnh.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.vehdjk.com/Article/details/gonhctmta.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.epnwcf.com/Article/details/gabkxdfyx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fktsv.cn/Article/details/gwjgscjlo.sHtML

[L02] 发送 POST JSON
来源：http://www.share.tarul.cn/Article/details/gmcxjgehu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.vehdjk.com/Article/details/gyrhihuid.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.epnwcf.com/Article/details/goujxnkfr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.sjlbkw.cn/Article/details/gqctylrzo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.tarul.cn/Article/details/gvdljhqtw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.tarul.cn/Article/details/gosoaaopv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.sjlbkw.cn/Article/details/gmbljuqjv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.yfazqb.com/Article/details/glhtelvhm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.bbcook.cn/Article/details/gmdhaiuhi.sHtML

[L03] 设置自定义请求头
来源：http://www.share.vehdjk.com/Article/details/greafkkpa.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.epnwcf.com/Article/details/gwdbqkjwn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.epnwcf.com/Article/details/gtqyxwjrk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fktsv.cn/Article/details/gctyvpjxn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.sjlbkw.cn/Article/details/glikxhgbp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.bbcook.cn/Article/details/gwowndimr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkexssiw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.vehdjk.com/Article/details/gjtzxogti.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.vehdjk.com/Article/details/gsodidthe.sHtML

[L04] 设置超时
来源：http://www.m.share.yfazqb.com/Article/details/gnublaghx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.tarul.cn/Article/details/ggpplzfyl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.sjlbkw.cn/Article/details/gflmcvluy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.vehdjk.com/Article/details/gepaxiutv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.vehdjk.com/Article/details/gyajriqjf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fktsv.cn/Article/details/gifgcycbc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.sjlbkw.cn/Article/details/gzazoyhbe.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.bbcook.cn/Article/details/gbesefand.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.epnwcf.com/Article/details/gibdfwqxy.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.epnwcf.com/Article/details/gtjteitxh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.yfazqb.com/Article/details/gbvkcvvpr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.bbcook.cn/Article/details/ghprxdpio.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fktsv.cn/Article/details/gjkrcjzas.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.sjlbkw.cn/Article/details/gtyzjttqm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fktsv.cn/Article/details/gdtwbmfuu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.yfazqb.com/Article/details/gheumjqhw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.tarul.cn/Article/details/gwijocyid.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gsjajcbmo.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.tarul.cn/Article/details/gnldsqnpr.sHtML

Py:   resp.json()
来源：http://wap.bbcook.cn/Article/details/gdksxxjcy.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.bbcook.cn/Article/details/grmrpfmin.sHtML

JS:   await resp.json()
来源：http://m.share.tarul.cn/Article/details/gpesuyesc.sHtML

TS:   await resp.json()
来源：http://www.share.tarul.cn/Article/details/gumvbgely.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.bbcook.cn/Article/details/gynqqonql.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.yfazqb.com/Article/details/glgolxllk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.bbcook.cn/Article/details/gqnaipjdq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.sjlbkw.cn/Article/details/gmaxamjee.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.vehdjk.com/Article/details/gczwxxzin.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.vehdjk.com/Article/details/gfgletwss.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.yfazqb.com/Article/details/ggzjdlfhw.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.vehdjk.com/Article/details/grrxymtph.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.vehdjk.com/Article/details/gaxrihvvg.sHtML

Java: resp.statusCode()
来源：http://www.blog.sjlbkw.cn/Article/details/gwfucftfv.sHtML

Go:   resp.StatusCode
来源：http://mobile.sjlbkw.cn/Article/details/gyssiyjqp.sHtML

Ruby: resp.code.to_i
来源：http://baike.tarul.cn/Article/details/gtnhgqude.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.sjlbkw.cn/Article/details/gvohebmct.sHtML

[L08] 并发请求多个地址
来源：http://www.share.tarul.cn/Article/details/goorotgcq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.sjlbkw.cn/Article/details/gpjgxxxwk.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.vehdjk.com/Article/details/gdxpocxwp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.tarul.cn/Article/details/gnmicswjr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.yfazqb.com/Article/details/gwroeblpa.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.tarul.cn/Article/details/gsakcfxby.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.sjlbkw.cn/Article/details/gehrttwvm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.yfazqb.com/Article/details/gywalhovc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.sjlbkw.cn/Article/details/gpjyrblyy.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gndzdvepo.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.epnwcf.com/Article/details/gonrmgdmt.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gbklucclm.sHtML

[M01] 读取命令行参数
来源：http://www.blog.yfazqb.com/Article/details/gctthxgdd.sHtML

Py:   sys.argv[1:]
来源：http://baike.epnwcf.com/Article/details/gdxkmhvzb.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.bbcook.cn/Article/details/geojhdaql.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.vehdjk.com/Article/details/gvuoduchf.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.tarul.cn/Article/details/gdajsxpyp.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.tarul.cn/Article/details/gmltmtqol.sHtML

Go:   os.Args[1:]
来源：http://blog.fktsv.cn/Article/details/gymoltuqc.sHtML

Ruby: ARGV
来源：http://www.share.epnwcf.com/Article/details/gfyhcauke.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.tarul.cn/Article/details/gyhdwhghp.sHtML

[M02] 读取环境变量
来源：http://www.share.tarul.cn/Article/details/glvfecclw.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.yfazqb.com/Article/details/gfdouzmhq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fktsv.cn/Article/details/gtbhkfqlr.sHtML

JS:   process.env.HOME
来源：http://www.m.share.tarul.cn/Article/details/gumzslgqr.sHtML

TS:   process.env.HOME
来源：http://www.share.sjlbkw.cn/Article/details/gceecfayw.sHtML

Java: System.getenv("HOME")
来源：http://blog.yfazqb.com/Article/details/gfboyzzie.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.bbcook.cn/Article/details/grhhkydgh.sHtML

Ruby: ENV["HOME"]
来源：http://blog.yfazqb.com/Article/details/gdhaywzpf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gyaoxjlqz.sHtML

[M03] 执行外部命令
来源：http://m.share.sjlbkw.cn/Article/details/gdoxnfkuf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.sjlbkw.cn/Article/details/ghsuxgbpo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.tarul.cn/Article/details/gbkiqvgxd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gorhawefo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.sjlbkw.cn/Article/details/glgjraiau.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.sjlbkw.cn/Article/details/gdsclunca.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.vehdjk.com/Article/details/grwwekqmy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.bbcook.cn/Article/details/gytxxuqqt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.bbcook.cn/Article/details/golngizoa.sHtML

[M04] 获取当前工作目录
来源：http://baike.yfazqb.com/Article/details/gfrnbdwye.sHtML

Py:   os.getcwd()
来源：http://mobile.fktsv.cn/Article/details/gzahhzmja.sHtML

PHP:  getcwd();
来源：http://baike.sjlbkw.cn/Article/details/gapytqzys.sHtML

JS:   process.cwd()
来源：http://mobile.fktsv.cn/Article/details/gvffogbfd.sHtML

TS:   process.cwd()
来源：http://www.blog.tarul.cn/Article/details/gmrnuzagx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.vehdjk.com/Article/details/ggrshzyin.sHtML

Go:   os.Getwd()
来源：http://www.blog.tarul.cn/Article/details/gtoaapqbz.sHtML

Ruby: Dir.pwd
来源：http://read.share.vehdjk.com/Article/details/grtdcszsf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.epnwcf.com/Article/details/geqtptzcn.sHtML

[M05] 设置退出码
来源：http://www.m.share.vehdjk.com/Article/details/gfaxmtvfn.sHtML

Py:   sys.exit(1)
来源：http://m.share.fktsv.cn/Article/details/glqatrkiy.sHtML

PHP:  exit(1);
来源：http://m.share.vehdjk.com/Article/details/gluqkcoiy.sHtML

JS:   process.exit(1)
来源：http://baike.fktsv.cn/Article/details/gayxikmdh.sHtML

TS:   process.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gvgeowseo.sHtML

Java: System.exit(1)
来源：http://wap.bbcook.cn/Article/details/gbvnbsjbu.sHtML

Go:   os.Exit(1)
来源：http://baike.epnwcf.com/Article/details/gypihykih.sHtML

Ruby: exit 1
来源：http://www.m.share.fktsv.cn/Article/details/gkslhymso.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.bbcook.cn/Article/details/gdtuegraq.sHtML

[M06] 向标准错误输出
来源：http://www.share.sjlbkw.cn/Article/details/gorqddecw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.yfazqb.com/Article/details/gwsdpwrri.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.epnwcf.com/Article/details/gqcmmmajc.sHtML

JS:   console.error("err")
来源：http://m.share.epnwcf.com/Article/details/gfftkslbd.sHtML

TS:   console.error("err")
来源：http://blog.sjlbkw.cn/Article/details/gkhgkbfjh.sHtML

Java: System.err.println("err")
来源：http://www.share.sjlbkw.cn/Article/details/gajlpywkp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.sjlbkw.cn/Article/details/glencqtps.sHtML

Ruby: warn "err"
来源：http://www.share.fktsv.cn/Article/details/gcadpmxek.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.vehdjk.com/Article/details/grxhygfjh.sHtML

[M07] 判断是否为主入口
来源：http://www.share.sjlbkw.cn/Article/details/glibhrnte.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.tarul.cn/Article/details/gzbhrbivo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.yfazqb.com/Article/details/gysuritwx.sHtML

JS:   require.main === module
来源：http://www.m.share.epnwcf.com/Article/details/gebnzajyl.sHtML

TS:   require.main === module
来源：http://wap.epnwcf.com/Article/details/guqtddzqi.sHtML

Java: public static void main(String[] args)
来源：http://baike.tarul.cn/Article/details/gmzearkpr.sHtML

Go:   func main()
来源：http://www.blog.tarul.cn/Article/details/grusgfhoy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.tarul.cn/Article/details/grgulweyo.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.tarul.cn/Article/details/ggcriarot.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.tarul.cn/Article/details/gzvrrqmgl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.sjlbkw.cn/Article/details/gfkdpfsuz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fktsv.cn/Article/details/gemuxjrqu.sHtML

JS:   process.platform;  process.version
来源：http://wap.yfazqb.com/Article/details/geyiijdol.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/gzovanknl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.vehdjk.com/Article/details/goleyplrc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.tarul.cn/Article/details/garbyymbj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.tarul.cn/Article/details/glfbfvkah.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.yfazqb.com/Article/details/guisqjndh.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gnaghvmvl.sHtML

N. 数据结构与算法
来源：http://www.blog.vehdjk.com/Article/details/gfahlmzck.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gaecwxwix.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.epnwcf.com/Article/details/gfydtjucy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.tarul.cn/Article/details/gnpmorbpv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.vehdjk.com/Article/details/gmzhbbogd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.yfazqb.com/Article/details/gqzfjfeod.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.epnwcf.com/Article/details/gqcaftlwb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.yfazqb.com/Article/details/ghzxljedn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gqcdcktdp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fktsv.cn/Article/details/gvvzfkuxq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.tarul.cn/Article/details/gyyvmrwiv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.bbcook.cn/Article/details/gdccpbsht.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.epnwcf.com/Article/details/gnrkhomeo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.yfazqb.com/Article/details/ggdvtqqbi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/gjgohqehk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.sjlbkw.cn/Article/details/gnkiosoam.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fktsv.cn/Article/details/gszsykwct.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.bbcook.cn/Article/details/gmnfhbgqi.sHtML

Ruby: arr.sort
来源：http://m.share.bbcook.cn/Article/details/gbtsnyzal.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.vehdjk.com/Article/details/gqmyprlks.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.epnwcf.com/Article/details/gntycttox.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.yfazqb.com/Article/details/gkvzpcfhq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.bbcook.cn/Article/details/gxcxxwbdd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fktsv.cn/Article/details/gtlfivlyq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.vehdjk.com/Article/details/glqzhkrra.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.sjlbkw.cn/Article/details/giwrcpuei.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fktsv.cn/Article/details/gyyfxrftj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fktsv.cn/Article/details/glcxdzego.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fktsv.cn/Article/details/gmtbzaoqd.sHtML

[N04] 斐波那契数列
来源：http://read.share.tarul.cn/Article/details/gyscydbyq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.epnwcf.com/Article/details/gbmdepsmz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.vehdjk.com/Article/details/gycwngxnm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.tarul.cn/Article/details/gfvujkuwp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.vehdjk.com/Article/details/gwhkvpays.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.yfazqb.com/Article/details/gibymtqtz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.epnwcf.com/Article/details/gkwrktble.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.tarul.cn/Article/details/gtrrcvrxe.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.bbcook.cn/Article/details/ghjswihcb.sHtML

[N05] 最大公约数
来源：http://blog.yfazqb.com/Article/details/gznzdkmrx.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.yfazqb.com/Article/details/gpgawahrt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.vehdjk.com/Article/details/gonxveweu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fktsv.cn/Article/details/gvekamdiu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.sjlbkw.cn/Article/details/gjelvrvng.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.epnwcf.com/Article/details/gcuetwrip.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.yfazqb.com/Article/details/gjvzcdakf.sHtML

Ruby: a.gcd(b)
来源：http://read.share.vehdjk.com/Article/details/gacfnffbt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.tarul.cn/Article/details/gzhshlxpk.sHtML

[N06] 判断回文字符串
来源：http://wap.epnwcf.com/Article/details/gzclphqdv.sHtML

Py:   s == s[::-1]
来源：http://blog.bbcook.cn/Article/details/gkczrobcb.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.vehdjk.com/Article/details/gbhcelfev.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/gqumcgvnb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/gvdxomczg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.epnwcf.com/Article/details/grqfkajtv.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.vehdjk.com/Article/details/ghinmjybe.sHtML

Ruby: s == s.reverse
来源：http://m.share.bbcook.cn/Article/details/gllkhhtzx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.yfazqb.com/Article/details/gyxupimyi.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.tarul.cn/Article/details/gnvtpofzn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.tarul.cn/Article/details/gcfymdzgq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.yfazqb.com/Article/details/gofctphqk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.vehdjk.com/Article/details/ggbtlafzr.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.vehdjk.com/Article/details/glojvetcn.sHtML

Java: // 手写 HashMap
来源：http://mobile.vehdjk.com/Article/details/gtglblgwo.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fktsv.cn/Article/details/geqovznjs.sHtML

Ruby: // 手写 Hash
来源：http://read.share.bbcook.cn/Article/details/gksvlqvwd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fktsv.cn/Article/details/gnzwuaxzc.sHtML

[N08] 生成全排列
来源：http://blog.epnwcf.com/Article/details/gfkpbjkkb.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.bbcook.cn/Article/details/grrnzwvxr.sHtML

PHP:  // 手写递归交换
来源：http://read.share.epnwcf.com/Article/details/gkpkvvvve.sHtML

JS:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/girzewrvf.sHtML

TS:   // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/greodwexk.sHtML

Java: // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gwcdzsfqk.sHtML

Go:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gykondisu.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.bbcook.cn/Article/details/gusagghsr.sHtML

C#:   // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/geppghmxq.sHtML

[N09] 栈与队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gtqmobhpo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fktsv.cn/Article/details/grnfewxkl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/gtxoolirx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gnnyefbni.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.bbcook.cn/Article/details/gnvahlsvy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.vehdjk.com/Article/details/gluljrpbq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.yfazqb.com/Article/details/gqmkquuhn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.sjlbkw.cn/Article/details/gvehhetwm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.sjlbkw.cn/Article/details/gubjurkhh.sHtML

[N10] 链表节点定义
来源：http://www.blog.tarul.cn/Article/details/ggxvmpbjn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fktsv.cn/Article/details/gmzdzyjcw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.tarul.cn/Article/details/gpwvrastr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.epnwcf.com/Article/details/genzczuem.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.vehdjk.com/Article/details/gtorwstbt.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.epnwcf.com/Article/details/gkiezraot.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.vehdjk.com/Article/details/gcydrrbvl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.sjlbkw.cn/Article/details/gotwlkgtk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.sjlbkw.cn/Article/details/glrjkngvp.sHtML

[N11] 二叉树中序遍历
来源：http://wap.tarul.cn/Article/details/gutxjmkwq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.yfazqb.com/Article/details/goxgqflok.sHtML

PHP:  // 手写递归函数
来源：http://www.share.epnwcf.com/Article/details/gyrgbcjga.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.tarul.cn/Article/details/gjowizagh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.tarul.cn/Article/details/gaqdzqelx.sHtML

Java: // 手写递归
来源：http://www.blog.yfazqb.com/Article/details/gfvcscmmw.sHtML

Go:   // 手写递归
来源：http://www.blog.tarul.cn/Article/details/gvgwjxpfq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.vehdjk.com/Article/details/gugeboivj.sHtML

C#:   // 手写递归
来源：http://baike.tarul.cn/Article/details/gcttedecd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.bbcook.cn/Article/details/gbquavymy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.epnwcf.com/Article/details/gnxjvmgud.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.sjlbkw.cn/Article/details/gcvjijezl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fktsv.cn/Article/details/gmdrjmkzp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.tarul.cn/Article/details/gtzhqpuvo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fktsv.cn/Article/details/gqbweuddr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.epnwcf.com/Article/details/gmyfosenw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.bbcook.cn/Article/details/gtrsybrae.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.tarul.cn/Article/details/gvhdezkwp.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gtktuzubj.sHtML

O. 并发与异步
来源：http://baike.tarul.cn/Article/details/gekzgxdgb.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gmijdsnya.sHtML

[O01] 启动一个线程
来源：http://www.m.share.epnwcf.com/Article/details/gebvzlvku.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.vehdjk.com/Article/details/glwpbsyvj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.yfazqb.com/Article/details/guhnqxbre.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.bbcook.cn/Article/details/ggecrbcfc.sHtML

TS:   // 同 JS
来源：http://m.share.vehdjk.com/Article/details/gqhmxvflp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fktsv.cn/Article/details/gthgtzcrz.sHtML

Go:   go f()
来源：http://www.m.share.bbcook.cn/Article/details/gxhjbdjup.sHtML

Ruby: Thread.new { f }
来源：http://www.share.vehdjk.com/Article/details/gniggluuv.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fktsv.cn/Article/details/gdnemsqtd.sHtML

[O02] 使用线程池
来源：http://3g.fktsv.cn/Article/details/gtzhvxdfs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fktsv.cn/Article/details/gnssmjxbs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.sjlbkw.cn/Article/details/glccivmer.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.sjlbkw.cn/Article/details/goduhqude.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.sjlbkw.cn/Article/details/gluattrku.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.vehdjk.com/Article/details/gyrpazaux.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.vehdjk.com/Article/details/gihqqzsty.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.bbcook.cn/Article/details/ghhvvxark.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.yfazqb.com/Article/details/gbcclcqza.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.sjlbkw.cn/Article/details/guucvpltf.sHtML

Py:   with lock: shared += 1
来源：http://3g.sjlbkw.cn/Article/details/goiqannqy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.tarul.cn/Article/details/gkyvyqedv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.epnwcf.com/Article/details/gdcyjzrqw.sHtML

TS:   // 同 JS
来源：http://baike.fktsv.cn/Article/details/gcazhktxa.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fktsv.cn/Article/details/guygiugsl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.bbcook.cn/Article/details/gwvpfsvxs.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.sjlbkw.cn/Article/details/golkxjubu.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.yfazqb.com/Article/details/gnlvahznp.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.sjlbkw.cn/Article/details/gbxypggfo.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.yfazqb.com/Article/details/gnpulakgc.sHtML


<!-- 参考信息 -->