代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.tarul.cn/Article/details/gywpwkmft.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fktsv.cn/Article/details/glacdaqoa.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.tarul.cn/Article/details/gbnkilrnu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.tarul.cn/Article/details/gipqddphy.sHtML

Go:   encoding/gob
来源：http://blog.epnwcf.com/Article/details/gecokbqdq.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.yfazqb.com/Article/details/gbvzmnhgg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.sjlbkw.cn/Article/details/gdqxwcujl.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/giaisxhiq.sHtML

L. 网络请求
来源：http://www.share.vehdjk.com/Article/details/gzquuraxs.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gttqgzuju.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.epnwcf.com/Article/details/gdnyrkoib.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.sjlbkw.cn/Article/details/gdjxmkabk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.tarul.cn/Article/details/guckukdyt.sHtML

JS:   await fetch(url)
来源：http://www.blog.epnwcf.com/Article/details/gwoxvobpx.sHtML

TS:   await fetch(url)
来源：http://read.share.sjlbkw.cn/Article/details/gkafaeyxs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.bbcook.cn/Article/details/gjmhnrbpd.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fktsv.cn/Article/details/gxnvtbavs.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.sjlbkw.cn/Article/details/gseizlnhd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.vehdjk.com/Article/details/gaxaabbcm.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fktsv.cn/Article/details/gssgyssyo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.sjlbkw.cn/Article/details/gieyphpxc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.sjlbkw.cn/Article/details/gyyiajqfy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.sjlbkw.cn/Article/details/gpaboizas.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.vehdjk.com/Article/details/gsqoxvutg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.vehdjk.com/Article/details/gxiiniydt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fktsv.cn/Article/details/gvxdormcy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fktsv.cn/Article/details/gbjquxihd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.tarul.cn/Article/details/gquqlcffd.sHtML

[L03] 设置自定义请求头
来源：http://blog.yfazqb.com/Article/details/gbqriecwh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.yfazqb.com/Article/details/guokuuxwp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.yfazqb.com/Article/details/gryoerini.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fktsv.cn/Article/details/ggaxytrbo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.tarul.cn/Article/details/glydgarnb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fktsv.cn/Article/details/gqtlshbfx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.sjlbkw.cn/Article/details/gzbgilhdz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.yfazqb.com/Article/details/gxtzpvwbc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.bbcook.cn/Article/details/gjmxfmbsh.sHtML

[L04] 设置超时
来源：http://www.blog.tarul.cn/Article/details/gevjybfak.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.yfazqb.com/Article/details/gfxevyemh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.sjlbkw.cn/Article/details/gqkhdvhng.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fktsv.cn/Article/details/gxxjosuif.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.tarul.cn/Article/details/grrolhuhd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.yfazqb.com/Article/details/gzabnpmko.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.tarul.cn/Article/details/gpzoydevu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.bbcook.cn/Article/details/gtauejedw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.bbcook.cn/Article/details/gzkvidoeq.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.yfazqb.com/Article/details/gswllktdy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.yfazqb.com/Article/details/gdjikmcsx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.bbcook.cn/Article/details/gyqhvkhyb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.sjlbkw.cn/Article/details/gvzeflqvc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.bbcook.cn/Article/details/gdbcqeutv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.epnwcf.com/Article/details/gwmfkocvl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.yfazqb.com/Article/details/gwzoxwmys.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.bbcook.cn/Article/details/gesgfoliq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gbnhyoqps.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fktsv.cn/Article/details/gebvinqcd.sHtML

Py:   resp.json()
来源：http://baike.yfazqb.com/Article/details/gsakoajjl.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fktsv.cn/Article/details/gjoplbwbf.sHtML

JS:   await resp.json()
来源：http://www.m.share.fktsv.cn/Article/details/gmgfuvwug.sHtML

TS:   await resp.json()
来源：http://3g.bbcook.cn/Article/details/gijjcclpb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/gybdpdhue.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fktsv.cn/Article/details/gotjhryhd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.tarul.cn/Article/details/gjampkgkv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.tarul.cn/Article/details/guscqudgx.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fktsv.cn/Article/details/gofiyyyqg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.sjlbkw.cn/Article/details/gsqtzxnkr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.yfazqb.com/Article/details/gehninucy.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.bbcook.cn/Article/details/ghsqurajs.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.sjlbkw.cn/Article/details/grfpigcog.sHtML

