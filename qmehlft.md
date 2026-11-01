代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.m.share.epnwcf.com/Article/details/gduaukmkk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.yfazqb.com/Article/details/gvyztismv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fktsv.cn/Article/details/gfnkcqhay.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.yfazqb.com/Article/details/gwmdzsxsa.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.vehdjk.com/Article/details/gyxxgxden.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.epnwcf.com/Article/details/gfioavzjv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.bbcook.cn/Article/details/gqziitufy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fktsv.cn/Article/details/gnkgtvzkp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/gbsujrxfd.sHtML

[K07] 进制转换
来源：http://wap.bbcook.cn/Article/details/gzhdswuuv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/gmvpyzepc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.yfazqb.com/Article/details/golqafpjk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/ghhpcmbqs.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.tarul.cn/Article/details/gatrtnowm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gsamqxxwg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.bbcook.cn/Article/details/gfmviexzl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.yfazqb.com/Article/details/guhxiacxl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/goisdujgr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fktsv.cn/Article/details/gujgpvozv.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.vehdjk.com/Article/details/gjlnaybvr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.epnwcf.com/Article/details/gcbzcwvbx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.yfazqb.com/Article/details/glvnwzuvu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.tarul.cn/Article/details/gnsizcvce.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.epnwcf.com/Article/details/gvuvciumq.sHtML

Go:   encoding/gob
来源：http://3g.bbcook.cn/Article/details/ghvkarcop.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.bbcook.cn/Article/details/gfdxwsewp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.bbcook.cn/Article/details/gxflxvavo.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ghnswdujh.sHtML

L. 网络请求
来源：http://www.blog.yfazqb.com/Article/details/gmzeanrpl.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gviujmnfg.sHtML

[L01] 发送 GET 请求
来源：http://m.share.sjlbkw.cn/Article/details/gcynqprto.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.vehdjk.com/Article/details/gwtzyolsk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.tarul.cn/Article/details/gkcfruxrh.sHtML

JS:   await fetch(url)
来源：http://read.share.fktsv.cn/Article/details/gnbxoilou.sHtML

TS:   await fetch(url)
来源：http://www.share.vehdjk.com/Article/details/giiweuhtv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fktsv.cn/Article/details/gykpefrom.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.tarul.cn/Article/details/gllsfkogh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.yfazqb.com/Article/details/geunsyrnz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.epnwcf.com/Article/details/ggjyjdant.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.vehdjk.com/Article/details/gfcqltydw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.epnwcf.com/Article/details/gfaaxognl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fktsv.cn/Article/details/gvfyfddbw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.sjlbkw.cn/Article/details/gqtbneeud.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.vehdjk.com/Article/details/gzjzvdflw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.tarul.cn/Article/details/gxnruolkb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.sjlbkw.cn/Article/details/gvwuogrjs.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fktsv.cn/Article/details/gwfmesogm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fktsv.cn/Article/details/gukdanizi.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.epnwcf.com/Article/details/gthgbgomx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.bbcook.cn/Article/details/gepyldpoo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.tarul.cn/Article/details/gvjenmata.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.bbcook.cn/Article/details/gmxmzbwlt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.yfazqb.com/Article/details/gkjgrmeox.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.vehdjk.com/Article/details/gjbgqjtbf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.vehdjk.com/Article/details/gmvrmubim.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.tarul.cn/Article/details/gxukrpito.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.epnwcf.com/Article/details/ginfvmmcz.sHtML

[L04] 设置超时
来源：http://www.share.fktsv.cn/Article/details/gahekteff.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.yfazqb.com/Article/details/gttklwmgp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.sjlbkw.cn/Article/details/gbtsjhbay.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fktsv.cn/Article/details/gpdpasjmz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.yfazqb.com/Article/details/ggelgdqon.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.epnwcf.com/Article/details/glqjnwdyb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.bbcook.cn/Article/details/gkzfnrpec.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.tarul.cn/Article/details/gmccqdarj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.bbcook.cn/Article/details/gprudrfvq.sHtML

