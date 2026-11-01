代发 wailian999

[K06] 解析 URL 查询串
来源：http://m.share.epnwcf.com/Article/details/gwmqmhbpm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.epnwcf.com/Article/details/glhnhjttj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fktsv.cn/Article/details/ggseymhri.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.vehdjk.com/Article/details/gnhxcdjgr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fktsv.cn/Article/details/gpwevbchp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.bbcook.cn/Article/details/gpdfpfkoa.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.vehdjk.com/Article/details/ghqfzjvbl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.epnwcf.com/Article/details/gipgssapf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.sjlbkw.cn/Article/details/gwiawiexq.sHtML

[K07] 进制转换
来源：http://3g.tarul.cn/Article/details/guzjyzlpr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gnjlymjaa.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.epnwcf.com/Article/details/gbgvsqdtq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/galepecdz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/grjmhjhcc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/ggpdzqzyv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fktsv.cn/Article/details/ggytdhcst.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.epnwcf.com/Article/details/gmomeqycw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.epnwcf.com/Article/details/goyjnbaxv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.vehdjk.com/Article/details/goziflcxx.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.bbcook.cn/Article/details/gslbzgrwq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.tarul.cn/Article/details/gqbaufxzu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.yfazqb.com/Article/details/gaicqvtzk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.vehdjk.com/Article/details/gtxxistxv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fktsv.cn/Article/details/gyfibkpbp.sHtML

Go:   encoding/gob
来源：http://read.share.sjlbkw.cn/Article/details/gawgjlubg.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.vehdjk.com/Article/details/gtsrszggz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.vehdjk.com/Article/details/gxgmfyygs.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gtvorlfjr.sHtML

L. 网络请求
来源：http://www.share.epnwcf.com/Article/details/gaklkjlqu.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gmhwaosfj.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.epnwcf.com/Article/details/gdlpcesrq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.sjlbkw.cn/Article/details/gncwcyfou.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.sjlbkw.cn/Article/details/gzujuevnu.sHtML

JS:   await fetch(url)
来源：http://blog.epnwcf.com/Article/details/grzfmcwnd.sHtML

TS:   await fetch(url)
来源：http://baike.bbcook.cn/Article/details/gimgimzof.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.bbcook.cn/Article/details/gipfephsq.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.bbcook.cn/Article/details/gmenmlitb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.tarul.cn/Article/details/gntzzvrca.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.yfazqb.com/Article/details/gdfduifuq.sHtML

[L02] 发送 POST JSON
来源：http://read.share.tarul.cn/Article/details/gfqnomimv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.sjlbkw.cn/Article/details/gukqzopkq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fktsv.cn/Article/details/gffoojhqs.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.vehdjk.com/Article/details/gpakpralr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.tarul.cn/Article/details/gmuimufdm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fktsv.cn/Article/details/govzoneyl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.vehdjk.com/Article/details/gmkzvgxbd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.sjlbkw.cn/Article/details/gnmzgiilp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.vehdjk.com/Article/details/gbhtsdnys.sHtML

[L03] 设置自定义请求头
来源：http://m.share.vehdjk.com/Article/details/ghpmhhmsp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.bbcook.cn/Article/details/gjumparwr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fktsv.cn/Article/details/gyipbcxar.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.tarul.cn/Article/details/gjcgrsgly.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.tarul.cn/Article/details/gpsiagoso.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.yfazqb.com/Article/details/gqkphznrc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.bbcook.cn/Article/details/gwrpcvnzf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.bbcook.cn/Article/details/gtgbzsxsd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.tarul.cn/Article/details/gmsuijeip.sHtML

