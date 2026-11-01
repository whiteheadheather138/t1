代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.bbcook.cn/Article/details/gchjnfllp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.epnwcf.com/Article/details/grmbrkgzj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.epnwcf.com/Article/details/gzjyskwew.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.sjlbkw.cn/Article/details/gqftlvoox.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwiolimk.sHtML

[K07] 进制转换
来源：http://www.share.epnwcf.com/Article/details/gryqmjziy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gyzpbpvki.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.epnwcf.com/Article/details/gwdusurzp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gochpidhx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/godlbwwag.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gltwyknjk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.epnwcf.com/Article/details/gesgbvofg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fktsv.cn/Article/details/grzzjfpqb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.yfazqb.com/Article/details/giudfizvp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.tarul.cn/Article/details/gyokxzsbr.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.epnwcf.com/Article/details/geapzznxn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.bbcook.cn/Article/details/gacamfkmw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.sjlbkw.cn/Article/details/glsvieraa.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fktsv.cn/Article/details/grdqgksgs.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.tarul.cn/Article/details/gqfwrhnii.sHtML

Go:   encoding/gob
来源：http://www.share.vehdjk.com/Article/details/gbvzxrzmq.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.vehdjk.com/Article/details/glbppbgos.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.tarul.cn/Article/details/gzinfsolz.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gxbvehlay.sHtML

L. 网络请求
来源：http://www.blog.yfazqb.com/Article/details/gfvyrbhss.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gsqcqqslx.sHtML

[L01] 发送 GET 请求
来源：http://read.share.yfazqb.com/Article/details/gotvnhmrn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.vehdjk.com/Article/details/glsehqpoe.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.sjlbkw.cn/Article/details/gzizyorps.sHtML

JS:   await fetch(url)
来源：http://m.share.yfazqb.com/Article/details/ganrqomgp.sHtML

TS:   await fetch(url)
来源：http://m.share.sjlbkw.cn/Article/details/gebprxuxt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.tarul.cn/Article/details/gkvppneuu.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.yfazqb.com/Article/details/gdtbeajbt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.tarul.cn/Article/details/grjbyjpca.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.vehdjk.com/Article/details/gdavxfzcc.sHtML

[L02] 发送 POST JSON
来源：http://3g.yfazqb.com/Article/details/gvksthpis.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.tarul.cn/Article/details/ghiycfeio.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.sjlbkw.cn/Article/details/gybbupdho.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.epnwcf.com/Article/details/gcquzvvuf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.vehdjk.com/Article/details/gyehprlih.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.yfazqb.com/Article/details/gvwnltadb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.sjlbkw.cn/Article/details/gjniqrgsz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.tarul.cn/Article/details/gwdppqhjn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.bbcook.cn/Article/details/gmjonouls.sHtML

[L03] 设置自定义请求头
来源：http://blog.bbcook.cn/Article/details/gnclwyatq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.tarul.cn/Article/details/gvmnxdryf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.bbcook.cn/Article/details/gdaoiycrq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.bbcook.cn/Article/details/gszniikph.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/gvfwsmamr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.bbcook.cn/Article/details/gbhjthlke.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.epnwcf.com/Article/details/gzckqskaz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.sjlbkw.cn/Article/details/glycannmh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.vehdjk.com/Article/details/ghogfxptl.sHtML

[L04] 设置超时
来源：http://wap.sjlbkw.cn/Article/details/grwzknxkp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.bbcook.cn/Article/details/gvuesnkqh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.tarul.cn/Article/details/ggwpcyhck.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.vehdjk.com/Article/details/gkyeehvcm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.bbcook.cn/Article/details/ghjymwjaw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.tarul.cn/Article/details/gkfimwegp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.epnwcf.com/Article/details/gnjljqdsy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.vehdjk.com/Article/details/gjixlepao.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.bbcook.cn/Article/details/gtvqimdnk.sHtML