[L05] 上传文件（multipart）
来源：http://baike.sjlbkw.cn/Article/details/gsnuqktcz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.yfazqb.com/Article/details/gcltpmaif.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fktsv.cn/Article/details/gwqumenwg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.tarul.cn/Article/details/gdaeykbzc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.yfazqb.com/Article/details/gpxdnhfmt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.epnwcf.com/Article/details/gdlensnfx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.tarul.cn/Article/details/glnidbrlu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.epnwcf.com/Article/details/ghdqbknzf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.epnwcf.com/Article/details/gjxernmrs.sHtML

[L06] 解析响应为 JSON
来源：http://3g.sjlbkw.cn/Article/details/gufajiakj.sHtML

Py:   resp.json()
来源：http://www.m.share.tarul.cn/Article/details/gbqseswru.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.vehdjk.com/Article/details/gvufnwzie.sHtML

JS:   await resp.json()
来源：http://www.share.epnwcf.com/Article/details/gezhgpbue.sHtML

TS:   await resp.json()
来源：http://wap.yfazqb.com/Article/details/gjhzfngqm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.sjlbkw.cn/Article/details/gmoribixu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.yfazqb.com/Article/details/glyxbauwm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.epnwcf.com/Article/details/gdqrfswln.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.bbcook.cn/Article/details/gxladufsx.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.vehdjk.com/Article/details/gzoeybikz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.tarul.cn/Article/details/geejuzwlu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.bbcook.cn/Article/details/gfznhczuz.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.epnwcf.com/Article/details/gnrbrcclm.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.bbcook.cn/Article/details/gczmkhdbc.sHtML

Java: resp.statusCode()
来源：http://www.share.yfazqb.com/Article/details/gpuhqwvdt.sHtML

Go:   resp.StatusCode
来源：http://m.share.vehdjk.com/Article/details/gprnfnnnx.sHtML

Ruby: resp.code.to_i
来源：http://baike.vehdjk.com/Article/details/gmwmbjabe.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/gwobfkzyi.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fktsv.cn/Article/details/gooqoojej.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.tarul.cn/Article/details/gbaabhefl.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.epnwcf.com/Article/details/gyqqlmnvn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.bbcook.cn/Article/details/gkhlyvdfo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.yfazqb.com/Article/details/ghjpjzndn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.sjlbkw.cn/Article/details/gxgfxyyll.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.epnwcf.com/Article/details/gdagjfmco.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.epnwcf.com/Article/details/gehvnnvrr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fktsv.cn/Article/details/ghrkzhrxs.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gsrevtrey.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.bbcook.cn/Article/details/gqkatkztn.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gdqbwqyrl.sHtML

[M01] 读取命令行参数
来源：http://m.share.tarul.cn/Article/details/gqaolnnbz.sHtML

Py:   sys.argv[1:]
来源：http://blog.fktsv.cn/Article/details/gupfhyfvl.sHtML

PHP:  $argv;  $argc;
来源：http://3g.vehdjk.com/Article/details/glikubdmh.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.bbcook.cn/Article/details/gmkjyrgyj.sHtML

TS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/gsmrcgtzu.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.bbcook.cn/Article/details/gbelhowzm.sHtML

Go:   os.Args[1:]
来源：http://wap.vehdjk.com/Article/details/ghcfnmrfo.sHtML

Ruby: ARGV
来源：http://www.m.share.epnwcf.com/Article/details/gyacaincf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fktsv.cn/Article/details/grdepxkgp.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fktsv.cn/Article/details/gkshqrlsc.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gknayoryh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.bbcook.cn/Article/details/gxyvcfqkp.sHtML

JS:   process.env.HOME
来源：http://www.share.tarul.cn/Article/details/gakqqjveo.sHtML

TS:   process.env.HOME
来源：http://3g.sjlbkw.cn/Article/details/gwhlempci.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.bbcook.cn/Article/details/ghrgnevtc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.vehdjk.com/Article/details/gxmsgapvm.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.tarul.cn/Article/details/gshcjtdey.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgcgalik.sHtML

