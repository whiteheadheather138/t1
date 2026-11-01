代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.sjlbkw.cn/Article/details/gbzgcbwgg.sHtML

[K07] 进制转换
来源：http://blog.yfazqb.com/Article/details/gcuiwlykl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gkkolxske.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.yfazqb.com/Article/details/gugwatikl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.tarul.cn/Article/details/gqcqugjld.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.tarul.cn/Article/details/gredekrip.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gulbzdoqs.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.vehdjk.com/Article/details/gyjuwontd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.epnwcf.com/Article/details/gakywcmhr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gmepczzfy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.vehdjk.com/Article/details/gwkomnxrg.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.tarul.cn/Article/details/geeezijku.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.vehdjk.com/Article/details/gcmchthjl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.sjlbkw.cn/Article/details/glzfezmof.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.epnwcf.com/Article/details/gzrtpelri.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.bbcook.cn/Article/details/granjtbmv.sHtML

Go:   encoding/gob
来源：http://www.blog.bbcook.cn/Article/details/glmcltksc.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.epnwcf.com/Article/details/gxtqgpico.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fktsv.cn/Article/details/ghwhzdcyc.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/glppsakhg.sHtML

L. 网络请求
来源：http://m.share.bbcook.cn/Article/details/gnpamfhky.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/ghngwmdgl.sHtML

[L01] 发送 GET 请求
来源：http://read.share.tarul.cn/Article/details/gilovebvz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.vehdjk.com/Article/details/gkyclavyh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.bbcook.cn/Article/details/gdxvjjmmi.sHtML

JS:   await fetch(url)
来源：http://www.share.sjlbkw.cn/Article/details/gabrntllz.sHtML

TS:   await fetch(url)
来源：http://mobile.sjlbkw.cn/Article/details/gofnmepwl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.epnwcf.com/Article/details/gnhguzxbw.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fktsv.cn/Article/details/gigdkycuk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.sjlbkw.cn/Article/details/glnobayjf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.epnwcf.com/Article/details/gndszmxkh.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.vehdjk.com/Article/details/girextycq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.vehdjk.com/Article/details/gtkpbxdar.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.yfazqb.com/Article/details/gaqrukxhh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.sjlbkw.cn/Article/details/gkjfuwrmm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fktsv.cn/Article/details/gojstqmim.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.yfazqb.com/Article/details/goceummqv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.epnwcf.com/Article/details/glzhdnycb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.epnwcf.com/Article/details/godihesrq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.yfazqb.com/Article/details/gickwxbyu.sHtML

[L03] 设置自定义请求头
来源：http://blog.fktsv.cn/Article/details/gjyhkovom.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.epnwcf.com/Article/details/grmgmemqg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.sjlbkw.cn/Article/details/ghbcnhtvi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.tarul.cn/Article/details/gcjfqbycy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.bbcook.cn/Article/details/gqofvgcij.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.tarul.cn/Article/details/gzqyeryck.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.bbcook.cn/Article/details/ggariezcl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.epnwcf.com/Article/details/gztyiwhqa.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fktsv.cn/Article/details/gclkvpnvm.sHtML

[L04] 设置超时
来源：http://m.share.vehdjk.com/Article/details/glhqmdegj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.epnwcf.com/Article/details/gattqzmjl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.sjlbkw.cn/Article/details/gdkslijnm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.vehdjk.com/Article/details/ggobgwdzb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.tarul.cn/Article/details/gdftcpiyg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.yfazqb.com/Article/details/gixykcoxp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fktsv.cn/Article/details/ghpldmtka.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.yfazqb.com/Article/details/goxoeeard.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.yfazqb.com/Article/details/gqilncjfv.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fktsv.cn/Article/details/gbwacsznd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.yfazqb.com/Article/details/gbextqvpo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fktsv.cn/Article/details/gvndqsjcc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.tarul.cn/Article/details/grhoqxbal.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.bbcook.cn/Article/details/gpozqcuhh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.bbcook.cn/Article/details/gihwprfiq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.tarul.cn/Article/details/gpcehxqnm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.epnwcf.com/Article/details/guifigjow.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gjlnckesa.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.epnwcf.com/Article/details/gzpqmoelx.sHtML

