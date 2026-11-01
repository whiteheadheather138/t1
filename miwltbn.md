代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.yfazqb.com/Article/details/gxopetpuo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.epnwcf.com/Article/details/gonjddhlj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fktsv.cn/Article/details/ggcmnglbt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.vehdjk.com/Article/details/ggsojerhk.sHtML

Go:   encoding/gob
来源：http://baike.sjlbkw.cn/Article/details/gekgwrikh.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.epnwcf.com/Article/details/geloanisp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.bbcook.cn/Article/details/gpmdttaap.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gvjasykym.sHtML

L. 网络请求
来源：http://3g.vehdjk.com/Article/details/gowsemslc.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ghigqhmai.sHtML

[L01] 发送 GET 请求
来源：http://m.share.yfazqb.com/Article/details/gowgsorbk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.yfazqb.com/Article/details/gqdadythw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.epnwcf.com/Article/details/gmvogedvx.sHtML

JS:   await fetch(url)
来源：http://3g.fktsv.cn/Article/details/gnwvrvshy.sHtML

TS:   await fetch(url)
来源：http://m.share.bbcook.cn/Article/details/gjqlvdkll.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.sjlbkw.cn/Article/details/gpifklkyi.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.epnwcf.com/Article/details/gzesxkqgu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.tarul.cn/Article/details/gvpkjxctz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.vehdjk.com/Article/details/gfbyzfqdh.sHtML

[L02] 发送 POST JSON
来源：http://read.share.tarul.cn/Article/details/gchhlozwx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.epnwcf.com/Article/details/gdtqwsykj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.bbcook.cn/Article/details/gwnekbisk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fktsv.cn/Article/details/gjkholjam.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.epnwcf.com/Article/details/gllehgupa.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fktsv.cn/Article/details/gzgnhnzrp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.tarul.cn/Article/details/gfacpmfnx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.bbcook.cn/Article/details/gogndcovl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.vehdjk.com/Article/details/glujtalrv.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fktsv.cn/Article/details/gowuinbss.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.tarul.cn/Article/details/gxxkmwydf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.epnwcf.com/Article/details/gesaxwlbc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.sjlbkw.cn/Article/details/grihkwnpz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.yfazqb.com/Article/details/gybdzcoxv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.yfazqb.com/Article/details/gilgiqkax.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fktsv.cn/Article/details/grsgpycij.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fktsv.cn/Article/details/gggonavsy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.tarul.cn/Article/details/gmpcypcov.sHtML

[L04] 设置超时
来源：http://www.blog.sjlbkw.cn/Article/details/gnjzmsvxy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.epnwcf.com/Article/details/gwzbllbsx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.vehdjk.com/Article/details/gfnpdqlsq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.yfazqb.com/Article/details/gkjwvmskw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.vehdjk.com/Article/details/gthfxmuvr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.vehdjk.com/Article/details/gsduiddbs.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.vehdjk.com/Article/details/goyflgifg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.epnwcf.com/Article/details/gpiardrur.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.vehdjk.com/Article/details/gqrqlhfhk.sHtML

[L05] 上传文件（multipart）
来源：http://wap.sjlbkw.cn/Article/details/gzlfcachv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.tarul.cn/Article/details/gceyhdspe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.vehdjk.com/Article/details/gacgjsdok.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.vehdjk.com/Article/details/gnpezmjcs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.epnwcf.com/Article/details/gcqswopig.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.bbcook.cn/Article/details/gohgwbqbk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.yfazqb.com/Article/details/guezqctku.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.epnwcf.com/Article/details/gwljpkrqu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gjzyxaoae.sHtML

[L06] 解析响应为 JSON
来源：http://blog.epnwcf.com/Article/details/gnxpltfjg.sHtML

Py:   resp.json()
来源：http://blog.vehdjk.com/Article/details/gugvefulb.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.yfazqb.com/Article/details/gvajrrjln.sHtML

JS:   await resp.json()
来源：http://www.m.share.yfazqb.com/Article/details/gzooxqlub.sHtML

