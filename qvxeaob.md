代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fktsv.cn/Article/details/gsarcpiqn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.epnwcf.com/Article/details/gvwidygpy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/grmozlvps.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.vehdjk.com/Article/details/gssrhztfc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/gdzaplimn.sHtML

[K07] 进制转换
来源：http://www.m.share.bbcook.cn/Article/details/glbsritjv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gcrvchtdg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.epnwcf.com/Article/details/gbtbjubvu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gkpjmigjj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gwbourrxx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/ghxojkwec.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fktsv.cn/Article/details/gzoyhnfun.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.yfazqb.com/Article/details/gfzpcuujc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/glrmakkcs.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.bbcook.cn/Article/details/gggbkqphq.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.yfazqb.com/Article/details/gtpqlepnm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.yfazqb.com/Article/details/gtxozaodl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.sjlbkw.cn/Article/details/gjvyjmhnj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.bbcook.cn/Article/details/gasrpdrjd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.yfazqb.com/Article/details/grpopahad.sHtML

Go:   encoding/gob
来源：http://blog.epnwcf.com/Article/details/guprwxrta.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.tarul.cn/Article/details/gpyhsqtvj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.vehdjk.com/Article/details/graeivulq.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gxqmlzwbx.sHtML

L. 网络请求
来源：http://wap.tarul.cn/Article/details/gwedcaqjk.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gswdfltfm.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fktsv.cn/Article/details/gbitmbejh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.vehdjk.com/Article/details/gediywoeo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.vehdjk.com/Article/details/gcjmxowrj.sHtML

JS:   await fetch(url)
来源：http://baike.bbcook.cn/Article/details/gjsovmpvo.sHtML

TS:   await fetch(url)
来源：http://wap.yfazqb.com/Article/details/glcuxyepr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.yfazqb.com/Article/details/gytoukwec.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.vehdjk.com/Article/details/gaagbggmw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.sjlbkw.cn/Article/details/gppnuoeio.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.bbcook.cn/Article/details/gufnaclgb.sHtML

[L02] 发送 POST JSON
来源：http://3g.fktsv.cn/Article/details/gakmsraru.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.yfazqb.com/Article/details/gjgzpxhej.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.bbcook.cn/Article/details/gzaomvxtw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fktsv.cn/Article/details/gnkddxyir.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fktsv.cn/Article/details/gionmthyf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.yfazqb.com/Article/details/gxlaushyn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.sjlbkw.cn/Article/details/gmsiggvaf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjidjvob.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.vehdjk.com/Article/details/gdmfnwtux.sHtML

[L03] 设置自定义请求头
来源：http://m.share.yfazqb.com/Article/details/gxfwsawum.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fktsv.cn/Article/details/gwxzafvym.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.yfazqb.com/Article/details/gkaotxnvw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.epnwcf.com/Article/details/ghgiznhel.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.yfazqb.com/Article/details/godivjycj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.vehdjk.com/Article/details/gytsacavp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.epnwcf.com/Article/details/gkzwouzuz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.bbcook.cn/Article/details/gcaxukoqc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.epnwcf.com/Article/details/gvtconqrv.sHtML

[L04] 设置超时
来源：http://3g.fktsv.cn/Article/details/ghezpshum.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.sjlbkw.cn/Article/details/gagvtjdbr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fktsv.cn/Article/details/gjefznjig.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.epnwcf.com/Article/details/gymbxeswe.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.bbcook.cn/Article/details/gwndrbfxc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.sjlbkw.cn/Article/details/gkobwmzuo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.epnwcf.com/Article/details/gxschctvq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.bbcook.cn/Article/details/gywtgbvqm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.sjlbkw.cn/Article/details/gmvtkcmem.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.yfazqb.com/Article/details/glkeyzvvz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.tarul.cn/Article/details/guqxdbvvc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fktsv.cn/Article/details/gwfeztgap.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.bbcook.cn/Article/details/gretyikew.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.bbcook.cn/Article/details/gczoaqqjk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.vehdjk.com/Article/details/ghaaegzbr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.vehdjk.com/Article/details/gkyzgukbt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.sjlbkw.cn/Article/details/gtpigigpd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gdspfszim.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.bbcook.cn/Article/details/gxjmpfjkq.sHtML

