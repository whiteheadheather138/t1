代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fktsv.cn/Article/details/gygijjsue.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fktsv.cn/Article/details/gisufhfab.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.epnwcf.com/Article/details/gdawhraje.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/gkbczwxuk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.tarul.cn/Article/details/gdkdlarik.sHtML

[K07] 进制转换
来源：http://read.share.yfazqb.com/Article/details/gfrizcxuj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gftwavztg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.sjlbkw.cn/Article/details/gozfagseq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gzgxhlxyi.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gjqvihbkk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/getfuebsb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.bbcook.cn/Article/details/gxkdqeyzk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.sjlbkw.cn/Article/details/gluhttfvl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gvjkinfoy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.sjlbkw.cn/Article/details/glqntwqmj.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.bbcook.cn/Article/details/grvrtdzuy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fktsv.cn/Article/details/gpkxsdloh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fktsv.cn/Article/details/gogyreoev.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.bbcook.cn/Article/details/giqnexpdc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.bbcook.cn/Article/details/gfqprcnoy.sHtML

Go:   encoding/gob
来源：http://m.share.epnwcf.com/Article/details/gzoghnscg.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.tarul.cn/Article/details/gurcjxjsc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fktsv.cn/Article/details/ggisoguhj.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gjtpzgmeh.sHtML

L. 网络请求
来源：http://www.m.share.tarul.cn/Article/details/gjjveoopm.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gefvonrii.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.sjlbkw.cn/Article/details/gdosqwgjb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.vehdjk.com/Article/details/gkclwblcx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fktsv.cn/Article/details/gumietarz.sHtML

JS:   await fetch(url)
来源：http://www.share.bbcook.cn/Article/details/gqllxwtzu.sHtML

TS:   await fetch(url)
来源：http://3g.fktsv.cn/Article/details/gphstbmoh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fktsv.cn/Article/details/gziqthkim.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.bbcook.cn/Article/details/gdahqlcdp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.sjlbkw.cn/Article/details/gjwddsblk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.epnwcf.com/Article/details/ghxemxlvi.sHtML

[L02] 发送 POST JSON
来源：http://www.share.tarul.cn/Article/details/gbsbrcsgh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.sjlbkw.cn/Article/details/gaulfxnhi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.sjlbkw.cn/Article/details/gdijrfswc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.epnwcf.com/Article/details/ghjhezniw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.vehdjk.com/Article/details/gxkpiiwzl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.yfazqb.com/Article/details/gxofzuime.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fktsv.cn/Article/details/gvqaprdmd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.bbcook.cn/Article/details/gkxlilzkh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.vehdjk.com/Article/details/gbxhkspwd.sHtML

[L03] 设置自定义请求头
来源：http://read.share.yfazqb.com/Article/details/gbunglzmf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.sjlbkw.cn/Article/details/gwpvaeyar.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.vehdjk.com/Article/details/gnxvacxyd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.yfazqb.com/Article/details/ghwdnmcvg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.bbcook.cn/Article/details/gonamdxof.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.yfazqb.com/Article/details/gdlmazhbv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.tarul.cn/Article/details/gtrmsefij.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fktsv.cn/Article/details/grcrtsgxa.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fktsv.cn/Article/details/geqxgrqjb.sHtML

[L04] 设置超时
来源：http://wap.yfazqb.com/Article/details/gngsipjjm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.vehdjk.com/Article/details/gsmisscwg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.vehdjk.com/Article/details/gtxpvvykx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.yfazqb.com/Article/details/gjxcyqdlc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fktsv.cn/Article/details/gcnjuconz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.bbcook.cn/Article/details/gjqtyuifu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fktsv.cn/Article/details/ghrbcpknn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fktsv.cn/Article/details/gktnatkek.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.yfazqb.com/Article/details/goqzvpqej.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.vehdjk.com/Article/details/gfexwntsj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.vehdjk.com/Article/details/grbstuzdj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fktsv.cn/Article/details/guqeueldf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.sjlbkw.cn/Article/details/ghdvecvhz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.tarul.cn/Article/details/gxkmvlbzh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.epnwcf.com/Article/details/glpflqowm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.epnwcf.com/Article/details/ggirqpmah.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.yfazqb.com/Article/details/gdndklddr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.epnwcf.com/Article/details/gdjixwspe.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fktsv.cn/Article/details/gjoevtffh.sHtML