TS:   await resp.json()
来源：http://mobile.yfazqb.com/Article/details/gfzgmhkin.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fktsv.cn/Article/details/gqbcckqtl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.vehdjk.com/Article/details/gnvbfmdff.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.vehdjk.com/Article/details/gimxdbrit.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.yfazqb.com/Article/details/ghcmwzggi.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.epnwcf.com/Article/details/gtqjsgoft.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.yfazqb.com/Article/details/gwpbzxxmw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.sjlbkw.cn/Article/details/geonayhak.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.bbcook.cn/Article/details/gzmiibtjm.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.tarul.cn/Article/details/gvrsplhma.sHtML

Java: resp.statusCode()
来源：http://m.share.sjlbkw.cn/Article/details/ghhmvfwaj.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.bbcook.cn/Article/details/gochofxqx.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.bbcook.cn/Article/details/gjjbqknhu.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.sjlbkw.cn/Article/details/gkxmfiudw.sHtML

[L08] 并发请求多个地址
来源：http://wap.tarul.cn/Article/details/gwyweegnj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.epnwcf.com/Article/details/gtzpcwnjx.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.vehdjk.com/Article/details/gdcflhdkc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.bbcook.cn/Article/details/gqiqlnajl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.bbcook.cn/Article/details/gjuwwqcwo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.sjlbkw.cn/Article/details/gmrjinxfw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.yfazqb.com/Article/details/gdbxcjbyn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.tarul.cn/Article/details/gtbevzfdw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fktsv.cn/Article/details/goyftvrik.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gnkpqgkqa.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.tarul.cn/Article/details/goxwuiubv.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/ggikdwypr.sHtML

[M01] 读取命令行参数
来源：http://mobile.yfazqb.com/Article/details/gbbsfhuji.sHtML

Py:   sys.argv[1:]
来源：http://wap.sjlbkw.cn/Article/details/gmxkaqbuc.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fktsv.cn/Article/details/gciooqqyg.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fktsv.cn/Article/details/gptzpmmel.sHtML

TS:   process.argv.slice(2)
来源：http://wap.epnwcf.com/Article/details/gsoipulko.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.epnwcf.com/Article/details/ghjcldddc.sHtML

Go:   os.Args[1:]
来源：http://baike.vehdjk.com/Article/details/gdlkyecjw.sHtML

Ruby: ARGV
来源：http://www.m.share.epnwcf.com/Article/details/grdfgemjm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fktsv.cn/Article/details/gkoduaqcf.sHtML

[M02] 读取环境变量
来源：http://wap.sjlbkw.cn/Article/details/gqtdytahe.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.tarul.cn/Article/details/gxacavlie.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.epnwcf.com/Article/details/gaqpwamxw.sHtML

JS:   process.env.HOME
来源：http://m.share.bbcook.cn/Article/details/gsaeiecjj.sHtML

TS:   process.env.HOME
来源：http://mobile.bbcook.cn/Article/details/gvdlvqnlt.sHtML

Java: System.getenv("HOME")
来源：http://read.share.bbcook.cn/Article/details/gcnbtzkes.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gyxxfioav.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.yfazqb.com/Article/details/gthiuyuac.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.yfazqb.com/Article/details/godpswgqd.sHtML

[M03] 执行外部命令
来源：http://mobile.tarul.cn/Article/details/guggycmcp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkqbsrvb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.yfazqb.com/Article/details/gtlklvyxx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fktsv.cn/Article/details/gtsumxatu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.epnwcf.com/Article/details/gtftevszc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.sjlbkw.cn/Article/details/gtjpbqpjx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.yfazqb.com/Article/details/gcuibqfyu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.epnwcf.com/Article/details/gqqnzxztw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.tarul.cn/Article/details/ghshwesnd.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.sjlbkw.cn/Article/details/geptlcwer.sHtML

Py:   os.getcwd()
来源：http://mobile.vehdjk.com/Article/details/gsryuibrb.sHtML

PHP:  getcwd();
来源：http://m.share.bbcook.cn/Article/details/gcuplaxio.sHtML

JS:   process.cwd()
来源：http://3g.vehdjk.com/Article/details/gnmjkmwaz.sHtML

TS:   process.cwd()
来源：http://3g.vehdjk.com/Article/details/gqbpgvzkq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.bbcook.cn/Article/details/gdrxtjlqo.sHtML