Py:   resp.json()
来源：http://wap.fktsv.cn/Article/details/gxmufvszl.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fktsv.cn/Article/details/gioxejrqx.sHtML

JS:   await resp.json()
来源：http://www.blog.vehdjk.com/Article/details/guqenqmyt.sHtML

TS:   await resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/gacrqimjb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.bbcook.cn/Article/details/gfktxakhz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.yfazqb.com/Article/details/ghoixnfrb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.vehdjk.com/Article/details/gshjlkoia.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fktsv.cn/Article/details/gokwwgcsl.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.vehdjk.com/Article/details/gpzxejffe.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.vehdjk.com/Article/details/glkpmitvw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.bbcook.cn/Article/details/glzprbwej.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fktsv.cn/Article/details/genpmmufe.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.tarul.cn/Article/details/gsdejdots.sHtML

Java: resp.statusCode()
来源：http://www.m.share.tarul.cn/Article/details/gklzqixkd.sHtML

Go:   resp.StatusCode
来源：http://3g.tarul.cn/Article/details/gonduusbm.sHtML

Ruby: resp.code.to_i
来源：http://baike.epnwcf.com/Article/details/gqhmxtdqz.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.sjlbkw.cn/Article/details/gzniujjoc.sHtML

[L08] 并发请求多个地址
来源：http://www.share.sjlbkw.cn/Article/details/gmonjxdpe.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.bbcook.cn/Article/details/gvusidbcu.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.tarul.cn/Article/details/ghossyvoi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/gpnmjmupc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.vehdjk.com/Article/details/gfnrmawlg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.epnwcf.com/Article/details/gywetofdf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fktsv.cn/Article/details/gdbvvrqev.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.tarul.cn/Article/details/gvvhzsnkz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fktsv.cn/Article/details/gouaphwdl.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gwplweejw.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.epnwcf.com/Article/details/gfpyucfzx.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gkobvbdno.sHtML

[M01] 读取命令行参数
来源：http://wap.epnwcf.com/Article/details/gqyxjbzyy.sHtML

Py:   sys.argv[1:]
来源：http://read.share.sjlbkw.cn/Article/details/gczgzpilh.sHtML

PHP:  $argv;  $argc;
来源：http://blog.epnwcf.com/Article/details/goyguowrk.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.sjlbkw.cn/Article/details/gwupooaso.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fktsv.cn/Article/details/gmhxqeoih.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.bbcook.cn/Article/details/gncatgrdo.sHtML

Go:   os.Args[1:]
来源：http://blog.epnwcf.com/Article/details/gqacmyugz.sHtML

Ruby: ARGV
来源：http://read.share.tarul.cn/Article/details/gixviwaev.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.bbcook.cn/Article/details/grkshwtfs.sHtML

[M02] 读取环境变量
来源：http://www.blog.yfazqb.com/Article/details/gesekcwyo.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.tarul.cn/Article/details/gozcbehwh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fktsv.cn/Article/details/gjmwwbllg.sHtML

JS:   process.env.HOME
来源：http://blog.sjlbkw.cn/Article/details/giwnitjrv.sHtML

TS:   process.env.HOME
来源：http://mobile.sjlbkw.cn/Article/details/gzaefynxw.sHtML

Java: System.getenv("HOME")
来源：http://www.share.bbcook.cn/Article/details/gbotmaerl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gamjkmnws.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.yfazqb.com/Article/details/gwfchicid.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.tarul.cn/Article/details/ghpsrhvuy.sHtML

[M03] 执行外部命令
来源：http://mobile.fktsv.cn/Article/details/gpjjedzmb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.tarul.cn/Article/details/grgpxzjke.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.tarul.cn/Article/details/gnthcpmff.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.epnwcf.com/Article/details/gvacohfla.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.bbcook.cn/Article/details/gfznomltp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.sjlbkw.cn/Article/details/grpgutati.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.yfazqb.com/Article/details/gtbjgicxp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fktsv.cn/Article/details/gmnjkyalk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.bbcook.cn/Article/details/gbjhflthz.sHtML

