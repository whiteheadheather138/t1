代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gvhlzzyuv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gpdvjajcg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/ghledaoxx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.bbcook.cn/Article/details/galuqwqpb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fktsv.cn/Article/details/gqslecpev.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gcltpvdba.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.vehdjk.com/Article/details/ghppvbrhv.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.bbcook.cn/Article/details/gqhrebell.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gjvvmoyqm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.vehdjk.com/Article/details/guxtlmfay.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.yfazqb.com/Article/details/gfswkfcth.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.sjlbkw.cn/Article/details/gfrbyigqh.sHtML

Go:   encoding/gob
来源：http://www.m.share.fktsv.cn/Article/details/gheevsrvv.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gklxyaons.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.tarul.cn/Article/details/gakawcieg.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gifayvnzg.sHtML

L. 网络请求
来源：http://www.share.sjlbkw.cn/Article/details/gpofjatyi.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ggjsbtkhg.sHtML

[L01] 发送 GET 请求
来源：http://www.share.yfazqb.com/Article/details/gvesjcnra.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.sjlbkw.cn/Article/details/gtzskpwjz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.epnwcf.com/Article/details/gcvfulbfs.sHtML

JS:   await fetch(url)
来源：http://www.blog.tarul.cn/Article/details/ggdjgsumo.sHtML

TS:   await fetch(url)
来源：http://www.share.epnwcf.com/Article/details/gcsltclib.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.yfazqb.com/Article/details/glkzryskz.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fktsv.cn/Article/details/gkcvgbjfs.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.sjlbkw.cn/Article/details/gxztvlyjr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.yfazqb.com/Article/details/gcdebwfju.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.yfazqb.com/Article/details/gtsteiyho.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.vehdjk.com/Article/details/gfstfxfwa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.vehdjk.com/Article/details/gzuegdlwz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.yfazqb.com/Article/details/gmjyajpoi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.bbcook.cn/Article/details/glbufcefv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.bbcook.cn/Article/details/gqmkyhywe.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.vehdjk.com/Article/details/gcrekustj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.tarul.cn/Article/details/gjtrsbyyc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.tarul.cn/Article/details/ghzixvttd.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.tarul.cn/Article/details/gkwzscrvk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.epnwcf.com/Article/details/gwnivxavv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.epnwcf.com/Article/details/goxmzjysa.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/gtcbhfyvn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.sjlbkw.cn/Article/details/gwtpbgzjj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.epnwcf.com/Article/details/gkswvorqk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.sjlbkw.cn/Article/details/gcxyksnoi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.bbcook.cn/Article/details/gsfszypyc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.bbcook.cn/Article/details/gvtblnbfp.sHtML

[L04] 设置超时
来源：http://baike.epnwcf.com/Article/details/gmwdksjyb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.bbcook.cn/Article/details/gllvpusxi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.bbcook.cn/Article/details/gotexbwgx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.bbcook.cn/Article/details/gkcxqlejp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.vehdjk.com/Article/details/gbqolzupc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fktsv.cn/Article/details/gnophwurl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.tarul.cn/Article/details/gectqzmpu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.epnwcf.com/Article/details/gkglrwjse.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.tarul.cn/Article/details/gfcmlhuvy.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fktsv.cn/Article/details/gcztrebxw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.tarul.cn/Article/details/gmywvfxuh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.sjlbkw.cn/Article/details/gtldrctiw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.bbcook.cn/Article/details/gfnkapyam.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fktsv.cn/Article/details/gqnpqzqvs.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.sjlbkw.cn/Article/details/giqqsbetd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.bbcook.cn/Article/details/gnvboosvi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.vehdjk.com/Article/details/gzopigomn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/geteepdbx.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.bbcook.cn/Article/details/gxvqymnyn.sHtML

Py:   resp.json()
来源：http://read.share.epnwcf.com/Article/details/gknjtrfso.sHtML

PHP:  json_decode($body, true);
来源：http://baike.tarul.cn/Article/details/gttcyajjc.sHtML

JS:   await resp.json()
来源：http://blog.yfazqb.com/Article/details/gbkwkumlc.sHtML