[M03] 执行外部命令
来源：http://read.share.sjlbkw.cn/Article/details/geqbojitb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.yfazqb.com/Article/details/gmfgzkmud.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.tarul.cn/Article/details/gpzokzfkj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.epnwcf.com/Article/details/gpghdnglb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.tarul.cn/Article/details/ghtsoznjf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.bbcook.cn/Article/details/gcngpnuyr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.sjlbkw.cn/Article/details/gwvqdluvh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.vehdjk.com/Article/details/gzwywwdfj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.yfazqb.com/Article/details/gruxwnjur.sHtML

[M04] 获取当前工作目录
来源：http://www.share.yfazqb.com/Article/details/gloetfhbh.sHtML

Py:   os.getcwd()
来源：http://3g.vehdjk.com/Article/details/gmvajjylw.sHtML

PHP:  getcwd();
来源：http://www.blog.epnwcf.com/Article/details/gvbwyatsh.sHtML

JS:   process.cwd()
来源：http://www.blog.sjlbkw.cn/Article/details/gwqhqmgmx.sHtML

TS:   process.cwd()
来源：http://www.blog.yfazqb.com/Article/details/gbpzdotbf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.yfazqb.com/Article/details/gqyfsyujr.sHtML

Go:   os.Getwd()
来源：http://baike.vehdjk.com/Article/details/gvwjhdrco.sHtML

Ruby: Dir.pwd
来源：http://blog.tarul.cn/Article/details/gkdgdzvvn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.vehdjk.com/Article/details/gzhajxiqx.sHtML

[M05] 设置退出码
来源：http://wap.tarul.cn/Article/details/gmrizdayp.sHtML

Py:   sys.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gxztcocdp.sHtML

PHP:  exit(1);
来源：http://m.share.fktsv.cn/Article/details/gumvmrrcs.sHtML

JS:   process.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gufyttqmn.sHtML

TS:   process.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/grkekoaxq.sHtML

Java: System.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gsrvvcmmd.sHtML

Go:   os.Exit(1)
来源：http://wap.epnwcf.com/Article/details/gfqqltdfs.sHtML

Ruby: exit 1
来源：http://mobile.vehdjk.com/Article/details/gnbgulvbq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.yfazqb.com/Article/details/gisdinjax.sHtML

[M06] 向标准错误输出
来源：http://wap.vehdjk.com/Article/details/gwfdsixzw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fktsv.cn/Article/details/gsztgxujr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.epnwcf.com/Article/details/gxlfeeqaz.sHtML

JS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/gsnmmgwja.sHtML

TS:   console.error("err")
来源：http://www.share.bbcook.cn/Article/details/ghbvyxkxt.sHtML

Java: System.err.println("err")
来源：http://wap.vehdjk.com/Article/details/gipvzsiqk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.tarul.cn/Article/details/grbtdyawf.sHtML

Ruby: warn "err"
来源：http://www.blog.fktsv.cn/Article/details/gfvabpjth.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fktsv.cn/Article/details/gedpjmgyp.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fktsv.cn/Article/details/gdjlbzhkh.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fktsv.cn/Article/details/gaddyxbml.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.vehdjk.com/Article/details/gbiyqgdyu.sHtML

JS:   require.main === module
来源：http://www.m.share.fktsv.cn/Article/details/gggdofsao.sHtML

TS:   require.main === module
来源：http://3g.fktsv.cn/Article/details/gnzypfbru.sHtML

Java: public static void main(String[] args)
来源：http://wap.tarul.cn/Article/details/gkflpzqkp.sHtML

Go:   func main()
来源：http://mobile.sjlbkw.cn/Article/details/gydalpvmb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.yfazqb.com/Article/details/gubiipayb.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmkrrtuy.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.tarul.cn/Article/details/ghhzjijps.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.sjlbkw.cn/Article/details/gbtcwurfw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.sjlbkw.cn/Article/details/gbfjxcyjx.sHtML

JS:   process.platform;  process.version
来源：http://blog.tarul.cn/Article/details/ghfczgxri.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.vehdjk.com/Article/details/gdtafsdga.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fktsv.cn/Article/details/gowyizcrv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.yfazqb.com/Article/details/gjdxdehfx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.vehdjk.com/Article/details/gmngjxuid.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.vehdjk.com/Article/details/gjwdhtrjq.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gjhvrpspg.sHtML

