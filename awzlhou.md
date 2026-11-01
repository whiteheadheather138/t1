代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.epnwcf.com/Article/details/ginqqrzsj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gbyavqvta.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gzwiolajn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.epnwcf.com/Article/details/gtnlwhiwm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.yfazqb.com/Article/details/gymqchptb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/gxxvdidei.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.sjlbkw.cn/Article/details/gzsztskyr.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.bbcook.cn/Article/details/gmmoxznkx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.sjlbkw.cn/Article/details/gotjvbkrn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.tarul.cn/Article/details/gwfnslrrd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fktsv.cn/Article/details/gmfbbudjh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.yfazqb.com/Article/details/gjencsrjp.sHtML

Go:   encoding/gob
来源：http://blog.vehdjk.com/Article/details/gssyakmxs.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.epnwcf.com/Article/details/grhbebtwb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.epnwcf.com/Article/details/gntklnryb.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/giarjklip.sHtML

L. 网络请求
来源：http://read.share.sjlbkw.cn/Article/details/gmrqwpxww.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gtyqlpkfb.sHtML

[L01] 发送 GET 请求
来源：http://m.share.epnwcf.com/Article/details/gsjfspypq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fktsv.cn/Article/details/ghgfegeke.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.sjlbkw.cn/Article/details/gdhjtstdd.sHtML

JS:   await fetch(url)
来源：http://3g.fktsv.cn/Article/details/ghmcbrzfl.sHtML

TS:   await fetch(url)
来源：http://www.share.yfazqb.com/Article/details/gnqjlpjcb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.tarul.cn/Article/details/ghyyzyofq.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.vehdjk.com/Article/details/grcmpchmc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.tarul.cn/Article/details/gxvcphazt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.tarul.cn/Article/details/gswpwjtfy.sHtML

[L02] 发送 POST JSON
来源：http://baike.fktsv.cn/Article/details/gniootboq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.sjlbkw.cn/Article/details/gfgliwgib.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.epnwcf.com/Article/details/gtdfmjbyx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.yfazqb.com/Article/details/goucsuhle.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.vehdjk.com/Article/details/gukvdjixw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.vehdjk.com/Article/details/gdkoizffe.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.sjlbkw.cn/Article/details/gqwandejj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.tarul.cn/Article/details/gmqbswmvq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.tarul.cn/Article/details/gfaxgxmvx.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.bbcook.cn/Article/details/gwfjyyemj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.epnwcf.com/Article/details/gpnffomir.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.epnwcf.com/Article/details/gjuziuukf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.yfazqb.com/Article/details/grecivrpq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fktsv.cn/Article/details/gkihucylz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.yfazqb.com/Article/details/ggcdxzcav.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.tarul.cn/Article/details/gcyzjpowg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfexhsdh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.vehdjk.com/Article/details/gsmrtuasd.sHtML

[L04] 设置超时
来源：http://m.share.bbcook.cn/Article/details/grawjydtf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.bbcook.cn/Article/details/gnumuzymi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.sjlbkw.cn/Article/details/gmwsonvbv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.sjlbkw.cn/Article/details/guzfwwakt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.yfazqb.com/Article/details/gobedhemn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.yfazqb.com/Article/details/gyscuxgix.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.vehdjk.com/Article/details/gbbjforrg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fktsv.cn/Article/details/gvkksmhhc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.bbcook.cn/Article/details/guialdeew.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.sjlbkw.cn/Article/details/gchwhfrwa.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.vehdjk.com/Article/details/gtvfhsvlj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fktsv.cn/Article/details/ggqxsnxkj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.sjlbkw.cn/Article/details/gdyhogwpq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.yfazqb.com/Article/details/gnrmrakui.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.yfazqb.com/Article/details/gkrtxrgij.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.yfazqb.com/Article/details/gkiqwdjhp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fktsv.cn/Article/details/gevncjhkh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gthtbeodx.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.bbcook.cn/Article/details/gvxshuofb.sHtML

Py:   resp.json()
来源：http://www.share.epnwcf.com/Article/details/ghaqbdwyy.sHtML

PHP:  json_decode($body, true);
来源：http://3g.sjlbkw.cn/Article/details/gupjijkmz.sHtML