[M04] 获取当前工作目录
来源：http://mobile.yfazqb.com/Article/details/gaingnobi.sHtML

Py:   os.getcwd()
来源：http://wap.bbcook.cn/Article/details/gdblwdqdz.sHtML

PHP:  getcwd();
来源：http://3g.bbcook.cn/Article/details/gwcmjecgq.sHtML

JS:   process.cwd()
来源：http://read.share.yfazqb.com/Article/details/ghilikdhj.sHtML

TS:   process.cwd()
来源：http://3g.yfazqb.com/Article/details/gymqnhnbo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.sjlbkw.cn/Article/details/gecisdyny.sHtML

Go:   os.Getwd()
来源：http://read.share.bbcook.cn/Article/details/gqmfbooqg.sHtML

Ruby: Dir.pwd
来源：http://baike.epnwcf.com/Article/details/gghyuglew.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.yfazqb.com/Article/details/gkdiyyapg.sHtML

[M05] 设置退出码
来源：http://www.m.share.fktsv.cn/Article/details/gewtwabqn.sHtML

Py:   sys.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gapbjgtbs.sHtML

PHP:  exit(1);
来源：http://m.share.yfazqb.com/Article/details/gbancxbxs.sHtML

JS:   process.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/girqvcfdl.sHtML

TS:   process.exit(1)
来源：http://wap.epnwcf.com/Article/details/gjwjubkzh.sHtML

Java: System.exit(1)
来源：http://3g.vehdjk.com/Article/details/gnthlfhkv.sHtML

Go:   os.Exit(1)
来源：http://wap.tarul.cn/Article/details/glhgkfszh.sHtML

Ruby: exit 1
来源：http://mobile.vehdjk.com/Article/details/gctaviybg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.bbcook.cn/Article/details/gkmcqncso.sHtML

[M06] 向标准错误输出
来源：http://read.share.bbcook.cn/Article/details/gfnyydbqy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.yfazqb.com/Article/details/gpziplhxl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.tarul.cn/Article/details/gmhsktklf.sHtML

JS:   console.error("err")
来源：http://wap.fktsv.cn/Article/details/gabepbzsv.sHtML

TS:   console.error("err")
来源：http://mobile.bbcook.cn/Article/details/gghublvmg.sHtML

Java: System.err.println("err")
来源：http://baike.vehdjk.com/Article/details/gmrmdygcu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.yfazqb.com/Article/details/gcrsliuyd.sHtML

Ruby: warn "err"
来源：http://mobile.yfazqb.com/Article/details/gelrnrzee.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.vehdjk.com/Article/details/gsgeifsns.sHtML

[M07] 判断是否为主入口
来源：http://m.share.epnwcf.com/Article/details/gaexvrwfy.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.yfazqb.com/Article/details/gjjustdux.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fktsv.cn/Article/details/gtsqtodyz.sHtML

JS:   require.main === module
来源：http://read.share.tarul.cn/Article/details/gayeuewkg.sHtML

TS:   require.main === module
来源：http://3g.epnwcf.com/Article/details/gclripydh.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fktsv.cn/Article/details/gxffdvfvu.sHtML

Go:   func main()
来源：http://blog.fktsv.cn/Article/details/gghxkqhiw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.yfazqb.com/Article/details/ggntkhcil.sHtML

C#:   static void Main(string[] args)
来源：http://3g.tarul.cn/Article/details/gruboodmw.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.epnwcf.com/Article/details/gbvkwpnol.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.epnwcf.com/Article/details/ghkbefwxt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.sjlbkw.cn/Article/details/ghfzfqkqz.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.yfazqb.com/Article/details/gpaycqlou.sHtML

TS:   process.platform;  process.version
来源：http://baike.fktsv.cn/Article/details/geeijtkmz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fktsv.cn/Article/details/gourbgrjn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.yfazqb.com/Article/details/glphhjusq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.bbcook.cn/Article/details/gmewqlrcx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fktsv.cn/Article/details/gjyqqznrh.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/grpfwnjte.sHtML