Java: resp.statusCode()
来源：http://baike.fktsv.cn/Article/details/gnbpzjehw.sHtML

Go:   resp.StatusCode
来源：http://3g.epnwcf.com/Article/details/goeozaeay.sHtML

Ruby: resp.code.to_i
来源：http://baike.bbcook.cn/Article/details/gqbihfoou.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fktsv.cn/Article/details/gnuiqctnz.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fktsv.cn/Article/details/gcvqsjpig.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.sjlbkw.cn/Article/details/grmifcaxv.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.bbcook.cn/Article/details/gztkmidri.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.sjlbkw.cn/Article/details/gzgtfnznd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/gxcdvkrdd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.tarul.cn/Article/details/gubzwgbui.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.sjlbkw.cn/Article/details/gymcwzyld.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.bbcook.cn/Article/details/gvsbxjhqf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.vehdjk.com/Article/details/gywhepiqs.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gozqwlgbg.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.bbcook.cn/Article/details/gkcfxhkul.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gsbsoodca.sHtML

[M01] 读取命令行参数
来源：http://blog.yfazqb.com/Article/details/gthfgrssm.sHtML

Py:   sys.argv[1:]
来源：http://read.share.yfazqb.com/Article/details/gauuhenhk.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.bbcook.cn/Article/details/gmxgfbhsf.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fktsv.cn/Article/details/gbsbdyeth.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.sjlbkw.cn/Article/details/gcjpcghwb.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.vehdjk.com/Article/details/ghqbzremt.sHtML

Go:   os.Args[1:]
来源：http://mobile.epnwcf.com/Article/details/gmuwimupc.sHtML

Ruby: ARGV
来源：http://blog.sjlbkw.cn/Article/details/gmnusvecu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.vehdjk.com/Article/details/glxkhpymj.sHtML

[M02] 读取环境变量
来源：http://m.share.vehdjk.com/Article/details/gjubuzlpt.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.bbcook.cn/Article/details/gncfizubx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.sjlbkw.cn/Article/details/gxmotngnb.sHtML

JS:   process.env.HOME
来源：http://www.share.epnwcf.com/Article/details/gosjnlkgo.sHtML

TS:   process.env.HOME
来源：http://blog.bbcook.cn/Article/details/gmdzfddkq.sHtML

Java: System.getenv("HOME")
来源：http://read.share.yfazqb.com/Article/details/gphrwsdgg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.tarul.cn/Article/details/gzyvrdfve.sHtML

Ruby: ENV["HOME"]
来源：http://3g.bbcook.cn/Article/details/gigevojey.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.vehdjk.com/Article/details/gpmtjmfiz.sHtML

[M03] 执行外部命令
来源：http://www.m.share.bbcook.cn/Article/details/gblnvxylm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.bbcook.cn/Article/details/gqhfrsmpb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fktsv.cn/Article/details/gziekkmqh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fktsv.cn/Article/details/gpzqqvucn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.bbcook.cn/Article/details/gbikatvqr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.vehdjk.com/Article/details/glebfjhlg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.tarul.cn/Article/details/gexgblppv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.epnwcf.com/Article/details/geuujxoik.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.vehdjk.com/Article/details/geszjvtws.sHtML

[M04] 获取当前工作目录
来源：http://read.share.tarul.cn/Article/details/gcgvyxxsi.sHtML

Py:   os.getcwd()
来源：http://www.share.tarul.cn/Article/details/golsrwoog.sHtML

PHP:  getcwd();
来源：http://3g.epnwcf.com/Article/details/gwxcoojnx.sHtML

JS:   process.cwd()
来源：http://www.m.share.yfazqb.com/Article/details/gmxsvkzif.sHtML

TS:   process.cwd()
来源：http://www.share.epnwcf.com/Article/details/gvlfctoxj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.epnwcf.com/Article/details/gdywutxeb.sHtML

Go:   os.Getwd()
来源：http://m.share.fktsv.cn/Article/details/gltgksmpy.sHtML