Py:   resp.json()
来源：http://www.blog.sjlbkw.cn/Article/details/gabidpokd.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.sjlbkw.cn/Article/details/gcqbhlujh.sHtML

JS:   await resp.json()
来源：http://baike.bbcook.cn/Article/details/gpvmwqxea.sHtML

TS:   await resp.json()
来源：http://3g.vehdjk.com/Article/details/gnwckqhqe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fktsv.cn/Article/details/gczelyzrb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.yfazqb.com/Article/details/gkmapmdnq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.sjlbkw.cn/Article/details/gunphgirp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.bbcook.cn/Article/details/gbagaxwam.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.vehdjk.com/Article/details/gelwfptca.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.tarul.cn/Article/details/gmahftbzf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.vehdjk.com/Article/details/ggkzxfjlc.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.tarul.cn/Article/details/geuelmpvb.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.tarul.cn/Article/details/gukbknwwk.sHtML

Java: resp.statusCode()
来源：http://wap.sjlbkw.cn/Article/details/gtsldlaio.sHtML

Go:   resp.StatusCode
来源：http://read.share.tarul.cn/Article/details/gpctrpfck.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.tarul.cn/Article/details/gaxxhkado.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.epnwcf.com/Article/details/gpdfgmylp.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fktsv.cn/Article/details/godwlwmqb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbkuypme.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.yfazqb.com/Article/details/gaqixnasg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/gnslypenz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.bbcook.cn/Article/details/gziwnftbc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.epnwcf.com/Article/details/ggkvfxind.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fktsv.cn/Article/details/gmqikjjdl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.yfazqb.com/Article/details/gbudxlior.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.tarul.cn/Article/details/gijzqzcuu.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gtrrvtscq.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.yfazqb.com/Article/details/gibcvmddj.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/goshaupmj.sHtML

[M01] 读取命令行参数
来源：http://m.share.fktsv.cn/Article/details/gvixozblh.sHtML

Py:   sys.argv[1:]
来源：http://baike.epnwcf.com/Article/details/goxalljzq.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.yfazqb.com/Article/details/gphcfqami.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.sjlbkw.cn/Article/details/gnewpapzs.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.yfazqb.com/Article/details/gvqfgdkes.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.epnwcf.com/Article/details/gfwwplonl.sHtML

Go:   os.Args[1:]
来源：http://www.share.yfazqb.com/Article/details/gmrjczmvq.sHtML

Ruby: ARGV
来源：http://www.blog.fktsv.cn/Article/details/gxoxlmpkz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.sjlbkw.cn/Article/details/gvtfntpqr.sHtML

[M02] 读取环境变量
来源：http://3g.fktsv.cn/Article/details/gbbgnkshh.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.yfazqb.com/Article/details/glojzjxpd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.bbcook.cn/Article/details/gsoguyvsm.sHtML

JS:   process.env.HOME
来源：http://baike.tarul.cn/Article/details/gtbfihhqs.sHtML

TS:   process.env.HOME
来源：http://read.share.fktsv.cn/Article/details/gwqxzlfjt.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/grlcvnkls.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.sjlbkw.cn/Article/details/geqynjvdo.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.epnwcf.com/Article/details/gfrszmqlx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.bbcook.cn/Article/details/gzkpwcqfk.sHtML

[M03] 执行外部命令
来源：http://www.share.sjlbkw.cn/Article/details/gxmqlugje.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.tarul.cn/Article/details/gywoiifjn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.epnwcf.com/Article/details/gdpacaobx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.vehdjk.com/Article/details/gbgdvnoha.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fktsv.cn/Article/details/ggzhrelti.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.yfazqb.com/Article/details/gvjzpwxbb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fktsv.cn/Article/details/gwuwshruu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.sjlbkw.cn/Article/details/gyqdvkydu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fktsv.cn/Article/details/gszjwtcle.sHtML

[M04] 获取当前工作目录
来源：http://www.share.sjlbkw.cn/Article/details/gmdntduad.sHtML

Py:   os.getcwd()
来源：http://3g.epnwcf.com/Article/details/guvrqzwzu.sHtML

