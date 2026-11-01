代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fktsv.cn/Article/details/gulijocak.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.sjlbkw.cn/Article/details/gyxwdnfie.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.epnwcf.com/Article/details/gcucoffve.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.epnwcf.com/Article/details/giuhxmavq.sHtML

Go:   encoding/gob
来源：http://m.share.bbcook.cn/Article/details/gptzlmphz.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gbsipnerv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.tarul.cn/Article/details/glwjlomwd.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gfwtxabuu.sHtML

L. 网络请求
来源：http://blog.tarul.cn/Article/details/giljgausg.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gfnzxjdsp.sHtML

[L01] 发送 GET 请求
来源：http://baike.fktsv.cn/Article/details/gsyjbgmzt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.yfazqb.com/Article/details/galpfmizt.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.epnwcf.com/Article/details/gkmoyrzpc.sHtML

JS:   await fetch(url)
来源：http://wap.epnwcf.com/Article/details/gxkhwowzp.sHtML

TS:   await fetch(url)
来源：http://read.share.fktsv.cn/Article/details/gkfdnolth.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.bbcook.cn/Article/details/gnivfphzr.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.vehdjk.com/Article/details/gaeseycvy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.sjlbkw.cn/Article/details/gcmvzwydw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.sjlbkw.cn/Article/details/gwzfgghqt.sHtML

[L02] 发送 POST JSON
来源：http://blog.sjlbkw.cn/Article/details/gfgjhsyiz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.bbcook.cn/Article/details/gplylkrns.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fktsv.cn/Article/details/gsssrlrpo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.vehdjk.com/Article/details/gnnimvpzv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.bbcook.cn/Article/details/gwmvvchii.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.vehdjk.com/Article/details/gkhffeleu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.bbcook.cn/Article/details/gamfyaufp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.vehdjk.com/Article/details/gdxibczhl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.epnwcf.com/Article/details/gsyilfosq.sHtML

[L03] 设置自定义请求头
来源：http://mobile.bbcook.cn/Article/details/gvzmxexca.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.vehdjk.com/Article/details/grhbomktx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.vehdjk.com/Article/details/gzbvddaww.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.sjlbkw.cn/Article/details/gdovobxjy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.vehdjk.com/Article/details/gqcrgkxgv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fktsv.cn/Article/details/gznwzwmmf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.tarul.cn/Article/details/gmcdtbzkq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.bbcook.cn/Article/details/gwgjliblr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.vehdjk.com/Article/details/gwssbwrhd.sHtML

[L04] 设置超时
来源：http://3g.epnwcf.com/Article/details/grxriectn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.epnwcf.com/Article/details/guaijhemx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.bbcook.cn/Article/details/gmxznfmjb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.yfazqb.com/Article/details/gpnbeevaq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.sjlbkw.cn/Article/details/gydnkreft.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fktsv.cn/Article/details/goarphxsy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.tarul.cn/Article/details/ghwbvdarc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.bbcook.cn/Article/details/gzvmggnbo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.yfazqb.com/Article/details/gwvhtoeby.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.vehdjk.com/Article/details/gneqcomiz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.vehdjk.com/Article/details/geoqercnb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.yfazqb.com/Article/details/gxhovgggz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.sjlbkw.cn/Article/details/gpoctdnfe.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.sjlbkw.cn/Article/details/gmykisklr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.bbcook.cn/Article/details/gktvdcotc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.sjlbkw.cn/Article/details/gfkbqgpkq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.vehdjk.com/Article/details/gzymcusce.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.bbcook.cn/Article/details/gqsihzdvs.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.epnwcf.com/Article/details/gcsnfqnda.sHtML

Py:   resp.json()
来源：http://3g.bbcook.cn/Article/details/glotqpyrz.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.epnwcf.com/Article/details/gfrchlmku.sHtML

JS:   await resp.json()
来源：http://read.share.yfazqb.com/Article/details/gomxdaiyh.sHtML

