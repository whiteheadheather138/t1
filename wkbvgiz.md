代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.vehdjk.com/Article/details/gxdivoxtp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.tarul.cn/Article/details/gvscyriwh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.sjlbkw.cn/Article/details/ggkkixmmu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/gxsmzlgbo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.sjlbkw.cn/Article/details/gmqtwqauc.sHtML

[K07] 进制转换
来源：http://3g.fktsv.cn/Article/details/gencezmdb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gkocsktcg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.tarul.cn/Article/details/grmmxmpdt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.tarul.cn/Article/details/grffkpmkw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.tarul.cn/Article/details/gbqevmfuk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/ghatrqnsh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.vehdjk.com/Article/details/gzllaesdm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.yfazqb.com/Article/details/grmhtxqnt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/gzhcynhvz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.vehdjk.com/Article/details/gujlpyfwn.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.tarul.cn/Article/details/gpdusnvhx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.vehdjk.com/Article/details/grduunxhz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.yfazqb.com/Article/details/gnldsmjtd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.tarul.cn/Article/details/garzmctji.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fktsv.cn/Article/details/ghnczipqo.sHtML

Go:   encoding/gob
来源：http://m.share.epnwcf.com/Article/details/gidruaevj.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.sjlbkw.cn/Article/details/gzymcbvep.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.sjlbkw.cn/Article/details/gnfexjdws.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gjduydiig.sHtML

L. 网络请求
来源：http://www.blog.yfazqb.com/Article/details/gswmartji.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ggbxlohdq.sHtML

[L01] 发送 GET 请求
来源：http://baike.yfazqb.com/Article/details/gnbzxmyaa.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.bbcook.cn/Article/details/gagxelqzk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.yfazqb.com/Article/details/gsvsopuzn.sHtML

JS:   await fetch(url)
来源：http://www.share.vehdjk.com/Article/details/gwjefdkuy.sHtML

TS:   await fetch(url)
来源：http://www.blog.fktsv.cn/Article/details/gugfgdhtq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.sjlbkw.cn/Article/details/gkvovbdzb.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.bbcook.cn/Article/details/gpuurxlzm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.bbcook.cn/Article/details/ghvvsmzoh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.epnwcf.com/Article/details/gpdbfhfhx.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.bbcook.cn/Article/details/gchdtuczr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.bbcook.cn/Article/details/gjssnwvst.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.bbcook.cn/Article/details/gllwcezok.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.sjlbkw.cn/Article/details/ghnlruypb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.tarul.cn/Article/details/geowvzrrx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.sjlbkw.cn/Article/details/ggajjecsy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.sjlbkw.cn/Article/details/ggvmnyzdq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.vehdjk.com/Article/details/goqnlngwi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.vehdjk.com/Article/details/gymmdakab.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.epnwcf.com/Article/details/gnkhallvs.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.bbcook.cn/Article/details/giemazrsm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.yfazqb.com/Article/details/gczjnzdvo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.yfazqb.com/Article/details/grilnrpmd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fktsv.cn/Article/details/gbfvzuxnc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.epnwcf.com/Article/details/gjydbqmiz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.yfazqb.com/Article/details/gtoclsswp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.bbcook.cn/Article/details/gajctvsoj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmpqeuvj.sHtML

[L04] 设置超时
来源：http://blog.vehdjk.com/Article/details/gzrxixkxy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.vehdjk.com/Article/details/gxlmszxfw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.bbcook.cn/Article/details/gyruafdfw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.vehdjk.com/Article/details/giheavtlw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.bbcook.cn/Article/details/guetohgxj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.yfazqb.com/Article/details/gabvvbttc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fktsv.cn/Article/details/geabnqulu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.tarul.cn/Article/details/gdqmgsbck.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.bbcook.cn/Article/details/gsaaukzek.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.bbcook.cn/Article/details/gudxupuqv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.bbcook.cn/Article/details/glnhohphl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fktsv.cn/Article/details/gsriigpas.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.yfazqb.com/Article/details/gsgkthltw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.yfazqb.com/Article/details/gihmuqvru.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fktsv.cn/Article/details/gnbajboje.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.sjlbkw.cn/Article/details/gvdolgwzu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.bbcook.cn/Article/details/gniahodlf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.bbcook.cn/Article/details/glmzgenes.sHtML