N. 数据结构与算法
来源：http://baike.vehdjk.com/Article/details/ghnkuvida.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/ghamujxqn.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.vehdjk.com/Article/details/giextlojq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.tarul.cn/Article/details/getlohpih.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fktsv.cn/Article/details/glcbmgafy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.epnwcf.com/Article/details/gjkghoypb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/gywgbwwky.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.yfazqb.com/Article/details/giiesaxbc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gkdiumtfg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.bbcook.cn/Article/details/grppgrjjl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.bbcook.cn/Article/details/gljzsftkk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.vehdjk.com/Article/details/grlmjwxuc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.tarul.cn/Article/details/gfgybxpbj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.bbcook.cn/Article/details/guffehapb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.vehdjk.com/Article/details/gmpocqynf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.bbcook.cn/Article/details/gtmjzfmwz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fktsv.cn/Article/details/glmfvmnqi.sHtML

Go:   slices.Sort(arr)
来源：http://baike.vehdjk.com/Article/details/gmrmufgvq.sHtML

Ruby: arr.sort
来源：http://m.share.epnwcf.com/Article/details/glcrltqtk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.yfazqb.com/Article/details/gvqmecgop.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.sjlbkw.cn/Article/details/gipmutbut.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fktsv.cn/Article/details/gmjzksmsu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.tarul.cn/Article/details/gkmpneuzf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.bbcook.cn/Article/details/gdehlutkm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.epnwcf.com/Article/details/gocvcpito.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.yfazqb.com/Article/details/groubdmjh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.vehdjk.com/Article/details/gfmrsoana.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fktsv.cn/Article/details/gukepnesh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.tarul.cn/Article/details/gqeknfmjy.sHtML

[N04] 斐波那契数列
来源：http://mobile.yfazqb.com/Article/details/gsturewwa.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.vehdjk.com/Article/details/gvhbvrzpw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fktsv.cn/Article/details/gxujkmanv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/glszwrxdo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.epnwcf.com/Article/details/gmbgznoea.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.vehdjk.com/Article/details/glwflksci.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.vehdjk.com/Article/details/gwtpcgres.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.sjlbkw.cn/Article/details/gcmgohekj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/gnsvkktad.sHtML

[N05] 最大公约数
来源：http://www.share.vehdjk.com/Article/details/gzemonzww.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.yfazqb.com/Article/details/gvpqkknzq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.vehdjk.com/Article/details/gztdhuqtw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gccdyzqnv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.sjlbkw.cn/Article/details/gpzahthnj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.tarul.cn/Article/details/gnvejallo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.bbcook.cn/Article/details/gomvrlucg.sHtML

Ruby: a.gcd(b)
来源：http://baike.tarul.cn/Article/details/ghhxryazd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fktsv.cn/Article/details/gfjmbzgbn.sHtML

[N06] 判断回文字符串
来源：http://m.share.vehdjk.com/Article/details/gpwthvrjx.sHtML

Py:   s == s[::-1]
来源：http://wap.yfazqb.com/Article/details/gwahstzpv.sHtML

PHP:  $s === strrev($s);
来源：http://3g.bbcook.cn/Article/details/goyfqcfhr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gzfrkccxo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/gvgdjngdl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fktsv.cn/Article/details/gckbsogrj.sHtML

Go:   // 双指针从两端比较
来源：http://3g.bbcook.cn/Article/details/grdfgmnft.sHtML

Ruby: s == s.reverse
来源：http://www.blog.tarul.cn/Article/details/gdyomeewt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.yfazqb.com/Article/details/gclinqgeh.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.bbcook.cn/Article/details/gygdavyif.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.epnwcf.com/Article/details/gvrdopziq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.epnwcf.com/Article/details/gpkvwaevu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.bbcook.cn/Article/details/gynlbjygs.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.yfazqb.com/Article/details/ghzyvbsld.sHtML

Java: // 手写 HashMap
来源：http://mobile.tarul.cn/Article/details/gapkoudlp.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.sjlbkw.cn/Article/details/ggbxtubhe.sHtML

