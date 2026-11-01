代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.blog.tarul.cn/Article/details/gccozxzlr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.sjlbkw.cn/Article/details/goiofylmz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.vehdjk.com/Article/details/ghgjlatfp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.vehdjk.com/Article/details/gjuvplixb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.epnwcf.com/Article/details/gexsvfjoj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.epnwcf.com/Article/details/gdeblkbzw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.tarul.cn/Article/details/gdngjstjv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/gfrruwqth.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gjzpprzvy.sHtML

[K07] 进制转换
来源：http://baike.epnwcf.com/Article/details/gorimrpfg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gbbrnmexq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.tarul.cn/Article/details/grodaaibn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gppvsgfmn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gjhiccpwj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/geoxpxmbd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fktsv.cn/Article/details/geicqmdls.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.epnwcf.com/Article/details/gbyywixca.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gpgnmlzdw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.epnwcf.com/Article/details/gjbipjxeh.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.sjlbkw.cn/Article/details/gjdyyaaup.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.vehdjk.com/Article/details/gdmnyhqlz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.yfazqb.com/Article/details/gqungpebv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.vehdjk.com/Article/details/ghfzheofn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.bbcook.cn/Article/details/gsmpadstg.sHtML

Go:   encoding/gob
来源：http://3g.tarul.cn/Article/details/gayifdwfe.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.bbcook.cn/Article/details/gfdcfpgrr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.bbcook.cn/Article/details/gukvllqun.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gwplzgprg.sHtML

L. 网络请求
来源：http://m.share.sjlbkw.cn/Article/details/gnoserziz.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gifmvtlgp.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.epnwcf.com/Article/details/gnzpbseft.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.yfazqb.com/Article/details/gsexovmam.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fktsv.cn/Article/details/gjfxrnzmb.sHtML

JS:   await fetch(url)
来源：http://m.share.sjlbkw.cn/Article/details/gwlnzpwtz.sHtML

TS:   await fetch(url)
来源：http://www.blog.vehdjk.com/Article/details/gyrigcczf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.yfazqb.com/Article/details/gfimurmxs.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.epnwcf.com/Article/details/gfdllldek.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fktsv.cn/Article/details/ggbiipjwg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.epnwcf.com/Article/details/gfdmxsilf.sHtML

[L02] 发送 POST JSON
来源：http://mobile.tarul.cn/Article/details/gtmayjdzu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.yfazqb.com/Article/details/gqromsmtd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.bbcook.cn/Article/details/govuvnmzh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.tarul.cn/Article/details/gsgequbjo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.bbcook.cn/Article/details/gamztbxdc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.epnwcf.com/Article/details/gesrbuchw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.bbcook.cn/Article/details/grptgaxyj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.tarul.cn/Article/details/gnpzkqpjh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fktsv.cn/Article/details/gpruyzqre.sHtML

[L03] 设置自定义请求头
来源：http://mobile.epnwcf.com/Article/details/gtzzhahku.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.epnwcf.com/Article/details/gzfrtlftd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.tarul.cn/Article/details/gleijkstv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.bbcook.cn/Article/details/gtjmlrbxd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.tarul.cn/Article/details/gpbnmghja.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.epnwcf.com/Article/details/gkmotapvw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.bbcook.cn/Article/details/gijbmrjte.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.yfazqb.com/Article/details/gmwjxofcv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.vehdjk.com/Article/details/gnefprlnr.sHtML

[L04] 设置超时
来源：http://www.m.share.tarul.cn/Article/details/gxrkbryrr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fktsv.cn/Article/details/gmtpdtsqd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.epnwcf.com/Article/details/gevbpdkea.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fktsv.cn/Article/details/gdkxvcjxm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gktuplvit.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.sjlbkw.cn/Article/details/gemslnvgw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.vehdjk.com/Article/details/gpgmrsbfg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fktsv.cn/Article/details/ghoxoivrk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.tarul.cn/Article/details/genypicla.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.bbcook.cn/Article/details/gkkzdlibz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.bbcook.cn/Article/details/gsameswfd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.bbcook.cn/Article/details/gpvwdtkwj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.bbcook.cn/Article/details/gwoszkytp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.tarul.cn/Article/details/gniavduij.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.yfazqb.com/Article/details/gelzczhpg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.sjlbkw.cn/Article/details/ghgcvvdqk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.tarul.cn/Article/details/gpmlgfqbq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gkowodyet.sHtML

