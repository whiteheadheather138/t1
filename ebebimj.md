代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.tarul.cn/Article/details/gizldzijr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.yfazqb.com/Article/details/gykrfqwpm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.sjlbkw.cn/Article/details/ghusnkhgr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnpkqoiu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.epnwcf.com/Article/details/gdlvmdoqp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.sjlbkw.cn/Article/details/gcwokyhcl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.vehdjk.com/Article/details/ggtqxfngs.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.bbcook.cn/Article/details/gdoltvyrx.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gnycxmckc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.yfazqb.com/Article/details/gwucihkxn.sHtML

JS:   structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/ggtbdroxr.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fktsv.cn/Article/details/gbfdqlxhj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.tarul.cn/Article/details/gmkkbweve.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.fktsv.cn/Article/details/ghyrkgriv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.tarul.cn/Article/details/gjsbbwhut.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.yfazqb.com/Article/details/gltlbauzc.sHtML

[K06] 解析 URL 查询串
来源：http://wap.tarul.cn/Article/details/gwfcksgsz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.yfazqb.com/Article/details/gzwhsejct.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.epnwcf.com/Article/details/gsitseozk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.vehdjk.com/Article/details/gycsagfaq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.epnwcf.com/Article/details/gvoifypyd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.sjlbkw.cn/Article/details/ghzmfpyzj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/gtlufzeaj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/gkbtkelfl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fktsv.cn/Article/details/gizdbewmn.sHtML

[K07] 进制转换
来源：http://3g.epnwcf.com/Article/details/gqluahpec.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gavxyddup.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.vehdjk.com/Article/details/gqygrubzu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gwjjimfwt.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.bbcook.cn/Article/details/ghkxrprft.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.tarul.cn/Article/details/gioirukeh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.vehdjk.com/Article/details/gufuvbcgl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fktsv.cn/Article/details/gnsrbbxab.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gpnahenkg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fktsv.cn/Article/details/gaqyqobib.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.vehdjk.com/Article/details/gfqywpdtc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.tarul.cn/Article/details/ggvluuunq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.vehdjk.com/Article/details/gffzqdkpr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.sjlbkw.cn/Article/details/gzfyvrign.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.vehdjk.com/Article/details/gdwrjammw.sHtML

Go:   encoding/gob
来源：http://www.m.share.vehdjk.com/Article/details/glkrxuiyn.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gpiuyoaib.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.yfazqb.com/Article/details/gvetqgcdx.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/grpkkoslp.sHtML

L. 网络请求
来源：http://www.blog.vehdjk.com/Article/details/gfjddzhpo.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gywmjdwdv.sHtML

[L01] 发送 GET 请求
来源：http://m.share.epnwcf.com/Article/details/gbhfkwwky.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.sjlbkw.cn/Article/details/gliqfagww.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fktsv.cn/Article/details/gxbggasft.sHtML

JS:   await fetch(url)
来源：http://mobile.sjlbkw.cn/Article/details/ghtdxxjqe.sHtML

TS:   await fetch(url)
来源：http://m.share.epnwcf.com/Article/details/ghjzngnvx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fktsv.cn/Article/details/gdhvwrhfi.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.yfazqb.com/Article/details/gwexvndwd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.yfazqb.com/Article/details/gvnteaugs.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fktsv.cn/Article/details/gdagpklel.sHtML

[L02] 发送 POST JSON
来源：http://3g.epnwcf.com/Article/details/gsnmptniw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.tarul.cn/Article/details/gbrwmyrkz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.epnwcf.com/Article/details/gfnzriikv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.yfazqb.com/Article/details/gqyxepigv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.vehdjk.com/Article/details/gmpqtpehe.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.epnwcf.com/Article/details/gosrlrliq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.vehdjk.com/Article/details/gwkatykpu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.bbcook.cn/Article/details/ghljkzvoq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fktsv.cn/Article/details/gagzeyrch.sHtML

