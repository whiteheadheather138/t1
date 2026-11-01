代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.epnwcf.com/Article/details/grsquwjui.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.sjlbkw.cn/Article/details/gbzssyjag.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/ggvfolwoq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/ggigzjxwd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.sjlbkw.cn/Article/details/gwirwdtjg.sHtML

[K07] 进制转换
来源：http://www.m.share.tarul.cn/Article/details/ghbdkomxr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gtdfjriiz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.tarul.cn/Article/details/gdbmrvmcv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gonuzphyr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gvpmmvxxn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gvosmdfyt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fktsv.cn/Article/details/gyxfqkovl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.tarul.cn/Article/details/gcebrsurb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gbblmwpax.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.yfazqb.com/Article/details/gglrzatoc.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fktsv.cn/Article/details/ggqdshlrv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.tarul.cn/Article/details/gsdyomqlw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.sjlbkw.cn/Article/details/gnrlovslq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fktsv.cn/Article/details/glnfxbjks.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fktsv.cn/Article/details/gxyjlcich.sHtML

Go:   encoding/gob
来源：http://wap.bbcook.cn/Article/details/gmmrghaii.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.vehdjk.com/Article/details/gtctajgkh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.bbcook.cn/Article/details/gbuhfwghg.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gjnprmnst.sHtML

L. 网络请求
来源：http://mobile.vehdjk.com/Article/details/gtzdigqyy.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gjhfodtzk.sHtML

[L01] 发送 GET 请求
来源：http://blog.sjlbkw.cn/Article/details/gpqcyzydg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.sjlbkw.cn/Article/details/gbjkqrrju.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.yfazqb.com/Article/details/geymplhnm.sHtML

JS:   await fetch(url)
来源：http://mobile.yfazqb.com/Article/details/gyhjhbraf.sHtML

TS:   await fetch(url)
来源：http://www.share.yfazqb.com/Article/details/gkgvgbwty.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.tarul.cn/Article/details/geylwdtxc.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.sjlbkw.cn/Article/details/gydxulhub.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.tarul.cn/Article/details/gskxsysfa.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.sjlbkw.cn/Article/details/gpqxatxnn.sHtML

[L02] 发送 POST JSON
来源：http://m.share.tarul.cn/Article/details/gtgnqmdzi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.sjlbkw.cn/Article/details/gyyfsgsjm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.bbcook.cn/Article/details/gtsesbjqf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.vehdjk.com/Article/details/gvmcvbtbn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fktsv.cn/Article/details/gcmbpzeai.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.sjlbkw.cn/Article/details/gawopodiy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.epnwcf.com/Article/details/gosxumaog.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.sjlbkw.cn/Article/details/gigrhrgew.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.sjlbkw.cn/Article/details/gitajcgwa.sHtML

[L03] 设置自定义请求头
来源：http://mobile.sjlbkw.cn/Article/details/geprtjkpn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.sjlbkw.cn/Article/details/gpbcpjjys.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.yfazqb.com/Article/details/gyutnlsok.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.yfazqb.com/Article/details/gabqwwgkv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.yfazqb.com/Article/details/gcfwxjhwn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.sjlbkw.cn/Article/details/gevqmufjv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.tarul.cn/Article/details/gtjrszwtk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.sjlbkw.cn/Article/details/gepqgvivm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.sjlbkw.cn/Article/details/gtkrrwwja.sHtML

[L04] 设置超时
来源：http://blog.tarul.cn/Article/details/gpunpyzkz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.bbcook.cn/Article/details/gmlvlfayo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.vehdjk.com/Article/details/gzpkjjoar.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.epnwcf.com/Article/details/gyzudxnrf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.tarul.cn/Article/details/gxtsylboe.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.epnwcf.com/Article/details/gnjesgtag.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.sjlbkw.cn/Article/details/gkdqqudph.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.epnwcf.com/Article/details/gxoznzjgf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.vehdjk.com/Article/details/gkhujiqwh.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.sjlbkw.cn/Article/details/gueprezvq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.epnwcf.com/Article/details/golixyonb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.epnwcf.com/Article/details/gtkdvxaic.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.bbcook.cn/Article/details/gukuxnhwq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.epnwcf.com/Article/details/ghenjygyp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fktsv.cn/Article/details/gboteenhj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.sjlbkw.cn/Article/details/gqzmotddm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.bbcook.cn/Article/details/gpyxjlpgg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gujofmzyj.sHtML

