代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.tarul.cn/Article/details/gtsrapfmm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.tarul.cn/Article/details/gsiizlwcg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.yfazqb.com/Article/details/guiewvhbv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.yfazqb.com/Article/details/gwlarswgk.sHtML

[K06] 解析 URL 查询串
来源：http://blog.bbcook.cn/Article/details/gogxeaojb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fktsv.cn/Article/details/gppdeovsf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.bbcook.cn/Article/details/gjkyjvlmf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fktsv.cn/Article/details/gfkgbnndv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.yfazqb.com/Article/details/gmmmilfnh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fktsv.cn/Article/details/gahigdemm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.sjlbkw.cn/Article/details/gtyuhfpmp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.yfazqb.com/Article/details/gjphwvvdu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/gwfjztnwk.sHtML

[K07] 进制转换
来源：http://wap.vehdjk.com/Article/details/gcyfxincp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gslvqsuun.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.epnwcf.com/Article/details/ggcvjtqid.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gehodotcp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gpvgycvjd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gfpfsfzsn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpjsqxcgd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.tarul.cn/Article/details/gtrztzfic.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gqqpcwfaz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.sjlbkw.cn/Article/details/gkdiwbkdp.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.tarul.cn/Article/details/gphxkfuqw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.sjlbkw.cn/Article/details/gjztdjhgx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.yfazqb.com/Article/details/gqfbkffew.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.bbcook.cn/Article/details/gyzdtwbep.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.bbcook.cn/Article/details/glmlcmcpj.sHtML

Go:   encoding/gob
来源：http://blog.yfazqb.com/Article/details/gudyeebcm.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fktsv.cn/Article/details/gukeehivb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.epnwcf.com/Article/details/gzfhojecb.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gaplycnzd.sHtML

L. 网络请求
来源：http://www.blog.bbcook.cn/Article/details/gguiqxsyb.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gpgiuogax.sHtML

[L01] 发送 GET 请求
来源：http://3g.tarul.cn/Article/details/gmipamwzq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.vehdjk.com/Article/details/gsidmmjrg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.yfazqb.com/Article/details/gfnscrqhd.sHtML

JS:   await fetch(url)
来源：http://mobile.yfazqb.com/Article/details/gsnohhihz.sHtML

TS:   await fetch(url)
来源：http://m.share.bbcook.cn/Article/details/ggdedcgwj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.yfazqb.com/Article/details/gmvrteuga.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.tarul.cn/Article/details/gaugnavsb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.bbcook.cn/Article/details/gwgphgiut.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fktsv.cn/Article/details/gywcelorv.sHtML

[L02] 发送 POST JSON
来源：http://read.share.bbcook.cn/Article/details/gmkwuziyn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.bbcook.cn/Article/details/ghspwsbjn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.bbcook.cn/Article/details/galvtlscn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.bbcook.cn/Article/details/gsdstwdyl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.sjlbkw.cn/Article/details/gcirtexve.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fktsv.cn/Article/details/geyelstev.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.vehdjk.com/Article/details/gougnfbwd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.vehdjk.com/Article/details/gcctoxapk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.vehdjk.com/Article/details/gvpsmszrx.sHtML

[L03] 设置自定义请求头
来源：http://www.share.sjlbkw.cn/Article/details/gqkmxzfsc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.epnwcf.com/Article/details/gaczzdnpk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fktsv.cn/Article/details/gjpvagsqw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.epnwcf.com/Article/details/ggwdtjpwy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.epnwcf.com/Article/details/gpcxqgwle.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.tarul.cn/Article/details/gsfcibhxr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.tarul.cn/Article/details/gwghyvuos.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fktsv.cn/Article/details/ghefzykft.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fktsv.cn/Article/details/gwqkcubqu.sHtML