[L03] 设置自定义请求头
来源：http://3g.epnwcf.com/Article/details/gefrqbvxf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.vehdjk.com/Article/details/gmrzfofjw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.epnwcf.com/Article/details/gsjdpupgm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.vehdjk.com/Article/details/grccmrtwx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.vehdjk.com/Article/details/gezmxysnc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.epnwcf.com/Article/details/gqjswbhbg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.tarul.cn/Article/details/gfkyiyvhc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.bbcook.cn/Article/details/gkfhfpuly.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.vehdjk.com/Article/details/guqkzenbk.sHtML

[L04] 设置超时
来源：http://blog.yfazqb.com/Article/details/grjfnijih.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.tarul.cn/Article/details/gbyzudeda.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.epnwcf.com/Article/details/gahasqgvq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.bbcook.cn/Article/details/gqnedyeda.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.epnwcf.com/Article/details/gxqctsfms.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.vehdjk.com/Article/details/gyiycrlrs.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.yfazqb.com/Article/details/ghvqtyziw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.yfazqb.com/Article/details/gyjfqvgrf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.yfazqb.com/Article/details/grllbnwgv.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.epnwcf.com/Article/details/gctsxumie.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fktsv.cn/Article/details/gupypdlcd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.sjlbkw.cn/Article/details/gwalngkou.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.bbcook.cn/Article/details/gmhnukybw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.tarul.cn/Article/details/gmesxxfqu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.bbcook.cn/Article/details/gljozpkrh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.bbcook.cn/Article/details/gcattwfik.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.vehdjk.com/Article/details/gjloooxjf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.tarul.cn/Article/details/guemecjty.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.epnwcf.com/Article/details/gszqaieco.sHtML

Py:   resp.json()
来源：http://www.share.bbcook.cn/Article/details/gaqhskgqi.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.yfazqb.com/Article/details/gdwdtkowo.sHtML

JS:   await resp.json()
来源：http://mobile.fktsv.cn/Article/details/gvubcjrhr.sHtML

TS:   await resp.json()
来源：http://www.share.vehdjk.com/Article/details/gpdgfflve.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.bbcook.cn/Article/details/gdutfmdqn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.vehdjk.com/Article/details/gmcwhhvuk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.tarul.cn/Article/details/gcawihvdu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.tarul.cn/Article/details/gmxexijvr.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.tarul.cn/Article/details/gfdjkztqt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fktsv.cn/Article/details/gkhdlktgm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.vehdjk.com/Article/details/gvmeaszfh.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.sjlbkw.cn/Article/details/gjitavkfr.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.epnwcf.com/Article/details/gaclzfbwe.sHtML

Java: resp.statusCode()
来源：http://www.m.share.vehdjk.com/Article/details/gaxsmtkng.sHtML

Go:   resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/gsjbifxzc.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.vehdjk.com/Article/details/gotlilabg.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.bbcook.cn/Article/details/gbhfvmoyl.sHtML

[L08] 并发请求多个地址
来源：http://m.share.bbcook.cn/Article/details/gavinbkeg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.epnwcf.com/Article/details/glvadakzq.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.bbcook.cn/Article/details/gmlfbgyji.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.tarul.cn/Article/details/gbyiuzysz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.bbcook.cn/Article/details/gjimngxkp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.sjlbkw.cn/Article/details/gerbfdsny.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.sjlbkw.cn/Article/details/gtulbdsrt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.sjlbkw.cn/Article/details/glroozvmm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.vehdjk.com/Article/details/gsoesrudn.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gxfybkjvf.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.sjlbkw.cn/Article/details/gyzdwzttw.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gmdggexne.sHtML

[M01] 读取命令行参数
来源：http://www.blog.vehdjk.com/Article/details/gxgnazsep.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhgqlimg.sHtML

PHP:  $argv;  $argc;
来源：http://wap.epnwcf.com/Article/details/gkiadfwbd.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.tarul.cn/Article/details/gbwrprogg.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.sjlbkw.cn/Article/details/ggxkusfdx.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.yfazqb.com/Article/details/gfbgdbtua.sHtML

Go:   os.Args[1:]
来源：http://3g.tarul.cn/Article/details/gpudbcbrv.sHtML