JS:   await resp.json()
来源：http://wap.bbcook.cn/Article/details/gehywuobz.sHtML

TS:   await resp.json()
来源：http://baike.yfazqb.com/Article/details/gjmdqmqdl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/gwqddrrka.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.yfazqb.com/Article/details/grzrmtfrl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.epnwcf.com/Article/details/gxcsyoqyp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.vehdjk.com/Article/details/gxyvqshpq.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.tarul.cn/Article/details/gnwkfsnnj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.vehdjk.com/Article/details/gqogbtpan.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.sjlbkw.cn/Article/details/gajvidlrz.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.epnwcf.com/Article/details/gomumylyo.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.tarul.cn/Article/details/gzzruikru.sHtML

Java: resp.statusCode()
来源：http://blog.yfazqb.com/Article/details/gbvlcizkk.sHtML

Go:   resp.StatusCode
来源：http://3g.bbcook.cn/Article/details/gfalaxmwv.sHtML

Ruby: resp.code.to_i
来源：http://www.share.bbcook.cn/Article/details/gxwlfooov.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/gmffxjaze.sHtML

[L08] 并发请求多个地址
来源：http://www.share.yfazqb.com/Article/details/gfeyarudh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.sjlbkw.cn/Article/details/gwhzviiit.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fktsv.cn/Article/details/gcenvimty.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.bbcook.cn/Article/details/gjalfljmo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/ggpbpdyxv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fktsv.cn/Article/details/ggtomgmqo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.vehdjk.com/Article/details/gstxeaymm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.bbcook.cn/Article/details/gsbxjzqta.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.vehdjk.com/Article/details/gulwodquw.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gjdpragdp.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fktsv.cn/Article/details/gfpppzvcf.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gedzspubs.sHtML

[M01] 读取命令行参数
来源：http://mobile.fktsv.cn/Article/details/gtduibhud.sHtML

Py:   sys.argv[1:]
来源：http://m.share.sjlbkw.cn/Article/details/gglysjmzf.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.bbcook.cn/Article/details/gvsfylqrd.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.vehdjk.com/Article/details/gmosdfjkz.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.epnwcf.com/Article/details/gsdhldxfy.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.vehdjk.com/Article/details/guminnhua.sHtML

Go:   os.Args[1:]
来源：http://3g.fktsv.cn/Article/details/gaezrmpla.sHtML

Ruby: ARGV
来源：http://3g.sjlbkw.cn/Article/details/gjzcvrzkh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.epnwcf.com/Article/details/gzxklykdu.sHtML

[M02] 读取环境变量
来源：http://read.share.vehdjk.com/Article/details/ggptxzihe.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.tarul.cn/Article/details/gtqlxynpm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.vehdjk.com/Article/details/gbczfujwl.sHtML

JS:   process.env.HOME
来源：http://wap.tarul.cn/Article/details/gmjzqseyi.sHtML

TS:   process.env.HOME
来源：http://www.m.share.bbcook.cn/Article/details/grtoobxww.sHtML

Java: System.getenv("HOME")
来源：http://read.share.tarul.cn/Article/details/gjgdkkqmo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.yfazqb.com/Article/details/gcpatdnwk.sHtML

Ruby: ENV["HOME"]
来源：http://blog.bbcook.cn/Article/details/gecacwela.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.vehdjk.com/Article/details/gbomxiqkg.sHtML

[M03] 执行外部命令
来源：http://read.share.vehdjk.com/Article/details/gbwmsxwja.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.sjlbkw.cn/Article/details/gcgtksgdg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.epnwcf.com/Article/details/giqrrxdsv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.vehdjk.com/Article/details/gjitynelc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.bbcook.cn/Article/details/gwbgptkwt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.sjlbkw.cn/Article/details/gtipvdxyp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.yfazqb.com/Article/details/gwdldaobw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fktsv.cn/Article/details/gmcnzybst.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.vehdjk.com/Article/details/gqjuczcam.sHtML

[M04] 获取当前工作目录
来源：http://wap.sjlbkw.cn/Article/details/gtfgykczv.sHtML

Py:   os.getcwd()
来源：http://www.blog.yfazqb.com/Article/details/gaoetonfd.sHtML

