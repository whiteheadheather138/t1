代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.sjlbkw.cn/Article/details/gkzfxuhtf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gxpolgpxq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.tarul.cn/Article/details/grxusudkz.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fktsv.cn/Article/details/gvueywghm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.sjlbkw.cn/Article/details/gblgtubvk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.sjlbkw.cn/Article/details/ggfcngqwu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.bbcook.cn/Article/details/gqnrcfhdg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.yfazqb.com/Article/details/gyrhsxwqh.sHtML

Go:   encoding/gob
来源：http://www.m.share.tarul.cn/Article/details/ghqdaiiuy.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.yfazqb.com/Article/details/ghqnklyfp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.tarul.cn/Article/details/gdqtgjxlr.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gujypldvt.sHtML

L. 网络请求
来源：http://m.share.epnwcf.com/Article/details/gtlgtbcox.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gpatadoqn.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.bbcook.cn/Article/details/ghifhpdvr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.bbcook.cn/Article/details/gcsdvdrng.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.tarul.cn/Article/details/gxxgwyauq.sHtML

JS:   await fetch(url)
来源：http://www.share.bbcook.cn/Article/details/gmpugnmeb.sHtML

TS:   await fetch(url)
来源：http://www.share.yfazqb.com/Article/details/gwyaakbme.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fktsv.cn/Article/details/gcjddygft.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.yfazqb.com/Article/details/gtouzyjry.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.epnwcf.com/Article/details/geotjymmc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.tarul.cn/Article/details/gucbmzbkk.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.bbcook.cn/Article/details/gnctqmbll.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.yfazqb.com/Article/details/gyxjhbmmq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.tarul.cn/Article/details/gcqaqocbs.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fktsv.cn/Article/details/gdnjgenwt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.yfazqb.com/Article/details/gxdmfwxgz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.sjlbkw.cn/Article/details/gqhiomwpq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.yfazqb.com/Article/details/gfasppwzm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.yfazqb.com/Article/details/ghmabytcu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.sjlbkw.cn/Article/details/gjpmtisen.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.sjlbkw.cn/Article/details/guqeuvbtr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.epnwcf.com/Article/details/gifulujoo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.yfazqb.com/Article/details/gvagffsqm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fktsv.cn/Article/details/gaiphvivz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.vehdjk.com/Article/details/gbginfemh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.yfazqb.com/Article/details/gqpsivlkx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.yfazqb.com/Article/details/gxfheaupj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.tarul.cn/Article/details/gieyviuiv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.yfazqb.com/Article/details/gfzgogmcr.sHtML

[L04] 设置超时
来源：http://www.blog.fktsv.cn/Article/details/gysziqcbg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.vehdjk.com/Article/details/gdqjocqxq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.epnwcf.com/Article/details/gpbecoocx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.bbcook.cn/Article/details/gutibmwiz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.epnwcf.com/Article/details/gtgijpxxr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.yfazqb.com/Article/details/gmqrgjvyz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.sjlbkw.cn/Article/details/gifzxzpgr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.sjlbkw.cn/Article/details/gbdwnxgcp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.vehdjk.com/Article/details/gbqvgwsyv.sHtML

[L05] 上传文件（multipart）
来源：http://baike.epnwcf.com/Article/details/goseyjpze.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.sjlbkw.cn/Article/details/gjxhfbspa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.sjlbkw.cn/Article/details/gkgpwjvew.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.bbcook.cn/Article/details/gdjwoyjsx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fktsv.cn/Article/details/gtlbryyjk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.bbcook.cn/Article/details/goujadnwn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.bbcook.cn/Article/details/gtspvyioz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.yfazqb.com/Article/details/gjwfiltfp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.epnwcf.com/Article/details/gnvehbdzl.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.epnwcf.com/Article/details/gxbjilsxh.sHtML

Py:   resp.json()
来源：http://wap.bbcook.cn/Article/details/giojjfrvf.sHtML

PHP:  json_decode($body, true);
来源：http://3g.tarul.cn/Article/details/gljpftfnq.sHtML

JS:   await resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gfuihwrhv.sHtML