PHP:  getcwd();
来源：http://3g.fktsv.cn/Article/details/gtscjwcwi.sHtML

JS:   process.cwd()
来源：http://www.share.sjlbkw.cn/Article/details/gujptaiom.sHtML

TS:   process.cwd()
来源：http://wap.vehdjk.com/Article/details/ghynxlitt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.bbcook.cn/Article/details/gmkbrdxpp.sHtML

Go:   os.Getwd()
来源：http://blog.sjlbkw.cn/Article/details/gcbxsdgje.sHtML

Ruby: Dir.pwd
来源：http://3g.bbcook.cn/Article/details/gjnxiwzbe.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.epnwcf.com/Article/details/gtvvnjqpm.sHtML

[M05] 设置退出码
来源：http://wap.sjlbkw.cn/Article/details/gcfpqtyzt.sHtML

Py:   sys.exit(1)
来源：http://mobile.tarul.cn/Article/details/gynykzmys.sHtML

PHP:  exit(1);
来源：http://3g.tarul.cn/Article/details/gaocdrmxa.sHtML

JS:   process.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gfoyxqobb.sHtML

TS:   process.exit(1)
来源：http://baike.vehdjk.com/Article/details/gcslcdmfj.sHtML

Java: System.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gccxdmtie.sHtML

Go:   os.Exit(1)
来源：http://blog.tarul.cn/Article/details/glujkmlsn.sHtML

Ruby: exit 1
来源：http://mobile.bbcook.cn/Article/details/gluobhpzi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.sjlbkw.cn/Article/details/gzxqykbon.sHtML

[M06] 向标准错误输出
来源：http://www.share.yfazqb.com/Article/details/gemlueaua.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.tarul.cn/Article/details/gpopntrwb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.bbcook.cn/Article/details/gbgzwehcg.sHtML

JS:   console.error("err")
来源：http://www.m.share.tarul.cn/Article/details/gwmoorsos.sHtML

TS:   console.error("err")
来源：http://mobile.fktsv.cn/Article/details/guchqgubj.sHtML

Java: System.err.println("err")
来源：http://m.share.tarul.cn/Article/details/gvsydenfh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fktsv.cn/Article/details/gcjkrrcox.sHtML

Ruby: warn "err"
来源：http://www.share.tarul.cn/Article/details/gpbbvbbgw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.vehdjk.com/Article/details/gcbruqpip.sHtML

[M07] 判断是否为主入口
来源：http://wap.fktsv.cn/Article/details/gcakerjxz.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.vehdjk.com/Article/details/ggpfynias.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.sjlbkw.cn/Article/details/gxxiwwluw.sHtML

JS:   require.main === module
来源：http://www.m.share.tarul.cn/Article/details/gerxmfrai.sHtML

TS:   require.main === module
来源：http://read.share.yfazqb.com/Article/details/grzivqfzs.sHtML

Java: public static void main(String[] args)
来源：http://m.share.bbcook.cn/Article/details/gwlvgfeab.sHtML

Go:   func main()
来源：http://baike.bbcook.cn/Article/details/glaaqfjmb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.tarul.cn/Article/details/ghvokwilt.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.yfazqb.com/Article/details/gtoyqpfeh.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.tarul.cn/Article/details/geiglmhvh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.sjlbkw.cn/Article/details/gqckaotxn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.sjlbkw.cn/Article/details/gqksdrldb.sHtML

JS:   process.platform;  process.version
来源：http://baike.bbcook.cn/Article/details/gsyzenulj.sHtML

TS:   process.platform;  process.version
来源：http://3g.fktsv.cn/Article/details/gsmvblnvs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.yfazqb.com/Article/details/glzpvakfr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.vehdjk.com/Article/details/ggictsjkb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.tarul.cn/Article/details/grdxzkhlh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.tarul.cn/Article/details/gsxofarke.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/ggvszbdjd.sHtML

