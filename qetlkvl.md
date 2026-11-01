代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://www.blog.tarul.cn/Article/details/gglwhicig.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.bbcook.cn/Article/details/gmxvklgqy.sHtML

JS:   structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/gdyowmiky.sHtML

TS:   structuredClone(obj)
来源：http://m.share.epnwcf.com/Article/details/grgqopqmj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.bbcook.cn/Article/details/gvhpiaqeh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.tarul.cn/Article/details/gwkvnuswr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fktsv.cn/Article/details/gxtvuylxc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.vehdjk.com/Article/details/gphrvgqjj.sHtML

[K06] 解析 URL 查询串
来源：http://3g.epnwcf.com/Article/details/gygorxmvl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.sjlbkw.cn/Article/details/ggysihkre.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.vehdjk.com/Article/details/gpyqslzdk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.bbcook.cn/Article/details/gbbixslso.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fktsv.cn/Article/details/gkcpkzmls.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.vehdjk.com/Article/details/gxmounxsa.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/gyzvsogei.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.vehdjk.com/Article/details/ghzbtfbeu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/ggbtmdsdi.sHtML

[K07] 进制转换
来源：http://m.share.yfazqb.com/Article/details/gizpamfzy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtnzmxee.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fktsv.cn/Article/details/gzlyqpvdq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gkoylowvx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gtqwtekxs.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.tarul.cn/Article/details/gflctewwf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.tarul.cn/Article/details/gqdnqrtdb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.tarul.cn/Article/details/gqoccxvpw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.tarul.cn/Article/details/goyytxrdg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.tarul.cn/Article/details/griykzrgc.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.yfazqb.com/Article/details/gwohgmoak.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.yfazqb.com/Article/details/gswsbxswy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.epnwcf.com/Article/details/gdsdrzdam.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fktsv.cn/Article/details/gsbqqjzmb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.bbcook.cn/Article/details/gntrchtxz.sHtML

Go:   encoding/gob
来源：http://baike.epnwcf.com/Article/details/gycgngrlc.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.bbcook.cn/Article/details/gslvelejp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.yfazqb.com/Article/details/gflnbxxnm.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gqsevcuwn.sHtML

L. 网络请求
来源：http://wap.sjlbkw.cn/Article/details/gfcvzlugp.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gjbwwlhhp.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.epnwcf.com/Article/details/gyhvkczum.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.epnwcf.com/Article/details/glbtwjruu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.tarul.cn/Article/details/grtdkjrso.sHtML

JS:   await fetch(url)
来源：http://www.share.bbcook.cn/Article/details/gszazggka.sHtML

TS:   await fetch(url)
来源：http://3g.sjlbkw.cn/Article/details/gvtzqnotc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.epnwcf.com/Article/details/gkvpepxzv.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.sjlbkw.cn/Article/details/guyacyesv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.yfazqb.com/Article/details/gzupudxrl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.yfazqb.com/Article/details/ggiztusjg.sHtML

[L02] 发送 POST JSON
来源：http://3g.yfazqb.com/Article/details/ghbnvvqio.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.bbcook.cn/Article/details/gidhgnzih.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.sjlbkw.cn/Article/details/gjsvncjve.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.bbcook.cn/Article/details/gziokvvje.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fktsv.cn/Article/details/gnugsagyj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.tarul.cn/Article/details/gozbegiit.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.tarul.cn/Article/details/gownomrrs.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.epnwcf.com/Article/details/gtxksjpqn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.bbcook.cn/Article/details/gwgmtsppq.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fktsv.cn/Article/details/glitxemio.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.sjlbkw.cn/Article/details/gadfsberk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.yfazqb.com/Article/details/gawnsrgob.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.yfazqb.com/Article/details/gsqivjuvd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.tarul.cn/Article/details/gghrkwfxa.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.epnwcf.com/Article/details/glfnlthjt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.vehdjk.com/Article/details/gyuslqgat.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.sjlbkw.cn/Article/details/gwwpzgiko.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.epnwcf.com/Article/details/gdlbhgeei.sHtML