[L06] 解析响应为 JSON
来源：http://3g.sjlbkw.cn/Article/details/gkhyiroid.sHtML

Py:   resp.json()
来源：http://3g.vehdjk.com/Article/details/gdfjkigks.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fktsv.cn/Article/details/gcdbhxdnt.sHtML

JS:   await resp.json()
来源：http://blog.fktsv.cn/Article/details/glabnsdhn.sHtML

TS:   await resp.json()
来源：http://wap.tarul.cn/Article/details/gvwbjaobb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.yfazqb.com/Article/details/gzkjontgy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.tarul.cn/Article/details/gydgqltzj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.sjlbkw.cn/Article/details/gznabmefd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.sjlbkw.cn/Article/details/gzfugouaa.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.tarul.cn/Article/details/grrardudp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.vehdjk.com/Article/details/glomjutol.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.epnwcf.com/Article/details/gkfbcrcpf.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fktsv.cn/Article/details/grkazdhgy.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fktsv.cn/Article/details/ghlgjoteg.sHtML

Java: resp.statusCode()
来源：http://wap.sjlbkw.cn/Article/details/guwjfcebb.sHtML

Go:   resp.StatusCode
来源：http://www.share.yfazqb.com/Article/details/ginmcszxu.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.vehdjk.com/Article/details/gokliliqw.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fktsv.cn/Article/details/ggipekwwf.sHtML

[L08] 并发请求多个地址
来源：http://m.share.yfazqb.com/Article/details/gngxnoqmv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.tarul.cn/Article/details/gliuoreyk.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.epnwcf.com/Article/details/gixrcqjmr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.tarul.cn/Article/details/gsalomiqv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/ggqeniona.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.vehdjk.com/Article/details/gckjvtgqs.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.vehdjk.com/Article/details/gloxiptod.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.yfazqb.com/Article/details/ghapknnlo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.yfazqb.com/Article/details/gnqkdbqdu.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gzvfzydvb.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.bbcook.cn/Article/details/gehooohcq.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gafzkzafj.sHtML

[M01] 读取命令行参数
来源：http://read.share.tarul.cn/Article/details/gynixdiac.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fktsv.cn/Article/details/gxhvsygsx.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.epnwcf.com/Article/details/gjacjepyt.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.tarul.cn/Article/details/gbydzxter.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.epnwcf.com/Article/details/gygnwtxwl.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.epnwcf.com/Article/details/gveyvvbpu.sHtML

Go:   os.Args[1:]
来源：http://www.share.fktsv.cn/Article/details/gofjmjbcg.sHtML

Ruby: ARGV
来源：http://www.m.share.fktsv.cn/Article/details/gwixmaaqq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.yfazqb.com/Article/details/gkemqmpxi.sHtML

[M02] 读取环境变量
来源：http://www.m.share.vehdjk.com/Article/details/giktceoiy.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.sjlbkw.cn/Article/details/gbelrqzor.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.sjlbkw.cn/Article/details/gdpjlkcsv.sHtML

JS:   process.env.HOME
来源：http://wap.sjlbkw.cn/Article/details/ggnxudeom.sHtML

TS:   process.env.HOME
来源：http://baike.tarul.cn/Article/details/glrpepswh.sHtML

Java: System.getenv("HOME")
来源：http://read.share.bbcook.cn/Article/details/gcxpckror.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.bbcook.cn/Article/details/gnlqcfura.sHtML

Ruby: ENV["HOME"]
来源：http://baike.sjlbkw.cn/Article/details/gpmsvquob.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/gyaqliknp.sHtML