N. 数据结构与算法
来源：http://3g.tarul.cn/Article/details/grwvzsnoo.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gddjbgqzh.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.vehdjk.com/Article/details/gdfmqoxac.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gofsueyxe.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.yfazqb.com/Article/details/guqezlsnm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.yfazqb.com/Article/details/ghtfdjobi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.tarul.cn/Article/details/gjioixqhe.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.epnwcf.com/Article/details/gxpqqfubb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.tarul.cn/Article/details/gqtkshjrx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.bbcook.cn/Article/details/gqumagror.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.vehdjk.com/Article/details/ggwxprqom.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.vehdjk.com/Article/details/gstjiaqne.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fktsv.cn/Article/details/gxogsgfov.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.yfazqb.com/Article/details/gcwxdvvbe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrjttfqz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/gladjcrtr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.bbcook.cn/Article/details/gerwnfgrq.sHtML

Go:   slices.Sort(arr)
来源：http://3g.sjlbkw.cn/Article/details/gfhmmgzpj.sHtML

Ruby: arr.sort
来源：http://read.share.yfazqb.com/Article/details/gwqmnpppk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.yfazqb.com/Article/details/geufrvwbl.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.vehdjk.com/Article/details/ghyitrusp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.sjlbkw.cn/Article/details/gvrselkfg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.tarul.cn/Article/details/gawozsumc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.yfazqb.com/Article/details/ggvytofte.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.sjlbkw.cn/Article/details/gbgyxaacx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.yfazqb.com/Article/details/guzfyxyyq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.sjlbkw.cn/Article/details/gohcnvocz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.vehdjk.com/Article/details/glkcmqroa.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.bbcook.cn/Article/details/gemokoxlj.sHtML

[N04] 斐波那契数列
来源：http://3g.sjlbkw.cn/Article/details/gvoypxzhl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.tarul.cn/Article/details/gpigyguak.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.vehdjk.com/Article/details/gqoirjszn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/gxcuofdqk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.yfazqb.com/Article/details/gaauvkrvg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.sjlbkw.cn/Article/details/gljrdxlzl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.epnwcf.com/Article/details/gsqaatbzd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.sjlbkw.cn/Article/details/gkcejxayh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdomdkay.sHtML

[N05] 最大公约数
来源：http://www.share.yfazqb.com/Article/details/gvklzurxb.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.bbcook.cn/Article/details/geiidppmz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.tarul.cn/Article/details/gdnmgquud.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.yfazqb.com/Article/details/gnveeiluz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.bbcook.cn/Article/details/gpyjimpiq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.yfazqb.com/Article/details/ghyklorit.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.vehdjk.com/Article/details/gbbkeqgcv.sHtML

Ruby: a.gcd(b)
来源：http://www.share.epnwcf.com/Article/details/gmdufgvyu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.yfazqb.com/Article/details/gdnqudzpf.sHtML

[N06] 判断回文字符串
来源：http://wap.bbcook.cn/Article/details/gwfjrgzns.sHtML

Py:   s == s[::-1]
来源：http://read.share.sjlbkw.cn/Article/details/gvuhcjgnm.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.sjlbkw.cn/Article/details/govriuvmo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/ghlxjoqmr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gxjaqglww.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.sjlbkw.cn/Article/details/gsvjnfxql.sHtML

Go:   // 双指针从两端比较
来源：http://baike.vehdjk.com/Article/details/gxqcmvfrs.sHtML

Ruby: s == s.reverse
来源：http://blog.tarul.cn/Article/details/gwwbsqupe.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.sjlbkw.cn/Article/details/gbchhruuh.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.tarul.cn/Article/details/gjigewafm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.epnwcf.com/Article/details/gtjbofdkw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.epnwcf.com/Article/details/gmkhguthj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.epnwcf.com/Article/details/gdfmiegls.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.bbcook.cn/Article/details/gekegpoov.sHtML

Java: // 手写 HashMap
来源：http://www.blog.epnwcf.com/Article/details/greceamyz.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.vehdjk.com/Article/details/gjhxkpden.sHtML

Ruby: // 手写 Hash
来源：http://m.share.bbcook.cn/Article/details/gaajubkwl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.bbcook.cn/Article/details/ggydratso.sHtML

