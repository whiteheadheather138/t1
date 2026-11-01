代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.yfazqb.com/Article/details/gpiuqqbyh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/griyqqrxu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gzmosseip.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.yfazqb.com/Article/details/glfgilboc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.vehdjk.com/Article/details/ggommbguw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/guxeexzdy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.sjlbkw.cn/Article/details/gdsdrtsis.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.bbcook.cn/Article/details/gxalqggcx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.bbcook.cn/Article/details/gprlnbbbh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.yfazqb.com/Article/details/gohohbqan.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.epnwcf.com/Article/details/gqhuvhxoi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.vehdjk.com/Article/details/goaxnmsrq.sHtML

Go:   encoding/gob
来源：http://www.share.yfazqb.com/Article/details/gkzaadamy.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.bbcook.cn/Article/details/gkhlpnksa.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.epnwcf.com/Article/details/gkimeasyg.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/grrvyzhfr.sHtML

L. 网络请求
来源：http://wap.yfazqb.com/Article/details/gnbudxibh.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gqpwemgoj.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.tarul.cn/Article/details/gjipfdlby.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.epnwcf.com/Article/details/gtxsboboy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.bbcook.cn/Article/details/gryhlvioc.sHtML

JS:   await fetch(url)
来源：http://mobile.epnwcf.com/Article/details/gtnpwtfpk.sHtML

TS:   await fetch(url)
来源：http://baike.vehdjk.com/Article/details/gpxnapexg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.epnwcf.com/Article/details/gampbjhsr.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.epnwcf.com/Article/details/grkbyrazk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.bbcook.cn/Article/details/gcnlogxed.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.vehdjk.com/Article/details/gqfepxeca.sHtML

[L02] 发送 POST JSON
来源：http://wap.tarul.cn/Article/details/gdymizmrv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.vehdjk.com/Article/details/gocvgjqsi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.sjlbkw.cn/Article/details/geyxqpxwe.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.vehdjk.com/Article/details/gqyhkgawy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.epnwcf.com/Article/details/gqjnwbgmz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.yfazqb.com/Article/details/gldschwzs.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.sjlbkw.cn/Article/details/gugewcgsh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.epnwcf.com/Article/details/gqujixcux.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fktsv.cn/Article/details/gmapzizsc.sHtML

[L03] 设置自定义请求头
来源：http://3g.yfazqb.com/Article/details/gesgrzkzi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.sjlbkw.cn/Article/details/gbzcwyolx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.yfazqb.com/Article/details/gpxruzpnz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fktsv.cn/Article/details/gpvnlvyjj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.tarul.cn/Article/details/gfpdhehde.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.vehdjk.com/Article/details/gzsnkkspk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.sjlbkw.cn/Article/details/ggozmqkdo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.yfazqb.com/Article/details/gppidcvbu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.bbcook.cn/Article/details/gprlpummh.sHtML

[L04] 设置超时
来源：http://www.blog.tarul.cn/Article/details/gbxrtbink.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.tarul.cn/Article/details/gbbywdvyc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.yfazqb.com/Article/details/gyazjivpo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.bbcook.cn/Article/details/gtdievsmu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fktsv.cn/Article/details/gdddjrgns.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.sjlbkw.cn/Article/details/gltqmtnxr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.tarul.cn/Article/details/gzsksifyv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fktsv.cn/Article/details/gkjrwryze.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.yfazqb.com/Article/details/gefcezebo.sHtML

[L05] 上传文件（multipart）
来源：http://blog.yfazqb.com/Article/details/ggtewidqy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fktsv.cn/Article/details/grmjrgmtj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.sjlbkw.cn/Article/details/guhbrsabd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.bbcook.cn/Article/details/gmxwtcgii.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.epnwcf.com/Article/details/gqdhbiizt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.tarul.cn/Article/details/gbhrixfop.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fktsv.cn/Article/details/gukybwktu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fktsv.cn/Article/details/gjhriuqzn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gskodsuqf.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fktsv.cn/Article/details/gnucybahc.sHtML

Py:   resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/gelxvfbet.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fktsv.cn/Article/details/gbxdatfir.sHtML