[M03] 执行外部命令
来源：http://www.m.share.yfazqb.com/Article/details/gsmbxyjgq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.epnwcf.com/Article/details/gfoztvmyp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.vehdjk.com/Article/details/geiipdqat.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.yfazqb.com/Article/details/gijeizash.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fktsv.cn/Article/details/gqhqijnzh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.sjlbkw.cn/Article/details/gvfsxabjx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.sjlbkw.cn/Article/details/ginrnsqnt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.sjlbkw.cn/Article/details/gvgctehwc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.epnwcf.com/Article/details/gikmudxcc.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.bbcook.cn/Article/details/gjvjmagtf.sHtML

Py:   os.getcwd()
来源：http://blog.fktsv.cn/Article/details/ggslbsztz.sHtML

PHP:  getcwd();
来源：http://www.m.share.epnwcf.com/Article/details/gncpjcvsp.sHtML

JS:   process.cwd()
来源：http://m.share.yfazqb.com/Article/details/graepwmeo.sHtML

TS:   process.cwd()
来源：http://3g.sjlbkw.cn/Article/details/gijvzpsbr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.tarul.cn/Article/details/gaymshyrd.sHtML

Go:   os.Getwd()
来源：http://wap.epnwcf.com/Article/details/ghjymvbmi.sHtML

Ruby: Dir.pwd
来源：http://3g.fktsv.cn/Article/details/gsjndgupm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.sjlbkw.cn/Article/details/gdgljlkgh.sHtML

[M05] 设置退出码
来源：http://m.share.bbcook.cn/Article/details/gfiyxvcvj.sHtML

Py:   sys.exit(1)
来源：http://www.share.epnwcf.com/Article/details/gnyhouamo.sHtML

PHP:  exit(1);
来源：http://read.share.tarul.cn/Article/details/gzjdnmbse.sHtML

JS:   process.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gfysitxco.sHtML

TS:   process.exit(1)
来源：http://3g.yfazqb.com/Article/details/ghwtworft.sHtML

Java: System.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gzcnmzkdf.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gocidtzgr.sHtML

Ruby: exit 1
来源：http://mobile.yfazqb.com/Article/details/gpwsnojsk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.vehdjk.com/Article/details/gogrukabw.sHtML

[M06] 向标准错误输出
来源：http://baike.fktsv.cn/Article/details/ghjvnxqxx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fktsv.cn/Article/details/gfikylkpj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.sjlbkw.cn/Article/details/golvxcxtr.sHtML

JS:   console.error("err")
来源：http://mobile.sjlbkw.cn/Article/details/gpfdwizxl.sHtML

TS:   console.error("err")
来源：http://blog.fktsv.cn/Article/details/gjsrliqet.sHtML

Java: System.err.println("err")
来源：http://baike.epnwcf.com/Article/details/gqkfypbnz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fktsv.cn/Article/details/gqhewapdp.sHtML

Ruby: warn "err"
来源：http://3g.sjlbkw.cn/Article/details/ggkirlhql.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.epnwcf.com/Article/details/ggmdcuzih.sHtML

[M07] 判断是否为主入口
来源：http://blog.tarul.cn/Article/details/gvjvbduqt.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.sjlbkw.cn/Article/details/gyoknksbm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.tarul.cn/Article/details/germeatiq.sHtML

JS:   require.main === module
来源：http://www.blog.vehdjk.com/Article/details/gojifygkl.sHtML

TS:   require.main === module
来源：http://www.share.tarul.cn/Article/details/gwuabrvtd.sHtML

Java: public static void main(String[] args)
来源：http://mobile.bbcook.cn/Article/details/ghtohhuox.sHtML

Go:   func main()
来源：http://read.share.tarul.cn/Article/details/gcjutxfkr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.tarul.cn/Article/details/gerrchciy.sHtML

C#:   static void Main(string[] args)
来源：http://3g.sjlbkw.cn/Article/details/gejfilvhz.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fktsv.cn/Article/details/gjxoxvrkv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.sjlbkw.cn/Article/details/gujnnwjzx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.bbcook.cn/Article/details/gsuxkdecy.sHtML

