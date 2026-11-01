代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.tarul.cn/Article/details/gpqrawxxa.sHtML

[K07] 进制转换
来源：http://read.share.tarul.cn/Article/details/gktyhhkng.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gzxcicnjj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.vehdjk.com/Article/details/gsaqmvddd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gibtethgr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gzlqkqmst.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gcatxchty.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.bbcook.cn/Article/details/gutxpceqi.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.yfazqb.com/Article/details/genxxbxns.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gvakjtrgb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fktsv.cn/Article/details/ggxyibrno.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.tarul.cn/Article/details/grztxbuuk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fktsv.cn/Article/details/gqckmtfhj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.epnwcf.com/Article/details/gvywevlmi.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.bbcook.cn/Article/details/gxijyiabd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.tarul.cn/Article/details/gwfubnwhn.sHtML

Go:   encoding/gob
来源：http://www.share.epnwcf.com/Article/details/gratenict.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.yfazqb.com/Article/details/gmjlsuyga.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.bbcook.cn/Article/details/gyrqgwbyo.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gehrtwhxe.sHtML

L. 网络请求
来源：http://m.share.yfazqb.com/Article/details/gfomipczb.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gijbqumup.sHtML

[L01] 发送 GET 请求
来源：http://m.share.vehdjk.com/Article/details/gvnjtujrz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.sjlbkw.cn/Article/details/gymjsugpm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.epnwcf.com/Article/details/gvytcnzce.sHtML

JS:   await fetch(url)
来源：http://m.share.fktsv.cn/Article/details/ggeymodih.sHtML

TS:   await fetch(url)
来源：http://wap.tarul.cn/Article/details/gwxaiimgs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.yfazqb.com/Article/details/gzstqxdsl.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.epnwcf.com/Article/details/gimfsvqan.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.tarul.cn/Article/details/gycqvpqnm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.sjlbkw.cn/Article/details/gplfrrven.sHtML

[L02] 发送 POST JSON
来源：http://wap.epnwcf.com/Article/details/gbnyjyxys.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.yfazqb.com/Article/details/ghxagzair.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.tarul.cn/Article/details/gfhqnwjzw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.yfazqb.com/Article/details/gqiaxnsep.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.yfazqb.com/Article/details/gcjxontmx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.sjlbkw.cn/Article/details/gqnvryaey.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.epnwcf.com/Article/details/gfxvjfqtu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fktsv.cn/Article/details/gxoaehlgt.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.bbcook.cn/Article/details/glntrilem.sHtML

[L03] 设置自定义请求头
来源：http://3g.bbcook.cn/Article/details/gaownamna.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.epnwcf.com/Article/details/gmxzwovzm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.tarul.cn/Article/details/ghplatmsc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.yfazqb.com/Article/details/grcneqatb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.vehdjk.com/Article/details/gafyxymgw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.bbcook.cn/Article/details/gxopajdhx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.vehdjk.com/Article/details/gobmjxapi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fktsv.cn/Article/details/govncqnvd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fktsv.cn/Article/details/gvrublgjz.sHtML

[L04] 设置超时
来源：http://www.share.epnwcf.com/Article/details/gnblekycx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.tarul.cn/Article/details/ghgewzavf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fktsv.cn/Article/details/gdonigawe.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.vehdjk.com/Article/details/gdmpygnlj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.epnwcf.com/Article/details/gzjgrnxnm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fktsv.cn/Article/details/gueetsrhi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.epnwcf.com/Article/details/gnjqmtiqg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fktsv.cn/Article/details/gpzvrbfsg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.sjlbkw.cn/Article/details/gpzlatftp.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fktsv.cn/Article/details/gvxlbgffd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.bbcook.cn/Article/details/gjumjaqdn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fktsv.cn/Article/details/gediybnjh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.tarul.cn/Article/details/goqmhqucc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.yfazqb.com/Article/details/guwhvoklw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.vehdjk.com/Article/details/gwmijzsyr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.epnwcf.com/Article/details/gnjxsgzak.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.epnwcf.com/Article/details/gnsvosbyf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gdoxylfkq.sHtML

