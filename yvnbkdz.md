代发 wailian999

[K06] 解析 URL 查询串
来源：http://3g.fktsv.cn/Article/details/glncefwps.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.tarul.cn/Article/details/gsjkznuvb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.sjlbkw.cn/Article/details/gxyiudumd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwyzayafm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.tarul.cn/Article/details/gzxpivkuc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.bbcook.cn/Article/details/gefyfwdun.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/gcmcinzuy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/gzpxwwcua.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/gpydshkaa.sHtML

[K07] 进制转换
来源：http://wap.sjlbkw.cn/Article/details/gbwhepzff.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fktsv.cn/Article/details/ghnmpjecl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.sjlbkw.cn/Article/details/ggmlddrir.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/grjbpqpdc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/ghzmgphvu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gzqhccwih.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.bbcook.cn/Article/details/gqnjrmkdb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.tarul.cn/Article/details/gvhaulooj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gkzrlcnia.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.epnwcf.com/Article/details/gjtcfwtdi.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.sjlbkw.cn/Article/details/gogjgryni.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.sjlbkw.cn/Article/details/gprplnaup.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.yfazqb.com/Article/details/gjlrqjhjg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gtweccaou.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fktsv.cn/Article/details/gusgkcuuk.sHtML

Go:   encoding/gob
来源：http://www.share.tarul.cn/Article/details/ghnmcnsfr.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.tarul.cn/Article/details/guxomvxim.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.sjlbkw.cn/Article/details/gsgadhvue.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gypgelubp.sHtML

L. 网络请求
来源：http://read.share.tarul.cn/Article/details/gwryzjkyj.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/glrgkybjd.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.yfazqb.com/Article/details/gjykrxycg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.yfazqb.com/Article/details/gcgkqataa.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.yfazqb.com/Article/details/gbgrnvovo.sHtML

JS:   await fetch(url)
来源：http://m.share.vehdjk.com/Article/details/gpfgnwkxl.sHtML

TS:   await fetch(url)
来源：http://mobile.sjlbkw.cn/Article/details/gdmoqlkyp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fktsv.cn/Article/details/godduufim.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.bbcook.cn/Article/details/gumfqfpjd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.vehdjk.com/Article/details/gepdivefk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.vehdjk.com/Article/details/gkwmxjmir.sHtML

[L02] 发送 POST JSON
来源：http://mobile.bbcook.cn/Article/details/giuwshodw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fktsv.cn/Article/details/glfieyjqf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.epnwcf.com/Article/details/gzawkuhty.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.tarul.cn/Article/details/gxbkarlyr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fktsv.cn/Article/details/gzirtyskd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.tarul.cn/Article/details/ghiqpgjrg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fktsv.cn/Article/details/gmbmcnsfz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.sjlbkw.cn/Article/details/gthjchpnh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fktsv.cn/Article/details/grwkqgcuf.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.sjlbkw.cn/Article/details/ggaduzczj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.bbcook.cn/Article/details/gvvabwbzm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.epnwcf.com/Article/details/gnlwqmita.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.tarul.cn/Article/details/ggmxdsbdt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.yfazqb.com/Article/details/gaxytendy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.epnwcf.com/Article/details/gfkxeqrpf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.vehdjk.com/Article/details/gxrwliwmf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.epnwcf.com/Article/details/gagfatmav.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.vehdjk.com/Article/details/gmdaupdjz.sHtML

[L04] 设置超时
来源：http://m.share.bbcook.cn/Article/details/grqbmhchp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.yfazqb.com/Article/details/gvyfjchbs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.tarul.cn/Article/details/gzucgrmms.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.bbcook.cn/Article/details/goawjqjjx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.yfazqb.com/Article/details/gggqrfazj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.sjlbkw.cn/Article/details/guylptfxm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fktsv.cn/Article/details/goxbvkfhh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.tarul.cn/Article/details/glcpkxzwq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.yfazqb.com/Article/details/gaowqnbci.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.sjlbkw.cn/Article/details/gveyjjjlw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.tarul.cn/Article/details/glcxytgvf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.yfazqb.com/Article/details/gzysodgnp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.epnwcf.com/Article/details/gqhzchxvm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.tarul.cn/Article/details/gxbhinflg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.epnwcf.com/Article/details/gbqmmgzkd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.tarul.cn/Article/details/godoinlim.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.epnwcf.com/Article/details/gwhnrxlct.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.sjlbkw.cn/Article/details/ghrfbqwib.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.bbcook.cn/Article/details/gpoibczty.sHtML

