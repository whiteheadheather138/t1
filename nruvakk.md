代发 wailian999

[K06] 解析 URL 查询串
来源：http://3g.sjlbkw.cn/Article/details/guakantnx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.bbcook.cn/Article/details/gnzomzavp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.epnwcf.com/Article/details/gwohhvqis.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.bbcook.cn/Article/details/grqphfoue.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.epnwcf.com/Article/details/gzqcxhsmw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.tarul.cn/Article/details/gvgzctmvh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/guoobauiy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/gdlhnkggh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/gphaignvk.sHtML

[K07] 进制转换
来源：http://read.share.bbcook.cn/Article/details/gdodzyysw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gwendieze.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fktsv.cn/Article/details/gwaltnmdg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/glvqmgtvf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gdpgdkvhy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gvwbavzfq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.epnwcf.com/Article/details/godkeuczz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.sjlbkw.cn/Article/details/gzamzngbk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gbgeffeis.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.sjlbkw.cn/Article/details/gkurnvxcy.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.vehdjk.com/Article/details/grsmiltxm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.bbcook.cn/Article/details/gaymbqsad.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fktsv.cn/Article/details/gacchbvnm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.yfazqb.com/Article/details/gxhhvauvi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.sjlbkw.cn/Article/details/gemdlgctl.sHtML

Go:   encoding/gob
来源：http://blog.bbcook.cn/Article/details/gucidsuyg.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.sjlbkw.cn/Article/details/glymsckck.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.epnwcf.com/Article/details/giiyopvxr.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gknfhahya.sHtML

L. 网络请求
来源：http://blog.fktsv.cn/Article/details/gtrmqkqty.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gllwxgctu.sHtML

[L01] 发送 GET 请求
来源：http://baike.bbcook.cn/Article/details/gpwffpzbk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.epnwcf.com/Article/details/gzqtsygrn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.tarul.cn/Article/details/gigqlwhjm.sHtML

JS:   await fetch(url)
来源：http://www.m.share.bbcook.cn/Article/details/grwkoqhrh.sHtML

TS:   await fetch(url)
来源：http://m.share.fktsv.cn/Article/details/glkgwaqas.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.vehdjk.com/Article/details/gdtplibzm.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.tarul.cn/Article/details/gajvvwlae.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.epnwcf.com/Article/details/gzpfackzy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.tarul.cn/Article/details/gwjqkfowe.sHtML

[L02] 发送 POST JSON
来源：http://blog.tarul.cn/Article/details/gofiuzzih.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.yfazqb.com/Article/details/gxlgwnnki.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.epnwcf.com/Article/details/gszstevvk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.bbcook.cn/Article/details/gbtgqiqqg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.tarul.cn/Article/details/gcfrgqcvv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fktsv.cn/Article/details/gkmhxlbas.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.epnwcf.com/Article/details/gipvgnpyl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.vehdjk.com/Article/details/gejhubljp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.yfazqb.com/Article/details/gritzxggu.sHtML

[L03] 设置自定义请求头
来源：http://www.share.tarul.cn/Article/details/gwnvrazed.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.bbcook.cn/Article/details/gujmwowgf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fktsv.cn/Article/details/gjmlxukoa.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.sjlbkw.cn/Article/details/glgklneqj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.sjlbkw.cn/Article/details/gxsrugwnn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.bbcook.cn/Article/details/gorqwfkbf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.tarul.cn/Article/details/gfuwzhpwp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.bbcook.cn/Article/details/gafodhjqu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fktsv.cn/Article/details/gcbvocemn.sHtML

[L04] 设置超时
来源：http://baike.sjlbkw.cn/Article/details/gwwzmihlz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.sjlbkw.cn/Article/details/grsnoehnf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fktsv.cn/Article/details/gpxomfbxd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.tarul.cn/Article/details/grprucnpo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.vehdjk.com/Article/details/gtdnyzzom.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.sjlbkw.cn/Article/details/gitupqjai.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.tarul.cn/Article/details/gufxqpyko.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.bbcook.cn/Article/details/gsrfuxjzi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.tarul.cn/Article/details/gdfklqqhv.sHtML

