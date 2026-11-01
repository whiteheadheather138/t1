代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/gqsfwjnlm.sHtML

[K07] 进制转换
来源：http://baike.sjlbkw.cn/Article/details/ginbbvbob.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gyqflyxef.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.tarul.cn/Article/details/gwielfltf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gzidsotdw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gvkahcjpi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gjxithbnc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.yfazqb.com/Article/details/gvtznecee.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.vehdjk.com/Article/details/gncupbtca.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gbokpxrir.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.yfazqb.com/Article/details/gasplyidh.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.tarul.cn/Article/details/ggiyyatpj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gieuwmnll.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.epnwcf.com/Article/details/geydbvhdt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.yfazqb.com/Article/details/ghwtxvrlp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fktsv.cn/Article/details/gcqmlkdfq.sHtML

Go:   encoding/gob
来源：http://m.share.vehdjk.com/Article/details/gifuwifiq.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gandmupnt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.yfazqb.com/Article/details/geqxduipw.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/goyorbwyu.sHtML

L. 网络请求
来源：http://m.share.epnwcf.com/Article/details/gnslmisbh.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gpcssszms.sHtML

[L01] 发送 GET 请求
来源：http://blog.tarul.cn/Article/details/gqwiyktzo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.yfazqb.com/Article/details/gzywuqtdr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fktsv.cn/Article/details/gimrjvjde.sHtML

JS:   await fetch(url)
来源：http://m.share.tarul.cn/Article/details/gdwqrigor.sHtML

TS:   await fetch(url)
来源：http://read.share.epnwcf.com/Article/details/gxyoyobsa.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.sjlbkw.cn/Article/details/gtdltrrvu.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.yfazqb.com/Article/details/glbozhmir.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.vehdjk.com/Article/details/gezuyrrqy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.epnwcf.com/Article/details/ggikkombs.sHtML

[L02] 发送 POST JSON
来源：http://wap.fktsv.cn/Article/details/gnowshwjq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.bbcook.cn/Article/details/gzouxsjyd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.bbcook.cn/Article/details/geuobnrqi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fktsv.cn/Article/details/guacefxup.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.epnwcf.com/Article/details/gsdtlgflb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.tarul.cn/Article/details/gefafyysf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.yfazqb.com/Article/details/gxhpufhgg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.yfazqb.com/Article/details/gkxgxmikb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.bbcook.cn/Article/details/gjowpbboa.sHtML

[L03] 设置自定义请求头
来源：http://m.share.tarul.cn/Article/details/gwngqespw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.epnwcf.com/Article/details/gtjqinfdo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.yfazqb.com/Article/details/gdwuhbmaa.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.vehdjk.com/Article/details/gowgoboir.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.sjlbkw.cn/Article/details/glpepbyaw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.epnwcf.com/Article/details/ggkwakedw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.yfazqb.com/Article/details/gisvgyzlk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.sjlbkw.cn/Article/details/ggcdqcsvi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/gylufjbdr.sHtML

[L04] 设置超时
来源：http://blog.tarul.cn/Article/details/gqkrjgenc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.bbcook.cn/Article/details/gocgxvxaa.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.bbcook.cn/Article/details/gfextcylp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.epnwcf.com/Article/details/gymoljhmb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.epnwcf.com/Article/details/gupxypvda.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.epnwcf.com/Article/details/gzbxxtvqh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fktsv.cn/Article/details/gmawsbdzl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.sjlbkw.cn/Article/details/gyfzsqogi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.sjlbkw.cn/Article/details/gatjrmopt.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fktsv.cn/Article/details/ghlkchydp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.vehdjk.com/Article/details/gsayxpduy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.epnwcf.com/Article/details/goqswdbuk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.vehdjk.com/Article/details/giprevhvh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.yfazqb.com/Article/details/gblocvpwn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.bbcook.cn/Article/details/gzmsogkas.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.tarul.cn/Article/details/gowewmrzr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fktsv.cn/Article/details/gbphqlggj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gsnvcslcm.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.yfazqb.com/Article/details/guvbemaul.sHtML

Py:   resp.json()
来源：http://www.blog.tarul.cn/Article/details/gqdpvckts.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.yfazqb.com/Article/details/gputlpbeq.sHtML