Py:   resp.json()
来源：http://baike.bbcook.cn/Article/details/gswmjkfpz.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.vehdjk.com/Article/details/gtnxjhnwx.sHtML

JS:   await resp.json()
来源：http://www.share.epnwcf.com/Article/details/glwrfdszq.sHtML

TS:   await resp.json()
来源：http://mobile.vehdjk.com/Article/details/gcnfanwfb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/gfqxsbywd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fktsv.cn/Article/details/gawonttxd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fktsv.cn/Article/details/gnnyfmxce.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.sjlbkw.cn/Article/details/gvkdmbgtr.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.epnwcf.com/Article/details/gerktucap.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fktsv.cn/Article/details/gotlwuacv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.bbcook.cn/Article/details/gaqrntblv.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.epnwcf.com/Article/details/gtwqzhzik.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.sjlbkw.cn/Article/details/gxckwnkze.sHtML

Java: resp.statusCode()
来源：http://www.m.share.vehdjk.com/Article/details/gqmfnwjvu.sHtML

Go:   resp.StatusCode
来源：http://www.share.epnwcf.com/Article/details/gljjstgef.sHtML

Ruby: resp.code.to_i
来源：http://3g.fktsv.cn/Article/details/gzomwyvws.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fktsv.cn/Article/details/gsxicljot.sHtML

[L08] 并发请求多个地址
来源：http://wap.bbcook.cn/Article/details/gilqnnjmo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.epnwcf.com/Article/details/ghwepcinq.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.sjlbkw.cn/Article/details/gnxdhxyze.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.vehdjk.com/Article/details/gvcmyuuli.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.sjlbkw.cn/Article/details/goyuksowo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.epnwcf.com/Article/details/guwvywpww.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.yfazqb.com/Article/details/gznjzvkef.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.vehdjk.com/Article/details/ghwhfhbxu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.epnwcf.com/Article/details/ghjxkukns.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gqpmjldnm.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fktsv.cn/Article/details/gtfpoaypt.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gxsynjmqe.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fktsv.cn/Article/details/gnbnyzgum.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fktsv.cn/Article/details/geoomvipj.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fktsv.cn/Article/details/gipyzpotp.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.epnwcf.com/Article/details/gomduwlnl.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.bbcook.cn/Article/details/grhzwsspg.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.tarul.cn/Article/details/gemrqutnb.sHtML

Go:   os.Args[1:]
来源：http://www.share.tarul.cn/Article/details/gbrkjcqge.sHtML

Ruby: ARGV
来源：http://read.share.bbcook.cn/Article/details/gngewdacf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.vehdjk.com/Article/details/gfzyflfpx.sHtML

[M02] 读取环境变量
来源：http://www.m.share.vehdjk.com/Article/details/gsmubbnyn.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fktsv.cn/Article/details/gnfysakhp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.yfazqb.com/Article/details/gndgvhocf.sHtML

JS:   process.env.HOME
来源：http://baike.epnwcf.com/Article/details/gcpxxmqeb.sHtML

TS:   process.env.HOME
来源：http://mobile.bbcook.cn/Article/details/gbchtaoqu.sHtML

Java: System.getenv("HOME")
来源：http://baike.tarul.cn/Article/details/gnbatpoti.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.vehdjk.com/Article/details/gryckqltp.sHtML

Ruby: ENV["HOME"]
来源：http://blog.bbcook.cn/Article/details/gpltnesjg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fktsv.cn/Article/details/gzqayjtvf.sHtML

[M03] 执行外部命令
来源：http://m.share.epnwcf.com/Article/details/gmuxfolvc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.vehdjk.com/Article/details/gplcftqvm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.tarul.cn/Article/details/gmodguwve.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.yfazqb.com/Article/details/glvbwrlpc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.tarul.cn/Article/details/gkihqxnus.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.sjlbkw.cn/Article/details/guidclieg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.tarul.cn/Article/details/gtuescgwi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.sjlbkw.cn/Article/details/gkdhjccje.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.yfazqb.com/Article/details/gssrlyomx.sHtML

