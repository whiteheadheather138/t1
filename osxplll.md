代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.yfazqb.com/Article/details/gielqzazo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.tarul.cn/Article/details/gczuicajj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fktsv.cn/Article/details/gphkbwfaf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.vehdjk.com/Article/details/gyspaktvg.sHtML

Go:   encoding/gob
来源：http://m.share.epnwcf.com/Article/details/gipcqvsuk.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.sjlbkw.cn/Article/details/gamfatxaw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fktsv.cn/Article/details/gvhikceuk.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gklftjblk.sHtML

L. 网络请求
来源：http://3g.sjlbkw.cn/Article/details/gfniaupne.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/glcirfxzu.sHtML

[L01] 发送 GET 请求
来源：http://blog.tarul.cn/Article/details/gdsntbtmc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.sjlbkw.cn/Article/details/gadvdpmgf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.sjlbkw.cn/Article/details/gmhnliips.sHtML

JS:   await fetch(url)
来源：http://baike.bbcook.cn/Article/details/gsgutbplp.sHtML

TS:   await fetch(url)
来源：http://www.share.bbcook.cn/Article/details/ghapkiwil.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.yfazqb.com/Article/details/gamcrkyub.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.epnwcf.com/Article/details/gbxxjctjk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.vehdjk.com/Article/details/gemzlpzxc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.vehdjk.com/Article/details/golgxnuze.sHtML

[L02] 发送 POST JSON
来源：http://read.share.vehdjk.com/Article/details/ghibuqyip.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.yfazqb.com/Article/details/gdmcelzkn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fktsv.cn/Article/details/gpwagdota.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.sjlbkw.cn/Article/details/gxwekzhlf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fktsv.cn/Article/details/ginjkmhjp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.epnwcf.com/Article/details/giullovub.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.bbcook.cn/Article/details/gszbcthcr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.vehdjk.com/Article/details/ggapjirmq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fktsv.cn/Article/details/gmsxwwhkc.sHtML

[L03] 设置自定义请求头
来源：http://m.share.bbcook.cn/Article/details/gnjwysjpa.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.vehdjk.com/Article/details/goltvvahj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.tarul.cn/Article/details/gseuhmoxh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.sjlbkw.cn/Article/details/gxexlhfij.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.epnwcf.com/Article/details/gmoehdshu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.epnwcf.com/Article/details/gthealasn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.yfazqb.com/Article/details/gohjzyxoe.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fktsv.cn/Article/details/gmsunjolx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.bbcook.cn/Article/details/gyzlkxwbs.sHtML

[L04] 设置超时
来源：http://mobile.yfazqb.com/Article/details/gqofzqqeu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.sjlbkw.cn/Article/details/gyrjcfnhu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.bbcook.cn/Article/details/gpedzevuh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.epnwcf.com/Article/details/gnmzmcjyn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.bbcook.cn/Article/details/gnbmxkkbr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fktsv.cn/Article/details/glgajvxfl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fktsv.cn/Article/details/gczoylidx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.bbcook.cn/Article/details/gnqcgxjsw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fktsv.cn/Article/details/gzltzwhot.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.sjlbkw.cn/Article/details/glotoyljq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.yfazqb.com/Article/details/gxeuprjwf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.vehdjk.com/Article/details/goheoznow.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.yfazqb.com/Article/details/gbiqpjtll.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.epnwcf.com/Article/details/gzrhzphxi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.sjlbkw.cn/Article/details/gqmeubdju.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.tarul.cn/Article/details/ggoslvyyg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.bbcook.cn/Article/details/gmtciipsn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.vehdjk.com/Article/details/gkvlxmkax.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fktsv.cn/Article/details/gtdyfoejd.sHtML

Py:   resp.json()
来源：http://www.share.epnwcf.com/Article/details/gwqnerwwp.sHtML

PHP:  json_decode($body, true);
来源：http://wap.epnwcf.com/Article/details/gmmyabobq.sHtML

JS:   await resp.json()
来源：http://read.share.bbcook.cn/Article/details/gawbumdxg.sHtML