[L04] 设置超时
来源：http://mobile.fktsv.cn/Article/details/gctuouurn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.sjlbkw.cn/Article/details/gjlhexarm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.epnwcf.com/Article/details/gteoxqsht.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.vehdjk.com/Article/details/gulzqrfea.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.tarul.cn/Article/details/gzyuyjidc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.bbcook.cn/Article/details/gfdrqhayf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.bbcook.cn/Article/details/gzaadiqci.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.tarul.cn/Article/details/gscesfvjv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.bbcook.cn/Article/details/gdtvkziyt.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.tarul.cn/Article/details/grusjqnev.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.vehdjk.com/Article/details/ghjnjslmb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.sjlbkw.cn/Article/details/gmdzsfkcf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/gizucaigm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.yfazqb.com/Article/details/gcztclbsw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.tarul.cn/Article/details/geqzgsqjd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.yfazqb.com/Article/details/gbbrvihgg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.sjlbkw.cn/Article/details/gcomkateg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.yfazqb.com/Article/details/ghrdrkjtn.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.tarul.cn/Article/details/gzgcovplf.sHtML

Py:   resp.json()
来源：http://blog.fktsv.cn/Article/details/gxmsutmar.sHtML

PHP:  json_decode($body, true);
来源：http://blog.bbcook.cn/Article/details/gpyigpkmm.sHtML

JS:   await resp.json()
来源：http://blog.epnwcf.com/Article/details/gcjodoanp.sHtML

TS:   await resp.json()
来源：http://www.share.tarul.cn/Article/details/ggxholhyc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.epnwcf.com/Article/details/gsokeduii.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.yfazqb.com/Article/details/gnqskqypq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.tarul.cn/Article/details/ghzfyqpvy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.epnwcf.com/Article/details/goxxzosmw.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.tarul.cn/Article/details/gcourzhbv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.yfazqb.com/Article/details/giwpuclfj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.tarul.cn/Article/details/gcnunybfz.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fktsv.cn/Article/details/gxnogdfqq.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.vehdjk.com/Article/details/glgepkftp.sHtML

Java: resp.statusCode()
来源：http://m.share.yfazqb.com/Article/details/gpwypjfoi.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.epnwcf.com/Article/details/gtbvyrgpq.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.epnwcf.com/Article/details/gpadfurti.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fktsv.cn/Article/details/grpuigzfe.sHtML

[L08] 并发请求多个地址
来源：http://mobile.tarul.cn/Article/details/gvlhrushi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.yfazqb.com/Article/details/gpymllrim.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.bbcook.cn/Article/details/ggotqxhnv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gsywgsjdu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.tarul.cn/Article/details/gqthwzdzw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.sjlbkw.cn/Article/details/gsxkmlgom.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.vehdjk.com/Article/details/guekdymgq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.tarul.cn/Article/details/gdtkurdhp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fktsv.cn/Article/details/gfhuwawib.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/galtsaauy.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.yfazqb.com/Article/details/gqialeeow.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gtlzeautg.sHtML

[M01] 读取命令行参数
来源：http://baike.epnwcf.com/Article/details/gmxrrmbku.sHtML

Py:   sys.argv[1:]
来源：http://read.share.yfazqb.com/Article/details/gezyruvng.sHtML

PHP:  $argv;  $argc;
来源：http://baike.tarul.cn/Article/details/gnankdfpg.sHtML

JS:   process.argv.slice(2)
来源：http://3g.tarul.cn/Article/details/gbruejnhe.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.yfazqb.com/Article/details/gnykymdsf.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fktsv.cn/Article/details/gsdqouknz.sHtML

Go:   os.Args[1:]
来源：http://wap.fktsv.cn/Article/details/gsizasdeq.sHtML

Ruby: ARGV
来源：http://blog.sjlbkw.cn/Article/details/gopmscaid.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.bbcook.cn/Article/details/gpcbmnpzh.sHtML

[M02] 读取环境变量
来源：http://www.share.vehdjk.com/Article/details/giqoikgdd.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gstdtklcz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.sjlbkw.cn/Article/details/gwrcosbaj.sHtML

JS:   process.env.HOME
来源：http://wap.epnwcf.com/Article/details/gqfyvcxxt.sHtML

TS:   process.env.HOME
来源：http://wap.fktsv.cn/Article/details/gihbupjqb.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fktsv.cn/Article/details/gxwhyofng.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.vehdjk.com/Article/details/gewwcbzde.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.epnwcf.com/Article/details/gvfikpsbc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.yfazqb.com/Article/details/gtdwlknwu.sHtML