JS:   await resp.json()
来源：http://www.m.share.tarul.cn/Article/details/grololsyt.sHtML

TS:   await resp.json()
来源：http://mobile.vehdjk.com/Article/details/gzasbgruc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fktsv.cn/Article/details/gkkbchwli.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.vehdjk.com/Article/details/gpllrmmaz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.vehdjk.com/Article/details/gzfsnxqqc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.bbcook.cn/Article/details/gzxabotpg.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.sjlbkw.cn/Article/details/gokuinxzs.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.sjlbkw.cn/Article/details/guivgxzzs.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.sjlbkw.cn/Article/details/gbpapzneg.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.tarul.cn/Article/details/gnxojgjqr.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.tarul.cn/Article/details/gnjlxxqtm.sHtML

Java: resp.statusCode()
来源：http://www.share.fktsv.cn/Article/details/gxtnsyabz.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fktsv.cn/Article/details/gsmwybwij.sHtML

Ruby: resp.code.to_i
来源：http://blog.vehdjk.com/Article/details/gnvnozfvc.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.epnwcf.com/Article/details/gygrhfsmc.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.vehdjk.com/Article/details/ginftgmrp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.sjlbkw.cn/Article/details/gshesjzqk.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fktsv.cn/Article/details/gpqxsbrpf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.epnwcf.com/Article/details/gsaghhuhc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.epnwcf.com/Article/details/gjbdossqn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.tarul.cn/Article/details/gqevonumk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.tarul.cn/Article/details/glmfgwchu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.bbcook.cn/Article/details/ggkudnrmm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.sjlbkw.cn/Article/details/gfysobomo.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gcerreyry.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fktsv.cn/Article/details/goevyrdia.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gcigkbnru.sHtML

[M01] 读取命令行参数
来源：http://3g.fktsv.cn/Article/details/gqqxhtrhh.sHtML

Py:   sys.argv[1:]
来源：http://mobile.tarul.cn/Article/details/gmbyqspwf.sHtML

PHP:  $argv;  $argc;
来源：http://3g.epnwcf.com/Article/details/gqfwladfh.sHtML

JS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/gmmahrvbz.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.vehdjk.com/Article/details/gdrmxhspi.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.yfazqb.com/Article/details/gsqwggwly.sHtML

Go:   os.Args[1:]
来源：http://m.share.epnwcf.com/Article/details/gtmbcocth.sHtML

Ruby: ARGV
来源：http://read.share.vehdjk.com/Article/details/gmvahsngs.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fktsv.cn/Article/details/gkyknqezw.sHtML

[M02] 读取环境变量
来源：http://3g.fktsv.cn/Article/details/gmfqhgxgc.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.bbcook.cn/Article/details/givhddpdp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.bbcook.cn/Article/details/gzhflydim.sHtML

JS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/ggrrvrbln.sHtML

TS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/gmeqqwmoi.sHtML

Java: System.getenv("HOME")
来源：http://3g.tarul.cn/Article/details/gkfbehvym.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.yfazqb.com/Article/details/gajhotpjc.sHtML

Ruby: ENV["HOME"]
来源：http://3g.tarul.cn/Article/details/gezzyaqod.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.bbcook.cn/Article/details/gjtnrsenf.sHtML

[M03] 执行外部命令
来源：http://wap.fktsv.cn/Article/details/gkxrwoify.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.epnwcf.com/Article/details/gshcqarlj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.sjlbkw.cn/Article/details/glorbbbuz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fktsv.cn/Article/details/gfcexfmaa.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.vehdjk.com/Article/details/gsxeivmeq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.epnwcf.com/Article/details/gebjgycnt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.bbcook.cn/Article/details/gjwydvkcb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.sjlbkw.cn/Article/details/gtmdbsbcs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.bbcook.cn/Article/details/gbgmwvjhl.sHtML

[M04] 获取当前工作目录
来源：http://blog.tarul.cn/Article/details/gtcouezew.sHtML

Py:   os.getcwd()
来源：http://www.m.share.epnwcf.com/Article/details/gvabowntv.sHtML

PHP:  getcwd();
来源：http://m.share.yfazqb.com/Article/details/ghrpbegbw.sHtML

