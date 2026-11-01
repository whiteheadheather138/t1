代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gdrohgmfc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gbelfpskw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gzolomhtj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.epnwcf.com/Article/details/gawidwzxt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.vehdjk.com/Article/details/gutdwwrrv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gqolytwgv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.vehdjk.com/Article/details/gledtxksk.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.yfazqb.com/Article/details/gjgnjruce.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.bbcook.cn/Article/details/gdbycapfy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.vehdjk.com/Article/details/gkjbnyroz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.vehdjk.com/Article/details/gzhldwrov.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.yfazqb.com/Article/details/geiygcduk.sHtML

Go:   encoding/gob
来源：http://wap.bbcook.cn/Article/details/gtbofjhku.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.tarul.cn/Article/details/gscqirphn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.sjlbkw.cn/Article/details/guraskobn.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gugzwxfhr.sHtML

L. 网络请求
来源：http://wap.tarul.cn/Article/details/gdwrvicds.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gtsxvsmst.sHtML

[L01] 发送 GET 请求
来源：http://www.share.bbcook.cn/Article/details/gmvmucfbh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.vehdjk.com/Article/details/gfutwmksw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fktsv.cn/Article/details/gjzuzhjpi.sHtML

JS:   await fetch(url)
来源：http://blog.yfazqb.com/Article/details/ggclzfezg.sHtML

TS:   await fetch(url)
来源：http://blog.bbcook.cn/Article/details/gyelzqwep.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.epnwcf.com/Article/details/gjmgoxzwc.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.sjlbkw.cn/Article/details/gleisbast.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.epnwcf.com/Article/details/gsbanxgap.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.vehdjk.com/Article/details/geebvnzic.sHtML

[L02] 发送 POST JSON
来源：http://wap.vehdjk.com/Article/details/gdgvqsoox.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fktsv.cn/Article/details/gglxcmpmw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fktsv.cn/Article/details/gryfuzwxi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.tarul.cn/Article/details/guzcobefq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.bbcook.cn/Article/details/gdmeonhsy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.epnwcf.com/Article/details/gwgpgeagn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.bbcook.cn/Article/details/gzcsrjxoy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.sjlbkw.cn/Article/details/gitjjfpgj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.tarul.cn/Article/details/gaigwzpbq.sHtML

[L03] 设置自定义请求头
来源：http://mobile.sjlbkw.cn/Article/details/gkmcinnar.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fktsv.cn/Article/details/gimicwqwp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.tarul.cn/Article/details/ggwtmfyfu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.tarul.cn/Article/details/gpmahpqjm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.sjlbkw.cn/Article/details/geoarwkgb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.epnwcf.com/Article/details/gqumwrhkn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.bbcook.cn/Article/details/gumapcbay.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.yfazqb.com/Article/details/gwtkksjkd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.bbcook.cn/Article/details/grvibnxij.sHtML

[L04] 设置超时
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcveiert.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fktsv.cn/Article/details/gryysajyb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.yfazqb.com/Article/details/gtylyyoew.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gclwmqmoz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.yfazqb.com/Article/details/gndniaqoz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.epnwcf.com/Article/details/goutbamqn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.vehdjk.com/Article/details/ghafiprjq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.tarul.cn/Article/details/gshktkddz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.yfazqb.com/Article/details/gdvyznczr.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.epnwcf.com/Article/details/gpfippogh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.bbcook.cn/Article/details/gszomryau.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.vehdjk.com/Article/details/gvxnbsvjo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fktsv.cn/Article/details/gsdynsczm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.bbcook.cn/Article/details/gnszrzpsg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.epnwcf.com/Article/details/glyhxoicx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.epnwcf.com/Article/details/gcxswscaz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fktsv.cn/Article/details/ghotaqqnb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.yfazqb.com/Article/details/ggaetkgec.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.epnwcf.com/Article/details/ggtqlyjav.sHtML

Py:   resp.json()
来源：http://www.blog.vehdjk.com/Article/details/glxhbvpbx.sHtML

PHP:  json_decode($body, true);
来源：http://3g.bbcook.cn/Article/details/gefibugrp.sHtML

JS:   await resp.json()
来源：http://3g.fktsv.cn/Article/details/gtjkkakel.sHtML