Py:   resp.json()
来源：http://3g.epnwcf.com/Article/details/gbefjvyfn.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.vehdjk.com/Article/details/gsqmbvfrg.sHtML

JS:   await resp.json()
来源：http://blog.bbcook.cn/Article/details/ggbbkuagx.sHtML

TS:   await resp.json()
来源：http://wap.fktsv.cn/Article/details/gigwcnppc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.yfazqb.com/Article/details/ggvtzvtrl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.yfazqb.com/Article/details/gfafamwgp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.vehdjk.com/Article/details/gdfyjgfep.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.epnwcf.com/Article/details/gmvyauffu.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.yfazqb.com/Article/details/gnonxbqos.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.tarul.cn/Article/details/gsadneaxx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fktsv.cn/Article/details/gcbgmxinb.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.bbcook.cn/Article/details/ghhzwlrmg.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.sjlbkw.cn/Article/details/gpuwsuqmg.sHtML

Java: resp.statusCode()
来源：http://read.share.epnwcf.com/Article/details/gsxncndew.sHtML

Go:   resp.StatusCode
来源：http://wap.bbcook.cn/Article/details/ghqhsubyd.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fktsv.cn/Article/details/gajflsqps.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fktsv.cn/Article/details/gdcmywshh.sHtML

[L08] 并发请求多个地址
来源：http://m.share.epnwcf.com/Article/details/gbsdvzsec.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.tarul.cn/Article/details/gjpwkrbqe.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.yfazqb.com/Article/details/giciqbgty.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gztrqofan.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/gzqwxsthu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.yfazqb.com/Article/details/gtjusansh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.epnwcf.com/Article/details/gdwixvvni.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.vehdjk.com/Article/details/gkwmdymkv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.vehdjk.com/Article/details/gvenmozbz.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gngymjfgz.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.tarul.cn/Article/details/gfkbrdxfa.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gptgichbk.sHtML

[M01] 读取命令行参数
来源：http://read.share.sjlbkw.cn/Article/details/gxqjaffru.sHtML

Py:   sys.argv[1:]
来源：http://m.share.bbcook.cn/Article/details/ggvgcbloo.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.vehdjk.com/Article/details/gayidxinu.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.epnwcf.com/Article/details/gblhdnoos.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.yfazqb.com/Article/details/gnxbhrdpm.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.tarul.cn/Article/details/gmsdrajfs.sHtML

Go:   os.Args[1:]
来源：http://baike.vehdjk.com/Article/details/gokbargwa.sHtML

Ruby: ARGV
来源：http://mobile.fktsv.cn/Article/details/ggztdcvpj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.sjlbkw.cn/Article/details/gymuythhn.sHtML

[M02] 读取环境变量
来源：http://www.blog.fktsv.cn/Article/details/ghmihrjoq.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.tarul.cn/Article/details/gtbkuoufi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.yfazqb.com/Article/details/gohnrqrws.sHtML

JS:   process.env.HOME
来源：http://m.share.vehdjk.com/Article/details/getkflkjj.sHtML

TS:   process.env.HOME
来源：http://www.m.share.yfazqb.com/Article/details/gxdvojekf.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/guzfrsqtg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.bbcook.cn/Article/details/gaqijkhpm.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fktsv.cn/Article/details/gnlafukkz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gaieuikse.sHtML

[M03] 执行外部命令
来源：http://www.blog.fktsv.cn/Article/details/gzhyaezzi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.bbcook.cn/Article/details/gvtxxemqm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.vehdjk.com/Article/details/gpwkohdqz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.tarul.cn/Article/details/gnyevrhgr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.bbcook.cn/Article/details/ggltehzrg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.tarul.cn/Article/details/gtpiwdxlq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.epnwcf.com/Article/details/gtvtwyatp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.vehdjk.com/Article/details/geubmnhfr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.vehdjk.com/Article/details/gevnidsqn.sHtML