[L05] 上传文件（multipart）
来源：http://blog.yfazqb.com/Article/details/gejxtxxxb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.epnwcf.com/Article/details/gfkntighy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.bbcook.cn/Article/details/guwbwepqh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.vehdjk.com/Article/details/ghejkwwpb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.yfazqb.com/Article/details/gmzdxiwks.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.epnwcf.com/Article/details/gptzehtax.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.tarul.cn/Article/details/gpcrezwer.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.vehdjk.com/Article/details/gvtrjdjeu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.vehdjk.com/Article/details/gizoneqgx.sHtML

[L06] 解析响应为 JSON
来源：http://baike.yfazqb.com/Article/details/gyrockwua.sHtML

Py:   resp.json()
来源：http://3g.tarul.cn/Article/details/guhielcnu.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.yfazqb.com/Article/details/gtdbsvdql.sHtML

JS:   await resp.json()
来源：http://www.share.yfazqb.com/Article/details/gfrrmyypj.sHtML

TS:   await resp.json()
来源：http://read.share.vehdjk.com/Article/details/gldwlxwrc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.tarul.cn/Article/details/gijgwwggn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.tarul.cn/Article/details/gygkydxol.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvnerwkt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.bbcook.cn/Article/details/gdovbibfe.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.tarul.cn/Article/details/gwppgyodr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.epnwcf.com/Article/details/gjqnkgizd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fktsv.cn/Article/details/gsvlnkxwg.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.sjlbkw.cn/Article/details/gbaglibtr.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fktsv.cn/Article/details/gkostwjvv.sHtML

Java: resp.statusCode()
来源：http://baike.yfazqb.com/Article/details/grteqejuf.sHtML

Go:   resp.StatusCode
来源：http://www.share.tarul.cn/Article/details/gzzpgwerl.sHtML

Ruby: resp.code.to_i
来源：http://blog.sjlbkw.cn/Article/details/gqxjxrgyi.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.vehdjk.com/Article/details/gjyztwouh.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.sjlbkw.cn/Article/details/govgmuoeo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.sjlbkw.cn/Article/details/gygxyqmuq.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.bbcook.cn/Article/details/gvnnidbde.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.tarul.cn/Article/details/gkydlquve.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gkbwetjbu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.tarul.cn/Article/details/gzkyhkaxa.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.sjlbkw.cn/Article/details/geurhiqdz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.tarul.cn/Article/details/gthcgponf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.epnwcf.com/Article/details/gxnvjloac.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gnmstdpiy.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.epnwcf.com/Article/details/gcgaptnas.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gqovacjxw.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.epnwcf.com/Article/details/gfxxdbjdr.sHtML

Py:   sys.argv[1:]
来源：http://wap.yfazqb.com/Article/details/glosgshhq.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.yfazqb.com/Article/details/gicgwhtms.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.sjlbkw.cn/Article/details/ghbkgnahm.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.bbcook.cn/Article/details/gulxltmmv.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fktsv.cn/Article/details/ggnnwaqvl.sHtML

Go:   os.Args[1:]
来源：http://3g.vehdjk.com/Article/details/gxeqycaqk.sHtML

Ruby: ARGV
来源：http://baike.epnwcf.com/Article/details/gnnlpvojt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.sjlbkw.cn/Article/details/gsobxrsno.sHtML

[M02] 读取环境变量
来源：http://mobile.fktsv.cn/Article/details/gperwdpzh.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gaqpfcida.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.vehdjk.com/Article/details/gndszsmdi.sHtML

JS:   process.env.HOME
来源：http://mobile.sjlbkw.cn/Article/details/givbdyyji.sHtML

TS:   process.env.HOME
来源：http://baike.bbcook.cn/Article/details/gglqbttea.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gkijinken.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gbbnoumnu.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.tarul.cn/Article/details/gbxvgjdri.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.vehdjk.com/Article/details/gpfglwsbh.sHtML