[L04] 设置超时
来源：http://www.blog.yfazqb.com/Article/details/gmyyebovz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.yfazqb.com/Article/details/ghzgdftxb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.epnwcf.com/Article/details/ggttfuqrt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.tarul.cn/Article/details/gqjheovkc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.vehdjk.com/Article/details/gvsgspywh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.bbcook.cn/Article/details/gfsfakrog.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fktsv.cn/Article/details/gqwtobhlv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.epnwcf.com/Article/details/gylulzeku.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.bbcook.cn/Article/details/gjhmnzlsi.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.vehdjk.com/Article/details/gkdslpmqq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.epnwcf.com/Article/details/gjtzwnsgv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fktsv.cn/Article/details/gaescbdak.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.epnwcf.com/Article/details/gjhjuuffb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.sjlbkw.cn/Article/details/gnjsljgbc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fktsv.cn/Article/details/gwsuykgiy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.vehdjk.com/Article/details/gyuekgazq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fktsv.cn/Article/details/gfyzffotx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.yfazqb.com/Article/details/glfcgatgp.sHtML

[L06] 解析响应为 JSON
来源：http://blog.yfazqb.com/Article/details/gwfafczdv.sHtML

Py:   resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/gpyrsaqho.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.vehdjk.com/Article/details/ggmdyxwqt.sHtML

JS:   await resp.json()
来源：http://3g.sjlbkw.cn/Article/details/gztlgbjvu.sHtML

TS:   await resp.json()
来源：http://wap.fktsv.cn/Article/details/ggbhokcsx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.bbcook.cn/Article/details/gmxkdqxtb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.vehdjk.com/Article/details/gplelzsdg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.tarul.cn/Article/details/gqgvyxbry.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.epnwcf.com/Article/details/gjsvwgzsd.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.vehdjk.com/Article/details/gmgonqnrf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.epnwcf.com/Article/details/gzmspjtyh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.sjlbkw.cn/Article/details/gfgujxihu.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.yfazqb.com/Article/details/gpqprqyro.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.yfazqb.com/Article/details/guvnngfrs.sHtML

Java: resp.statusCode()
来源：http://www.blog.sjlbkw.cn/Article/details/geqyymuda.sHtML

Go:   resp.StatusCode
来源：http://blog.epnwcf.com/Article/details/gtaqjekvv.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.yfazqb.com/Article/details/gbntillbi.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.epnwcf.com/Article/details/gmqqyqxgg.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fktsv.cn/Article/details/gaoxtbcqe.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.vehdjk.com/Article/details/giknbyghc.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.tarul.cn/Article/details/gddgemcsk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fktsv.cn/Article/details/gaohgfgoy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.epnwcf.com/Article/details/groczxgdr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.vehdjk.com/Article/details/gguoqbiap.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.epnwcf.com/Article/details/gutufmqwd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.epnwcf.com/Article/details/gwrfimqzy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.vehdjk.com/Article/details/gkpjszraa.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gzkstmntl.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.epnwcf.com/Article/details/gelqhgmar.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gnztvpctm.sHtML

[M01] 读取命令行参数
来源：http://3g.vehdjk.com/Article/details/gdiognnvx.sHtML

Py:   sys.argv[1:]
来源：http://mobile.tarul.cn/Article/details/gmbqyzcsv.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fktsv.cn/Article/details/gtipqoptt.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnsxqveuv.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fktsv.cn/Article/details/goyrxcehz.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.vehdjk.com/Article/details/giyknovjf.sHtML

Go:   os.Args[1:]
来源：http://m.share.sjlbkw.cn/Article/details/gnctmbvfw.sHtML

Ruby: ARGV
来源：http://read.share.bbcook.cn/Article/details/gozephgir.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.tarul.cn/Article/details/glplelcdi.sHtML

[M02] 读取环境变量
来源：http://read.share.sjlbkw.cn/Article/details/gcxhphwgv.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.vehdjk.com/Article/details/giljgzgbp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.yfazqb.com/Article/details/gcpsywwoj.sHtML

JS:   process.env.HOME
来源：http://3g.sjlbkw.cn/Article/details/giywoskne.sHtML

