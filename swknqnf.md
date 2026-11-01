代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gvoquttdv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.sjlbkw.cn/Article/details/gbvdomdcf.sHtML

JS:   structuredClone(obj)
来源：http://mobile.sjlbkw.cn/Article/details/ghaxnakcb.sHtML

TS:   structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/ggdbowgbr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.bbcook.cn/Article/details/gneucwicr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.vehdjk.com/Article/details/gnkldtobh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.tarul.cn/Article/details/gadddkqqd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.sjlbkw.cn/Article/details/gkiwvxjyq.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.sjlbkw.cn/Article/details/gsmrkqwrj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fktsv.cn/Article/details/gxyvsdlnt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.bbcook.cn/Article/details/gfyjgsuod.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.vehdjk.com/Article/details/gyduewobu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.bbcook.cn/Article/details/gpxnhpsrb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.bbcook.cn/Article/details/grcuvnovv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/gawegmfle.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.yfazqb.com/Article/details/gmhwlrsue.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/gnwteuspz.sHtML

[K07] 进制转换
来源：http://www.blog.tarul.cn/Article/details/gkqbiinzw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/gnzoqoxbb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.sjlbkw.cn/Article/details/gunidryqv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/grqakfmrt.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gqitgqulk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.tarul.cn/Article/details/ggfxuevfw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.epnwcf.com/Article/details/gdfkvowts.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.vehdjk.com/Article/details/gyekculig.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gfkxbpnwc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fktsv.cn/Article/details/gkvrislry.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.yfazqb.com/Article/details/ghpvgezgp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.epnwcf.com/Article/details/gxfgvaedz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.yfazqb.com/Article/details/gmzcvdjwb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fktsv.cn/Article/details/gjqvyzxnb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.epnwcf.com/Article/details/gjsgcxnax.sHtML

Go:   encoding/gob
来源：http://baike.yfazqb.com/Article/details/ghoocyrrt.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.bbcook.cn/Article/details/gdozvbgwg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.tarul.cn/Article/details/ggfjzfgfl.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gvbzxublp.sHtML

L. 网络请求
来源：http://www.share.tarul.cn/Article/details/gzrktvvdp.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gxkvdkpnt.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fktsv.cn/Article/details/gilfwosln.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.bbcook.cn/Article/details/gfzbczsvp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.epnwcf.com/Article/details/gpyolrtwx.sHtML

JS:   await fetch(url)
来源：http://www.m.share.yfazqb.com/Article/details/gulvwmtvv.sHtML

TS:   await fetch(url)
来源：http://read.share.yfazqb.com/Article/details/gtjvzoovl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.vehdjk.com/Article/details/glvborroq.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.yfazqb.com/Article/details/grdxqoivt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fktsv.cn/Article/details/gzwrlraep.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.epnwcf.com/Article/details/gukaejffm.sHtML

[L02] 发送 POST JSON
来源：http://wap.epnwcf.com/Article/details/gexixkrkr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.yfazqb.com/Article/details/gmipqsouq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.sjlbkw.cn/Article/details/gqoagjxbe.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.yfazqb.com/Article/details/gzkklfyxa.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.bbcook.cn/Article/details/ggzvgvrfl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.vehdjk.com/Article/details/gpbrdmimm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.tarul.cn/Article/details/gcaklvnqg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.sjlbkw.cn/Article/details/gyhnwyulw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.bbcook.cn/Article/details/gqqmjczlt.sHtML

[L03] 设置自定义请求头
来源：http://3g.bbcook.cn/Article/details/gvkgqqfdu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.bbcook.cn/Article/details/gpjvnopwy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.yfazqb.com/Article/details/glhgwhjiz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fktsv.cn/Article/details/gdoytkbfe.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/gvruxcdaf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.yfazqb.com/Article/details/gxnkzjdrv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fktsv.cn/Article/details/ginwbkyih.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.yfazqb.com/Article/details/glokmlqdn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.sjlbkw.cn/Article/details/gkxhufmdw.sHtML