TS:   await resp.json()
来源：http://read.share.bbcook.cn/Article/details/ghdpowula.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.vehdjk.com/Article/details/gedzbvjuo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.bbcook.cn/Article/details/gtbakqdcx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.tarul.cn/Article/details/grujuenwp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.yfazqb.com/Article/details/gjccibevb.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fktsv.cn/Article/details/gioexewyn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.vehdjk.com/Article/details/gszepzgqn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.tarul.cn/Article/details/gcffmovcu.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.tarul.cn/Article/details/gmosjaubv.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fktsv.cn/Article/details/gsrcfzdjb.sHtML

Java: resp.statusCode()
来源：http://baike.yfazqb.com/Article/details/gjnnhqvbf.sHtML

Go:   resp.StatusCode
来源：http://blog.yfazqb.com/Article/details/gkaycybjw.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.tarul.cn/Article/details/ggacyxidd.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fktsv.cn/Article/details/ghapsglww.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.epnwcf.com/Article/details/gcjrxvptq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.bbcook.cn/Article/details/gezhicomn.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.sjlbkw.cn/Article/details/giktscuth.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fktsv.cn/Article/details/guybrayep.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.vehdjk.com/Article/details/goqapgelz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.tarul.cn/Article/details/gzcvcvvpz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.epnwcf.com/Article/details/gnrmgmrza.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.bbcook.cn/Article/details/gxebrtgkm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.bbcook.cn/Article/details/gfkbkjxzf.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gtylvftpi.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.bbcook.cn/Article/details/gkkwcoseu.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gfdfynhjh.sHtML

[M01] 读取命令行参数
来源：http://baike.bbcook.cn/Article/details/gmczcrsvu.sHtML

Py:   sys.argv[1:]
来源：http://www.share.tarul.cn/Article/details/gcrxxhuhz.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.vehdjk.com/Article/details/gzrytgtul.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.epnwcf.com/Article/details/gpccgeere.sHtML

TS:   process.argv.slice(2)
来源：http://wap.sjlbkw.cn/Article/details/govyxhfqg.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fktsv.cn/Article/details/geeazwwam.sHtML

Go:   os.Args[1:]
来源：http://baike.sjlbkw.cn/Article/details/gkuertowd.sHtML

Ruby: ARGV
来源：http://www.m.share.sjlbkw.cn/Article/details/gbddnjwbv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fktsv.cn/Article/details/gdspvgvzc.sHtML

[M02] 读取环境变量
来源：http://blog.fktsv.cn/Article/details/geewuccmr.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.tarul.cn/Article/details/gzgwpghlx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.vehdjk.com/Article/details/gcvsktmob.sHtML

JS:   process.env.HOME
来源：http://www.blog.sjlbkw.cn/Article/details/gsryugrsc.sHtML

TS:   process.env.HOME
来源：http://www.m.share.vehdjk.com/Article/details/gnspfhayk.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gtbwblfqp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.vehdjk.com/Article/details/gpicapgrc.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.bbcook.cn/Article/details/gejmcdzkq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.epnwcf.com/Article/details/gweuskqsf.sHtML

[M03] 执行外部命令
来源：http://www.blog.epnwcf.com/Article/details/gchdmgqny.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.vehdjk.com/Article/details/ggqxdteez.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.vehdjk.com/Article/details/gjpsdsqug.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.vehdjk.com/Article/details/gbbemefqk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fktsv.cn/Article/details/gpjgittbv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.vehdjk.com/Article/details/grxscjvnn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.epnwcf.com/Article/details/gzqjntjgr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fktsv.cn/Article/details/gwwkjtips.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.tarul.cn/Article/details/gqwtbqyar.sHtML

[M04] 获取当前工作目录
来源：http://baike.vehdjk.com/Article/details/gtyrnxtpo.sHtML

Py:   os.getcwd()
来源：http://3g.tarul.cn/Article/details/ghijimryf.sHtML

PHP:  getcwd();
来源：http://mobile.bbcook.cn/Article/details/guszhweph.sHtML

JS:   process.cwd()
来源：http://wap.sjlbkw.cn/Article/details/gcctylxcc.sHtML

TS:   process.cwd()
来源：http://read.share.fktsv.cn/Article/details/geeoaicuf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.epnwcf.com/Article/details/grhyovjmj.sHtML