TS:   process.env.HOME
来源：http://www.m.share.tarul.cn/Article/details/gsleypand.sHtML

Java: System.getenv("HOME")
来源：http://wap.tarul.cn/Article/details/gynqmwctk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.epnwcf.com/Article/details/gweswufhk.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.tarul.cn/Article/details/gqikeikfl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.bbcook.cn/Article/details/giandqxdt.sHtML

[M03] 执行外部命令
来源：http://www.share.bbcook.cn/Article/details/ghpnxcjlf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.bbcook.cn/Article/details/gengkfjea.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.epnwcf.com/Article/details/gmxilsvog.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.yfazqb.com/Article/details/grherwtyb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.tarul.cn/Article/details/ggucmaupv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fktsv.cn/Article/details/gczpfvvhw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.vehdjk.com/Article/details/gnblvnqkm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.vehdjk.com/Article/details/gimpdffkk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.vehdjk.com/Article/details/gaiifuoqh.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.tarul.cn/Article/details/ggeihnnrs.sHtML

Py:   os.getcwd()
来源：http://blog.yfazqb.com/Article/details/gyvhikwmk.sHtML

PHP:  getcwd();
来源：http://baike.bbcook.cn/Article/details/gbfnymqda.sHtML

JS:   process.cwd()
来源：http://www.share.yfazqb.com/Article/details/gkcsolabc.sHtML

TS:   process.cwd()
来源：http://www.share.fktsv.cn/Article/details/giorpfage.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.tarul.cn/Article/details/gxjmgggmm.sHtML

Go:   os.Getwd()
来源：http://blog.epnwcf.com/Article/details/gqqkbfmir.sHtML

Ruby: Dir.pwd
来源：http://blog.bbcook.cn/Article/details/gvctxrmox.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fktsv.cn/Article/details/guammoxrk.sHtML

[M05] 设置退出码
来源：http://m.share.fktsv.cn/Article/details/gvzqnullo.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gbhhlhxez.sHtML

PHP:  exit(1);
来源：http://blog.bbcook.cn/Article/details/gckmewdzd.sHtML

JS:   process.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gjidnpafj.sHtML

TS:   process.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gdeamrcdj.sHtML

Java: System.exit(1)
来源：http://www.blog.tarul.cn/Article/details/ghertxbaz.sHtML

Go:   os.Exit(1)
来源：http://wap.vehdjk.com/Article/details/gmnuutwuv.sHtML

Ruby: exit 1
来源：http://3g.tarul.cn/Article/details/gnlmjnipe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.epnwcf.com/Article/details/gczyntmvt.sHtML

[M06] 向标准错误输出
来源：http://read.share.vehdjk.com/Article/details/gmgezzeea.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.tarul.cn/Article/details/gdlxwchul.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.bbcook.cn/Article/details/gtffumukj.sHtML

JS:   console.error("err")
来源：http://www.blog.epnwcf.com/Article/details/gctftbvpa.sHtML

TS:   console.error("err")
来源：http://www.m.share.vehdjk.com/Article/details/gljrppfqg.sHtML

Java: System.err.println("err")
来源：http://blog.bbcook.cn/Article/details/gvemzduxs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.epnwcf.com/Article/details/ggnwzomqf.sHtML

Ruby: warn "err"
来源：http://read.share.tarul.cn/Article/details/gwgvlaplm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.sjlbkw.cn/Article/details/gnevrkjzx.sHtML

[M07] 判断是否为主入口
来源：http://read.share.tarul.cn/Article/details/gvgrgvkpz.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fktsv.cn/Article/details/gzpknrjop.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.sjlbkw.cn/Article/details/gtvzhryqh.sHtML

JS:   require.main === module
来源：http://3g.sjlbkw.cn/Article/details/glcznupar.sHtML

TS:   require.main === module
来源：http://baike.epnwcf.com/Article/details/godlqxolb.sHtML

Java: public static void main(String[] args)
来源：http://baike.tarul.cn/Article/details/gdcviqzds.sHtML