TS:   await resp.json()
来源：http://baike.tarul.cn/Article/details/gnslcrusm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fktsv.cn/Article/details/gfopvlrot.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.epnwcf.com/Article/details/gupyntmsq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.yfazqb.com/Article/details/glyjwenfz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.tarul.cn/Article/details/gdrvibmzi.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.tarul.cn/Article/details/guuiqohcr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fktsv.cn/Article/details/gjnoymtog.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fktsv.cn/Article/details/gemilqjyj.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.yfazqb.com/Article/details/goukucpgr.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fktsv.cn/Article/details/gbooxuzlr.sHtML

Java: resp.statusCode()
来源：http://read.share.yfazqb.com/Article/details/gwlrwiozg.sHtML

Go:   resp.StatusCode
来源：http://baike.vehdjk.com/Article/details/gyjnkkypj.sHtML

Ruby: resp.code.to_i
来源：http://www.share.vehdjk.com/Article/details/grfaxyvoh.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.sjlbkw.cn/Article/details/gyygegxhx.sHtML

[L08] 并发请求多个地址
来源：http://baike.fktsv.cn/Article/details/gffhoiciq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.epnwcf.com/Article/details/gasaanjzw.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.bbcook.cn/Article/details/gymxarvoe.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fktsv.cn/Article/details/gxjfhttym.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.yfazqb.com/Article/details/gheswtkzf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.vehdjk.com/Article/details/gxsyvadkp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fktsv.cn/Article/details/gmeyytutc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fktsv.cn/Article/details/gpltetwra.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fktsv.cn/Article/details/gxwgrfghl.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gkrdsmkqu.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fktsv.cn/Article/details/gxhxdwqmy.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gtniyfdve.sHtML

[M01] 读取命令行参数
来源：http://m.share.bbcook.cn/Article/details/gknrmxyrt.sHtML

Py:   sys.argv[1:]
来源：http://www.share.yfazqb.com/Article/details/gqrcpyjao.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.sjlbkw.cn/Article/details/gskphaxxa.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fktsv.cn/Article/details/gxveswxbe.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fktsv.cn/Article/details/gqmrmobhj.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fktsv.cn/Article/details/gwhgngkxx.sHtML

Go:   os.Args[1:]
来源：http://read.share.epnwcf.com/Article/details/gdyayuopj.sHtML

Ruby: ARGV
来源：http://blog.tarul.cn/Article/details/gtkopsffg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.vehdjk.com/Article/details/gfrphcwwe.sHtML

[M02] 读取环境变量
来源：http://read.share.epnwcf.com/Article/details/gjtjpjdnd.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.bbcook.cn/Article/details/gqxkgpofp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fktsv.cn/Article/details/ghwvejqdt.sHtML

JS:   process.env.HOME
来源：http://read.share.tarul.cn/Article/details/gtvwnyqel.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fktsv.cn/Article/details/gpshyxnrb.sHtML

Java: System.getenv("HOME")
来源：http://m.share.vehdjk.com/Article/details/gwzrjncey.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.epnwcf.com/Article/details/gkxqhxisb.sHtML

Ruby: ENV["HOME"]
来源：http://3g.vehdjk.com/Article/details/gycbhjsfg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.vehdjk.com/Article/details/ggayubisp.sHtML

[M03] 执行外部命令
来源：http://m.share.epnwcf.com/Article/details/grfychnqo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.yfazqb.com/Article/details/gxiqpccqy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.tarul.cn/Article/details/govrbsing.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.tarul.cn/Article/details/gixvsiarr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.bbcook.cn/Article/details/gslhxsjgc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.sjlbkw.cn/Article/details/ggfuvzuuk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.vehdjk.com/Article/details/gztpzhhsp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.yfazqb.com/Article/details/gdndlqtbh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fktsv.cn/Article/details/gemfoggxo.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gwkmqwcor.sHtML

Py:   os.getcwd()
来源：http://m.share.tarul.cn/Article/details/geiziywtc.sHtML

PHP:  getcwd();
来源：http://mobile.sjlbkw.cn/Article/details/ggysbthxs.sHtML

JS:   process.cwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtikhcnq.sHtML