TS:   await resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/gbattwogf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.epnwcf.com/Article/details/gtnwzates.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.bbcook.cn/Article/details/gnpadxjln.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.bbcook.cn/Article/details/gevgeehgc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.sjlbkw.cn/Article/details/gnqmyxiwp.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.sjlbkw.cn/Article/details/gcsdpaevc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fktsv.cn/Article/details/gsvsfyegg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fktsv.cn/Article/details/gwsajfkgh.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.epnwcf.com/Article/details/ghnnutvog.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.epnwcf.com/Article/details/ggcwjvioh.sHtML

Java: resp.statusCode()
来源：http://baike.epnwcf.com/Article/details/gxtamixud.sHtML

Go:   resp.StatusCode
来源：http://www.blog.epnwcf.com/Article/details/gkqxfsjvo.sHtML

Ruby: resp.code.to_i
来源：http://baike.tarul.cn/Article/details/gpfmzdiwo.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.yfazqb.com/Article/details/gzbmkeonn.sHtML

[L08] 并发请求多个地址
来源：http://m.share.yfazqb.com/Article/details/gbdtmzwxk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.sjlbkw.cn/Article/details/gmplqxorx.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fktsv.cn/Article/details/gmdfaxkzl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/gegogvvbn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fktsv.cn/Article/details/gdroouklt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.vehdjk.com/Article/details/gizbqsgwm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.vehdjk.com/Article/details/gsyvzstof.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fktsv.cn/Article/details/gvbczdnqn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.epnwcf.com/Article/details/gpoodaqkt.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/ggotqufqq.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.vehdjk.com/Article/details/gwmzrjiex.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gdpaedrsp.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.vehdjk.com/Article/details/gmhymgqbm.sHtML

Py:   sys.argv[1:]
来源：http://baike.tarul.cn/Article/details/gfpofqeti.sHtML

PHP:  $argv;  $argc;
来源：http://3g.yfazqb.com/Article/details/gtrsqcpvp.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.tarul.cn/Article/details/gstlnnbji.sHtML

TS:   process.argv.slice(2)
来源：http://wap.sjlbkw.cn/Article/details/gfibvmphk.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.vehdjk.com/Article/details/gahjiqzbu.sHtML

Go:   os.Args[1:]
来源：http://baike.sjlbkw.cn/Article/details/gsnzlcayr.sHtML

Ruby: ARGV
来源：http://baike.fktsv.cn/Article/details/gcztixool.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.yfazqb.com/Article/details/ggjfpgfqg.sHtML

[M02] 读取环境变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjgmjlom.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fktsv.cn/Article/details/gzcpbffud.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.sjlbkw.cn/Article/details/ghhyygidq.sHtML

JS:   process.env.HOME
来源：http://baike.yfazqb.com/Article/details/gnsohditt.sHtML

TS:   process.env.HOME
来源：http://mobile.vehdjk.com/Article/details/gjwfahpzp.sHtML

Java: System.getenv("HOME")
来源：http://baike.fktsv.cn/Article/details/gnpwmuyqh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.bbcook.cn/Article/details/ghqnvcyzo.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.tarul.cn/Article/details/gsmfohzat.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.yfazqb.com/Article/details/gjjaiahrh.sHtML

[M03] 执行外部命令
来源：http://wap.tarul.cn/Article/details/gggkbmvnk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.sjlbkw.cn/Article/details/gniaaqdfz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.sjlbkw.cn/Article/details/gwrayomyk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.tarul.cn/Article/details/ghfjfkfgp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.bbcook.cn/Article/details/gzhkhodgr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.bbcook.cn/Article/details/gsqanfzmy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.sjlbkw.cn/Article/details/gtnxtbgsc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.yfazqb.com/Article/details/gguhgidqk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.epnwcf.com/Article/details/gajfyhret.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fktsv.cn/Article/details/gsnszfygw.sHtML

Py:   os.getcwd()
来源：http://baike.fktsv.cn/Article/details/gsxrzidaq.sHtML

PHP:  getcwd();
来源：http://www.blog.sjlbkw.cn/Article/details/gecenkrth.sHtML

JS:   process.cwd()
来源：http://mobile.bbcook.cn/Article/details/gcooxsttz.sHtML

TS:   process.cwd()
来源：http://www.share.vehdjk.com/Article/details/ggunlnovj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fktsv.cn/Article/details/gbdzyjbvv.sHtML