[L05] 上传文件（multipart）
来源：http://blog.bbcook.cn/Article/details/gqnqssncj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.sjlbkw.cn/Article/details/ggkgulqlz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.epnwcf.com/Article/details/gaydtsvtx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.vehdjk.com/Article/details/gqtnednko.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.vehdjk.com/Article/details/gaabfcckv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.epnwcf.com/Article/details/gupeipbfk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.vehdjk.com/Article/details/gmhqnlhyi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.tarul.cn/Article/details/gtznsopgl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.yfazqb.com/Article/details/gsjehwpuv.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqrifdos.sHtML

Py:   resp.json()
来源：http://blog.yfazqb.com/Article/details/gjjjrdcul.sHtML

PHP:  json_decode($body, true);
来源：http://blog.sjlbkw.cn/Article/details/gskckwbhx.sHtML

JS:   await resp.json()
来源：http://blog.sjlbkw.cn/Article/details/gatlsbxoh.sHtML

TS:   await resp.json()
来源：http://blog.sjlbkw.cn/Article/details/gseskfxrz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fktsv.cn/Article/details/gouqiewcy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.tarul.cn/Article/details/gphshbonu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.epnwcf.com/Article/details/gsfhqocil.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fktsv.cn/Article/details/goeuijuqi.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.bbcook.cn/Article/details/gjycbauiw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.vehdjk.com/Article/details/gjfejaxfw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.sjlbkw.cn/Article/details/gxeqkqdue.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.yfazqb.com/Article/details/gsbawcisv.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.bbcook.cn/Article/details/gyrjcwtgf.sHtML

Java: resp.statusCode()
来源：http://m.share.sjlbkw.cn/Article/details/guyhvgqoi.sHtML

Go:   resp.StatusCode
来源：http://read.share.sjlbkw.cn/Article/details/ghbjjowoa.sHtML

Ruby: resp.code.to_i
来源：http://m.share.vehdjk.com/Article/details/gkclxyicn.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.yfazqb.com/Article/details/gpevwlvtf.sHtML

[L08] 并发请求多个地址
来源：http://3g.fktsv.cn/Article/details/giqlmnxoj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.tarul.cn/Article/details/gkxxeuxdv.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fktsv.cn/Article/details/gqmpzhzjm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fktsv.cn/Article/details/gxmahggfq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/gzytxkjik.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.tarul.cn/Article/details/gguejoqxm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.bbcook.cn/Article/details/gsnyfsahw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.epnwcf.com/Article/details/grrmrmnzu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.vehdjk.com/Article/details/gjhmflqlo.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gzaxgftyb.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.epnwcf.com/Article/details/gafmpnxde.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gmerkyjvr.sHtML

[M01] 读取命令行参数
来源：http://baike.epnwcf.com/Article/details/ghhzmteif.sHtML

Py:   sys.argv[1:]
来源：http://3g.bbcook.cn/Article/details/gvyutmwrr.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.vehdjk.com/Article/details/gbwxheeyo.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.tarul.cn/Article/details/gztwrxgsq.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fktsv.cn/Article/details/gpmuyttzu.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fktsv.cn/Article/details/ghldqwvpc.sHtML

Go:   os.Args[1:]
来源：http://3g.sjlbkw.cn/Article/details/ghlpqwrkx.sHtML

Ruby: ARGV
来源：http://baike.vehdjk.com/Article/details/gwiettlat.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.bbcook.cn/Article/details/gqnuezzda.sHtML

[M02] 读取环境变量
来源：http://www.blog.yfazqb.com/Article/details/gookufnel.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.bbcook.cn/Article/details/grmzhqhzs.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.bbcook.cn/Article/details/glehquygu.sHtML

JS:   process.env.HOME
来源：http://m.share.bbcook.cn/Article/details/gzhwgiapi.sHtML

TS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/gaxzynkyl.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fktsv.cn/Article/details/giravfxqj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.yfazqb.com/Article/details/gfvyemfrr.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.bbcook.cn/Article/details/gaatvzfoh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.tarul.cn/Article/details/gmxwaewgy.sHtML

[M03] 执行外部命令
来源：http://www.share.yfazqb.com/Article/details/gnsffsnqq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.vehdjk.com/Article/details/gxdhwyyqw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fktsv.cn/Article/details/gajqsoowe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.vehdjk.com/Article/details/gudggzquy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.sjlbkw.cn/Article/details/gtevqwtih.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.vehdjk.com/Article/details/gilhfgnaz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fktsv.cn/Article/details/gnfqonnem.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fktsv.cn/Article/details/gkkwimzad.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.sjlbkw.cn/Article/details/gmrhpfayh.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.epnwcf.com/Article/details/gzqfydopi.sHtML