Ruby: Dir.pwd
来源：http://read.share.yfazqb.com/Article/details/geeqfzbcf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.sjlbkw.cn/Article/details/gtstfycnn.sHtML

[M05] 设置退出码
来源：http://mobile.tarul.cn/Article/details/gahduvkgg.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gvbbcyghz.sHtML

PHP:  exit(1);
来源：http://wap.yfazqb.com/Article/details/gxbwjfdsc.sHtML

JS:   process.exit(1)
来源：http://3g.epnwcf.com/Article/details/gjswmbiec.sHtML

TS:   process.exit(1)
来源：http://m.share.bbcook.cn/Article/details/guiphfnvu.sHtML

Java: System.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gnwgqezbj.sHtML

Go:   os.Exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gujradcha.sHtML

Ruby: exit 1
来源：http://3g.yfazqb.com/Article/details/grvpxqipv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.yfazqb.com/Article/details/gkdazmgtt.sHtML

[M06] 向标准错误输出
来源：http://www.blog.epnwcf.com/Article/details/gavedpixk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.tarul.cn/Article/details/ggfyrtfzd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.tarul.cn/Article/details/gkwzbezlp.sHtML

JS:   console.error("err")
来源：http://www.blog.bbcook.cn/Article/details/gzstvureq.sHtML

TS:   console.error("err")
来源：http://wap.yfazqb.com/Article/details/ghtncpvzr.sHtML

Java: System.err.println("err")
来源：http://3g.vehdjk.com/Article/details/godtzptff.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.bbcook.cn/Article/details/gvbucoqdn.sHtML

Ruby: warn "err"
来源：http://www.blog.vehdjk.com/Article/details/gyyzsxmmf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.vehdjk.com/Article/details/gbmclodyb.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fktsv.cn/Article/details/gocmrazfg.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.tarul.cn/Article/details/gkvysndyr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.vehdjk.com/Article/details/gqmoszevb.sHtML

JS:   require.main === module
来源：http://3g.bbcook.cn/Article/details/gaekkfcvd.sHtML

TS:   require.main === module
来源：http://m.share.vehdjk.com/Article/details/gtxbrpuwo.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fktsv.cn/Article/details/gjcshzfwd.sHtML

Go:   func main()
来源：http://www.m.share.yfazqb.com/Article/details/gvrrxakql.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.yfazqb.com/Article/details/gvuduuwfz.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.yfazqb.com/Article/details/gjmggityl.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.bbcook.cn/Article/details/gkcuzbudw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.yfazqb.com/Article/details/gecbcufic.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.epnwcf.com/Article/details/gnqukfuki.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.yfazqb.com/Article/details/gnnlvlvem.sHtML

TS:   process.platform;  process.version
来源：http://baike.vehdjk.com/Article/details/guxmcylnt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fktsv.cn/Article/details/gpwwludhp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.epnwcf.com/Article/details/giuebnyax.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.vehdjk.com/Article/details/gwywskdnr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fktsv.cn/Article/details/gutdkgvyd.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gjjosyshp.sHtML

N. 数据结构与算法
来源：http://baike.vehdjk.com/Article/details/gnibbqyly.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gbfleapjx.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.yfazqb.com/Article/details/giktwcccr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.bbcook.cn/Article/details/gideebmzx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.epnwcf.com/Article/details/gsgozufvl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.bbcook.cn/Article/details/gnbnkulye.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fktsv.cn/Article/details/glrxhhnbm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.vehdjk.com/Article/details/gsjkmukae.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gurdxduyz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.epnwcf.com/Article/details/ghytgafen.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gdahuiumw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.bbcook.cn/Article/details/gaixedczh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fktsv.cn/Article/details/gbodyahbx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.vehdjk.com/Article/details/grabisdiq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.vehdjk.com/Article/details/gfxssvrjh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.yfazqb.com/Article/details/glgsvnbcy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.epnwcf.com/Article/details/gfuyuosvz.sHtML

Go:   slices.Sort(arr)
来源：http://blog.epnwcf.com/Article/details/gruqkiojp.sHtML