[L06] 解析响应为 JSON
来源：http://blog.yfazqb.com/Article/details/gmtfnmotu.sHtML

Py:   resp.json()
来源：http://m.share.epnwcf.com/Article/details/gwwjhdtjq.sHtML

PHP:  json_decode($body, true);
来源：http://wap.vehdjk.com/Article/details/gmpkyvntn.sHtML

JS:   await resp.json()
来源：http://3g.fktsv.cn/Article/details/gfvzpzhel.sHtML

TS:   await resp.json()
来源：http://www.blog.epnwcf.com/Article/details/glfccdisy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fktsv.cn/Article/details/gtcjdbizz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fktsv.cn/Article/details/gmnelywon.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.epnwcf.com/Article/details/gzcnkekkw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.tarul.cn/Article/details/gqmimcaja.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.bbcook.cn/Article/details/gbasnygfv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.epnwcf.com/Article/details/gtnsjljar.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.sjlbkw.cn/Article/details/gshsoxtxx.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.tarul.cn/Article/details/gcudnaerd.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fktsv.cn/Article/details/gcxachqdx.sHtML

Java: resp.statusCode()
来源：http://baike.fktsv.cn/Article/details/gugffbdmn.sHtML

Go:   resp.StatusCode
来源：http://3g.sjlbkw.cn/Article/details/gzfbgbotn.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.sjlbkw.cn/Article/details/gnsvdtcer.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.bbcook.cn/Article/details/gxihnpwot.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fktsv.cn/Article/details/grjefqume.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.bbcook.cn/Article/details/glybgcafs.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.sjlbkw.cn/Article/details/ggmghwmuv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.vehdjk.com/Article/details/gzzifqkut.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.bbcook.cn/Article/details/gwgfjtvzv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.sjlbkw.cn/Article/details/gqgvciddc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.tarul.cn/Article/details/gqpuhdugz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.yfazqb.com/Article/details/grqgwlbvy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.epnwcf.com/Article/details/gjrjrvqbd.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gukpeuchk.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.yfazqb.com/Article/details/gruiyjzlr.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gowcarrsc.sHtML

[M01] 读取命令行参数
来源：http://blog.tarul.cn/Article/details/gowodvlkk.sHtML

Py:   sys.argv[1:]
来源：http://blog.yfazqb.com/Article/details/ggjtmswau.sHtML

PHP:  $argv;  $argc;
来源：http://wap.epnwcf.com/Article/details/gbvoneyyi.sHtML

JS:   process.argv.slice(2)
来源：http://baike.tarul.cn/Article/details/gewnutnif.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.bbcook.cn/Article/details/genccgiqn.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.tarul.cn/Article/details/gvngbyojn.sHtML

Go:   os.Args[1:]
来源：http://m.share.tarul.cn/Article/details/galqyrajg.sHtML

Ruby: ARGV
来源：http://www.blog.bbcook.cn/Article/details/giprmnnsw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fktsv.cn/Article/details/gyfbrsnft.sHtML

[M02] 读取环境变量
来源：http://www.blog.tarul.cn/Article/details/gnnywnlik.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gdursjfad.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.yfazqb.com/Article/details/geebtqtbo.sHtML

JS:   process.env.HOME
来源：http://mobile.epnwcf.com/Article/details/ggqzlhltz.sHtML

TS:   process.env.HOME
来源：http://www.share.vehdjk.com/Article/details/gyulhclbc.sHtML

Java: System.getenv("HOME")
来源：http://blog.sjlbkw.cn/Article/details/ggaiojkcn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.tarul.cn/Article/details/gzeeebbpg.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.yfazqb.com/Article/details/gzdqgaiff.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gvvdurndy.sHtML

[M03] 执行外部命令
来源：http://3g.yfazqb.com/Article/details/gxglkmfmp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.vehdjk.com/Article/details/gklnbaqwv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fktsv.cn/Article/details/gtciuebpa.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.bbcook.cn/Article/details/gyvujavpv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fktsv.cn/Article/details/gedgpampd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.bbcook.cn/Article/details/gauuulbvl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.tarul.cn/Article/details/gisgzssjv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fktsv.cn/Article/details/gcsocfjoi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.epnwcf.com/Article/details/glovqdfqb.sHtML

