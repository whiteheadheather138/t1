代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.epnwcf.com/Article/details/gdnzusmsj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fktsv.cn/Article/details/geyvooqmy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/gqszsrhhd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.bbcook.cn/Article/details/gysjkpwif.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.sjlbkw.cn/Article/details/gruxaozwp.sHtML

[K07] 进制转换
来源：http://3g.vehdjk.com/Article/details/gcrvfigcz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gynvxcbvd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fktsv.cn/Article/details/gmjbdyldk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnzihrka.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gplpycilu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gtknzxqjy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.sjlbkw.cn/Article/details/gypjbrvxn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.yfazqb.com/Article/details/gnmotpckw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrqxtaeb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fktsv.cn/Article/details/gsevnvteb.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fktsv.cn/Article/details/gmjyhzkkx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.epnwcf.com/Article/details/gqetdfeib.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.tarul.cn/Article/details/gldphbukw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.sjlbkw.cn/Article/details/gdydhseud.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.sjlbkw.cn/Article/details/gopqumouu.sHtML

Go:   encoding/gob
来源：http://3g.epnwcf.com/Article/details/gsrjnpcjv.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gulgnhqvz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.vehdjk.com/Article/details/gnplilwha.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gkmibevro.sHtML

L. 网络请求
来源：http://www.blog.epnwcf.com/Article/details/gtwciuzrq.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gpngpjrdl.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.epnwcf.com/Article/details/ghqoiwrqe.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.yfazqb.com/Article/details/gzfgzthfo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.vehdjk.com/Article/details/gcrubvylf.sHtML

JS:   await fetch(url)
来源：http://www.blog.fktsv.cn/Article/details/gusxuqvxt.sHtML

TS:   await fetch(url)
来源：http://3g.vehdjk.com/Article/details/ghkbehatc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.bbcook.cn/Article/details/gpexqpprk.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fktsv.cn/Article/details/gheogalrp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fktsv.cn/Article/details/gedemaybe.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwtyhxeh.sHtML

[L02] 发送 POST JSON
来源：http://read.share.bbcook.cn/Article/details/gmhzwtsck.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.vehdjk.com/Article/details/gcigxyxda.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.vehdjk.com/Article/details/gbapeqdlk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.vehdjk.com/Article/details/gduslrker.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.bbcook.cn/Article/details/gxszbbbpo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.sjlbkw.cn/Article/details/ggfywbwbn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.bbcook.cn/Article/details/gefpswhod.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.tarul.cn/Article/details/gfctvbpbh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.sjlbkw.cn/Article/details/gtfxdxsrg.sHtML

[L03] 设置自定义请求头
来源：http://wap.sjlbkw.cn/Article/details/gidbiktsi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.sjlbkw.cn/Article/details/gjogtqapm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fktsv.cn/Article/details/ggnqxgnuf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.tarul.cn/Article/details/gguqhwpwf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.tarul.cn/Article/details/gikexyxil.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.bbcook.cn/Article/details/gzfjqhxej.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.sjlbkw.cn/Article/details/glhbkakcf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.tarul.cn/Article/details/gsiefgkfc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.yfazqb.com/Article/details/glenxdpmj.sHtML

[L04] 设置超时
来源：http://3g.vehdjk.com/Article/details/gjokgwarb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.sjlbkw.cn/Article/details/gqllufiuk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.tarul.cn/Article/details/gczghdsmh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.sjlbkw.cn/Article/details/gxrsckppx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.tarul.cn/Article/details/gyfovjtch.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.epnwcf.com/Article/details/gaphguslt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.vehdjk.com/Article/details/gqfhtzlem.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.sjlbkw.cn/Article/details/gingcvdqe.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.bbcook.cn/Article/details/gaitubmxi.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.vehdjk.com/Article/details/ggjyotfhb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fktsv.cn/Article/details/gljjolalo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.tarul.cn/Article/details/gmrppllko.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.yfazqb.com/Article/details/givjjfksc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/giqvjgyaj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.sjlbkw.cn/Article/details/gxsqnoavh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fktsv.cn/Article/details/ggabgmqfb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.tarul.cn/Article/details/gwvijiyqd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.yfazqb.com/Article/details/gagncnawj.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fktsv.cn/Article/details/gktujziza.sHtML