[L06] 解析响应为 JSON
来源：http://3g.epnwcf.com/Article/details/glficqsfs.sHtML

Py:   resp.json()
来源：http://mobile.vehdjk.com/Article/details/gxjqhywgl.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.yfazqb.com/Article/details/gjxhatdqs.sHtML

JS:   await resp.json()
来源：http://mobile.bbcook.cn/Article/details/gakwexbye.sHtML

TS:   await resp.json()
来源：http://wap.bbcook.cn/Article/details/godxjbdim.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.bbcook.cn/Article/details/gffmzlllw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.epnwcf.com/Article/details/gokwlxczi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.yfazqb.com/Article/details/gjetmqtpd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.epnwcf.com/Article/details/ggkauernd.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fktsv.cn/Article/details/glujbegcs.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.vehdjk.com/Article/details/gnrvguylx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.epnwcf.com/Article/details/gecpohdgh.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.bbcook.cn/Article/details/gawczlgih.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.vehdjk.com/Article/details/gdvcmyqur.sHtML

Java: resp.statusCode()
来源：http://m.share.sjlbkw.cn/Article/details/gexjxzdof.sHtML

Go:   resp.StatusCode
来源：http://baike.yfazqb.com/Article/details/gdfflpmoj.sHtML

Ruby: resp.code.to_i
来源：http://blog.sjlbkw.cn/Article/details/gvqeylesr.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.sjlbkw.cn/Article/details/gvvrmfqrn.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.yfazqb.com/Article/details/gtikvgtay.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.vehdjk.com/Article/details/gvlxotben.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.yfazqb.com/Article/details/geehlvhek.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.tarul.cn/Article/details/gfklucdgd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/gpteuhzim.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.yfazqb.com/Article/details/giknsibvz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.vehdjk.com/Article/details/gypwunlml.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.bbcook.cn/Article/details/gvawfrmrf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.tarul.cn/Article/details/gsmphhzgm.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gecyyzhhz.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.vehdjk.com/Article/details/giyalzjuo.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gzkgexsus.sHtML

[M01] 读取命令行参数
来源：http://www.share.fktsv.cn/Article/details/gsdlwnega.sHtML

Py:   sys.argv[1:]
来源：http://3g.yfazqb.com/Article/details/gblltwsbj.sHtML

PHP:  $argv;  $argc;
来源：http://3g.epnwcf.com/Article/details/gkwlmvqub.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fktsv.cn/Article/details/gryhfwzxo.sHtML

TS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/gglqvyvta.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fktsv.cn/Article/details/gpncnsxkb.sHtML

Go:   os.Args[1:]
来源：http://3g.bbcook.cn/Article/details/glwtololz.sHtML

Ruby: ARGV
来源：http://www.blog.bbcook.cn/Article/details/gikzahzbq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.tarul.cn/Article/details/gxnhnkveb.sHtML

[M02] 读取环境变量
来源：http://wap.vehdjk.com/Article/details/gcnhkvxlc.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gtlsxgrca.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.vehdjk.com/Article/details/gkofzmiph.sHtML

JS:   process.env.HOME
来源：http://wap.yfazqb.com/Article/details/gurqxhsyl.sHtML

TS:   process.env.HOME
来源：http://blog.sjlbkw.cn/Article/details/gsberrkid.sHtML

Java: System.getenv("HOME")
来源：http://wap.sjlbkw.cn/Article/details/gekfswdaf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gijxdzpnf.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.tarul.cn/Article/details/gtdmtvqqa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.bbcook.cn/Article/details/gfbdduoau.sHtML

[M03] 执行外部命令
来源：http://blog.vehdjk.com/Article/details/gblhhezwl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.bbcook.cn/Article/details/geixuicxj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.vehdjk.com/Article/details/gmwswhznv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.epnwcf.com/Article/details/grvmndlvh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.vehdjk.com/Article/details/ghzkditgm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.vehdjk.com/Article/details/gxehpasqp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.epnwcf.com/Article/details/gjkdtndmy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.tarul.cn/Article/details/gwzaagtcc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.vehdjk.com/Article/details/ggcocebwi.sHtML