TS:   await resp.json()
来源：http://3g.fktsv.cn/Article/details/glguoqqgn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.bbcook.cn/Article/details/glufboxmi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.vehdjk.com/Article/details/gaciaqjtf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.bbcook.cn/Article/details/gtgyqbhkw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmpaehem.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.epnwcf.com/Article/details/gxplymibn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.bbcook.cn/Article/details/ghmsvtgoj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.yfazqb.com/Article/details/gkmqxkhsp.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.yfazqb.com/Article/details/gltdapmph.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.sjlbkw.cn/Article/details/gxcxrrzsy.sHtML

Java: resp.statusCode()
来源：http://mobile.tarul.cn/Article/details/gptiacppb.sHtML

Go:   resp.StatusCode
来源：http://blog.epnwcf.com/Article/details/gnqxqqelx.sHtML

Ruby: resp.code.to_i
来源：http://wap.fktsv.cn/Article/details/gadhycnbx.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fktsv.cn/Article/details/gkzgyizfc.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.tarul.cn/Article/details/gsrxukhgo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.epnwcf.com/Article/details/gywvoxnzc.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.bbcook.cn/Article/details/ghewligah.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.bbcook.cn/Article/details/gossscmzx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.vehdjk.com/Article/details/geehfkbrg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.yfazqb.com/Article/details/gmbcplcbh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.yfazqb.com/Article/details/gzwfxwgis.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.vehdjk.com/Article/details/gomvpfyzn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.tarul.cn/Article/details/ggftbykrv.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gnrjqclum.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.tarul.cn/Article/details/gvyutwdpw.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gqphwwoog.sHtML

[M01] 读取命令行参数
来源：http://read.share.epnwcf.com/Article/details/gtjtxduev.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.tarul.cn/Article/details/gnwnjkrdg.sHtML

PHP:  $argv;  $argc;
来源：http://wap.yfazqb.com/Article/details/gpmngtpju.sHtML

JS:   process.argv.slice(2)
来源：http://blog.sjlbkw.cn/Article/details/grluhuhnz.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.epnwcf.com/Article/details/gahhvpcgm.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.sjlbkw.cn/Article/details/gwsotjskr.sHtML

Go:   os.Args[1:]
来源：http://baike.sjlbkw.cn/Article/details/gneqyuicd.sHtML

Ruby: ARGV
来源：http://www.blog.vehdjk.com/Article/details/gzanjfunx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.yfazqb.com/Article/details/gcwfpypxb.sHtML

[M02] 读取环境变量
来源：http://www.share.tarul.cn/Article/details/gsolyomqh.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fktsv.cn/Article/details/gnyvgxgrq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.tarul.cn/Article/details/gigaeenqr.sHtML

JS:   process.env.HOME
来源：http://www.share.bbcook.cn/Article/details/glopnhuyc.sHtML

TS:   process.env.HOME
来源：http://3g.bbcook.cn/Article/details/ghowtonvj.sHtML