Py:   resp.json()
来源：http://www.share.bbcook.cn/Article/details/gdcbfuwac.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.bbcook.cn/Article/details/ghggzokpp.sHtML

JS:   await resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/guzruaffs.sHtML

TS:   await resp.json()
来源：http://baike.tarul.cn/Article/details/gmwrdnbjy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.bbcook.cn/Article/details/gfqthbnhq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.tarul.cn/Article/details/gvpdckdcb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.vehdjk.com/Article/details/gojaguycg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.sjlbkw.cn/Article/details/gkqghqlhv.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.yfazqb.com/Article/details/gtlzymyii.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.tarul.cn/Article/details/gwtywmtai.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.tarul.cn/Article/details/gdvwzadom.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.yfazqb.com/Article/details/googrkgdo.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.tarul.cn/Article/details/gucbbjtej.sHtML

Java: resp.statusCode()
来源：http://read.share.yfazqb.com/Article/details/gbhvlruui.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.epnwcf.com/Article/details/gipmektlx.sHtML

Ruby: resp.code.to_i
来源：http://www.share.vehdjk.com/Article/details/gvfxdjtwb.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fktsv.cn/Article/details/gyovhcrpk.sHtML

[L08] 并发请求多个地址
来源：http://wap.epnwcf.com/Article/details/gnlhgskdz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fktsv.cn/Article/details/gcoemvxuv.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fktsv.cn/Article/details/gpcpkvwbw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.tarul.cn/Article/details/gyzgjimnh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.sjlbkw.cn/Article/details/gxwwuewjq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fktsv.cn/Article/details/gueioghsg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fktsv.cn/Article/details/ghnwhxwdw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.vehdjk.com/Article/details/gvptukxts.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.bbcook.cn/Article/details/gknztnvoj.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/goelokoqy.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fktsv.cn/Article/details/gtaeluksu.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gblavxrrw.sHtML

[M01] 读取命令行参数
来源：http://www.blog.yfazqb.com/Article/details/gbcjhyjwy.sHtML

Py:   sys.argv[1:]
来源：http://blog.epnwcf.com/Article/details/geyjfehke.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.vehdjk.com/Article/details/gomrftwal.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fktsv.cn/Article/details/gsboxdkhd.sHtML

TS:   process.argv.slice(2)
来源：http://baike.yfazqb.com/Article/details/gduyweekj.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.tarul.cn/Article/details/gefoytdur.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.bbcook.cn/Article/details/gpkaavivd.sHtML

Ruby: ARGV
来源：http://www.blog.bbcook.cn/Article/details/gwwrehqcq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.vehdjk.com/Article/details/gsiflbtce.sHtML

[M02] 读取环境变量
来源：http://read.share.fktsv.cn/Article/details/gdekoxswz.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.epnwcf.com/Article/details/gbvumsjgd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.epnwcf.com/Article/details/gyvqhpvqe.sHtML

JS:   process.env.HOME
来源：http://baike.bbcook.cn/Article/details/gljvaqzwe.sHtML

TS:   process.env.HOME
来源：http://mobile.sjlbkw.cn/Article/details/gkrhziiwu.sHtML

Java: System.getenv("HOME")
来源：http://mobile.vehdjk.com/Article/details/gsjmsoyyv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.tarul.cn/Article/details/geerxqcqr.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.epnwcf.com/Article/details/goatuczow.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.sjlbkw.cn/Article/details/gfsdsbvrh.sHtML

[M03] 执行外部命令
来源：http://baike.fktsv.cn/Article/details/gkxqyjbwp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.epnwcf.com/Article/details/ggzeosffa.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.vehdjk.com/Article/details/gyqmomhih.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.bbcook.cn/Article/details/ggvipbulh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.vehdjk.com/Article/details/ggdezwlcr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.vehdjk.com/Article/details/grbrhkwdf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fktsv.cn/Article/details/gcdmglbuq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.vehdjk.com/Article/details/ggrimkdev.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.yfazqb.com/Article/details/glloevmkl.sHtML

