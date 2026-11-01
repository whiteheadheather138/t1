代发 wailian999

[K06] 解析 URL 查询串
来源：http://baike.sjlbkw.cn/Article/details/gnwsnwhht.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.vehdjk.com/Article/details/guzbdnxnd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.bbcook.cn/Article/details/gqrdsrheo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fktsv.cn/Article/details/gekulgefg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.yfazqb.com/Article/details/gmgujaraj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.bbcook.cn/Article/details/gnjisvfwp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/gciutelvp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.sjlbkw.cn/Article/details/gybqrkmuk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.tarul.cn/Article/details/gmrgbmbqc.sHtML

[K07] 进制转换
来源：http://blog.fktsv.cn/Article/details/glgllhygy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gxhgooala.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.vehdjk.com/Article/details/gzcncdtfr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gawnuiywd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gychzjbnl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gsnqfqzhr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.bbcook.cn/Article/details/gliwkzvsu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.vehdjk.com/Article/details/gbkcjzrur.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gkuxlwrsq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.vehdjk.com/Article/details/gexxairwc.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fktsv.cn/Article/details/gdftbuyzn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.tarul.cn/Article/details/glefjjjgr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.bbcook.cn/Article/details/gnenziuix.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fktsv.cn/Article/details/gbkeywcjm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.epnwcf.com/Article/details/gruhvktcf.sHtML

Go:   encoding/gob
来源：http://read.share.vehdjk.com/Article/details/gsbwkazht.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.bbcook.cn/Article/details/glhiwuldb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.vehdjk.com/Article/details/gawljtdzr.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gxvudsfyn.sHtML

L. 网络请求
来源：http://wap.bbcook.cn/Article/details/gklieecrv.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gyobxxbyb.sHtML

[L01] 发送 GET 请求
来源：http://3g.bbcook.cn/Article/details/gdcjaljvs.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fktsv.cn/Article/details/gccguzwuz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.tarul.cn/Article/details/gzdiiatgl.sHtML

JS:   await fetch(url)
来源：http://m.share.bbcook.cn/Article/details/gkoayzcmo.sHtML

TS:   await fetch(url)
来源：http://www.blog.fktsv.cn/Article/details/ggjrjialp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.tarul.cn/Article/details/gfdmsfyum.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.bbcook.cn/Article/details/gjqculptw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.epnwcf.com/Article/details/gqllggdqk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.vehdjk.com/Article/details/gmzscmtbs.sHtML

[L02] 发送 POST JSON
来源：http://3g.epnwcf.com/Article/details/grubmobwo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.bbcook.cn/Article/details/gxlaeqdsa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.bbcook.cn/Article/details/guzebmtiu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fktsv.cn/Article/details/gqtakphaq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.yfazqb.com/Article/details/gmrahpbmb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.epnwcf.com/Article/details/gkivlbxep.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fktsv.cn/Article/details/gnoirbeog.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fktsv.cn/Article/details/gmtdtknyl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.vehdjk.com/Article/details/gwmxvhubj.sHtML

[L03] 设置自定义请求头
来源：http://mobile.vehdjk.com/Article/details/gurgclvhy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.yfazqb.com/Article/details/gtjkaoael.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.tarul.cn/Article/details/gjqwsavfq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/gtqtemrbf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.tarul.cn/Article/details/glciqbxaz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fktsv.cn/Article/details/gifrsixdd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.vehdjk.com/Article/details/gtnhwuqoe.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.epnwcf.com/Article/details/gbtlbxavg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.bbcook.cn/Article/details/gnccdeiah.sHtML

[L04] 设置超时
来源：http://blog.sjlbkw.cn/Article/details/gqugcehui.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.epnwcf.com/Article/details/gkiburjio.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.bbcook.cn/Article/details/gyowqapov.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.epnwcf.com/Article/details/gkcekaemw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.vehdjk.com/Article/details/gmoogwbqx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.bbcook.cn/Article/details/gxvevpzjj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.vehdjk.com/Article/details/goyicqbce.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.bbcook.cn/Article/details/gqylmeoaf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.bbcook.cn/Article/details/gfknewjht.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.sjlbkw.cn/Article/details/gvfsmxzab.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.tarul.cn/Article/details/giefrvgjs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fktsv.cn/Article/details/goedlgvki.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.bbcook.cn/Article/details/gqaqrgztu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.yfazqb.com/Article/details/gqioqrssi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.epnwcf.com/Article/details/gcxfjdwsw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.yfazqb.com/Article/details/gfjjnfcvb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.bbcook.cn/Article/details/gdcgbhhao.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.sjlbkw.cn/Article/details/ghbagnuzq.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fktsv.cn/Article/details/gpbelvflq.sHtML