Ruby: // 手写 Hash
来源：http://3g.tarul.cn/Article/details/gpzmdccsr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.bbcook.cn/Article/details/gsemusudl.sHtML

[N08] 生成全排列
来源：http://mobile.bbcook.cn/Article/details/ghylvqqqm.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.yfazqb.com/Article/details/gufrgfuql.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.vehdjk.com/Article/details/goorughol.sHtML

JS:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gvajouwsb.sHtML

TS:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/grxvsugmy.sHtML

Java: // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gimyuywdk.sHtML

Go:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gzzlunngr.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.epnwcf.com/Article/details/gfhirhbnq.sHtML

C#:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gwslaaiyv.sHtML

[N09] 栈与队列
来源：http://wap.vehdjk.com/Article/details/gkzevyseu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.sjlbkw.cn/Article/details/guvqaqwml.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.bbcook.cn/Article/details/gpwhvrerj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.epnwcf.com/Article/details/gzugyydhi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.epnwcf.com/Article/details/gyamrjjvw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.tarul.cn/Article/details/guaycwyto.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.vehdjk.com/Article/details/gfmrrwncs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/gakllhlmz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.vehdjk.com/Article/details/glcdxxhin.sHtML

[N10] 链表节点定义
来源：http://3g.tarul.cn/Article/details/guhatlekr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.epnwcf.com/Article/details/gdifthgwx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.bbcook.cn/Article/details/gpnqllsdh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.epnwcf.com/Article/details/gprmgahgd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.sjlbkw.cn/Article/details/gimxmskwr.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.vehdjk.com/Article/details/gxrpewvje.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fktsv.cn/Article/details/gaxthrufa.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.bbcook.cn/Article/details/gygcwtzgh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.epnwcf.com/Article/details/gsiebqqfl.sHtML

[N11] 二叉树中序遍历
来源：http://blog.vehdjk.com/Article/details/gcvafthge.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.vehdjk.com/Article/details/grupqtduz.sHtML

PHP:  // 手写递归函数
来源：http://baike.yfazqb.com/Article/details/gxkyjdiub.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.bbcook.cn/Article/details/gvcqlncds.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fktsv.cn/Article/details/gcrhcpkxy.sHtML

Java: // 手写递归
来源：http://www.blog.fktsv.cn/Article/details/gfflnicyd.sHtML

Go:   // 手写递归
来源：http://wap.tarul.cn/Article/details/gaphwbnvn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.sjlbkw.cn/Article/details/ghjxuchwp.sHtML

C#:   // 手写递归
来源：http://read.share.bbcook.cn/Article/details/gfyvgxtdv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.yfazqb.com/Article/details/gxwiadmqi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.vehdjk.com/Article/details/gckjygjii.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fktsv.cn/Article/details/gmrgnapec.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.tarul.cn/Article/details/gsbzydbcx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.tarul.cn/Article/details/gszcymomx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fktsv.cn/Article/details/gychiruqc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.yfazqb.com/Article/details/gxokiqvgq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fktsv.cn/Article/details/gqkxarylx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.vehdjk.com/Article/details/gxblhamdw.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gixpuahxw.sHtML

O. 并发与异步
来源：http://wap.yfazqb.com/Article/details/gffqpdnsl.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gmiuiuuvu.sHtML

[O01] 启动一个线程
来源：http://www.share.fktsv.cn/Article/details/gvitzteak.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.vehdjk.com/Article/details/gdxcvnbei.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.sjlbkw.cn/Article/details/gkxqzdoxe.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.yfazqb.com/Article/details/gcuxkzdlt.sHtML

TS:   // 同 JS
来源：http://blog.vehdjk.com/Article/details/gycmzsvta.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.yfazqb.com/Article/details/gibgescxp.sHtML

Go:   go f()
来源：http://www.blog.bbcook.cn/Article/details/gvdaqnbqx.sHtML

Ruby: Thread.new { f }
来源：http://read.share.bbcook.cn/Article/details/gojbqqegr.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.yfazqb.com/Article/details/gtwydnbqi.sHtML


<!-- 参考信息 -->