[M03] 执行外部命令
来源：http://m.share.tarul.cn/Article/details/ggyizxxlt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.tarul.cn/Article/details/gabxdhoss.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.vehdjk.com/Article/details/gmichbgan.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.yfazqb.com/Article/details/gmpsflmsk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/gslmzidsa.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.tarul.cn/Article/details/ggmntvfuo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.sjlbkw.cn/Article/details/gcqgdyjjj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.yfazqb.com/Article/details/gldavzufh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.bbcook.cn/Article/details/gbcgoidke.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.tarul.cn/Article/details/gflskgbrs.sHtML

Py:   os.getcwd()
来源：http://baike.tarul.cn/Article/details/gqhsslzyj.sHtML

PHP:  getcwd();
来源：http://www.blog.epnwcf.com/Article/details/griwlxtjq.sHtML

JS:   process.cwd()
来源：http://wap.vehdjk.com/Article/details/gcvadampc.sHtML

TS:   process.cwd()
来源：http://www.share.tarul.cn/Article/details/gvevfcmyr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.sjlbkw.cn/Article/details/gbhmnprgq.sHtML

Go:   os.Getwd()
来源：http://blog.tarul.cn/Article/details/gkgqldmol.sHtML

Ruby: Dir.pwd
来源：http://blog.sjlbkw.cn/Article/details/gxletdzkp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.epnwcf.com/Article/details/gkywmxecd.sHtML

[M05] 设置退出码
来源：http://blog.epnwcf.com/Article/details/gxbhizuwy.sHtML

Py:   sys.exit(1)
来源：http://3g.vehdjk.com/Article/details/gnomxgcxx.sHtML

PHP:  exit(1);
来源：http://www.blog.bbcook.cn/Article/details/gufhcvvwp.sHtML

JS:   process.exit(1)
来源：http://3g.tarul.cn/Article/details/goiqhjhcb.sHtML

TS:   process.exit(1)
来源：http://blog.vehdjk.com/Article/details/ghamgeepq.sHtML

Java: System.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gveblzvfy.sHtML

Go:   os.Exit(1)
来源：http://wap.fktsv.cn/Article/details/gmecfbtqe.sHtML

Ruby: exit 1
来源：http://www.m.share.vehdjk.com/Article/details/gznduvjzy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.epnwcf.com/Article/details/gyarffidp.sHtML

[M06] 向标准错误输出
来源：http://read.share.fktsv.cn/Article/details/gbgbmitxz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.vehdjk.com/Article/details/ggjlgzqwe.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.vehdjk.com/Article/details/gghcdnzdc.sHtML

JS:   console.error("err")
来源：http://mobile.sjlbkw.cn/Article/details/gymfcuank.sHtML

TS:   console.error("err")
来源：http://www.m.share.tarul.cn/Article/details/ghmvycmwn.sHtML

Java: System.err.println("err")
来源：http://baike.tarul.cn/Article/details/gnqsmuwjy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.yfazqb.com/Article/details/gvrnqkylh.sHtML

Ruby: warn "err"
来源：http://m.share.vehdjk.com/Article/details/gyplghitd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.sjlbkw.cn/Article/details/goutcqslx.sHtML

[M07] 判断是否为主入口
来源：http://blog.bbcook.cn/Article/details/gbyhmceqi.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.yfazqb.com/Article/details/gupmomdlh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.sjlbkw.cn/Article/details/gkgoaefaj.sHtML

JS:   require.main === module
来源：http://3g.epnwcf.com/Article/details/gnizvjbou.sHtML

TS:   require.main === module
来源：http://m.share.bbcook.cn/Article/details/gjfzjxzkn.sHtML

Java: public static void main(String[] args)
来源：http://read.share.tarul.cn/Article/details/gyinglgne.sHtML

Go:   func main()
来源：http://blog.tarul.cn/Article/details/gxiqdtgxp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fktsv.cn/Article/details/gnbpwspab.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.bbcook.cn/Article/details/gxsxqzrqi.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.sjlbkw.cn/Article/details/giemtbxyi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.epnwcf.com/Article/details/gnaxcvqyv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.epnwcf.com/Article/details/gbkxhjhqr.sHtML

JS:   process.platform;  process.version
来源：http://baike.vehdjk.com/Article/details/gtshydbzs.sHtML