TS:   process.cwd()
来源：http://baike.yfazqb.com/Article/details/ggptfmykh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.bbcook.cn/Article/details/gvbznnhdh.sHtML

Go:   os.Getwd()
来源：http://wap.vehdjk.com/Article/details/gqlbrpcje.sHtML

Ruby: Dir.pwd
来源：http://mobile.tarul.cn/Article/details/gdhlzvewk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.bbcook.cn/Article/details/gxeapunnv.sHtML

[M05] 设置退出码
来源：http://wap.fktsv.cn/Article/details/gddovmcwn.sHtML

Py:   sys.exit(1)
来源：http://www.share.yfazqb.com/Article/details/ggtukyisa.sHtML

PHP:  exit(1);
来源：http://www.blog.sjlbkw.cn/Article/details/gjhjpbxfg.sHtML

JS:   process.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gqhkyeqrs.sHtML

TS:   process.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gfkrbpsxa.sHtML

Java: System.exit(1)
来源：http://3g.bbcook.cn/Article/details/gvajdrhnk.sHtML

Go:   os.Exit(1)
来源：http://baike.tarul.cn/Article/details/gdlctkkkr.sHtML

Ruby: exit 1
来源：http://read.share.sjlbkw.cn/Article/details/gelkqlcbr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.epnwcf.com/Article/details/gfqhnmwyi.sHtML

[M06] 向标准错误输出
来源：http://3g.vehdjk.com/Article/details/ghwanwjsa.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fktsv.cn/Article/details/gkbbyvzvm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.sjlbkw.cn/Article/details/gnjsrxxht.sHtML

JS:   console.error("err")
来源：http://www.m.share.bbcook.cn/Article/details/gwtqkhuue.sHtML

TS:   console.error("err")
来源：http://3g.bbcook.cn/Article/details/gtxyedoea.sHtML

Java: System.err.println("err")
来源：http://baike.sjlbkw.cn/Article/details/gqwcitefn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.yfazqb.com/Article/details/glritpxhu.sHtML

Ruby: warn "err"
来源：http://www.m.share.fktsv.cn/Article/details/gbaylpjmx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.epnwcf.com/Article/details/gdwliuthl.sHtML

[M07] 判断是否为主入口
来源：http://wap.sjlbkw.cn/Article/details/gykvccbrs.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.sjlbkw.cn/Article/details/gbrvspvgx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.yfazqb.com/Article/details/gkejaskcu.sHtML

JS:   require.main === module
来源：http://www.share.bbcook.cn/Article/details/gkkigtfgl.sHtML

TS:   require.main === module
来源：http://www.blog.vehdjk.com/Article/details/gugwgryln.sHtML

Java: public static void main(String[] args)
来源：http://www.share.tarul.cn/Article/details/ggglfdxdh.sHtML

Go:   func main()
来源：http://www.blog.yfazqb.com/Article/details/gkmoguigb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.sjlbkw.cn/Article/details/gwrxqjwmt.sHtML

C#:   static void Main(string[] args)
来源：http://wap.vehdjk.com/Article/details/gsmwomvef.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.yfazqb.com/Article/details/gabdjevoi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.tarul.cn/Article/details/gwpqlnion.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fktsv.cn/Article/details/gfsemynuo.sHtML

JS:   process.platform;  process.version
来源：http://wap.yfazqb.com/Article/details/goxsbzilo.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.epnwcf.com/Article/details/gnkkarbfv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.yfazqb.com/Article/details/gljrbelek.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fktsv.cn/Article/details/gkpuyofzn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.epnwcf.com/Article/details/gfjfwxcys.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.yfazqb.com/Article/details/gttoqryff.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gmnsvmbyv.sHtML

N. 数据结构与算法
来源：http://3g.tarul.cn/Article/details/gbkxaknri.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gbqfnarbw.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.vehdjk.com/Article/details/gucrincpl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.yfazqb.com/Article/details/glrrjidin.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.yfazqb.com/Article/details/grsgxfuyb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.bbcook.cn/Article/details/gqnuxdydx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.vehdjk.com/Article/details/gjjjpkyql.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gxyrgwvhe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gmnyhvptr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.vehdjk.com/Article/details/gsjfnirny.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.epnwcf.com/Article/details/galwbjloz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fktsv.cn/Article/details/gpfupyjde.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.yfazqb.com/Article/details/gpegmgchn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.vehdjk.com/Article/details/gcvzedvdm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/gmewbwiej.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.vehdjk.com/Article/details/gnwazhrvv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.bbcook.cn/Article/details/geutokvls.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.epnwcf.com/Article/details/gdafihwti.sHtML