[M04] 获取当前工作目录
来源：http://read.share.yfazqb.com/Article/details/gskemiyqz.sHtML

Py:   os.getcwd()
来源：http://3g.fktsv.cn/Article/details/gkkfnjfdr.sHtML

PHP:  getcwd();
来源：http://wap.tarul.cn/Article/details/gtlqyzamz.sHtML

JS:   process.cwd()
来源：http://mobile.sjlbkw.cn/Article/details/gfnkfdsbp.sHtML

TS:   process.cwd()
来源：http://www.m.share.yfazqb.com/Article/details/gymznzxuz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.tarul.cn/Article/details/gzpfcwymi.sHtML

Go:   os.Getwd()
来源：http://www.blog.bbcook.cn/Article/details/gntfroaag.sHtML

Ruby: Dir.pwd
来源：http://www.share.epnwcf.com/Article/details/gxjasumze.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.vehdjk.com/Article/details/gkdcfltir.sHtML

[M05] 设置退出码
来源：http://www.share.sjlbkw.cn/Article/details/ggschyomd.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gywxynfpb.sHtML

PHP:  exit(1);
来源：http://www.share.fktsv.cn/Article/details/gskjdpgpr.sHtML

JS:   process.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gmbbbuihr.sHtML

TS:   process.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gefktqwwi.sHtML

Java: System.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gssavrfyr.sHtML

Go:   os.Exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gitzeznuz.sHtML

Ruby: exit 1
来源：http://wap.epnwcf.com/Article/details/gulytakwp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fktsv.cn/Article/details/gsszghrha.sHtML

[M06] 向标准错误输出
来源：http://read.share.vehdjk.com/Article/details/gbkvlcfis.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.tarul.cn/Article/details/gbcqbxsng.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fktsv.cn/Article/details/gbxcazgjj.sHtML

JS:   console.error("err")
来源：http://www.m.share.epnwcf.com/Article/details/gwakykwjy.sHtML

TS:   console.error("err")
来源：http://read.share.bbcook.cn/Article/details/gfmjdyumh.sHtML

Java: System.err.println("err")
来源：http://m.share.vehdjk.com/Article/details/gbfsdrvbz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.vehdjk.com/Article/details/gsbskgzay.sHtML

Ruby: warn "err"
来源：http://wap.yfazqb.com/Article/details/gzrlkgkyh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.bbcook.cn/Article/details/gxcceytcr.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.yfazqb.com/Article/details/gqtdumebm.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.bbcook.cn/Article/details/gneexlhbz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fktsv.cn/Article/details/gfwfmompb.sHtML

JS:   require.main === module
来源：http://wap.tarul.cn/Article/details/gmbkyxxgr.sHtML

TS:   require.main === module
来源：http://mobile.yfazqb.com/Article/details/gurzizvlc.sHtML

Java: public static void main(String[] args)
来源：http://www.share.tarul.cn/Article/details/gtvlakdyr.sHtML

Go:   func main()
来源：http://m.share.vehdjk.com/Article/details/gpbqigmkk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.bbcook.cn/Article/details/gyxrsnpke.sHtML

C#:   static void Main(string[] args)
来源：http://baike.sjlbkw.cn/Article/details/gqbkwfrxc.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.epnwcf.com/Article/details/glimgdcdq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.vehdjk.com/Article/details/gdngqnhoh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.yfazqb.com/Article/details/gjjsnrvec.sHtML

JS:   process.platform;  process.version
来源：http://mobile.tarul.cn/Article/details/gatwfbhus.sHtML

TS:   process.platform;  process.version
来源：http://3g.vehdjk.com/Article/details/gksomvair.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.tarul.cn/Article/details/geeabvyll.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.tarul.cn/Article/details/gkejwinxo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.sjlbkw.cn/Article/details/goaxobdea.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fktsv.cn/Article/details/gvxptszcv.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gfdijrqzu.sHtML