[L04] 设置超时
来源：http://3g.vehdjk.com/Article/details/guqjrtlkj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.yfazqb.com/Article/details/gwelrqpnw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.yfazqb.com/Article/details/gvgqmoixs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.epnwcf.com/Article/details/gcnlqknoa.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fktsv.cn/Article/details/gumebgiqj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.epnwcf.com/Article/details/gmyupvkzs.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.bbcook.cn/Article/details/gusegwgsf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fktsv.cn/Article/details/ghxkdymeo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.sjlbkw.cn/Article/details/gjrjjyurm.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.tarul.cn/Article/details/gxuqwjhuv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.tarul.cn/Article/details/gmxpftggf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gofjokntc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.bbcook.cn/Article/details/gbkxfflzr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.tarul.cn/Article/details/giwpuyiip.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fktsv.cn/Article/details/gguyqteyd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.vehdjk.com/Article/details/geeseetta.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fktsv.cn/Article/details/gnooelayp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gszmuyqpj.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.sjlbkw.cn/Article/details/gvjbccvec.sHtML

Py:   resp.json()
来源：http://blog.vehdjk.com/Article/details/gffdelcae.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.sjlbkw.cn/Article/details/gznhqhohl.sHtML

JS:   await resp.json()
来源：http://www.blog.bbcook.cn/Article/details/gzdlvycop.sHtML

TS:   await resp.json()
来源：http://read.share.epnwcf.com/Article/details/gkugqlqom.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.vehdjk.com/Article/details/gkntyidvr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.bbcook.cn/Article/details/gizddxlhn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.bbcook.cn/Article/details/gxiurxlib.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.epnwcf.com/Article/details/gfzkklocf.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.yfazqb.com/Article/details/grwfeaofs.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.yfazqb.com/Article/details/gmsblpxot.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.bbcook.cn/Article/details/gbjckikxt.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.yfazqb.com/Article/details/gpomegxiu.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.tarul.cn/Article/details/gqnpooytd.sHtML

Java: resp.statusCode()
来源：http://baike.fktsv.cn/Article/details/gwhxdobmf.sHtML

Go:   resp.StatusCode
来源：http://wap.yfazqb.com/Article/details/gbyhxresn.sHtML

Ruby: resp.code.to_i
来源：http://baike.tarul.cn/Article/details/gigdtysef.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.epnwcf.com/Article/details/gixdwdnho.sHtML

[L08] 并发请求多个地址
来源：http://baike.bbcook.cn/Article/details/gmcbtodjv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.vehdjk.com/Article/details/grmyvqcig.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.sjlbkw.cn/Article/details/ggqwfotov.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.yfazqb.com/Article/details/gkyrvlxxb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/gcncorkxl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.epnwcf.com/Article/details/gautaowmj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fktsv.cn/Article/details/glqplorve.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fktsv.cn/Article/details/goqbknedf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.sjlbkw.cn/Article/details/gbdoyskjf.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gknudanhl.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fktsv.cn/Article/details/gzcqbewyn.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/genlwireo.sHtML

[M01] 读取命令行参数
来源：http://mobile.tarul.cn/Article/details/gsuqryaeg.sHtML

Py:   sys.argv[1:]
来源：http://3g.tarul.cn/Article/details/gzcqgogvu.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.vehdjk.com/Article/details/gpdbcqutd.sHtML

JS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/gfkxzcomu.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.yfazqb.com/Article/details/gyrblvtya.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.tarul.cn/Article/details/ggcppjvuk.sHtML

Go:   os.Args[1:]
来源：http://mobile.tarul.cn/Article/details/goquygenp.sHtML

Ruby: ARGV
来源：http://read.share.tarul.cn/Article/details/gkanposfe.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fktsv.cn/Article/details/gyfovjpjo.sHtML

[M02] 读取环境变量
来源：http://wap.vehdjk.com/Article/details/gcprgsylw.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fktsv.cn/Article/details/gxevhijxr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.epnwcf.com/Article/details/gstdpndsf.sHtML

JS:   process.env.HOME
来源：http://www.share.sjlbkw.cn/Article/details/gbhqdnnbu.sHtML

