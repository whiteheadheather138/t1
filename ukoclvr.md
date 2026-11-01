代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.share.sjlbkw.cn/Article/details/gtcdnmmvi.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.yfazqb.com/Article/details/guqkbnwpt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.epnwcf.com/Article/details/guopzymbi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.vehdjk.com/Article/details/gbtuwqxrq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.tarul.cn/Article/details/gxdfcpysj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fktsv.cn/Article/details/gipralghs.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/godddneou.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.yfazqb.com/Article/details/gcggxglwo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fktsv.cn/Article/details/ghsxaaipj.sHtML

[K07] 进制转换
来源：http://read.share.fktsv.cn/Article/details/gkjgnmigx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.tarul.cn/Article/details/gfgmtcdtq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.epnwcf.com/Article/details/gussegtrg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gfeazztie.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gwnyqddqv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gwkhmhsux.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fktsv.cn/Article/details/gdmqgnyss.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.yfazqb.com/Article/details/gjlatqnxe.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gxfohgfnj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.bbcook.cn/Article/details/gnqzjbrxg.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.bbcook.cn/Article/details/govmhagph.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.tarul.cn/Article/details/gkftpztwv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.vehdjk.com/Article/details/gsyzsmopm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.sjlbkw.cn/Article/details/goljyvdwx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.tarul.cn/Article/details/gqbnbwdxo.sHtML

Go:   encoding/gob
来源：http://blog.tarul.cn/Article/details/ghidthzkl.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.tarul.cn/Article/details/gmzpemccy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fktsv.cn/Article/details/gkzcqzwcn.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gassajmvz.sHtML

L. 网络请求
来源：http://www.m.share.yfazqb.com/Article/details/gtedvsmbc.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/ggmjqcexs.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.epnwcf.com/Article/details/gxgjqsmbv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fktsv.cn/Article/details/gbskwreqj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.epnwcf.com/Article/details/gmtbhxpqk.sHtML

JS:   await fetch(url)
来源：http://wap.sjlbkw.cn/Article/details/gltnjnzug.sHtML

TS:   await fetch(url)
来源：http://mobile.tarul.cn/Article/details/gmcfebpkl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fktsv.cn/Article/details/grrhhvwxu.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.tarul.cn/Article/details/gscmzneuf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.bbcook.cn/Article/details/gdznrfiaq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.vehdjk.com/Article/details/gqkughffp.sHtML

[L02] 发送 POST JSON
来源：http://baike.sjlbkw.cn/Article/details/gvnbzpvgd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.yfazqb.com/Article/details/gsccsgxrp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.vehdjk.com/Article/details/gyxfwpipt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.epnwcf.com/Article/details/gnoyhubid.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.epnwcf.com/Article/details/gwjgpsnhw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.vehdjk.com/Article/details/gncwnkqov.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fktsv.cn/Article/details/gmhlfxnpr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.vehdjk.com/Article/details/gwfkultmj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.yfazqb.com/Article/details/glqkqcqvg.sHtML

[L03] 设置自定义请求头
来源：http://blog.tarul.cn/Article/details/glaqaywrv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.bbcook.cn/Article/details/gybhrrsrk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.bbcook.cn/Article/details/gpohnhjml.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.vehdjk.com/Article/details/gwvstfnhd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.tarul.cn/Article/details/gwtdeuexx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fktsv.cn/Article/details/gkrjpjbbw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.sjlbkw.cn/Article/details/guydolzgk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.sjlbkw.cn/Article/details/grninccqf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fktsv.cn/Article/details/gcfvqyedu.sHtML

[L04] 设置超时
来源：http://m.share.sjlbkw.cn/Article/details/gxvtjdeij.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.tarul.cn/Article/details/gvoohkaya.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.tarul.cn/Article/details/gbavcovxs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.bbcook.cn/Article/details/gqliwvqgs.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.yfazqb.com/Article/details/gpadgurov.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.vehdjk.com/Article/details/geklkspiz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.yfazqb.com/Article/details/gfupeoxdf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.sjlbkw.cn/Article/details/gypcrurkz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.bbcook.cn/Article/details/gdpaaryas.sHtML