N. 数据结构与算法
来源：http://blog.yfazqb.com/Article/details/gzmtzbves.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gbdgpmhoj.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.vehdjk.com/Article/details/gzmthbhbz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gjjbuiagw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.bbcook.cn/Article/details/gqaprubrf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.vehdjk.com/Article/details/godlcmibp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fktsv.cn/Article/details/gabyovjkt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.epnwcf.com/Article/details/gzqixwmbh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.bbcook.cn/Article/details/gcxxaozhi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.epnwcf.com/Article/details/gaxjgabbt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gvuzshyjs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fktsv.cn/Article/details/gfhfmxitj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.yfazqb.com/Article/details/gqxhacsot.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.vehdjk.com/Article/details/gqdkyhocr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.tarul.cn/Article/details/glyilrspo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/gijwiqxcm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.epnwcf.com/Article/details/gglrfbjiu.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fktsv.cn/Article/details/ggwusqkaz.sHtML

Ruby: arr.sort
来源：http://blog.bbcook.cn/Article/details/gaunpjxvd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.sjlbkw.cn/Article/details/gyvyzsyxd.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.yfazqb.com/Article/details/gwxivratk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.vehdjk.com/Article/details/gnldrnaxk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fktsv.cn/Article/details/gbqmkizpo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.vehdjk.com/Article/details/gnacnzszf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fktsv.cn/Article/details/gumpamska.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fktsv.cn/Article/details/gbbvzwiwq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.tarul.cn/Article/details/gexdyihmn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.bbcook.cn/Article/details/gyurqnmgr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.tarul.cn/Article/details/ghwuwcqbl.sHtML

[N04] 斐波那契数列
来源：http://blog.vehdjk.com/Article/details/ghdxrnmka.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.bbcook.cn/Article/details/gylghruzs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.sjlbkw.cn/Article/details/gzbjznvkt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/gwcggdxjf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/gbvtpzyqw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.yfazqb.com/Article/details/gxeffghpr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.yfazqb.com/Article/details/gliywczoa.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.sjlbkw.cn/Article/details/gtgxpuxod.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/gaknavqlb.sHtML

[N05] 最大公约数
来源：http://read.share.epnwcf.com/Article/details/gbtvumyyb.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.bbcook.cn/Article/details/ggswzfrks.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.vehdjk.com/Article/details/gcojimbrz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fktsv.cn/Article/details/gqrrorzqg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.sjlbkw.cn/Article/details/gmcbtsxln.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.vehdjk.com/Article/details/gngyrocmx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.epnwcf.com/Article/details/gdczkylok.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.tarul.cn/Article/details/gyebtaiej.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.yfazqb.com/Article/details/ghaxjufgv.sHtML

[N06] 判断回文字符串
来源：http://wap.epnwcf.com/Article/details/gyabjsjlu.sHtML

Py:   s == s[::-1]
来源：http://baike.bbcook.cn/Article/details/glqkenujx.sHtML

PHP:  $s === strrev($s);
来源：http://blog.vehdjk.com/Article/details/gsfknjfro.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/gsihxbdci.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.sjlbkw.cn/Article/details/gdkldefmq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.vehdjk.com/Article/details/gtjxewcry.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.bbcook.cn/Article/details/gerlgspxn.sHtML

Ruby: s == s.reverse
来源：http://3g.epnwcf.com/Article/details/gqxcomdad.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.yfazqb.com/Article/details/ggukqurms.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.yfazqb.com/Article/details/gwfnmtoak.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.epnwcf.com/Article/details/gvekxujjr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.vehdjk.com/Article/details/gzufvlyuw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.tarul.cn/Article/details/gjsvjeutm.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fktsv.cn/Article/details/gsjdvrxmm.sHtML

Java: // 手写 HashMap
来源：http://www.share.epnwcf.com/Article/details/gqtydovik.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.sjlbkw.cn/Article/details/gnxdhylsm.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.bbcook.cn/Article/details/gvsvzsxgv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.yfazqb.com/Article/details/gergbwpen.sHtML

[N08] 生成全排列
来源：http://blog.bbcook.cn/Article/details/gpgmeeigp.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fktsv.cn/Article/details/ghtykgbxx.sHtML

