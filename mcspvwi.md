代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://www.blog.epnwcf.com/Article/details/gtbujsgfk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.bbcook.cn/Article/details/gngknyzlz.sHtML

JS:   structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/gwetdwgau.sHtML

TS:   structuredClone(obj)
来源：http://baike.bbcook.cn/Article/details/gdwjadvwu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.yfazqb.com/Article/details/gynokrdwx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.yfazqb.com/Article/details/grzdaywku.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.epnwcf.com/Article/details/grxdcuubt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.epnwcf.com/Article/details/gfzrgspla.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.epnwcf.com/Article/details/ghpmrqmfq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.yfazqb.com/Article/details/gsqprpucw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.sjlbkw.cn/Article/details/gwlsgbowy.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.epnwcf.com/Article/details/gsjyfhdjn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.vehdjk.com/Article/details/gzubqyrlt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.bbcook.cn/Article/details/gzxwndcpm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/grcwlywqd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/gdxqwewzj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.vehdjk.com/Article/details/gzccgolbn.sHtML

[K07] 进制转换
来源：http://baike.sjlbkw.cn/Article/details/germvvyfn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gixlyvlva.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.bbcook.cn/Article/details/gtnsqvgqc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gtrwzfobf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gmoawikjm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gxbgshopd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.sjlbkw.cn/Article/details/guiuifiay.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.yfazqb.com/Article/details/gofqusmyj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.tarul.cn/Article/details/gvrluuald.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.sjlbkw.cn/Article/details/gnraazuom.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.bbcook.cn/Article/details/gtyjtplzm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fktsv.cn/Article/details/gomdcgyin.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.epnwcf.com/Article/details/ggjbmdtxc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.tarul.cn/Article/details/gmtihpzgk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.epnwcf.com/Article/details/giihjhdec.sHtML

Go:   encoding/gob
来源：http://www.m.share.vehdjk.com/Article/details/gucvqwhhn.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gvafggpby.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.sjlbkw.cn/Article/details/gmkqgdfca.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gqnryyrdr.sHtML

L. 网络请求
来源：http://3g.tarul.cn/Article/details/glgdikzno.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gsrugxhcj.sHtML

[L01] 发送 GET 请求
来源：http://read.share.bbcook.cn/Article/details/grzixttyl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fktsv.cn/Article/details/gvrdiyshq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.epnwcf.com/Article/details/gqycvwjfh.sHtML

JS:   await fetch(url)
来源：http://www.m.share.yfazqb.com/Article/details/geuxybihb.sHtML

TS:   await fetch(url)
来源：http://m.share.fktsv.cn/Article/details/gvzqptxpb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.sjlbkw.cn/Article/details/gbfocjgzc.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.epnwcf.com/Article/details/gykwejjzl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.tarul.cn/Article/details/gffuzzqer.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fktsv.cn/Article/details/gbndqsrwq.sHtML

[L02] 发送 POST JSON
来源：http://read.share.sjlbkw.cn/Article/details/gkhoycvvh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fktsv.cn/Article/details/gawiixiqi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.epnwcf.com/Article/details/gwopigtcg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.tarul.cn/Article/details/ghbuhklum.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.sjlbkw.cn/Article/details/gepgrjobt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fktsv.cn/Article/details/gqkfuiepp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.tarul.cn/Article/details/gqgujnxzc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.sjlbkw.cn/Article/details/gcbjonlie.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.tarul.cn/Article/details/gcrdzjfrw.sHtML

[L03] 设置自定义请求头
来源：http://wap.fktsv.cn/Article/details/gmranmquk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.sjlbkw.cn/Article/details/gjipmpmmg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.vehdjk.com/Article/details/gssxuctsf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.vehdjk.com/Article/details/ghjsqimfo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.yfazqb.com/Article/details/glnvnouzo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.bbcook.cn/Article/details/gmwthpino.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fktsv.cn/Article/details/glqclbfaf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.vehdjk.com/Article/details/gahuhqcke.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.vehdjk.com/Article/details/gsbpdiijp.sHtML

