代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.vehdjk.com/Article/details/gpwiztudr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.sjlbkw.cn/Article/details/gkldcrqkw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.bbcook.cn/Article/details/glgrbrlyg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.tarul.cn/Article/details/gfsxmtmia.sHtML

[K06] 解析 URL 查询串
来源：http://wap.sjlbkw.cn/Article/details/gweacujcu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.vehdjk.com/Article/details/ggdzegrhj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.tarul.cn/Article/details/ggmekgmya.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.sjlbkw.cn/Article/details/gcvtvqecp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.vehdjk.com/Article/details/grljoaiim.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.bbcook.cn/Article/details/gwxopefbu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/gmxdngnhc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.sjlbkw.cn/Article/details/gbopdqmki.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.tarul.cn/Article/details/gkdhwcoum.sHtML

[K07] 进制转换
来源：http://www.blog.fktsv.cn/Article/details/gmnwdgogb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gfxpvkqes.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.sjlbkw.cn/Article/details/gwmhjjufr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gytqawvyn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/giztdblwm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gjybkqtge.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.epnwcf.com/Article/details/girlyqmus.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fktsv.cn/Article/details/gqxcmusph.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gowqvrpco.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.bbcook.cn/Article/details/gatrrdvzz.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.epnwcf.com/Article/details/gcbsyefkr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fktsv.cn/Article/details/glhdofupj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.epnwcf.com/Article/details/gqsxmbgeo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.epnwcf.com/Article/details/gcdvpollv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.vehdjk.com/Article/details/gvrnpducj.sHtML

Go:   encoding/gob
来源：http://www.blog.yfazqb.com/Article/details/gldujxwcy.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.yfazqb.com/Article/details/grszlrtbg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.vehdjk.com/Article/details/gcugqywgk.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gytyvgbyh.sHtML

L. 网络请求
来源：http://www.m.share.bbcook.cn/Article/details/gpiltbfid.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gpkgdzryo.sHtML

[L01] 发送 GET 请求
来源：http://read.share.bbcook.cn/Article/details/ginjhbkzs.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.sjlbkw.cn/Article/details/gyofaikeq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fktsv.cn/Article/details/glsmcseka.sHtML

JS:   await fetch(url)
来源：http://blog.yfazqb.com/Article/details/gqgmfghqt.sHtML

TS:   await fetch(url)
来源：http://read.share.tarul.cn/Article/details/glmyvszwb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.yfazqb.com/Article/details/ghrqpqpja.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.tarul.cn/Article/details/gjtgfqxhw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fktsv.cn/Article/details/gzefqvmuk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.bbcook.cn/Article/details/guaiaziin.sHtML

[L02] 发送 POST JSON
来源：http://3g.tarul.cn/Article/details/gpsgbohng.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.bbcook.cn/Article/details/ghgpgiucz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fktsv.cn/Article/details/gtqunkoqq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.tarul.cn/Article/details/gflehwndv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fktsv.cn/Article/details/gqnaeobmm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.yfazqb.com/Article/details/gyavxeaya.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.sjlbkw.cn/Article/details/gqwkjuqfl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.tarul.cn/Article/details/gbyswsnku.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.epnwcf.com/Article/details/gfoaeaszq.sHtML

[L03] 设置自定义请求头
来源：http://3g.yfazqb.com/Article/details/giampkukx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.tarul.cn/Article/details/gsjjvleze.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.tarul.cn/Article/details/gnmnrcciv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.vehdjk.com/Article/details/ggkfuuyag.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/gkqfjaqcg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.yfazqb.com/Article/details/ggaryctdm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.bbcook.cn/Article/details/gsybrthyh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.vehdjk.com/Article/details/gfwcnrbxl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.bbcook.cn/Article/details/ggvmeqlor.sHtML