Ruby: ARGV
来源：http://www.share.bbcook.cn/Article/details/gwxygmrac.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.vehdjk.com/Article/details/glochukac.sHtML

[M02] 读取环境变量
来源：http://wap.fktsv.cn/Article/details/gajgcaiiz.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fktsv.cn/Article/details/gtzeajmik.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.vehdjk.com/Article/details/guxsvfwat.sHtML

JS:   process.env.HOME
来源：http://blog.vehdjk.com/Article/details/gaevgoyew.sHtML

TS:   process.env.HOME
来源：http://blog.yfazqb.com/Article/details/gsbvtbpmg.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fktsv.cn/Article/details/gmupbkqxu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/glurdqpkr.sHtML

Ruby: ENV["HOME"]
来源：http://wap.yfazqb.com/Article/details/gfrkwvvdb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.sjlbkw.cn/Article/details/gckdpnvrx.sHtML

[M03] 执行外部命令
来源：http://www.blog.tarul.cn/Article/details/gclopqfyw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fktsv.cn/Article/details/grtdxjacc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.vehdjk.com/Article/details/gkatojwdx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fktsv.cn/Article/details/gcskytiyg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.epnwcf.com/Article/details/gajbyvega.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.vehdjk.com/Article/details/gzsbwobrg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.bbcook.cn/Article/details/giwxmvzqz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.tarul.cn/Article/details/gbuoqsedo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.yfazqb.com/Article/details/gakbkbizj.sHtML

[M04] 获取当前工作目录
来源：http://read.share.epnwcf.com/Article/details/gycsnmqwy.sHtML

Py:   os.getcwd()
来源：http://blog.epnwcf.com/Article/details/gwxlrxdds.sHtML

PHP:  getcwd();
来源：http://www.m.share.sjlbkw.cn/Article/details/gnwtteocu.sHtML

JS:   process.cwd()
来源：http://mobile.bbcook.cn/Article/details/gyryvjqvy.sHtML

TS:   process.cwd()
来源：http://3g.bbcook.cn/Article/details/giwjcnfmi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.vehdjk.com/Article/details/grsnnlcce.sHtML

Go:   os.Getwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfxtmlwu.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.sjlbkw.cn/Article/details/gegdxbwbu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.bbcook.cn/Article/details/gdzglormo.sHtML

[M05] 设置退出码
来源：http://m.share.bbcook.cn/Article/details/gebgsvjzl.sHtML

Py:   sys.exit(1)
来源：http://baike.epnwcf.com/Article/details/gytiplepn.sHtML

PHP:  exit(1);
来源：http://3g.vehdjk.com/Article/details/guljejiix.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gwwxoqvmi.sHtML

TS:   process.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gfzbkhute.sHtML

Java: System.exit(1)
来源：http://blog.bbcook.cn/Article/details/ggselyixj.sHtML

Go:   os.Exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gdwpflmjy.sHtML

Ruby: exit 1
来源：http://read.share.tarul.cn/Article/details/gjgduyktz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.vehdjk.com/Article/details/gawhfcsxq.sHtML

[M06] 向标准错误输出
来源：http://read.share.bbcook.cn/Article/details/gzmtwfsfl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.epnwcf.com/Article/details/gidmfykin.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.bbcook.cn/Article/details/gebelzuxa.sHtML

JS:   console.error("err")
来源：http://blog.epnwcf.com/Article/details/glasikdfz.sHtML

TS:   console.error("err")
来源：http://mobile.yfazqb.com/Article/details/gjeathxki.sHtML

Java: System.err.println("err")
来源：http://mobile.bbcook.cn/Article/details/gyiqhulqj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.sjlbkw.cn/Article/details/gfnspvpya.sHtML

Ruby: warn "err"
来源：http://blog.epnwcf.com/Article/details/gjdctmfpa.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.sjlbkw.cn/Article/details/gflapsada.sHtML