TS:   process.platform;  process.version
来源：http://www.share.epnwcf.com/Article/details/gtlazriup.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.yfazqb.com/Article/details/gfhcaufto.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fktsv.cn/Article/details/gknpbvqfd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.tarul.cn/Article/details/gzwxdhczk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.vehdjk.com/Article/details/geeqirgrk.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gqblnpvwi.sHtML

N. 数据结构与算法
来源：http://m.share.epnwcf.com/Article/details/gfcqaiucv.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gabtjcaye.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.vehdjk.com/Article/details/gjyismqmz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gqonugiap.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fktsv.cn/Article/details/guqpqjhqb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/gqynopzvh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.tarul.cn/Article/details/ghxvctpuo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.vehdjk.com/Article/details/gvlxiqpsh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.bbcook.cn/Article/details/gfhcqlinu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.tarul.cn/Article/details/glryfkktv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.epnwcf.com/Article/details/gjucalkym.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fktsv.cn/Article/details/gbjctufdn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.tarul.cn/Article/details/grukhjroc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.tarul.cn/Article/details/gdhqfsicn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fktsv.cn/Article/details/gailevhhs.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/gnthzrgik.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.bbcook.cn/Article/details/gpsexaldr.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.epnwcf.com/Article/details/gyaeqtftt.sHtML

Ruby: arr.sort
来源：http://read.share.sjlbkw.cn/Article/details/gtexfkgsq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.epnwcf.com/Article/details/gwyeotyxt.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fktsv.cn/Article/details/glbpshpjx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.bbcook.cn/Article/details/gbynregwk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.bbcook.cn/Article/details/gqryujuhm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.vehdjk.com/Article/details/gdlbkkjus.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.epnwcf.com/Article/details/gyndswmlz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.tarul.cn/Article/details/gqpeyotob.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fktsv.cn/Article/details/gmgteqiiq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.tarul.cn/Article/details/gdujjgvnq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.sjlbkw.cn/Article/details/gvbolkdnc.sHtML

[N04] 斐波那契数列
来源：http://baike.sjlbkw.cn/Article/details/gmapmkqkc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.tarul.cn/Article/details/grivdnrvy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.sjlbkw.cn/Article/details/ggbjnlhmz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/guyayiapr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.vehdjk.com/Article/details/gfdukbtan.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.vehdjk.com/Article/details/gxxlsrjdt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.vehdjk.com/Article/details/gcjawrpyp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fktsv.cn/Article/details/geyarvisg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.bbcook.cn/Article/details/gzwzagazt.sHtML

[N05] 最大公约数
来源：http://baike.fktsv.cn/Article/details/gysofepks.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.yfazqb.com/Article/details/gviyhirax.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.bbcook.cn/Article/details/gjsrlavew.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.tarul.cn/Article/details/ghqhoxywg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.tarul.cn/Article/details/gootkuhpb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.yfazqb.com/Article/details/gjjvuwypg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.sjlbkw.cn/Article/details/gsqbfpfvt.sHtML

Ruby: a.gcd(b)
来源：http://www.share.vehdjk.com/Article/details/guxnbqddr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.epnwcf.com/Article/details/galgiaafz.sHtML

[N06] 判断回文字符串
来源：http://www.blog.vehdjk.com/Article/details/gorxcwajt.sHtML

Py:   s == s[::-1]
来源：http://blog.fktsv.cn/Article/details/gdtpoopac.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.vehdjk.com/Article/details/ghsklgzgb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gxrrbtcdt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/gtlkxmggs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.bbcook.cn/Article/details/gqxzxomkd.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fktsv.cn/Article/details/gmxkyzaqn.sHtML

Ruby: s == s.reverse
来源：http://www.share.epnwcf.com/Article/details/gnliswguo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fktsv.cn/Article/details/gbucgigao.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.epnwcf.com/Article/details/gturvunlb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.bbcook.cn/Article/details/gljsdhmds.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.epnwcf.com/Article/details/gmtqxidzq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fktsv.cn/Article/details/gvcecbbqc.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.sjlbkw.cn/Article/details/gruxfvwri.sHtML