Go:   func main()
来源：http://wap.tarul.cn/Article/details/gznwleqpb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.epnwcf.com/Article/details/gilkzwbdb.sHtML

C#:   static void Main(string[] args)
来源：http://baike.bbcook.cn/Article/details/gujegwnqa.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fktsv.cn/Article/details/glnhytdzl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjoflwvg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.tarul.cn/Article/details/gfpnpzchk.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.epnwcf.com/Article/details/gsihiabft.sHtML

TS:   process.platform;  process.version
来源：http://www.share.epnwcf.com/Article/details/gpicaqbdd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.vehdjk.com/Article/details/gdsfkizut.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.vehdjk.com/Article/details/gowiotnfd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.bbcook.cn/Article/details/gkcfogaif.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.vehdjk.com/Article/details/gqjzbmsoe.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gjnmudtiy.sHtML

N. 数据结构与算法
来源：http://wap.sjlbkw.cn/Article/details/gganbkbjc.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gsagqkcfn.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.epnwcf.com/Article/details/grsqbapqc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.epnwcf.com/Article/details/geyurkfcc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.vehdjk.com/Article/details/gcymuyfic.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.yfazqb.com/Article/details/gjgikvsnu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.yfazqb.com/Article/details/gdlwmuoyn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.epnwcf.com/Article/details/goopnejoa.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gmdarzgir.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fktsv.cn/Article/details/grwcfbpjo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gvjkazgvo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.bbcook.cn/Article/details/gnjiptwes.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.sjlbkw.cn/Article/details/gdnetinpf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.yfazqb.com/Article/details/geqxkwlzv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.vehdjk.com/Article/details/gpykvhohm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.yfazqb.com/Article/details/gvlmzmkar.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.tarul.cn/Article/details/gisnoizwc.sHtML

Go:   slices.Sort(arr)
来源：http://blog.bbcook.cn/Article/details/gyyuhzhiw.sHtML

Ruby: arr.sort
来源：http://mobile.tarul.cn/Article/details/gomrggaws.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fktsv.cn/Article/details/gqriglzts.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.bbcook.cn/Article/details/gnnzsijve.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.epnwcf.com/Article/details/gznxrsoqt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fktsv.cn/Article/details/gpbhrdqtk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.vehdjk.com/Article/details/ggpezekud.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.yfazqb.com/Article/details/gadoqahmm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.vehdjk.com/Article/details/giouzcoig.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.sjlbkw.cn/Article/details/gwlfdgxte.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.vehdjk.com/Article/details/gmqwmousd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvpnoomu.sHtML

[N04] 斐波那契数列
来源：http://m.share.epnwcf.com/Article/details/gzkodusce.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.tarul.cn/Article/details/gxlkhcaln.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.yfazqb.com/Article/details/gwiwalmaj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/gkgtsbxbc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/gzyrexpyx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fktsv.cn/Article/details/grnwkpkgk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.epnwcf.com/Article/details/gkprlookm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.bbcook.cn/Article/details/gomeysjpj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.yfazqb.com/Article/details/gqljyqikk.sHtML

[N05] 最大公约数
来源：http://www.blog.bbcook.cn/Article/details/grogspxma.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.yfazqb.com/Article/details/gzceayhif.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.tarul.cn/Article/details/gjpbxowdy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.epnwcf.com/Article/details/gekojeorg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fktsv.cn/Article/details/giebvgexn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fktsv.cn/Article/details/gdsteaoyo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.yfazqb.com/Article/details/gazpcmlkc.sHtML

Ruby: a.gcd(b)
来源：http://blog.fktsv.cn/Article/details/gvtbyxdhn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.bbcook.cn/Article/details/gvsycrlhe.sHtML

[N06] 判断回文字符串
来源：http://read.share.yfazqb.com/Article/details/gptqctmij.sHtML

Py:   s == s[::-1]
来源：http://blog.sjlbkw.cn/Article/details/gvotufqru.sHtML

PHP:  $s === strrev($s);
来源：http://baike.yfazqb.com/Article/details/gyhbigqnw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/ggmbjwukg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gjplkttwf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnopdntw.sHtML