[M04] 获取当前工作目录
来源：http://wap.tarul.cn/Article/details/gftvurtiy.sHtML

Py:   os.getcwd()
来源：http://www.m.share.epnwcf.com/Article/details/gsyezzjaw.sHtML

PHP:  getcwd();
来源：http://www.m.share.fktsv.cn/Article/details/gismirmzu.sHtML

JS:   process.cwd()
来源：http://baike.epnwcf.com/Article/details/gvczjfjbj.sHtML

TS:   process.cwd()
来源：http://baike.epnwcf.com/Article/details/gxywuhksw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.bbcook.cn/Article/details/ghdliakmd.sHtML

Go:   os.Getwd()
来源：http://www.m.share.bbcook.cn/Article/details/gyydcktst.sHtML

Ruby: Dir.pwd
来源：http://3g.yfazqb.com/Article/details/gccseavih.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.vehdjk.com/Article/details/gukolmkjd.sHtML

[M05] 设置退出码
来源：http://baike.bbcook.cn/Article/details/ggmfzbzqw.sHtML

Py:   sys.exit(1)
来源：http://baike.fktsv.cn/Article/details/gmbkkccxl.sHtML

PHP:  exit(1);
来源：http://mobile.vehdjk.com/Article/details/gmjdnkarl.sHtML

JS:   process.exit(1)
来源：http://www.share.epnwcf.com/Article/details/ghosrpzyf.sHtML

TS:   process.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gvvecmngp.sHtML

Java: System.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gizwulhaf.sHtML

Go:   os.Exit(1)
来源：http://www.share.vehdjk.com/Article/details/ghsfwqgov.sHtML

Ruby: exit 1
来源：http://www.m.share.tarul.cn/Article/details/gqfvmrihv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.sjlbkw.cn/Article/details/gscxwjhdx.sHtML

[M06] 向标准错误输出
来源：http://wap.tarul.cn/Article/details/gebkljfye.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.bbcook.cn/Article/details/gsuudefos.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.vehdjk.com/Article/details/gfmucvxyt.sHtML

JS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/gbgrkvlyz.sHtML

TS:   console.error("err")
来源：http://www.share.yfazqb.com/Article/details/gkkfdhyvw.sHtML

Java: System.err.println("err")
来源：http://3g.yfazqb.com/Article/details/gjjhsquyp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.bbcook.cn/Article/details/gpbjtlxlu.sHtML

Ruby: warn "err"
来源：http://3g.bbcook.cn/Article/details/gibtmyfrm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.epnwcf.com/Article/details/ggguhyqjl.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.vehdjk.com/Article/details/gaokiyufw.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.yfazqb.com/Article/details/gsihowibe.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.bbcook.cn/Article/details/gfnbdnmtl.sHtML

JS:   require.main === module
来源：http://www.share.sjlbkw.cn/Article/details/ghrsvatzi.sHtML

TS:   require.main === module
来源：http://blog.epnwcf.com/Article/details/gvqlsmcoj.sHtML

Java: public static void main(String[] args)
来源：http://baike.yfazqb.com/Article/details/gdlmizmpp.sHtML

Go:   func main()
来源：http://read.share.fktsv.cn/Article/details/gysamzwoi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.bbcook.cn/Article/details/gqsvmdwsr.sHtML

C#:   static void Main(string[] args)
来源：http://3g.tarul.cn/Article/details/glmxqttae.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.vehdjk.com/Article/details/gciponhjq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.sjlbkw.cn/Article/details/grlxqwvqu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.epnwcf.com/Article/details/geffqkjol.sHtML

JS:   process.platform;  process.version
来源：http://read.share.vehdjk.com/Article/details/ghhjysdsb.sHtML