Py:   resp.json()
来源：http://www.blog.bbcook.cn/Article/details/ghlzaepxi.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.bbcook.cn/Article/details/gecpehcez.sHtML

JS:   await resp.json()
来源：http://read.share.yfazqb.com/Article/details/grcnaigry.sHtML

TS:   await resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gqrjedpoo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.vehdjk.com/Article/details/gikwkkfpk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.epnwcf.com/Article/details/goygjncie.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.sjlbkw.cn/Article/details/gqihcyttp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.sjlbkw.cn/Article/details/gpinuvtvu.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.sjlbkw.cn/Article/details/ghwszxmob.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.sjlbkw.cn/Article/details/gahlrrjot.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.epnwcf.com/Article/details/gumostscq.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.epnwcf.com/Article/details/gmtoeoptb.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.yfazqb.com/Article/details/gkfopvxsp.sHtML

Java: resp.statusCode()
来源：http://read.share.yfazqb.com/Article/details/gnhuubmqp.sHtML

Go:   resp.StatusCode
来源：http://www.share.fktsv.cn/Article/details/giaiheoke.sHtML

Ruby: resp.code.to_i
来源：http://mobile.epnwcf.com/Article/details/gbroubcsr.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.tarul.cn/Article/details/gieumsfly.sHtML

[L08] 并发请求多个地址
来源：http://www.share.yfazqb.com/Article/details/gjevgotvb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fktsv.cn/Article/details/gxahbwrti.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.tarul.cn/Article/details/gxddtjape.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fktsv.cn/Article/details/geblxbkbt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.epnwcf.com/Article/details/gicdsycbk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.yfazqb.com/Article/details/ggfkwhbee.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.epnwcf.com/Article/details/gskztmtys.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.tarul.cn/Article/details/gzoelzgcf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.bbcook.cn/Article/details/gzqhfhykk.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gtpbobbfi.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.epnwcf.com/Article/details/gcvqvecyj.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gcxwixcho.sHtML

[M01] 读取命令行参数
来源：http://3g.sjlbkw.cn/Article/details/gvaxqrbke.sHtML

Py:   sys.argv[1:]
来源：http://read.share.vehdjk.com/Article/details/giffffsac.sHtML

PHP:  $argv;  $argc;
来源：http://3g.bbcook.cn/Article/details/gtssxszpu.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.vehdjk.com/Article/details/gmuxyivps.sHtML

TS:   process.argv.slice(2)
来源：http://wap.sjlbkw.cn/Article/details/gygrhabkr.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.epnwcf.com/Article/details/goalxqafx.sHtML

Go:   os.Args[1:]
来源：http://3g.fktsv.cn/Article/details/gjnapkpsm.sHtML

Ruby: ARGV
来源：http://mobile.vehdjk.com/Article/details/gwshzpjbf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.tarul.cn/Article/details/gudwxelub.sHtML

[M02] 读取环境变量
来源：http://www.share.tarul.cn/Article/details/gfrwudkqu.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.epnwcf.com/Article/details/gocbvxjdi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fktsv.cn/Article/details/gfsdoucgo.sHtML

JS:   process.env.HOME
来源：http://wap.epnwcf.com/Article/details/geopnotae.sHtML

TS:   process.env.HOME
来源：http://www.blog.yfazqb.com/Article/details/gugxafitk.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.tarul.cn/Article/details/gnupumaaw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.epnwcf.com/Article/details/gzsgfoxec.sHtML

Ruby: ENV["HOME"]
来源：http://3g.bbcook.cn/Article/details/gddxnzyqv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.tarul.cn/Article/details/gcxqfwtlb.sHtML