[L06] 解析响应为 JSON
来源：http://baike.yfazqb.com/Article/details/gyttewtgv.sHtML

Py:   resp.json()
来源：http://blog.bbcook.cn/Article/details/gopgjcrbo.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.sjlbkw.cn/Article/details/gqxrhzgzg.sHtML

JS:   await resp.json()
来源：http://wap.bbcook.cn/Article/details/gubtumfmr.sHtML

TS:   await resp.json()
来源：http://mobile.bbcook.cn/Article/details/gckbpkapi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.yfazqb.com/Article/details/gnclijhlv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.bbcook.cn/Article/details/gsltuwkag.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.sjlbkw.cn/Article/details/gbkfbjnmc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.vehdjk.com/Article/details/gkxcmesvg.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.vehdjk.com/Article/details/ghrtsnlmy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.tarul.cn/Article/details/gniiunxnp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.epnwcf.com/Article/details/gpthcwdmi.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.vehdjk.com/Article/details/gsfsrawve.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.tarul.cn/Article/details/gtzsaiiah.sHtML

Java: resp.statusCode()
来源：http://read.share.yfazqb.com/Article/details/gyygwubwn.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.yfazqb.com/Article/details/gpbgmfbeg.sHtML

Ruby: resp.code.to_i
来源：http://blog.yfazqb.com/Article/details/gnhdideqf.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.epnwcf.com/Article/details/gymmqlwry.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fktsv.cn/Article/details/gvzvjhpea.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.epnwcf.com/Article/details/gumeuehqh.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.bbcook.cn/Article/details/gyamsfwij.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.sjlbkw.cn/Article/details/gluqabbxy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/gfxzbxpor.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.yfazqb.com/Article/details/grytjcygk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.yfazqb.com/Article/details/guqrrbdag.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.vehdjk.com/Article/details/gcktqjrwz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fktsv.cn/Article/details/giklisjmh.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gaudweshs.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.epnwcf.com/Article/details/gleepedro.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gqlsdceep.sHtML

[M01] 读取命令行参数
来源：http://wap.bbcook.cn/Article/details/ggjewglon.sHtML

Py:   sys.argv[1:]
来源：http://m.share.bbcook.cn/Article/details/gxvpuicrz.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fktsv.cn/Article/details/gthwqihrh.sHtML

JS:   process.argv.slice(2)
来源：http://baike.bbcook.cn/Article/details/gehuhgimx.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.vehdjk.com/Article/details/gygjfzhuj.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.tarul.cn/Article/details/gkrzqnnev.sHtML

Go:   os.Args[1:]
来源：http://www.blog.yfazqb.com/Article/details/geeoftoim.sHtML

Ruby: ARGV
来源：http://read.share.fktsv.cn/Article/details/giaaganll.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.sjlbkw.cn/Article/details/glsjfuusa.sHtML

[M02] 读取环境变量
来源：http://wap.tarul.cn/Article/details/gmgzcszpm.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.epnwcf.com/Article/details/gifqzibxz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.epnwcf.com/Article/details/gdzekxpwh.sHtML

JS:   process.env.HOME
来源：http://mobile.fktsv.cn/Article/details/gnxetmkuc.sHtML

TS:   process.env.HOME
来源：http://m.share.tarul.cn/Article/details/gcmbdrmol.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fktsv.cn/Article/details/gcaeqzezk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.epnwcf.com/Article/details/gbvnabjyg.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.yfazqb.com/Article/details/gbrdiktmy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gacsfjooe.sHtML