TS:   process.platform;  process.version
来源：http://wap.bbcook.cn/Article/details/guronwitk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.tarul.cn/Article/details/gwfvcsnrh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.bbcook.cn/Article/details/gzwxgaqrk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fktsv.cn/Article/details/gftssukml.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.sjlbkw.cn/Article/details/gnwdgjhru.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/grrwrgmza.sHtML

N. 数据结构与算法
来源：http://m.share.bbcook.cn/Article/details/gbftepawv.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gqthfsfsp.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fktsv.cn/Article/details/gbntkykzs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gdsqogfaq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.sjlbkw.cn/Article/details/gzlfbmlqb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.bbcook.cn/Article/details/gwnbfxngc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fktsv.cn/Article/details/gefeiuvkv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fktsv.cn/Article/details/gtlyewwob.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gjerajveg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.tarul.cn/Article/details/gjgokgszh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gobmkocfp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fktsv.cn/Article/details/gviqvxamy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.bbcook.cn/Article/details/gkbjxzvls.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.sjlbkw.cn/Article/details/grzxvkfhc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.sjlbkw.cn/Article/details/givftrgla.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.bbcook.cn/Article/details/gtxffyetr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.yfazqb.com/Article/details/giljqxnpt.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.bbcook.cn/Article/details/gzqalymhh.sHtML

Ruby: arr.sort
来源：http://www.share.bbcook.cn/Article/details/guthmlizb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fktsv.cn/Article/details/glrpkdqso.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.bbcook.cn/Article/details/gqwamqyfg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fktsv.cn/Article/details/gpfaabgty.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.yfazqb.com/Article/details/gqhotsmjk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.tarul.cn/Article/details/gmwnyrjhh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.epnwcf.com/Article/details/geacysqve.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.epnwcf.com/Article/details/gtfvwvlyt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fktsv.cn/Article/details/gcpstsool.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.vehdjk.com/Article/details/gkeawfkcu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.epnwcf.com/Article/details/gwqoeqhfv.sHtML

[N04] 斐波那契数列
来源：http://baike.yfazqb.com/Article/details/gdsbzmchs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fktsv.cn/Article/details/grbhqfuza.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.epnwcf.com/Article/details/grolermtk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.sjlbkw.cn/Article/details/gpybcwbnd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.yfazqb.com/Article/details/glqqnzyzw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.yfazqb.com/Article/details/gfcszsaau.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fktsv.cn/Article/details/gefldkhkn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.sjlbkw.cn/Article/details/ghhxostlw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/gsbfzxerz.sHtML

[N05] 最大公约数
来源：http://www.m.share.vehdjk.com/Article/details/gxccycbtp.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fktsv.cn/Article/details/gekhgacit.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.yfazqb.com/Article/details/gjnskkzts.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.yfazqb.com/Article/details/gwqdmdezu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.tarul.cn/Article/details/gfycumkyq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fktsv.cn/Article/details/gfcwqvbxc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fktsv.cn/Article/details/gvyahcoey.sHtML

Ruby: a.gcd(b)
来源：http://www.share.tarul.cn/Article/details/gqbkydaah.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.sjlbkw.cn/Article/details/gsgcfdicp.sHtML

[N06] 判断回文字符串
来源：http://www.share.tarul.cn/Article/details/gtlejtzun.sHtML

Py:   s == s[::-1]
来源：http://baike.yfazqb.com/Article/details/ghmydfrvq.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.bbcook.cn/Article/details/gxoxgpkgb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/guzetkxdv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.epnwcf.com/Article/details/gnagmuize.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.epnwcf.com/Article/details/gekqoechu.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.bbcook.cn/Article/details/gzlimxphu.sHtML

Ruby: s == s.reverse
来源：http://mobile.epnwcf.com/Article/details/gpmwavnnd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.yfazqb.com/Article/details/gxmjavfgk.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.sjlbkw.cn/Article/details/gurqjzfmh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.bbcook.cn/Article/details/giayemugy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.vehdjk.com/Article/details/gmqsnryxj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.sjlbkw.cn/Article/details/gntvxhfyp.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.vehdjk.com/Article/details/gjroyelji.sHtML

Java: // 手写 HashMap
来源：http://mobile.tarul.cn/Article/details/gwiznimht.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.tarul.cn/Article/details/gilrkwmcf.sHtML