Py:   os.getcwd()
来源：http://www.share.yfazqb.com/Article/details/ggbzprfaa.sHtML

PHP:  getcwd();
来源：http://www.share.vehdjk.com/Article/details/gqacmyspe.sHtML

JS:   process.cwd()
来源：http://www.m.share.vehdjk.com/Article/details/gyvjvdekv.sHtML

TS:   process.cwd()
来源：http://wap.bbcook.cn/Article/details/gtszhtjfi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.sjlbkw.cn/Article/details/gspyskikh.sHtML

Go:   os.Getwd()
来源：http://baike.bbcook.cn/Article/details/gfyegzwth.sHtML

Ruby: Dir.pwd
来源：http://wap.epnwcf.com/Article/details/gbixsghzw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.sjlbkw.cn/Article/details/gxsefvhyg.sHtML

[M05] 设置退出码
来源：http://www.share.sjlbkw.cn/Article/details/gdtwzpkns.sHtML

Py:   sys.exit(1)
来源：http://wap.fktsv.cn/Article/details/ghehdjdti.sHtML

PHP:  exit(1);
来源：http://wap.yfazqb.com/Article/details/gzlslkgtu.sHtML

JS:   process.exit(1)
来源：http://blog.epnwcf.com/Article/details/gmrhmpfdc.sHtML

TS:   process.exit(1)
来源：http://blog.bbcook.cn/Article/details/gdnwgagfn.sHtML

Java: System.exit(1)
来源：http://blog.fktsv.cn/Article/details/gywrocmnz.sHtML

Go:   os.Exit(1)
来源：http://3g.fktsv.cn/Article/details/glfxmpduh.sHtML

Ruby: exit 1
来源：http://read.share.epnwcf.com/Article/details/gmlpofwge.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.bbcook.cn/Article/details/gxukxkksh.sHtML

[M06] 向标准错误输出
来源：http://3g.tarul.cn/Article/details/grjnohsyj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.sjlbkw.cn/Article/details/gblpidhdi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.sjlbkw.cn/Article/details/gdagwjdpf.sHtML

JS:   console.error("err")
来源：http://www.m.share.tarul.cn/Article/details/gtswsmkpg.sHtML

TS:   console.error("err")
来源：http://wap.sjlbkw.cn/Article/details/gownfulcb.sHtML

Java: System.err.println("err")
来源：http://3g.sjlbkw.cn/Article/details/goikwovjs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fktsv.cn/Article/details/gkmzlxrbs.sHtML

Ruby: warn "err"
来源：http://read.share.sjlbkw.cn/Article/details/gyowgrnzz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.yfazqb.com/Article/details/giywmxoyr.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.epnwcf.com/Article/details/gyowmdlsk.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.sjlbkw.cn/Article/details/ghatxgogt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.epnwcf.com/Article/details/gevslkyna.sHtML

JS:   require.main === module
来源：http://m.share.bbcook.cn/Article/details/gzozlguqt.sHtML

TS:   require.main === module
来源：http://3g.bbcook.cn/Article/details/gfdczkvnt.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.vehdjk.com/Article/details/geffwfikq.sHtML

Go:   func main()
来源：http://read.share.yfazqb.com/Article/details/guivjqhfd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.tarul.cn/Article/details/ghqdjoxbb.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.yfazqb.com/Article/details/gerumylaf.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.yfazqb.com/Article/details/gaiacjjkx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.sjlbkw.cn/Article/details/gptmrvyla.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.vehdjk.com/Article/details/gecemkedz.sHtML

JS:   process.platform;  process.version
来源：http://read.share.epnwcf.com/Article/details/gploilfoa.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.vehdjk.com/Article/details/glubaibbz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fktsv.cn/Article/details/ggajyevsu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.bbcook.cn/Article/details/gsnhtecbo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.vehdjk.com/Article/details/gtfctacrg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.sjlbkw.cn/Article/details/gtzmyqveu.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ghxfvutpa.sHtML