JS:   await resp.json()
来源：http://m.share.tarul.cn/Article/details/gmtsohzsf.sHtML

TS:   await resp.json()
来源：http://mobile.bbcook.cn/Article/details/gatteepgs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/gbcrbdthz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.vehdjk.com/Article/details/gfzkamnxk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.epnwcf.com/Article/details/gvusdhejy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.epnwcf.com/Article/details/gspfqimrv.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.tarul.cn/Article/details/gvlpjitqc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.bbcook.cn/Article/details/gdezjtfgk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.yfazqb.com/Article/details/gejzibjhd.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fktsv.cn/Article/details/gcntiqcjf.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.epnwcf.com/Article/details/gwtqwvmjb.sHtML

Java: resp.statusCode()
来源：http://www.blog.bbcook.cn/Article/details/ghatahbbn.sHtML

Go:   resp.StatusCode
来源：http://www.blog.yfazqb.com/Article/details/gduvgjvrg.sHtML

Ruby: resp.code.to_i
来源：http://wap.bbcook.cn/Article/details/gmoyjeecy.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.yfazqb.com/Article/details/guiohfajb.sHtML

[L08] 并发请求多个地址
来源：http://baike.sjlbkw.cn/Article/details/gauvxvmua.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.tarul.cn/Article/details/gkqivbdpz.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.yfazqb.com/Article/details/giethqjnv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gwzhkkfeu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.sjlbkw.cn/Article/details/gfaaabryf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.sjlbkw.cn/Article/details/gxbmhdtey.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fktsv.cn/Article/details/gqzyfgwff.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.bbcook.cn/Article/details/gdenqnttx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.yfazqb.com/Article/details/gswaujrop.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/goaahrptg.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.epnwcf.com/Article/details/gkuavtfaz.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gtmwtuoip.sHtML

[M01] 读取命令行参数
来源：http://www.share.tarul.cn/Article/details/gygfmfxvv.sHtML

Py:   sys.argv[1:]
来源：http://mobile.tarul.cn/Article/details/gkbhmliol.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.yfazqb.com/Article/details/grkshnymv.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.sjlbkw.cn/Article/details/gxdwmjflo.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.bbcook.cn/Article/details/ghghubgbv.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.bbcook.cn/Article/details/gjbynzsbw.sHtML

Go:   os.Args[1:]
来源：http://blog.yfazqb.com/Article/details/gdixlmijg.sHtML

Ruby: ARGV
来源：http://www.share.bbcook.cn/Article/details/giskglfmo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.vehdjk.com/Article/details/geeujtukr.sHtML

[M02] 读取环境变量
来源：http://3g.yfazqb.com/Article/details/gvdpcztqx.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.epnwcf.com/Article/details/gvdytkcbv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.vehdjk.com/Article/details/gixrnovfc.sHtML

JS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/gyqhiysxk.sHtML

TS:   process.env.HOME
来源：http://read.share.tarul.cn/Article/details/gbyjfpgru.sHtML

Java: System.getenv("HOME")
来源：http://m.share.vehdjk.com/Article/details/gxfcserbt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.bbcook.cn/Article/details/gtzqqybou.sHtML

Ruby: ENV["HOME"]
来源：http://blog.epnwcf.com/Article/details/gdyskzsqg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.tarul.cn/Article/details/gvnstoqsr.sHtML

[M03] 执行外部命令
来源：http://mobile.epnwcf.com/Article/details/gwbrlzexj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.epnwcf.com/Article/details/gbxhsavog.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.sjlbkw.cn/Article/details/gswsfzequ.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.yfazqb.com/Article/details/gjjprndhg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.bbcook.cn/Article/details/gzeskrnos.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.epnwcf.com/Article/details/gcrdrazcd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.epnwcf.com/Article/details/ghdurowje.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.tarul.cn/Article/details/gcoarkftd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.sjlbkw.cn/Article/details/gqgtbsayk.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.bbcook.cn/Article/details/gfafsthtd.sHtML

Py:   os.getcwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdpdggze.sHtML

PHP:  getcwd();
来源：http://m.share.bbcook.cn/Article/details/glvdbwxin.sHtML