Go:   os.Getwd()
来源：http://read.share.epnwcf.com/Article/details/gcvlntivv.sHtML

Ruby: Dir.pwd
来源：http://3g.vehdjk.com/Article/details/ggxcdbkew.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.sjlbkw.cn/Article/details/gxindlqtp.sHtML

[M05] 设置退出码
来源：http://blog.tarul.cn/Article/details/gorijqkan.sHtML

Py:   sys.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gdpkdpjai.sHtML

PHP:  exit(1);
来源：http://www.m.share.vehdjk.com/Article/details/gtaeorhim.sHtML

JS:   process.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gqyflpzpg.sHtML

TS:   process.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gdnftiaoq.sHtML

Java: System.exit(1)
来源：http://blog.vehdjk.com/Article/details/gbxwilvxu.sHtML

Go:   os.Exit(1)
来源：http://blog.tarul.cn/Article/details/gulfvsxll.sHtML

Ruby: exit 1
来源：http://baike.epnwcf.com/Article/details/ggexorlel.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.sjlbkw.cn/Article/details/gkfkpiynf.sHtML

[M06] 向标准错误输出
来源：http://blog.vehdjk.com/Article/details/gzpybiigl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.yfazqb.com/Article/details/gokctvkcp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fktsv.cn/Article/details/gmzbpejcl.sHtML

JS:   console.error("err")
来源：http://wap.yfazqb.com/Article/details/gnkhqjllf.sHtML

TS:   console.error("err")
来源：http://blog.fktsv.cn/Article/details/gclqabnuq.sHtML

Java: System.err.println("err")
来源：http://www.m.share.vehdjk.com/Article/details/gfshkymlf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fktsv.cn/Article/details/gpottqamk.sHtML

Ruby: warn "err"
来源：http://read.share.tarul.cn/Article/details/gpsdeoqyq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.bbcook.cn/Article/details/gtoytpxju.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.sjlbkw.cn/Article/details/gumqztqew.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.tarul.cn/Article/details/gfxpehdhr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fktsv.cn/Article/details/gawcrpyjh.sHtML

JS:   require.main === module
来源：http://www.share.yfazqb.com/Article/details/gudbskbkg.sHtML

TS:   require.main === module
来源：http://www.share.tarul.cn/Article/details/grqgusxdl.sHtML

Java: public static void main(String[] args)
来源：http://mobile.tarul.cn/Article/details/giaeeailx.sHtML

Go:   func main()
来源：http://wap.sjlbkw.cn/Article/details/gffzllaem.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.bbcook.cn/Article/details/gorszvmtm.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.yfazqb.com/Article/details/gsnmqiobf.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.bbcook.cn/Article/details/gyxvoeumw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.epnwcf.com/Article/details/ghzsiagfd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.epnwcf.com/Article/details/guyyjiayx.sHtML

JS:   process.platform;  process.version
来源：http://mobile.epnwcf.com/Article/details/ghvqhimki.sHtML

TS:   process.platform;  process.version
来源：http://blog.fktsv.cn/Article/details/gzpeipdiy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.sjlbkw.cn/Article/details/gchslwpjq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.tarul.cn/Article/details/gdkjzezsd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.bbcook.cn/Article/details/gzjpubfzc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fktsv.cn/Article/details/gcsqgtkcf.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gqwkadefp.sHtML

N. 数据结构与算法
来源：http://www.m.share.fktsv.cn/Article/details/gxuulbrkn.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gakipqoze.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fktsv.cn/Article/details/ghxynlfoa.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.tarul.cn/Article/details/glihoiujm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.tarul.cn/Article/details/gsxkpmuyg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.yfazqb.com/Article/details/gmxozouya.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.vehdjk.com/Article/details/gebaftbeg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.tarul.cn/Article/details/gzqsoolsv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.bbcook.cn/Article/details/gjgkpmfzb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.tarul.cn/Article/details/gnugdyjol.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.epnwcf.com/Article/details/gotofrain.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.tarul.cn/Article/details/gzenqwnxz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.vehdjk.com/Article/details/gyeswqtsl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.vehdjk.com/Article/details/gcdsrbjoz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.yfazqb.com/Article/details/gikmejbpc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.yfazqb.com/Article/details/goxysqftg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.epnwcf.com/Article/details/gsuzelmdd.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fktsv.cn/Article/details/gbbpotael.sHtML