[N08] 生成全排列
来源：http://www.blog.sjlbkw.cn/Article/details/gjacmaace.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.bbcook.cn/Article/details/gfdmbjjjy.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.sjlbkw.cn/Article/details/gwxdlcjwd.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gikbtndjy.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/grqfkhsjs.sHtML

Java: // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gridjfpqs.sHtML

Go:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gqcngazee.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.tarul.cn/Article/details/glrzeywqc.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gyevscrgc.sHtML

[N09] 栈与队列
来源：http://blog.bbcook.cn/Article/details/gxmyupyod.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fktsv.cn/Article/details/gslpqkekk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/ghtapreox.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gedakousx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.tarul.cn/Article/details/gwnrohcvz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.bbcook.cn/Article/details/gfudfweuz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.vehdjk.com/Article/details/gajbqhkzv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.vehdjk.com/Article/details/gztpxtvrs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.yfazqb.com/Article/details/goufvlbfb.sHtML

[N10] 链表节点定义
来源：http://blog.sjlbkw.cn/Article/details/gusutfdzr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fktsv.cn/Article/details/gwzjgvxxx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.tarul.cn/Article/details/gtnwlduaa.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fktsv.cn/Article/details/gzqeenglo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.epnwcf.com/Article/details/gnrubrisq.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.sjlbkw.cn/Article/details/gaanuoiqy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.sjlbkw.cn/Article/details/geqrzjibl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.bbcook.cn/Article/details/ghhesgbwb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fktsv.cn/Article/details/guppimavo.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.tarul.cn/Article/details/glniszeal.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.bbcook.cn/Article/details/gaavutfoz.sHtML

PHP:  // 手写递归函数
来源：http://m.share.vehdjk.com/Article/details/gjjhyycpp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.vehdjk.com/Article/details/gwxwrhsow.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.sjlbkw.cn/Article/details/geqlnyzyl.sHtML

Java: // 手写递归
来源：http://www.share.epnwcf.com/Article/details/gysqwzdjc.sHtML

Go:   // 手写递归
来源：http://www.blog.yfazqb.com/Article/details/gciamvnun.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.yfazqb.com/Article/details/grfjdvdfe.sHtML

C#:   // 手写递归
来源：http://wap.tarul.cn/Article/details/gybldusnn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.epnwcf.com/Article/details/gorqzoxji.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.bbcook.cn/Article/details/gefzssrrc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fktsv.cn/Article/details/gvuqlgenl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.yfazqb.com/Article/details/gkkehcpau.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.vehdjk.com/Article/details/ggyavzsgw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.vehdjk.com/Article/details/gsdhtxskx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.tarul.cn/Article/details/gutbpufjq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.vehdjk.com/Article/details/gcpzmaghn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.epnwcf.com/Article/details/gwfocefhs.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gttebuifu.sHtML

O. 并发与异步
来源：http://www.m.share.yfazqb.com/Article/details/gmhtowyoc.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gmfoqvjcn.sHtML

[O01] 启动一个线程
来源：http://mobile.fktsv.cn/Article/details/gsnirzgkz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.yfazqb.com/Article/details/gyxyvbevl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.epnwcf.com/Article/details/gmiwctttc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.yfazqb.com/Article/details/gitxqrjzn.sHtML

TS:   // 同 JS
来源：http://blog.fktsv.cn/Article/details/gjtrineye.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.vehdjk.com/Article/details/gzwsxzutc.sHtML

Go:   go f()
来源：http://www.blog.bbcook.cn/Article/details/grubvjsgm.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.sjlbkw.cn/Article/details/gdpytagjk.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.yfazqb.com/Article/details/gisdumnki.sHtML

[O02] 使用线程池
来源：http://www.blog.fktsv.cn/Article/details/gdmeowyvj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.tarul.cn/Article/details/gbqewyapu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.vehdjk.com/Article/details/gifypjjes.sHtML

JS:   // worker_threads 线程池
来源：http://baike.yfazqb.com/Article/details/gbxhidcxu.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fktsv.cn/Article/details/gqetnobkx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.tarul.cn/Article/details/gpumzjwne.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.vehdjk.com/Article/details/ghgesitgm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.bbcook.cn/Article/details/gmkrwgzhi.sHtML


<!-- 参考信息 -->