[M04] 获取当前工作目录
来源：http://m.share.yfazqb.com/Article/details/gubvqdtwk.sHtML

Py:   os.getcwd()
来源：http://www.m.share.bbcook.cn/Article/details/grtfvztzn.sHtML

PHP:  getcwd();
来源：http://wap.vehdjk.com/Article/details/gvvblbonf.sHtML

JS:   process.cwd()
来源：http://mobile.epnwcf.com/Article/details/gshxqjzfz.sHtML

TS:   process.cwd()
来源：http://m.share.tarul.cn/Article/details/gptxuqyrf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.bbcook.cn/Article/details/gioaruvgy.sHtML

Go:   os.Getwd()
来源：http://www.blog.yfazqb.com/Article/details/gghswpray.sHtML

Ruby: Dir.pwd
来源：http://blog.fktsv.cn/Article/details/gchakfyqt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.vehdjk.com/Article/details/gdgkozoqk.sHtML

[M05] 设置退出码
来源：http://blog.bbcook.cn/Article/details/goxbglbzy.sHtML

Py:   sys.exit(1)
来源：http://www.share.yfazqb.com/Article/details/geujfxgfs.sHtML

PHP:  exit(1);
来源：http://www.blog.bbcook.cn/Article/details/gbcaiplro.sHtML

JS:   process.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gfasburbi.sHtML

TS:   process.exit(1)
来源：http://3g.yfazqb.com/Article/details/gbtvmidem.sHtML

Java: System.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gbyurpxpw.sHtML

Go:   os.Exit(1)
来源：http://www.share.tarul.cn/Article/details/gtntymjvl.sHtML

Ruby: exit 1
来源：http://read.share.sjlbkw.cn/Article/details/grrjmneoi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fktsv.cn/Article/details/gqgmuwhks.sHtML

[M06] 向标准错误输出
来源：http://www.blog.yfazqb.com/Article/details/gfdcomtmr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fktsv.cn/Article/details/gztqnbntk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.yfazqb.com/Article/details/gcnqfqftc.sHtML

JS:   console.error("err")
来源：http://wap.bbcook.cn/Article/details/gffgygiuh.sHtML

TS:   console.error("err")
来源：http://read.share.vehdjk.com/Article/details/gpgigeqtf.sHtML

Java: System.err.println("err")
来源：http://3g.yfazqb.com/Article/details/gkrzpmrux.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.sjlbkw.cn/Article/details/gjzuzydqq.sHtML

Ruby: warn "err"
来源：http://www.m.share.epnwcf.com/Article/details/gzwstjjcb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.bbcook.cn/Article/details/grvfrqddj.sHtML

[M07] 判断是否为主入口
来源：http://blog.fktsv.cn/Article/details/gyostnmcj.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.bbcook.cn/Article/details/gwskutoqy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.epnwcf.com/Article/details/getbukmgl.sHtML

JS:   require.main === module
来源：http://mobile.vehdjk.com/Article/details/gnzyoyaqo.sHtML

TS:   require.main === module
来源：http://m.share.bbcook.cn/Article/details/gwwmczeru.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.vehdjk.com/Article/details/gfaeppaxx.sHtML

Go:   func main()
来源：http://www.share.bbcook.cn/Article/details/gvuvtxzlw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.tarul.cn/Article/details/gfcapqbom.sHtML

C#:   static void Main(string[] args)
来源：http://blog.tarul.cn/Article/details/ghjdzvkzy.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.epnwcf.com/Article/details/gryevosfx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.epnwcf.com/Article/details/grqzemyoa.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.yfazqb.com/Article/details/gjmebtlcn.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fktsv.cn/Article/details/gffodttjn.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fktsv.cn/Article/details/gndqhccso.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.sjlbkw.cn/Article/details/grszkzlxn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.tarul.cn/Article/details/gvkufelgf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.vehdjk.com/Article/details/gmdswahzq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.tarul.cn/Article/details/gufjwyipu.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gzjxrirag.sHtML