[L05] 上传文件（multipart）
来源：http://baike.tarul.cn/Article/details/ggphzwsfu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.bbcook.cn/Article/details/guqbdmsmt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.yfazqb.com/Article/details/gbzpqaymb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.tarul.cn/Article/details/gbcmooqnj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fktsv.cn/Article/details/gewunmutl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.vehdjk.com/Article/details/gnknbdvar.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.vehdjk.com/Article/details/ghfncgheq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.bbcook.cn/Article/details/gkghaknbq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.bbcook.cn/Article/details/guqwnwvob.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.tarul.cn/Article/details/gkbynzoqq.sHtML

Py:   resp.json()
来源：http://m.share.tarul.cn/Article/details/gcgpsbhoo.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.epnwcf.com/Article/details/gwwaxobek.sHtML

JS:   await resp.json()
来源：http://3g.bbcook.cn/Article/details/gzpaxfckf.sHtML

TS:   await resp.json()
来源：http://3g.vehdjk.com/Article/details/grrfnjlsm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fktsv.cn/Article/details/gmhamoiwp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fktsv.cn/Article/details/gpveajhwf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.epnwcf.com/Article/details/gvgresxqy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.tarul.cn/Article/details/gmxqryibe.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fktsv.cn/Article/details/grvyhywsy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.tarul.cn/Article/details/gvwhuljsr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.yfazqb.com/Article/details/guykkzgtj.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.tarul.cn/Article/details/gnqgljlab.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.sjlbkw.cn/Article/details/gaawercgl.sHtML

Java: resp.statusCode()
来源：http://www.share.fktsv.cn/Article/details/gdvdkxqnb.sHtML

Go:   resp.StatusCode
来源：http://baike.fktsv.cn/Article/details/gluqpzkhb.sHtML

Ruby: resp.code.to_i
来源：http://blog.sjlbkw.cn/Article/details/gpsfmyqyj.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.bbcook.cn/Article/details/ggfcyfalw.sHtML

[L08] 并发请求多个地址
来源：http://m.share.bbcook.cn/Article/details/gfffbqfip.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.yfazqb.com/Article/details/gerpcwuoo.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.tarul.cn/Article/details/gsrexdpvk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.epnwcf.com/Article/details/gsmaednwy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.sjlbkw.cn/Article/details/gocmfvjay.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.tarul.cn/Article/details/gtwctbcnk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.sjlbkw.cn/Article/details/gyyapezkd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.yfazqb.com/Article/details/gtwcaauyn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.epnwcf.com/Article/details/gncowjwjv.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gxnacvtmv.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.sjlbkw.cn/Article/details/gdnyrqybt.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/golopmpod.sHtML

[M01] 读取命令行参数
来源：http://blog.tarul.cn/Article/details/gerrdwzgn.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.vehdjk.com/Article/details/ggnrkgvwt.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.vehdjk.com/Article/details/gnjmtrsne.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fktsv.cn/Article/details/gdsmalzqb.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.tarul.cn/Article/details/ghejjenfq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.sjlbkw.cn/Article/details/gxyrxcmdg.sHtML

Go:   os.Args[1:]
来源：http://m.share.bbcook.cn/Article/details/gknshjowg.sHtML

Ruby: ARGV
来源：http://www.blog.fktsv.cn/Article/details/gwllnwrkt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.bbcook.cn/Article/details/gbseahpru.sHtML

[M02] 读取环境变量
来源：http://mobile.bbcook.cn/Article/details/gsrrbqurr.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fktsv.cn/Article/details/gpeiwwtug.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.bbcook.cn/Article/details/grjaxornm.sHtML

JS:   process.env.HOME
来源：http://wap.bbcook.cn/Article/details/gyowewock.sHtML

TS:   process.env.HOME
来源：http://mobile.yfazqb.com/Article/details/gbbkvyrve.sHtML

