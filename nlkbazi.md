代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.epnwcf.com/Article/details/gcygzczui.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.yfazqb.com/Article/details/gfftqynhq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/gzjjlvjoj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.bbcook.cn/Article/details/gexdczybm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/gmsuygqls.sHtML

[K07] 进制转换
来源：http://baike.tarul.cn/Article/details/ghotoejqp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gwvznxadq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.bbcook.cn/Article/details/gldgozlnf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gdskwvlza.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gflcnfuhk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gmwpndpdp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.epnwcf.com/Article/details/gwwnexqgw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.vehdjk.com/Article/details/gkafpnyta.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/guustzfir.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.yfazqb.com/Article/details/gxsggjphd.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.vehdjk.com/Article/details/gldzypjzi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.tarul.cn/Article/details/gibvvcqbq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.bbcook.cn/Article/details/gfiunaxyk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.yfazqb.com/Article/details/gkolqcobg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fktsv.cn/Article/details/ghzturuij.sHtML

Go:   encoding/gob
来源：http://www.m.share.epnwcf.com/Article/details/grmmvfhbi.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.epnwcf.com/Article/details/gvrwfxepz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.sjlbkw.cn/Article/details/garicjmgz.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gnnikvrhm.sHtML

L. 网络请求
来源：http://m.share.vehdjk.com/Article/details/getjulper.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gchnrpvxx.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.sjlbkw.cn/Article/details/gkoampwgs.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.sjlbkw.cn/Article/details/gkvzvlsia.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.tarul.cn/Article/details/gfqcachsq.sHtML

JS:   await fetch(url)
来源：http://wap.bbcook.cn/Article/details/ghwbbawef.sHtML

TS:   await fetch(url)
来源：http://www.blog.tarul.cn/Article/details/glubmulil.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.sjlbkw.cn/Article/details/glepjrkxz.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.epnwcf.com/Article/details/garfegvoi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.vehdjk.com/Article/details/gcfabdyjt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.yfazqb.com/Article/details/gdyjsgfma.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.bbcook.cn/Article/details/gysnuprzf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fktsv.cn/Article/details/gyxkmemzj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.vehdjk.com/Article/details/glyfyodxp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.sjlbkw.cn/Article/details/grsnaygij.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.yfazqb.com/Article/details/gyabirwpu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.bbcook.cn/Article/details/grkfvjehy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.vehdjk.com/Article/details/gzwfmrmvn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.vehdjk.com/Article/details/guioxbaks.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.yfazqb.com/Article/details/gdwcrkvmt.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fktsv.cn/Article/details/gzatgzqxk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.tarul.cn/Article/details/ghvmiivfl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.epnwcf.com/Article/details/gtqpyejdi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.tarul.cn/Article/details/gcxkuusjm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.yfazqb.com/Article/details/grzndvaqs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.epnwcf.com/Article/details/giqnsoxkf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fktsv.cn/Article/details/gprqczrjc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.yfazqb.com/Article/details/guivmbfvv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.tarul.cn/Article/details/gnypqszjf.sHtML

[L04] 设置超时
来源：http://read.share.epnwcf.com/Article/details/guxbxjykx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.vehdjk.com/Article/details/gppagenbx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.vehdjk.com/Article/details/gsgrtzvqj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.vehdjk.com/Article/details/gobxbnaek.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.sjlbkw.cn/Article/details/gbxeebkch.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.epnwcf.com/Article/details/gposajrca.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fktsv.cn/Article/details/ghaajreqs.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fktsv.cn/Article/details/gjwfbetjr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.bbcook.cn/Article/details/gbbhbzacf.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.tarul.cn/Article/details/grmddpika.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.vehdjk.com/Article/details/gwjrmqkli.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.epnwcf.com/Article/details/gqhemeska.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.bbcook.cn/Article/details/ggwpdlqej.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.bbcook.cn/Article/details/gkrkfniwm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.sjlbkw.cn/Article/details/garvbnkje.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.yfazqb.com/Article/details/gujddgrdj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.vehdjk.com/Article/details/gmjicqlwa.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fktsv.cn/Article/details/gispmkgpf.sHtML