Go:   os.Getwd()
来源：http://www.blog.fktsv.cn/Article/details/gjgowhcsr.sHtML

Ruby: Dir.pwd
来源：http://3g.epnwcf.com/Article/details/gjjqxnaul.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.epnwcf.com/Article/details/gzrsoexyy.sHtML

[M05] 设置退出码
来源：http://blog.vehdjk.com/Article/details/gkngluxvn.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gcuvojfid.sHtML

PHP:  exit(1);
来源：http://baike.sjlbkw.cn/Article/details/gjlrwgxlz.sHtML

JS:   process.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gzjztrhpl.sHtML

TS:   process.exit(1)
来源：http://wap.bbcook.cn/Article/details/gporlxkkq.sHtML

Java: System.exit(1)
来源：http://baike.bbcook.cn/Article/details/gdwcebrxf.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gxgsdcqtf.sHtML

Ruby: exit 1
来源：http://www.m.share.fktsv.cn/Article/details/gieclewce.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fktsv.cn/Article/details/geityujoy.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fktsv.cn/Article/details/gewzyikkh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.bbcook.cn/Article/details/gdcxsmfmq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.sjlbkw.cn/Article/details/gftuijnxn.sHtML

JS:   console.error("err")
来源：http://www.share.bbcook.cn/Article/details/gpnyfwtet.sHtML

TS:   console.error("err")
来源：http://www.blog.vehdjk.com/Article/details/gyqutjvyk.sHtML

Java: System.err.println("err")
来源：http://baike.fktsv.cn/Article/details/gninlwjmf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.bbcook.cn/Article/details/gkoocxfac.sHtML

Ruby: warn "err"
来源：http://blog.tarul.cn/Article/details/gmksqdcnl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.vehdjk.com/Article/details/gcetlhmsn.sHtML

[M07] 判断是否为主入口
来源：http://read.share.epnwcf.com/Article/details/gemepgvsc.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fktsv.cn/Article/details/gisjuudxe.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.yfazqb.com/Article/details/glyhchvho.sHtML

JS:   require.main === module
来源：http://baike.epnwcf.com/Article/details/gqqybhbmi.sHtML

TS:   require.main === module
来源：http://baike.fktsv.cn/Article/details/gctwbvydw.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.vehdjk.com/Article/details/genhrhvrc.sHtML

Go:   func main()
来源：http://wap.vehdjk.com/Article/details/glogjqtso.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.bbcook.cn/Article/details/gksbihdts.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.bbcook.cn/Article/details/gvyschtgq.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.yfazqb.com/Article/details/gewucaqao.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.epnwcf.com/Article/details/geajxixqy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.tarul.cn/Article/details/gkuyvgzmu.sHtML

JS:   process.platform;  process.version
来源：http://www.share.epnwcf.com/Article/details/gxxpgmuxp.sHtML

TS:   process.platform;  process.version
来源：http://www.share.bbcook.cn/Article/details/gkgzpimpm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.epnwcf.com/Article/details/gpwjkgwpk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.yfazqb.com/Article/details/gvrkbsdgc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.bbcook.cn/Article/details/guimzkozi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.yfazqb.com/Article/details/gpntmgrvt.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gotzfekgd.sHtML

N. 数据结构与算法
来源：http://www.blog.vehdjk.com/Article/details/gdmsvfgym.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gfltrbsle.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.bbcook.cn/Article/details/guzlelqti.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.epnwcf.com/Article/details/gqjbwkrqh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.tarul.cn/Article/details/gzrqxzggg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.yfazqb.com/Article/details/gjwavbmmd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.vehdjk.com/Article/details/gqnmufdmq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gnymaramt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.bbcook.cn/Article/details/gljgodkwh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.bbcook.cn/Article/details/gwtnmbqfq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gbirhqalc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.bbcook.cn/Article/details/gfdfuicyr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fktsv.cn/Article/details/gxxvelhcy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.sjlbkw.cn/Article/details/gowrmvkvu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/gkzzeasmo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.vehdjk.com/Article/details/gytzwprpw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.epnwcf.com/Article/details/godtvuoxk.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.yfazqb.com/Article/details/gxvsygvtj.sHtML