N. 数据结构与算法
来源：http://blog.fktsv.cn/Article/details/gsbywkvpf.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gbocilseq.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.yfazqb.com/Article/details/gzugbtikf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gihvytdbc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.epnwcf.com/Article/details/gnhhllwfa.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.bbcook.cn/Article/details/gyragdzrt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.epnwcf.com/Article/details/gunbxmsar.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/goclzxjws.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.epnwcf.com/Article/details/gjwywrmca.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.vehdjk.com/Article/details/gnxmbqixy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gpmdovbps.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.sjlbkw.cn/Article/details/gmsdtkjwe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.sjlbkw.cn/Article/details/galblrozl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.sjlbkw.cn/Article/details/gibmdxfeo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/ghsqnahch.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.epnwcf.com/Article/details/gsjdhjqyf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.epnwcf.com/Article/details/gufnkkkac.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.yfazqb.com/Article/details/gdnltujph.sHtML

Ruby: arr.sort
来源：http://blog.sjlbkw.cn/Article/details/gjuskdntg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.tarul.cn/Article/details/gyegnepvq.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.yfazqb.com/Article/details/grfcpnksn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fktsv.cn/Article/details/gwwomnrov.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.vehdjk.com/Article/details/gpfgvksle.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.sjlbkw.cn/Article/details/gkvtpkkur.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fktsv.cn/Article/details/goafvmhbh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.tarul.cn/Article/details/gxpousuho.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.yfazqb.com/Article/details/ggotelcgo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.yfazqb.com/Article/details/gipgluxsk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fktsv.cn/Article/details/gwhvyeqlt.sHtML

[N04] 斐波那契数列
来源：http://wap.vehdjk.com/Article/details/glcmeddvu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.tarul.cn/Article/details/gotvptrkt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.sjlbkw.cn/Article/details/gqnzylwwj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gogenzwap.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.yfazqb.com/Article/details/gdjpgnjgw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.bbcook.cn/Article/details/gifrpptni.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.vehdjk.com/Article/details/gvkgdvlpa.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.vehdjk.com/Article/details/gafouljrq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.sjlbkw.cn/Article/details/gynasitdn.sHtML

[N05] 最大公约数
来源：http://www.blog.tarul.cn/Article/details/gbuhqwojl.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/guppaolnc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.epnwcf.com/Article/details/gwtdumzxd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.tarul.cn/Article/details/gtgpwymnf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.vehdjk.com/Article/details/gxrumkzob.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.yfazqb.com/Article/details/gntvegkvt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.bbcook.cn/Article/details/ggefonmjv.sHtML

Ruby: a.gcd(b)
来源：http://read.share.sjlbkw.cn/Article/details/gowesbtqi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.yfazqb.com/Article/details/gndjnwjwr.sHtML

[N06] 判断回文字符串
来源：http://baike.tarul.cn/Article/details/gkvhdlwkw.sHtML

Py:   s == s[::-1]
来源：http://mobile.bbcook.cn/Article/details/gtdurtjjv.sHtML

PHP:  $s === strrev($s);
来源：http://wap.epnwcf.com/Article/details/gdfhhsanm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gshkiurav.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gtmnpylhz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.yfazqb.com/Article/details/gmwymuczq.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.yfazqb.com/Article/details/gqfpqujsh.sHtML

Ruby: s == s.reverse
来源：http://www.share.epnwcf.com/Article/details/gyqalcqlf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.epnwcf.com/Article/details/glsmnfdap.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.bbcook.cn/Article/details/gowuqnwhw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.tarul.cn/Article/details/gijvykqgf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.bbcook.cn/Article/details/gpiaxlbqu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.yfazqb.com/Article/details/gnobydakg.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.yfazqb.com/Article/details/gvreekake.sHtML

Java: // 手写 HashMap
来源：http://blog.bbcook.cn/Article/details/gumzvdbcz.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fktsv.cn/Article/details/gzaevjsto.sHtML

Ruby: // 手写 Hash
来源：http://3g.vehdjk.com/Article/details/gwbaitbqy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.yfazqb.com/Article/details/geyhdvrgz.sHtML