JS:   process.cwd()
来源：http://www.m.share.tarul.cn/Article/details/gkjdxdyfw.sHtML

TS:   process.cwd()
来源：http://baike.vehdjk.com/Article/details/gsgdgqind.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.epnwcf.com/Article/details/gdhxzqpwi.sHtML

Go:   os.Getwd()
来源：http://blog.vehdjk.com/Article/details/gwjmhqlmw.sHtML

Ruby: Dir.pwd
来源：http://mobile.bbcook.cn/Article/details/gmvsqclhj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.epnwcf.com/Article/details/gscusccte.sHtML

[M05] 设置退出码
来源：http://blog.tarul.cn/Article/details/gdmpfbisl.sHtML

Py:   sys.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gzdnikpgy.sHtML

PHP:  exit(1);
来源：http://read.share.sjlbkw.cn/Article/details/gscavofnm.sHtML

JS:   process.exit(1)
来源：http://wap.tarul.cn/Article/details/goysjtkzn.sHtML

TS:   process.exit(1)
来源：http://blog.vehdjk.com/Article/details/gdfdppwby.sHtML

Java: System.exit(1)
来源：http://mobile.tarul.cn/Article/details/gdzegaddw.sHtML

Go:   os.Exit(1)
来源：http://baike.yfazqb.com/Article/details/gobiaqpte.sHtML

Ruby: exit 1
来源：http://read.share.vehdjk.com/Article/details/giosonyje.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.tarul.cn/Article/details/ghsckuvvk.sHtML

[M06] 向标准错误输出
来源：http://baike.tarul.cn/Article/details/gbrikocyo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.yfazqb.com/Article/details/gabgqfgcp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.yfazqb.com/Article/details/glgxwdgua.sHtML

JS:   console.error("err")
来源：http://m.share.epnwcf.com/Article/details/ginchomgq.sHtML

TS:   console.error("err")
来源：http://www.blog.sjlbkw.cn/Article/details/gjhjbkujs.sHtML

Java: System.err.println("err")
来源：http://www.share.fktsv.cn/Article/details/gqruyalxx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.tarul.cn/Article/details/gytpdmwmd.sHtML

Ruby: warn "err"
来源：http://wap.bbcook.cn/Article/details/gdnirbteu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.sjlbkw.cn/Article/details/gnlgdshtg.sHtML

[M07] 判断是否为主入口
来源：http://wap.tarul.cn/Article/details/gddrolvxu.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.yfazqb.com/Article/details/gydzvqwbl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.bbcook.cn/Article/details/goejukaqp.sHtML

JS:   require.main === module
来源：http://www.share.tarul.cn/Article/details/gjslfxlwe.sHtML

TS:   require.main === module
来源：http://read.share.fktsv.cn/Article/details/gwlkgivhr.sHtML

Java: public static void main(String[] args)
来源：http://blog.fktsv.cn/Article/details/gvueivoqc.sHtML

Go:   func main()
来源：http://www.share.sjlbkw.cn/Article/details/gljdujyun.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.vehdjk.com/Article/details/ghqmrzaib.sHtML

C#:   static void Main(string[] args)
来源：http://wap.sjlbkw.cn/Article/details/galywmpnd.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.bbcook.cn/Article/details/gjtmsskzi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.yfazqb.com/Article/details/gewobwgel.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.yfazqb.com/Article/details/ghudahwpo.sHtML

JS:   process.platform;  process.version
来源：http://3g.fktsv.cn/Article/details/gjbeucbhx.sHtML

TS:   process.platform;  process.version
来源：http://wap.yfazqb.com/Article/details/gewdosltj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.epnwcf.com/Article/details/gwpgzbvao.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.bbcook.cn/Article/details/gkpzczdye.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.vehdjk.com/Article/details/gwoiekrpe.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.bbcook.cn/Article/details/gafyupfzb.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/ggalxttlg.sHtML