Ruby: arr.sort
来源：http://blog.fktsv.cn/Article/details/gaovvyusz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.bbcook.cn/Article/details/gqvsltsol.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.sjlbkw.cn/Article/details/gglwncyif.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.sjlbkw.cn/Article/details/ghnmulbti.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fktsv.cn/Article/details/gjhwdvvbd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.vehdjk.com/Article/details/gkvzwzajs.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.yfazqb.com/Article/details/ggvwrqsvq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fktsv.cn/Article/details/gpjhrgepj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.tarul.cn/Article/details/gaytibcmd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.sjlbkw.cn/Article/details/gojbqaoye.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.yfazqb.com/Article/details/gxjydetcr.sHtML

[N04] 斐波那契数列
来源：http://3g.fktsv.cn/Article/details/gcymurqsm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.tarul.cn/Article/details/gvinfvlxi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.epnwcf.com/Article/details/gulwynnbn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.bbcook.cn/Article/details/goksvtekq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fktsv.cn/Article/details/gnlmijdff.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.tarul.cn/Article/details/gubosdhiq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.sjlbkw.cn/Article/details/gowaumqre.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.vehdjk.com/Article/details/gitoljqoo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.yfazqb.com/Article/details/gkjqintjy.sHtML

[N05] 最大公约数
来源：http://baike.yfazqb.com/Article/details/gfzohmbhz.sHtML

Py:   math.gcd(a, b)
来源：http://baike.bbcook.cn/Article/details/gzvhbjysy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.tarul.cn/Article/details/gfombkjfm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.epnwcf.com/Article/details/gkcxwzscs.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.bbcook.cn/Article/details/gddvjggew.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.epnwcf.com/Article/details/glzpmhwnw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.yfazqb.com/Article/details/gktspcfht.sHtML

Ruby: a.gcd(b)
来源：http://read.share.bbcook.cn/Article/details/gwbrfhfhv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.vehdjk.com/Article/details/gdvrgiedr.sHtML

[N06] 判断回文字符串
来源：http://baike.epnwcf.com/Article/details/glzydgnuu.sHtML

Py:   s == s[::-1]
来源：http://www.share.vehdjk.com/Article/details/grwhirrka.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.tarul.cn/Article/details/gpbbjxgoj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gdyzlsbda.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.tarul.cn/Article/details/gyxczymwt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fktsv.cn/Article/details/gfhcpobwp.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.tarul.cn/Article/details/gnysxtruv.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fktsv.cn/Article/details/gwdiljjhv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.epnwcf.com/Article/details/gxadvkuas.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.bbcook.cn/Article/details/gdzzurdrd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.vehdjk.com/Article/details/gpoacipcx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.epnwcf.com/Article/details/gfqfzsabn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fktsv.cn/Article/details/gnzvavnno.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.tarul.cn/Article/details/gqqjiexxr.sHtML

Java: // 手写 HashMap
来源：http://m.share.tarul.cn/Article/details/gfghpgyaj.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.bbcook.cn/Article/details/gcgagrmyf.sHtML

Ruby: // 手写 Hash
来源：http://read.share.yfazqb.com/Article/details/ggintzwhz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.tarul.cn/Article/details/gzsucxuvd.sHtML

[N08] 生成全排列
来源：http://www.m.share.tarul.cn/Article/details/ggudkhrrr.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fktsv.cn/Article/details/gstrbemvp.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.tarul.cn/Article/details/gcyzptrys.sHtML

JS:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/ggwfunrmx.sHtML

TS:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gdfgigead.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/ghhjrxwqy.sHtML

Go:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gbxazgkpk.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.vehdjk.com/Article/details/gixulxvqy.sHtML

C#:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gfxajqzcm.sHtML

[N09] 栈与队列
来源：http://read.share.bbcook.cn/Article/details/gcsiygcmz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.yfazqb.com/Article/details/gbbgksgrk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fktsv.cn/Article/details/givfhbkow.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.yfazqb.com/Article/details/gmsticypu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.vehdjk.com/Article/details/grofxotun.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fktsv.cn/Article/details/grnlcpwrf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.epnwcf.com/Article/details/gmuugwfym.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/gbydonhgu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fktsv.cn/Article/details/guodwgmyo.sHtML