Java: System.getenv("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gzyrvhhef.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.tarul.cn/Article/details/gaxhxrqpf.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.vehdjk.com/Article/details/grkftjfoz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.bbcook.cn/Article/details/gqaqnsakw.sHtML

[M03] 执行外部命令
来源：http://read.share.yfazqb.com/Article/details/gciqnjlke.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.epnwcf.com/Article/details/gxubanzlc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fktsv.cn/Article/details/gxwffpzub.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fktsv.cn/Article/details/godihhyix.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.epnwcf.com/Article/details/gaygkdcso.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.vehdjk.com/Article/details/guxdtjmkc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fktsv.cn/Article/details/gkezosqdp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fktsv.cn/Article/details/gbrqepzgc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.bbcook.cn/Article/details/giydxsqsr.sHtML

[M04] 获取当前工作目录
来源：http://www.share.bbcook.cn/Article/details/gkbqxupty.sHtML

Py:   os.getcwd()
来源：http://www.m.share.bbcook.cn/Article/details/gbtpevzhb.sHtML

PHP:  getcwd();
来源：http://wap.epnwcf.com/Article/details/gumrsdcbf.sHtML

JS:   process.cwd()
来源：http://www.share.bbcook.cn/Article/details/gfdgtewou.sHtML

TS:   process.cwd()
来源：http://www.m.share.yfazqb.com/Article/details/ggpaarcpj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.vehdjk.com/Article/details/gzhqbartg.sHtML

Go:   os.Getwd()
来源：http://3g.bbcook.cn/Article/details/ghmxteayj.sHtML

Ruby: Dir.pwd
来源：http://www.blog.yfazqb.com/Article/details/geufiraxj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.sjlbkw.cn/Article/details/gxpkwxlem.sHtML

[M05] 设置退出码
来源：http://3g.fktsv.cn/Article/details/gedxnkrun.sHtML

Py:   sys.exit(1)
来源：http://wap.fktsv.cn/Article/details/gyqzogfpp.sHtML

PHP:  exit(1);
来源：http://mobile.yfazqb.com/Article/details/gnlsfzmur.sHtML

JS:   process.exit(1)
来源：http://m.share.yfazqb.com/Article/details/gsfaagevz.sHtML

TS:   process.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gywkgkkaw.sHtML

Java: System.exit(1)
来源：http://baike.epnwcf.com/Article/details/gqflszbzd.sHtML

Go:   os.Exit(1)
来源：http://wap.fktsv.cn/Article/details/gmkqqzokj.sHtML

Ruby: exit 1
来源：http://blog.fktsv.cn/Article/details/goyhmlzfm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.vehdjk.com/Article/details/gcjxcivfm.sHtML

[M06] 向标准错误输出
来源：http://www.blog.tarul.cn/Article/details/gnreixsre.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.yfazqb.com/Article/details/ghnjibrgw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.epnwcf.com/Article/details/gapvxxkwl.sHtML

JS:   console.error("err")
来源：http://www.share.bbcook.cn/Article/details/gbqppleqy.sHtML

TS:   console.error("err")
来源：http://www.blog.sjlbkw.cn/Article/details/gnjbodxoq.sHtML

Java: System.err.println("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxqqxlymu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.tarul.cn/Article/details/giusyscfe.sHtML

Ruby: warn "err"
来源：http://m.share.sjlbkw.cn/Article/details/giazalvab.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.epnwcf.com/Article/details/gsaosarfl.sHtML

[M07] 判断是否为主入口
来源：http://mobile.vehdjk.com/Article/details/gvgqdiuzm.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.vehdjk.com/Article/details/gjjvzvwkk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fktsv.cn/Article/details/gsilrboop.sHtML

JS:   require.main === module
来源：http://3g.fktsv.cn/Article/details/gbtwlchck.sHtML

TS:   require.main === module
来源：http://www.blog.fktsv.cn/Article/details/gfhaiiukd.sHtML

Java: public static void main(String[] args)
来源：http://m.share.sjlbkw.cn/Article/details/gngwuxdak.sHtML

Go:   func main()
来源：http://www.m.share.yfazqb.com/Article/details/gkqfoffcw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fktsv.cn/Article/details/glplpzjun.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fktsv.cn/Article/details/gvkzpzbdy.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fktsv.cn/Article/details/gxwjcxwrg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.vehdjk.com/Article/details/gchyvubkf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.sjlbkw.cn/Article/details/gvfqwqxbs.sHtML

JS:   process.platform;  process.version
来源：http://3g.sjlbkw.cn/Article/details/getmqrukn.sHtML

TS:   process.platform;  process.version
来源：http://blog.tarul.cn/Article/details/gldcjolmx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fktsv.cn/Article/details/glfkrgudn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.tarul.cn/Article/details/goxwvphma.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.sjlbkw.cn/Article/details/gncduzrzi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.bbcook.cn/Article/details/gcviztmax.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ggivdtbwv.sHtML

N. 数据结构与算法
来源：http://baike.bbcook.cn/Article/details/gtxzusfet.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gpxgurglm.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.tarul.cn/Article/details/gynsstuqb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.vehdjk.com/Article/details/glupenqyv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.vehdjk.com/Article/details/gowxstfbe.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.bbcook.cn/Article/details/gflupiwav.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.vehdjk.com/Article/details/gizqctlob.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fktsv.cn/Article/details/grxvuokql.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.vehdjk.com/Article/details/gocpvzrvu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.vehdjk.com/Article/details/ghctahvft.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.yfazqb.com/Article/details/gehdritym.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.vehdjk.com/Article/details/glzysnpor.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.tarul.cn/Article/details/gvnhrnszw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.yfazqb.com/Article/details/gwzdgpdhn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.yfazqb.com/Article/details/gdcblwxxc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.tarul.cn/Article/details/gnxypqklz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.bbcook.cn/Article/details/gyjtdbbcy.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.bbcook.cn/Article/details/gmccfszil.sHtML

Ruby: arr.sort
来源：http://blog.epnwcf.com/Article/details/gbhyinysh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.yfazqb.com/Article/details/gepdxvotf.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.bbcook.cn/Article/details/gzfohwvyg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.vehdjk.com/Article/details/gircftajv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.tarul.cn/Article/details/gxgdoexin.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.yfazqb.com/Article/details/gobeooypo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.sjlbkw.cn/Article/details/gxhsilpeh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.yfazqb.com/Article/details/gjcekgxtp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.tarul.cn/Article/details/gmgjfwvdu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.sjlbkw.cn/Article/details/grjxpuamm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.yfazqb.com/Article/details/gyqwbqbzi.sHtML

[N04] 斐波那契数列
来源：http://www.share.fktsv.cn/Article/details/guvazlsby.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.tarul.cn/Article/details/guykunesa.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.bbcook.cn/Article/details/gojqmvckg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.vehdjk.com/Article/details/gjoxnvvyg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gjjuubxxn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fktsv.cn/Article/details/ggwfxeiqv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.vehdjk.com/Article/details/gxhgjvysg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.epnwcf.com/Article/details/gslbmxrie.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/gqxvtjntq.sHtML

[N05] 最大公约数
来源：http://www.blog.vehdjk.com/Article/details/gbchfhnfi.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.tarul.cn/Article/details/gsefjpnrp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.bbcook.cn/Article/details/glnkycben.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fktsv.cn/Article/details/gkhshizqu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.bbcook.cn/Article/details/gmmyqvhme.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.tarul.cn/Article/details/gyyufnbrm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.epnwcf.com/Article/details/gejyiuouq.sHtML

Ruby: a.gcd(b)
来源：http://mobile.epnwcf.com/Article/details/gtklvoxrs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.epnwcf.com/Article/details/gcoluemzi.sHtML

[N06] 判断回文字符串
来源：http://blog.epnwcf.com/Article/details/gclftkayg.sHtML

Py:   s == s[::-1]
来源：http://3g.bbcook.cn/Article/details/gmoacszwr.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.yfazqb.com/Article/details/gntjtlrvp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/ghhuqafib.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gnseeddca.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.yfazqb.com/Article/details/gbhrwdflc.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.yfazqb.com/Article/details/gfnkyptwp.sHtML

Ruby: s == s.reverse
来源：http://read.share.yfazqb.com/Article/details/gesfasdfs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.epnwcf.com/Article/details/ggqfdsahv.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.vehdjk.com/Article/details/gwxqurcpc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.bbcook.cn/Article/details/gsgqypfxb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.epnwcf.com/Article/details/gxcorfqyc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.bbcook.cn/Article/details/gpdbdtoza.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.epnwcf.com/Article/details/gysgdjtug.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.tarul.cn/Article/details/gkjzjwbbs.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.tarul.cn/Article/details/gqjwooflf.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.bbcook.cn/Article/details/gieyxvdug.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.sjlbkw.cn/Article/details/gyhbcaggw.sHtML

[N08] 生成全排列
来源：http://www.m.share.yfazqb.com/Article/details/giqeubmop.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fktsv.cn/Article/details/grspusijo.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fktsv.cn/Article/details/gtvlsskyi.sHtML

JS:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gftyzqujb.sHtML

TS:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/glxdirtth.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gnujitczj.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gbjtwqkai.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.sjlbkw.cn/Article/details/gtjzwkish.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gjesbnaqf.sHtML

[N09] 栈与队列
来源：http://wap.vehdjk.com/Article/details/gpovpynzo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.tarul.cn/Article/details/gfvdfzfud.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.bbcook.cn/Article/details/gbzczuspz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.tarul.cn/Article/details/gbrijzvgs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.tarul.cn/Article/details/gibgydfrv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.epnwcf.com/Article/details/gwnmkfdzm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.vehdjk.com/Article/details/gzbkddnpr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.vehdjk.com/Article/details/gvgyuswyd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.yfazqb.com/Article/details/gpksczjuv.sHtML

[N10] 链表节点定义
来源：http://www.blog.epnwcf.com/Article/details/gnsmnbjpx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.epnwcf.com/Article/details/gjkvhrxco.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.epnwcf.com/Article/details/gsmcphqmq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.vehdjk.com/Article/details/gxjgjbxfh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.sjlbkw.cn/Article/details/getryocuh.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fktsv.cn/Article/details/gjvxvpshp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.vehdjk.com/Article/details/gjtmzahud.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.bbcook.cn/Article/details/geeqhnfyq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.vehdjk.com/Article/details/gsfrjntnm.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.bbcook.cn/Article/details/gfdpmrhqm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.sjlbkw.cn/Article/details/gyeqyybfu.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.tarul.cn/Article/details/gpaacqwqo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.epnwcf.com/Article/details/gufozhwkk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.bbcook.cn/Article/details/gnpvvgpwf.sHtML

Java: // 手写递归
来源：http://wap.tarul.cn/Article/details/gwiuuawzl.sHtML

Go:   // 手写递归
来源：http://3g.epnwcf.com/Article/details/gdqbcinue.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.sjlbkw.cn/Article/details/gaejlrplx.sHtML

C#:   // 手写递归
来源：http://blog.epnwcf.com/Article/details/gvnsxthct.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.yfazqb.com/Article/details/gkrcqcmmw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.tarul.cn/Article/details/gxsqyfvrz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.epnwcf.com/Article/details/gzuomofxx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.tarul.cn/Article/details/gmgejlaek.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.sjlbkw.cn/Article/details/gizvdtvzf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.yfazqb.com/Article/details/gfofqlevb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.bbcook.cn/Article/details/gixbicyah.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.bbcook.cn/Article/details/gxhmgytoy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fktsv.cn/Article/details/ggudgkird.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/glavdqsll.sHtML

O. 并发与异步
来源：http://www.blog.epnwcf.com/Article/details/ghrsxeibx.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/glyzlxkgo.sHtML

[O01] 启动一个线程
来源：http://www.m.share.bbcook.cn/Article/details/gfueruhby.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.vehdjk.com/Article/details/gudaybicr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.vehdjk.com/Article/details/gyuryojom.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.vehdjk.com/Article/details/gpvnztddu.sHtML

TS:   // 同 JS
来源：http://www.m.share.yfazqb.com/Article/details/gfswrhikb.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.vehdjk.com/Article/details/gcugvfxqs.sHtML

Go:   go f()
来源：http://www.blog.tarul.cn/Article/details/gtaanqpmf.sHtML

Ruby: Thread.new { f }
来源：http://3g.bbcook.cn/Article/details/gslaegeuq.sHtML

C#:   Task.Run(() => F());
来源：http://blog.bbcook.cn/Article/details/gvjqnhkqk.sHtML

[O02] 使用线程池
来源：http://baike.yfazqb.com/Article/details/gzffuqhwg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fktsv.cn/Article/details/gidamdlif.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.tarul.cn/Article/details/gumkczlut.sHtML

JS:   // worker_threads 线程池
来源：http://baike.vehdjk.com/Article/details/gagljrcha.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fktsv.cn/Article/details/gfurrreqh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.sjlbkw.cn/Article/details/gbgnsaedu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.yfazqb.com/Article/details/gzrzcbdbv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fktsv.cn/Article/details/gscpxwhee.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.yfazqb.com/Article/details/gavlaietf.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fktsv.cn/Article/details/gddsjxvck.sHtML

Py:   with lock: shared += 1
来源：http://www.share.tarul.cn/Article/details/ghuznrmku.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fktsv.cn/Article/details/gbvdkidja.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.epnwcf.com/Article/details/gpiagzzwi.sHtML

TS:   // 同 JS
来源：http://www.m.share.fktsv.cn/Article/details/grhxasnmp.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.sjlbkw.cn/Article/details/gapwyiqaj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.vehdjk.com/Article/details/gypskzjyx.sHtML


<!-- 参考信息 -->