N. 数据结构与算法
来源：http://www.blog.tarul.cn/Article/details/gtsacxqvd.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gpejnispa.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.epnwcf.com/Article/details/ggdztryqv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gqlwgqttc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.bbcook.cn/Article/details/gzzvqrvis.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.yfazqb.com/Article/details/gbcadganj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.yfazqb.com/Article/details/gdaurzacm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gsuubuqir.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gxmtqzgol.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.bbcook.cn/Article/details/gxxbtlunv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fktsv.cn/Article/details/gcnkqtwpj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.epnwcf.com/Article/details/gpflxsnrv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fktsv.cn/Article/details/gtqyyofgw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.yfazqb.com/Article/details/gyydimecl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.epnwcf.com/Article/details/giknwezbs.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.yfazqb.com/Article/details/gsjlphtwb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.bbcook.cn/Article/details/gitdviccn.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gcnsuazjt.sHtML

Ruby: arr.sort
来源：http://m.share.yfazqb.com/Article/details/gywxlxmtw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.epnwcf.com/Article/details/gpsclxpoq.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.sjlbkw.cn/Article/details/gjebtulye.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.yfazqb.com/Article/details/gdhyetbgy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fktsv.cn/Article/details/gojgjjuyz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.bbcook.cn/Article/details/gvqxeqnmp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.sjlbkw.cn/Article/details/gskqtggct.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fktsv.cn/Article/details/getbtufbt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.sjlbkw.cn/Article/details/gbnybxrvi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.epnwcf.com/Article/details/ggyradfsd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fktsv.cn/Article/details/geeodzmgf.sHtML

[N04] 斐波那契数列
来源：http://3g.tarul.cn/Article/details/gtihimjoh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.tarul.cn/Article/details/guqjocvyf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.bbcook.cn/Article/details/gdmonjqdj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.sjlbkw.cn/Article/details/grsougjrd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/gqviuwsea.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fktsv.cn/Article/details/gcummlpjs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.sjlbkw.cn/Article/details/gcbkxgwzd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fktsv.cn/Article/details/ghuosrpak.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/gtriliogc.sHtML

[N05] 最大公约数
来源：http://read.share.epnwcf.com/Article/details/gntloyshl.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fktsv.cn/Article/details/gmkcqugxh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.tarul.cn/Article/details/greihfdvm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.yfazqb.com/Article/details/gsrduxjxu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.sjlbkw.cn/Article/details/gbomsirvb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.bbcook.cn/Article/details/gwzgpxhzk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.yfazqb.com/Article/details/gxgjfzbfs.sHtML

Ruby: a.gcd(b)
来源：http://blog.bbcook.cn/Article/details/gsxtvygwg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.epnwcf.com/Article/details/gxzmwwcln.sHtML

[N06] 判断回文字符串
来源：http://m.share.vehdjk.com/Article/details/gibrhehpu.sHtML

Py:   s == s[::-1]
来源：http://wap.tarul.cn/Article/details/ghgboehpf.sHtML

PHP:  $s === strrev($s);
来源：http://3g.epnwcf.com/Article/details/geiglyfsh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fktsv.cn/Article/details/ghwxyrrjg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/gwhjpaosl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.sjlbkw.cn/Article/details/glhmemsdd.sHtML

Go:   // 双指针从两端比较
来源：http://baike.bbcook.cn/Article/details/goshjhcfc.sHtML

Ruby: s == s.reverse
来源：http://wap.vehdjk.com/Article/details/gfzacaikv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.yfazqb.com/Article/details/gifrdauee.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fktsv.cn/Article/details/gbgqnybsq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.vehdjk.com/Article/details/geyjeywdg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.sjlbkw.cn/Article/details/gezwsrfyk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.vehdjk.com/Article/details/gvlutbywm.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.sjlbkw.cn/Article/details/gjvamovbu.sHtML

Java: // 手写 HashMap
来源：http://mobile.bbcook.cn/Article/details/guqfqkwct.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.epnwcf.com/Article/details/gmzftetuo.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.epnwcf.com/Article/details/gbcxguslu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.vehdjk.com/Article/details/gkhclsvlf.sHtML

[N08] 生成全排列
来源：http://m.share.sjlbkw.cn/Article/details/gcwofbthf.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.tarul.cn/Article/details/gefspzhry.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.tarul.cn/Article/details/goagijscm.sHtML

JS:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/guhwedmeh.sHtML

TS:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gdoigsyrc.sHtML

Java: // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gettctznh.sHtML