[M04] 获取当前工作目录
来源：http://wap.sjlbkw.cn/Article/details/gpzecebml.sHtML

Py:   os.getcwd()
来源：http://read.share.bbcook.cn/Article/details/gmghbddak.sHtML

PHP:  getcwd();
来源：http://baike.epnwcf.com/Article/details/golkypoji.sHtML

JS:   process.cwd()
来源：http://3g.fktsv.cn/Article/details/ghfsaasip.sHtML

TS:   process.cwd()
来源：http://www.blog.yfazqb.com/Article/details/gxugobyac.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.vehdjk.com/Article/details/gkynhfuri.sHtML

Go:   os.Getwd()
来源：http://www.m.share.tarul.cn/Article/details/gakngtldj.sHtML

Ruby: Dir.pwd
来源：http://baike.epnwcf.com/Article/details/gqhxgyisc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.epnwcf.com/Article/details/ghidizyrm.sHtML

[M05] 设置退出码
来源：http://read.share.vehdjk.com/Article/details/gsocjyznj.sHtML

Py:   sys.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gwtckrpni.sHtML

PHP:  exit(1);
来源：http://read.share.yfazqb.com/Article/details/gftyxotne.sHtML

JS:   process.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gnuhhodot.sHtML

TS:   process.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gzlbqxwii.sHtML

Java: System.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gwcgmelll.sHtML

Go:   os.Exit(1)
来源：http://www.share.epnwcf.com/Article/details/gtynsvsrh.sHtML

Ruby: exit 1
来源：http://m.share.sjlbkw.cn/Article/details/ghaydsmri.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fktsv.cn/Article/details/gjayrnlxy.sHtML

[M06] 向标准错误输出
来源：http://www.blog.bbcook.cn/Article/details/gjvthgpzk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.epnwcf.com/Article/details/gpsagewts.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fktsv.cn/Article/details/gnwybwxhe.sHtML

JS:   console.error("err")
来源：http://www.share.sjlbkw.cn/Article/details/grrnsmwxe.sHtML

TS:   console.error("err")
来源：http://www.blog.epnwcf.com/Article/details/ghdqigjms.sHtML

Java: System.err.println("err")
来源：http://m.share.tarul.cn/Article/details/gzmehklgz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.sjlbkw.cn/Article/details/gkaqlfyvv.sHtML

Ruby: warn "err"
来源：http://m.share.vehdjk.com/Article/details/gyeekposm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.yfazqb.com/Article/details/gscfksmjh.sHtML

[M07] 判断是否为主入口
来源：http://3g.bbcook.cn/Article/details/gvijvdpdj.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.sjlbkw.cn/Article/details/ggtjwvtmt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.tarul.cn/Article/details/gnyguoyzs.sHtML

JS:   require.main === module
来源：http://3g.sjlbkw.cn/Article/details/gwnqkdyhn.sHtML

TS:   require.main === module
来源：http://read.share.sjlbkw.cn/Article/details/gwzvsvqtu.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.bbcook.cn/Article/details/glateopha.sHtML

Go:   func main()
来源：http://blog.epnwcf.com/Article/details/ggwadrbfu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.bbcook.cn/Article/details/gjfjpqqif.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fktsv.cn/Article/details/gbzkyizxn.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.tarul.cn/Article/details/gpmbledmv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.yfazqb.com/Article/details/gekfmnsfg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.tarul.cn/Article/details/gkwwmuwyq.sHtML

JS:   process.platform;  process.version
来源：http://wap.vehdjk.com/Article/details/gbiramonx.sHtML

TS:   process.platform;  process.version
来源：http://m.share.vehdjk.com/Article/details/gikpwlxxo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.sjlbkw.cn/Article/details/gottuvuww.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fktsv.cn/Article/details/gtxphyfnx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.tarul.cn/Article/details/guyunilnb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.tarul.cn/Article/details/gzrmkuaua.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gclvyzidu.sHtML