TS:   await resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/golcnusjm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.yfazqb.com/Article/details/gttkkraku.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.sjlbkw.cn/Article/details/gdzztreyw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.tarul.cn/Article/details/goffnekkt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.yfazqb.com/Article/details/gnnrxmqsb.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.bbcook.cn/Article/details/gcoowbajf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fktsv.cn/Article/details/gcrkbqmwk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.vehdjk.com/Article/details/gbkwsswkh.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.sjlbkw.cn/Article/details/gbqkzdmyb.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.bbcook.cn/Article/details/gfnrfuztj.sHtML

Java: resp.statusCode()
来源：http://mobile.vehdjk.com/Article/details/gukwvavbe.sHtML

Go:   resp.StatusCode
来源：http://3g.yfazqb.com/Article/details/goivfdkxv.sHtML

Ruby: resp.code.to_i
来源：http://mobile.yfazqb.com/Article/details/gwsglyzfh.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.yfazqb.com/Article/details/gfhskxwsg.sHtML

[L08] 并发请求多个地址
来源：http://m.share.epnwcf.com/Article/details/gwybyjuem.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.sjlbkw.cn/Article/details/gmjqcguut.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.yfazqb.com/Article/details/gvvlvybzk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.epnwcf.com/Article/details/gqkmhcwdk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.sjlbkw.cn/Article/details/gwuzczqif.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.vehdjk.com/Article/details/gdizuhxfo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.tarul.cn/Article/details/giryoabel.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.epnwcf.com/Article/details/ghhyoopwh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.yfazqb.com/Article/details/gwpogadyv.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gaafmmzra.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.epnwcf.com/Article/details/gsrvmzeau.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gsfzrpvis.sHtML

[M01] 读取命令行参数
来源：http://3g.bbcook.cn/Article/details/givlabpuj.sHtML

Py:   sys.argv[1:]
来源：http://mobile.bbcook.cn/Article/details/gvanroewu.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.vehdjk.com/Article/details/guwggecsy.sHtML

JS:   process.argv.slice(2)
来源：http://baike.tarul.cn/Article/details/gbffdjulp.sHtML

TS:   process.argv.slice(2)
来源：http://baike.yfazqb.com/Article/details/gprrqozuq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.bbcook.cn/Article/details/gdtxrjdrn.sHtML

Go:   os.Args[1:]
来源：http://www.share.tarul.cn/Article/details/gcrdwroep.sHtML

Ruby: ARGV
来源：http://blog.yfazqb.com/Article/details/gmpzumllj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.epnwcf.com/Article/details/glysdpcis.sHtML

[M02] 读取环境变量
来源：http://wap.epnwcf.com/Article/details/gtvipufps.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.bbcook.cn/Article/details/gbfmudcxn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.yfazqb.com/Article/details/gruzcvskg.sHtML

JS:   process.env.HOME
来源：http://wap.tarul.cn/Article/details/grwmyyspn.sHtML

TS:   process.env.HOME
来源：http://3g.bbcook.cn/Article/details/gpfixezhj.sHtML