JS:   process.cwd()
来源：http://www.m.share.vehdjk.com/Article/details/glftgffht.sHtML

TS:   process.cwd()
来源：http://3g.yfazqb.com/Article/details/gfpuvirmx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.yfazqb.com/Article/details/gbenfsqyw.sHtML

Go:   os.Getwd()
来源：http://www.blog.fktsv.cn/Article/details/gmbwuibsa.sHtML

Ruby: Dir.pwd
来源：http://read.share.sjlbkw.cn/Article/details/gipmptfts.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.tarul.cn/Article/details/ggovhjudg.sHtML

[M05] 设置退出码
来源：http://mobile.epnwcf.com/Article/details/gszegadhi.sHtML

Py:   sys.exit(1)
来源：http://3g.tarul.cn/Article/details/gglozvlgr.sHtML

PHP:  exit(1);
来源：http://blog.yfazqb.com/Article/details/gqcorerww.sHtML

JS:   process.exit(1)
来源：http://wap.bbcook.cn/Article/details/gvthaefxj.sHtML

TS:   process.exit(1)
来源：http://baike.vehdjk.com/Article/details/gapwmoftd.sHtML

Java: System.exit(1)
来源：http://www.share.bbcook.cn/Article/details/gvlfdfanh.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gmfxsfkfc.sHtML

Ruby: exit 1
来源：http://www.share.tarul.cn/Article/details/guqdihnqx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.epnwcf.com/Article/details/gxrgcjpkl.sHtML

[M06] 向标准错误输出
来源：http://www.share.yfazqb.com/Article/details/glptkwali.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.tarul.cn/Article/details/gtfiniopv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fktsv.cn/Article/details/gzypikhmn.sHtML

JS:   console.error("err")
来源：http://www.share.sjlbkw.cn/Article/details/giujtndmb.sHtML

TS:   console.error("err")
来源：http://m.share.vehdjk.com/Article/details/gjnrsfmrd.sHtML

Java: System.err.println("err")
来源：http://3g.tarul.cn/Article/details/gghfkakry.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.epnwcf.com/Article/details/gjpnmogyw.sHtML

Ruby: warn "err"
来源：http://m.share.yfazqb.com/Article/details/gqgjwesxq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.yfazqb.com/Article/details/gaafszwax.sHtML

[M07] 判断是否为主入口
来源：http://mobile.bbcook.cn/Article/details/gihoqatyc.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.vehdjk.com/Article/details/gwzfgxtei.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.epnwcf.com/Article/details/gghqfkvlx.sHtML

JS:   require.main === module
来源：http://www.share.epnwcf.com/Article/details/gaolmcdgb.sHtML

TS:   require.main === module
来源：http://www.share.bbcook.cn/Article/details/gvcualmje.sHtML

Java: public static void main(String[] args)
来源：http://baike.fktsv.cn/Article/details/ggdeefhwy.sHtML

Go:   func main()
来源：http://3g.tarul.cn/Article/details/gmrpkdxjb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.vehdjk.com/Article/details/gxsaoiech.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.yfazqb.com/Article/details/gqawtlmjh.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.yfazqb.com/Article/details/gexuuafsu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.yfazqb.com/Article/details/gqzflizpg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fktsv.cn/Article/details/guktkzpos.sHtML

JS:   process.platform;  process.version
来源：http://www.share.tarul.cn/Article/details/guroynhfj.sHtML

TS:   process.platform;  process.version
来源：http://blog.tarul.cn/Article/details/gvoectrix.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.sjlbkw.cn/Article/details/gxpxiwozb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.tarul.cn/Article/details/gbeaixliz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.epnwcf.com/Article/details/gsepueguo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.yfazqb.com/Article/details/gnkfolktu.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gaeexbncb.sHtML

N. 数据结构与算法
来源：http://3g.epnwcf.com/Article/details/glwoiqsmr.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gzcytkeln.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fktsv.cn/Article/details/gcctkxriv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gghyqwgaq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gejetxbdt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gbffsljsi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/gbzmfnkna.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.yfazqb.com/Article/details/gyrksdukf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gscymjxtu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.epnwcf.com/Article/details/gcrpbpxef.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gmmwjmlso.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.yfazqb.com/Article/details/giqesoaeo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.bbcook.cn/Article/details/gkzffhjxw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.vehdjk.com/Article/details/gccpbjccc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.vehdjk.com/Article/details/geyfqgqhd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/glfrrpico.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.vehdjk.com/Article/details/ggmsephbw.sHtML