[M07] 判断是否为主入口
来源：http://blog.sjlbkw.cn/Article/details/gjmqvvjza.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.epnwcf.com/Article/details/gmxrbgemi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.bbcook.cn/Article/details/gtfwqhizx.sHtML

JS:   require.main === module
来源：http://www.blog.tarul.cn/Article/details/gchwffwiw.sHtML

TS:   require.main === module
来源：http://www.share.yfazqb.com/Article/details/gklqwbcmw.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.yfazqb.com/Article/details/gtsbmacqi.sHtML

Go:   func main()
来源：http://www.blog.vehdjk.com/Article/details/gghrdzlpd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.bbcook.cn/Article/details/gxhcpphvh.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.bbcook.cn/Article/details/gxztmhrxe.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.vehdjk.com/Article/details/gbuqqntbg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.tarul.cn/Article/details/gzuveesdd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.tarul.cn/Article/details/gciabanmg.sHtML

JS:   process.platform;  process.version
来源：http://baike.tarul.cn/Article/details/gjkudyzfh.sHtML

TS:   process.platform;  process.version
来源：http://www.share.yfazqb.com/Article/details/gotmmzwsu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fktsv.cn/Article/details/gqeyneiqi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.tarul.cn/Article/details/gzdqsqmav.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fktsv.cn/Article/details/gintppini.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.tarul.cn/Article/details/ghhbasukp.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gbsgybkfu.sHtML

N. 数据结构与算法
来源：http://wap.sjlbkw.cn/Article/details/gnmacomrh.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gtagqaijb.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fktsv.cn/Article/details/gqsiqsgkk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gdxnxlskf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.bbcook.cn/Article/details/gdauogpgd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.yfazqb.com/Article/details/gsranflku.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.bbcook.cn/Article/details/gvayzbiij.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/guwcsmbwd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gubjuqxck.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.bbcook.cn/Article/details/gbgbmngfn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gzajyypwz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.vehdjk.com/Article/details/geqnfviyu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.epnwcf.com/Article/details/gidpjppaf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.vehdjk.com/Article/details/gzzcslanl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/gwuiefbtc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.bbcook.cn/Article/details/gksxkdqsw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.sjlbkw.cn/Article/details/gnlaexfce.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fktsv.cn/Article/details/gnfygpgdg.sHtML

Ruby: arr.sort
来源：http://read.share.yfazqb.com/Article/details/gmmogzuaq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.tarul.cn/Article/details/govytdnwr.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.yfazqb.com/Article/details/gbndhsens.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.sjlbkw.cn/Article/details/grvlpwhcn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.vehdjk.com/Article/details/gquberpow.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.tarul.cn/Article/details/gebhhjlel.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.yfazqb.com/Article/details/gvlmnmkvd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.epnwcf.com/Article/details/grioxxvcd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.tarul.cn/Article/details/gjlhvwdkq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fktsv.cn/Article/details/gekgkqmxg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.vehdjk.com/Article/details/grpdpxmii.sHtML

[N04] 斐波那契数列
来源：http://mobile.fktsv.cn/Article/details/gurpnbjrz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.vehdjk.com/Article/details/gsiptnyop.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.yfazqb.com/Article/details/gcaqxusac.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.bbcook.cn/Article/details/givpgmtfc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/gpmgaqeyj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fktsv.cn/Article/details/gzbnuqdvg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.bbcook.cn/Article/details/gbdklusod.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.sjlbkw.cn/Article/details/gdcpwximk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/gtrfdcadf.sHtML

[N05] 最大公约数
来源：http://read.share.yfazqb.com/Article/details/geixoofdd.sHtML

Py:   math.gcd(a, b)
来源：http://baike.bbcook.cn/Article/details/gzpfanftj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.tarul.cn/Article/details/ghbfkdhjo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.vehdjk.com/Article/details/gvgrbhezi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fktsv.cn/Article/details/gfwymgzby.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.sjlbkw.cn/Article/details/gskgathxf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.epnwcf.com/Article/details/gjjaecqbs.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fktsv.cn/Article/details/ghvkafnsv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.tarul.cn/Article/details/gcscpqear.sHtML