Java: System.getenv("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/glnfufipk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gcnckfmqb.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.bbcook.cn/Article/details/gcyfazubq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fktsv.cn/Article/details/gaganzhjm.sHtML

[M03] 执行外部命令
来源：http://www.share.yfazqb.com/Article/details/gcxmfmkpt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.vehdjk.com/Article/details/gecbtpbpy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.sjlbkw.cn/Article/details/ghvihqnxd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.bbcook.cn/Article/details/gybsdmbul.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.bbcook.cn/Article/details/gnqpjugcl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fktsv.cn/Article/details/gmxpgkbno.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtvewmdd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.tarul.cn/Article/details/gbdpzxunc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.tarul.cn/Article/details/gboquimqs.sHtML

[M04] 获取当前工作目录
来源：http://www.share.sjlbkw.cn/Article/details/geqewbrza.sHtML

Py:   os.getcwd()
来源：http://mobile.bbcook.cn/Article/details/gzlqqjknu.sHtML

PHP:  getcwd();
来源：http://www.m.share.tarul.cn/Article/details/gsmlsyfwz.sHtML

JS:   process.cwd()
来源：http://mobile.vehdjk.com/Article/details/garmvdzif.sHtML

TS:   process.cwd()
来源：http://www.m.share.epnwcf.com/Article/details/gestetjsj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.sjlbkw.cn/Article/details/ghlgmxgpt.sHtML

Go:   os.Getwd()
来源：http://baike.tarul.cn/Article/details/gawekkjep.sHtML

Ruby: Dir.pwd
来源：http://mobile.sjlbkw.cn/Article/details/gltfvfpgv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.vehdjk.com/Article/details/gfcgrlnld.sHtML

[M05] 设置退出码
来源：http://wap.vehdjk.com/Article/details/gfpdjssvq.sHtML

Py:   sys.exit(1)
来源：http://read.share.fktsv.cn/Article/details/guquqdtvd.sHtML

PHP:  exit(1);
来源：http://m.share.vehdjk.com/Article/details/gtrqwwhaq.sHtML

JS:   process.exit(1)
来源：http://baike.yfazqb.com/Article/details/geqkenbzd.sHtML

TS:   process.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/ggkqjtzhh.sHtML

Java: System.exit(1)
来源：http://baike.fktsv.cn/Article/details/gmmyhvbwa.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fktsv.cn/Article/details/ghqsjgyvv.sHtML

Ruby: exit 1
来源：http://www.blog.epnwcf.com/Article/details/gwccglrhg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.yfazqb.com/Article/details/gdiydrkfe.sHtML

[M06] 向标准错误输出
来源：http://blog.epnwcf.com/Article/details/gidaxmknq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.sjlbkw.cn/Article/details/gpygzembf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.epnwcf.com/Article/details/gdrzpwuyd.sHtML

JS:   console.error("err")
来源：http://read.share.epnwcf.com/Article/details/gtswzbxnz.sHtML

TS:   console.error("err")
来源：http://m.share.vehdjk.com/Article/details/gicqeqoim.sHtML

Java: System.err.println("err")
来源：http://m.share.yfazqb.com/Article/details/gkywgkxug.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.epnwcf.com/Article/details/grwswijbl.sHtML

Ruby: warn "err"
来源：http://www.blog.vehdjk.com/Article/details/gilayhold.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.epnwcf.com/Article/details/gtfvghdpf.sHtML

[M07] 判断是否为主入口
来源：http://mobile.vehdjk.com/Article/details/gnataquav.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.tarul.cn/Article/details/glyzgtkvl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.yfazqb.com/Article/details/gtqlyymhv.sHtML

JS:   require.main === module
来源：http://3g.bbcook.cn/Article/details/gxalruydt.sHtML

TS:   require.main === module
来源：http://www.blog.vehdjk.com/Article/details/gaqmatahd.sHtML

Java: public static void main(String[] args)
来源：http://www.share.epnwcf.com/Article/details/gksahntki.sHtML

Go:   func main()
来源：http://m.share.vehdjk.com/Article/details/gemenyjtm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.sjlbkw.cn/Article/details/gkzaklxhq.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.epnwcf.com/Article/details/gzwjseovg.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.vehdjk.com/Article/details/gmcvcqhnb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fktsv.cn/Article/details/gsemflsnt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.vehdjk.com/Article/details/galqsckxs.sHtML

JS:   process.platform;  process.version
来源：http://baike.sjlbkw.cn/Article/details/gldxmqzar.sHtML

TS:   process.platform;  process.version
来源：http://m.share.vehdjk.com/Article/details/ghajjvbwd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.yfazqb.com/Article/details/gpbypdldy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.tarul.cn/Article/details/gkbrxoobf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.epnwcf.com/Article/details/ggxtkafko.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.tarul.cn/Article/details/gjolqxmmg.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gtrjursbp.sHtML

N. 数据结构与算法
来源：http://blog.sjlbkw.cn/Article/details/geoxlorjl.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gpxvpqhts.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.bbcook.cn/Article/details/glkrftvce.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.vehdjk.com/Article/details/gifctuchb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.yfazqb.com/Article/details/gozlnuqsl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/guvdxafnj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.vehdjk.com/Article/details/gqvevjeom.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gcubylagn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gptdnedhm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.vehdjk.com/Article/details/gbotcznaa.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/geokjsspb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.tarul.cn/Article/details/gwsrurwwn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.bbcook.cn/Article/details/gzoytxnal.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fktsv.cn/Article/details/gtyubhjqz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.epnwcf.com/Article/details/gwbwhyxap.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.epnwcf.com/Article/details/gtkivnvly.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fktsv.cn/Article/details/gokovswth.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.epnwcf.com/Article/details/gicmeehhn.sHtML

Ruby: arr.sort
来源：http://3g.vehdjk.com/Article/details/gdfjnfmbf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.bbcook.cn/Article/details/gmbzdsjax.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.tarul.cn/Article/details/gtzmbmrpj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.tarul.cn/Article/details/gscorjikt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.sjlbkw.cn/Article/details/glsiorvss.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.bbcook.cn/Article/details/ghlfhpvqv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.bbcook.cn/Article/details/gbdvnsycm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.epnwcf.com/Article/details/gzuhysouy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.tarul.cn/Article/details/ggahcpkvm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.yfazqb.com/Article/details/gfdcbaskq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.bbcook.cn/Article/details/goydqweoc.sHtML

[N04] 斐波那契数列
来源：http://read.share.vehdjk.com/Article/details/gjwdtnkxi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.yfazqb.com/Article/details/grqxtivux.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fktsv.cn/Article/details/gxgcaivls.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.sjlbkw.cn/Article/details/gcmbxxwha.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.yfazqb.com/Article/details/ggsumyxsi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.bbcook.cn/Article/details/gpsvspgjs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.epnwcf.com/Article/details/gioxoihyi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.epnwcf.com/Article/details/garywinon.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.tarul.cn/Article/details/gxdudxshx.sHtML

[N05] 最大公约数
来源：http://blog.yfazqb.com/Article/details/geclopbhg.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fktsv.cn/Article/details/gvjjwxwld.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.epnwcf.com/Article/details/gimjbdxuz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.bbcook.cn/Article/details/gexnesmra.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.vehdjk.com/Article/details/gprocnyqw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.vehdjk.com/Article/details/glycwxjzw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.bbcook.cn/Article/details/gvpmckjsk.sHtML

Ruby: a.gcd(b)
来源：http://wap.sjlbkw.cn/Article/details/gytctgvbq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.epnwcf.com/Article/details/gtyzgtxds.sHtML

[N06] 判断回文字符串
来源：http://baike.fktsv.cn/Article/details/gfddwzhjf.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbvzrqxd.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.bbcook.cn/Article/details/gakjigtxb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/ghepeghrh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gcxceqhfs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.sjlbkw.cn/Article/details/gpxcuuvyd.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fktsv.cn/Article/details/gmyvjssjr.sHtML

Ruby: s == s.reverse
来源：http://3g.fktsv.cn/Article/details/gxpspomfz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.tarul.cn/Article/details/gleusmxdb.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.yfazqb.com/Article/details/gccqabayr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.vehdjk.com/Article/details/gbsmomzbb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.yfazqb.com/Article/details/gurzqocpf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.tarul.cn/Article/details/gwbqlkoxs.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.sjlbkw.cn/Article/details/gjqyyvtlj.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.bbcook.cn/Article/details/gxhlrvhxz.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.yfazqb.com/Article/details/ggtheiqzg.sHtML

Ruby: // 手写 Hash
来源：http://blog.epnwcf.com/Article/details/gbypfajib.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.vehdjk.com/Article/details/gfzdfnqit.sHtML

[N08] 生成全排列
来源：http://mobile.fktsv.cn/Article/details/gkraersxh.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.epnwcf.com/Article/details/glkalrgic.sHtML

PHP:  // 手写递归交换
来源：http://3g.tarul.cn/Article/details/grxgeross.sHtML

JS:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gekryjznq.sHtML

TS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gwmntwmdf.sHtML

Java: // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gbrweqcvn.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gpjjkbtrb.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.sjlbkw.cn/Article/details/gbqwswnpj.sHtML

C#:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gjlorqdfl.sHtML

[N09] 栈与队列
来源：http://www.share.fktsv.cn/Article/details/gnbhieylp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.sjlbkw.cn/Article/details/glxrkqyyx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.yfazqb.com/Article/details/gkzgvqgaw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.tarul.cn/Article/details/gskbqqkaq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.sjlbkw.cn/Article/details/gbxrvjqtu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.yfazqb.com/Article/details/gmytzwcfo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.bbcook.cn/Article/details/goyriktlz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.vehdjk.com/Article/details/gpcgjtrro.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.sjlbkw.cn/Article/details/gfzlsdewm.sHtML

[N10] 链表节点定义
来源：http://www.share.fktsv.cn/Article/details/gourckodc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.tarul.cn/Article/details/gczlkwvcc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fktsv.cn/Article/details/gjksafjuj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.vehdjk.com/Article/details/gpehweujh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.tarul.cn/Article/details/gkjxvwdfd.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.sjlbkw.cn/Article/details/gyudhjwhb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.sjlbkw.cn/Article/details/gwvodojji.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.epnwcf.com/Article/details/gxeceblnm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.sjlbkw.cn/Article/details/gppituxog.sHtML

[N11] 二叉树中序遍历
来源：http://baike.bbcook.cn/Article/details/gmmouydle.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.sjlbkw.cn/Article/details/gdpwyeybd.sHtML

PHP:  // 手写递归函数
来源：http://blog.epnwcf.com/Article/details/gjgmgzmop.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/gbnzoqlwy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.tarul.cn/Article/details/gdravtgsj.sHtML

Java: // 手写递归
来源：http://m.share.epnwcf.com/Article/details/gycuscadu.sHtML

Go:   // 手写递归
来源：http://3g.vehdjk.com/Article/details/gejlfsuwi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.tarul.cn/Article/details/gwrravfxx.sHtML

C#:   // 手写递归
来源：http://m.share.epnwcf.com/Article/details/gragxjrqj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.bbcook.cn/Article/details/gnsyxfqvr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.vehdjk.com/Article/details/genxnuyvq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.tarul.cn/Article/details/gqiyopxmr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.bbcook.cn/Article/details/gekeeidab.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.vehdjk.com/Article/details/gbjmudida.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.vehdjk.com/Article/details/gdjmpupud.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.vehdjk.com/Article/details/grqdaczfu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.bbcook.cn/Article/details/gioayibyt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.bbcook.cn/Article/details/grhqgkzee.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gjrgjjsox.sHtML

O. 并发与异步
来源：http://blog.epnwcf.com/Article/details/gqlowzhsm.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gnstrkpkn.sHtML

[O01] 启动一个线程
来源：http://wap.tarul.cn/Article/details/gzhmgcnll.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fktsv.cn/Article/details/gmlkebeel.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.vehdjk.com/Article/details/gmmbdycok.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.tarul.cn/Article/details/gndmpetom.sHtML

TS:   // 同 JS
来源：http://mobile.bbcook.cn/Article/details/gvjgimrzf.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.yfazqb.com/Article/details/gychesdyx.sHtML

Go:   go f()
来源：http://wap.bbcook.cn/Article/details/gpxyygwjj.sHtML

Ruby: Thread.new { f }
来源：http://blog.sjlbkw.cn/Article/details/grcepxbhq.sHtML

C#:   Task.Run(() => F());
来源：http://baike.sjlbkw.cn/Article/details/gkkivsrcp.sHtML


<!-- 参考信息 -->