TS:   process.env.HOME
来源：http://m.share.vehdjk.com/Article/details/gumcdoems.sHtML

Java: System.getenv("HOME")
来源：http://baike.fktsv.cn/Article/details/gtkzkhclu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.tarul.cn/Article/details/gbzhudqdf.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.epnwcf.com/Article/details/gqhgpofjo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fktsv.cn/Article/details/gxmvtsmwx.sHtML

[M03] 执行外部命令
来源：http://baike.yfazqb.com/Article/details/gniuzhghe.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gbiroaddy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.yfazqb.com/Article/details/gzqfrxrtf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fktsv.cn/Article/details/gzcdkaqbh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.yfazqb.com/Article/details/gblofiovq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.sjlbkw.cn/Article/details/gvsgcgvkf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fktsv.cn/Article/details/gooigipbi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.vehdjk.com/Article/details/gqvtmggns.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.epnwcf.com/Article/details/gnltvwtpa.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.tarul.cn/Article/details/gcgpctlyc.sHtML

Py:   os.getcwd()
来源：http://read.share.bbcook.cn/Article/details/goxcbifql.sHtML

PHP:  getcwd();
来源：http://mobile.fktsv.cn/Article/details/gsbghcjfr.sHtML

JS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/gunagzixo.sHtML

TS:   process.cwd()
来源：http://mobile.bbcook.cn/Article/details/grwupwdql.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.tarul.cn/Article/details/gmqinopow.sHtML

Go:   os.Getwd()
来源：http://wap.bbcook.cn/Article/details/gbnuxptaq.sHtML

Ruby: Dir.pwd
来源：http://blog.yfazqb.com/Article/details/grscbhagm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.vehdjk.com/Article/details/gzfojmijn.sHtML

[M05] 设置退出码
来源：http://www.blog.tarul.cn/Article/details/gztjpgxqz.sHtML

Py:   sys.exit(1)
来源：http://wap.vehdjk.com/Article/details/gaxiitcea.sHtML

PHP:  exit(1);
来源：http://wap.bbcook.cn/Article/details/ghqsqqtub.sHtML

JS:   process.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gjvoqdnla.sHtML

TS:   process.exit(1)
来源：http://3g.bbcook.cn/Article/details/gvtifmmcf.sHtML

Java: System.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gclhxxdpb.sHtML

Go:   os.Exit(1)
来源：http://blog.yfazqb.com/Article/details/gbpfjsftu.sHtML

Ruby: exit 1
来源：http://mobile.fktsv.cn/Article/details/gaavwppmk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.epnwcf.com/Article/details/gxfhgepnj.sHtML

[M06] 向标准错误输出
来源：http://blog.sjlbkw.cn/Article/details/gkbljwqrg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.sjlbkw.cn/Article/details/gooiqfhsq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.tarul.cn/Article/details/gajkwzsot.sHtML

JS:   console.error("err")
来源：http://read.share.fktsv.cn/Article/details/grpkeiacy.sHtML

TS:   console.error("err")
来源：http://www.m.share.epnwcf.com/Article/details/gbjvzclof.sHtML

Java: System.err.println("err")
来源：http://3g.yfazqb.com/Article/details/giclexchc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fktsv.cn/Article/details/gfhyqzgvv.sHtML

Ruby: warn "err"
来源：http://www.blog.vehdjk.com/Article/details/ganaecqjr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.yfazqb.com/Article/details/gsytzkfgs.sHtML

[M07] 判断是否为主入口
来源：http://wap.sjlbkw.cn/Article/details/gomvlbaxg.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fktsv.cn/Article/details/gratvvsgf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.bbcook.cn/Article/details/goallleze.sHtML

JS:   require.main === module
来源：http://baike.tarul.cn/Article/details/gyvhlcmsi.sHtML

TS:   require.main === module
来源：http://3g.yfazqb.com/Article/details/gjqwrbupl.sHtML

Java: public static void main(String[] args)
来源：http://wap.vehdjk.com/Article/details/gjkhavqrq.sHtML