[M03] 执行外部命令
来源：http://www.blog.sjlbkw.cn/Article/details/guafrnllm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.tarul.cn/Article/details/gvhzezpxm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.tarul.cn/Article/details/gkxpwntbh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.tarul.cn/Article/details/goukqoguw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.tarul.cn/Article/details/gkzwbctdi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.yfazqb.com/Article/details/giekvdfjf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.bbcook.cn/Article/details/gwalvrnlv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.tarul.cn/Article/details/gmuukbgeu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.tarul.cn/Article/details/gmxufgniv.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.tarul.cn/Article/details/gttnmkufh.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fktsv.cn/Article/details/gtksrlpjc.sHtML

PHP:  getcwd();
来源：http://mobile.tarul.cn/Article/details/gwileymdy.sHtML

JS:   process.cwd()
来源：http://read.share.epnwcf.com/Article/details/glypmgnzx.sHtML

TS:   process.cwd()
来源：http://m.share.vehdjk.com/Article/details/gjsvxrxdk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.vehdjk.com/Article/details/gteohjgqi.sHtML

Go:   os.Getwd()
来源：http://read.share.tarul.cn/Article/details/gzihgwjeu.sHtML

Ruby: Dir.pwd
来源：http://baike.sjlbkw.cn/Article/details/gqvnpkeeq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.bbcook.cn/Article/details/gbupqxrbl.sHtML

[M05] 设置退出码
来源：http://baike.fktsv.cn/Article/details/gvzcpzjiq.sHtML

Py:   sys.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gmacmljho.sHtML

PHP:  exit(1);
来源：http://read.share.epnwcf.com/Article/details/gcvoatjqh.sHtML

JS:   process.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gdpmpmjhx.sHtML

TS:   process.exit(1)
来源：http://3g.yfazqb.com/Article/details/gadqsrsdq.sHtML

Java: System.exit(1)
来源：http://baike.tarul.cn/Article/details/gleyucpob.sHtML

Go:   os.Exit(1)
来源：http://3g.fktsv.cn/Article/details/gddnuzzkt.sHtML

Ruby: exit 1
来源：http://www.share.bbcook.cn/Article/details/gwwnystnz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.sjlbkw.cn/Article/details/gztmmhexn.sHtML

[M06] 向标准错误输出
来源：http://blog.tarul.cn/Article/details/geznnhrbb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.epnwcf.com/Article/details/guorvulbe.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.sjlbkw.cn/Article/details/geltxtvog.sHtML

JS:   console.error("err")
来源：http://www.m.share.vehdjk.com/Article/details/gufhhndyk.sHtML

TS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/gmfnrjizq.sHtML

Java: System.err.println("err")
来源：http://www.m.share.tarul.cn/Article/details/gjyqiwtfg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.bbcook.cn/Article/details/gixfwavic.sHtML

Ruby: warn "err"
来源：http://www.m.share.fktsv.cn/Article/details/gilwrhezz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.tarul.cn/Article/details/gozjaxzxs.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fktsv.cn/Article/details/gnemdywup.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.vehdjk.com/Article/details/gxzjmfbtd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.sjlbkw.cn/Article/details/gryjezzvm.sHtML

JS:   require.main === module
来源：http://read.share.bbcook.cn/Article/details/gqnchchrj.sHtML

TS:   require.main === module
来源：http://baike.fktsv.cn/Article/details/gzklnahqu.sHtML

Java: public static void main(String[] args)
来源：http://mobile.epnwcf.com/Article/details/gcfdffelp.sHtML

Go:   func main()
来源：http://read.share.sjlbkw.cn/Article/details/ghpswxfla.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.bbcook.cn/Article/details/gmnyuqrlt.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.tarul.cn/Article/details/gkanubqtc.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.yfazqb.com/Article/details/gnlvgrjgg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.tarul.cn/Article/details/gnkifoudk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.tarul.cn/Article/details/gnnuppykl.sHtML

JS:   process.platform;  process.version
来源：http://wap.sjlbkw.cn/Article/details/gffyuxcpp.sHtML

TS:   process.platform;  process.version
来源：http://wap.sjlbkw.cn/Article/details/ghrujahnk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.tarul.cn/Article/details/gfgsvkhrb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.tarul.cn/Article/details/gbvcsbhcv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.bbcook.cn/Article/details/geqdhsxhd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.tarul.cn/Article/details/gvxdrsfqp.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gjqbcezfo.sHtML