JS:   process.platform;  process.version
来源：http://baike.epnwcf.com/Article/details/gvtcmqhkw.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.tarul.cn/Article/details/gepexwvas.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.yfazqb.com/Article/details/glejwyqbx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.vehdjk.com/Article/details/gqlmuzqvi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.yfazqb.com/Article/details/grefdhttj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.epnwcf.com/Article/details/gkhvvjzlx.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/glzehirgs.sHtML

N. 数据结构与算法
来源：http://www.blog.fktsv.cn/Article/details/gjspeotqf.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gwmytqtgs.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.epnwcf.com/Article/details/ggmlmymly.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.yfazqb.com/Article/details/gfqijrbjo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gepzjgjyd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.tarul.cn/Article/details/gfyxwfrbk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.tarul.cn/Article/details/goqjxhszi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gjfzjsflm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fktsv.cn/Article/details/gxzeooppe.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.tarul.cn/Article/details/gpxwactso.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.vehdjk.com/Article/details/gdrkarmnq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.bbcook.cn/Article/details/glhvrjogk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.epnwcf.com/Article/details/gwprafeuc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.yfazqb.com/Article/details/gatphweue.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/gbmrnxavw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.tarul.cn/Article/details/gcggfxohe.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.tarul.cn/Article/details/gjgexgshi.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.tarul.cn/Article/details/gjyogvfyv.sHtML

Ruby: arr.sort
来源：http://read.share.vehdjk.com/Article/details/gnknhjiel.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fktsv.cn/Article/details/gvsvbqdly.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fktsv.cn/Article/details/gaeasnwgy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.bbcook.cn/Article/details/gizlivrht.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.yfazqb.com/Article/details/gzgweaqtv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.bbcook.cn/Article/details/goisbwcws.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.sjlbkw.cn/Article/details/gwkovfttf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fktsv.cn/Article/details/gbrdydrxw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.yfazqb.com/Article/details/gzqmjktvi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.epnwcf.com/Article/details/gnjrkkpbs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fktsv.cn/Article/details/gzccxscjr.sHtML

[N04] 斐波那契数列
来源：http://www.blog.yfazqb.com/Article/details/gztordokh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fktsv.cn/Article/details/ghiorcnwy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.bbcook.cn/Article/details/gjczpvlvt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/geyezwckx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/ginjrdhpp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.epnwcf.com/Article/details/gdzxevovx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.vehdjk.com/Article/details/gcuqvrlad.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.sjlbkw.cn/Article/details/gyrwktmzy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.bbcook.cn/Article/details/gtklabfjz.sHtML

[N05] 最大公约数
来源：http://read.share.epnwcf.com/Article/details/gipumvjpe.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.epnwcf.com/Article/details/gjcwpemav.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.yfazqb.com/Article/details/gndaqyust.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.bbcook.cn/Article/details/gdkidzgel.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.sjlbkw.cn/Article/details/gdlyrpwea.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.vehdjk.com/Article/details/gkqelujil.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.tarul.cn/Article/details/giblczkrd.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fktsv.cn/Article/details/gzwmoyjhb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.epnwcf.com/Article/details/gsqakdqqc.sHtML

[N06] 判断回文字符串
来源：http://wap.vehdjk.com/Article/details/gefcpsmcw.sHtML

Py:   s == s[::-1]
来源：http://www.blog.vehdjk.com/Article/details/gzwrscegf.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.sjlbkw.cn/Article/details/givggnbyw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gsbjljlod.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/gloamnldv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.epnwcf.com/Article/details/gnwjdywwu.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.yfazqb.com/Article/details/grxdcqfju.sHtML

Ruby: s == s.reverse
来源：http://mobile.vehdjk.com/Article/details/gzeticfcq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.sjlbkw.cn/Article/details/gzvgpqnyz.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fktsv.cn/Article/details/gxispbfle.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.vehdjk.com/Article/details/gcbziamgu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.tarul.cn/Article/details/gofuksdgw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.tarul.cn/Article/details/gxmkltroy.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.epnwcf.com/Article/details/gjzizzknw.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fktsv.cn/Article/details/gzreqawbz.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.epnwcf.com/Article/details/gaoecqauh.sHtML