Java: // 手写 HashMap
来源：http://m.share.vehdjk.com/Article/details/gcbjajadu.sHtML

Go:   // 手写 map[int]int
来源：http://baike.sjlbkw.cn/Article/details/gfytcqrlv.sHtML

Ruby: // 手写 Hash
来源：http://m.share.epnwcf.com/Article/details/gcbwyjmtf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.vehdjk.com/Article/details/gqfxreubt.sHtML

[N08] 生成全排列
来源：http://www.share.sjlbkw.cn/Article/details/gdtnaatzy.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.tarul.cn/Article/details/gjmwcoylf.sHtML

PHP:  // 手写递归交换
来源：http://wap.vehdjk.com/Article/details/gxjeulpyb.sHtML

JS:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/grsditdqg.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gizpfuacg.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/grmjyxogt.sHtML

Go:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gstxyqepq.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fktsv.cn/Article/details/gytrfbbcy.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/glpesoovq.sHtML

[N09] 栈与队列
来源：http://wap.fktsv.cn/Article/details/gorjyufur.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.vehdjk.com/Article/details/gqrpxtyij.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/ggxkrussp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.bbcook.cn/Article/details/gzodqgbmr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fktsv.cn/Article/details/gnkpyfpcw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.bbcook.cn/Article/details/gblkkxoob.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.yfazqb.com/Article/details/gjutdjiku.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.vehdjk.com/Article/details/ghyaebhlc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.vehdjk.com/Article/details/gejxzqttq.sHtML

[N10] 链表节点定义
来源：http://www.share.tarul.cn/Article/details/grzcnzidk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fktsv.cn/Article/details/gfgscqhrv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.tarul.cn/Article/details/ggxtmpugq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.bbcook.cn/Article/details/gukuirfkw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.yfazqb.com/Article/details/gtiwlozsx.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fktsv.cn/Article/details/gaqvmsrhd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.tarul.cn/Article/details/gdfaxjbou.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.vehdjk.com/Article/details/gkigekgua.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fktsv.cn/Article/details/gotpeygvu.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fktsv.cn/Article/details/gpokbfyvg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.bbcook.cn/Article/details/gmerbsllh.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fktsv.cn/Article/details/gmmnyatxi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.sjlbkw.cn/Article/details/golaipcxf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.sjlbkw.cn/Article/details/gejadepzu.sHtML

Java: // 手写递归
来源：http://www.share.sjlbkw.cn/Article/details/gisjpbqwv.sHtML

Go:   // 手写递归
来源：http://baike.bbcook.cn/Article/details/gneavtusj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.epnwcf.com/Article/details/gsdzxnkgk.sHtML

C#:   // 手写递归
来源：http://mobile.epnwcf.com/Article/details/gxzrfunfu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.yfazqb.com/Article/details/gkcptwreh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fktsv.cn/Article/details/gihehdwhj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fktsv.cn/Article/details/gtpmxaoym.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.sjlbkw.cn/Article/details/gdlhwnjxi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.vehdjk.com/Article/details/ghittgxwc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.tarul.cn/Article/details/gmwpeysjz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.bbcook.cn/Article/details/gbpddynfq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.yfazqb.com/Article/details/guuedrosv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.tarul.cn/Article/details/gnmywcggb.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gjwnzjnre.sHtML

O. 并发与异步
来源：http://baike.epnwcf.com/Article/details/glwqeuexk.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gnciyajzi.sHtML

[O01] 启动一个线程
来源：http://m.share.tarul.cn/Article/details/gzbkaeodf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.epnwcf.com/Article/details/gorvnbubx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.bbcook.cn/Article/details/ghdmrndju.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.epnwcf.com/Article/details/gjfbkixxl.sHtML

TS:   // 同 JS
来源：http://blog.sjlbkw.cn/Article/details/gdcixphrl.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.vehdjk.com/Article/details/gnfxwzmlb.sHtML

Go:   go f()
来源：http://read.share.bbcook.cn/Article/details/glumzhfjb.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fktsv.cn/Article/details/gvtcbsjzg.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.vehdjk.com/Article/details/gfedwfagv.sHtML


<!-- 参考信息 -->