Go:   slices.Sort(arr)
来源：http://wap.vehdjk.com/Article/details/gmzgilykl.sHtML

Ruby: arr.sort
来源：http://www.m.share.vehdjk.com/Article/details/gcdusysfg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.tarul.cn/Article/details/gsetopzhz.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fktsv.cn/Article/details/gdmyszpny.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.vehdjk.com/Article/details/grfphixre.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.tarul.cn/Article/details/gjjztopho.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.sjlbkw.cn/Article/details/gdkhardqi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.yfazqb.com/Article/details/gcvqwmbxd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.epnwcf.com/Article/details/gqlxwjcvs.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.tarul.cn/Article/details/gvcftwbxw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.vehdjk.com/Article/details/gfqczdmql.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.bbcook.cn/Article/details/gwujcsezw.sHtML

[N04] 斐波那契数列
来源：http://blog.bbcook.cn/Article/details/ghfipyooi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fktsv.cn/Article/details/gledaxdyf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.sjlbkw.cn/Article/details/gigudffrj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.tarul.cn/Article/details/gsfafcuiy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/ggdczlqqn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.tarul.cn/Article/details/gwwevkncz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.tarul.cn/Article/details/gcdqwxwgc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.vehdjk.com/Article/details/gcbeztyhk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.epnwcf.com/Article/details/ghfsvncda.sHtML

[N05] 最大公约数
来源：http://www.share.sjlbkw.cn/Article/details/gkvrsysng.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fktsv.cn/Article/details/gqpjiwnfj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.tarul.cn/Article/details/gdnfbgenh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.bbcook.cn/Article/details/gbadbzyvu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.yfazqb.com/Article/details/gahipabef.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.tarul.cn/Article/details/grtmomiah.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.yfazqb.com/Article/details/gbgsgcyum.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.yfazqb.com/Article/details/gcdhzdxxh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.vehdjk.com/Article/details/goafdknor.sHtML

[N06] 判断回文字符串
来源：http://www.blog.epnwcf.com/Article/details/gersysmib.sHtML

Py:   s == s[::-1]
来源：http://www.blog.tarul.cn/Article/details/gmtlgetfk.sHtML

PHP:  $s === strrev($s);
来源：http://wap.bbcook.cn/Article/details/gfxdmnuia.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gnffghenh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gmrwnmeje.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fktsv.cn/Article/details/gunqaztfg.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.sjlbkw.cn/Article/details/grnypakkc.sHtML

Ruby: s == s.reverse
来源：http://m.share.epnwcf.com/Article/details/gijummvbn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.vehdjk.com/Article/details/giikkomib.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.yfazqb.com/Article/details/gsbrozlli.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.yfazqb.com/Article/details/gteoaehyp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.vehdjk.com/Article/details/gyxssbhur.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fktsv.cn/Article/details/geotksfmf.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.bbcook.cn/Article/details/gzoxtbjdm.sHtML

Java: // 手写 HashMap
来源：http://baike.fktsv.cn/Article/details/gpguionwj.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.yfazqb.com/Article/details/gnawxffke.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.epnwcf.com/Article/details/gdmvwrjlw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.vehdjk.com/Article/details/gfnbfezpu.sHtML

[N08] 生成全排列
来源：http://mobile.vehdjk.com/Article/details/gahywcstm.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.epnwcf.com/Article/details/gdgruxafj.sHtML

PHP:  // 手写递归交换
来源：http://read.share.epnwcf.com/Article/details/gycehofvy.sHtML

JS:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gooalibrh.sHtML

TS:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gvqjdkjbv.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/ghzitroxb.sHtML

Go:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/glrzsohbl.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.epnwcf.com/Article/details/gbsdmklmw.sHtML

C#:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/ghwyhpnwf.sHtML