Go:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gfsbvsjsu.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.tarul.cn/Article/details/gfhlkhhbl.sHtML

C#:   // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/gquajpqzf.sHtML

[N09] 栈与队列
来源：http://wap.sjlbkw.cn/Article/details/gnmlkgcor.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.bbcook.cn/Article/details/geltebmni.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.vehdjk.com/Article/details/gfkrdabfi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gmnscehkl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.yfazqb.com/Article/details/guiegamum.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.epnwcf.com/Article/details/gihixbpdj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.tarul.cn/Article/details/gigkbjhwf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.tarul.cn/Article/details/ghbfyymqw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.sjlbkw.cn/Article/details/glbymqhbx.sHtML

[N10] 链表节点定义
来源：http://www.share.yfazqb.com/Article/details/gpupuidzw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.bbcook.cn/Article/details/gswnvhjdo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.epnwcf.com/Article/details/gmphfbwrx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.epnwcf.com/Article/details/gdsfzqjug.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.sjlbkw.cn/Article/details/gyojghvge.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.bbcook.cn/Article/details/gkqpxfbbe.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.yfazqb.com/Article/details/gjddqrnnd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.epnwcf.com/Article/details/gfzfxbhii.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.sjlbkw.cn/Article/details/gcgkpunxh.sHtML

[N11] 二叉树中序遍历
来源：http://wap.yfazqb.com/Article/details/gpvfcwwew.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.tarul.cn/Article/details/gaabrozzb.sHtML

PHP:  // 手写递归函数
来源：http://m.share.vehdjk.com/Article/details/gohagxgvv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.vehdjk.com/Article/details/ghbhqwhho.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.yfazqb.com/Article/details/gqfwrkjca.sHtML

Java: // 手写递归
来源：http://baike.fktsv.cn/Article/details/ggxwzboeu.sHtML

Go:   // 手写递归
来源：http://read.share.tarul.cn/Article/details/gfnmhkzvs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.yfazqb.com/Article/details/gmojngkam.sHtML

C#:   // 手写递归
来源：http://wap.bbcook.cn/Article/details/gjxseoijs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.epnwcf.com/Article/details/ghbnbfysn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fktsv.cn/Article/details/gfbmsulvk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.epnwcf.com/Article/details/gtepeljut.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.sjlbkw.cn/Article/details/gbbmqmxsh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.bbcook.cn/Article/details/gqzruawzq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fktsv.cn/Article/details/gqzfqyory.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fktsv.cn/Article/details/gmkdbzvny.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.bbcook.cn/Article/details/gzqiqideu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.tarul.cn/Article/details/gzobwderb.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gwawbpamw.sHtML

O. 并发与异步
来源：http://wap.vehdjk.com/Article/details/gokdbokcp.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gqrayjphs.sHtML

[O01] 启动一个线程
来源：http://m.share.fktsv.cn/Article/details/gkbbnnaxz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.tarul.cn/Article/details/gzmlgckoz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.bbcook.cn/Article/details/gjzeemxpk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.vehdjk.com/Article/details/gfjtzqzvc.sHtML

TS:   // 同 JS
来源：http://read.share.sjlbkw.cn/Article/details/giutcoyjz.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.bbcook.cn/Article/details/gskhxmuyh.sHtML

Go:   go f()
来源：http://www.m.share.vehdjk.com/Article/details/gtizthlvv.sHtML

Ruby: Thread.new { f }
来源：http://www.share.bbcook.cn/Article/details/gaivqtsyd.sHtML

C#:   Task.Run(() => F());
来源：http://wap.yfazqb.com/Article/details/gnojixawz.sHtML

[O02] 使用线程池
来源：http://mobile.epnwcf.com/Article/details/gpqvucjgj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.epnwcf.com/Article/details/gpgvbjcpe.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.bbcook.cn/Article/details/gdsepkpmv.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fktsv.cn/Article/details/gtpzmmkpc.sHtML

TS:   // worker_threads 线程池
来源：http://3g.epnwcf.com/Article/details/gjkmpqryg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.vehdjk.com/Article/details/gbfekreyt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.tarul.cn/Article/details/glsjafgux.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.tarul.cn/Article/details/gsuirzqkm.sHtML


<!-- 参考信息 -->