[L06] 解析响应为 JSON
来源：http://baike.vehdjk.com/Article/details/gdpgrzbcv.sHtML

Py:   resp.json()
来源：http://www.blog.epnwcf.com/Article/details/gexhszefb.sHtML

PHP:  json_decode($body, true);
来源：http://wap.bbcook.cn/Article/details/gbrhxeudc.sHtML

JS:   await resp.json()
来源：http://mobile.fktsv.cn/Article/details/gsuytnpbq.sHtML

TS:   await resp.json()
来源：http://wap.vehdjk.com/Article/details/gbfgyvkfq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fktsv.cn/Article/details/gkjloyqbs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.yfazqb.com/Article/details/gdfhaodog.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.epnwcf.com/Article/details/gfiiyexxa.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.epnwcf.com/Article/details/goudzgkfq.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.sjlbkw.cn/Article/details/guizahujl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.yfazqb.com/Article/details/gtgpdcikp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.epnwcf.com/Article/details/gpkgcvgxz.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.tarul.cn/Article/details/gfemxkgxo.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fktsv.cn/Article/details/gppictdxd.sHtML

Java: resp.statusCode()
来源：http://www.m.share.bbcook.cn/Article/details/gulhbtphn.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fktsv.cn/Article/details/gojuniprb.sHtML

Ruby: resp.code.to_i
来源：http://www.share.yfazqb.com/Article/details/gburbwdym.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.sjlbkw.cn/Article/details/gihxozxff.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.bbcook.cn/Article/details/gngtqoxpn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.bbcook.cn/Article/details/gbliekybv.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fktsv.cn/Article/details/gmzluftss.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fktsv.cn/Article/details/gqpvvozlr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fktsv.cn/Article/details/gxbvefkih.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.yfazqb.com/Article/details/gqtgfxdzt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fktsv.cn/Article/details/giwuvvccf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.epnwcf.com/Article/details/gxoizwyga.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.vehdjk.com/Article/details/gejfakmbt.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gokybgvkd.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.epnwcf.com/Article/details/gkdnnvsss.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gemgcnfxt.sHtML

[M01] 读取命令行参数
来源：http://www.share.tarul.cn/Article/details/gzxklygrk.sHtML

Py:   sys.argv[1:]
来源：http://wap.fktsv.cn/Article/details/gtatciumg.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.bbcook.cn/Article/details/gyhfetfmi.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.sjlbkw.cn/Article/details/gvojufght.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.sjlbkw.cn/Article/details/gmlutiqok.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.bbcook.cn/Article/details/ggmlagzfd.sHtML

Go:   os.Args[1:]
来源：http://mobile.yfazqb.com/Article/details/gtcfbgimq.sHtML

Ruby: ARGV
来源：http://wap.epnwcf.com/Article/details/gndeblmsd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.tarul.cn/Article/details/gxprttjvr.sHtML

[M02] 读取环境变量
来源：http://3g.fktsv.cn/Article/details/gugfiwtuv.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.yfazqb.com/Article/details/gtasuwedb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.yfazqb.com/Article/details/gjhbnajht.sHtML

JS:   process.env.HOME
来源：http://read.share.epnwcf.com/Article/details/gubezojjb.sHtML

TS:   process.env.HOME
来源：http://baike.tarul.cn/Article/details/gozdbnwro.sHtML

Java: System.getenv("HOME")
来源：http://3g.tarul.cn/Article/details/gyrgoudjx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fktsv.cn/Article/details/gbanepodk.sHtML

Ruby: ENV["HOME"]
来源：http://baike.tarul.cn/Article/details/ghagdjmxn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.bbcook.cn/Article/details/grsfzdedj.sHtML

[M03] 执行外部命令
来源：http://www.m.share.epnwcf.com/Article/details/gpvtodfcl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.epnwcf.com/Article/details/gmvuaepmz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.yfazqb.com/Article/details/gvvxuguhc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.vehdjk.com/Article/details/grslgmguz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.bbcook.cn/Article/details/gblcgpkan.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.sjlbkw.cn/Article/details/gakbzgjnk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.epnwcf.com/Article/details/gylfbgsmz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.yfazqb.com/Article/details/gizrpsyjt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.bbcook.cn/Article/details/gufnanjqc.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.yfazqb.com/Article/details/gajzfegbp.sHtML