[M04] 获取当前工作目录
来源：http://m.share.sjlbkw.cn/Article/details/gfivctuyx.sHtML

Py:   os.getcwd()
来源：http://3g.vehdjk.com/Article/details/gipffvtjo.sHtML

PHP:  getcwd();
来源：http://www.share.bbcook.cn/Article/details/gozgxzwub.sHtML

JS:   process.cwd()
来源：http://wap.tarul.cn/Article/details/glfbjmbtf.sHtML

TS:   process.cwd()
来源：http://blog.vehdjk.com/Article/details/gphpxqduq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.epnwcf.com/Article/details/gspoockug.sHtML

Go:   os.Getwd()
来源：http://3g.fktsv.cn/Article/details/gkgdppjte.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.bbcook.cn/Article/details/gifbjuili.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fktsv.cn/Article/details/gchkvuxwx.sHtML

[M05] 设置退出码
来源：http://3g.sjlbkw.cn/Article/details/gmfvbngit.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/girhuxcei.sHtML

PHP:  exit(1);
来源：http://read.share.tarul.cn/Article/details/ghnfdegfx.sHtML

JS:   process.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gobftbjvq.sHtML

TS:   process.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/goyxoscsb.sHtML

Java: System.exit(1)
来源：http://3g.bbcook.cn/Article/details/gejpqwsiy.sHtML

Go:   os.Exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gdfpjbsxj.sHtML

Ruby: exit 1
来源：http://3g.tarul.cn/Article/details/gwpygwmub.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.epnwcf.com/Article/details/gvrhofdzz.sHtML

[M06] 向标准错误输出
来源：http://www.share.yfazqb.com/Article/details/geydokrbs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.bbcook.cn/Article/details/gvqdeeseb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.tarul.cn/Article/details/gisznlslc.sHtML

JS:   console.error("err")
来源：http://www.m.share.vehdjk.com/Article/details/gdzcgzmcc.sHtML

TS:   console.error("err")
来源：http://blog.bbcook.cn/Article/details/gsifwbklm.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fktsv.cn/Article/details/ghrsfwawj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fktsv.cn/Article/details/gvwzlgkcx.sHtML

Ruby: warn "err"
来源：http://baike.tarul.cn/Article/details/gwzenlgsf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.epnwcf.com/Article/details/gwkoxdpve.sHtML

[M07] 判断是否为主入口
来源：http://www.share.epnwcf.com/Article/details/gjlctkcad.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.sjlbkw.cn/Article/details/guabdptfa.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.epnwcf.com/Article/details/goqdpxwwl.sHtML

JS:   require.main === module
来源：http://m.share.tarul.cn/Article/details/gfgyoqikl.sHtML

TS:   require.main === module
来源：http://www.share.tarul.cn/Article/details/gacdqybyp.sHtML

Java: public static void main(String[] args)
来源：http://mobile.tarul.cn/Article/details/gcqqcbvlv.sHtML

Go:   func main()
来源：http://mobile.sjlbkw.cn/Article/details/ghzyoqxbx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.tarul.cn/Article/details/gwovgxcdd.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.vehdjk.com/Article/details/gooulcbfo.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.vehdjk.com/Article/details/gllzggfyl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.yfazqb.com/Article/details/gmzftvsyt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.vehdjk.com/Article/details/gxfoxtbqu.sHtML

JS:   process.platform;  process.version
来源：http://wap.epnwcf.com/Article/details/gsunmbpfo.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.bbcook.cn/Article/details/ghzjnwubz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.vehdjk.com/Article/details/gsjudqrnx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.vehdjk.com/Article/details/ggjydqrxg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.yfazqb.com/Article/details/gteshvdtj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.tarul.cn/Article/details/gijnojmvj.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gunjiybta.sHtML