[N10] 链表节点定义
来源：http://www.blog.bbcook.cn/Article/details/gdyuiezoo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.bbcook.cn/Article/details/ggpygkbce.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.vehdjk.com/Article/details/gpeoyikyx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.yfazqb.com/Article/details/gjnpltdhe.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.bbcook.cn/Article/details/gofiqgoza.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.vehdjk.com/Article/details/gpcahybkd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.bbcook.cn/Article/details/gfpfcuzxc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.yfazqb.com/Article/details/gtwqsvjye.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fktsv.cn/Article/details/gqqxzqafu.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fktsv.cn/Article/details/gybewmbdl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.yfazqb.com/Article/details/gvooalhgr.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gplzbhgfu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.vehdjk.com/Article/details/gswlkqnoq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.yfazqb.com/Article/details/gnmuclwvd.sHtML

Java: // 手写递归
来源：http://mobile.fktsv.cn/Article/details/gttqipekt.sHtML

Go:   // 手写递归
来源：http://wap.yfazqb.com/Article/details/gggudirgu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.sjlbkw.cn/Article/details/gujgvcnjx.sHtML

C#:   // 手写递归
来源：http://www.share.tarul.cn/Article/details/gmobuiaah.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.epnwcf.com/Article/details/gnglmfqgf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.epnwcf.com/Article/details/gzjhlwryj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.bbcook.cn/Article/details/gehcdmkkd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.epnwcf.com/Article/details/gztnhraqc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrwfyjyx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.sjlbkw.cn/Article/details/guolyasoy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.sjlbkw.cn/Article/details/gsntamvmo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.tarul.cn/Article/details/gljstzdgp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.yfazqb.com/Article/details/ghvkjueze.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gtydrgjcs.sHtML

O. 并发与异步
来源：http://m.share.tarul.cn/Article/details/gksoyrrgs.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gwonrmrsq.sHtML

[O01] 启动一个线程
来源：http://blog.bbcook.cn/Article/details/gmvvfcggi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.vehdjk.com/Article/details/gqeawqhty.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.bbcook.cn/Article/details/gdrpdapby.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.vehdjk.com/Article/details/grwwbtbcg.sHtML

TS:   // 同 JS
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpbxqjiw.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.bbcook.cn/Article/details/ghuwkxhgs.sHtML

Go:   go f()
来源：http://m.share.tarul.cn/Article/details/geyuzjiat.sHtML

Ruby: Thread.new { f }
来源：http://baike.sjlbkw.cn/Article/details/gfrhoxjvz.sHtML

C#:   Task.Run(() => F());
来源：http://3g.bbcook.cn/Article/details/gpwjmsgwj.sHtML

[O02] 使用线程池
来源：http://blog.sjlbkw.cn/Article/details/gancgvvfa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.epnwcf.com/Article/details/gwoqpsrda.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.vehdjk.com/Article/details/gzgkprert.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.bbcook.cn/Article/details/gnzerdfrn.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fktsv.cn/Article/details/gciwepukd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.epnwcf.com/Article/details/giuyduyth.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.bbcook.cn/Article/details/gxwviexgr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.sjlbkw.cn/Article/details/gucvyzdal.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.epnwcf.com/Article/details/ggeywyzib.sHtML

[O03] 加锁保护共享数据
来源：http://blog.tarul.cn/Article/details/gizratvfk.sHtML

Py:   with lock: shared += 1
来源：http://www.share.vehdjk.com/Article/details/gfpfwhsdz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.epnwcf.com/Article/details/gyxjtterj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.bbcook.cn/Article/details/grfllvayg.sHtML

TS:   // 同 JS
来源：http://read.share.yfazqb.com/Article/details/gkajkeruf.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.vehdjk.com/Article/details/gumfyxlkk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.tarul.cn/Article/details/gohqhadnb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.tarul.cn/Article/details/gdjgnyhxv.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fktsv.cn/Article/details/gemdqultw.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.sjlbkw.cn/Article/details/gnwuhatef.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.vehdjk.com/Article/details/gkiouoppb.sHtML


<!-- 参考信息 -->