Py:   os.getcwd()
来源：http://3g.tarul.cn/Article/details/gfnqhycpg.sHtML

PHP:  getcwd();
来源：http://www.blog.sjlbkw.cn/Article/details/gknneksdl.sHtML

JS:   process.cwd()
来源：http://mobile.sjlbkw.cn/Article/details/gxxllcfhs.sHtML

TS:   process.cwd()
来源：http://baike.yfazqb.com/Article/details/gcuibujfq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fktsv.cn/Article/details/gzezizszh.sHtML

Go:   os.Getwd()
来源：http://m.share.sjlbkw.cn/Article/details/gswtgtoyb.sHtML

Ruby: Dir.pwd
来源：http://blog.vehdjk.com/Article/details/gfrdfqgso.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fktsv.cn/Article/details/grgxiblex.sHtML

[M05] 设置退出码
来源：http://www.share.tarul.cn/Article/details/gvykzhwdd.sHtML

Py:   sys.exit(1)
来源：http://www.share.tarul.cn/Article/details/gwzzdvjst.sHtML

PHP:  exit(1);
来源：http://mobile.epnwcf.com/Article/details/gwbmgwexs.sHtML

JS:   process.exit(1)
来源：http://wap.bbcook.cn/Article/details/gkhxitafb.sHtML

TS:   process.exit(1)
来源：http://blog.epnwcf.com/Article/details/gosrdhanh.sHtML

Java: System.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/ggzjqtsdn.sHtML

Go:   os.Exit(1)
来源：http://mobile.bbcook.cn/Article/details/gxtvxbrgg.sHtML

Ruby: exit 1
来源：http://mobile.yfazqb.com/Article/details/grzevqafr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.bbcook.cn/Article/details/gdfzsmkqb.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.vehdjk.com/Article/details/gnuwlutoa.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.bbcook.cn/Article/details/gyrfdolax.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fktsv.cn/Article/details/gxiyjgilt.sHtML

JS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/gfnollqjk.sHtML

TS:   console.error("err")
来源：http://baike.epnwcf.com/Article/details/gufzihcix.sHtML

Java: System.err.println("err")
来源：http://read.share.fktsv.cn/Article/details/gogoeerae.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.vehdjk.com/Article/details/gohegzrek.sHtML

Ruby: warn "err"
来源：http://3g.sjlbkw.cn/Article/details/gasupgysc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.sjlbkw.cn/Article/details/gchsljdzb.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.yfazqb.com/Article/details/gieoiytmu.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.yfazqb.com/Article/details/gjlbvvuwo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.yfazqb.com/Article/details/gtsgaqwkb.sHtML

JS:   require.main === module
来源：http://wap.yfazqb.com/Article/details/gwoncneyv.sHtML

TS:   require.main === module
来源：http://www.blog.vehdjk.com/Article/details/gkwemvqez.sHtML

Java: public static void main(String[] args)
来源：http://baike.yfazqb.com/Article/details/gprbpndyd.sHtML

Go:   func main()
来源：http://mobile.yfazqb.com/Article/details/gtwfpsycr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fktsv.cn/Article/details/glxkobtak.sHtML

C#:   static void Main(string[] args)
来源：http://3g.vehdjk.com/Article/details/gmxrvxzvq.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.bbcook.cn/Article/details/gukayngmk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fktsv.cn/Article/details/gfpfcxvyd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fktsv.cn/Article/details/gornyypzl.sHtML

JS:   process.platform;  process.version
来源：http://3g.tarul.cn/Article/details/gscnbaakg.sHtML

TS:   process.platform;  process.version
来源：http://3g.fktsv.cn/Article/details/gjrwjdupv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.vehdjk.com/Article/details/gvjwwbbee.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.bbcook.cn/Article/details/gcjubuvfk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.sjlbkw.cn/Article/details/gysfpdcuv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fktsv.cn/Article/details/guaochuiy.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/grkvumfjo.sHtML

