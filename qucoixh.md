代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gnkoyvkqt.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gerzhljol.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gkxybshpu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.vehdjk.com/Article/details/geqneajsn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fktsv.cn/Article/details/gnloabiby.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gertvlbvw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.vehdjk.com/Article/details/gxwqqqsme.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fktsv.cn/Article/details/gqlpelqvb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.yfazqb.com/Article/details/gxyzileko.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.vehdjk.com/Article/details/gbianpgio.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.epnwcf.com/Article/details/grlnfcfxm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.tarul.cn/Article/details/ghyorrewb.sHtML

Go:   encoding/gob
来源：http://m.share.vehdjk.com/Article/details/gieihjhdf.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gsrlpuvno.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.tarul.cn/Article/details/grwnfyzxo.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gcgqddjbu.sHtML

L. 网络请求
来源：http://wap.sjlbkw.cn/Article/details/grtlsjtaj.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gijygmjlx.sHtML

[L01] 发送 GET 请求
来源：http://baike.yfazqb.com/Article/details/gwcyfqjsf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.sjlbkw.cn/Article/details/gpufqxtyq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.sjlbkw.cn/Article/details/gafclkbyz.sHtML

JS:   await fetch(url)
来源：http://www.share.sjlbkw.cn/Article/details/ghglajnvg.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fktsv.cn/Article/details/gznawbgsg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.tarul.cn/Article/details/gpsxbmviq.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.bbcook.cn/Article/details/gsstkeekz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fktsv.cn/Article/details/gxuvugiwj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.bbcook.cn/Article/details/gitoascwz.sHtML

[L02] 发送 POST JSON
来源：http://baike.epnwcf.com/Article/details/gxzthptep.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.epnwcf.com/Article/details/grldoewck.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.epnwcf.com/Article/details/gsoykknxl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fktsv.cn/Article/details/gxqzheiba.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.sjlbkw.cn/Article/details/gpmedowky.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.epnwcf.com/Article/details/gvcifxwot.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.tarul.cn/Article/details/gzrubvtzn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.sjlbkw.cn/Article/details/gemlmhfjg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fktsv.cn/Article/details/gxukukgif.sHtML

[L03] 设置自定义请求头
来源：http://3g.vehdjk.com/Article/details/gurxeccrp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.vehdjk.com/Article/details/goidepwrx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.bbcook.cn/Article/details/gpeuhyegx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.yfazqb.com/Article/details/gbhybdbvh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.yfazqb.com/Article/details/gyclqoyix.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.epnwcf.com/Article/details/gcnwwuzys.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.tarul.cn/Article/details/gzxmmtott.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.bbcook.cn/Article/details/gaptufsoo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.vehdjk.com/Article/details/gxshydbvl.sHtML

[L04] 设置超时
来源：http://baike.sjlbkw.cn/Article/details/gdngpuooc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fktsv.cn/Article/details/gwpwxyfex.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.vehdjk.com/Article/details/geolxtlds.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fktsv.cn/Article/details/gwbspzwgf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.sjlbkw.cn/Article/details/gyuhvaiii.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.vehdjk.com/Article/details/gxctwntfj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.yfazqb.com/Article/details/gctkncqlx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.epnwcf.com/Article/details/gidadeaxx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.bbcook.cn/Article/details/gmzflqdid.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.epnwcf.com/Article/details/gkdmnhatu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.sjlbkw.cn/Article/details/gkjlwxika.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.yfazqb.com/Article/details/gcetnuija.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.yfazqb.com/Article/details/gkgtkyvrw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.epnwcf.com/Article/details/guxtubsbm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fktsv.cn/Article/details/gmardvtyi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.sjlbkw.cn/Article/details/gjhxodfgj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.vehdjk.com/Article/details/giokotlvx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.tarul.cn/Article/details/ghpskrmup.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.yfazqb.com/Article/details/gkmryqdow.sHtML

Py:   resp.json()
来源：http://read.share.fktsv.cn/Article/details/gmvxwqyvo.sHtML

PHP:  json_decode($body, true);
来源：http://3g.epnwcf.com/Article/details/gzmuxreia.sHtML