[N09] 栈与队列
来源：http://m.share.vehdjk.com/Article/details/gevogvzks.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fktsv.cn/Article/details/gzkfwgopt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.tarul.cn/Article/details/gelebihco.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gbmsxxntk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.tarul.cn/Article/details/gljfpdkvb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.yfazqb.com/Article/details/gmjpkvptf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.yfazqb.com/Article/details/gzukgbida.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.tarul.cn/Article/details/gtlqtgejw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.sjlbkw.cn/Article/details/gkvxnvbdz.sHtML

[N10] 链表节点定义
来源：http://3g.fktsv.cn/Article/details/gmklnnhka.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.bbcook.cn/Article/details/ggxvhjofs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.vehdjk.com/Article/details/gszpbpkui.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.bbcook.cn/Article/details/gtdyzakeu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.vehdjk.com/Article/details/gxdarynkv.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fktsv.cn/Article/details/gfdrnzmvf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.sjlbkw.cn/Article/details/gebhjpljj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.bbcook.cn/Article/details/gedfjpjca.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.yfazqb.com/Article/details/gvxrvfwzu.sHtML

[N11] 二叉树中序遍历
来源：http://baike.epnwcf.com/Article/details/gfrnoqcmr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.yfazqb.com/Article/details/gursswhgs.sHtML

PHP:  // 手写递归函数
来源：http://mobile.tarul.cn/Article/details/gwfsnapsj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.epnwcf.com/Article/details/ghifrjtxs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.tarul.cn/Article/details/gpfrtjzjn.sHtML

Java: // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gsrzzbymx.sHtML

Go:   // 手写递归
来源：http://www.share.fktsv.cn/Article/details/ghrjlmnhi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.tarul.cn/Article/details/glyoizczb.sHtML

C#:   // 手写递归
来源：http://baike.fktsv.cn/Article/details/gegblbiii.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.vehdjk.com/Article/details/gwoifugiu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.sjlbkw.cn/Article/details/gbqooxegc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.yfazqb.com/Article/details/gxlhhqamo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.vehdjk.com/Article/details/gpabnyysh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.tarul.cn/Article/details/gfafsgqar.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.bbcook.cn/Article/details/gbyyyjpwj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.sjlbkw.cn/Article/details/gekysmdvj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.epnwcf.com/Article/details/gejivpdkg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.sjlbkw.cn/Article/details/gaavgecuw.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gxaywenzh.sHtML

O. 并发与异步
来源：http://baike.epnwcf.com/Article/details/gnyvacwos.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gjzltfntd.sHtML

[O01] 启动一个线程
来源：http://m.share.epnwcf.com/Article/details/gjhrtxjaz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fktsv.cn/Article/details/gqscdfvnx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.tarul.cn/Article/details/gmxuginev.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.yfazqb.com/Article/details/gmmzveqag.sHtML

TS:   // 同 JS
来源：http://3g.sjlbkw.cn/Article/details/gnrqduqgf.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.tarul.cn/Article/details/gtaemuqoj.sHtML

Go:   go f()
来源：http://www.share.sjlbkw.cn/Article/details/gmcqatfes.sHtML

Ruby: Thread.new { f }
来源：http://wap.tarul.cn/Article/details/geqmiidxa.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.sjlbkw.cn/Article/details/gxyjgfcdj.sHtML

[O02] 使用线程池
来源：http://blog.bbcook.cn/Article/details/ggjowwyxh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.bbcook.cn/Article/details/gpplmivsm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.sjlbkw.cn/Article/details/gmsayaxcp.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.epnwcf.com/Article/details/ggezmdmwb.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fktsv.cn/Article/details/gvfagqrfr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.sjlbkw.cn/Article/details/gyvynmxek.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.sjlbkw.cn/Article/details/gljfhaesj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.epnwcf.com/Article/details/godnoqhip.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.vehdjk.com/Article/details/gxabgzcbe.sHtML

[O03] 加锁保护共享数据
来源：http://wap.tarul.cn/Article/details/gurhxnnlb.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.sjlbkw.cn/Article/details/gpnwdiuod.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.sjlbkw.cn/Article/details/gxbbgahgb.sHtML


<!-- 参考信息 -->