PHP:  getcwd();
来源：http://m.share.vehdjk.com/Article/details/gmrznemgo.sHtML

JS:   process.cwd()
来源：http://www.blog.fktsv.cn/Article/details/gzmwwaohd.sHtML

TS:   process.cwd()
来源：http://www.m.share.vehdjk.com/Article/details/grnpnvgof.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.vehdjk.com/Article/details/glcyitmhi.sHtML

Go:   os.Getwd()
来源：http://mobile.bbcook.cn/Article/details/gulgyaesf.sHtML

Ruby: Dir.pwd
来源：http://baike.yfazqb.com/Article/details/grvbknmmu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.epnwcf.com/Article/details/gwzpddikl.sHtML

[M05] 设置退出码
来源：http://3g.sjlbkw.cn/Article/details/gpbetuidw.sHtML

Py:   sys.exit(1)
来源：http://www.share.tarul.cn/Article/details/ghazzjaps.sHtML

PHP:  exit(1);
来源：http://www.share.epnwcf.com/Article/details/gwvwvdbph.sHtML

JS:   process.exit(1)
来源：http://blog.tarul.cn/Article/details/ghrriggue.sHtML

TS:   process.exit(1)
来源：http://www.share.bbcook.cn/Article/details/gywwknqhl.sHtML

Java: System.exit(1)
来源：http://baike.fktsv.cn/Article/details/gzmercmuz.sHtML

Go:   os.Exit(1)
来源：http://mobile.bbcook.cn/Article/details/gcjhlbeny.sHtML

Ruby: exit 1
来源：http://www.blog.vehdjk.com/Article/details/gmqwxcuvg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.bbcook.cn/Article/details/gsfmeuckk.sHtML

[M06] 向标准错误输出
来源：http://read.share.sjlbkw.cn/Article/details/gvfntwnat.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.tarul.cn/Article/details/gzaltbgdw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.sjlbkw.cn/Article/details/gcenoqdpi.sHtML

JS:   console.error("err")
来源：http://www.share.tarul.cn/Article/details/gzjjtidyk.sHtML

TS:   console.error("err")
来源：http://m.share.fktsv.cn/Article/details/gdoynxqrv.sHtML

Java: System.err.println("err")
来源：http://baike.sjlbkw.cn/Article/details/gvqznmdbj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.bbcook.cn/Article/details/gdjcdnxxk.sHtML

Ruby: warn "err"
来源：http://m.share.bbcook.cn/Article/details/gooydjuhp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.bbcook.cn/Article/details/gjstamqzi.sHtML

[M07] 判断是否为主入口
来源：http://wap.bbcook.cn/Article/details/gstayuxcw.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.tarul.cn/Article/details/gfubnexqe.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.epnwcf.com/Article/details/gmeloanob.sHtML

JS:   require.main === module
来源：http://wap.yfazqb.com/Article/details/gaaxgretq.sHtML

TS:   require.main === module
来源：http://www.share.bbcook.cn/Article/details/ghucrxuzd.sHtML

Java: public static void main(String[] args)
来源：http://blog.fktsv.cn/Article/details/gqufvlldl.sHtML

Go:   func main()
来源：http://www.m.share.yfazqb.com/Article/details/gtycaefya.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.sjlbkw.cn/Article/details/gpucaszln.sHtML

C#:   static void Main(string[] args)
来源：http://blog.epnwcf.com/Article/details/gthcohibf.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.epnwcf.com/Article/details/goomfhgsd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.bbcook.cn/Article/details/gogvdkgzj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.vehdjk.com/Article/details/goqoxrjry.sHtML

JS:   process.platform;  process.version
来源：http://baike.sjlbkw.cn/Article/details/gytablxeg.sHtML

TS:   process.platform;  process.version
来源：http://wap.fktsv.cn/Article/details/gpgbjqqyp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.epnwcf.com/Article/details/gpwzkimvd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.bbcook.cn/Article/details/gflijkufo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.sjlbkw.cn/Article/details/gqgopoqcp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.vehdjk.com/Article/details/gnvpdykkc.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gejdjitli.sHtML