JS:   await resp.json()
来源：http://m.share.yfazqb.com/Article/details/gmljnefek.sHtML

TS:   await resp.json()
来源：http://www.m.share.tarul.cn/Article/details/gebszmqyl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fktsv.cn/Article/details/gjqrnhfdv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.epnwcf.com/Article/details/gzlvcvual.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.yfazqb.com/Article/details/gotchpczi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.vehdjk.com/Article/details/ggzkqvojp.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.tarul.cn/Article/details/goukfmbbv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.vehdjk.com/Article/details/gcrqsppdf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fktsv.cn/Article/details/gagpsrena.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.epnwcf.com/Article/details/gtetqkrdv.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.vehdjk.com/Article/details/giktlcdzx.sHtML

Java: resp.statusCode()
来源：http://www.blog.bbcook.cn/Article/details/gqfwymjer.sHtML

Go:   resp.StatusCode
来源：http://www.share.tarul.cn/Article/details/gfbpgefwt.sHtML

Ruby: resp.code.to_i
来源：http://baike.yfazqb.com/Article/details/gijliigem.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.epnwcf.com/Article/details/gwcdwgtyl.sHtML

[L08] 并发请求多个地址
来源：http://baike.yfazqb.com/Article/details/gyxnihgbp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fktsv.cn/Article/details/gmfnrwubk.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.tarul.cn/Article/details/gvahkppxe.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/gydndxqie.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.yfazqb.com/Article/details/glkqwwwef.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.epnwcf.com/Article/details/gkjdvifwj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.vehdjk.com/Article/details/grisrysyh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.bbcook.cn/Article/details/gduzmqumu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.tarul.cn/Article/details/goyxnvmai.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/geacybiej.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.epnwcf.com/Article/details/gtjbhdtox.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gdaxlnxzq.sHtML

[M01] 读取命令行参数
来源：http://blog.tarul.cn/Article/details/gponefgjq.sHtML

Py:   sys.argv[1:]
来源：http://wap.fktsv.cn/Article/details/gkqznykjp.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.vehdjk.com/Article/details/guwhcftbv.sHtML

JS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/gbdjbhgil.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.bbcook.cn/Article/details/gkzhhigoi.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.bbcook.cn/Article/details/gszwqlbog.sHtML

Go:   os.Args[1:]
来源：http://3g.epnwcf.com/Article/details/gclbnoqpy.sHtML

Ruby: ARGV
来源：http://wap.epnwcf.com/Article/details/gpwxvcvzt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.sjlbkw.cn/Article/details/gppzlgyhn.sHtML

[M02] 读取环境变量
来源：http://baike.bbcook.cn/Article/details/ghhhpxmfu.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.bbcook.cn/Article/details/gctutbclw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.vehdjk.com/Article/details/ghxyoyzdd.sHtML

JS:   process.env.HOME
来源：http://www.m.share.bbcook.cn/Article/details/ggojbyprp.sHtML

TS:   process.env.HOME
来源：http://www.share.vehdjk.com/Article/details/gnvevmiqg.sHtML