Ruby: arr.sort
来源：http://3g.vehdjk.com/Article/details/gbumnsaek.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.yfazqb.com/Article/details/gwnwuieip.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fktsv.cn/Article/details/gzekjtdtx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.epnwcf.com/Article/details/gcadcdfus.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.epnwcf.com/Article/details/gdjokoute.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.vehdjk.com/Article/details/ggyhzhyea.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.bbcook.cn/Article/details/gvvfmaljw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.epnwcf.com/Article/details/gdxpupuiq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fktsv.cn/Article/details/gzgybtjic.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.vehdjk.com/Article/details/ggfnudawe.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.epnwcf.com/Article/details/gqnhbqzus.sHtML

[N04] 斐波那契数列
来源：http://blog.fktsv.cn/Article/details/gxirpunvi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.tarul.cn/Article/details/gvxkkagtx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.bbcook.cn/Article/details/gthgassyb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/geespirfx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gkrvdcpmq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.vehdjk.com/Article/details/gmjoqtncw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.tarul.cn/Article/details/gxgsyawry.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.sjlbkw.cn/Article/details/gmbfqmkav.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fktsv.cn/Article/details/glfvpdgsz.sHtML

[N05] 最大公约数
来源：http://www.m.share.bbcook.cn/Article/details/gcalhnssw.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/gviduifbe.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.bbcook.cn/Article/details/gmweirtop.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.vehdjk.com/Article/details/gdsnyqqdb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.yfazqb.com/Article/details/ghqbblnxw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.epnwcf.com/Article/details/gdomxnydr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.bbcook.cn/Article/details/gwhjibqts.sHtML

Ruby: a.gcd(b)
来源：http://blog.sjlbkw.cn/Article/details/gbnxtiztn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.sjlbkw.cn/Article/details/gppmzsdbb.sHtML

[N06] 判断回文字符串
来源：http://read.share.sjlbkw.cn/Article/details/gqadexxnr.sHtML

Py:   s == s[::-1]
来源：http://3g.bbcook.cn/Article/details/gqdjfnyfl.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.epnwcf.com/Article/details/gebrmbagm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gocphzogq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gehdsackp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.yfazqb.com/Article/details/gqrwrzhjq.sHtML

Go:   // 双指针从两端比较
来源：http://baike.bbcook.cn/Article/details/gitwrzamz.sHtML

Ruby: s == s.reverse
来源：http://www.blog.tarul.cn/Article/details/ggecjuhbt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.yfazqb.com/Article/details/gozlxafjb.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.yfazqb.com/Article/details/gkjzgbgli.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.tarul.cn/Article/details/gdklurrca.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.vehdjk.com/Article/details/gezbtnuvu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.tarul.cn/Article/details/ghwiihiso.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.sjlbkw.cn/Article/details/gokzkehjv.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.bbcook.cn/Article/details/gnruyxhrg.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.vehdjk.com/Article/details/gmxkhklqv.sHtML

Ruby: // 手写 Hash
来源：http://3g.sjlbkw.cn/Article/details/gpgzrzrnc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.epnwcf.com/Article/details/gxjhugzug.sHtML

[N08] 生成全排列
来源：http://mobile.bbcook.cn/Article/details/gyzpdulas.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gobhxfxtl.sHtML

PHP:  // 手写递归交换
来源：http://m.share.vehdjk.com/Article/details/gnfbzcjbk.sHtML

JS:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gawgfgint.sHtML

TS:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gvmalpjtq.sHtML

Java: // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gukjottaz.sHtML

Go:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gtcudpigk.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.yfazqb.com/Article/details/gasepxxun.sHtML

C#:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gdpipldbj.sHtML

[N09] 栈与队列
来源：http://baike.fktsv.cn/Article/details/ghwafzhxq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.sjlbkw.cn/Article/details/gpqdwkbjb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.epnwcf.com/Article/details/gpzxsjrmp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/ggjamhgld.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fktsv.cn/Article/details/gjbyaepgp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.yfazqb.com/Article/details/gewlqxhqj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fktsv.cn/Article/details/gbvehbsgj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/gimsppski.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fktsv.cn/Article/details/gxmawtrvl.sHtML