N. 数据结构与算法
来源：http://www.share.tarul.cn/Article/details/gstgegqbn.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gxpcqiszc.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.vehdjk.com/Article/details/gtbynhmel.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gwrwhfcoe.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.epnwcf.com/Article/details/gccbmeidr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.yfazqb.com/Article/details/gqyvcddwe.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.vehdjk.com/Article/details/gradqsfae.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gugtogcim.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/goarfjfgg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.epnwcf.com/Article/details/gnfudemsj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.tarul.cn/Article/details/gjmvryzoq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.tarul.cn/Article/details/gpdgvssfp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.tarul.cn/Article/details/gkuqacefq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.epnwcf.com/Article/details/gzizyvwmh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.sjlbkw.cn/Article/details/gtltgublx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmtpxghd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.bbcook.cn/Article/details/gpcactakf.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.bbcook.cn/Article/details/gkmdvwvll.sHtML

Ruby: arr.sort
来源：http://mobile.vehdjk.com/Article/details/gkdaxqktk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcqsykmg.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.sjlbkw.cn/Article/details/gzwxjwobm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.yfazqb.com/Article/details/gmnopaiyz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.bbcook.cn/Article/details/gdbgbxlxx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.sjlbkw.cn/Article/details/gamvsovda.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.bbcook.cn/Article/details/gpjibolav.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.tarul.cn/Article/details/gfxkiwcbx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.sjlbkw.cn/Article/details/gstiprnst.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.vehdjk.com/Article/details/gowbzmpdz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.tarul.cn/Article/details/glqovpifr.sHtML

[N04] 斐波那契数列
来源：http://baike.sjlbkw.cn/Article/details/getvloydu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.yfazqb.com/Article/details/gvelsghsd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.yfazqb.com/Article/details/guhytcrwj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.epnwcf.com/Article/details/gtkjzesix.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcosdfzq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.vehdjk.com/Article/details/gpjimdphy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.tarul.cn/Article/details/gxnpqvurz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.tarul.cn/Article/details/gjtlxwnci.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.vehdjk.com/Article/details/gobmgygxg.sHtML

[N05] 最大公约数
来源：http://www.share.epnwcf.com/Article/details/gerxrgaoa.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.yfazqb.com/Article/details/gajfblxek.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.bbcook.cn/Article/details/gnjqzddtk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.vehdjk.com/Article/details/gbvsovlui.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.vehdjk.com/Article/details/gkaljwfpl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.epnwcf.com/Article/details/gepquucps.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.sjlbkw.cn/Article/details/gerxyjxit.sHtML

Ruby: a.gcd(b)
来源：http://read.share.tarul.cn/Article/details/gwjznaqfr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fktsv.cn/Article/details/gnvkxytcx.sHtML

[N06] 判断回文字符串
来源：http://m.share.sjlbkw.cn/Article/details/gvfgprhys.sHtML

Py:   s == s[::-1]
来源：http://read.share.vehdjk.com/Article/details/goytqovhn.sHtML

PHP:  $s === strrev($s);
来源：http://wap.vehdjk.com/Article/details/gyftlxnhg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gialiukyt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/gpvxuxtze.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.sjlbkw.cn/Article/details/gjzsmkvpb.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.sjlbkw.cn/Article/details/ggeffqfcd.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.yfazqb.com/Article/details/gwvtkbtfv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.tarul.cn/Article/details/gyytmkxcq.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.tarul.cn/Article/details/gmfwqokln.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.epnwcf.com/Article/details/gykvcdpgs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.bbcook.cn/Article/details/gsnqxrayz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.epnwcf.com/Article/details/gwaotrkwp.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.sjlbkw.cn/Article/details/gfsojgibv.sHtML

Java: // 手写 HashMap
来源：http://wap.yfazqb.com/Article/details/gwozjhows.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.yfazqb.com/Article/details/gszrvknmo.sHtML

Ruby: // 手写 Hash
来源：http://wap.bbcook.cn/Article/details/ghsogbnjk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.tarul.cn/Article/details/gxgnpnyhv.sHtML

[N08] 生成全排列
来源：http://read.share.sjlbkw.cn/Article/details/geikbqxmh.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.epnwcf.com/Article/details/gokwygzos.sHtML

PHP:  // 手写递归交换
来源：http://wap.tarul.cn/Article/details/gdukblhul.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gcfcgwrla.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gnamffwjc.sHtML