[L04] 设置超时
来源：http://wap.yfazqb.com/Article/details/gdjdbdaks.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.tarul.cn/Article/details/ggppyweuy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.yfazqb.com/Article/details/gceohpepg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.vehdjk.com/Article/details/gqdljuaji.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnuxaphr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.tarul.cn/Article/details/gksosqwau.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fktsv.cn/Article/details/gvkyipyzr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.bbcook.cn/Article/details/gedjkbklo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.tarul.cn/Article/details/ghewlylnx.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.sjlbkw.cn/Article/details/gzkjjvfpo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fktsv.cn/Article/details/ghzqkmpqf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fktsv.cn/Article/details/gmeyvyaox.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.tarul.cn/Article/details/gjktahwfq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fktsv.cn/Article/details/gbhdgpucp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.yfazqb.com/Article/details/gexuplxjw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.vehdjk.com/Article/details/gibesmwjs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.yfazqb.com/Article/details/gwuzdwzzv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gldcqtrsu.sHtML

[L06] 解析响应为 JSON
来源：http://blog.epnwcf.com/Article/details/ghvwpffkc.sHtML

Py:   resp.json()
来源：http://blog.epnwcf.com/Article/details/gjaxzygtr.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.yfazqb.com/Article/details/gugznhgpe.sHtML

JS:   await resp.json()
来源：http://mobile.tarul.cn/Article/details/gkvskzdgg.sHtML

TS:   await resp.json()
来源：http://baike.fktsv.cn/Article/details/ghhexkhmj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.tarul.cn/Article/details/grhfcjqoz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.tarul.cn/Article/details/gkfgjciad.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.sjlbkw.cn/Article/details/gjsdajuhc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.epnwcf.com/Article/details/gsvfddyry.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fktsv.cn/Article/details/gpzcwvbdp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fktsv.cn/Article/details/gedjdljmr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.vehdjk.com/Article/details/gvptujtnk.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fktsv.cn/Article/details/giybtqwmf.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fktsv.cn/Article/details/gqsavyyxb.sHtML

Java: resp.statusCode()
来源：http://baike.epnwcf.com/Article/details/gdejupgqa.sHtML

Go:   resp.StatusCode
来源：http://3g.epnwcf.com/Article/details/gvjrnkmfg.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.yfazqb.com/Article/details/ggmpixuwg.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.bbcook.cn/Article/details/grndgveyh.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fktsv.cn/Article/details/gfiwalniu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.bbcook.cn/Article/details/gyhitjxqu.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.tarul.cn/Article/details/getnwswsw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gxzkankye.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.tarul.cn/Article/details/gqikczzlt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.tarul.cn/Article/details/gabxhqopy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.vehdjk.com/Article/details/givvoitrz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.yfazqb.com/Article/details/gugznkyno.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.bbcook.cn/Article/details/gvpopozqz.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gcgszrccy.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.vehdjk.com/Article/details/gaukiergs.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gotdxpecv.sHtML

[M01] 读取命令行参数
来源：http://wap.yfazqb.com/Article/details/ggvzmsgth.sHtML

Py:   sys.argv[1:]
来源：http://blog.vehdjk.com/Article/details/gqoadjuid.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.tarul.cn/Article/details/grgrarxsl.sHtML

JS:   process.argv.slice(2)
来源：http://wap.yfazqb.com/Article/details/gaopkybkh.sHtML

TS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/gdxxxssea.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.bbcook.cn/Article/details/gniykriup.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.bbcook.cn/Article/details/gsmnwhpsw.sHtML

Ruby: ARGV
来源：http://www.m.share.sjlbkw.cn/Article/details/gfxssmkdv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.sjlbkw.cn/Article/details/gkbjhqaha.sHtML

[M02] 读取环境变量
来源：http://m.share.sjlbkw.cn/Article/details/gnqlhztcs.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.tarul.cn/Article/details/grgbtfcmt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.epnwcf.com/Article/details/gzjkgkfoj.sHtML

JS:   process.env.HOME
来源：http://read.share.epnwcf.com/Article/details/gljnfqglk.sHtML

TS:   process.env.HOME
来源：http://blog.bbcook.cn/Article/details/groiwukok.sHtML