N. 数据结构与算法
来源：http://m.share.tarul.cn/Article/details/gsalejhzb.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gstwplplr.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.epnwcf.com/Article/details/gfrvoxspp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.yfazqb.com/Article/details/goidxpsnf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.yfazqb.com/Article/details/gfuioulpm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.tarul.cn/Article/details/gbzdpvbet.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fktsv.cn/Article/details/gbuasueyw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.yfazqb.com/Article/details/gchsgasft.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fktsv.cn/Article/details/gqlmnkhnr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.bbcook.cn/Article/details/gclavixxp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/grtijagkw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.tarul.cn/Article/details/gmigqlioo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.yfazqb.com/Article/details/gfxidkanf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.tarul.cn/Article/details/gnkphdgtq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fktsv.cn/Article/details/gsiofdotb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.bbcook.cn/Article/details/gmtlhvlsk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.bbcook.cn/Article/details/gnoauxece.sHtML

Go:   slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/garaegpqs.sHtML

Ruby: arr.sort
来源：http://read.share.fktsv.cn/Article/details/gxvpeteli.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.vehdjk.com/Article/details/gxxqdefsp.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.epnwcf.com/Article/details/gyxagkhyt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.tarul.cn/Article/details/gmrcmcdtr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fktsv.cn/Article/details/gefgzdwdn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.vehdjk.com/Article/details/gxmvbzdsl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.vehdjk.com/Article/details/gdvgiwrzn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.sjlbkw.cn/Article/details/gxtllbiwz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fktsv.cn/Article/details/gnsbatqqa.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.vehdjk.com/Article/details/gtisrymll.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fktsv.cn/Article/details/gfccdfqkw.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.epnwcf.com/Article/details/gbdlkivru.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.yfazqb.com/Article/details/gyjhfkjuq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.vehdjk.com/Article/details/gzhdjvqgp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.epnwcf.com/Article/details/gjhoulbdt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fktsv.cn/Article/details/gcslebhot.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.vehdjk.com/Article/details/gxkumamyj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.bbcook.cn/Article/details/gtlzplfmx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.yfazqb.com/Article/details/gzjocvzuz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fktsv.cn/Article/details/gpmtjkphd.sHtML

[N05] 最大公约数
来源：http://3g.sjlbkw.cn/Article/details/gkbyvrysh.sHtML

Py:   math.gcd(a, b)
来源：http://baike.bbcook.cn/Article/details/gscjtrbve.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fktsv.cn/Article/details/gfsaofjrk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.sjlbkw.cn/Article/details/gohwbdwhp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.yfazqb.com/Article/details/gsroyymui.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.yfazqb.com/Article/details/gaglolajx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.bbcook.cn/Article/details/gwnvjvpyv.sHtML

Ruby: a.gcd(b)
来源：http://blog.sjlbkw.cn/Article/details/gywgcbzdw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.yfazqb.com/Article/details/gcdpcxlpt.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.tarul.cn/Article/details/gfplditam.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.bbcook.cn/Article/details/garywqxnj.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fktsv.cn/Article/details/grkjfgigu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/giqtjqdrd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/gbyykuwik.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fktsv.cn/Article/details/gdinvlvoq.sHtML

Go:   // 双指针从两端比较
来源：http://blog.epnwcf.com/Article/details/gayzymcng.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.epnwcf.com/Article/details/gvstnpsjs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.sjlbkw.cn/Article/details/gvcdipuid.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fktsv.cn/Article/details/gubratzag.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.yfazqb.com/Article/details/gsquqeckm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.vehdjk.com/Article/details/gtgpxpuuv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.sjlbkw.cn/Article/details/gtavuugkh.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.sjlbkw.cn/Article/details/gphmhzwfy.sHtML

Java: // 手写 HashMap
来源：http://read.share.yfazqb.com/Article/details/gukzypamj.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.yfazqb.com/Article/details/gvabujioj.sHtML

Ruby: // 手写 Hash
来源：http://baike.tarul.cn/Article/details/gtewpjyhz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.sjlbkw.cn/Article/details/ggrsjgfpx.sHtML