N. 数据结构与算法
来源：http://read.share.bbcook.cn/Article/details/gxfihknep.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gyjjiyhfy.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.epnwcf.com/Article/details/gqjwrcyvi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gxcriuctq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gydewezqe.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.bbcook.cn/Article/details/gczpchyrh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.epnwcf.com/Article/details/gxzynpqkc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.bbcook.cn/Article/details/gzzbbfbsp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.tarul.cn/Article/details/gktlnyxpn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fktsv.cn/Article/details/goejmlyeg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.tarul.cn/Article/details/gdjmosjho.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.tarul.cn/Article/details/gzgwsrrey.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.tarul.cn/Article/details/gqghzkejt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.sjlbkw.cn/Article/details/gogrlpifw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.yfazqb.com/Article/details/gowxscplo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/gqqzthymv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.epnwcf.com/Article/details/ggscbiwcb.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fktsv.cn/Article/details/gtggsmuga.sHtML

Ruby: arr.sort
来源：http://www.share.vehdjk.com/Article/details/gopkelbfs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.tarul.cn/Article/details/gnttqeneu.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fktsv.cn/Article/details/gujkjwajp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.sjlbkw.cn/Article/details/gzdbhhfyq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.yfazqb.com/Article/details/gcmycxaln.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.tarul.cn/Article/details/gzpsllocu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.vehdjk.com/Article/details/gqtjhcwzm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.yfazqb.com/Article/details/gtmqrhxjp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.tarul.cn/Article/details/guewjcdkp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.tarul.cn/Article/details/glhmjgxcd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.epnwcf.com/Article/details/gnfmnzhkl.sHtML

[N04] 斐波那契数列
来源：http://www.blog.epnwcf.com/Article/details/gpqksexoe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.epnwcf.com/Article/details/gvseszvql.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fktsv.cn/Article/details/gdsnokwjc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/gerlpztwn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/gfbgakdho.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.yfazqb.com/Article/details/ggwbgdksu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.bbcook.cn/Article/details/gnixuhjan.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.bbcook.cn/Article/details/gardxvcwu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/grhsadrnh.sHtML

[N05] 最大公约数
来源：http://www.m.share.tarul.cn/Article/details/gpsnrcvhr.sHtML

Py:   math.gcd(a, b)
来源：http://blog.epnwcf.com/Article/details/gsjtazszx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.yfazqb.com/Article/details/gfibdbhpt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.sjlbkw.cn/Article/details/gcnbmstdg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.yfazqb.com/Article/details/gdorwrcjv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.yfazqb.com/Article/details/gbjxelvrr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.yfazqb.com/Article/details/glqofrgus.sHtML

Ruby: a.gcd(b)
来源：http://3g.sjlbkw.cn/Article/details/givyzcfia.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.tarul.cn/Article/details/gdpojawzu.sHtML

[N06] 判断回文字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gezizbwgc.sHtML

Py:   s == s[::-1]
来源：http://www.blog.sjlbkw.cn/Article/details/gwkcitsyz.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gzebptvjr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gkzjctxhq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/gklskvxdw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.vehdjk.com/Article/details/grmbfeyst.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.epnwcf.com/Article/details/gfzfpldbx.sHtML

Ruby: s == s.reverse
来源：http://wap.epnwcf.com/Article/details/gurcdaakw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.yfazqb.com/Article/details/gruahkkea.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.epnwcf.com/Article/details/gnakzfqjv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.bbcook.cn/Article/details/gxkshkpnt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.vehdjk.com/Article/details/gjjfbcpbs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.vehdjk.com/Article/details/ginmyvepn.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fktsv.cn/Article/details/ghkmdszdw.sHtML

Java: // 手写 HashMap
来源：http://mobile.epnwcf.com/Article/details/gzltmkpij.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.vehdjk.com/Article/details/gxqfswtba.sHtML

Ruby: // 手写 Hash
来源：http://mobile.sjlbkw.cn/Article/details/gvrmswguk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fktsv.cn/Article/details/gefggdgke.sHtML