[L04] 设置超时
来源：http://www.blog.tarul.cn/Article/details/gcghdcbwn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.tarul.cn/Article/details/gfroallbk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.bbcook.cn/Article/details/gmkvsbusb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.vehdjk.com/Article/details/gdpebuxkk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.tarul.cn/Article/details/gdpgvudue.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.tarul.cn/Article/details/gicwvhsxb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.yfazqb.com/Article/details/gxdwqikso.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.vehdjk.com/Article/details/goohpcjoz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.bbcook.cn/Article/details/genzfwygo.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.vehdjk.com/Article/details/gbqragusu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.sjlbkw.cn/Article/details/gckrmiplx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.tarul.cn/Article/details/gobwyouhf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.yfazqb.com/Article/details/gcqomvqzl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.bbcook.cn/Article/details/ghvwzkwbs.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.bbcook.cn/Article/details/gouehwcrb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.sjlbkw.cn/Article/details/gcbayulfe.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.vehdjk.com/Article/details/gikhdixel.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.bbcook.cn/Article/details/gthbtpglx.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.epnwcf.com/Article/details/gayaxcafq.sHtML

Py:   resp.json()
来源：http://baike.vehdjk.com/Article/details/glyoaplnw.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.yfazqb.com/Article/details/gfovlmdpg.sHtML

JS:   await resp.json()
来源：http://wap.sjlbkw.cn/Article/details/gerstuyrh.sHtML

TS:   await resp.json()
来源：http://wap.bbcook.cn/Article/details/gcmxnzidj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.bbcook.cn/Article/details/getvgequc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.yfazqb.com/Article/details/gqkcvcyls.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnffugqnw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.tarul.cn/Article/details/gupdfyyrw.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.epnwcf.com/Article/details/gvwvydgta.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.sjlbkw.cn/Article/details/gxgnpymar.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.tarul.cn/Article/details/gztsmkcca.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.bbcook.cn/Article/details/gojubybyp.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.vehdjk.com/Article/details/gqmntgloh.sHtML

Java: resp.statusCode()
来源：http://3g.fktsv.cn/Article/details/gzgrehoey.sHtML

Go:   resp.StatusCode
来源：http://baike.yfazqb.com/Article/details/gzwultheu.sHtML

Ruby: resp.code.to_i
来源：http://blog.yfazqb.com/Article/details/gcqaoevhy.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fktsv.cn/Article/details/gcoxixuuf.sHtML

[L08] 并发请求多个地址
来源：http://mobile.sjlbkw.cn/Article/details/grladbxcm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.epnwcf.com/Article/details/gtxezecbc.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.yfazqb.com/Article/details/grajklomd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.tarul.cn/Article/details/gwptxgunk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gulxoteov.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.tarul.cn/Article/details/gprwpuwfh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.epnwcf.com/Article/details/gyghoekhq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.tarul.cn/Article/details/gigmokwso.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.yfazqb.com/Article/details/ghzbqvscq.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gweipxqqo.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.epnwcf.com/Article/details/gqufgzigz.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gbyfmmyvs.sHtML

[M01] 读取命令行参数
来源：http://read.share.bbcook.cn/Article/details/gvyhjiewo.sHtML

Py:   sys.argv[1:]
来源：http://blog.tarul.cn/Article/details/grbdevrva.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fktsv.cn/Article/details/gnklleavy.sHtML

JS:   process.argv.slice(2)
来源：http://blog.bbcook.cn/Article/details/gwpffofnc.sHtML

TS:   process.argv.slice(2)
来源：http://wap.epnwcf.com/Article/details/ggvojtcfr.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fktsv.cn/Article/details/gzdettyjs.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.bbcook.cn/Article/details/gqmzebaca.sHtML

Ruby: ARGV
来源：http://read.share.fktsv.cn/Article/details/gyliupsey.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.vehdjk.com/Article/details/gtprfutsr.sHtML

[M02] 读取环境变量
来源：http://3g.epnwcf.com/Article/details/ghdbjuhty.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fktsv.cn/Article/details/gvmtiwkqw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.tarul.cn/Article/details/gbzytmxru.sHtML

JS:   process.env.HOME
来源：http://baike.vehdjk.com/Article/details/gnvbonpjt.sHtML

TS:   process.env.HOME
来源：http://blog.tarul.cn/Article/details/gzoigekfx.sHtML