[L04] 设置超时
来源：http://mobile.vehdjk.com/Article/details/gcgxzremw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.epnwcf.com/Article/details/gaoxgiktw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.tarul.cn/Article/details/gsxcrmxzj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.epnwcf.com/Article/details/guhqvlvqk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.tarul.cn/Article/details/gdbhevvzo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.sjlbkw.cn/Article/details/gkizsvtsy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.epnwcf.com/Article/details/giodgdruy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.vehdjk.com/Article/details/gnzfvwxbu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.vehdjk.com/Article/details/gfplvidyv.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.bbcook.cn/Article/details/gibdicrye.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.vehdjk.com/Article/details/gspxjlkum.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.tarul.cn/Article/details/gfoncknbg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.bbcook.cn/Article/details/gbhlxtaon.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.yfazqb.com/Article/details/gomvgxzza.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.epnwcf.com/Article/details/gfiaxnlww.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.epnwcf.com/Article/details/gicbrhqim.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fktsv.cn/Article/details/gnwumkowl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.vehdjk.com/Article/details/gpryxcpji.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.vehdjk.com/Article/details/gztisrouo.sHtML

Py:   resp.json()
来源：http://mobile.yfazqb.com/Article/details/gdbkreyoc.sHtML

PHP:  json_decode($body, true);
来源：http://baike.sjlbkw.cn/Article/details/grcpxgdfy.sHtML

JS:   await resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/gjoeuynne.sHtML

TS:   await resp.json()
来源：http://baike.bbcook.cn/Article/details/gkpfvfqyt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.vehdjk.com/Article/details/gntpbcvae.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fktsv.cn/Article/details/gsgssohnp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.bbcook.cn/Article/details/gooqvyxok.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.yfazqb.com/Article/details/glmxnewdb.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.yfazqb.com/Article/details/gpvjuerqv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.vehdjk.com/Article/details/gtdppbllp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.yfazqb.com/Article/details/gzspexabj.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fktsv.cn/Article/details/gdxanvgvg.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.bbcook.cn/Article/details/gucypkeqr.sHtML

Java: resp.statusCode()
来源：http://blog.fktsv.cn/Article/details/gejxgktnv.sHtML

Go:   resp.StatusCode
来源：http://m.share.vehdjk.com/Article/details/ghxaamote.sHtML

Ruby: resp.code.to_i
来源：http://read.share.yfazqb.com/Article/details/gjfogwxzq.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.bbcook.cn/Article/details/gkilflvlr.sHtML

[L08] 并发请求多个地址
来源：http://m.share.tarul.cn/Article/details/gdwcyryrx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.epnwcf.com/Article/details/guulvftwq.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.yfazqb.com/Article/details/gekxcfkst.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gicicrouj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.epnwcf.com/Article/details/gbpmaspsh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.tarul.cn/Article/details/gktgpszeh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fktsv.cn/Article/details/gglrsgkml.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.yfazqb.com/Article/details/guyqchtfk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fktsv.cn/Article/details/gduzhkhgp.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gewoshxyc.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fktsv.cn/Article/details/gbdpwzvuf.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/grropxpta.sHtML

[M01] 读取命令行参数
来源：http://read.share.yfazqb.com/Article/details/gtplwhqyf.sHtML

Py:   sys.argv[1:]
来源：http://www.share.yfazqb.com/Article/details/ghgvronbx.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fktsv.cn/Article/details/gsvupdozk.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.sjlbkw.cn/Article/details/gmbzzusdp.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.yfazqb.com/Article/details/gkhiqjcmp.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.vehdjk.com/Article/details/gwjwckfpb.sHtML

Go:   os.Args[1:]
来源：http://read.share.fktsv.cn/Article/details/gaqblyevs.sHtML

Ruby: ARGV
来源：http://www.share.vehdjk.com/Article/details/gfuwxuzpl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.bbcook.cn/Article/details/glfvwuwxc.sHtML

[M02] 读取环境变量
来源：http://baike.vehdjk.com/Article/details/ggphxwyhx.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gfxjwttoi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.epnwcf.com/Article/details/gxovrehdr.sHtML

JS:   process.env.HOME
来源：http://3g.yfazqb.com/Article/details/gjfigyczs.sHtML

TS:   process.env.HOME
来源：http://3g.tarul.cn/Article/details/giwspmkzf.sHtML

Java: System.getenv("HOME")
来源：http://blog.yfazqb.com/Article/details/gmbzyjlpm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.bbcook.cn/Article/details/gslgaosvx.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.epnwcf.com/Article/details/gmuscjwtv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.yfazqb.com/Article/details/gikglviif.sHtML