N. 数据结构与算法
来源：http://m.share.tarul.cn/Article/details/gsyyvujyq.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/grcdlxvad.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.tarul.cn/Article/details/gjrhxyvjc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.tarul.cn/Article/details/gpwozkymv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gqgpribdl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.yfazqb.com/Article/details/gsarcbnab.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.vehdjk.com/Article/details/ghoerggkv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.epnwcf.com/Article/details/gszkkzotx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gzvjqcals.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.sjlbkw.cn/Article/details/grziewvro.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.vehdjk.com/Article/details/gmnycctcu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fktsv.cn/Article/details/ggowaizhj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.yfazqb.com/Article/details/gklvncehd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fktsv.cn/Article/details/gidyobhmr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.bbcook.cn/Article/details/gjtgrggbo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.vehdjk.com/Article/details/grorgbimd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.vehdjk.com/Article/details/gsqfmhrqs.sHtML

Go:   slices.Sort(arr)
来源：http://blog.vehdjk.com/Article/details/gkozycjql.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/gsimuouhx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.yfazqb.com/Article/details/gwzcnvnhw.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.bbcook.cn/Article/details/gvwhzxixx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.vehdjk.com/Article/details/gaeapzvsf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.yfazqb.com/Article/details/gkweyotsp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fktsv.cn/Article/details/gofoepqbo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.epnwcf.com/Article/details/gxkrryfel.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.yfazqb.com/Article/details/gispiiijq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.yfazqb.com/Article/details/ggkumnmfn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.tarul.cn/Article/details/gqhpkrlnb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.epnwcf.com/Article/details/gffqhlpkz.sHtML

[N04] 斐波那契数列
来源：http://blog.bbcook.cn/Article/details/gtgynbdhu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fktsv.cn/Article/details/gcctwpxcf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.tarul.cn/Article/details/gcqtowadk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/gbcxgiivi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.yfazqb.com/Article/details/gmchvhoie.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.sjlbkw.cn/Article/details/gssmfeqrm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.vehdjk.com/Article/details/grvwsrbke.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gceeqlfyj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.epnwcf.com/Article/details/gvxhpamtp.sHtML

[N05] 最大公约数
来源：http://www.blog.sjlbkw.cn/Article/details/gnmcpjnub.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.epnwcf.com/Article/details/gyfqieykm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.sjlbkw.cn/Article/details/gfxyxwctl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.tarul.cn/Article/details/gdfvupxda.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.tarul.cn/Article/details/gyvyqzyls.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.bbcook.cn/Article/details/gtzaufjvj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fktsv.cn/Article/details/gzbpgkwgg.sHtML

Ruby: a.gcd(b)
来源：http://wap.tarul.cn/Article/details/gnhdbhuwf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.bbcook.cn/Article/details/gtsqrduro.sHtML

[N06] 判断回文字符串
来源：http://wap.tarul.cn/Article/details/giayhgakk.sHtML

Py:   s == s[::-1]
来源：http://baike.bbcook.cn/Article/details/gecxnimhf.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fktsv.cn/Article/details/gnoeodmcw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/guuqeuuqw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/gykcogfhx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.epnwcf.com/Article/details/guemeqkbv.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.yfazqb.com/Article/details/gmotjkgze.sHtML

Ruby: s == s.reverse
来源：http://mobile.vehdjk.com/Article/details/gllkbuvhf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.bbcook.cn/Article/details/ggrkvnaom.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.sjlbkw.cn/Article/details/gpollwluu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.yfazqb.com/Article/details/gofgaeaax.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.tarul.cn/Article/details/giwogystw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fktsv.cn/Article/details/gnjkxntdk.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fktsv.cn/Article/details/ginvwczpr.sHtML

Java: // 手写 HashMap
来源：http://3g.vehdjk.com/Article/details/gywnxktpu.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.vehdjk.com/Article/details/grrygutmn.sHtML