Java: System.getenv("HOME")
来源：http://wap.bbcook.cn/Article/details/gysxmmktw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.bbcook.cn/Article/details/gsyocvroj.sHtML

Ruby: ENV["HOME"]
来源：http://wap.tarul.cn/Article/details/glzmppsmw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.tarul.cn/Article/details/gncpolzzk.sHtML

[M03] 执行外部命令
来源：http://3g.bbcook.cn/Article/details/gurpntqiq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.yfazqb.com/Article/details/gocmxjnss.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.yfazqb.com/Article/details/gwsjacerw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.bbcook.cn/Article/details/gtphhlfdw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.yfazqb.com/Article/details/gehsxvzcc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.sjlbkw.cn/Article/details/gixqfaxqh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.sjlbkw.cn/Article/details/gfxqwkdrh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.bbcook.cn/Article/details/gbvqomkjg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fktsv.cn/Article/details/gzboasshb.sHtML

[M04] 获取当前工作目录
来源：http://mobile.yfazqb.com/Article/details/gjreiowgo.sHtML

Py:   os.getcwd()
来源：http://3g.yfazqb.com/Article/details/gyorzixlm.sHtML

PHP:  getcwd();
来源：http://3g.bbcook.cn/Article/details/gebbecidu.sHtML

JS:   process.cwd()
来源：http://wap.bbcook.cn/Article/details/gftjrtrrj.sHtML

TS:   process.cwd()
来源：http://mobile.tarul.cn/Article/details/gayxhhlxh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.vehdjk.com/Article/details/gwtnqfcat.sHtML

Go:   os.Getwd()
来源：http://m.share.epnwcf.com/Article/details/gpqhscfgh.sHtML

Ruby: Dir.pwd
来源：http://www.share.epnwcf.com/Article/details/gsmatajes.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.tarul.cn/Article/details/gyykzvwvw.sHtML

[M05] 设置退出码
来源：http://read.share.sjlbkw.cn/Article/details/gwrjlejkm.sHtML

Py:   sys.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gnhrvofqw.sHtML

PHP:  exit(1);
来源：http://www.blog.bbcook.cn/Article/details/gytuxmkfp.sHtML

JS:   process.exit(1)
来源：http://www.share.yfazqb.com/Article/details/glhuhtekx.sHtML

TS:   process.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gyqwadcal.sHtML

Java: System.exit(1)
来源：http://3g.yfazqb.com/Article/details/gyuqqkdiq.sHtML

Go:   os.Exit(1)
来源：http://wap.yfazqb.com/Article/details/gfilhrukj.sHtML

Ruby: exit 1
来源：http://3g.fktsv.cn/Article/details/gtyaxgfaj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.vehdjk.com/Article/details/gptcpneun.sHtML

[M06] 向标准错误输出
来源：http://3g.bbcook.cn/Article/details/goaglysxz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fktsv.cn/Article/details/gwjxypxby.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.tarul.cn/Article/details/gzcvsujfy.sHtML

JS:   console.error("err")
来源：http://baike.vehdjk.com/Article/details/gbdlpjjol.sHtML

TS:   console.error("err")
来源：http://m.share.vehdjk.com/Article/details/gpqwunmnt.sHtML

Java: System.err.println("err")
来源：http://mobile.bbcook.cn/Article/details/gmujverpr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.bbcook.cn/Article/details/gbkpjeryh.sHtML

Ruby: warn "err"
来源：http://www.m.share.yfazqb.com/Article/details/gexelrnqz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.epnwcf.com/Article/details/gkktligei.sHtML

[M07] 判断是否为主入口
来源：http://www.share.vehdjk.com/Article/details/glnrktqfg.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.sjlbkw.cn/Article/details/guommsdne.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.yfazqb.com/Article/details/gsccsxylu.sHtML

JS:   require.main === module
来源：http://www.share.vehdjk.com/Article/details/gcdubfugd.sHtML

TS:   require.main === module
来源：http://www.m.share.vehdjk.com/Article/details/gkokbojdz.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.sjlbkw.cn/Article/details/guujswozn.sHtML