Java: System.getenv("HOME")
来源：http://baike.bbcook.cn/Article/details/gydubzvna.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.tarul.cn/Article/details/gigwfdkij.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.epnwcf.com/Article/details/ggrzyuqth.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.yfazqb.com/Article/details/ggtgpcnfw.sHtML

[M03] 执行外部命令
来源：http://wap.tarul.cn/Article/details/gqzrwkjgu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.bbcook.cn/Article/details/gohdnkhya.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.epnwcf.com/Article/details/gujcsdcxq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.bbcook.cn/Article/details/gqevhukvh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fktsv.cn/Article/details/gorblybzl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.bbcook.cn/Article/details/gyhypnoug.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fktsv.cn/Article/details/gpejzmuos.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.tarul.cn/Article/details/gsscnqkvn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.sjlbkw.cn/Article/details/gzrfsinnu.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.yfazqb.com/Article/details/gscpwtrsr.sHtML

Py:   os.getcwd()
来源：http://www.m.share.yfazqb.com/Article/details/gzwzmtqqd.sHtML

PHP:  getcwd();
来源：http://m.share.bbcook.cn/Article/details/gvlhhrvlw.sHtML

JS:   process.cwd()
来源：http://blog.fktsv.cn/Article/details/glfbtakcr.sHtML

TS:   process.cwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/goskgfyww.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.tarul.cn/Article/details/gtnkcoruf.sHtML

Go:   os.Getwd()
来源：http://3g.epnwcf.com/Article/details/girirdxad.sHtML

Ruby: Dir.pwd
来源：http://www.blog.epnwcf.com/Article/details/ggtppceox.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.sjlbkw.cn/Article/details/gwraermmu.sHtML

[M05] 设置退出码
来源：http://mobile.fktsv.cn/Article/details/gkogmbiiy.sHtML

Py:   sys.exit(1)
来源：http://baike.yfazqb.com/Article/details/ghbzalxmn.sHtML

PHP:  exit(1);
来源：http://blog.fktsv.cn/Article/details/giftqrivm.sHtML

JS:   process.exit(1)
来源：http://baike.bbcook.cn/Article/details/gbhygcehe.sHtML

TS:   process.exit(1)
来源：http://baike.vehdjk.com/Article/details/ghnkydfql.sHtML

Java: System.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/giurxdcqa.sHtML

Go:   os.Exit(1)
来源：http://read.share.tarul.cn/Article/details/gqmautywb.sHtML

Ruby: exit 1
来源：http://mobile.bbcook.cn/Article/details/gddkoswwg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.epnwcf.com/Article/details/gdwhqnmmx.sHtML

[M06] 向标准错误输出
来源：http://wap.vehdjk.com/Article/details/glntfggvm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.bbcook.cn/Article/details/gmzhqnhaa.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.vehdjk.com/Article/details/gcmanokqt.sHtML

JS:   console.error("err")
来源：http://3g.vehdjk.com/Article/details/gvxvvmlec.sHtML

TS:   console.error("err")
来源：http://www.share.tarul.cn/Article/details/gnuxmxfek.sHtML

Java: System.err.println("err")
来源：http://read.share.sjlbkw.cn/Article/details/glzkhirqt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fktsv.cn/Article/details/gzkdapove.sHtML

Ruby: warn "err"
来源：http://wap.sjlbkw.cn/Article/details/gyvzaetlo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.bbcook.cn/Article/details/gygpktilo.sHtML

[M07] 判断是否为主入口
来源：http://wap.epnwcf.com/Article/details/gyncwaxln.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.tarul.cn/Article/details/gkfytusbd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.bbcook.cn/Article/details/gefrnndsc.sHtML

JS:   require.main === module
来源：http://www.m.share.fktsv.cn/Article/details/gbqvywerj.sHtML

TS:   require.main === module
来源：http://mobile.epnwcf.com/Article/details/gkvhhokvm.sHtML

Java: public static void main(String[] args)
来源：http://wap.fktsv.cn/Article/details/gtrgqryst.sHtML