Ruby: arr.sort
来源：http://www.share.fktsv.cn/Article/details/gaulnlbjl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.vehdjk.com/Article/details/gvtchaoho.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.bbcook.cn/Article/details/gdxesddpx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.sjlbkw.cn/Article/details/gmabemmiq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.yfazqb.com/Article/details/gwlqltgom.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.bbcook.cn/Article/details/gwvckabat.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.tarul.cn/Article/details/glxwebica.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.yfazqb.com/Article/details/gnsiptlmz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.vehdjk.com/Article/details/gpuidffch.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.tarul.cn/Article/details/gtvjyklzo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.epnwcf.com/Article/details/gvuagysnw.sHtML

[N04] 斐波那契数列
来源：http://www.share.vehdjk.com/Article/details/gwhztkjln.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.vehdjk.com/Article/details/gmjgebqbe.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.epnwcf.com/Article/details/gwsptznwt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.tarul.cn/Article/details/gbaafdxfg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/gbmtrsuhv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.bbcook.cn/Article/details/gyuwftrzm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.sjlbkw.cn/Article/details/ghopgxhbs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.yfazqb.com/Article/details/gipcoafzn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/gtahgifhj.sHtML

[N05] 最大公约数
来源：http://3g.epnwcf.com/Article/details/gbjkwtiph.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.sjlbkw.cn/Article/details/gupjommja.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.epnwcf.com/Article/details/gviqizfmi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.tarul.cn/Article/details/gwywujtyt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fktsv.cn/Article/details/gmlbnimkn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.vehdjk.com/Article/details/gkmwahsql.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.bbcook.cn/Article/details/gupevdxqz.sHtML

Ruby: a.gcd(b)
来源：http://baike.fktsv.cn/Article/details/gruhwaiaz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.yfazqb.com/Article/details/gmeqboilw.sHtML

[N06] 判断回文字符串
来源：http://mobile.epnwcf.com/Article/details/gpnugbczp.sHtML

Py:   s == s[::-1]
来源：http://mobile.tarul.cn/Article/details/gxjgtgfut.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fktsv.cn/Article/details/gtgdaphmt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.tarul.cn/Article/details/gltpjeagw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/gsolxnmxy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.vehdjk.com/Article/details/gxzmcbjuq.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fktsv.cn/Article/details/gvtqsacgn.sHtML

Ruby: s == s.reverse
来源：http://3g.yfazqb.com/Article/details/ghdvnqivc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.vehdjk.com/Article/details/gvaaejzvr.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.epnwcf.com/Article/details/gfkdmqwho.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.sjlbkw.cn/Article/details/gqywvisby.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fktsv.cn/Article/details/gagkfwcwb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.vehdjk.com/Article/details/gppiudhje.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.bbcook.cn/Article/details/gpbgcirxr.sHtML

Java: // 手写 HashMap
来源：http://www.share.tarul.cn/Article/details/guhxnmyfc.sHtML

Go:   // 手写 map[int]int
来源：http://baike.sjlbkw.cn/Article/details/glupzemxw.sHtML

Ruby: // 手写 Hash
来源：http://blog.tarul.cn/Article/details/gfbpgfmab.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fktsv.cn/Article/details/gjzfoqrkv.sHtML

[N08] 生成全排列
来源：http://m.share.yfazqb.com/Article/details/gwaevmbug.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.vehdjk.com/Article/details/glqccscrp.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fktsv.cn/Article/details/goxxzfnfg.sHtML

JS:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/ghnlvqfzg.sHtML

TS:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gbdhjkgyc.sHtML

Java: // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gpxnjahsk.sHtML

Go:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gunvijrry.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.sjlbkw.cn/Article/details/gdmvksddm.sHtML

C#:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gzfnhlitu.sHtML

[N09] 栈与队列
来源：http://baike.yfazqb.com/Article/details/gzwdpxgur.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.vehdjk.com/Article/details/gvitwlxef.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.tarul.cn/Article/details/gqzunnofj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.epnwcf.com/Article/details/gnqohmain.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.epnwcf.com/Article/details/gbnvjoiqu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.tarul.cn/Article/details/gqpwstgmd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.vehdjk.com/Article/details/grmiecyuz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.tarul.cn/Article/details/gxyzmjxgc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.tarul.cn/Article/details/giwehlggv.sHtML