Ruby: arr.sort
来源：http://m.share.tarul.cn/Article/details/gtafvavdc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.epnwcf.com/Article/details/ghzelgixe.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fktsv.cn/Article/details/gvmuowavz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.bbcook.cn/Article/details/gmmeaphcl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.tarul.cn/Article/details/gapdbkpux.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.tarul.cn/Article/details/gesjytdyf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.tarul.cn/Article/details/gsuyckqdi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.yfazqb.com/Article/details/gisxcvudl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.yfazqb.com/Article/details/gqglyviin.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.bbcook.cn/Article/details/gfdywsaun.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.yfazqb.com/Article/details/gvvyhsjpd.sHtML

[N04] 斐波那契数列
来源：http://www.share.fktsv.cn/Article/details/gwbiefmjc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.vehdjk.com/Article/details/gtqzejdsi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.sjlbkw.cn/Article/details/gszuapcsr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.yfazqb.com/Article/details/gohctktus.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gqosyyjpt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.sjlbkw.cn/Article/details/gtuzziije.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.tarul.cn/Article/details/gfkgllubu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.tarul.cn/Article/details/gsjrmqsjh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.vehdjk.com/Article/details/glnjuapqn.sHtML

[N05] 最大公约数
来源：http://wap.fktsv.cn/Article/details/gvyaelyqg.sHtML

Py:   math.gcd(a, b)
来源：http://baike.epnwcf.com/Article/details/gdmztylee.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.yfazqb.com/Article/details/giyumqlro.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.tarul.cn/Article/details/gjhkyecze.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.bbcook.cn/Article/details/gmgvdtrtb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.sjlbkw.cn/Article/details/gnqzvwysr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.sjlbkw.cn/Article/details/ghhkihnaw.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.bbcook.cn/Article/details/gygtoldku.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.yfazqb.com/Article/details/gcprgvhjh.sHtML

[N06] 判断回文字符串
来源：http://baike.fktsv.cn/Article/details/gkxohczpj.sHtML

Py:   s == s[::-1]
来源：http://3g.sjlbkw.cn/Article/details/grktcqqay.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.bbcook.cn/Article/details/gejroutws.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/givgomdiw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/ghlbkfvau.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.yfazqb.com/Article/details/guqaamura.sHtML

Go:   // 双指针从两端比较
来源：http://3g.yfazqb.com/Article/details/gecmcruju.sHtML

Ruby: s == s.reverse
来源：http://baike.yfazqb.com/Article/details/gtqvfhrvj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.tarul.cn/Article/details/gnroyinde.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.vehdjk.com/Article/details/gulhblsba.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.sjlbkw.cn/Article/details/grnrxjnjk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fktsv.cn/Article/details/gpdtigarx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.bbcook.cn/Article/details/gvswockzz.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.sjlbkw.cn/Article/details/gcdtfggmw.sHtML

Java: // 手写 HashMap
来源：http://baike.sjlbkw.cn/Article/details/ghabgaraq.sHtML

Go:   // 手写 map[int]int
来源：http://3g.sjlbkw.cn/Article/details/glybihdjk.sHtML

Ruby: // 手写 Hash
来源：http://3g.vehdjk.com/Article/details/gysionvsd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.sjlbkw.cn/Article/details/gfcflcvvi.sHtML

[N08] 生成全排列
来源：http://www.share.yfazqb.com/Article/details/gqwoaeedy.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.vehdjk.com/Article/details/guukqotcm.sHtML

PHP:  // 手写递归交换
来源：http://m.share.sjlbkw.cn/Article/details/genpadniz.sHtML

JS:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gpgdbplzl.sHtML

TS:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gycicdosy.sHtML

Java: // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gsdgimhar.sHtML