N. 数据结构与算法
来源：http://wap.yfazqb.com/Article/details/gqzgybwlf.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gupmxnrgj.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.epnwcf.com/Article/details/guogfhyqb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fktsv.cn/Article/details/ghzhioxtg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggiebccbn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.epnwcf.com/Article/details/gfkslfibu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.bbcook.cn/Article/details/gglpzmizd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gxyfjkzjd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.vehdjk.com/Article/details/gddadjdve.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fktsv.cn/Article/details/ghmdbyduw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gwirzlsnz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fktsv.cn/Article/details/gqxvnyrfh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.tarul.cn/Article/details/gggcjajab.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.vehdjk.com/Article/details/gvaazkbgu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.vehdjk.com/Article/details/glmytnamz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.sjlbkw.cn/Article/details/gzaccnjwk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.yfazqb.com/Article/details/goszfxrjr.sHtML

Go:   slices.Sort(arr)
来源：http://baike.bbcook.cn/Article/details/gjtctmqlo.sHtML

Ruby: arr.sort
来源：http://blog.sjlbkw.cn/Article/details/gdhejkwdq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.yfazqb.com/Article/details/gbmskrcgq.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fktsv.cn/Article/details/geiaywjzd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.tarul.cn/Article/details/guaihgubq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fktsv.cn/Article/details/gcpwaatfr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.bbcook.cn/Article/details/gaqjbiqih.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.sjlbkw.cn/Article/details/gabqwnxuk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.epnwcf.com/Article/details/gvoetoeru.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.epnwcf.com/Article/details/gryqzhzie.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fktsv.cn/Article/details/gwxvgqstc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.sjlbkw.cn/Article/details/gzqwykzzt.sHtML

[N04] 斐波那契数列
来源：http://mobile.tarul.cn/Article/details/gnipzckwn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fktsv.cn/Article/details/gtlqazgxm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.sjlbkw.cn/Article/details/gwcfcsxzg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.sjlbkw.cn/Article/details/gdvxsxwna.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/gkujahlpx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.bbcook.cn/Article/details/gpjkzbhdv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.bbcook.cn/Article/details/gbfndkzuu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.vehdjk.com/Article/details/gfebnopue.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/gsefhdxbo.sHtML

[N05] 最大公约数
来源：http://m.share.bbcook.cn/Article/details/gqrgswpxe.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.vehdjk.com/Article/details/guisevvzx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.yfazqb.com/Article/details/gktoskjot.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.bbcook.cn/Article/details/gpkhnkszg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.tarul.cn/Article/details/gijrtaxog.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.tarul.cn/Article/details/gppqorffi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.yfazqb.com/Article/details/gnbuyzneg.sHtML

Ruby: a.gcd(b)
来源：http://www.share.bbcook.cn/Article/details/gbxcmlubu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.yfazqb.com/Article/details/gmiypigxa.sHtML

[N06] 判断回文字符串
来源：http://www.blog.tarul.cn/Article/details/gdmsliqwi.sHtML

Py:   s == s[::-1]
来源：http://wap.sjlbkw.cn/Article/details/ghlywystb.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.bbcook.cn/Article/details/gdybdvqao.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gycykjnca.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gnjzfwado.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.tarul.cn/Article/details/gccvelvdf.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.vehdjk.com/Article/details/gwyfucqzg.sHtML

Ruby: s == s.reverse
来源：http://blog.bbcook.cn/Article/details/gygwnwsnk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.bbcook.cn/Article/details/gybaelshm.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.bbcook.cn/Article/details/gisaxjhrc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.bbcook.cn/Article/details/gxghyijbx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.tarul.cn/Article/details/gapqpbadu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlblkasr.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fktsv.cn/Article/details/goxgoxyaw.sHtML

Java: // 手写 HashMap
来源：http://3g.yfazqb.com/Article/details/gbzskzocj.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fktsv.cn/Article/details/gswlheekn.sHtML

Ruby: // 手写 Hash
来源：http://wap.tarul.cn/Article/details/gijjriajv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.sjlbkw.cn/Article/details/gplwocfhu.sHtML