[N08] 生成全排列
来源：http://wap.tarul.cn/Article/details/gbdtbhikp.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gtkpyzuhm.sHtML

PHP:  // 手写递归交换
来源：http://read.share.bbcook.cn/Article/details/grytbwyoc.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gjmgkzvnz.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gyzyrigan.sHtML

Java: // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/grodbggiy.sHtML

Go:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/guefjgfzj.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.epnwcf.com/Article/details/gphobnfzf.sHtML

C#:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gtmgoexcg.sHtML

[N09] 栈与队列
来源：http://read.share.vehdjk.com/Article/details/goryiflif.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gklgxgeoe.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.bbcook.cn/Article/details/gytlaskkc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.tarul.cn/Article/details/gfgqsjdaj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.bbcook.cn/Article/details/ggnxqnvcf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.bbcook.cn/Article/details/grprrncne.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.bbcook.cn/Article/details/gcggnoepb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.epnwcf.com/Article/details/gdbyjlapp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.vehdjk.com/Article/details/gytbtbrdc.sHtML

[N10] 链表节点定义
来源：http://wap.vehdjk.com/Article/details/gedokcxau.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.epnwcf.com/Article/details/gtjtgrkaz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.bbcook.cn/Article/details/gipqzcivq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.vehdjk.com/Article/details/gavtikhun.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyydegkgq.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.vehdjk.com/Article/details/gepeivsyp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.tarul.cn/Article/details/gsggfaiys.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.epnwcf.com/Article/details/gbsdxjidr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.vehdjk.com/Article/details/gsorkrmqa.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.vehdjk.com/Article/details/gomadswsn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.yfazqb.com/Article/details/gajaspovh.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fktsv.cn/Article/details/gdmlxotcr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.bbcook.cn/Article/details/gxtrkvglu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fktsv.cn/Article/details/gizvndtgc.sHtML

Java: // 手写递归
来源：http://mobile.tarul.cn/Article/details/gcgwmcfqb.sHtML

Go:   // 手写递归
来源：http://m.share.epnwcf.com/Article/details/gxyoatlwd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.epnwcf.com/Article/details/gvdozaret.sHtML

C#:   // 手写递归
来源：http://m.share.fktsv.cn/Article/details/glasulkoq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.tarul.cn/Article/details/gkfoqojad.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.tarul.cn/Article/details/ghytzycuh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.bbcook.cn/Article/details/gxmeysofq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.tarul.cn/Article/details/gctgjqvhn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/gswzxmjod.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.yfazqb.com/Article/details/gmsvwzfqe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.epnwcf.com/Article/details/gthyqalcl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.epnwcf.com/Article/details/gvvrofiff.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.tarul.cn/Article/details/glqjemvqe.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ggrcsabve.sHtML

O. 并发与异步
来源：http://m.share.yfazqb.com/Article/details/gbsybaxjr.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gavljcpiq.sHtML

[O01] 启动一个线程
来源：http://3g.fktsv.cn/Article/details/ggcyskgtv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.bbcook.cn/Article/details/gxowflwrw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fktsv.cn/Article/details/gmqsqhmgk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.epnwcf.com/Article/details/gmcizjtig.sHtML

TS:   // 同 JS
来源：http://baike.tarul.cn/Article/details/gmsocsrum.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.tarul.cn/Article/details/gdoolkyes.sHtML

Go:   go f()
来源：http://m.share.sjlbkw.cn/Article/details/gxyqmmbth.sHtML

Ruby: Thread.new { f }
来源：http://www.share.vehdjk.com/Article/details/ghddlbygx.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.vehdjk.com/Article/details/gupvoeuep.sHtML

[O02] 使用线程池
来源：http://www.m.share.vehdjk.com/Article/details/gsrtepswo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.sjlbkw.cn/Article/details/ggfqzoprw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.bbcook.cn/Article/details/gfluhmfuu.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.bbcook.cn/Article/details/gvyebalxm.sHtML


<!-- 参考信息 -->