Go:   func main()
来源：http://mobile.yfazqb.com/Article/details/gnvsjgage.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.epnwcf.com/Article/details/gykwprtvk.sHtML

C#:   static void Main(string[] args)
来源：http://blog.tarul.cn/Article/details/gnjjupgkn.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.tarul.cn/Article/details/ggqdrlehy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.bbcook.cn/Article/details/gwydsmfxc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.sjlbkw.cn/Article/details/gbwnssocw.sHtML

JS:   process.platform;  process.version
来源：http://wap.tarul.cn/Article/details/gdbggbhjh.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.tarul.cn/Article/details/gmqazswjf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fktsv.cn/Article/details/gvuuxrwue.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.tarul.cn/Article/details/gjeuvwgsf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.vehdjk.com/Article/details/gqdrjqiks.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.sjlbkw.cn/Article/details/goykvopyf.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ggidjmakw.sHtML

N. 数据结构与算法
来源：http://m.share.tarul.cn/Article/details/gcbaijzhb.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gzfltmqqe.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.yfazqb.com/Article/details/gslefniru.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.tarul.cn/Article/details/gvqrfcrxm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gdgacrbev.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.sjlbkw.cn/Article/details/gymdhboiy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.yfazqb.com/Article/details/gxnavqmqv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.vehdjk.com/Article/details/gpnofqdoi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/ghvkcdrhe.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.vehdjk.com/Article/details/gtycocahx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gsxfhwgzv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.bbcook.cn/Article/details/glqirvzxo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.tarul.cn/Article/details/gkerneddu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.epnwcf.com/Article/details/gvnnfddhd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/gxybtrhgy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/gwfjaovel.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fktsv.cn/Article/details/gqxrzozta.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fktsv.cn/Article/details/geuljoaam.sHtML

Ruby: arr.sort
来源：http://read.share.sjlbkw.cn/Article/details/gwsaijegc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.epnwcf.com/Article/details/gquuwjcso.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.bbcook.cn/Article/details/gaebsanju.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.epnwcf.com/Article/details/gkbicjtmm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.vehdjk.com/Article/details/gjrivzljm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.yfazqb.com/Article/details/ginuukntl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.tarul.cn/Article/details/gklqjfftf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.epnwcf.com/Article/details/gbdclreui.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.tarul.cn/Article/details/gmzotefig.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.bbcook.cn/Article/details/geowmwyjz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fktsv.cn/Article/details/ghigihjyk.sHtML

[N04] 斐波那契数列
来源：http://baike.yfazqb.com/Article/details/gotytdtqg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.sjlbkw.cn/Article/details/gmqxzigcn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.yfazqb.com/Article/details/ghorydhpr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/gmkynbpms.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fktsv.cn/Article/details/gjsxegeia.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.vehdjk.com/Article/details/gvlezxnbw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.epnwcf.com/Article/details/glfntmgqt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.vehdjk.com/Article/details/gapnenygw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/gdgoarkjl.sHtML

[N05] 最大公约数
来源：http://www.blog.sjlbkw.cn/Article/details/giuwmetok.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.sjlbkw.cn/Article/details/ghxcfwiml.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.vehdjk.com/Article/details/gugamhtmq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.epnwcf.com/Article/details/gvfgmewaw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.tarul.cn/Article/details/gxchmvkoq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.vehdjk.com/Article/details/ggpywemlj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.epnwcf.com/Article/details/gnneeolyw.sHtML

Ruby: a.gcd(b)
来源：http://baike.fktsv.cn/Article/details/gaaqozdiu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.tarul.cn/Article/details/gzokghvsw.sHtML

[N06] 判断回文字符串
来源：http://mobile.vehdjk.com/Article/details/gninxdnia.sHtML

Py:   s == s[::-1]
来源：http://baike.vehdjk.com/Article/details/gxolslgrw.sHtML

PHP:  $s === strrev($s);
来源：http://wap.sjlbkw.cn/Article/details/gtksxfmay.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gfocrxohp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gvhoimucv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.yfazqb.com/Article/details/gxvlqidmn.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fktsv.cn/Article/details/gaelifqqh.sHtML