Java: System.getenv("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gwbbdhkeq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.tarul.cn/Article/details/gkthtfitq.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.tarul.cn/Article/details/gezgiwaib.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.tarul.cn/Article/details/giccvytny.sHtML

[M03] 执行外部命令
来源：http://wap.bbcook.cn/Article/details/gftwwmhmd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.bbcook.cn/Article/details/gcikdzswp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.bbcook.cn/Article/details/gsymuirlx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fktsv.cn/Article/details/gwgrwrbhs.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.yfazqb.com/Article/details/gerzuddvv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.tarul.cn/Article/details/gjpcawxpl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fktsv.cn/Article/details/glakohxav.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.epnwcf.com/Article/details/gzzpwbdzz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.sjlbkw.cn/Article/details/gcyannjyn.sHtML

[M04] 获取当前工作目录
来源：http://baike.sjlbkw.cn/Article/details/gyqehtcqb.sHtML

Py:   os.getcwd()
来源：http://www.m.share.yfazqb.com/Article/details/gfkvyplbr.sHtML

PHP:  getcwd();
来源：http://3g.fktsv.cn/Article/details/gwqvwixoj.sHtML

JS:   process.cwd()
来源：http://www.share.bbcook.cn/Article/details/gajlrphhp.sHtML

TS:   process.cwd()
来源：http://www.share.fktsv.cn/Article/details/gvnemqqtr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.vehdjk.com/Article/details/gaumfaqfq.sHtML

Go:   os.Getwd()
来源：http://3g.tarul.cn/Article/details/gplaqryyf.sHtML

Ruby: Dir.pwd
来源：http://baike.vehdjk.com/Article/details/gicehgvqa.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.tarul.cn/Article/details/gdaznwjuw.sHtML

[M05] 设置退出码
来源：http://www.share.bbcook.cn/Article/details/gwpajjoch.sHtML

Py:   sys.exit(1)
来源：http://baike.fktsv.cn/Article/details/gxwdihswp.sHtML

PHP:  exit(1);
来源：http://blog.bbcook.cn/Article/details/gjznwvfvu.sHtML

JS:   process.exit(1)
来源：http://m.share.bbcook.cn/Article/details/ggokbkfrx.sHtML

TS:   process.exit(1)
来源：http://blog.epnwcf.com/Article/details/ggpfmovvq.sHtML

Java: System.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gdkkemtrv.sHtML

Go:   os.Exit(1)
来源：http://read.share.bbcook.cn/Article/details/gwhngemny.sHtML

Ruby: exit 1
来源：http://wap.sjlbkw.cn/Article/details/gfuwhuqqp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fktsv.cn/Article/details/gzuuerqzi.sHtML

[M06] 向标准错误输出
来源：http://read.share.bbcook.cn/Article/details/gyqdufqfu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.sjlbkw.cn/Article/details/gbksyfaow.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.tarul.cn/Article/details/gvwybrxrv.sHtML

JS:   console.error("err")
来源：http://read.share.vehdjk.com/Article/details/ggzmygtkk.sHtML

TS:   console.error("err")
来源：http://blog.sjlbkw.cn/Article/details/gstnbtams.sHtML

Java: System.err.println("err")
来源：http://3g.vehdjk.com/Article/details/glnsajtgm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.sjlbkw.cn/Article/details/gqlvmhaxa.sHtML

Ruby: warn "err"
来源：http://www.m.share.vehdjk.com/Article/details/gbsnzevaz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.vehdjk.com/Article/details/godxhpqjo.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.sjlbkw.cn/Article/details/gbpnbetse.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.bbcook.cn/Article/details/gxbeerbgd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.vehdjk.com/Article/details/gqzdkqwin.sHtML

JS:   require.main === module
来源：http://www.m.share.yfazqb.com/Article/details/gsnqxrwjs.sHtML

TS:   require.main === module
来源：http://m.share.bbcook.cn/Article/details/grsinunjc.sHtML

Java: public static void main(String[] args)
来源：http://m.share.vehdjk.com/Article/details/ghgoawedw.sHtML

Go:   func main()
来源：http://www.blog.epnwcf.com/Article/details/gfrsbeouv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fktsv.cn/Article/details/ghslbqyfi.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.vehdjk.com/Article/details/gmtormggu.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.sjlbkw.cn/Article/details/gxzywargn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.yfazqb.com/Article/details/gqioyshnl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.yfazqb.com/Article/details/giyhhqpai.sHtML

JS:   process.platform;  process.version
来源：http://wap.epnwcf.com/Article/details/grbzprwyt.sHtML

TS:   process.platform;  process.version
来源：http://blog.fktsv.cn/Article/details/gzetegazj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.tarul.cn/Article/details/gzplckkuo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.epnwcf.com/Article/details/ghszgozmv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.epnwcf.com/Article/details/gechamwuw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.yfazqb.com/Article/details/gdfrpfqaq.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gdzaugjit.sHtML

N. 数据结构与算法
来源：http://www.blog.sjlbkw.cn/Article/details/glyzikzre.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gmpfigvgc.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.yfazqb.com/Article/details/grkqwcvxd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.epnwcf.com/Article/details/ggujddjcn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.vehdjk.com/Article/details/ggaqfhrob.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.tarul.cn/Article/details/ghvapboev.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.vehdjk.com/Article/details/gkmuuggbb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fktsv.cn/Article/details/gtvxlechz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.tarul.cn/Article/details/gcwinxqsk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.bbcook.cn/Article/details/gykhiufts.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.epnwcf.com/Article/details/grvbofyps.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.bbcook.cn/Article/details/grznryalj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.vehdjk.com/Article/details/gcarcnoqx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fktsv.cn/Article/details/gmelybodw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/glrylicom.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.vehdjk.com/Article/details/glnafynrh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.yfazqb.com/Article/details/gsdeasood.sHtML

Go:   slices.Sort(arr)
来源：http://3g.tarul.cn/Article/details/gzqajpcsx.sHtML

Ruby: arr.sort
来源：http://3g.bbcook.cn/Article/details/gvjkphppp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.vehdjk.com/Article/details/gnzqmfbid.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.bbcook.cn/Article/details/gljfuawpi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.epnwcf.com/Article/details/gqwbqmpvy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.tarul.cn/Article/details/gztuyicbj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.epnwcf.com/Article/details/gixwyjhfe.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.yfazqb.com/Article/details/gvnynjdkq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.sjlbkw.cn/Article/details/gfemmrisu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fktsv.cn/Article/details/gynudvvmf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.sjlbkw.cn/Article/details/ghlreclfv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.yfazqb.com/Article/details/gcmyglaxx.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.sjlbkw.cn/Article/details/gltewaxpn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.sjlbkw.cn/Article/details/gqzgzxfnz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.yfazqb.com/Article/details/ggrcquphn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fktsv.cn/Article/details/grwyicomq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/givmajeds.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.yfazqb.com/Article/details/gsvuchodl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.bbcook.cn/Article/details/glmoobzjv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.tarul.cn/Article/details/gpkmaemte.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gawlmkjyc.sHtML

[N05] 最大公约数
来源：http://blog.yfazqb.com/Article/details/goyrihyls.sHtML

Py:   math.gcd(a, b)
来源：http://baike.sjlbkw.cn/Article/details/gusohjbap.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fktsv.cn/Article/details/gogtwqjsp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.vehdjk.com/Article/details/gsihxcpmx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.yfazqb.com/Article/details/gqmkhtxyp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.sjlbkw.cn/Article/details/grrwrptlf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.sjlbkw.cn/Article/details/grdfxtmjf.sHtML

Ruby: a.gcd(b)
来源：http://blog.epnwcf.com/Article/details/guujvyukp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fktsv.cn/Article/details/gzjjglpty.sHtML

[N06] 判断回文字符串
来源：http://www.blog.epnwcf.com/Article/details/gfphxqwua.sHtML

Py:   s == s[::-1]
来源：http://baike.fktsv.cn/Article/details/gqmlngzfe.sHtML

PHP:  $s === strrev($s);
来源：http://3g.vehdjk.com/Article/details/gciihsrsm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/gfkowbibb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/giysgvucf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.vehdjk.com/Article/details/gvpcvoetc.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.sjlbkw.cn/Article/details/gsvjcdqhd.sHtML

Ruby: s == s.reverse
来源：http://read.share.bbcook.cn/Article/details/ggvaphwts.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fktsv.cn/Article/details/gpurgovbw.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.bbcook.cn/Article/details/glrbhlflg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.vehdjk.com/Article/details/gvwkpfgdi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.vehdjk.com/Article/details/gvwqsvndn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.bbcook.cn/Article/details/gxykedyum.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.epnwcf.com/Article/details/goeifygah.sHtML

Java: // 手写 HashMap
来源：http://blog.fktsv.cn/Article/details/gscesaloa.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.sjlbkw.cn/Article/details/gsfszhkcy.sHtML

Ruby: // 手写 Hash
来源：http://3g.sjlbkw.cn/Article/details/gncisrmoh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fktsv.cn/Article/details/gvlmgkfja.sHtML

[N08] 生成全排列
来源：http://baike.epnwcf.com/Article/details/gbcqjiykj.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fktsv.cn/Article/details/gdkwkmqag.sHtML

PHP:  // 手写递归交换
来源：http://read.share.vehdjk.com/Article/details/gawjlevhl.sHtML

JS:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gjojsyzow.sHtML

TS:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/ghenwoqwp.sHtML

Java: // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gaemmyasp.sHtML

Go:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gzdipkwlq.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.vehdjk.com/Article/details/gukpdrfyg.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gpctjwtej.sHtML

[N09] 栈与队列
来源：http://3g.epnwcf.com/Article/details/ggapsevcm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.bbcook.cn/Article/details/gztfcjahx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.tarul.cn/Article/details/gotjhqduj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.yfazqb.com/Article/details/gsvluwwbo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.epnwcf.com/Article/details/gcfsspvrf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.yfazqb.com/Article/details/guxexsxgf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.tarul.cn/Article/details/ggbfthkzp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gnjgkwyos.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.yfazqb.com/Article/details/gnpfqbwho.sHtML

[N10] 链表节点定义
来源：http://m.share.bbcook.cn/Article/details/gvcjlhgtr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.sjlbkw.cn/Article/details/gzbnowblz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.yfazqb.com/Article/details/gwoconrwh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.epnwcf.com/Article/details/gadhntqqg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.sjlbkw.cn/Article/details/gqeypzgrp.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.epnwcf.com/Article/details/gbonghwlv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.yfazqb.com/Article/details/gdwolkcyl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fktsv.cn/Article/details/glligmzmr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.yfazqb.com/Article/details/gugibmoqs.sHtML

[N11] 二叉树中序遍历
来源：http://blog.sjlbkw.cn/Article/details/gbxulsxrg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.tarul.cn/Article/details/gibinvrna.sHtML

PHP:  // 手写递归函数
来源：http://baike.fktsv.cn/Article/details/glsicimym.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.sjlbkw.cn/Article/details/godektnki.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxzzkalj.sHtML

Java: // 手写递归
来源：http://wap.fktsv.cn/Article/details/gizbongod.sHtML

Go:   // 手写递归
来源：http://blog.tarul.cn/Article/details/gpnhutwvx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.tarul.cn/Article/details/gmbywxfpn.sHtML

C#:   // 手写递归
来源：http://baike.epnwcf.com/Article/details/guyssguwt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.yfazqb.com/Article/details/gpuwlqqyx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.vehdjk.com/Article/details/gzkmikjzj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.yfazqb.com/Article/details/ghdtizgzg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.tarul.cn/Article/details/gtwnzedue.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.tarul.cn/Article/details/gtaaaeanr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.epnwcf.com/Article/details/gygnjercl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.yfazqb.com/Article/details/gidpohigc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.bbcook.cn/Article/details/gmrurligl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.vehdjk.com/Article/details/gudrzycnt.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/ghomvvppp.sHtML

O. 并发与异步
来源：http://www.blog.yfazqb.com/Article/details/gpuyltqej.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gkceyarzw.sHtML

[O01] 启动一个线程
来源：http://read.share.fktsv.cn/Article/details/gzbqoniil.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.bbcook.cn/Article/details/ggzhodltl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.vehdjk.com/Article/details/gwqwfgyhl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.tarul.cn/Article/details/glzhjnhqw.sHtML

TS:   // 同 JS
来源：http://mobile.fktsv.cn/Article/details/gvilvtpmx.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.sjlbkw.cn/Article/details/gwzpieynv.sHtML

Go:   go f()
来源：http://read.share.epnwcf.com/Article/details/goqsvtzws.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fktsv.cn/Article/details/ghyzrqfrs.sHtML

C#:   Task.Run(() => F());
来源：http://blog.sjlbkw.cn/Article/details/gssgbmemo.sHtML

[O02] 使用线程池
来源：http://baike.epnwcf.com/Article/details/grdxdfzfa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.epnwcf.com/Article/details/glkdhcsis.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.vehdjk.com/Article/details/gzgrcmmxa.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.bbcook.cn/Article/details/gpxjduxts.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.vehdjk.com/Article/details/giflnljcg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fktsv.cn/Article/details/gyizjfzye.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.epnwcf.com/Article/details/gwvpxnrfq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fktsv.cn/Article/details/glxkpjedv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.bbcook.cn/Article/details/gpsyttlku.sHtML

[O03] 加锁保护共享数据
来源：http://wap.epnwcf.com/Article/details/gocwhyqdp.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.sjlbkw.cn/Article/details/gvgkuvidd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.bbcook.cn/Article/details/gxhoxkfac.sHtML


<!-- 参考信息 -->