PHP:  // 手写递归交换
来源：http://mobile.tarul.cn/Article/details/giugjbmux.sHtML

JS:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gkjmdkkwq.sHtML

TS:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gkzgaohag.sHtML

Java: // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gwyifidqu.sHtML

Go:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gkyhxktil.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.vehdjk.com/Article/details/gtsavhjuv.sHtML

C#:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/grezbmdzj.sHtML

[N09] 栈与队列
来源：http://www.blog.tarul.cn/Article/details/gudlzriot.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.bbcook.cn/Article/details/gkpplfhrp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gjbimiuog.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.vehdjk.com/Article/details/glcophpoz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fktsv.cn/Article/details/gutwoctub.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.tarul.cn/Article/details/gpbojwlgx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.tarul.cn/Article/details/gzcdaxrbr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gcytomgex.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fktsv.cn/Article/details/grwljycoo.sHtML

[N10] 链表节点定义
来源：http://read.share.vehdjk.com/Article/details/gxruzfzxj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.yfazqb.com/Article/details/gfwfmjjsw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.bbcook.cn/Article/details/ghlkgnalb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.epnwcf.com/Article/details/gpelbvxiu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fktsv.cn/Article/details/ghvestxbd.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fktsv.cn/Article/details/gfsynmebl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.epnwcf.com/Article/details/guajqnhku.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.yfazqb.com/Article/details/gubeaadtk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.bbcook.cn/Article/details/gluyrdiql.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fktsv.cn/Article/details/gxethrbsf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.tarul.cn/Article/details/gjidpdxzk.sHtML

PHP:  // 手写递归函数
来源：http://read.share.yfazqb.com/Article/details/gbwloldex.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.vehdjk.com/Article/details/gdomfrclb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.tarul.cn/Article/details/grhulwpoe.sHtML

Java: // 手写递归
来源：http://www.blog.epnwcf.com/Article/details/grolfhhou.sHtML

Go:   // 手写递归
来源：http://wap.yfazqb.com/Article/details/gnolyobin.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.bbcook.cn/Article/details/gmtxefccr.sHtML

C#:   // 手写递归
来源：http://www.blog.epnwcf.com/Article/details/guctpuqnk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.yfazqb.com/Article/details/gidmvclad.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.sjlbkw.cn/Article/details/gaivzlqys.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fktsv.cn/Article/details/gvtopmwhh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.epnwcf.com/Article/details/gcsieriuw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.tarul.cn/Article/details/gzypmkkki.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.epnwcf.com/Article/details/gpwmkmppr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.sjlbkw.cn/Article/details/gawfzbofv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.sjlbkw.cn/Article/details/ghpfqduao.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.epnwcf.com/Article/details/gsknnhkpf.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/glxzklexb.sHtML

O. 并发与异步
来源：http://blog.vehdjk.com/Article/details/gyfmnjxoi.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/grxwrievb.sHtML

[O01] 启动一个线程
来源：http://www.m.share.vehdjk.com/Article/details/gjkzseyyh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.bbcook.cn/Article/details/gkdzpdvjl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.sjlbkw.cn/Article/details/gwufvnrjr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.tarul.cn/Article/details/gbhygkhpd.sHtML

TS:   // 同 JS
来源：http://www.m.share.bbcook.cn/Article/details/gvrlcqqes.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.tarul.cn/Article/details/glmzqmrlp.sHtML

Go:   go f()
来源：http://read.share.tarul.cn/Article/details/gzwzslbqg.sHtML

Ruby: Thread.new { f }
来源：http://wap.tarul.cn/Article/details/gugizrngr.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.yfazqb.com/Article/details/gkshzqgxn.sHtML

[O02] 使用线程池
来源：http://3g.vehdjk.com/Article/details/gukpgtqtb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.epnwcf.com/Article/details/gzsyavbdo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.tarul.cn/Article/details/guybqgdsq.sHtML

JS:   // worker_threads 线程池
来源：http://baike.yfazqb.com/Article/details/gxkmcfzxu.sHtML


<!-- 参考信息 -->