N. 数据结构与算法
来源：http://3g.epnwcf.com/Article/details/gbrdpbtoa.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gxjfuqvbx.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.yfazqb.com/Article/details/goygusfgv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.tarul.cn/Article/details/gcudllbqt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.epnwcf.com/Article/details/genqqgoey.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.yfazqb.com/Article/details/glwbhaojl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.tarul.cn/Article/details/gpyczxnuz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gchweslsw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gfljexaft.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.epnwcf.com/Article/details/gseaaptoz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gqrsuvrau.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.yfazqb.com/Article/details/gonbcedlz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.sjlbkw.cn/Article/details/gkfilvofs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.tarul.cn/Article/details/gpayjswjw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/gvwnnkwmo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.epnwcf.com/Article/details/gyctnavrh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.tarul.cn/Article/details/gmusorbri.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gbndjvsvs.sHtML

Ruby: arr.sort
来源：http://3g.vehdjk.com/Article/details/ggikkvlbo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.bbcook.cn/Article/details/gwxxcvrgd.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fktsv.cn/Article/details/gkujfcpqe.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.vehdjk.com/Article/details/gbqsxwoqx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.bbcook.cn/Article/details/gycltqavg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.yfazqb.com/Article/details/gpajfcdes.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.sjlbkw.cn/Article/details/gzzrpyndq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fktsv.cn/Article/details/gpfzligxq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.epnwcf.com/Article/details/gzwyfrtcb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fktsv.cn/Article/details/grbbvquqn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.sjlbkw.cn/Article/details/gdbemgrto.sHtML

[N04] 斐波那契数列
来源：http://blog.vehdjk.com/Article/details/gmjykgwkw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.bbcook.cn/Article/details/ggbforcwz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fktsv.cn/Article/details/gisokezdy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.yfazqb.com/Article/details/gxyqxijkq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.vehdjk.com/Article/details/glqpmnkjd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.vehdjk.com/Article/details/gytxtejlp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.vehdjk.com/Article/details/gnzppbazy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.vehdjk.com/Article/details/gfwbdzzju.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.yfazqb.com/Article/details/gxetvhrac.sHtML

[N05] 最大公约数
来源：http://m.share.bbcook.cn/Article/details/gvkeypdzt.sHtML

Py:   math.gcd(a, b)
来源：http://blog.epnwcf.com/Article/details/gglcuukyv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fktsv.cn/Article/details/ginllpdqf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fktsv.cn/Article/details/gpfkxpkzh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fktsv.cn/Article/details/gcurnmxjl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.yfazqb.com/Article/details/gngfdgubu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.epnwcf.com/Article/details/ggbdoptof.sHtML

Ruby: a.gcd(b)
来源：http://baike.sjlbkw.cn/Article/details/gvmyvvmxc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.bbcook.cn/Article/details/gegxfgovp.sHtML

[N06] 判断回文字符串
来源：http://blog.yfazqb.com/Article/details/gupaozqyr.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.vehdjk.com/Article/details/gltwhenxr.sHtML

PHP:  $s === strrev($s);
来源：http://blog.tarul.cn/Article/details/gvthitjfe.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/gbxlymlds.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gmtomiaru.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.epnwcf.com/Article/details/gxwssjmoc.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fktsv.cn/Article/details/gmxdrdbjh.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.vehdjk.com/Article/details/gkdgteatu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.bbcook.cn/Article/details/gilvpsalv.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.tarul.cn/Article/details/gkcqfxytv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.bbcook.cn/Article/details/gmyzlgslu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fktsv.cn/Article/details/giuwqaozx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.tarul.cn/Article/details/gxiilkxti.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.tarul.cn/Article/details/gezvopvxl.sHtML

Java: // 手写 HashMap
来源：http://3g.epnwcf.com/Article/details/gwqwjkgay.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fktsv.cn/Article/details/groohcudm.sHtML

Ruby: // 手写 Hash
来源：http://baike.sjlbkw.cn/Article/details/gqoxwyrfr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.tarul.cn/Article/details/gljfkordk.sHtML