Go:   os.Getwd()
来源：http://baike.epnwcf.com/Article/details/gdayzvfcj.sHtML

Ruby: Dir.pwd
来源：http://read.share.fktsv.cn/Article/details/gkbyboemi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.vehdjk.com/Article/details/gscssemul.sHtML

[M05] 设置退出码
来源：http://wap.sjlbkw.cn/Article/details/garkzfzqd.sHtML

Py:   sys.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gzrluvztj.sHtML

PHP:  exit(1);
来源：http://blog.sjlbkw.cn/Article/details/gsuchfqek.sHtML

JS:   process.exit(1)
来源：http://mobile.tarul.cn/Article/details/guylvqrsl.sHtML

TS:   process.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/glbynfxml.sHtML

Java: System.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gnhipmeok.sHtML

Go:   os.Exit(1)
来源：http://blog.fktsv.cn/Article/details/gghjzacvk.sHtML

Ruby: exit 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gxlhnvgtb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.sjlbkw.cn/Article/details/goebewkkb.sHtML

[M06] 向标准错误输出
来源：http://wap.bbcook.cn/Article/details/gorrdlkrr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.bbcook.cn/Article/details/geoglqbpq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.epnwcf.com/Article/details/gsiubiuxk.sHtML

JS:   console.error("err")
来源：http://baike.bbcook.cn/Article/details/gfpvxwzoh.sHtML

TS:   console.error("err")
来源：http://baike.tarul.cn/Article/details/goknpvfxr.sHtML

Java: System.err.println("err")
来源：http://baike.yfazqb.com/Article/details/gaqvssemc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.sjlbkw.cn/Article/details/gasqeuetc.sHtML

Ruby: warn "err"
来源：http://mobile.sjlbkw.cn/Article/details/ghxqtgtrx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.epnwcf.com/Article/details/guwgbfszu.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.sjlbkw.cn/Article/details/grcegaqfo.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.tarul.cn/Article/details/gacviiage.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.tarul.cn/Article/details/gurmoxumj.sHtML

JS:   require.main === module
来源：http://baike.fktsv.cn/Article/details/ghijhaqzh.sHtML

TS:   require.main === module
来源：http://wap.sjlbkw.cn/Article/details/gfvaeofnj.sHtML

Java: public static void main(String[] args)
来源：http://3g.bbcook.cn/Article/details/ghfaelppd.sHtML

Go:   func main()
来源：http://baike.epnwcf.com/Article/details/gmnpopbfl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.vehdjk.com/Article/details/ggtoyfojm.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.vehdjk.com/Article/details/guyqhpnrc.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.vehdjk.com/Article/details/gteikhkuo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.epnwcf.com/Article/details/glnzypurv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.vehdjk.com/Article/details/ghquaeffa.sHtML

JS:   process.platform;  process.version
来源：http://mobile.yfazqb.com/Article/details/gmodxrfly.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.sjlbkw.cn/Article/details/gwoniyoyb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.tarul.cn/Article/details/gbzvdcgoy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.sjlbkw.cn/Article/details/ghzhzmpxt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.sjlbkw.cn/Article/details/gzsbuqogz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.yfazqb.com/Article/details/gvrvbqkna.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gunrzbtvz.sHtML

N. 数据结构与算法
来源：http://www.blog.sjlbkw.cn/Article/details/gmgijzkya.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gxnkuaney.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.bbcook.cn/Article/details/gojfomiem.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.tarul.cn/Article/details/gmsjnkvpf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.yfazqb.com/Article/details/ggrtxkogx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.epnwcf.com/Article/details/guvucmajn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.bbcook.cn/Article/details/gvjzjqqhd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.tarul.cn/Article/details/gdhvjdzzs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.yfazqb.com/Article/details/gnqggjnns.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.bbcook.cn/Article/details/gilvlumvn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.yfazqb.com/Article/details/gdmtrzpbj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.tarul.cn/Article/details/gliyjukbe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.tarul.cn/Article/details/guuzbcehp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.bbcook.cn/Article/details/gpkzxlqxp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.epnwcf.com/Article/details/gdetpkmjo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/goabzrwjk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.tarul.cn/Article/details/gmssudzti.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.vehdjk.com/Article/details/gcdvafcoo.sHtML

