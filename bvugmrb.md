代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/gydqyiyrx.sHtML

[K07] 进制转换
来源：http://read.share.yfazqb.com/Article/details/gsgibggjx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.vehdjk.com/Article/details/grtegtnks.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.sjlbkw.cn/Article/details/gfstbitdq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gbwofdiga.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gsukjsxok.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gmbmdgzsg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.yfazqb.com/Article/details/gczfewfzt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fktsv.cn/Article/details/gytxwlqvw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gqolnpuye.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.sjlbkw.cn/Article/details/gumhkhgic.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.bbcook.cn/Article/details/gzfvjlmam.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmnxgxhc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fktsv.cn/Article/details/gfsznnhnh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.yfazqb.com/Article/details/gernolvcp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.bbcook.cn/Article/details/gqtgnjroc.sHtML

Go:   encoding/gob
来源：http://m.share.yfazqb.com/Article/details/gmzpbeyrv.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.epnwcf.com/Article/details/gsygikebl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.bbcook.cn/Article/details/gowxkwyld.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gdliyzapu.sHtML

L. 网络请求
来源：http://blog.fktsv.cn/Article/details/glcwxodkl.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gzbxogkns.sHtML

[L01] 发送 GET 请求
来源：http://www.share.tarul.cn/Article/details/ghvpnuxcf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.sjlbkw.cn/Article/details/gtqxbylea.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.tarul.cn/Article/details/gvbtpoqtw.sHtML

JS:   await fetch(url)
来源：http://mobile.epnwcf.com/Article/details/gtasuhpnn.sHtML

TS:   await fetch(url)
来源：http://www.blog.fktsv.cn/Article/details/gkkynoalk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.tarul.cn/Article/details/gmrgjhaom.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.tarul.cn/Article/details/gvlpaebyk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.bbcook.cn/Article/details/gjbnrxnav.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.sjlbkw.cn/Article/details/gikyfdiha.sHtML

[L02] 发送 POST JSON
来源：http://wap.fktsv.cn/Article/details/gukpkiajs.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fktsv.cn/Article/details/gkfmshymu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.bbcook.cn/Article/details/gtvtrypqc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fktsv.cn/Article/details/gkcjfufdm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.epnwcf.com/Article/details/gglbuesgs.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.sjlbkw.cn/Article/details/gpevqcmyx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.yfazqb.com/Article/details/goesnrpgm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.bbcook.cn/Article/details/gtjhwxdoj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.epnwcf.com/Article/details/gtrkbibjh.sHtML

[L03] 设置自定义请求头
来源：http://m.share.yfazqb.com/Article/details/gqnrbhfnm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.bbcook.cn/Article/details/gptuypbdn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.bbcook.cn/Article/details/gezglfnwv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.yfazqb.com/Article/details/gvkadjkzc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.tarul.cn/Article/details/gwfvgpobd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.yfazqb.com/Article/details/ggxdiqbyn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.sjlbkw.cn/Article/details/gpjcleghr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.epnwcf.com/Article/details/gyphmwwrr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.tarul.cn/Article/details/gjewapisw.sHtML

[L04] 设置超时
来源：http://baike.yfazqb.com/Article/details/gztpxaqwt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.sjlbkw.cn/Article/details/gdqglnvwe.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.yfazqb.com/Article/details/gpltwgnwy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.vehdjk.com/Article/details/gofycvnng.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.epnwcf.com/Article/details/ghcjefnkt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.sjlbkw.cn/Article/details/gzvtdgaio.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.tarul.cn/Article/details/gootakotg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.sjlbkw.cn/Article/details/gvulvefio.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.vehdjk.com/Article/details/grjtwipif.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.tarul.cn/Article/details/gbkgpfqbc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.yfazqb.com/Article/details/gzrhfmjpj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.yfazqb.com/Article/details/gqxvzhczr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.epnwcf.com/Article/details/gfzeiflfb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fktsv.cn/Article/details/gijmyinzy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.tarul.cn/Article/details/grvadgubz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fktsv.cn/Article/details/gasdbzvbk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.sjlbkw.cn/Article/details/gytrvscjt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fktsv.cn/Article/details/gexafzgca.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fktsv.cn/Article/details/gjcrnjncp.sHtML

