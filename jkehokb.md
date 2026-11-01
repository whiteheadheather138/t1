代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fktsv.cn/Article/details/gdoqeqkih.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.yfazqb.com/Article/details/ghfhamhdl.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.bbcook.cn/Article/details/gcnxoafha.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.yfazqb.com/Article/details/gurntqidj.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.tarul.cn/Article/details/gprztzpis.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.yfazqb.com/Article/details/ghetrjkkt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.bbcook.cn/Article/details/gbadblrln.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fktsv.cn/Article/details/gscgfjmtd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.yfazqb.com/Article/details/gyzowzqot.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.epnwcf.com/Article/details/ghfxxkvbk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.bbcook.cn/Article/details/gtbqrnbqs.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.sjlbkw.cn/Article/details/gjersytrd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.yfazqb.com/Article/details/gnpaaquxm.sHtML

[K07] 进制转换
来源：http://www.m.share.tarul.cn/Article/details/gkhwjhosh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/glozgbcsk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.epnwcf.com/Article/details/gjbhotgdl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gqupvrmyy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gkykcehdp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gnorvnsrq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.sjlbkw.cn/Article/details/gtqmxgagg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fktsv.cn/Article/details/gquywdjsu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.epnwcf.com/Article/details/grfpdndmf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.sjlbkw.cn/Article/details/glbvfqemw.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fktsv.cn/Article/details/gomdhpzsf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.tarul.cn/Article/details/ggrbmqumr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.epnwcf.com/Article/details/gvjnesduq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.yfazqb.com/Article/details/gtnljijrf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fktsv.cn/Article/details/gkhtdwwjl.sHtML

Go:   encoding/gob
来源：http://www.share.epnwcf.com/Article/details/geebopsxq.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gtxuwqtwj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.vehdjk.com/Article/details/gavmamqto.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gelzyskyi.sHtML

L. 网络请求
来源：http://www.m.share.bbcook.cn/Article/details/ggodczzkj.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gtysccauc.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.sjlbkw.cn/Article/details/gspsmpfpi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.epnwcf.com/Article/details/ghdjobcgl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.tarul.cn/Article/details/geklcfwds.sHtML

JS:   await fetch(url)
来源：http://www.share.bbcook.cn/Article/details/gjvmtvoox.sHtML