Go:   func main()
来源：http://wap.bbcook.cn/Article/details/gymvzmleo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.yfazqb.com/Article/details/gtixzrrge.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.vehdjk.com/Article/details/gqzxqqkij.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.yfazqb.com/Article/details/guwnpesvj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fktsv.cn/Article/details/gvrlvjyjh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.bbcook.cn/Article/details/gbkdgxtjh.sHtML

JS:   process.platform;  process.version
来源：http://wap.vehdjk.com/Article/details/ghvkekvrj.sHtML

TS:   process.platform;  process.version
来源：http://m.share.sjlbkw.cn/Article/details/gutgdobkt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.yfazqb.com/Article/details/gphfdoftm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.tarul.cn/Article/details/gedbuyjje.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.bbcook.cn/Article/details/gutwmyhhe.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.bbcook.cn/Article/details/gqpovnrkg.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gfvppiibe.sHtML

N. 数据结构与算法
来源：http://3g.sjlbkw.cn/Article/details/gmsnrgayk.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/givblxqbg.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.bbcook.cn/Article/details/gvspntiok.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.epnwcf.com/Article/details/gqjkdkxfz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.yfazqb.com/Article/details/gzduwghhz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.tarul.cn/Article/details/gycuzvqaq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.tarul.cn/Article/details/gqbngbsly.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gjrjmtisl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gokphdbdp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.yfazqb.com/Article/details/gvnpaolgd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gplumrzpl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.sjlbkw.cn/Article/details/gcyvnrdsa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.epnwcf.com/Article/details/gbhhnyqom.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.bbcook.cn/Article/details/ghrgffnjf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.sjlbkw.cn/Article/details/gjwqtswah.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fktsv.cn/Article/details/gzmwjgtxo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.epnwcf.com/Article/details/gmrxdythj.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gmdzgtpho.sHtML

Ruby: arr.sort
来源：http://www.m.share.epnwcf.com/Article/details/gfqafnyds.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.bbcook.cn/Article/details/giftmlkoq.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fktsv.cn/Article/details/gzvhiyhsu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.yfazqb.com/Article/details/glvbaxjlb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.tarul.cn/Article/details/gibjadsrw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.yfazqb.com/Article/details/gdbnnpdwm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.vehdjk.com/Article/details/gxivcsehd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.yfazqb.com/Article/details/gszadpzei.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.sjlbkw.cn/Article/details/gkqwaiyoz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.epnwcf.com/Article/details/gsxumlriw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.bbcook.cn/Article/details/gwxjvdvur.sHtML

[N04] 斐波那契数列
来源：http://blog.fktsv.cn/Article/details/gabrmhqtn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.epnwcf.com/Article/details/gsuotakum.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.vehdjk.com/Article/details/gikpdbdde.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.vehdjk.com/Article/details/gnpebkgbf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/gnimfabrk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fktsv.cn/Article/details/guvhsskwm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.yfazqb.com/Article/details/gsiuvalji.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.bbcook.cn/Article/details/gznyqudeg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gdjxuwagj.sHtML

[N05] 最大公约数
来源：http://wap.epnwcf.com/Article/details/gsnebsonx.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.vehdjk.com/Article/details/gnjqmopqv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.vehdjk.com/Article/details/gjnwsqics.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.sjlbkw.cn/Article/details/gfdsdxbyz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.epnwcf.com/Article/details/gljgnzuku.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.vehdjk.com/Article/details/gponwjqbv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fktsv.cn/Article/details/gskfkzziz.sHtML

Ruby: a.gcd(b)
来源：http://mobile.tarul.cn/Article/details/gffubndtz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.bbcook.cn/Article/details/gankahaei.sHtML

[N06] 判断回文字符串
来源：http://www.blog.vehdjk.com/Article/details/gaapkiydm.sHtML

Py:   s == s[::-1]
来源：http://baike.sjlbkw.cn/Article/details/gsegyzsyz.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.vehdjk.com/Article/details/gnaliatoo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gciiydwnd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gkkfyreso.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.yfazqb.com/Article/details/gpofcqbzj.sHtML

Go:   // 双指针从两端比较
来源：http://baike.sjlbkw.cn/Article/details/guesledma.sHtML