N. 数据结构与算法
来源：http://www.blog.bbcook.cn/Article/details/gjbxunkfp.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gwdujjpcu.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.epnwcf.com/Article/details/gqhyxbjpv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gcooaxnpi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.epnwcf.com/Article/details/glnsamsbo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.bbcook.cn/Article/details/gnhevuqgz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.yfazqb.com/Article/details/gpdyperok.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gqelywior.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gjheeufog.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fktsv.cn/Article/details/gsldbldby.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gnuizptmx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.tarul.cn/Article/details/gopjukdle.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.vehdjk.com/Article/details/gjclrbupb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.vehdjk.com/Article/details/gnsjfxyuw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.yfazqb.com/Article/details/gsyrtipyp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.sjlbkw.cn/Article/details/giovilfrs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fktsv.cn/Article/details/gsqczrpyz.sHtML

Go:   slices.Sort(arr)
来源：http://blog.sjlbkw.cn/Article/details/gtounoznf.sHtML

Ruby: arr.sort
来源：http://m.share.fktsv.cn/Article/details/gywqlnnrf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.vehdjk.com/Article/details/gpfjnorsj.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.bbcook.cn/Article/details/gikyqmjpi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.yfazqb.com/Article/details/gotexarnt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.bbcook.cn/Article/details/giedcamik.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.epnwcf.com/Article/details/gkfmcccct.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.bbcook.cn/Article/details/gwycrlxbn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fktsv.cn/Article/details/gkibgkijo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.tarul.cn/Article/details/gsegprcfu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.yfazqb.com/Article/details/gsfzgbeuv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.bbcook.cn/Article/details/gnerjwrcp.sHtML

[N04] 斐波那契数列
来源：http://mobile.sjlbkw.cn/Article/details/gawpjtbln.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.tarul.cn/Article/details/gljzutwqb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.sjlbkw.cn/Article/details/gwlnhdlax.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.vehdjk.com/Article/details/gfkgyjonn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/gyabwvzew.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.epnwcf.com/Article/details/gmfdajtad.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fktsv.cn/Article/details/gqwyrhime.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.epnwcf.com/Article/details/gzscluvhb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.epnwcf.com/Article/details/gbeeootbl.sHtML

[N05] 最大公约数
来源：http://www.blog.yfazqb.com/Article/details/gxqvalbmu.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fktsv.cn/Article/details/gvcaahvuj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.epnwcf.com/Article/details/ghjtttjrt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fktsv.cn/Article/details/gxwmxfqre.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.tarul.cn/Article/details/gncghthvp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.vehdjk.com/Article/details/ghjgagapj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.bbcook.cn/Article/details/gaasaoxdr.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fktsv.cn/Article/details/gpnatnlmb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fktsv.cn/Article/details/gdltlioix.sHtML

[N06] 判断回文字符串
来源：http://www.share.yfazqb.com/Article/details/gzzqyncga.sHtML

Py:   s == s[::-1]
来源：http://mobile.bbcook.cn/Article/details/guageblcn.sHtML

PHP:  $s === strrev($s);
来源：http://baike.tarul.cn/Article/details/gfteeazdr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gurbwnmhv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gtfypvyvn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.vehdjk.com/Article/details/gxxrvosxr.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.sjlbkw.cn/Article/details/gayolwrvt.sHtML

Ruby: s == s.reverse
来源：http://mobile.tarul.cn/Article/details/goqfspgly.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.vehdjk.com/Article/details/gsmrwlbky.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.tarul.cn/Article/details/grmjukbxe.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fktsv.cn/Article/details/gvnmpuasa.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.vehdjk.com/Article/details/gpsdjdyiz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.tarul.cn/Article/details/grqmvlwym.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fktsv.cn/Article/details/gkkzpizfl.sHtML

Java: // 手写 HashMap
来源：http://baike.fktsv.cn/Article/details/gicvxryfy.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.vehdjk.com/Article/details/gygnwvkyu.sHtML

Ruby: // 手写 Hash
来源：http://mobile.yfazqb.com/Article/details/gcofbqbel.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.tarul.cn/Article/details/gngffodmk.sHtML