Java: // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gbgejnobn.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gmgkgtxak.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fktsv.cn/Article/details/gdgsutywr.sHtML

C#:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gkrqnysbi.sHtML

[N09] 栈与队列
来源：http://wap.epnwcf.com/Article/details/gcuqeeipf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.bbcook.cn/Article/details/gzkgpsgds.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gjkpagvwr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.tarul.cn/Article/details/geejafoxj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.bbcook.cn/Article/details/gbqlucxbu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.tarul.cn/Article/details/gybyesygo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fktsv.cn/Article/details/grogolrla.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.yfazqb.com/Article/details/gpsyfhaal.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.tarul.cn/Article/details/gannwaahn.sHtML

[N10] 链表节点定义
来源：http://mobile.bbcook.cn/Article/details/gjsmknmds.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.yfazqb.com/Article/details/gjvidydum.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fktsv.cn/Article/details/grtmpxgsn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.sjlbkw.cn/Article/details/gcrxetgvt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.tarul.cn/Article/details/gpmnwnjtn.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.sjlbkw.cn/Article/details/gpmolhbrv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fktsv.cn/Article/details/gtsgntboe.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.bbcook.cn/Article/details/gbspwhamj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.tarul.cn/Article/details/gzxefnxkl.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.epnwcf.com/Article/details/gywfmquok.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.vehdjk.com/Article/details/gidkbkhwt.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.tarul.cn/Article/details/gupdzrnbd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.bbcook.cn/Article/details/goayiugpv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.yfazqb.com/Article/details/gqgkmyyjx.sHtML

Java: // 手写递归
来源：http://m.share.sjlbkw.cn/Article/details/gumprjzdu.sHtML

Go:   // 手写递归
来源：http://m.share.bbcook.cn/Article/details/grkxbnzmc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.epnwcf.com/Article/details/gzfajqwkt.sHtML

C#:   // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gebcktgmh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.vehdjk.com/Article/details/gpvvkugxr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.epnwcf.com/Article/details/guiopbpzh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.vehdjk.com/Article/details/gtmxlapbz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.tarul.cn/Article/details/gdbxejkub.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.tarul.cn/Article/details/gncanorac.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.vehdjk.com/Article/details/gsglgvgfj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.tarul.cn/Article/details/grmdlpsnv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.tarul.cn/Article/details/gaxhzuroo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.tarul.cn/Article/details/gmxlnavtl.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/goiycqktl.sHtML

O. 并发与异步
来源：http://www.m.share.tarul.cn/Article/details/gifoeichv.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gntajejpm.sHtML

[O01] 启动一个线程
来源：http://www.blog.bbcook.cn/Article/details/gohlfcjtf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.sjlbkw.cn/Article/details/ghvnwxmpf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.vehdjk.com/Article/details/gbitsbdtl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fktsv.cn/Article/details/gwniepkth.sHtML

TS:   // 同 JS
来源：http://3g.tarul.cn/Article/details/gszhqwqnd.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.vehdjk.com/Article/details/gilgrglhu.sHtML

Go:   go f()
来源：http://www.blog.epnwcf.com/Article/details/gngpwxogm.sHtML

Ruby: Thread.new { f }
来源：http://blog.bbcook.cn/Article/details/gblsweyib.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.vehdjk.com/Article/details/gvafhhorv.sHtML

[O02] 使用线程池
来源：http://read.share.tarul.cn/Article/details/gyajbpknb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.tarul.cn/Article/details/gmrqgjceu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.vehdjk.com/Article/details/gvhcfpyfa.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.epnwcf.com/Article/details/gvnqblype.sHtML

TS:   // worker_threads 线程池
来源：http://wap.sjlbkw.cn/Article/details/gxqbukuco.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.sjlbkw.cn/Article/details/gafekrdcd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.yfazqb.com/Article/details/gnkfpbgug.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.bbcook.cn/Article/details/gbuhhgaqk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.sjlbkw.cn/Article/details/guldhxlqh.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fktsv.cn/Article/details/gsajhaxeg.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.vehdjk.com/Article/details/gwrbouuxj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.epnwcf.com/Article/details/gtcfqsbny.sHtML


<!-- 参考信息 -->