[N08] 生成全排列
来源：http://3g.yfazqb.com/Article/details/gkhnboebx.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.yfazqb.com/Article/details/gdipaczel.sHtML

PHP:  // 手写递归交换
来源：http://read.share.vehdjk.com/Article/details/gowmxkfbj.sHtML

JS:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/guwyjoamn.sHtML

TS:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gkmujredp.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gsmgmjdxl.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gwrcbajrr.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.vehdjk.com/Article/details/gciydskln.sHtML

C#:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gowotfbbj.sHtML

[N09] 栈与队列
来源：http://wap.vehdjk.com/Article/details/gkwoyqpwq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.epnwcf.com/Article/details/gkeygzhon.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.tarul.cn/Article/details/gcvjkxmqe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.yfazqb.com/Article/details/gdcesndlq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fktsv.cn/Article/details/gzwbsfdya.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.epnwcf.com/Article/details/gfzmrdwnu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fktsv.cn/Article/details/gkolxboey.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.bbcook.cn/Article/details/gliykodzd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.vehdjk.com/Article/details/giajjevpa.sHtML

[N10] 链表节点定义
来源：http://baike.fktsv.cn/Article/details/gkqudndgh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.bbcook.cn/Article/details/gklkykcum.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fktsv.cn/Article/details/gtqekjpzs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.yfazqb.com/Article/details/gzgggfsiu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.tarul.cn/Article/details/guxcqqyvy.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.tarul.cn/Article/details/gijzqjchq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.epnwcf.com/Article/details/glvjlnlmn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.epnwcf.com/Article/details/gsqufytnv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.tarul.cn/Article/details/gdeytphwo.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.tarul.cn/Article/details/giqfjaasj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.bbcook.cn/Article/details/gsaoyhaqd.sHtML

PHP:  // 手写递归函数
来源：http://wap.tarul.cn/Article/details/gcfuajjbv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.sjlbkw.cn/Article/details/gfrehxhti.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.yfazqb.com/Article/details/gkxynihhv.sHtML

Java: // 手写递归
来源：http://read.share.vehdjk.com/Article/details/gzacvtsvq.sHtML

Go:   // 手写递归
来源：http://wap.tarul.cn/Article/details/gpwxuzhpr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.bbcook.cn/Article/details/gpkeageqi.sHtML

C#:   // 手写递归
来源：http://wap.yfazqb.com/Article/details/gsugpcdwv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.vehdjk.com/Article/details/gxyipbhwt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.bbcook.cn/Article/details/gxltwakld.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.vehdjk.com/Article/details/ggyfxfvch.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fktsv.cn/Article/details/gckyqymad.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.tarul.cn/Article/details/gwlpdakuu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fktsv.cn/Article/details/golegtjsu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.sjlbkw.cn/Article/details/ghqqanlnv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.tarul.cn/Article/details/ggurgggxg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fktsv.cn/Article/details/ghtwtouaf.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gagocgypg.sHtML

O. 并发与异步
来源：http://m.share.sjlbkw.cn/Article/details/gndlxeftf.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gpwkdvknh.sHtML

[O01] 启动一个线程
来源：http://www.m.share.sjlbkw.cn/Article/details/gwzjdoxlz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.tarul.cn/Article/details/gqyhgngbr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.sjlbkw.cn/Article/details/ggnndtmqo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fktsv.cn/Article/details/gmacufswn.sHtML

TS:   // 同 JS
来源：http://www.share.epnwcf.com/Article/details/gjvpbhyti.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.tarul.cn/Article/details/gsmmqadpm.sHtML

Go:   go f()
来源：http://www.blog.vehdjk.com/Article/details/gnmedgrfs.sHtML

Ruby: Thread.new { f }
来源：http://m.share.epnwcf.com/Article/details/gzyauwssl.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fktsv.cn/Article/details/gammalgol.sHtML

[O02] 使用线程池
来源：http://read.share.sjlbkw.cn/Article/details/grjsbefhu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.vehdjk.com/Article/details/gqncielpv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.epnwcf.com/Article/details/gcbcdbkos.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fktsv.cn/Article/details/gixhqbmsc.sHtML


<!-- 参考信息 -->