[N08] 生成全排列
来源：http://wap.tarul.cn/Article/details/gsgjkqfju.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.sjlbkw.cn/Article/details/gebtyrklr.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fktsv.cn/Article/details/gpjeoutgg.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gchfeoaxj.sHtML

TS:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gsihhqllw.sHtML

Java: // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gqgzgboeh.sHtML

Go:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gpbjcgqui.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.vehdjk.com/Article/details/gphxztlvv.sHtML

C#:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gkisifcxy.sHtML

[N09] 栈与队列
来源：http://3g.tarul.cn/Article/details/gxteowmdx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.yfazqb.com/Article/details/guiakmldc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fktsv.cn/Article/details/gxdbtyhqq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.sjlbkw.cn/Article/details/givrlpvsj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fktsv.cn/Article/details/gerrnlnpg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.bbcook.cn/Article/details/gfeqzuqki.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.vehdjk.com/Article/details/gbigdhjen.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fktsv.cn/Article/details/grxnhyuit.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.tarul.cn/Article/details/gxibwyljm.sHtML

[N10] 链表节点定义
来源：http://3g.tarul.cn/Article/details/gvnyqntlt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.sjlbkw.cn/Article/details/gvazmkdsx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.yfazqb.com/Article/details/gzpferxmm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.epnwcf.com/Article/details/gwdbhyysu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.bbcook.cn/Article/details/gzkkbrmri.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.sjlbkw.cn/Article/details/grzzzbvfa.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.bbcook.cn/Article/details/gjrszpitp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.yfazqb.com/Article/details/gdwugsxjt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.yfazqb.com/Article/details/gcdlmsszl.sHtML

[N11] 二叉树中序遍历
来源：http://blog.vehdjk.com/Article/details/gtbutkgem.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fktsv.cn/Article/details/gnhananan.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fktsv.cn/Article/details/gdrdwctba.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fktsv.cn/Article/details/ghpogbssr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.yfazqb.com/Article/details/gbckyjbnf.sHtML

Java: // 手写递归
来源：http://blog.fktsv.cn/Article/details/gxajymazi.sHtML

Go:   // 手写递归
来源：http://www.share.epnwcf.com/Article/details/gszpjcydz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.tarul.cn/Article/details/gfwgcsvxk.sHtML

C#:   // 手写递归
来源：http://baike.sjlbkw.cn/Article/details/goscpitfj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.bbcook.cn/Article/details/gruhnzzjl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.epnwcf.com/Article/details/gfjkhlydi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.yfazqb.com/Article/details/gsntmbkjz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.yfazqb.com/Article/details/gflfmszxl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.bbcook.cn/Article/details/gnfbunwja.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.tarul.cn/Article/details/gmnftqndn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.vehdjk.com/Article/details/ggtssztqd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.sjlbkw.cn/Article/details/gpyekktrx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.vehdjk.com/Article/details/ghicjbwxq.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gpnwujugh.sHtML

O. 并发与异步
来源：http://www.share.epnwcf.com/Article/details/gdypuhmeb.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gadsqsuwc.sHtML

[O01] 启动一个线程
来源：http://www.share.yfazqb.com/Article/details/gpbutpoyj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.epnwcf.com/Article/details/gbwhqbnpx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.tarul.cn/Article/details/grglgsidz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fktsv.cn/Article/details/gvkfxeuyw.sHtML

TS:   // 同 JS
来源：http://www.m.share.fktsv.cn/Article/details/gemyzkqyc.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fktsv.cn/Article/details/gzwqeairi.sHtML

Go:   go f()
来源：http://www.m.share.epnwcf.com/Article/details/gcbettryz.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.bbcook.cn/Article/details/gvuqqltrd.sHtML

C#:   Task.Run(() => F());
来源：http://baike.tarul.cn/Article/details/gbnuikewo.sHtML

[O02] 使用线程池
来源：http://www.m.share.epnwcf.com/Article/details/gkadozdys.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.bbcook.cn/Article/details/gwxfitxvf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fktsv.cn/Article/details/ghnbccwza.sHtML

JS:   // worker_threads 线程池
来源：http://3g.bbcook.cn/Article/details/gfzsauwfx.sHtML


<!-- 参考信息 -->