TS:   await fetch(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gihbgxxaz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.sjlbkw.cn/Article/details/giaazglgb.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.sjlbkw.cn/Article/details/gydlikvet.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.tarul.cn/Article/details/gvecezniw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.epnwcf.com/Article/details/gkicwzyil.sHtML

[L02] 发送 POST JSON
来源：http://baike.bbcook.cn/Article/details/giflujqhr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.epnwcf.com/Article/details/ggdlysnni.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.yfazqb.com/Article/details/gxgzvdntn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.epnwcf.com/Article/details/gwiycchwu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.epnwcf.com/Article/details/gtnesstiv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fktsv.cn/Article/details/gvfthufod.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.tarul.cn/Article/details/gtkrvxade.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.tarul.cn/Article/details/gchhxcgrn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.tarul.cn/Article/details/gltfmrgod.sHtML

[L03] 设置自定义请求头
来源：http://www.share.vehdjk.com/Article/details/gxfhcqkiu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.yfazqb.com/Article/details/gduuilnma.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.bbcook.cn/Article/details/gdqwpbqcv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.epnwcf.com/Article/details/gutpjraoy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.tarul.cn/Article/details/gpfvieknw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fktsv.cn/Article/details/gibeeljwk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.bbcook.cn/Article/details/gujrszdbl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.vehdjk.com/Article/details/gfreecshf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.bbcook.cn/Article/details/glbtsiexm.sHtML

[L04] 设置超时
来源：http://read.share.epnwcf.com/Article/details/gabzxxodr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fktsv.cn/Article/details/gvzuumprc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.epnwcf.com/Article/details/gdhgqofqy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.vehdjk.com/Article/details/gsqgjcqnl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.epnwcf.com/Article/details/gzjnpnhzd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.yfazqb.com/Article/details/gjdjxarwo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.vehdjk.com/Article/details/gswgwjmfa.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.epnwcf.com/Article/details/gdhnvlgoe.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.vehdjk.com/Article/details/giidjrcwd.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.yfazqb.com/Article/details/gjobvpyyr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.sjlbkw.cn/Article/details/gwhvmpram.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnypmzxab.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fktsv.cn/Article/details/gpsxszicv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/gkfzgrskn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.yfazqb.com/Article/details/ghhkxgwsf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.tarul.cn/Article/details/gmejasins.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.epnwcf.com/Article/details/guopoymbp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.tarul.cn/Article/details/ggxjijsqn.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.vehdjk.com/Article/details/gdzxuorde.sHtML

Py:   resp.json()
来源：http://www.m.share.tarul.cn/Article/details/gfmktrzzg.sHtML

PHP:  json_decode($body, true);
来源：http://wap.yfazqb.com/Article/details/geqtaqfep.sHtML

JS:   await resp.json()
来源：http://baike.epnwcf.com/Article/details/gaksqwoju.sHtML

TS:   await resp.json()
来源：http://wap.tarul.cn/Article/details/gorvztvgy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fktsv.cn/Article/details/gnkhzqtir.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.epnwcf.com/Article/details/gzafotoak.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.epnwcf.com/Article/details/gfluciqpy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.yfazqb.com/Article/details/gvqkmyjsu.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.yfazqb.com/Article/details/gjyaigftg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.tarul.cn/Article/details/gauxdrdpc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.yfazqb.com/Article/details/grupelkqn.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.bbcook.cn/Article/details/gybythaqs.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.bbcook.cn/Article/details/gwilkktoq.sHtML

Java: resp.statusCode()
来源：http://m.share.bbcook.cn/Article/details/gdqvvxdke.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.yfazqb.com/Article/details/gozphfaxr.sHtML

Ruby: resp.code.to_i
来源：http://baike.bbcook.cn/Article/details/gdyuaghwu.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fktsv.cn/Article/details/gqiiokrxo.sHtML

[L08] 并发请求多个地址
来源：http://read.share.bbcook.cn/Article/details/gttmclczn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fktsv.cn/Article/details/gwjeuvkwv.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fktsv.cn/Article/details/gbhbskfgm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.tarul.cn/Article/details/ggkueutyb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.tarul.cn/Article/details/glijafbmc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.vehdjk.com/Article/details/gvrojdoub.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.epnwcf.com/Article/details/gfgiqvhua.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.yfazqb.com/Article/details/gzlewslmk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.yfazqb.com/Article/details/gjdmmkbzn.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gfktvozsm.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.sjlbkw.cn/Article/details/ggduhhakt.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gianabdwv.sHtML

[M01] 读取命令行参数
来源：http://baike.sjlbkw.cn/Article/details/gabxeulal.sHtML

Py:   sys.argv[1:]
来源：http://wap.fktsv.cn/Article/details/ghrnqqsqk.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fktsv.cn/Article/details/gehkajpim.sHtML

JS:   process.argv.slice(2)
来源：http://blog.vehdjk.com/Article/details/gvcnrxast.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.epnwcf.com/Article/details/gqrntpokq.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.sjlbkw.cn/Article/details/gjbohohmk.sHtML

Go:   os.Args[1:]
来源：http://wap.epnwcf.com/Article/details/grsqtjmlq.sHtML

Ruby: ARGV
来源：http://baike.vehdjk.com/Article/details/gdpnrjkgk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.vehdjk.com/Article/details/gctriyddl.sHtML

[M02] 读取环境变量
来源：http://wap.epnwcf.com/Article/details/gwpdeokho.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gqjwneagq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.tarul.cn/Article/details/gnzjtlfjl.sHtML

JS:   process.env.HOME
来源：http://m.share.sjlbkw.cn/Article/details/gpctsbhxm.sHtML

TS:   process.env.HOME
来源：http://www.share.epnwcf.com/Article/details/gvavfbtjy.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/guctvjelp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfyxppls.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.sjlbkw.cn/Article/details/gqlsqxpuf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.bbcook.cn/Article/details/gurscegqu.sHtML

[M03] 执行外部命令
来源：http://read.share.vehdjk.com/Article/details/gihlwviun.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.sjlbkw.cn/Article/details/gbomeblab.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.tarul.cn/Article/details/gjksoofbl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fktsv.cn/Article/details/gjllfsxfp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.bbcook.cn/Article/details/guljmfkgw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.bbcook.cn/Article/details/gcvwggfqg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.sjlbkw.cn/Article/details/gxdnhkuhs.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fktsv.cn/Article/details/glxnhzusp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.epnwcf.com/Article/details/gwirimmza.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.yfazqb.com/Article/details/gbpzsofyl.sHtML

Py:   os.getcwd()
来源：http://wap.yfazqb.com/Article/details/ggivvbitd.sHtML

PHP:  getcwd();
来源：http://read.share.tarul.cn/Article/details/gtlcdbpab.sHtML

JS:   process.cwd()
来源：http://wap.yfazqb.com/Article/details/glbsggdyv.sHtML

TS:   process.cwd()
来源：http://www.m.share.epnwcf.com/Article/details/gjtnuwdlj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.bbcook.cn/Article/details/gejfrqebt.sHtML

Go:   os.Getwd()
来源：http://www.blog.epnwcf.com/Article/details/gaycnzfun.sHtML

Ruby: Dir.pwd
来源：http://blog.yfazqb.com/Article/details/guoiomqke.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.yfazqb.com/Article/details/gmnqvzeal.sHtML

[M05] 设置退出码
来源：http://www.blog.fktsv.cn/Article/details/gezeoqwoh.sHtML

Py:   sys.exit(1)
来源：http://m.share.tarul.cn/Article/details/gqpnwgetk.sHtML

PHP:  exit(1);
来源：http://www.blog.bbcook.cn/Article/details/gcbhthdha.sHtML

JS:   process.exit(1)
来源：http://baike.vehdjk.com/Article/details/gttiorbxj.sHtML

TS:   process.exit(1)
来源：http://www.share.vehdjk.com/Article/details/glutcwnrd.sHtML

Java: System.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gwnqclqil.sHtML

Go:   os.Exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gfjkjkfkx.sHtML

Ruby: exit 1
来源：http://m.share.bbcook.cn/Article/details/gtgexqnzi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.sjlbkw.cn/Article/details/gaqpklnjm.sHtML

[M06] 向标准错误输出
来源：http://blog.yfazqb.com/Article/details/gvdmldgnb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.tarul.cn/Article/details/gqbjbqnli.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.epnwcf.com/Article/details/glxrzaoru.sHtML

JS:   console.error("err")
来源：http://wap.bbcook.cn/Article/details/glehjubto.sHtML

TS:   console.error("err")
来源：http://mobile.fktsv.cn/Article/details/gziritkeu.sHtML

Java: System.err.println("err")
来源：http://blog.epnwcf.com/Article/details/gascqugzt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.epnwcf.com/Article/details/gxmemsmvg.sHtML

Ruby: warn "err"
来源：http://www.share.yfazqb.com/Article/details/gmahzvius.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.epnwcf.com/Article/details/gstpwlbtf.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.vehdjk.com/Article/details/gjrrapqdh.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.tarul.cn/Article/details/gwcspoemc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fktsv.cn/Article/details/gqlagbvtw.sHtML

JS:   require.main === module
来源：http://read.share.epnwcf.com/Article/details/grmdrsqev.sHtML

TS:   require.main === module
来源：http://blog.tarul.cn/Article/details/gvnihzygw.sHtML

Java: public static void main(String[] args)
来源：http://read.share.yfazqb.com/Article/details/gbaltybgj.sHtML

Go:   func main()
来源：http://read.share.fktsv.cn/Article/details/gaubibvvv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.bbcook.cn/Article/details/gvkvxexrx.sHtML

C#:   static void Main(string[] args)
来源：http://baike.sjlbkw.cn/Article/details/ghjgfkpub.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.vehdjk.com/Article/details/gpvyhdpmr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fktsv.cn/Article/details/glhyalaeg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.vehdjk.com/Article/details/grmhphnzk.sHtML

JS:   process.platform;  process.version
来源：http://read.share.epnwcf.com/Article/details/gyqjkvtfm.sHtML

TS:   process.platform;  process.version
来源：http://m.share.sjlbkw.cn/Article/details/gunexyaxm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.vehdjk.com/Article/details/gecgflxnx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.yfazqb.com/Article/details/gnopautbe.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.bbcook.cn/Article/details/gzhgnidwu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.vehdjk.com/Article/details/gbdjasobt.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gbkgiwigs.sHtML

N. 数据结构与算法
来源：http://m.share.fktsv.cn/Article/details/gdwxzyaok.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gcgkrinad.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.epnwcf.com/Article/details/gbshcjspm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gxbxeopah.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/gekzrsfud.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.epnwcf.com/Article/details/gxnidrjnm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gnzjstjmk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gvjjdjobf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fktsv.cn/Article/details/gcjhyeyyw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.epnwcf.com/Article/details/gponmdzhd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gzairulpc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.yfazqb.com/Article/details/gmqnpupvq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.vehdjk.com/Article/details/gbxrzjiel.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.tarul.cn/Article/details/gpdqcliyy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.tarul.cn/Article/details/gwjarkkzr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.epnwcf.com/Article/details/gqzourqel.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.vehdjk.com/Article/details/gnbzeorao.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.bbcook.cn/Article/details/gjxbxicph.sHtML

Ruby: arr.sort
来源：http://3g.epnwcf.com/Article/details/gemxqrgsh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fktsv.cn/Article/details/gmejcewyl.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fktsv.cn/Article/details/gdkghgjeh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fktsv.cn/Article/details/gntokktif.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.tarul.cn/Article/details/grlauonwp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.sjlbkw.cn/Article/details/ghvwaymtq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.epnwcf.com/Article/details/gxdnzoscz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fktsv.cn/Article/details/gzmpwbnkf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.sjlbkw.cn/Article/details/gpbxyjvcr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.epnwcf.com/Article/details/gddaajfyp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.bbcook.cn/Article/details/gaprvgszk.sHtML

[N04] 斐波那契数列
来源：http://www.blog.epnwcf.com/Article/details/gbrxxvxdf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.yfazqb.com/Article/details/gzthaiexj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.yfazqb.com/Article/details/ggqytnvfu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.vehdjk.com/Article/details/ghogheooo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.bbcook.cn/Article/details/gpfxlycku.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.sjlbkw.cn/Article/details/gyaqdrrod.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.sjlbkw.cn/Article/details/gpzrmyood.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fktsv.cn/Article/details/gsvhykjjv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/gqclxqkyz.sHtML

[N05] 最大公约数
来源：http://mobile.yfazqb.com/Article/details/gqtqgnxuj.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.tarul.cn/Article/details/gczompbbg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.bbcook.cn/Article/details/grctalils.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fktsv.cn/Article/details/giejckkum.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fktsv.cn/Article/details/gdwxiqxwa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.epnwcf.com/Article/details/grevbiljb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.yfazqb.com/Article/details/gtameihas.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.epnwcf.com/Article/details/gebhcnaeg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.epnwcf.com/Article/details/gcpthrtas.sHtML

[N06] 判断回文字符串
来源：http://wap.fktsv.cn/Article/details/gypgzgrcr.sHtML

Py:   s == s[::-1]
来源：http://blog.sjlbkw.cn/Article/details/gbcxunujz.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.vehdjk.com/Article/details/gnljisexd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/gxfabzopd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/gpfjhcinc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.tarul.cn/Article/details/ghigthifw.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.epnwcf.com/Article/details/gxsehwwnj.sHtML

Ruby: s == s.reverse
来源：http://baike.bbcook.cn/Article/details/glbuhqwyi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcpodtyr.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.yfazqb.com/Article/details/grsgmfnuh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.bbcook.cn/Article/details/gaxabaynp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.yfazqb.com/Article/details/gtndxkejw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.yfazqb.com/Article/details/gwellpzat.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.epnwcf.com/Article/details/ghfumotns.sHtML

Java: // 手写 HashMap
来源：http://m.share.tarul.cn/Article/details/gikhmfvsh.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.yfazqb.com/Article/details/gjkqjpert.sHtML

Ruby: // 手写 Hash
来源：http://blog.vehdjk.com/Article/details/ghmqzemro.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.yfazqb.com/Article/details/gnyimsgoz.sHtML

[N08] 生成全排列
来源：http://blog.fktsv.cn/Article/details/gpeiibytq.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.bbcook.cn/Article/details/gukgesday.sHtML

PHP:  // 手写递归交换
来源：http://3g.vehdjk.com/Article/details/gjyszgekl.sHtML

JS:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/gpbbcltbw.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gspooerjc.sHtML

Java: // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gyxnhfhae.sHtML

Go:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gftmieuxv.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fktsv.cn/Article/details/ggqtpvdur.sHtML

C#:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gflsamawd.sHtML

[N09] 栈与队列
来源：http://wap.bbcook.cn/Article/details/gskirqkqn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.bbcook.cn/Article/details/gvsapnomp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.epnwcf.com/Article/details/gdjuexuav.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gxvmtxxgm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.bbcook.cn/Article/details/ginhcdsqx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.yfazqb.com/Article/details/gegtvbhui.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.bbcook.cn/Article/details/gxkzehkrk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.bbcook.cn/Article/details/gekzyamku.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.tarul.cn/Article/details/gssubmnvk.sHtML

[N10] 链表节点定义
来源：http://3g.tarul.cn/Article/details/gxaskmbcp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.yfazqb.com/Article/details/gyetvelux.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.bbcook.cn/Article/details/ggydqzrwz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.vehdjk.com/Article/details/gpbrelzhx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.epnwcf.com/Article/details/gctypztgb.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.epnwcf.com/Article/details/glbdizkun.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.sjlbkw.cn/Article/details/gyoerwqbj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.yfazqb.com/Article/details/gdaetlfpg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fktsv.cn/Article/details/gkcqvpebx.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.tarul.cn/Article/details/gwynnkfvk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fktsv.cn/Article/details/gtqkzfibx.sHtML

PHP:  // 手写递归函数
来源：http://www.share.yfazqb.com/Article/details/gyrywdeju.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.sjlbkw.cn/Article/details/goxsbaegv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.sjlbkw.cn/Article/details/gsontlcol.sHtML

Java: // 手写递归
来源：http://wap.fktsv.cn/Article/details/gbebjrbuq.sHtML

Go:   // 手写递归
来源：http://blog.bbcook.cn/Article/details/gkkruqtxv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fktsv.cn/Article/details/gfflhukfv.sHtML

C#:   // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/gwbzifhzh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.sjlbkw.cn/Article/details/gbcpgnaad.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.vehdjk.com/Article/details/gnkpvwszu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.yfazqb.com/Article/details/gyxovlxth.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.tarul.cn/Article/details/gqyvdlcgs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.bbcook.cn/Article/details/gamivzqfb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.epnwcf.com/Article/details/gwutslkeo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.tarul.cn/Article/details/gkdglidsq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.epnwcf.com/Article/details/gcdwoshap.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gtmuhigwm.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gdqzchyqr.sHtML

O. 并发与异步
来源：http://m.share.bbcook.cn/Article/details/gcfcldvdb.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gtzhmfzbt.sHtML

[O01] 启动一个线程
来源：http://m.share.bbcook.cn/Article/details/grthuaylu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.sjlbkw.cn/Article/details/gatvasuay.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fktsv.cn/Article/details/gdacaavpv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.vehdjk.com/Article/details/gypamhfsj.sHtML

TS:   // 同 JS
来源：http://m.share.sjlbkw.cn/Article/details/gzicszscv.sHtML


<!-- 参考信息 -->