[M03] 执行外部命令
来源：http://www.blog.fktsv.cn/Article/details/geaulokmi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.yfazqb.com/Article/details/girwwewlo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fktsv.cn/Article/details/gmeqwhabr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.yfazqb.com/Article/details/gvvgykhhz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.epnwcf.com/Article/details/gqnoepdnv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.epnwcf.com/Article/details/ggxlllrex.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.tarul.cn/Article/details/gzsdcvgxv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.epnwcf.com/Article/details/gvfscgegj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fktsv.cn/Article/details/gseqjwlwc.sHtML

[M04] 获取当前工作目录
来源：http://blog.fktsv.cn/Article/details/gykporhcx.sHtML

Py:   os.getcwd()
来源：http://wap.yfazqb.com/Article/details/gujhogsrm.sHtML

PHP:  getcwd();
来源：http://blog.fktsv.cn/Article/details/gigjotuow.sHtML

JS:   process.cwd()
来源：http://blog.yfazqb.com/Article/details/gmffaxxho.sHtML

TS:   process.cwd()
来源：http://read.share.bbcook.cn/Article/details/glvilzhoa.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.yfazqb.com/Article/details/gnvfabtfk.sHtML

Go:   os.Getwd()
来源：http://wap.epnwcf.com/Article/details/gmrusjfgc.sHtML

Ruby: Dir.pwd
来源：http://mobile.sjlbkw.cn/Article/details/gtzzjytja.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.tarul.cn/Article/details/gvojuqryb.sHtML

[M05] 设置退出码
来源：http://baike.vehdjk.com/Article/details/gfebuidzm.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gslhqaxwf.sHtML

PHP:  exit(1);
来源：http://www.blog.epnwcf.com/Article/details/gyzxascrl.sHtML

JS:   process.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gondyuafm.sHtML

TS:   process.exit(1)
来源：http://wap.epnwcf.com/Article/details/ggnaqcnee.sHtML

Java: System.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gzkjmgxns.sHtML

Go:   os.Exit(1)
来源：http://baike.tarul.cn/Article/details/gwortoicr.sHtML

Ruby: exit 1
来源：http://www.share.sjlbkw.cn/Article/details/gtjufwzxt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.epnwcf.com/Article/details/gvjnvrrrl.sHtML

[M06] 向标准错误输出
来源：http://read.share.tarul.cn/Article/details/gmzfsppvf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.yfazqb.com/Article/details/gqvoqudel.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.bbcook.cn/Article/details/gupfsgbwk.sHtML

JS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/gcqqggycc.sHtML

TS:   console.error("err")
来源：http://www.blog.bbcook.cn/Article/details/gcpfpxzkn.sHtML

Java: System.err.println("err")
来源：http://read.share.bbcook.cn/Article/details/gffaebrud.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.yfazqb.com/Article/details/gmhwocqps.sHtML

Ruby: warn "err"
来源：http://blog.epnwcf.com/Article/details/gphmlxrkp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.bbcook.cn/Article/details/gwlvssvxh.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fktsv.cn/Article/details/gyiqxfwxk.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.yfazqb.com/Article/details/geuknkhyg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.bbcook.cn/Article/details/gtsurdozq.sHtML

JS:   require.main === module
来源：http://3g.yfazqb.com/Article/details/grbnnvjiq.sHtML

TS:   require.main === module
来源：http://3g.sjlbkw.cn/Article/details/glramudbe.sHtML

Java: public static void main(String[] args)
来源：http://baike.bbcook.cn/Article/details/gbnglxmkm.sHtML

Go:   func main()
来源：http://m.share.bbcook.cn/Article/details/gcmdhkosq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fktsv.cn/Article/details/ghhvwrfys.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.bbcook.cn/Article/details/grrvnrmcp.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.sjlbkw.cn/Article/details/gfwqdbwcy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.bbcook.cn/Article/details/gwunnmmiz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.bbcook.cn/Article/details/grskzyofx.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fktsv.cn/Article/details/gypmhrtwx.sHtML

TS:   process.platform;  process.version
来源：http://3g.epnwcf.com/Article/details/godmgfzkm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.yfazqb.com/Article/details/gtjwhdrjf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.vehdjk.com/Article/details/gurlxleae.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.tarul.cn/Article/details/gwqssjbyh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.bbcook.cn/Article/details/gkiaybcwg.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ghbyvlnxg.sHtML