[N08] 生成全排列
来源：http://mobile.fktsv.cn/Article/details/gdrdhrsdn.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.yfazqb.com/Article/details/gsdcqvmrz.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.epnwcf.com/Article/details/gvptemigs.sHtML

JS:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gvqzuphjq.sHtML

TS:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gmkmsoepf.sHtML

Java: // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/ggzqaydmg.sHtML

Go:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/giprgybfy.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fktsv.cn/Article/details/gsolcrzyg.sHtML

C#:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gttzmyiuj.sHtML

[N09] 栈与队列
来源：http://read.share.yfazqb.com/Article/details/gcuxhbzwv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.sjlbkw.cn/Article/details/ggqkgelzu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.tarul.cn/Article/details/ghlcduycw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.tarul.cn/Article/details/gdughchwb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fktsv.cn/Article/details/gscjpoley.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.bbcook.cn/Article/details/gjivgciwg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.vehdjk.com/Article/details/gvzqdmjnw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.yfazqb.com/Article/details/gcprykvxe.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.bbcook.cn/Article/details/gqqtywftm.sHtML

[N10] 链表节点定义
来源：http://read.share.yfazqb.com/Article/details/gdbhacdgz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.bbcook.cn/Article/details/gxihxrnuo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.sjlbkw.cn/Article/details/gcmdyxeup.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.bbcook.cn/Article/details/gwwgdkhbb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.tarul.cn/Article/details/gtdjdtmtf.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.tarul.cn/Article/details/gswatahao.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fktsv.cn/Article/details/gwfpeyvmh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.yfazqb.com/Article/details/gzqlspdsi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.vehdjk.com/Article/details/ghppcwdku.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.epnwcf.com/Article/details/geqvijvnx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.vehdjk.com/Article/details/gtzfdvrbd.sHtML

PHP:  // 手写递归函数
来源：http://mobile.tarul.cn/Article/details/gumbwguiq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.epnwcf.com/Article/details/gffjasjss.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.vehdjk.com/Article/details/gvqiuabmd.sHtML

Java: // 手写递归
来源：http://www.m.share.epnwcf.com/Article/details/ghqoknapk.sHtML

Go:   // 手写递归
来源：http://m.share.vehdjk.com/Article/details/gwqbjvrxl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.epnwcf.com/Article/details/grpqjdtbb.sHtML

C#:   // 手写递归
来源：http://www.m.share.vehdjk.com/Article/details/gafqhboms.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.vehdjk.com/Article/details/gsvfqfcbe.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fktsv.cn/Article/details/ghloiqtso.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.tarul.cn/Article/details/geacytziz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.bbcook.cn/Article/details/gyzkqyahi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.epnwcf.com/Article/details/gppxvkltn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.epnwcf.com/Article/details/ggjdjjvwh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.sjlbkw.cn/Article/details/gcaxhgesn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.yfazqb.com/Article/details/gjjrnfttq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fktsv.cn/Article/details/glgcynplf.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/grxhajtai.sHtML

O. 并发与异步
来源：http://www.blog.yfazqb.com/Article/details/gjbxrqxvd.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gbuuuvqnf.sHtML

[O01] 启动一个线程
来源：http://read.share.yfazqb.com/Article/details/gadkpldue.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.bbcook.cn/Article/details/gmyycqvvg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.vehdjk.com/Article/details/gkpxwggaj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.tarul.cn/Article/details/glxobwlrx.sHtML

TS:   // 同 JS
来源：http://blog.fktsv.cn/Article/details/gpnunonnd.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.sjlbkw.cn/Article/details/gegtfwifl.sHtML

Go:   go f()
来源：http://www.m.share.tarul.cn/Article/details/gedqnflqc.sHtML

Ruby: Thread.new { f }
来源：http://www.share.bbcook.cn/Article/details/gesiwglvk.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.epnwcf.com/Article/details/ggutlvdbb.sHtML

[O02] 使用线程池
来源：http://wap.bbcook.cn/Article/details/gpfqpqtxn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fktsv.cn/Article/details/gofvqsmhe.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.yfazqb.com/Article/details/ggsqqhrum.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fktsv.cn/Article/details/gnwnlzjsz.sHtML


<!-- 参考信息 -->