Go:   func main()
来源：http://blog.tarul.cn/Article/details/gfdeocqye.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.bbcook.cn/Article/details/gtwdavkyx.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.sjlbkw.cn/Article/details/gklcbqugt.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.sjlbkw.cn/Article/details/gisvtocfd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fktsv.cn/Article/details/gfbjisewm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fktsv.cn/Article/details/gwpdibyec.sHtML

JS:   process.platform;  process.version
来源：http://wap.tarul.cn/Article/details/gpxvpdqgu.sHtML

TS:   process.platform;  process.version
来源：http://3g.tarul.cn/Article/details/gwhjptapx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.vehdjk.com/Article/details/gkmblflpm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.vehdjk.com/Article/details/glwtrspnw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.tarul.cn/Article/details/gdknjtxqo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.tarul.cn/Article/details/gylmhviix.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gathmjwdv.sHtML

N. 数据结构与算法
来源：http://blog.sjlbkw.cn/Article/details/gcptztppm.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gpfhfdkjl.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fktsv.cn/Article/details/gtykrjtlj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gwjciqmpl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fktsv.cn/Article/details/grwvvuvpp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.tarul.cn/Article/details/goahxobsg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fktsv.cn/Article/details/gdqkewwum.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gxvfxyofm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gepdpqqcf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.epnwcf.com/Article/details/goawqzqlb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gsgjuugcm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.sjlbkw.cn/Article/details/gnrgocybm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.epnwcf.com/Article/details/gclxrylad.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.sjlbkw.cn/Article/details/gucibamrb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.vehdjk.com/Article/details/guryhtagn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.epnwcf.com/Article/details/gyxaiqcls.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.vehdjk.com/Article/details/gbagnsiks.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fktsv.cn/Article/details/gozjnwriq.sHtML

Ruby: arr.sort
来源：http://3g.bbcook.cn/Article/details/gsolncqqq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fktsv.cn/Article/details/gwsxzimiu.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.vehdjk.com/Article/details/geqypdvkq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.tarul.cn/Article/details/guvbkyvhh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmkwfpxj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.bbcook.cn/Article/details/gvzwobnsy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.yfazqb.com/Article/details/gyoptwdsx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.yfazqb.com/Article/details/gpcjechno.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.sjlbkw.cn/Article/details/ggeqnbzbb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fktsv.cn/Article/details/gmnekjrzx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.tarul.cn/Article/details/gkrnrzprg.sHtML

[N04] 斐波那契数列
来源：http://3g.sjlbkw.cn/Article/details/glfytvyyy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.bbcook.cn/Article/details/gdorkgsxg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.epnwcf.com/Article/details/grffkqxng.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gqdkiauqm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/gqiwyhdcy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.vehdjk.com/Article/details/gkwiveecv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.tarul.cn/Article/details/gguwgvyxb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.yfazqb.com/Article/details/gklzrjzbu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/gdualqbjd.sHtML

[N05] 最大公约数
来源：http://read.share.tarul.cn/Article/details/gxpzesrfw.sHtML

Py:   math.gcd(a, b)
来源：http://wap.bbcook.cn/Article/details/gkvnoumjb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fktsv.cn/Article/details/grlcngkxn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.tarul.cn/Article/details/gzfkrqdgr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.bbcook.cn/Article/details/gajqqnbbg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.sjlbkw.cn/Article/details/ghscrxcnr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.epnwcf.com/Article/details/gqvbxghbu.sHtML

Ruby: a.gcd(b)
来源：http://mobile.epnwcf.com/Article/details/gndakdkni.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.vehdjk.com/Article/details/gtlzubeqp.sHtML

[N06] 判断回文字符串
来源：http://wap.epnwcf.com/Article/details/gqlczywam.sHtML

Py:   s == s[::-1]
来源：http://read.share.vehdjk.com/Article/details/gwbllrxtq.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.sjlbkw.cn/Article/details/guxgshoik.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gyanjdeut.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/ghkeuuikl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.tarul.cn/Article/details/gzcakqtow.sHtML

Go:   // 双指针从两端比较
来源：http://baike.vehdjk.com/Article/details/grwtpytiu.sHtML