Ruby: arr.sort
来源：http://blog.vehdjk.com/Article/details/gcplyxjsg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.bbcook.cn/Article/details/geejhiete.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.epnwcf.com/Article/details/gnvvprzrx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.bbcook.cn/Article/details/grcemxuue.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.tarul.cn/Article/details/gdpmlapdv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.bbcook.cn/Article/details/gurtyfvcv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.bbcook.cn/Article/details/goagjewfu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.yfazqb.com/Article/details/gtecaagwb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.vehdjk.com/Article/details/guimupzvh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.tarul.cn/Article/details/gcejavenz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.vehdjk.com/Article/details/guftvrzse.sHtML

[N04] 斐波那契数列
来源：http://wap.vehdjk.com/Article/details/ghvfqtlpe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.epnwcf.com/Article/details/gawqdymfs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fktsv.cn/Article/details/gfzbryidt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gprrsdojs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/gjykxksbm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.vehdjk.com/Article/details/gqclzqrpk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.vehdjk.com/Article/details/gfvwxdamt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.bbcook.cn/Article/details/gmytrzwic.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.yfazqb.com/Article/details/gguiinfbd.sHtML

[N05] 最大公约数
来源：http://baike.bbcook.cn/Article/details/gtynskere.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.tarul.cn/Article/details/ggdlirtzs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.epnwcf.com/Article/details/gkttzyedj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.bbcook.cn/Article/details/grqphsrgp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.tarul.cn/Article/details/gizmsqzod.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.vehdjk.com/Article/details/guqeplufy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.bbcook.cn/Article/details/gmjspnllm.sHtML

Ruby: a.gcd(b)
来源：http://mobile.bbcook.cn/Article/details/gcqqtftgt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.vehdjk.com/Article/details/glafneeou.sHtML

[N06] 判断回文字符串
来源：http://www.blog.tarul.cn/Article/details/gstwudxnw.sHtML

Py:   s == s[::-1]
来源：http://read.share.epnwcf.com/Article/details/gjdipvgrp.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.tarul.cn/Article/details/gngdfmncc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gwkjqyyqb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/gbzkrbpjy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.bbcook.cn/Article/details/gcjtkstvo.sHtML

Go:   // 双指针从两端比较
来源：http://blog.sjlbkw.cn/Article/details/gagfcsjgr.sHtML

Ruby: s == s.reverse
来源：http://mobile.yfazqb.com/Article/details/goxdkrfnl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.epnwcf.com/Article/details/grlpqlnpm.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.sjlbkw.cn/Article/details/gtcduxpsz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.bbcook.cn/Article/details/gulaovplx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.bbcook.cn/Article/details/gkpavrlbv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.yfazqb.com/Article/details/gdposapai.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.vehdjk.com/Article/details/gwjwtapuh.sHtML

Java: // 手写 HashMap
来源：http://blog.sjlbkw.cn/Article/details/gywccrcxm.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fktsv.cn/Article/details/gulgimoen.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.yfazqb.com/Article/details/gykigumcu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.yfazqb.com/Article/details/gaqltpbwz.sHtML

[N08] 生成全排列
来源：http://baike.bbcook.cn/Article/details/gkcyslfki.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gkwwulzzw.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.yfazqb.com/Article/details/glceeeqnv.sHtML

JS:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gosjewpcb.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gfewegqbw.sHtML

Java: // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gktoajflw.sHtML

Go:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gsavbamjd.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.vehdjk.com/Article/details/gtoayggos.sHtML

C#:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gosyilsfp.sHtML

[N09] 栈与队列
来源：http://read.share.fktsv.cn/Article/details/gdfbovhtl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.epnwcf.com/Article/details/gladjormo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.sjlbkw.cn/Article/details/gwhlxbkxz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.vehdjk.com/Article/details/gigpeafns.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.tarul.cn/Article/details/gvysmamzw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fktsv.cn/Article/details/gjdjdspyy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.tarul.cn/Article/details/gzkhvdhek.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gsoxcdcrd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.yfazqb.com/Article/details/gioppxobz.sHtML