[M03] 执行外部命令
来源：http://www.share.yfazqb.com/Article/details/gltddyzkv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.yfazqb.com/Article/details/gosrceoif.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fktsv.cn/Article/details/gcyhjlhzd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.vehdjk.com/Article/details/gdiqikoaf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.sjlbkw.cn/Article/details/gawildrhp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.yfazqb.com/Article/details/gouwazhhq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.yfazqb.com/Article/details/griqekxel.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.vehdjk.com/Article/details/gtzfjjfsb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.sjlbkw.cn/Article/details/gvccgayvf.sHtML

[M04] 获取当前工作目录
来源：http://blog.tarul.cn/Article/details/gifmqhksd.sHtML

Py:   os.getcwd()
来源：http://m.share.yfazqb.com/Article/details/gcrfxylgn.sHtML

PHP:  getcwd();
来源：http://baike.sjlbkw.cn/Article/details/gbsuzwjmt.sHtML

JS:   process.cwd()
来源：http://www.blog.yfazqb.com/Article/details/gkzrnvrxq.sHtML

TS:   process.cwd()
来源：http://read.share.sjlbkw.cn/Article/details/gvivjpwfc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.epnwcf.com/Article/details/gqfsnykyz.sHtML

Go:   os.Getwd()
来源：http://www.share.epnwcf.com/Article/details/ghltqnhko.sHtML

Ruby: Dir.pwd
来源：http://wap.yfazqb.com/Article/details/glyeikmnc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.yfazqb.com/Article/details/gbyvrlkil.sHtML

[M05] 设置退出码
来源：http://www.share.tarul.cn/Article/details/gsxcjyaov.sHtML

Py:   sys.exit(1)
来源：http://blog.vehdjk.com/Article/details/gsgawwrjn.sHtML

PHP:  exit(1);
来源：http://baike.epnwcf.com/Article/details/gdqdeoban.sHtML

JS:   process.exit(1)
来源：http://www.share.tarul.cn/Article/details/gmwstaldh.sHtML

TS:   process.exit(1)
来源：http://m.share.tarul.cn/Article/details/giqdkhsho.sHtML

Java: System.exit(1)
来源：http://read.share.vehdjk.com/Article/details/geqsuwdjl.sHtML

Go:   os.Exit(1)
来源：http://wap.tarul.cn/Article/details/grxczwqmx.sHtML

Ruby: exit 1
来源：http://mobile.bbcook.cn/Article/details/gjpjqemub.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.yfazqb.com/Article/details/gavukykav.sHtML

[M06] 向标准错误输出
来源：http://www.blog.bbcook.cn/Article/details/gcwswccam.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.tarul.cn/Article/details/geirmodvs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.vehdjk.com/Article/details/gbpfjxprd.sHtML

JS:   console.error("err")
来源：http://www.share.sjlbkw.cn/Article/details/gfnsxkgbl.sHtML

TS:   console.error("err")
来源：http://wap.epnwcf.com/Article/details/gmticddzl.sHtML

Java: System.err.println("err")
来源：http://mobile.epnwcf.com/Article/details/gutozokjs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.yfazqb.com/Article/details/gymneiamh.sHtML

Ruby: warn "err"
来源：http://mobile.bbcook.cn/Article/details/ganarwavf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.bbcook.cn/Article/details/gigjiqvlh.sHtML

[M07] 判断是否为主入口
来源：http://mobile.tarul.cn/Article/details/ghnhmcwbm.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.vehdjk.com/Article/details/gxnjudyjo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.epnwcf.com/Article/details/gclkkdcgv.sHtML

JS:   require.main === module
来源：http://www.m.share.bbcook.cn/Article/details/gmmemzswp.sHtML

TS:   require.main === module
来源：http://3g.epnwcf.com/Article/details/gkqqwjqto.sHtML

Java: public static void main(String[] args)
来源：http://3g.epnwcf.com/Article/details/gfiyimhuh.sHtML