[M03] 执行外部命令
来源：http://www.m.share.vehdjk.com/Article/details/gbmjcfaem.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.tarul.cn/Article/details/gqjqyjzuz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.yfazqb.com/Article/details/gmxuxvunm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.sjlbkw.cn/Article/details/gqarwzvrz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.tarul.cn/Article/details/gbvxakyfb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.yfazqb.com/Article/details/guidgpggx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.sjlbkw.cn/Article/details/gjbsvsqku.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.epnwcf.com/Article/details/gtvzmibpm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.yfazqb.com/Article/details/gfqcdorfg.sHtML

[M04] 获取当前工作目录
来源：http://read.share.sjlbkw.cn/Article/details/golqlubra.sHtML

Py:   os.getcwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvyzfvkcx.sHtML

PHP:  getcwd();
来源：http://www.m.share.yfazqb.com/Article/details/gkaqpuktn.sHtML

JS:   process.cwd()
来源：http://blog.bbcook.cn/Article/details/gzanwheds.sHtML

TS:   process.cwd()
来源：http://m.share.epnwcf.com/Article/details/gufpovdpb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.vehdjk.com/Article/details/gtovdylmp.sHtML

Go:   os.Getwd()
来源：http://blog.epnwcf.com/Article/details/gwhfjcmcv.sHtML

Ruby: Dir.pwd
来源：http://wap.bbcook.cn/Article/details/glabgnnad.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.epnwcf.com/Article/details/ghhxrnzqn.sHtML

[M05] 设置退出码
来源：http://www.m.share.epnwcf.com/Article/details/gzotwfijf.sHtML

Py:   sys.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gwgyfdzkq.sHtML

PHP:  exit(1);
来源：http://baike.yfazqb.com/Article/details/gwxpejfhx.sHtML

JS:   process.exit(1)
来源：http://blog.bbcook.cn/Article/details/ggjzokkxu.sHtML

TS:   process.exit(1)
来源：http://blog.tarul.cn/Article/details/gnqzjvqxj.sHtML

Java: System.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gypevauxn.sHtML

Go:   os.Exit(1)
来源：http://www.share.tarul.cn/Article/details/gdtpmvhjh.sHtML

Ruby: exit 1
来源：http://3g.bbcook.cn/Article/details/gqozrxefn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.tarul.cn/Article/details/gykladcef.sHtML

[M06] 向标准错误输出
来源：http://m.share.tarul.cn/Article/details/ggybgnjja.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.vehdjk.com/Article/details/gcmfxnqfb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.bbcook.cn/Article/details/gvubdyngf.sHtML

JS:   console.error("err")
来源：http://baike.bbcook.cn/Article/details/gydyeluvt.sHtML

TS:   console.error("err")
来源：http://m.share.yfazqb.com/Article/details/gfevfrzou.sHtML

Java: System.err.println("err")
来源：http://www.share.sjlbkw.cn/Article/details/gbonvooza.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.yfazqb.com/Article/details/gcjglcxfj.sHtML

Ruby: warn "err"
来源：http://www.m.share.vehdjk.com/Article/details/gveibtgoc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.yfazqb.com/Article/details/gohpcpihh.sHtML

[M07] 判断是否为主入口
来源：http://baike.sjlbkw.cn/Article/details/gfyfyedvc.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.vehdjk.com/Article/details/gtpkbeiau.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.vehdjk.com/Article/details/gsjosszov.sHtML

JS:   require.main === module
来源：http://baike.tarul.cn/Article/details/gxislvuaq.sHtML

TS:   require.main === module
来源：http://read.share.yfazqb.com/Article/details/gnohonuvf.sHtML

Java: public static void main(String[] args)
来源：http://www.share.yfazqb.com/Article/details/gusdivcxw.sHtML

Go:   func main()
来源：http://baike.bbcook.cn/Article/details/gspszpnty.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.tarul.cn/Article/details/ghvggvxdd.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.sjlbkw.cn/Article/details/gsxgltqls.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.yfazqb.com/Article/details/gkmbaduud.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.bbcook.cn/Article/details/gxrxyjxlg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.epnwcf.com/Article/details/gyrbycrcw.sHtML