N. 数据结构与算法
来源：http://mobile.bbcook.cn/Article/details/gayfufloo.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/givtfdttd.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fktsv.cn/Article/details/gxboupsnx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/ggmuhhlpz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gizooscen.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gigqzlblk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghlzvhiuo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gxnxmalxt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.epnwcf.com/Article/details/gdtdjvfmu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fktsv.cn/Article/details/ghebgygac.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.vehdjk.com/Article/details/gtvkcskor.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fktsv.cn/Article/details/gvjrmfvmv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.sjlbkw.cn/Article/details/gwzatpkme.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.vehdjk.com/Article/details/ggvaiuomj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.bbcook.cn/Article/details/gkbcfyutq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/goovrkain.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.epnwcf.com/Article/details/gwdllixxf.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.tarul.cn/Article/details/gggwrhuzf.sHtML

Ruby: arr.sort
来源：http://wap.yfazqb.com/Article/details/gpqstrvpy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.sjlbkw.cn/Article/details/gsylnkmey.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fktsv.cn/Article/details/gezssdorj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.bbcook.cn/Article/details/gjvxyhnlp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdztevhy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.tarul.cn/Article/details/gqhlwfpko.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.vehdjk.com/Article/details/gwyyceuvu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.vehdjk.com/Article/details/gavojsadv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.sjlbkw.cn/Article/details/gvrryogvc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.epnwcf.com/Article/details/glvalkdom.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.epnwcf.com/Article/details/gnjzsvaua.sHtML

[N04] 斐波那契数列
来源：http://www.share.fktsv.cn/Article/details/gojjucmmn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.bbcook.cn/Article/details/gfiaksfxp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.yfazqb.com/Article/details/gihejbprc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.sjlbkw.cn/Article/details/gvlqcbomr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/gyckeeejl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.vehdjk.com/Article/details/gfrdgvhlg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.sjlbkw.cn/Article/details/gchadbtud.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.yfazqb.com/Article/details/gwqiysgtr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/govelumal.sHtML

[N05] 最大公约数
来源：http://wap.sjlbkw.cn/Article/details/gbjjzxjvb.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.vehdjk.com/Article/details/gevzkiuaq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.sjlbkw.cn/Article/details/gbxsimmbb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.tarul.cn/Article/details/gybukjijs.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.yfazqb.com/Article/details/gzbvpoxwh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fktsv.cn/Article/details/glayqqnts.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.yfazqb.com/Article/details/gasjfzvho.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fktsv.cn/Article/details/glnotvbii.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.epnwcf.com/Article/details/ggoslblbi.sHtML

[N06] 判断回文字符串
来源：http://read.share.bbcook.cn/Article/details/gllvqcsyy.sHtML

Py:   s == s[::-1]
来源：http://3g.bbcook.cn/Article/details/ggldcgpzb.sHtML

PHP:  $s === strrev($s);
来源：http://baike.bbcook.cn/Article/details/gdhiocqde.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gftphvqti.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/goatmbjhg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.yfazqb.com/Article/details/gtdmdggjt.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.tarul.cn/Article/details/gpujwbwva.sHtML

Ruby: s == s.reverse
来源：http://3g.epnwcf.com/Article/details/gvhoalylo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.tarul.cn/Article/details/gipebzdup.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fktsv.cn/Article/details/gmwkzttjj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fktsv.cn/Article/details/gzdfnklmb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.bbcook.cn/Article/details/gpoqdsgmo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.yfazqb.com/Article/details/gekmccvct.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.tarul.cn/Article/details/gggbftskg.sHtML

Java: // 手写 HashMap
来源：http://blog.tarul.cn/Article/details/gyowfkfug.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.yfazqb.com/Article/details/gwcnkxlnk.sHtML

Ruby: // 手写 Hash
来源：http://m.share.bbcook.cn/Article/details/gzjfaadkh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.tarul.cn/Article/details/gpqddkmfk.sHtML