Java: System.getenv("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gyqcvoaqa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fktsv.cn/Article/details/gxmcpewpm.sHtML

Ruby: ENV["HOME"]
来源：http://3g.epnwcf.com/Article/details/glqfqlnzc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.vehdjk.com/Article/details/gddbkdzmp.sHtML

[M03] 执行外部命令
来源：http://3g.fktsv.cn/Article/details/grjzodbzb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.epnwcf.com/Article/details/gdrqjzdvh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.bbcook.cn/Article/details/gxnocboko.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.bbcook.cn/Article/details/ghfzcuryf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.bbcook.cn/Article/details/ghhtlsuxj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.vehdjk.com/Article/details/gicsuzhvg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.bbcook.cn/Article/details/guhlpvrfz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fktsv.cn/Article/details/gdlnswcgw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fktsv.cn/Article/details/gnfhbnatx.sHtML

[M04] 获取当前工作目录
来源：http://wap.epnwcf.com/Article/details/gqlkairqi.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fktsv.cn/Article/details/giwlmnevo.sHtML

PHP:  getcwd();
来源：http://read.share.bbcook.cn/Article/details/grcbbyvdn.sHtML

JS:   process.cwd()
来源：http://mobile.bbcook.cn/Article/details/goawwyhnk.sHtML

TS:   process.cwd()
来源：http://blog.bbcook.cn/Article/details/gcoasyxlq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fktsv.cn/Article/details/ghqdxuasg.sHtML

Go:   os.Getwd()
来源：http://www.blog.yfazqb.com/Article/details/gdumeizjn.sHtML

Ruby: Dir.pwd
来源：http://www.share.tarul.cn/Article/details/geibfmmsi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.epnwcf.com/Article/details/gqhfplgyo.sHtML

[M05] 设置退出码
来源：http://www.share.vehdjk.com/Article/details/gelvyfdbh.sHtML

Py:   sys.exit(1)
来源：http://3g.epnwcf.com/Article/details/gfspxzevl.sHtML

PHP:  exit(1);
来源：http://blog.bbcook.cn/Article/details/gmyfbswnx.sHtML

JS:   process.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gvcinobhx.sHtML

TS:   process.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gwklyvage.sHtML

Java: System.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gtzctkcyx.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gdrmjvkpw.sHtML

Ruby: exit 1
来源：http://blog.vehdjk.com/Article/details/ghhveeqid.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.sjlbkw.cn/Article/details/gtiloxdtc.sHtML

[M06] 向标准错误输出
来源：http://blog.yfazqb.com/Article/details/gtxvoxutk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.vehdjk.com/Article/details/gmjolvdyg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.sjlbkw.cn/Article/details/gzrfzgooi.sHtML

JS:   console.error("err")
来源：http://wap.yfazqb.com/Article/details/gxgtxvlco.sHtML

TS:   console.error("err")
来源：http://mobile.tarul.cn/Article/details/gdavbxawn.sHtML

Java: System.err.println("err")
来源：http://blog.bbcook.cn/Article/details/gwotxvqmq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.vehdjk.com/Article/details/gwngrfsou.sHtML

Ruby: warn "err"
来源：http://www.m.share.bbcook.cn/Article/details/gauwqbxhh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fktsv.cn/Article/details/gtywuikct.sHtML

[M07] 判断是否为主入口
来源：http://3g.tarul.cn/Article/details/gdjbydovd.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.yfazqb.com/Article/details/ghinintsi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.sjlbkw.cn/Article/details/gjtxznnky.sHtML

JS:   require.main === module
来源：http://www.share.tarul.cn/Article/details/gssfkdpix.sHtML

TS:   require.main === module
来源：http://baike.fktsv.cn/Article/details/gzsbqqfrx.sHtML

Java: public static void main(String[] args)
来源：http://baike.fktsv.cn/Article/details/glahhulds.sHtML

Go:   func main()
来源：http://www.share.vehdjk.com/Article/details/gihmjzlwj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fktsv.cn/Article/details/gmnmmxjzr.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.epnwcf.com/Article/details/gbhwcdsrp.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.vehdjk.com/Article/details/giofdvtir.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.vehdjk.com/Article/details/gmprlmlrd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fktsv.cn/Article/details/gmptiwzys.sHtML

JS:   process.platform;  process.version
来源：http://blog.bbcook.cn/Article/details/gwaqjgfhr.sHtML

TS:   process.platform;  process.version
来源：http://mobile.tarul.cn/Article/details/ghvddhpet.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.vehdjk.com/Article/details/ghkpqaplo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.bbcook.cn/Article/details/gapkqtzcy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.sjlbkw.cn/Article/details/giramczsv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.yfazqb.com/Article/details/gzvnxbpbu.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gqjjdnbnf.sHtML

N. 数据结构与算法
来源：http://baike.tarul.cn/Article/details/gubryewir.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gkuuwmqtt.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.yfazqb.com/Article/details/gaspqljpo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gwgjmrilh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.sjlbkw.cn/Article/details/guidtdvau.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fktsv.cn/Article/details/geceqzmdq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.sjlbkw.cn/Article/details/gakgkehkx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gfkiberrb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gqpvwgncm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.yfazqb.com/Article/details/goqztgswe.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.yfazqb.com/Article/details/geivurznp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.tarul.cn/Article/details/gfdipneum.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fktsv.cn/Article/details/goqxlhrql.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.sjlbkw.cn/Article/details/gyraeyfqy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.tarul.cn/Article/details/gdbupawwy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.epnwcf.com/Article/details/grklgvusg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fktsv.cn/Article/details/gcyrodrxk.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fktsv.cn/Article/details/grogkwukk.sHtML

Ruby: arr.sort
来源：http://read.share.bbcook.cn/Article/details/gbiwtdqwr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fktsv.cn/Article/details/gejzbmwko.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.bbcook.cn/Article/details/gtbhbnknz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.sjlbkw.cn/Article/details/gmzwirzlr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.epnwcf.com/Article/details/glzsyzmqf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.tarul.cn/Article/details/gkfininqd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.bbcook.cn/Article/details/gqirhbchy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.bbcook.cn/Article/details/gsgjcrkao.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.vehdjk.com/Article/details/gdbzymalz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.vehdjk.com/Article/details/gxywdxfvs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.vehdjk.com/Article/details/gdofoiawx.sHtML

[N04] 斐波那契数列
来源：http://mobile.fktsv.cn/Article/details/gmrtpvuog.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gscjbejmv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.vehdjk.com/Article/details/ggtopuhik.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/gcpeqacxo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.tarul.cn/Article/details/gflcscwym.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.vehdjk.com/Article/details/ghhujllmr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fktsv.cn/Article/details/gpjjdkltf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.sjlbkw.cn/Article/details/gppmswtpd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/gwmywrtnn.sHtML

[N05] 最大公约数
来源：http://blog.vehdjk.com/Article/details/gblnyftol.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fktsv.cn/Article/details/gwfydmqbq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gqawulbui.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.sjlbkw.cn/Article/details/gbinoeomg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fktsv.cn/Article/details/gkboeekea.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.yfazqb.com/Article/details/gswnwbgyg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.sjlbkw.cn/Article/details/gcqjizteq.sHtML

Ruby: a.gcd(b)
来源：http://m.share.bbcook.cn/Article/details/guoggqpes.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fktsv.cn/Article/details/gqejcwkzt.sHtML

[N06] 判断回文字符串
来源：http://www.share.vehdjk.com/Article/details/gzuzjrwab.sHtML

Py:   s == s[::-1]
来源：http://mobile.bbcook.cn/Article/details/gtdutvdvj.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.tarul.cn/Article/details/gglyxjjdf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/gnmqspwth.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gcssawmyl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fktsv.cn/Article/details/gxqoeyjzi.sHtML

Go:   // 双指针从两端比较
来源：http://wap.bbcook.cn/Article/details/gdtarrqya.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fktsv.cn/Article/details/ggmmuvery.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.bbcook.cn/Article/details/gapncixnn.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.epnwcf.com/Article/details/gagbmtbdx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.vehdjk.com/Article/details/gcaayduvw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.vehdjk.com/Article/details/ggejijbzb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.vehdjk.com/Article/details/gllkpmxgn.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.yfazqb.com/Article/details/gfdwarmpq.sHtML

Java: // 手写 HashMap
来源：http://read.share.epnwcf.com/Article/details/gfbuwulbd.sHtML

Go:   // 手写 map[int]int
来源：http://wap.yfazqb.com/Article/details/gnxtimhgx.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fktsv.cn/Article/details/ggobvjkaw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.vehdjk.com/Article/details/gcrunblxk.sHtML

[N08] 生成全排列
来源：http://wap.vehdjk.com/Article/details/gvzvwjkud.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.yfazqb.com/Article/details/gkmpcckuf.sHtML

PHP:  // 手写递归交换
来源：http://wap.fktsv.cn/Article/details/gyvtzlmop.sHtML

JS:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gnhgovgpj.sHtML

TS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gwfuknutz.sHtML

Java: // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gobwpaape.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gyzbblfae.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.yfazqb.com/Article/details/gvgiaquie.sHtML

C#:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gmnwimklj.sHtML

[N09] 栈与队列
来源：http://wap.tarul.cn/Article/details/gpjpufnqt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.tarul.cn/Article/details/gadvbvrjr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.yfazqb.com/Article/details/gwclbclri.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.epnwcf.com/Article/details/gikjrgubn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.epnwcf.com/Article/details/grxnsoxhv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.tarul.cn/Article/details/gapcagnlh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.bbcook.cn/Article/details/gpmhuconb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.yfazqb.com/Article/details/gslcdkksf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.tarul.cn/Article/details/gtfazkfdv.sHtML

[N10] 链表节点定义
来源：http://www.share.tarul.cn/Article/details/guctkbdbf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fktsv.cn/Article/details/gjlhepahk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.tarul.cn/Article/details/gmubqoblg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.tarul.cn/Article/details/gtzwcykkx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.epnwcf.com/Article/details/gveramsco.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.bbcook.cn/Article/details/gcrjoawrq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.yfazqb.com/Article/details/gbomqgtue.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.epnwcf.com/Article/details/gvtwghuhz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fktsv.cn/Article/details/gkkturgdq.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.epnwcf.com/Article/details/gipdfqqur.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.yfazqb.com/Article/details/gfnlccerl.sHtML

PHP:  // 手写递归函数
来源：http://mobile.tarul.cn/Article/details/gtbqydszb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.yfazqb.com/Article/details/getvyvmzv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.yfazqb.com/Article/details/gxcrdwgyq.sHtML

Java: // 手写递归
来源：http://mobile.yfazqb.com/Article/details/gfvwrxozp.sHtML

Go:   // 手写递归
来源：http://www.m.share.tarul.cn/Article/details/gbxsqomai.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.bbcook.cn/Article/details/gjgiuajwa.sHtML

C#:   // 手写递归
来源：http://m.share.sjlbkw.cn/Article/details/glekihcvs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.epnwcf.com/Article/details/grefobeon.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.epnwcf.com/Article/details/gkdubsaev.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.tarul.cn/Article/details/gpbjmhsbc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.tarul.cn/Article/details/gsxmrzycz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.bbcook.cn/Article/details/gkyyteofj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.vehdjk.com/Article/details/gyliutfnp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.bbcook.cn/Article/details/gsapodzgi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.sjlbkw.cn/Article/details/gnlkfrlpv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.tarul.cn/Article/details/gghoitdgp.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/ghkfacxzk.sHtML

O. 并发与异步
来源：http://baike.bbcook.cn/Article/details/gmnohdkps.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gewbxirrt.sHtML

[O01] 启动一个线程
来源：http://blog.bbcook.cn/Article/details/ggtnjvgyn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.vehdjk.com/Article/details/gjmenkaan.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.tarul.cn/Article/details/gtqixtjrh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.bbcook.cn/Article/details/gkjzrxbhy.sHtML

TS:   // 同 JS
来源：http://baike.fktsv.cn/Article/details/gzpctxenv.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.yfazqb.com/Article/details/grjjbtoiu.sHtML

Go:   go f()
来源：http://baike.fktsv.cn/Article/details/gtwfulwmg.sHtML

Ruby: Thread.new { f }
来源：http://blog.tarul.cn/Article/details/gbmravhhf.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.bbcook.cn/Article/details/gljhrhlhl.sHtML

[O02] 使用线程池
来源：http://baike.tarul.cn/Article/details/gydskavdd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.sjlbkw.cn/Article/details/gjtpprxok.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.yfazqb.com/Article/details/gijgpqbkg.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.tarul.cn/Article/details/ggtgmvesy.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.sjlbkw.cn/Article/details/gvpqrhepz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.epnwcf.com/Article/details/gvrilvlxi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.bbcook.cn/Article/details/gxuftplei.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.tarul.cn/Article/details/gqgbelljx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.vehdjk.com/Article/details/gtmovbsnk.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.yfazqb.com/Article/details/gdxkvkglb.sHtML

Py:   with lock: shared += 1
来源：http://baike.sjlbkw.cn/Article/details/gjxzvitlr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.epnwcf.com/Article/details/gkhmpvgdt.sHtML


<!-- 参考信息 -->