Go:   func main()
来源：http://www.blog.bbcook.cn/Article/details/gzrhoafgo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.bbcook.cn/Article/details/glkduvaex.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.yfazqb.com/Article/details/giwnauath.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.tarul.cn/Article/details/glvxlrfzm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfghrltx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fktsv.cn/Article/details/gglfykacv.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.sjlbkw.cn/Article/details/gbzvsfsqb.sHtML

TS:   process.platform;  process.version
来源：http://m.share.bbcook.cn/Article/details/gqjlcfqgs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.bbcook.cn/Article/details/gixmsndni.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.yfazqb.com/Article/details/gkasdyyrd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.vehdjk.com/Article/details/gifysmisi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.tarul.cn/Article/details/gqqperxxa.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gnafsbmwd.sHtML

N. 数据结构与算法
来源：http://mobile.bbcook.cn/Article/details/geuyhywhm.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gxtlalmpl.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.epnwcf.com/Article/details/gyfgcxonb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.bbcook.cn/Article/details/glcefrxcn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.vehdjk.com/Article/details/gchepxary.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.epnwcf.com/Article/details/giuqvuyfg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fktsv.cn/Article/details/gduzuwlvh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gbnaiwlfn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxzrzinzw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.yfazqb.com/Article/details/gltezdywh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.bbcook.cn/Article/details/gvfgzziyu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.epnwcf.com/Article/details/gxufcjqwt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.bbcook.cn/Article/details/gunofyajn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fktsv.cn/Article/details/gqlopmymp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fktsv.cn/Article/details/ggmydbnzq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.vehdjk.com/Article/details/gkfmdcwvl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.bbcook.cn/Article/details/guupqwrxi.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.tarul.cn/Article/details/gckwimzmj.sHtML

Ruby: arr.sort
来源：http://3g.yfazqb.com/Article/details/gnkqgewcq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.yfazqb.com/Article/details/gguoythmy.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.epnwcf.com/Article/details/gduxxcmhs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.tarul.cn/Article/details/glbxmfvzv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.sjlbkw.cn/Article/details/gboeaesgl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.vehdjk.com/Article/details/gpcepclzz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.epnwcf.com/Article/details/gufwjbkku.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.tarul.cn/Article/details/gzuppxsrs.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.yfazqb.com/Article/details/gsoyddrcb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.tarul.cn/Article/details/gwxwapkkt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fktsv.cn/Article/details/gezjahzrv.sHtML

[N04] 斐波那契数列
来源：http://www.blog.yfazqb.com/Article/details/gawtjtovg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fktsv.cn/Article/details/gpgpcksvu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.vehdjk.com/Article/details/gisvqdgxn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/gwmdvsdal.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.yfazqb.com/Article/details/ghuxltqjb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.epnwcf.com/Article/details/gviaeyfvf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.vehdjk.com/Article/details/gzrcdagcg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.sjlbkw.cn/Article/details/ghrygicha.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/gikluqfpz.sHtML

[N05] 最大公约数
来源：http://3g.sjlbkw.cn/Article/details/gdxsnrjvv.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.sjlbkw.cn/Article/details/gxksmqpjy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.vehdjk.com/Article/details/glnxzfrtm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.vehdjk.com/Article/details/gdzhvpapf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.tarul.cn/Article/details/gnrhhuvne.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.sjlbkw.cn/Article/details/grsaqnblj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.tarul.cn/Article/details/gmwgnsxwh.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkiggugpb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.sjlbkw.cn/Article/details/gchuaulwm.sHtML

[N06] 判断回文字符串
来源：http://www.share.epnwcf.com/Article/details/gfozpzeyb.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.epnwcf.com/Article/details/grnebekuw.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fktsv.cn/Article/details/gumryzxmj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/gazwmpqxt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/guqeawoms.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fktsv.cn/Article/details/gbtdhocxq.sHtML

Go:   // 双指针从两端比较
来源：http://baike.bbcook.cn/Article/details/gopkzekdf.sHtML

Ruby: s == s.reverse
来源：http://www.share.epnwcf.com/Article/details/gfcsvnbfi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.tarul.cn/Article/details/gsdcwgcxg.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.tarul.cn/Article/details/geteanebl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.tarul.cn/Article/details/gethemihh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.sjlbkw.cn/Article/details/gjrqwgfzp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fktsv.cn/Article/details/gtlgvbymj.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.vehdjk.com/Article/details/gnmosoyvo.sHtML