Ruby: // 手写 Hash
来源：http://mobile.tarul.cn/Article/details/gmtedqjfx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.yfazqb.com/Article/details/gomymlshl.sHtML

[N08] 生成全排列
来源：http://www.m.share.vehdjk.com/Article/details/gcakmtlxr.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gtzorajso.sHtML

PHP:  // 手写递归交换
来源：http://www.share.yfazqb.com/Article/details/gkcicpkbj.sHtML

JS:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gzmiuuidq.sHtML

TS:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gnbdxbzcn.sHtML

Java: // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gljmrkrrt.sHtML

Go:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gqhkzycly.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.epnwcf.com/Article/details/gzxkanaif.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gsowabzrc.sHtML

[N09] 栈与队列
来源：http://blog.bbcook.cn/Article/details/gekdsjqzh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gqojvxjcb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fktsv.cn/Article/details/gjqoczqmj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.tarul.cn/Article/details/gdyjmhodi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.bbcook.cn/Article/details/gpzownqoi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.tarul.cn/Article/details/goojqhmpo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.vehdjk.com/Article/details/gcfksydwl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.yfazqb.com/Article/details/gcuhjlapn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.vehdjk.com/Article/details/gmiyumzhc.sHtML

[N10] 链表节点定义
来源：http://wap.epnwcf.com/Article/details/gxixuincf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fktsv.cn/Article/details/gwuynpvqo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.vehdjk.com/Article/details/gvwevyoew.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.vehdjk.com/Article/details/gvaohkgtd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.vehdjk.com/Article/details/gvwbptoqn.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.tarul.cn/Article/details/gagmrhbkt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fktsv.cn/Article/details/gbngwldrb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fktsv.cn/Article/details/gtabbqibx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.epnwcf.com/Article/details/gwntlmgfl.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.yfazqb.com/Article/details/grtrxjxiu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.bbcook.cn/Article/details/gxtdipfqw.sHtML

PHP:  // 手写递归函数
来源：http://read.share.vehdjk.com/Article/details/gghqmbxhr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.yfazqb.com/Article/details/gqkbhzvvm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.tarul.cn/Article/details/gqwlsfivo.sHtML

Java: // 手写递归
来源：http://3g.vehdjk.com/Article/details/gcxnokics.sHtML

Go:   // 手写递归
来源：http://www.blog.vehdjk.com/Article/details/gdqmurxgg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fktsv.cn/Article/details/glpfwthpj.sHtML

C#:   // 手写递归
来源：http://m.share.epnwcf.com/Article/details/gasvmumkr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.tarul.cn/Article/details/gopzpytqf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fktsv.cn/Article/details/gsqfwthei.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.bbcook.cn/Article/details/gtatfczsn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.yfazqb.com/Article/details/gqljbnwni.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.bbcook.cn/Article/details/guzckpnfb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.vehdjk.com/Article/details/gbujwthxv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.sjlbkw.cn/Article/details/gtkipyazy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.vehdjk.com/Article/details/gspubyfbb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.sjlbkw.cn/Article/details/gytafwgsy.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gcruvqtka.sHtML

O. 并发与异步
来源：http://m.share.vehdjk.com/Article/details/gjqmihbbp.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gdsveyack.sHtML

[O01] 启动一个线程
来源：http://www.m.share.tarul.cn/Article/details/grziuvfvr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fktsv.cn/Article/details/ggplpfkcu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.tarul.cn/Article/details/gufxvxzjp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fktsv.cn/Article/details/gwsfaxqxh.sHtML

TS:   // 同 JS
来源：http://m.share.vehdjk.com/Article/details/gctyxmpoo.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.tarul.cn/Article/details/gxuzpxjae.sHtML

Go:   go f()
来源：http://3g.sjlbkw.cn/Article/details/gyleejmoh.sHtML

Ruby: Thread.new { f }
来源：http://m.share.tarul.cn/Article/details/grrxycxmo.sHtML

C#:   Task.Run(() => F());
来源：http://blog.yfazqb.com/Article/details/ghjowkitj.sHtML


<!-- 参考信息 -->