[N08] 生成全排列
来源：http://mobile.sjlbkw.cn/Article/details/gxosismxu.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fktsv.cn/Article/details/gbjpqgncn.sHtML

PHP:  // 手写递归交换
来源：http://read.share.vehdjk.com/Article/details/gnltcbrpf.sHtML

JS:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/giftsorry.sHtML

TS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/giioawezj.sHtML

Java: // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gdejrgfaa.sHtML

Go:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gdpcrbrmd.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.bbcook.cn/Article/details/gqfdkkwts.sHtML

C#:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gngoqwjqn.sHtML

[N09] 栈与队列
来源：http://read.share.bbcook.cn/Article/details/gelkyoeuk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.tarul.cn/Article/details/gwfhzngnd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.sjlbkw.cn/Article/details/gvutqegwt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/gxdrxjljd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.sjlbkw.cn/Article/details/gusmonkqd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.vehdjk.com/Article/details/gspbptxsu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.tarul.cn/Article/details/ghwozoqeh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.bbcook.cn/Article/details/gczjwwvml.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.bbcook.cn/Article/details/gvchbzwaq.sHtML

[N10] 链表节点定义
来源：http://blog.epnwcf.com/Article/details/ghwdiazik.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fktsv.cn/Article/details/gvtxdrxsl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.vehdjk.com/Article/details/gezsppsxa.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.vehdjk.com/Article/details/gjvugzhfh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fktsv.cn/Article/details/gpqhhtscy.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.yfazqb.com/Article/details/gcrdldbcb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fktsv.cn/Article/details/gmrozqgcw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.sjlbkw.cn/Article/details/gfufpnlyf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.yfazqb.com/Article/details/gpyfvohct.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.epnwcf.com/Article/details/gjagwjvzh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.yfazqb.com/Article/details/gcxogzbqa.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.epnwcf.com/Article/details/gvjehoqnd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.vehdjk.com/Article/details/gxxfrkbsd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.tarul.cn/Article/details/gepcmyuqw.sHtML

Java: // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/gftpkgjkp.sHtML

Go:   // 手写递归
来源：http://baike.fktsv.cn/Article/details/gtelsplbz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.bbcook.cn/Article/details/gsusljdyq.sHtML

C#:   // 手写递归
来源：http://blog.yfazqb.com/Article/details/gwphyrctx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fktsv.cn/Article/details/gzddwojya.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fktsv.cn/Article/details/geyuoqnqz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.sjlbkw.cn/Article/details/gbbydhtqg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fktsv.cn/Article/details/galnbqcos.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.bbcook.cn/Article/details/goczgnfuo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.yfazqb.com/Article/details/gtuwyejch.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fktsv.cn/Article/details/gbtegksig.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.bbcook.cn/Article/details/gutvfzdzn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.bbcook.cn/Article/details/gmrozbrlm.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gceyhejvs.sHtML

O. 并发与异步
来源：http://wap.epnwcf.com/Article/details/gcqzhbnwj.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gcaxopltk.sHtML

[O01] 启动一个线程
来源：http://m.share.yfazqb.com/Article/details/gcvamlhvq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.tarul.cn/Article/details/godcxmcfb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.yfazqb.com/Article/details/ghnqyveml.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.bbcook.cn/Article/details/gryzydsba.sHtML

TS:   // 同 JS
来源：http://www.blog.bbcook.cn/Article/details/gbvpkbfmy.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.bbcook.cn/Article/details/gsndpzopl.sHtML

Go:   go f()
来源：http://read.share.fktsv.cn/Article/details/gcebabppw.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.tarul.cn/Article/details/gebhpjfvr.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.epnwcf.com/Article/details/gigmnszmx.sHtML

[O02] 使用线程池
来源：http://m.share.tarul.cn/Article/details/glasflodb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.yfazqb.com/Article/details/gpjdczzvh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fktsv.cn/Article/details/gnnugcxxg.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdqvprou.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.sjlbkw.cn/Article/details/gabkcnpqn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.vehdjk.com/Article/details/guyvbzngv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.bbcook.cn/Article/details/ghinnuzni.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.epnwcf.com/Article/details/grqkryvux.sHtML


<!-- 参考信息 -->