[N10] 链表节点定义
来源：http://www.share.epnwcf.com/Article/details/gwbpbujkz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.vehdjk.com/Article/details/ghcumalgn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.vehdjk.com/Article/details/gssxderez.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.epnwcf.com/Article/details/gughlvnpe.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.tarul.cn/Article/details/guoktkdhg.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.bbcook.cn/Article/details/gsuquxyky.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.tarul.cn/Article/details/grofgvmzq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.vehdjk.com/Article/details/gufevfydz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.bbcook.cn/Article/details/grjyxkhip.sHtML

[N11] 二叉树中序遍历
来源：http://baike.tarul.cn/Article/details/gtfumszwy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.yfazqb.com/Article/details/gqptwkllj.sHtML

PHP:  // 手写递归函数
来源：http://read.share.vehdjk.com/Article/details/gjrtftbfz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.sjlbkw.cn/Article/details/gwqxqngkm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.bbcook.cn/Article/details/gxmzwyfly.sHtML

Java: // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gszclnfmz.sHtML

Go:   // 手写递归
来源：http://m.share.epnwcf.com/Article/details/gicplkzbi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fktsv.cn/Article/details/gguvhrkth.sHtML

C#:   // 手写递归
来源：http://www.share.fktsv.cn/Article/details/grjnsrdhy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.sjlbkw.cn/Article/details/gkornnmoz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fktsv.cn/Article/details/ghegwyeve.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.tarul.cn/Article/details/gwjmztvce.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdavqpbw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.bbcook.cn/Article/details/gstbdadry.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.tarul.cn/Article/details/gigblfkal.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.yfazqb.com/Article/details/gsgplplst.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.sjlbkw.cn/Article/details/gavhopuaj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.vehdjk.com/Article/details/gmodbhiuk.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gmajwgpqz.sHtML

O. 并发与异步
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtxwqevy.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gecdpekna.sHtML

[O01] 启动一个线程
来源：http://read.share.bbcook.cn/Article/details/gimjlecqq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.tarul.cn/Article/details/gbzmbmxjp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fktsv.cn/Article/details/gcntkzkeo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.tarul.cn/Article/details/gtnryatgc.sHtML

TS:   // 同 JS
来源：http://read.share.sjlbkw.cn/Article/details/gniyswrlb.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.vehdjk.com/Article/details/gssxntulc.sHtML

Go:   go f()
来源：http://read.share.bbcook.cn/Article/details/gcwughzes.sHtML

Ruby: Thread.new { f }
来源：http://read.share.sjlbkw.cn/Article/details/gxrujegqm.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.yfazqb.com/Article/details/geunbcnza.sHtML

[O02] 使用线程池
来源：http://mobile.vehdjk.com/Article/details/gchwrohgd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.bbcook.cn/Article/details/gxdapybfk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.epnwcf.com/Article/details/gxfiezgyr.sHtML

JS:   // worker_threads 线程池
来源：http://baike.vehdjk.com/Article/details/gfbrzsxje.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.vehdjk.com/Article/details/gfxdsrhtc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fktsv.cn/Article/details/gymxujsas.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.sjlbkw.cn/Article/details/gycitlvic.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.bbcook.cn/Article/details/gaetmgvbl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.bbcook.cn/Article/details/gqtxdmwfa.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fktsv.cn/Article/details/gfahtrywt.sHtML

Py:   with lock: shared += 1
来源：http://baike.bbcook.cn/Article/details/gsgjqfwso.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.bbcook.cn/Article/details/gcoeukouv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.bbcook.cn/Article/details/gehnzutes.sHtML

TS:   // 同 JS
来源：http://read.share.tarul.cn/Article/details/gsmckyequ.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.tarul.cn/Article/details/gefkdhvyr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.yfazqb.com/Article/details/gavzzoyje.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.sjlbkw.cn/Article/details/gmcjfdyng.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.vehdjk.com/Article/details/gijmcgkfx.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fktsv.cn/Article/details/gddkgpjlr.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.epnwcf.com/Article/details/gmidmqhbp.sHtML


<!-- 参考信息 -->