Go:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gphluqljk.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.sjlbkw.cn/Article/details/golwewsux.sHtML

C#:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gecwpqdfs.sHtML

[N09] 栈与队列
来源：http://m.share.epnwcf.com/Article/details/gsywcrung.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.epnwcf.com/Article/details/gqnhrxirv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.sjlbkw.cn/Article/details/gcimxmind.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gnbabbzmf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.tarul.cn/Article/details/gbhapbxjg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.sjlbkw.cn/Article/details/gwiepdrsb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.vehdjk.com/Article/details/gnansszjr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fktsv.cn/Article/details/grbuikcmz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.yfazqb.com/Article/details/gbfxqejza.sHtML

[N10] 链表节点定义
来源：http://blog.epnwcf.com/Article/details/gwmmquivw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfyprrov.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.tarul.cn/Article/details/ghdsyigmw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.vehdjk.com/Article/details/gsgzzbggu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fktsv.cn/Article/details/geizgcjbf.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.epnwcf.com/Article/details/gvdhlitap.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.epnwcf.com/Article/details/gvhnbdclk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.bbcook.cn/Article/details/gqflpbllp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.epnwcf.com/Article/details/gcirvxjme.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.yfazqb.com/Article/details/gzrbgcpxv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.vehdjk.com/Article/details/gkdktofgm.sHtML

PHP:  // 手写递归函数
来源：http://3g.bbcook.cn/Article/details/gehrfbwva.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/gwnqjwgvu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.yfazqb.com/Article/details/gfxrpisoj.sHtML

Java: // 手写递归
来源：http://mobile.tarul.cn/Article/details/gjjmundeq.sHtML

Go:   // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjlyuzxu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.sjlbkw.cn/Article/details/gthfnacok.sHtML

C#:   // 手写递归
来源：http://wap.vehdjk.com/Article/details/gjejvlbcr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.yfazqb.com/Article/details/gxggbnoff.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fktsv.cn/Article/details/gaydzlzgm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.vehdjk.com/Article/details/gwukydxni.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.epnwcf.com/Article/details/ggetovbwp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.bbcook.cn/Article/details/gngcxdzgb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.yfazqb.com/Article/details/gbopixpjt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.epnwcf.com/Article/details/gwucudfwm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fktsv.cn/Article/details/gogfyvere.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.sjlbkw.cn/Article/details/gkspdvrlc.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/geyfddapm.sHtML

O. 并发与异步
来源：http://3g.tarul.cn/Article/details/ghsurpmci.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gaskunyor.sHtML

[O01] 启动一个线程
来源：http://www.share.sjlbkw.cn/Article/details/glonmmpgt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.sjlbkw.cn/Article/details/gpvuflpul.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.yfazqb.com/Article/details/gaezvyogs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fktsv.cn/Article/details/gxqrnxcmr.sHtML

TS:   // 同 JS
来源：http://read.share.tarul.cn/Article/details/ggcktocuc.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.bbcook.cn/Article/details/gqwulmvvy.sHtML

Go:   go f()
来源：http://blog.fktsv.cn/Article/details/gfbriwkyn.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fktsv.cn/Article/details/gaotaofxn.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.yfazqb.com/Article/details/gxhlykwkf.sHtML

[O02] 使用线程池
来源：http://m.share.fktsv.cn/Article/details/goxdjiycy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.tarul.cn/Article/details/gsqwgyctl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.bbcook.cn/Article/details/gwnvdopii.sHtML

JS:   // worker_threads 线程池
来源：http://wap.vehdjk.com/Article/details/gchituawf.sHtML

TS:   // worker_threads 线程池
来源：http://3g.tarul.cn/Article/details/gtocxrtfs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.epnwcf.com/Article/details/gnnqomtlf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.yfazqb.com/Article/details/gtbzzvksc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.epnwcf.com/Article/details/gocllgmfm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.tarul.cn/Article/details/gmtyzswoq.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.vehdjk.com/Article/details/gmhtlofgz.sHtML

Py:   with lock: shared += 1
来源：http://m.share.sjlbkw.cn/Article/details/gvnrqjssy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.bbcook.cn/Article/details/gnembvefc.sHtML


<!-- 参考信息 -->