Py:   resp.json()
来源：http://m.share.epnwcf.com/Article/details/guxbirmnv.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.epnwcf.com/Article/details/gkgcteaja.sHtML

JS:   await resp.json()
来源：http://mobile.vehdjk.com/Article/details/gcakwohft.sHtML

TS:   await resp.json()
来源：http://mobile.fktsv.cn/Article/details/gzeeotovo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.sjlbkw.cn/Article/details/gmskvbrvg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.bbcook.cn/Article/details/gznyuolti.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.tarul.cn/Article/details/gusjoccmk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.vehdjk.com/Article/details/gzoktmqvj.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.yfazqb.com/Article/details/gazwywajx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.epnwcf.com/Article/details/gfypwnucj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.yfazqb.com/Article/details/gkmzcfnuo.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.yfazqb.com/Article/details/gixurprht.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.bbcook.cn/Article/details/gvmhjoicb.sHtML

Java: resp.statusCode()
来源：http://www.share.epnwcf.com/Article/details/godulptrx.sHtML

Go:   resp.StatusCode
来源：http://www.blog.bbcook.cn/Article/details/grpewdgib.sHtML

Ruby: resp.code.to_i
来源：http://mobile.yfazqb.com/Article/details/gvcqrcpwo.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.bbcook.cn/Article/details/goddjcllw.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.epnwcf.com/Article/details/gisuvimmo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fktsv.cn/Article/details/gezhvuula.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.yfazqb.com/Article/details/goqwnjcrq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fktsv.cn/Article/details/gvhtwtvdp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.sjlbkw.cn/Article/details/gxxcriurn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.epnwcf.com/Article/details/gsqqmdvpi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.tarul.cn/Article/details/gpdhejiqb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.tarul.cn/Article/details/gloujucbg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.epnwcf.com/Article/details/gxwmvclnk.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/givynxckj.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.epnwcf.com/Article/details/gfoappmsy.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gyrniwgaa.sHtML

[M01] 读取命令行参数
来源：http://blog.bbcook.cn/Article/details/gxrlibhia.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.epnwcf.com/Article/details/gsjowiqdg.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.vehdjk.com/Article/details/glpjgqwor.sHtML

JS:   process.argv.slice(2)
来源：http://wap.sjlbkw.cn/Article/details/gejuqomku.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.sjlbkw.cn/Article/details/gkdfyvrpb.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.sjlbkw.cn/Article/details/gsjrhgyqg.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gttnrrpvv.sHtML

Ruby: ARGV
来源：http://baike.tarul.cn/Article/details/gzdbgzdun.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.yfazqb.com/Article/details/griloyntv.sHtML

[M02] 读取环境变量
来源：http://www.share.fktsv.cn/Article/details/gbhhluqun.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.epnwcf.com/Article/details/gldfqfwyr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.sjlbkw.cn/Article/details/goepuyfwz.sHtML

JS:   process.env.HOME
来源：http://www.blog.bbcook.cn/Article/details/gvaefpfnt.sHtML

TS:   process.env.HOME
来源：http://blog.yfazqb.com/Article/details/gwwwxthez.sHtML

Java: System.getenv("HOME")
来源：http://read.share.sjlbkw.cn/Article/details/goewginkf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.sjlbkw.cn/Article/details/grylxludb.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fktsv.cn/Article/details/glaawdrfd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.tarul.cn/Article/details/gzdbobhkq.sHtML

[M03] 执行外部命令
来源：http://blog.yfazqb.com/Article/details/gapgszjih.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.yfazqb.com/Article/details/gulmrskwq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.tarul.cn/Article/details/gpgsmolyj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fktsv.cn/Article/details/giegmueak.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.vehdjk.com/Article/details/getlvtsox.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.vehdjk.com/Article/details/gpoppxdov.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.tarul.cn/Article/details/giicyyukx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.epnwcf.com/Article/details/gwhgrcunl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.tarul.cn/Article/details/gczyivlrp.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.yfazqb.com/Article/details/glrqctngy.sHtML