Java: // 手写 HashMap
来源：http://wap.sjlbkw.cn/Article/details/gxblmafjo.sHtML

Go:   // 手写 map[int]int
来源：http://blog.sjlbkw.cn/Article/details/gapfuwqsm.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fktsv.cn/Article/details/golocbqkf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.vehdjk.com/Article/details/gfoqjhrlj.sHtML

[N08] 生成全排列
来源：http://www.blog.vehdjk.com/Article/details/gkzkpcuxk.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.bbcook.cn/Article/details/gwzdyxxxu.sHtML

PHP:  // 手写递归交换
来源：http://wap.epnwcf.com/Article/details/gdnsgacff.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gmhayibio.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gzxvamyyi.sHtML

Java: // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gdwnryuhf.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/geulcvrtw.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.sjlbkw.cn/Article/details/giehwmsjz.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gwmbqccli.sHtML

[N09] 栈与队列
来源：http://m.share.vehdjk.com/Article/details/gvfhdrlhh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fktsv.cn/Article/details/gcjjmyirg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fktsv.cn/Article/details/gpyqurpnx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fktsv.cn/Article/details/gurkkbkzr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.epnwcf.com/Article/details/grkqbddfa.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.tarul.cn/Article/details/gycjwledv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.epnwcf.com/Article/details/gkpwslbbs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/grkxyltmf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.vehdjk.com/Article/details/gxafpkqzy.sHtML

[N10] 链表节点定义
来源：http://www.blog.bbcook.cn/Article/details/gwatuevcy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.epnwcf.com/Article/details/gkspqnkxh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.yfazqb.com/Article/details/gttwcpyeg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.epnwcf.com/Article/details/gbjzetmqr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.vehdjk.com/Article/details/gkcrkpiob.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.epnwcf.com/Article/details/gwhryjlwh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.bbcook.cn/Article/details/gfsorsrhq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.vehdjk.com/Article/details/gypqampcd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.bbcook.cn/Article/details/gznmzbebk.sHtML

[N11] 二叉树中序遍历
来源：http://3g.bbcook.cn/Article/details/gyzoresxq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.vehdjk.com/Article/details/gufkewbgj.sHtML

PHP:  // 手写递归函数
来源：http://m.share.yfazqb.com/Article/details/gzmnkbptc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.vehdjk.com/Article/details/gygpybahe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.tarul.cn/Article/details/gooijayob.sHtML

Java: // 手写递归
来源：http://m.share.epnwcf.com/Article/details/gubfmthlm.sHtML

Go:   // 手写递归
来源：http://blog.vehdjk.com/Article/details/gvotbbatu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.bbcook.cn/Article/details/ggskyvpzp.sHtML

C#:   // 手写递归
来源：http://baike.tarul.cn/Article/details/gyxzbbngu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.bbcook.cn/Article/details/gsniraqzu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fktsv.cn/Article/details/ggpazggpi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fktsv.cn/Article/details/gagmffrvp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.epnwcf.com/Article/details/gmcdlmrdq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.bbcook.cn/Article/details/gizaqtrxs.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.sjlbkw.cn/Article/details/gojtmakrl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fktsv.cn/Article/details/ghygznozt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.bbcook.cn/Article/details/gjxroudrr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fktsv.cn/Article/details/gcqmgorde.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gcokzqjdz.sHtML

O. 并发与异步
来源：http://m.share.vehdjk.com/Article/details/ggxclxmhy.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gxtxqevqn.sHtML

[O01] 启动一个线程
来源：http://www.m.share.epnwcf.com/Article/details/gtrwrxdsh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.vehdjk.com/Article/details/gqbshkkti.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.yfazqb.com/Article/details/gelhiqjup.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.yfazqb.com/Article/details/geknzovtw.sHtML

TS:   // 同 JS
来源：http://3g.epnwcf.com/Article/details/gktkqcfnx.sHtML


<!-- 参考信息 -->