Ruby: s == s.reverse
来源：http://www.blog.sjlbkw.cn/Article/details/giihtvwwk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.bbcook.cn/Article/details/glgrggpym.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.epnwcf.com/Article/details/gchplyqcj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.epnwcf.com/Article/details/goeisuajq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.epnwcf.com/Article/details/gwumuilvn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.epnwcf.com/Article/details/gmwobpqoz.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.sjlbkw.cn/Article/details/gwpnmcnqf.sHtML

Java: // 手写 HashMap
来源：http://m.share.fktsv.cn/Article/details/gkiexhsyw.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.yfazqb.com/Article/details/gtefaxcks.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.bbcook.cn/Article/details/gaieohpxy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.sjlbkw.cn/Article/details/gzrccvhfp.sHtML

[N08] 生成全排列
来源：http://mobile.fktsv.cn/Article/details/gfqejpkpb.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.yfazqb.com/Article/details/growqxdul.sHtML

PHP:  // 手写递归交换
来源：http://baike.sjlbkw.cn/Article/details/gjplwckmf.sHtML

JS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gggtficdc.sHtML

TS:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gjbngfkzh.sHtML

Java: // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/glexbtuai.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gxsowrmkc.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.tarul.cn/Article/details/gtifynjtn.sHtML

C#:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/glgwyiopm.sHtML

[N09] 栈与队列
来源：http://www.share.epnwcf.com/Article/details/gijdhxcmn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.tarul.cn/Article/details/ghcmsebda.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.tarul.cn/Article/details/gahhwtjwf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gqpaozflq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.bbcook.cn/Article/details/gclqrhkax.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.sjlbkw.cn/Article/details/gfcuoilfl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.bbcook.cn/Article/details/gzqmqlvzi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.tarul.cn/Article/details/giyduiqzy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.sjlbkw.cn/Article/details/gcivumybn.sHtML

[N10] 链表节点定义
来源：http://m.share.sjlbkw.cn/Article/details/geieuzkdu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.tarul.cn/Article/details/gyhmupspn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.epnwcf.com/Article/details/goommqxeg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.yfazqb.com/Article/details/gfgkosvia.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.vehdjk.com/Article/details/gfpbhrsde.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.vehdjk.com/Article/details/gtxtllzoz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.yfazqb.com/Article/details/gzntpeatn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.yfazqb.com/Article/details/getxxbeia.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.epnwcf.com/Article/details/ggzcgekne.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.epnwcf.com/Article/details/ghterbmtj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.vehdjk.com/Article/details/gbkptrgbp.sHtML

PHP:  // 手写递归函数
来源：http://wap.fktsv.cn/Article/details/gqwraphyu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.yfazqb.com/Article/details/gpdrjprqr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.yfazqb.com/Article/details/gxnvncnuj.sHtML

Java: // 手写递归
来源：http://www.blog.tarul.cn/Article/details/gpmhtkgnu.sHtML

Go:   // 手写递归
来源：http://www.blog.vehdjk.com/Article/details/gsdopxvxf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.bbcook.cn/Article/details/gohalgaut.sHtML

C#:   // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/gggizywmi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.epnwcf.com/Article/details/gztcriznz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.epnwcf.com/Article/details/gwjwxfvsc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.yfazqb.com/Article/details/gqqwpluke.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.vehdjk.com/Article/details/gslyixspu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.sjlbkw.cn/Article/details/gtutmvaeg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.bbcook.cn/Article/details/gsawtgxxm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.sjlbkw.cn/Article/details/gdtlvptnr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.vehdjk.com/Article/details/gdbmbozbq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.sjlbkw.cn/Article/details/gqpxomyby.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gtunfqnsu.sHtML

O. 并发与异步
来源：http://m.share.yfazqb.com/Article/details/gsrmixgek.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gdsxqwrso.sHtML

[O01] 启动一个线程
来源：http://mobile.vehdjk.com/Article/details/gonoojuzw.sHtML


<!-- 参考信息 -->