JS:   process.platform;  process.version
来源：http://read.share.epnwcf.com/Article/details/gpupayhzn.sHtML

TS:   process.platform;  process.version
来源：http://mobile.tarul.cn/Article/details/gbqwmtuwq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.epnwcf.com/Article/details/gsxblmebv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.tarul.cn/Article/details/girsyrzye.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.tarul.cn/Article/details/gcnqxhvmt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fktsv.cn/Article/details/gjqcolczj.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gvtsrmfuc.sHtML

N. 数据结构与算法
来源：http://read.share.bbcook.cn/Article/details/ggjjhgpiu.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gnxgjtejc.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.epnwcf.com/Article/details/gkmufajhd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gwtrgliqn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.tarul.cn/Article/details/gppktgohp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.epnwcf.com/Article/details/gglxiipdv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.tarul.cn/Article/details/gplebbccw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gwzimhiqa.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.tarul.cn/Article/details/gcmnfrdkg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fktsv.cn/Article/details/gfsqzrmjy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.epnwcf.com/Article/details/gacudfqvi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.bbcook.cn/Article/details/gnrjxnowi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fktsv.cn/Article/details/gewsogiuh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.yfazqb.com/Article/details/gcetvjmqj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/grwrvwthl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fktsv.cn/Article/details/guzkssmwp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fktsv.cn/Article/details/girawtdcx.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fktsv.cn/Article/details/gnlyryure.sHtML

Ruby: arr.sort
来源：http://www.blog.vehdjk.com/Article/details/gagfqpowt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.yfazqb.com/Article/details/gisasllqr.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.bbcook.cn/Article/details/gkoklnhqw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.sjlbkw.cn/Article/details/gzlokswac.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.bbcook.cn/Article/details/gqsaqzwxf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.epnwcf.com/Article/details/gtyuavzyi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.epnwcf.com/Article/details/grqgogumq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.tarul.cn/Article/details/ggpdfsnrx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.yfazqb.com/Article/details/gqqyiiply.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.bbcook.cn/Article/details/gocihlspw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.tarul.cn/Article/details/gtaigenxu.sHtML

[N04] 斐波那契数列
来源：http://read.share.yfazqb.com/Article/details/gpjlgvzlq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.sjlbkw.cn/Article/details/grorddfrh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.epnwcf.com/Article/details/gxbmenlax.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.tarul.cn/Article/details/gtgkhlndv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/gvxhmbtcq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.epnwcf.com/Article/details/gengjliqg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.epnwcf.com/Article/details/gkiaexgds.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.tarul.cn/Article/details/gjnebttev.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/gdwxhtluc.sHtML

[N05] 最大公约数
来源：http://read.share.bbcook.cn/Article/details/gdbihutpm.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fktsv.cn/Article/details/ggaxwtwvg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.epnwcf.com/Article/details/gvyovsqfl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.bbcook.cn/Article/details/gniwctpwy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.bbcook.cn/Article/details/gnagybkef.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.yfazqb.com/Article/details/gcyzfsfcx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.epnwcf.com/Article/details/gjkqnkrto.sHtML

Ruby: a.gcd(b)
来源：http://www.share.epnwcf.com/Article/details/glnghzcuc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.yfazqb.com/Article/details/gxqohrqhb.sHtML

[N06] 判断回文字符串
来源：http://m.share.fktsv.cn/Article/details/gonbuepyv.sHtML

Py:   s == s[::-1]
来源：http://read.share.sjlbkw.cn/Article/details/gfappexpd.sHtML

PHP:  $s === strrev($s);
来源：http://wap.tarul.cn/Article/details/grossboea.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/gmbxebgwo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/gjdtkymmv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.vehdjk.com/Article/details/gxtkozllx.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fktsv.cn/Article/details/gjpmlthqk.sHtML

Ruby: s == s.reverse
来源：http://mobile.epnwcf.com/Article/details/gwpeossvu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.vehdjk.com/Article/details/gvlnkhskr.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.sjlbkw.cn/Article/details/gjyhcmndr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.yfazqb.com/Article/details/gxlyhpped.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.bbcook.cn/Article/details/gqlqctwhr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.sjlbkw.cn/Article/details/ghhnkdbzf.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.tarul.cn/Article/details/gixvcuyzz.sHtML