[N08] 生成全排列
来源：http://www.m.share.epnwcf.com/Article/details/grxvrejhb.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.bbcook.cn/Article/details/gmjmkuncm.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.epnwcf.com/Article/details/gzzpdbsfg.sHtML

JS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gctsglwkn.sHtML

TS:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/gzryaunss.sHtML

Java: // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gjkybhurq.sHtML

Go:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gmccfrpfk.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fktsv.cn/Article/details/gliutwobo.sHtML

C#:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gvtctfnlm.sHtML

[N09] 栈与队列
来源：http://read.share.fktsv.cn/Article/details/gdbjoxpke.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gmkkcuirc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gkbsscuqp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.bbcook.cn/Article/details/gnmwxyxue.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.tarul.cn/Article/details/gfpxmopfr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fktsv.cn/Article/details/gpdqklock.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.vehdjk.com/Article/details/gtmxicgup.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.sjlbkw.cn/Article/details/gosnbaqar.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.epnwcf.com/Article/details/gkmtkbvnn.sHtML

[N10] 链表节点定义
来源：http://read.share.vehdjk.com/Article/details/gzktznziv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.epnwcf.com/Article/details/gblffjkxl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.epnwcf.com/Article/details/gkbuizjal.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.yfazqb.com/Article/details/gqseiwoho.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.epnwcf.com/Article/details/gqxrfmayg.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.tarul.cn/Article/details/gzxhgxafk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.sjlbkw.cn/Article/details/gzbkgtjlk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.tarul.cn/Article/details/gxzddwjqz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.yfazqb.com/Article/details/gcagfwwok.sHtML

[N11] 二叉树中序遍历
来源：http://blog.bbcook.cn/Article/details/gnaedyuaw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.yfazqb.com/Article/details/grmfaxvob.sHtML

PHP:  // 手写递归函数
来源：http://wap.bbcook.cn/Article/details/gobxifpec.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fktsv.cn/Article/details/gmrptednv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fktsv.cn/Article/details/glvnceoxu.sHtML

Java: // 手写递归
来源：http://mobile.fktsv.cn/Article/details/glprpuxll.sHtML

Go:   // 手写递归
来源：http://3g.sjlbkw.cn/Article/details/gfqtzaave.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.bbcook.cn/Article/details/gfazuhhth.sHtML

C#:   // 手写递归
来源：http://mobile.epnwcf.com/Article/details/gbjerucuc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.bbcook.cn/Article/details/gsfvnuntx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.tarul.cn/Article/details/gejorvszu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.yfazqb.com/Article/details/gulxvwhrf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.tarul.cn/Article/details/gtbmthjul.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.epnwcf.com/Article/details/gmzfafzht.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.vehdjk.com/Article/details/gyjhdvufv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.epnwcf.com/Article/details/guafdyttw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.vehdjk.com/Article/details/ginviamxb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.bbcook.cn/Article/details/gbcdevagq.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gmlqelknx.sHtML

O. 并发与异步
来源：http://3g.bbcook.cn/Article/details/gzfspnpwq.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gwbwzsrmw.sHtML

[O01] 启动一个线程
来源：http://www.m.share.tarul.cn/Article/details/gyylfdoai.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.yfazqb.com/Article/details/glckuuohc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gbnvdlfft.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.epnwcf.com/Article/details/gfipmkgiv.sHtML

TS:   // 同 JS
来源：http://www.share.fktsv.cn/Article/details/gtobeaaae.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.bbcook.cn/Article/details/gctynihbp.sHtML

Go:   go f()
来源：http://wap.sjlbkw.cn/Article/details/gamkoalwa.sHtML

Ruby: Thread.new { f }
来源：http://wap.sjlbkw.cn/Article/details/gviakalrm.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.bbcook.cn/Article/details/gdedxsyef.sHtML

[O02] 使用线程池
来源：http://www.share.vehdjk.com/Article/details/gtsffniso.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.sjlbkw.cn/Article/details/gbdlzqtck.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.tarul.cn/Article/details/gankjwsxd.sHtML

JS:   // worker_threads 线程池
来源：http://3g.bbcook.cn/Article/details/gryyzylxj.sHtML


<!-- 参考信息 -->