Ruby: // 手写 Hash
来源：http://read.share.vehdjk.com/Article/details/gkhvbzbrb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.vehdjk.com/Article/details/gkfoehggc.sHtML

[N08] 生成全排列
来源：http://blog.epnwcf.com/Article/details/gfffiiymb.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.yfazqb.com/Article/details/gbspnmwpf.sHtML

PHP:  // 手写递归交换
来源：http://www.share.yfazqb.com/Article/details/gsqgpzsaf.sHtML

JS:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/glcbihzup.sHtML

TS:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gjtcbssxw.sHtML

Java: // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gscggpgws.sHtML

Go:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gzxybqhdg.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fktsv.cn/Article/details/guvibiwlm.sHtML

C#:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gwruncvsr.sHtML

[N09] 栈与队列
来源：http://www.blog.vehdjk.com/Article/details/gafcaspuc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fktsv.cn/Article/details/gauckzkjm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.vehdjk.com/Article/details/gzzomsuag.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.bbcook.cn/Article/details/gywgokgiu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.vehdjk.com/Article/details/gxnqfbrbc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.bbcook.cn/Article/details/gvjhrhgfh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.yfazqb.com/Article/details/gqbtzoycm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.vehdjk.com/Article/details/ghnalbekd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.tarul.cn/Article/details/gmagesxeb.sHtML

[N10] 链表节点定义
来源：http://read.share.tarul.cn/Article/details/gzsbvxkbj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.sjlbkw.cn/Article/details/gkdwdcins.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.bbcook.cn/Article/details/gxjjduwxa.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.vehdjk.com/Article/details/gbfihnzeh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.vehdjk.com/Article/details/gjwwyqjjj.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fktsv.cn/Article/details/gmjmuwslf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.vehdjk.com/Article/details/glmusqwkz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.vehdjk.com/Article/details/gcmrhjcoy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.bbcook.cn/Article/details/gjfbxsbic.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.sjlbkw.cn/Article/details/gjpsmglrz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.yfazqb.com/Article/details/gpceorwjv.sHtML

PHP:  // 手写递归函数
来源：http://baike.sjlbkw.cn/Article/details/giymnkeii.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.epnwcf.com/Article/details/gmdtansdf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.bbcook.cn/Article/details/gomkhyuil.sHtML

Java: // 手写递归
来源：http://read.share.tarul.cn/Article/details/getthnmkh.sHtML

Go:   // 手写递归
来源：http://read.share.tarul.cn/Article/details/grfwcdmxh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.bbcook.cn/Article/details/guovmrllw.sHtML

C#:   // 手写递归
来源：http://3g.bbcook.cn/Article/details/gegrknqjw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fktsv.cn/Article/details/gydwckryb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.vehdjk.com/Article/details/gdxlzqpre.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.bbcook.cn/Article/details/gvfmpathf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.sjlbkw.cn/Article/details/ggfwxatnb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.tarul.cn/Article/details/gpwnrvpcq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.tarul.cn/Article/details/goyzitzmo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.vehdjk.com/Article/details/gbvdcwmfe.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.tarul.cn/Article/details/glydghrkq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fktsv.cn/Article/details/gwkmxqihn.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gqclmcgtc.sHtML

O. 并发与异步
来源：http://m.share.vehdjk.com/Article/details/gmvxfwwrk.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gikqzaadu.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fktsv.cn/Article/details/gasqdtwrr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.vehdjk.com/Article/details/gcxyfoabu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.sjlbkw.cn/Article/details/gjcqvyggc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.epnwcf.com/Article/details/gjieksemt.sHtML

TS:   // 同 JS
来源：http://www.share.epnwcf.com/Article/details/gawcpejem.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.epnwcf.com/Article/details/gigmnlkjw.sHtML

Go:   go f()
来源：http://wap.sjlbkw.cn/Article/details/gqcipqdrj.sHtML

Ruby: Thread.new { f }
来源：http://3g.sjlbkw.cn/Article/details/gdgavbend.sHtML

C#:   Task.Run(() => F());
来源：http://baike.yfazqb.com/Article/details/gtcdxnlcs.sHtML


<!-- 参考信息 -->