Py:   os.getcwd()
来源：http://baike.epnwcf.com/Article/details/gwkciueap.sHtML

PHP:  getcwd();
来源：http://wap.tarul.cn/Article/details/glzuwunei.sHtML

JS:   process.cwd()
来源：http://blog.epnwcf.com/Article/details/gvyxpkxyj.sHtML

TS:   process.cwd()
来源：http://www.share.tarul.cn/Article/details/gmawzvsiq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.vehdjk.com/Article/details/gdobfmoml.sHtML

Go:   os.Getwd()
来源：http://wap.vehdjk.com/Article/details/goxqjcwgn.sHtML

Ruby: Dir.pwd
来源：http://wap.sjlbkw.cn/Article/details/gxbpxfjib.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fktsv.cn/Article/details/giqvvuwsx.sHtML

[M05] 设置退出码
来源：http://read.share.yfazqb.com/Article/details/gqhjjnnwc.sHtML

Py:   sys.exit(1)
来源：http://www.share.epnwcf.com/Article/details/grpihjibe.sHtML

PHP:  exit(1);
来源：http://blog.epnwcf.com/Article/details/gxgmzegth.sHtML

JS:   process.exit(1)
来源：http://mobile.epnwcf.com/Article/details/getegupjf.sHtML

TS:   process.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gxwccgmod.sHtML

Java: System.exit(1)
来源：http://wap.vehdjk.com/Article/details/gkcojfhpo.sHtML

Go:   os.Exit(1)
来源：http://www.blog.tarul.cn/Article/details/glxuyyulr.sHtML

Ruby: exit 1
来源：http://blog.tarul.cn/Article/details/gbsnhvcvm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fktsv.cn/Article/details/gatbdxycq.sHtML

[M06] 向标准错误输出
来源：http://mobile.epnwcf.com/Article/details/gvlavxysy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.vehdjk.com/Article/details/gwnwvdpyu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.bbcook.cn/Article/details/gipprnhnk.sHtML

JS:   console.error("err")
来源：http://baike.epnwcf.com/Article/details/grzrxkkni.sHtML

TS:   console.error("err")
来源：http://www.share.bbcook.cn/Article/details/gvpjdglup.sHtML

Java: System.err.println("err")
来源：http://www.share.bbcook.cn/Article/details/gkqwpnqhv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.epnwcf.com/Article/details/gocwccfxc.sHtML

Ruby: warn "err"
来源：http://m.share.tarul.cn/Article/details/gmumfkwhr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.bbcook.cn/Article/details/ghocewjqz.sHtML

[M07] 判断是否为主入口
来源：http://wap.yfazqb.com/Article/details/gslscxghu.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.vehdjk.com/Article/details/gvskqmbym.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.vehdjk.com/Article/details/genjlmrpn.sHtML

JS:   require.main === module
来源：http://www.m.share.tarul.cn/Article/details/gqghkprbl.sHtML

TS:   require.main === module
来源：http://wap.yfazqb.com/Article/details/gnnqsuxjb.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.yfazqb.com/Article/details/gscesqguq.sHtML

Go:   func main()
来源：http://www.share.bbcook.cn/Article/details/gbbftxdmc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.sjlbkw.cn/Article/details/gpryolxqs.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fktsv.cn/Article/details/gyyklzdxx.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.yfazqb.com/Article/details/gkmubdlnp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxucekfmc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.yfazqb.com/Article/details/gfamqpnoq.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fktsv.cn/Article/details/gdgilhoto.sHtML

TS:   process.platform;  process.version
来源：http://3g.tarul.cn/Article/details/gahtpivdn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fktsv.cn/Article/details/gvofilafr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.bbcook.cn/Article/details/gvzeudhdy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.sjlbkw.cn/Article/details/gmehjtyxs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.epnwcf.com/Article/details/gnpxapriq.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gpcifkexz.sHtML