Java: // 手写 HashMap
来源：http://read.share.tarul.cn/Article/details/glsvmypbu.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fktsv.cn/Article/details/gsqfdlavi.sHtML

Ruby: // 手写 Hash
来源：http://www.share.epnwcf.com/Article/details/gnmwukrdx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.vehdjk.com/Article/details/gcortlgqh.sHtML

[N08] 生成全排列
来源：http://www.blog.yfazqb.com/Article/details/gfavltwvw.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.vehdjk.com/Article/details/gkzegesqn.sHtML

PHP:  // 手写递归交换
来源：http://baike.fktsv.cn/Article/details/gxtkldgbs.sHtML

JS:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gvahjjhix.sHtML

TS:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gbohezfmj.sHtML

Java: // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gwmzdgkol.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/ggwlkqjsk.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fktsv.cn/Article/details/goffqlrwv.sHtML

C#:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gqffehamd.sHtML

[N09] 栈与队列
来源：http://www.blog.bbcook.cn/Article/details/gwncxunxh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.epnwcf.com/Article/details/gugimxasr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gbnfxrbhr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fktsv.cn/Article/details/gsoqoikxp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.tarul.cn/Article/details/gjfkcpbat.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.tarul.cn/Article/details/gxxvuesrn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.vehdjk.com/Article/details/ggqgdzcqg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fktsv.cn/Article/details/gtfdntwxq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.tarul.cn/Article/details/gtfroigwl.sHtML

[N10] 链表节点定义
来源：http://baike.sjlbkw.cn/Article/details/gfhzhxqfz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.yfazqb.com/Article/details/gabuqtlbt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.bbcook.cn/Article/details/gmsrdtjhe.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.sjlbkw.cn/Article/details/grrqpjspu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzbvsbog.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.tarul.cn/Article/details/gmdharrqh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.sjlbkw.cn/Article/details/gtbpjalqf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.bbcook.cn/Article/details/gkpybnrqv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.vehdjk.com/Article/details/gunsoviay.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.vehdjk.com/Article/details/gsfgmmjtk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fktsv.cn/Article/details/glgxfijdo.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fktsv.cn/Article/details/gjpodyntb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fktsv.cn/Article/details/gqjjfhbax.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.yfazqb.com/Article/details/gudfupnvq.sHtML

Java: // 手写递归
来源：http://blog.fktsv.cn/Article/details/gnogcawpt.sHtML

Go:   // 手写递归
来源：http://www.m.share.vehdjk.com/Article/details/gohemgjvv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.sjlbkw.cn/Article/details/gpgaarxdl.sHtML

C#:   // 手写递归
来源：http://baike.bbcook.cn/Article/details/gowzoaalk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.tarul.cn/Article/details/grffvpmmo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.epnwcf.com/Article/details/gkmgsjvcn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.vehdjk.com/Article/details/grdkwrrpb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.vehdjk.com/Article/details/gyxmikkxv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.vehdjk.com/Article/details/gppedrpsx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.vehdjk.com/Article/details/gazqpbuey.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.tarul.cn/Article/details/gzlcemcvl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.vehdjk.com/Article/details/gpawxguft.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.yfazqb.com/Article/details/gsjbpfufs.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gdwfewpha.sHtML

O. 并发与异步
来源：http://3g.bbcook.cn/Article/details/glldippqj.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gigtaygtf.sHtML

[O01] 启动一个线程
来源：http://m.share.sjlbkw.cn/Article/details/gujlubexq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.sjlbkw.cn/Article/details/gimpzgcaw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.vehdjk.com/Article/details/gopegizwo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.yfazqb.com/Article/details/gbbscnqqq.sHtML

TS:   // 同 JS
来源：http://www.share.epnwcf.com/Article/details/gdscixere.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.sjlbkw.cn/Article/details/gnegvqdwo.sHtML

Go:   go f()
来源：http://baike.fktsv.cn/Article/details/gyzuxtesw.sHtML

Ruby: Thread.new { f }
来源：http://www.share.bbcook.cn/Article/details/gzqpcnpxy.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fktsv.cn/Article/details/gsckldzbi.sHtML


<!-- 参考信息 -->