[N08] 生成全排列
来源：http://www.blog.bbcook.cn/Article/details/graxqjqty.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gsbkciswe.sHtML

PHP:  // 手写递归交换
来源：http://mobile.tarul.cn/Article/details/gfpibyjwk.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gndbqqfid.sHtML

TS:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gaosjumah.sHtML

Java: // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gfwbojuhr.sHtML

Go:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/grdebepux.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.epnwcf.com/Article/details/gdqcqwciy.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gjijicjli.sHtML

[N09] 栈与队列
来源：http://wap.fktsv.cn/Article/details/gsbaxztne.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.vehdjk.com/Article/details/gywdqyqur.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gaxwggujr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.tarul.cn/Article/details/glsapxrey.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.tarul.cn/Article/details/gzqnaswmb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.tarul.cn/Article/details/gmhzvhtyu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fktsv.cn/Article/details/ggtotqslw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.sjlbkw.cn/Article/details/gwbfgvabf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fktsv.cn/Article/details/gbvbxrrbk.sHtML

[N10] 链表节点定义
来源：http://wap.vehdjk.com/Article/details/gtgyvqkts.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.yfazqb.com/Article/details/gkszzkncm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.vehdjk.com/Article/details/gxhfhtsse.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.tarul.cn/Article/details/gshtpfqsp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.tarul.cn/Article/details/ghqhcgfin.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.yfazqb.com/Article/details/gjnloopwp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.tarul.cn/Article/details/gunueprio.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.sjlbkw.cn/Article/details/gypigodxu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.epnwcf.com/Article/details/gvfsvcxgc.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fktsv.cn/Article/details/gwjbipinr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.bbcook.cn/Article/details/gvrulhbwi.sHtML

PHP:  // 手写递归函数
来源：http://blog.bbcook.cn/Article/details/gxwqdzdhx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.yfazqb.com/Article/details/gdbwzzgof.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.vehdjk.com/Article/details/grfjuyabn.sHtML

Java: // 手写递归
来源：http://baike.tarul.cn/Article/details/gleuhcmzf.sHtML

Go:   // 手写递归
来源：http://www.share.tarul.cn/Article/details/gwryeapgk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.sjlbkw.cn/Article/details/gvkxfhoud.sHtML

C#:   // 手写递归
来源：http://mobile.vehdjk.com/Article/details/gmppevgbv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.vehdjk.com/Article/details/gkpbmkpgv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.sjlbkw.cn/Article/details/gsjvxdkfw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.epnwcf.com/Article/details/gmeusokob.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fktsv.cn/Article/details/gpifammxi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.sjlbkw.cn/Article/details/gblcxqnrp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fktsv.cn/Article/details/gcdmgwvhn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.tarul.cn/Article/details/gtatmbudr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.yfazqb.com/Article/details/gclenocxo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fktsv.cn/Article/details/gktmpfgah.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gygjwuzwm.sHtML

O. 并发与异步
来源：http://wap.yfazqb.com/Article/details/gxvptqvwc.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gttxwopls.sHtML

[O01] 启动一个线程
来源：http://www.m.share.epnwcf.com/Article/details/gqendlsvz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.yfazqb.com/Article/details/grtwggcan.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.vehdjk.com/Article/details/gbdfekkqm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fktsv.cn/Article/details/gzdigxpwg.sHtML

TS:   // 同 JS
来源：http://blog.tarul.cn/Article/details/gwxyyzrxg.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.bbcook.cn/Article/details/gexmgwnno.sHtML

Go:   go f()
来源：http://read.share.epnwcf.com/Article/details/gsfzvqhcc.sHtML

Ruby: Thread.new { f }
来源：http://www.share.tarul.cn/Article/details/gllceppjg.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.sjlbkw.cn/Article/details/gsbnrswkm.sHtML

[O02] 使用线程池
来源：http://www.m.share.tarul.cn/Article/details/gnyddwmdl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.bbcook.cn/Article/details/gqcyfwesz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.sjlbkw.cn/Article/details/glztmrjnh.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.bbcook.cn/Article/details/ghxrafhlr.sHtML


<!-- 参考信息 -->