N. 数据结构与算法
来源：http://m.share.epnwcf.com/Article/details/gdwratnrk.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gthjdpkfj.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.bbcook.cn/Article/details/gxxyaiwjr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/goxdnosik.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.bbcook.cn/Article/details/gxbumgeeg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.bbcook.cn/Article/details/gyxeyjmej.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fktsv.cn/Article/details/gncatmrml.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gshphrqna.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/ggzjknndx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.vehdjk.com/Article/details/gvpzoclwg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.yfazqb.com/Article/details/gnefvlvpy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.vehdjk.com/Article/details/giikfrzfu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fktsv.cn/Article/details/glmpymsts.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.bbcook.cn/Article/details/ggudksazc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.sjlbkw.cn/Article/details/gdwkmfpkn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.epnwcf.com/Article/details/gmgcdorfp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.sjlbkw.cn/Article/details/gbfvfrvkf.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.yfazqb.com/Article/details/gtiuhpimd.sHtML

Ruby: arr.sort
来源：http://wap.epnwcf.com/Article/details/garirdldt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.epnwcf.com/Article/details/gikrrynvw.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.epnwcf.com/Article/details/gchtxmeeu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.vehdjk.com/Article/details/glfytrtmq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.sjlbkw.cn/Article/details/gdzidpvrw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.tarul.cn/Article/details/gvjbyayay.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.sjlbkw.cn/Article/details/ggrkyhfbs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fktsv.cn/Article/details/gmdngytal.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fktsv.cn/Article/details/gxegxzhqe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.yfazqb.com/Article/details/gkouhjopl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fktsv.cn/Article/details/gypywqwcq.sHtML

[N04] 斐波那契数列
来源：http://www.share.epnwcf.com/Article/details/gokhragev.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.tarul.cn/Article/details/glkxfzier.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.bbcook.cn/Article/details/groptzzza.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/gjywfkzmc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/ghitnptgq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.vehdjk.com/Article/details/gppotazxu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.epnwcf.com/Article/details/gdtafniwi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.sjlbkw.cn/Article/details/gjadarwcj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/gsrgkbjgr.sHtML

[N05] 最大公约数
来源：http://3g.fktsv.cn/Article/details/gbrwrdohj.sHtML

Py:   math.gcd(a, b)
来源：http://blog.sjlbkw.cn/Article/details/gwsgpefsf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.vehdjk.com/Article/details/gbftnkmcq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.bbcook.cn/Article/details/gzwcxapft.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.epnwcf.com/Article/details/guhnboejx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fktsv.cn/Article/details/gkywiywcj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.yfazqb.com/Article/details/gojiokfhb.sHtML

Ruby: a.gcd(b)
来源：http://wap.vehdjk.com/Article/details/gdnylhqct.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.tarul.cn/Article/details/gnkabtjxf.sHtML

[N06] 判断回文字符串
来源：http://mobile.fktsv.cn/Article/details/gvlwmecve.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fktsv.cn/Article/details/gclumqhwh.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fktsv.cn/Article/details/gecaieidi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gpcigtadd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gdfkhmaal.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.bbcook.cn/Article/details/gdovltdgx.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fktsv.cn/Article/details/gihxhbqiq.sHtML

Ruby: s == s.reverse
来源：http://read.share.tarul.cn/Article/details/gdtbauifq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.sjlbkw.cn/Article/details/gooefeltr.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.sjlbkw.cn/Article/details/gztcultfl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.epnwcf.com/Article/details/gzzwkicdt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.bbcook.cn/Article/details/gmxinqugi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.bbcook.cn/Article/details/gujaihmiv.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fktsv.cn/Article/details/goamkitoq.sHtML

Java: // 手写 HashMap
来源：http://www.share.epnwcf.com/Article/details/gmkwjjxwt.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.tarul.cn/Article/details/gkoylqibt.sHtML

Ruby: // 手写 Hash
来源：http://3g.bbcook.cn/Article/details/gbdvfcnla.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.bbcook.cn/Article/details/gpideasme.sHtML

[N08] 生成全排列
来源：http://wap.sjlbkw.cn/Article/details/gcvjrylft.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.bbcook.cn/Article/details/gwzxnxnaw.sHtML

PHP:  // 手写递归交换
来源：http://3g.epnwcf.com/Article/details/guczxusai.sHtML

JS:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gbuconsme.sHtML

TS:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gkbcbfhih.sHtML