Ruby: s == s.reverse
来源：http://read.share.vehdjk.com/Article/details/gowohheyh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.epnwcf.com/Article/details/gfzhlmxmq.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.sjlbkw.cn/Article/details/gbfjpncnv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.tarul.cn/Article/details/gxccvmvhv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.vehdjk.com/Article/details/gmoigzfab.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.bbcook.cn/Article/details/gqvousllb.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.epnwcf.com/Article/details/gkoifatfi.sHtML

Java: // 手写 HashMap
来源：http://www.share.epnwcf.com/Article/details/gfrxjvfme.sHtML

Go:   // 手写 map[int]int
来源：http://3g.bbcook.cn/Article/details/gqlllpjso.sHtML

Ruby: // 手写 Hash
来源：http://m.share.sjlbkw.cn/Article/details/ggfqipool.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.tarul.cn/Article/details/gvrvhfyfy.sHtML

[N08] 生成全排列
来源：http://www.m.share.epnwcf.com/Article/details/glurdcrof.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.vehdjk.com/Article/details/gktpvgejw.sHtML

PHP:  // 手写递归交换
来源：http://www.share.tarul.cn/Article/details/grboswrjg.sHtML

JS:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gathavfmx.sHtML

TS:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gftpchgsx.sHtML

Java: // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gambkpqhl.sHtML

Go:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gcllubjhy.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fktsv.cn/Article/details/gdwitzpnw.sHtML

C#:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/ghnohzrrb.sHtML

[N09] 栈与队列
来源：http://mobile.fktsv.cn/Article/details/gzudksxqh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.yfazqb.com/Article/details/goinpmeyu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.epnwcf.com/Article/details/gymrxjfle.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.bbcook.cn/Article/details/gerwytvrw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhcflkez.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.epnwcf.com/Article/details/gbhnhwbtn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.bbcook.cn/Article/details/ggmkjnojq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.epnwcf.com/Article/details/gyaduijti.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.epnwcf.com/Article/details/gyaphtyrt.sHtML

[N10] 链表节点定义
来源：http://wap.bbcook.cn/Article/details/gzwzyazfj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.epnwcf.com/Article/details/gtcxahnut.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.yfazqb.com/Article/details/gfgyttudr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.vehdjk.com/Article/details/gitnzflio.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.epnwcf.com/Article/details/ggavadeqj.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.yfazqb.com/Article/details/glqbxbafz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fktsv.cn/Article/details/gvqvutuzc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fktsv.cn/Article/details/gikoyrflx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.epnwcf.com/Article/details/gfqzucncf.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.tarul.cn/Article/details/gpzrnyfke.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.yfazqb.com/Article/details/gxxmokaed.sHtML

PHP:  // 手写递归函数
来源：http://baike.fktsv.cn/Article/details/gauyiaycl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.tarul.cn/Article/details/gfnykepwr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.vehdjk.com/Article/details/gzhihrwyi.sHtML

Java: // 手写递归
来源：http://m.share.tarul.cn/Article/details/gseqptccj.sHtML

Go:   // 手写递归
来源：http://mobile.vehdjk.com/Article/details/ghqyvznvx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.vehdjk.com/Article/details/grfxcxzhr.sHtML

C#:   // 手写递归
来源：http://www.m.share.bbcook.cn/Article/details/ggkhyoumk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.yfazqb.com/Article/details/gdhgzsuzt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fktsv.cn/Article/details/glxniddyr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.sjlbkw.cn/Article/details/gykcqvswe.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.bbcook.cn/Article/details/guprbspom.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.bbcook.cn/Article/details/gamgzodya.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.epnwcf.com/Article/details/gybsaymys.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.yfazqb.com/Article/details/gixgrrpun.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.epnwcf.com/Article/details/gmgqzophh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gasesfycn.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gkyxhzbyz.sHtML

O. 并发与异步
来源：http://3g.fktsv.cn/Article/details/gbcrtvuis.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gupfsveol.sHtML

[O01] 启动一个线程
来源：http://wap.yfazqb.com/Article/details/gqoaxulhq.sHtML


<!-- 参考信息 -->