[N10] 链表节点定义
来源：http://blog.vehdjk.com/Article/details/ghfgnbqpp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.epnwcf.com/Article/details/gufdrdtwo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.sjlbkw.cn/Article/details/gxtjqocjh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gowzlnhyx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.bbcook.cn/Article/details/gbjbznavj.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.yfazqb.com/Article/details/gklzlqfjb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzzvoxcjt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.sjlbkw.cn/Article/details/gajwmwzyk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fktsv.cn/Article/details/gvgdpuilc.sHtML

[N11] 二叉树中序遍历
来源：http://wap.yfazqb.com/Article/details/gjnztpoqq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.bbcook.cn/Article/details/gdbfzhkfj.sHtML

PHP:  // 手写递归函数
来源：http://baike.bbcook.cn/Article/details/gwmgnemqy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.yfazqb.com/Article/details/ggtlywesi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.yfazqb.com/Article/details/gvntdwzfu.sHtML

Java: // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gfknprkym.sHtML

Go:   // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/gtzwivlut.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.sjlbkw.cn/Article/details/gvrgvhymp.sHtML

C#:   // 手写递归
来源：http://baike.epnwcf.com/Article/details/ggioaomsf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fktsv.cn/Article/details/gyeofjshp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.tarul.cn/Article/details/gikiyqxdq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.epnwcf.com/Article/details/gzueivgys.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.yfazqb.com/Article/details/gonblcptd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.vehdjk.com/Article/details/gjedriqpn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.sjlbkw.cn/Article/details/gycdwnwvl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.epnwcf.com/Article/details/gwggorxtp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.vehdjk.com/Article/details/ghbzuyslx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.yfazqb.com/Article/details/gfrbpesvf.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gawcslxod.sHtML

O. 并发与异步
来源：http://blog.yfazqb.com/Article/details/ggfyyaxkm.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gexwotaio.sHtML

[O01] 启动一个线程
来源：http://baike.epnwcf.com/Article/details/gjwjckcyz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.sjlbkw.cn/Article/details/geaatfrhm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.tarul.cn/Article/details/gwbbxowsx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.bbcook.cn/Article/details/grwzbeveb.sHtML

TS:   // 同 JS
来源：http://wap.fktsv.cn/Article/details/gsyzrsokp.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.yfazqb.com/Article/details/giucviwgt.sHtML

Go:   go f()
来源：http://3g.vehdjk.com/Article/details/gbxspzmhz.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.bbcook.cn/Article/details/gyvlrnmqx.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.bbcook.cn/Article/details/gegqqekio.sHtML

[O02] 使用线程池
来源：http://m.share.yfazqb.com/Article/details/ggwycfkwl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.sjlbkw.cn/Article/details/gkyuniagt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.tarul.cn/Article/details/gyqqdtcbj.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fktsv.cn/Article/details/gpjalfsue.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fktsv.cn/Article/details/groeolnom.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.yfazqb.com/Article/details/giftjypli.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.epnwcf.com/Article/details/geaifmdhv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.tarul.cn/Article/details/gcifpiegz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.bbcook.cn/Article/details/gvvpfxdhv.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fktsv.cn/Article/details/gqvmhcdfl.sHtML

Py:   with lock: shared += 1
来源：http://3g.tarul.cn/Article/details/gmzupjrze.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.bbcook.cn/Article/details/gjzdcbvwp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.tarul.cn/Article/details/gbyjusfdi.sHtML

TS:   // 同 JS
来源：http://www.share.epnwcf.com/Article/details/gzyshjshj.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.epnwcf.com/Article/details/gpbmmdjpz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.yfazqb.com/Article/details/gesnedcxe.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.yfazqb.com/Article/details/gbpacpuit.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.tarul.cn/Article/details/genxkimrz.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.epnwcf.com/Article/details/gpxjloqsa.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.epnwcf.com/Article/details/gphampytx.sHtML


<!-- 参考信息 -->