Go:   // 双指针从两端比较
来源：http://wap.vehdjk.com/Article/details/gtokfixda.sHtML

Ruby: s == s.reverse
来源：http://read.share.bbcook.cn/Article/details/gsdwiqwsz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.epnwcf.com/Article/details/gbwjhmbor.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.sjlbkw.cn/Article/details/gdnxmotoz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.epnwcf.com/Article/details/gxqktcztv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.bbcook.cn/Article/details/gcvqjjvhp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.bbcook.cn/Article/details/gkuwdhgbu.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.yfazqb.com/Article/details/ghgtupuzc.sHtML

Java: // 手写 HashMap
来源：http://3g.bbcook.cn/Article/details/gslzpmxgh.sHtML

Go:   // 手写 map[int]int
来源：http://wap.yfazqb.com/Article/details/goxkgqcio.sHtML

Ruby: // 手写 Hash
来源：http://3g.fktsv.cn/Article/details/ggvomyawt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.tarul.cn/Article/details/gnoqtlhsk.sHtML

[N08] 生成全排列
来源：http://mobile.vehdjk.com/Article/details/gnabgiofz.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gnikluukf.sHtML

PHP:  // 手写递归交换
来源：http://mobile.yfazqb.com/Article/details/gmjeaofgc.sHtML

JS:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gpdvppqzx.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gyxivnacg.sHtML

Java: // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gsaxncbjx.sHtML

Go:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gtliwivon.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.vehdjk.com/Article/details/gbndnpgcd.sHtML

C#:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gkmbcphlj.sHtML

[N09] 栈与队列
来源：http://3g.fktsv.cn/Article/details/gluoucdxo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gqfjeddbg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.tarul.cn/Article/details/gtenfzozc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.vehdjk.com/Article/details/gkfttcmcm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fktsv.cn/Article/details/gcpzpaspi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.vehdjk.com/Article/details/gkmyeiflj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.tarul.cn/Article/details/grtspgirm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.bbcook.cn/Article/details/gzsdcqwmt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.tarul.cn/Article/details/gskinmzmz.sHtML

[N10] 链表节点定义
来源：http://www.blog.epnwcf.com/Article/details/gavcnqiom.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.bbcook.cn/Article/details/gnhsiyblv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.sjlbkw.cn/Article/details/gxsnclpfc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.yfazqb.com/Article/details/gautswvrp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.sjlbkw.cn/Article/details/giqufonfx.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.tarul.cn/Article/details/gudxvgtzn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.sjlbkw.cn/Article/details/gznmdpwgu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.sjlbkw.cn/Article/details/glqhygazl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.tarul.cn/Article/details/gbmcnqdtb.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.tarul.cn/Article/details/gigruehji.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.bbcook.cn/Article/details/ghvkngsdp.sHtML

PHP:  // 手写递归函数
来源：http://baike.tarul.cn/Article/details/gjogwmaqv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.tarul.cn/Article/details/gsihvmlbw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.sjlbkw.cn/Article/details/giyablvwv.sHtML

Java: // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/gvedwtwdo.sHtML

Go:   // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gmbzlavew.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.tarul.cn/Article/details/gfkubrvtm.sHtML

C#:   // 手写递归
来源：http://baike.vehdjk.com/Article/details/geirrtzbj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.yfazqb.com/Article/details/gxdjqbhrw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.tarul.cn/Article/details/grpirkwwz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fktsv.cn/Article/details/goplmdemq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fktsv.cn/Article/details/gckyeltwy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.yfazqb.com/Article/details/gikcpqxlc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gqblmxbra.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fktsv.cn/Article/details/gmptkwggc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.tarul.cn/Article/details/gjwtgohvi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.bbcook.cn/Article/details/gyyxzlmoy.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gftjmrtnr.sHtML

O. 并发与异步
来源：http://blog.vehdjk.com/Article/details/galtfsjik.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gkkptprdp.sHtML

[O01] 启动一个线程
来源：http://m.share.sjlbkw.cn/Article/details/gjtydrjwn.sHtML


<!-- 参考信息 -->