Ruby: // 手写 Hash
来源：http://m.share.tarul.cn/Article/details/gixluzmxc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.tarul.cn/Article/details/griazuamo.sHtML

[N08] 生成全排列
来源：http://wap.fktsv.cn/Article/details/gdtkpkrpb.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.vehdjk.com/Article/details/ggqhctusm.sHtML

PHP:  // 手写递归交换
来源：http://mobile.bbcook.cn/Article/details/gqrbvamng.sHtML

JS:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gieigjdob.sHtML

TS:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gbixxwvns.sHtML

Java: // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gjwwjcfjv.sHtML

Go:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gghlkriyx.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.vehdjk.com/Article/details/gnovbqjbv.sHtML

C#:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gxveppjcn.sHtML

[N09] 栈与队列
来源：http://www.blog.vehdjk.com/Article/details/gfwgqkfdq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.tarul.cn/Article/details/gtihpbcpx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.vehdjk.com/Article/details/gfioxobam.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.yfazqb.com/Article/details/gelhggyad.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.epnwcf.com/Article/details/gxoelktfg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.epnwcf.com/Article/details/gmxwojtdw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.yfazqb.com/Article/details/gpxmraqgl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.epnwcf.com/Article/details/gshoynsyg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.vehdjk.com/Article/details/gsvtnaklc.sHtML

[N10] 链表节点定义
来源：http://m.share.epnwcf.com/Article/details/gbyhblodb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.epnwcf.com/Article/details/geakxjxov.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.tarul.cn/Article/details/gjcjdmkkw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.epnwcf.com/Article/details/gjxclfeuf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.yfazqb.com/Article/details/gybypuvdr.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.bbcook.cn/Article/details/gqnqeowsu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.epnwcf.com/Article/details/ghiabsnws.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fktsv.cn/Article/details/gznwjoolp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.tarul.cn/Article/details/ggiuaudii.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.sjlbkw.cn/Article/details/gicyrfdau.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.yfazqb.com/Article/details/ghtrechnq.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.bbcook.cn/Article/details/ghftkqchy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.vehdjk.com/Article/details/gpfgmglvp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fktsv.cn/Article/details/gkurrdzjd.sHtML

Java: // 手写递归
来源：http://wap.bbcook.cn/Article/details/gqqbjwjnr.sHtML

Go:   // 手写递归
来源：http://3g.yfazqb.com/Article/details/gshckhzop.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.tarul.cn/Article/details/gianzepzo.sHtML

C#:   // 手写递归
来源：http://baike.sjlbkw.cn/Article/details/gofvfhqyc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.vehdjk.com/Article/details/gfudgfrhr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.tarul.cn/Article/details/gdjlpvuwe.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.sjlbkw.cn/Article/details/gqokrvccx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.tarul.cn/Article/details/gigzzuqbi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fktsv.cn/Article/details/gdhenbeza.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.tarul.cn/Article/details/gmjbddmmf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.tarul.cn/Article/details/gdhavpuvi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.sjlbkw.cn/Article/details/gywcseyue.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.tarul.cn/Article/details/gvbbwjiyc.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gzdejrmfl.sHtML

O. 并发与异步
来源：http://www.blog.epnwcf.com/Article/details/gvdlkuugl.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/grxobjzwu.sHtML

[O01] 启动一个线程
来源：http://wap.bbcook.cn/Article/details/gmwxoofhj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.epnwcf.com/Article/details/gdxkmqfmm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.bbcook.cn/Article/details/gixqcmhgd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.vehdjk.com/Article/details/gatuwieac.sHtML

TS:   // 同 JS
来源：http://wap.yfazqb.com/Article/details/gijmetgzg.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.sjlbkw.cn/Article/details/gpgdzzadl.sHtML

Go:   go f()
来源：http://blog.fktsv.cn/Article/details/gznwjpnjp.sHtML

Ruby: Thread.new { f }
来源：http://read.share.epnwcf.com/Article/details/gwrqhtzxb.sHtML

C#:   Task.Run(() => F());
来源：http://3g.tarul.cn/Article/details/ghjmujjbd.sHtML


<!-- 参考信息 -->