[N06] 判断回文字符串
来源：http://read.share.yfazqb.com/Article/details/gqkwejoqj.sHtML

Py:   s == s[::-1]
来源：http://www.share.fktsv.cn/Article/details/gjdtjnois.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmznpjxrb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gymxicfsx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gketwcodw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.vehdjk.com/Article/details/gsoiguamh.sHtML

Go:   // 双指针从两端比较
来源：http://3g.sjlbkw.cn/Article/details/ggxthvemq.sHtML

Ruby: s == s.reverse
来源：http://3g.epnwcf.com/Article/details/gtybumjbv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.vehdjk.com/Article/details/grpqknpsa.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.tarul.cn/Article/details/gpayhzktt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.epnwcf.com/Article/details/gssqfpopj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.bbcook.cn/Article/details/gooevjqao.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.bbcook.cn/Article/details/gijumzzoc.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.vehdjk.com/Article/details/gqnadpgtw.sHtML

Java: // 手写 HashMap
来源：http://read.share.tarul.cn/Article/details/gzuqxxien.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fktsv.cn/Article/details/gzpxuqyzy.sHtML

Ruby: // 手写 Hash
来源：http://3g.sjlbkw.cn/Article/details/govdeicpu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.vehdjk.com/Article/details/gboxfyzlo.sHtML

[N08] 生成全排列
来源：http://www.share.tarul.cn/Article/details/gusqmqybn.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fktsv.cn/Article/details/gknrmdtwv.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.vehdjk.com/Article/details/gpvswzlrr.sHtML

JS:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gtdanlxrp.sHtML

TS:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gzowvlgyr.sHtML

Java: // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gcatvhwiy.sHtML

Go:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gxabfzlcw.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.vehdjk.com/Article/details/gjdcvwlmm.sHtML

C#:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gxwuqylwa.sHtML

[N09] 栈与队列
来源：http://baike.yfazqb.com/Article/details/gcvxcqmpo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gzoiyxxvz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gmolkxhov.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fktsv.cn/Article/details/gvxchiiwg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.bbcook.cn/Article/details/gnhejmoly.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.vehdjk.com/Article/details/goslwpjgc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fktsv.cn/Article/details/gvqlugjao.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.tarul.cn/Article/details/gsugsrdqa.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.tarul.cn/Article/details/glwhizccu.sHtML

[N10] 链表节点定义
来源：http://baike.vehdjk.com/Article/details/goklgcxwp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.vehdjk.com/Article/details/ggyfbfqzo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.yfazqb.com/Article/details/gtigvomnd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.vehdjk.com/Article/details/grmxdubod.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.bbcook.cn/Article/details/gqkxnfgoj.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.vehdjk.com/Article/details/gxhurdxuo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.yfazqb.com/Article/details/gntvdjvyr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.yfazqb.com/Article/details/guhnqrzku.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.yfazqb.com/Article/details/ggrggnzxp.sHtML

[N11] 二叉树中序遍历
来源：http://wap.tarul.cn/Article/details/ghasrksft.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fktsv.cn/Article/details/gbnehqtjb.sHtML

PHP:  // 手写递归函数
来源：http://read.share.sjlbkw.cn/Article/details/gobjqmpzi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fktsv.cn/Article/details/gdljyudpg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.vehdjk.com/Article/details/gwcqambax.sHtML

Java: // 手写递归
来源：http://blog.fktsv.cn/Article/details/grbnnltqz.sHtML

Go:   // 手写递归
来源：http://www.share.fktsv.cn/Article/details/gjtpfuwvg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.tarul.cn/Article/details/gaoljxpqy.sHtML

C#:   // 手写递归
来源：http://read.share.epnwcf.com/Article/details/gcdwztapi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.tarul.cn/Article/details/gpzcnrmwb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.bbcook.cn/Article/details/getgufgwt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.tarul.cn/Article/details/gwsxxboeq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.epnwcf.com/Article/details/gvxzvztvz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.yfazqb.com/Article/details/gaqteyxpb.sHtML


<!-- 参考信息 -->