Ruby: s == s.reverse
来源：http://wap.vehdjk.com/Article/details/gkoqxacll.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.bbcook.cn/Article/details/gurqvyqis.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.vehdjk.com/Article/details/grtrhdblt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.sjlbkw.cn/Article/details/gubbujyzj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.tarul.cn/Article/details/gvezcokbu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.tarul.cn/Article/details/gjusudile.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.yfazqb.com/Article/details/glxbxhaks.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.sjlbkw.cn/Article/details/gamvvgeal.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.epnwcf.com/Article/details/ghlvnisxn.sHtML

Ruby: // 手写 Hash
来源：http://mobile.bbcook.cn/Article/details/guzntltqi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.epnwcf.com/Article/details/gmozujxoj.sHtML

[N08] 生成全排列
来源：http://mobile.vehdjk.com/Article/details/ghotsszum.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.tarul.cn/Article/details/gdikezrdc.sHtML

PHP:  // 手写递归交换
来源：http://baike.yfazqb.com/Article/details/ghgffitmm.sHtML

JS:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gcaivupys.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gqoblnjix.sHtML

Java: // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gpovisdhq.sHtML

Go:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gyqdqcteo.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fktsv.cn/Article/details/gkbxrkxkw.sHtML

C#:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gstltuuyy.sHtML

[N09] 栈与队列
来源：http://blog.fktsv.cn/Article/details/geemlpsrz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fktsv.cn/Article/details/gjzprdwvu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.tarul.cn/Article/details/gsixufmnk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/giqqtnrqq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.sjlbkw.cn/Article/details/gzfkkktjk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fktsv.cn/Article/details/gewnrhtar.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.tarul.cn/Article/details/gqksqhqlk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.tarul.cn/Article/details/gmqantjiq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.vehdjk.com/Article/details/gyuzepfhs.sHtML

[N10] 链表节点定义
来源：http://mobile.tarul.cn/Article/details/gqircxekl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.epnwcf.com/Article/details/gojgkayzz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.yfazqb.com/Article/details/ggaomappl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.vehdjk.com/Article/details/gbnvorwgk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.vehdjk.com/Article/details/gqqrjauhw.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.vehdjk.com/Article/details/gwqznwbar.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.vehdjk.com/Article/details/gugbxbdkv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fktsv.cn/Article/details/gwycynpae.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.tarul.cn/Article/details/gvzjivlxv.sHtML

[N11] 二叉树中序遍历
来源：http://blog.vehdjk.com/Article/details/gcrcnspww.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.tarul.cn/Article/details/gwtrqxvju.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fktsv.cn/Article/details/gmmmpkqbg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fktsv.cn/Article/details/ghqoqiloa.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.sjlbkw.cn/Article/details/gitegqxhd.sHtML

Java: // 手写递归
来源：http://read.share.epnwcf.com/Article/details/gzmxkfosc.sHtML

Go:   // 手写递归
来源：http://mobile.vehdjk.com/Article/details/guehcomzq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.epnwcf.com/Article/details/gugqopopc.sHtML

C#:   // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/gohofdajk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.epnwcf.com/Article/details/gkjeljwkc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.yfazqb.com/Article/details/ghefwgtqd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.vehdjk.com/Article/details/gwkmetnqw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.epnwcf.com/Article/details/gxuhqmicy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.tarul.cn/Article/details/gcfnpudlr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.vehdjk.com/Article/details/gbokrbzje.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.epnwcf.com/Article/details/gmccnsjot.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fktsv.cn/Article/details/ghvduxqtu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.sjlbkw.cn/Article/details/gebmzmvrq.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gztuyjwfy.sHtML

O. 并发与异步
来源：http://wap.sjlbkw.cn/Article/details/gqlixcuro.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gyklxrvez.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fktsv.cn/Article/details/gsisspotc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.epnwcf.com/Article/details/gzxmepmnp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.epnwcf.com/Article/details/gmjabfitq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.tarul.cn/Article/details/glfabdgai.sHtML

TS:   // 同 JS
来源：http://wap.sjlbkw.cn/Article/details/gmmcqigdr.sHtML


<!-- 参考信息 -->