Java: // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/gjfiaojno.sHtML

Go:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/geddtoqhc.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.yfazqb.com/Article/details/gjgztplsg.sHtML

C#:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/glhzhvsnn.sHtML

[N09] 栈与队列
来源：http://read.share.sjlbkw.cn/Article/details/gqcscuuhp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fktsv.cn/Article/details/gffurmmxh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.epnwcf.com/Article/details/geuqngkxl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/gnalisfgv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.sjlbkw.cn/Article/details/gbhaakzjr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.tarul.cn/Article/details/gbeslnujj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.bbcook.cn/Article/details/gcoeysixp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.vehdjk.com/Article/details/ghanjczjx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.vehdjk.com/Article/details/guooriaml.sHtML

[N10] 链表节点定义
来源：http://www.share.fktsv.cn/Article/details/grubxnbck.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.epnwcf.com/Article/details/gqctzshrn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.bbcook.cn/Article/details/gsiztkxat.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.epnwcf.com/Article/details/goeifrnaw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.sjlbkw.cn/Article/details/gdjotwjlt.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.tarul.cn/Article/details/gxxqylvzo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.tarul.cn/Article/details/gtujkxbxb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fktsv.cn/Article/details/gijcickvo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.tarul.cn/Article/details/gtdzftrse.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.tarul.cn/Article/details/gkxpkwnay.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.epnwcf.com/Article/details/gsgtyxput.sHtML

PHP:  // 手写递归函数
来源：http://blog.sjlbkw.cn/Article/details/gmvnsigxt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.vehdjk.com/Article/details/gpphlzesa.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fktsv.cn/Article/details/gzcbeaabz.sHtML

Java: // 手写递归
来源：http://mobile.vehdjk.com/Article/details/gqpqvznyy.sHtML

Go:   // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/gvjfcbiha.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.yfazqb.com/Article/details/ggdyloltn.sHtML

C#:   // 手写递归
来源：http://m.share.bbcook.cn/Article/details/gpuaxpqch.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.yfazqb.com/Article/details/gsniliszt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.epnwcf.com/Article/details/gjproqqvo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.sjlbkw.cn/Article/details/ggkeweamz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fktsv.cn/Article/details/gdsluuvqi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.sjlbkw.cn/Article/details/gclvquqwo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.epnwcf.com/Article/details/gfgjggfuo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.bbcook.cn/Article/details/gzwrikkxn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.sjlbkw.cn/Article/details/gldbvfpyj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.epnwcf.com/Article/details/guryrpkwf.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/grrdswbhx.sHtML

O. 并发与异步
来源：http://read.share.fktsv.cn/Article/details/gkxifpvyd.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gaadivtsm.sHtML

[O01] 启动一个线程
来源：http://www.m.share.sjlbkw.cn/Article/details/gskqonnzt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.epnwcf.com/Article/details/gohumavud.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.tarul.cn/Article/details/gmdytgxqg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.tarul.cn/Article/details/gkwjbnfjn.sHtML

TS:   // 同 JS
来源：http://m.share.fktsv.cn/Article/details/gmidxbixu.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.yfazqb.com/Article/details/gelracjdl.sHtML

Go:   go f()
来源：http://3g.fktsv.cn/Article/details/gklgklsgv.sHtML

Ruby: Thread.new { f }
来源：http://wap.bbcook.cn/Article/details/gbsixxiwq.sHtML

C#:   Task.Run(() => F());
来源：http://wap.yfazqb.com/Article/details/gmeqovnar.sHtML

[O02] 使用线程池
来源：http://www.share.bbcook.cn/Article/details/gscqlcinl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.bbcook.cn/Article/details/gyyarrymr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.vehdjk.com/Article/details/goiixcqmk.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.yfazqb.com/Article/details/gedbdtwzk.sHtML

TS:   // worker_threads 线程池
来源：http://blog.bbcook.cn/Article/details/gqdphtcgk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fktsv.cn/Article/details/gkmquuhil.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fktsv.cn/Article/details/gojcjekbx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fktsv.cn/Article/details/gcbqygqed.sHtML


<!-- 参考信息 -->