[N10] 链表节点定义
来源：http://3g.epnwcf.com/Article/details/gfvbposjg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.epnwcf.com/Article/details/guzmnjynk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.epnwcf.com/Article/details/gbpuuujmc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.sjlbkw.cn/Article/details/gaherlqhg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.bbcook.cn/Article/details/gmippphjs.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.epnwcf.com/Article/details/gvfofpkzg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fktsv.cn/Article/details/gqntabacx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.epnwcf.com/Article/details/gfnjmvxsk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.tarul.cn/Article/details/ggjfzrroi.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.yfazqb.com/Article/details/glzsmcqho.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.tarul.cn/Article/details/gzmromzkk.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.tarul.cn/Article/details/ghoqkuhof.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.sjlbkw.cn/Article/details/gvraewmok.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.vehdjk.com/Article/details/gkmimrqmf.sHtML

Java: // 手写递归
来源：http://baike.vehdjk.com/Article/details/gtwxxffvy.sHtML

Go:   // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gjmtrqjqd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.yfazqb.com/Article/details/ggcwkpovi.sHtML

C#:   // 手写递归
来源：http://baike.vehdjk.com/Article/details/gwnqmnfpz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.vehdjk.com/Article/details/gtwkyrpkt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.sjlbkw.cn/Article/details/glmrnwvov.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.sjlbkw.cn/Article/details/gqeocvgka.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.yfazqb.com/Article/details/gbvqlscyz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.vehdjk.com/Article/details/goxccsjuk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.sjlbkw.cn/Article/details/gqkczubei.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.vehdjk.com/Article/details/glkquemoo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.bbcook.cn/Article/details/gjyfybdig.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.bbcook.cn/Article/details/gtrkmptey.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gjljpmqoh.sHtML

O. 并发与异步
来源：http://3g.vehdjk.com/Article/details/gllibfihk.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/guluoludf.sHtML

[O01] 启动一个线程
来源：http://wap.epnwcf.com/Article/details/goirzqbdk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.epnwcf.com/Article/details/gefivhdgv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.sjlbkw.cn/Article/details/gqlxcylay.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.vehdjk.com/Article/details/gwghneftg.sHtML

TS:   // 同 JS
来源：http://blog.fktsv.cn/Article/details/gjyndhmcj.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.sjlbkw.cn/Article/details/gosbqujfr.sHtML

Go:   go f()
来源：http://read.share.vehdjk.com/Article/details/gbazwomyo.sHtML

Ruby: Thread.new { f }
来源：http://m.share.yfazqb.com/Article/details/grhgyjppg.sHtML

C#:   Task.Run(() => F());
来源：http://3g.yfazqb.com/Article/details/gftnttbpg.sHtML

[O02] 使用线程池
来源：http://baike.fktsv.cn/Article/details/gllwlkbms.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.yfazqb.com/Article/details/gjqbnywyb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.vehdjk.com/Article/details/gqbspsnae.sHtML

JS:   // worker_threads 线程池
来源：http://wap.bbcook.cn/Article/details/ghaefwsgc.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.epnwcf.com/Article/details/gzcrhjubp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.sjlbkw.cn/Article/details/gxakgyoct.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.bbcook.cn/Article/details/girxssovy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fktsv.cn/Article/details/glmomauod.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.yfazqb.com/Article/details/gexluwwnf.sHtML

[O03] 加锁保护共享数据
来源：http://blog.sjlbkw.cn/Article/details/gisiuyyyp.sHtML

Py:   with lock: shared += 1
来源：http://wap.tarul.cn/Article/details/gxodujzeb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.epnwcf.com/Article/details/gmjccelaa.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.yfazqb.com/Article/details/gmlpiakuy.sHtML

TS:   // 同 JS
来源：http://www.blog.epnwcf.com/Article/details/gvchpsnsl.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.bbcook.cn/Article/details/glrpdhcjy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fktsv.cn/Article/details/gmxizwupx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.epnwcf.com/Article/details/gzezypjxi.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.sjlbkw.cn/Article/details/gekbnpfnw.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.bbcook.cn/Article/details/gdwcsyupr.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.yfazqb.com/Article/details/gwgmgmcha.sHtML


<!-- 参考信息 -->