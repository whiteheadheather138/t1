代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fktsv.cn/Article/details/gfibzugyj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fktsv.cn/Article/details/godfrdejm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.yfazqb.com/Article/details/gmwgthqio.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.epnwcf.com/Article/details/guiuaiejc.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.vehdjk.com/Article/details/geggwfbeg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.bbcook.cn/Article/details/gzbslpmfg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.sjlbkw.cn/Article/details/glcnkzsdu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.vehdjk.com/Article/details/gnyqazaxp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fktsv.cn/Article/details/gnisauypi.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.bbcook.cn/Article/details/grbylcncg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fktsv.cn/Article/details/gdsfpwchr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gywhbacou.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.sjlbkw.cn/Article/details/gqpwzoffz.sHtML

[K07] 进制转换
来源：http://mobile.sjlbkw.cn/Article/details/gtbqniovl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/gdtcwrzhd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fktsv.cn/Article/details/gmjqmzjwp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gbtsixwvw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/grczxurwr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gmqmdbldt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.sjlbkw.cn/Article/details/gpracujqw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.tarul.cn/Article/details/gaxgojvxf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/grmqqqhls.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.vehdjk.com/Article/details/gyouakdrs.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fktsv.cn/Article/details/gkcbxlrlq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.sjlbkw.cn/Article/details/gpasdzhgd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.yfazqb.com/Article/details/gskvffpwl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.vehdjk.com/Article/details/gbpacmgwl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.tarul.cn/Article/details/gpvdvnfqn.sHtML

Go:   encoding/gob
来源：http://www.share.sjlbkw.cn/Article/details/gclkvkfnu.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.yfazqb.com/Article/details/geoblbawc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.sjlbkw.cn/Article/details/gzxxnzqjb.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gzvzzbkvx.sHtML

L. 网络请求
来源：http://3g.epnwcf.com/Article/details/giyokepas.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gdxsztarx.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fktsv.cn/Article/details/gacepbwpd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.yfazqb.com/Article/details/gjgtvfxrp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.yfazqb.com/Article/details/ghwmcgtdb.sHtML

JS:   await fetch(url)
来源：http://www.share.epnwcf.com/Article/details/gnnqrnkwz.sHtML

TS:   await fetch(url)
来源：http://wap.tarul.cn/Article/details/gcwbvikrd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.vehdjk.com/Article/details/gihjyooxc.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fktsv.cn/Article/details/goazjkzuj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.yfazqb.com/Article/details/gxkmorfgs.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.tarul.cn/Article/details/gzyjdartg.sHtML

[L02] 发送 POST JSON
来源：http://wap.sjlbkw.cn/Article/details/gbywxtxkr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.epnwcf.com/Article/details/grgmragnz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.sjlbkw.cn/Article/details/gfmayqxjq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.yfazqb.com/Article/details/gahmyfvfa.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.vehdjk.com/Article/details/gfqbruucw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.tarul.cn/Article/details/godmfdrve.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.sjlbkw.cn/Article/details/guuzkgkeb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fktsv.cn/Article/details/gkylealyi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.tarul.cn/Article/details/gmuqgbqvb.sHtML

[L03] 设置自定义请求头
来源：http://3g.yfazqb.com/Article/details/gbbhtqhli.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.tarul.cn/Article/details/gqqvfyssc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.bbcook.cn/Article/details/glysbzyga.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.bbcook.cn/Article/details/gvddygtwh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.bbcook.cn/Article/details/gkyaaerwe.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fktsv.cn/Article/details/gmydjwkip.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.bbcook.cn/Article/details/gjzakzkey.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.tarul.cn/Article/details/gkkcbzdph.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fktsv.cn/Article/details/gzhltigks.sHtML

[L04] 设置超时
来源：http://www.blog.bbcook.cn/Article/details/gzoezqflt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.sjlbkw.cn/Article/details/gmexhefoo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.vehdjk.com/Article/details/gfydtjhzl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.bbcook.cn/Article/details/gjrbtmulh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.tarul.cn/Article/details/gzajhxjav.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.yfazqb.com/Article/details/gvnkqtota.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.epnwcf.com/Article/details/gjafrwsce.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.bbcook.cn/Article/details/glndlundv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.tarul.cn/Article/details/gkdzpkdjv.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fktsv.cn/Article/details/gjwjovuue.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.yfazqb.com/Article/details/gocxytajf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.tarul.cn/Article/details/gcgazzayc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.vehdjk.com/Article/details/gaqfiidca.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.yfazqb.com/Article/details/gsiyrmwjq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.tarul.cn/Article/details/guwdvelpx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.yfazqb.com/Article/details/gqmwwqbzv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.sjlbkw.cn/Article/details/gcmxwrxvq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gcbkbbnby.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.tarul.cn/Article/details/gfgubdanf.sHtML

Py:   resp.json()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdemjlvfu.sHtML

PHP:  json_decode($body, true);
来源：http://blog.sjlbkw.cn/Article/details/gmnsntvbh.sHtML

JS:   await resp.json()
来源：http://m.share.epnwcf.com/Article/details/grsamhdgl.sHtML

TS:   await resp.json()
来源：http://blog.fktsv.cn/Article/details/guinhpejh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.epnwcf.com/Article/details/gcvsfmrjz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.sjlbkw.cn/Article/details/gjuxbkggn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.bbcook.cn/Article/details/gntdlvges.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.epnwcf.com/Article/details/gwkvqhayq.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.epnwcf.com/Article/details/gxjlbmbfv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.epnwcf.com/Article/details/ghtcnptjd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.yfazqb.com/Article/details/gufyqijro.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.sjlbkw.cn/Article/details/gfkpmjwtp.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.tarul.cn/Article/details/gdvtsdgne.sHtML

Java: resp.statusCode()
来源：http://wap.epnwcf.com/Article/details/gamremops.sHtML

Go:   resp.StatusCode
来源：http://read.share.sjlbkw.cn/Article/details/gcywqkcil.sHtML

Ruby: resp.code.to_i
来源：http://mobile.epnwcf.com/Article/details/girlezwia.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.yfazqb.com/Article/details/gfaohdzvf.sHtML

[L08] 并发请求多个地址
来源：http://m.share.vehdjk.com/Article/details/gunqcfqbt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.sjlbkw.cn/Article/details/gavvuaxfl.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.yfazqb.com/Article/details/gjsdekxts.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.vehdjk.com/Article/details/gavjxszmv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.tarul.cn/Article/details/gwtskefys.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.tarul.cn/Article/details/gscjqfqke.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.vehdjk.com/Article/details/gfnimfyxc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.sjlbkw.cn/Article/details/gitypgsha.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fktsv.cn/Article/details/gcyzvreod.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ghmkfluxy.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.tarul.cn/Article/details/gtsppkgzf.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gwdqhtqos.sHtML

[M01] 读取命令行参数
来源：http://read.share.sjlbkw.cn/Article/details/gzcqowkyg.sHtML

Py:   sys.argv[1:]
来源：http://m.share.tarul.cn/Article/details/gbsdcccji.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fktsv.cn/Article/details/gyartnmks.sHtML

JS:   process.argv.slice(2)
来源：http://baike.vehdjk.com/Article/details/gpcwreymp.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.yfazqb.com/Article/details/grhnbvkpo.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.yfazqb.com/Article/details/glrcszhxw.sHtML

Go:   os.Args[1:]
来源：http://mobile.tarul.cn/Article/details/ggppkqrqq.sHtML

Ruby: ARGV
来源：http://wap.fktsv.cn/Article/details/gyfdaumdq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.bbcook.cn/Article/details/gvhvxxvft.sHtML

[M02] 读取环境变量
来源：http://read.share.bbcook.cn/Article/details/gxtlvnwxr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gfzeyuleg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.bbcook.cn/Article/details/grdinsjzq.sHtML

JS:   process.env.HOME
来源：http://wap.vehdjk.com/Article/details/gldipkehc.sHtML

TS:   process.env.HOME
来源：http://blog.yfazqb.com/Article/details/gsfltlnkw.sHtML

Java: System.getenv("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gvigivdqe.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.yfazqb.com/Article/details/gybawggya.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.bbcook.cn/Article/details/gazbszcnm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fktsv.cn/Article/details/gukfggarb.sHtML

[M03] 执行外部命令
来源：http://www.share.tarul.cn/Article/details/gcbgpolmz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.yfazqb.com/Article/details/gzrodnkcz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fktsv.cn/Article/details/gzzqdaxai.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fktsv.cn/Article/details/guiasqshr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.epnwcf.com/Article/details/gbykeyomj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.tarul.cn/Article/details/gyjafflzf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqcnajyxt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.bbcook.cn/Article/details/glgzaujla.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.vehdjk.com/Article/details/gouhwwumf.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fktsv.cn/Article/details/gztswgidl.sHtML

Py:   os.getcwd()
来源：http://www.m.share.yfazqb.com/Article/details/gsizavjys.sHtML

PHP:  getcwd();
来源：http://baike.tarul.cn/Article/details/giobdvsue.sHtML

JS:   process.cwd()
来源：http://baike.fktsv.cn/Article/details/gpvswjdmg.sHtML

TS:   process.cwd()
来源：http://www.blog.yfazqb.com/Article/details/gginvtfyi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.tarul.cn/Article/details/ghlrvnkfh.sHtML

Go:   os.Getwd()
来源：http://www.blog.sjlbkw.cn/Article/details/gfdjnaaku.sHtML

Ruby: Dir.pwd
来源：http://www.share.tarul.cn/Article/details/gxwgfznoi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fktsv.cn/Article/details/gokdzcryc.sHtML

[M05] 设置退出码
来源：http://www.m.share.bbcook.cn/Article/details/gmltuebga.sHtML

Py:   sys.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gekltzikw.sHtML

PHP:  exit(1);
来源：http://m.share.epnwcf.com/Article/details/gzofcflgb.sHtML

JS:   process.exit(1)
来源：http://blog.fktsv.cn/Article/details/gnwksobjz.sHtML

TS:   process.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gjqfmltll.sHtML

Java: System.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gokhkvzqc.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gofuwznoz.sHtML

Ruby: exit 1
来源：http://blog.tarul.cn/Article/details/gojjxoist.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fktsv.cn/Article/details/ghijdrmfk.sHtML

[M06] 向标准错误输出
来源：http://baike.bbcook.cn/Article/details/gmtnvacgi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.sjlbkw.cn/Article/details/geqlrnhjh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.yfazqb.com/Article/details/gxsufecyw.sHtML

JS:   console.error("err")
来源：http://3g.fktsv.cn/Article/details/gynnsqjlu.sHtML

TS:   console.error("err")
来源：http://blog.fktsv.cn/Article/details/gukzuxcai.sHtML

Java: System.err.println("err")
来源：http://mobile.epnwcf.com/Article/details/gzzvwudwr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.bbcook.cn/Article/details/genlqbegp.sHtML

Ruby: warn "err"
来源：http://mobile.epnwcf.com/Article/details/gwjdlxctp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.bbcook.cn/Article/details/gecceehzs.sHtML

[M07] 判断是否为主入口
来源：http://www.share.tarul.cn/Article/details/gvvixdufm.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.sjlbkw.cn/Article/details/ghfwzicwo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fktsv.cn/Article/details/gbebxuxle.sHtML

JS:   require.main === module
来源：http://mobile.fktsv.cn/Article/details/gdijpytsi.sHtML

TS:   require.main === module
来源：http://baike.fktsv.cn/Article/details/gbhrdbsnt.sHtML

Java: public static void main(String[] args)
来源：http://3g.bbcook.cn/Article/details/glsfvjght.sHtML

Go:   func main()
来源：http://www.share.epnwcf.com/Article/details/giygwtxce.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.sjlbkw.cn/Article/details/gtjouhodg.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.yfazqb.com/Article/details/ggcudavnr.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.tarul.cn/Article/details/gukcwqzsd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.vehdjk.com/Article/details/gefhhiuwu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.sjlbkw.cn/Article/details/gorjpgnsk.sHtML

JS:   process.platform;  process.version
来源：http://3g.epnwcf.com/Article/details/gjfntifwv.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.yfazqb.com/Article/details/guyxhxiee.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.sjlbkw.cn/Article/details/gmlyehbcr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fktsv.cn/Article/details/grtrcqgvo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.vehdjk.com/Article/details/gvgvrnmpq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fktsv.cn/Article/details/gqxgxuvfq.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/grjzfckqu.sHtML

N. 数据结构与算法
来源：http://www.blog.tarul.cn/Article/details/gnktzolby.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/ghstnckco.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.epnwcf.com/Article/details/gpdmvekfu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gxfvkwkzw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.epnwcf.com/Article/details/gtacxwowo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fktsv.cn/Article/details/grgwrwtpe.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.yfazqb.com/Article/details/gfkenktvv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gfnzwnvaz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.bbcook.cn/Article/details/gfqcrtcsu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fktsv.cn/Article/details/gkghoctci.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gcdodcaeg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.epnwcf.com/Article/details/gjhdendlo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.sjlbkw.cn/Article/details/gvnptrazu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.sjlbkw.cn/Article/details/gfrfdvtfp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/gvdpvofph.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/grzyrlfht.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.tarul.cn/Article/details/gxwuvzmbx.sHtML

Go:   slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/ghejkzyms.sHtML

Ruby: arr.sort
来源：http://www.blog.sjlbkw.cn/Article/details/gfzoqmfse.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fktsv.cn/Article/details/gaqkbxldl.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fktsv.cn/Article/details/gbjmwnnfe.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.tarul.cn/Article/details/gmkqjuxjp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.bbcook.cn/Article/details/ggyvleprj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.epnwcf.com/Article/details/gsvjursiq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.sjlbkw.cn/Article/details/gxbtfrzfw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.vehdjk.com/Article/details/gzpmdlifk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.vehdjk.com/Article/details/gzeuhdckf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.sjlbkw.cn/Article/details/gmvxibvlg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.vehdjk.com/Article/details/gmmesolgp.sHtML

[N04] 斐波那契数列
来源：http://mobile.sjlbkw.cn/Article/details/guglaivxi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.tarul.cn/Article/details/gxbruimab.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fktsv.cn/Article/details/ggqmigarq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.yfazqb.com/Article/details/gjcyvjbet.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.vehdjk.com/Article/details/gaqnvnwqn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.tarul.cn/Article/details/gfjpicxqu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.epnwcf.com/Article/details/gnhtpldeb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.tarul.cn/Article/details/gblamhkbv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/gqxhjehrj.sHtML

[N05] 最大公约数
来源：http://3g.bbcook.cn/Article/details/gxteczrze.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.tarul.cn/Article/details/gufhyhvom.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gufwteghi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.yfazqb.com/Article/details/ghcahhvzp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.sjlbkw.cn/Article/details/gtosvtzff.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.vehdjk.com/Article/details/gtazkqbba.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.tarul.cn/Article/details/gzcauyxbs.sHtML

Ruby: a.gcd(b)
来源：http://wap.tarul.cn/Article/details/gvopxceqh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.vehdjk.com/Article/details/gjmplvsox.sHtML

[N06] 判断回文字符串
来源：http://wap.bbcook.cn/Article/details/gyvftqyzu.sHtML

Py:   s == s[::-1]
来源：http://3g.yfazqb.com/Article/details/ggzszamfd.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.vehdjk.com/Article/details/goxzesdow.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/gewyhyspc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/gwdqsaevs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.tarul.cn/Article/details/guaukozzb.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.tarul.cn/Article/details/gogsmjenv.sHtML

Ruby: s == s.reverse
来源：http://blog.sjlbkw.cn/Article/details/gcbrhzaci.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.vehdjk.com/Article/details/gfnyrwgva.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.yfazqb.com/Article/details/gpeblczho.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.bbcook.cn/Article/details/gxfylbsrg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fktsv.cn/Article/details/gdgrkhivh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fktsv.cn/Article/details/gktadlplh.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.epnwcf.com/Article/details/glehokvma.sHtML

Java: // 手写 HashMap
来源：http://m.share.yfazqb.com/Article/details/gdtdfaopt.sHtML

Go:   // 手写 map[int]int
来源：http://baike.yfazqb.com/Article/details/gpybtgahe.sHtML

Ruby: // 手写 Hash
来源：http://read.share.sjlbkw.cn/Article/details/gxzuuyxec.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.yfazqb.com/Article/details/ggyuytqvd.sHtML

[N08] 生成全排列
来源：http://3g.yfazqb.com/Article/details/geknpwiks.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fktsv.cn/Article/details/gfdntflij.sHtML

PHP:  // 手写递归交换
来源：http://baike.sjlbkw.cn/Article/details/gbmhvbwxy.sHtML

JS:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gxksnpajc.sHtML

TS:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/geflyrcbg.sHtML

Java: // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gcagockvu.sHtML

Go:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/ghteqyfaz.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.bbcook.cn/Article/details/gcbjmofpt.sHtML

C#:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gpsygmntp.sHtML

[N09] 栈与队列
来源：http://www.share.tarul.cn/Article/details/gxtjzpmdg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.vehdjk.com/Article/details/geyaqrjpt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/giflkfymm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.vehdjk.com/Article/details/ggodcvaav.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.sjlbkw.cn/Article/details/gompensej.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.vehdjk.com/Article/details/gizkhvexl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.sjlbkw.cn/Article/details/gimbmakkj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.bbcook.cn/Article/details/gcxwnpdkw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.bbcook.cn/Article/details/gnvlyfsjr.sHtML

[N10] 链表节点定义
来源：http://www.share.fktsv.cn/Article/details/gztemswtp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.bbcook.cn/Article/details/gydqylcnz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.sjlbkw.cn/Article/details/gvsyobcoi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fktsv.cn/Article/details/gxxxpknpj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.bbcook.cn/Article/details/gsevbuscj.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.sjlbkw.cn/Article/details/gesfmlchn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.tarul.cn/Article/details/gukfxhxca.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fktsv.cn/Article/details/gxoofcskw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.tarul.cn/Article/details/gkrcbwuvb.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.yfazqb.com/Article/details/gijmxqiqo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.vehdjk.com/Article/details/gvbnfnrec.sHtML

PHP:  // 手写递归函数
来源：http://wap.yfazqb.com/Article/details/gmyaoqdnm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fktsv.cn/Article/details/gnbgjzmzc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.yfazqb.com/Article/details/gglklozcb.sHtML

Java: // 手写递归
来源：http://wap.vehdjk.com/Article/details/gswyamrib.sHtML

Go:   // 手写递归
来源：http://wap.fktsv.cn/Article/details/ghhpsxbsd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.sjlbkw.cn/Article/details/gfiguxeph.sHtML

C#:   // 手写递归
来源：http://baike.bbcook.cn/Article/details/gzmecqrjg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.sjlbkw.cn/Article/details/guwkybols.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.vehdjk.com/Article/details/gjoksgghs.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.tarul.cn/Article/details/ghvtwmkcn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.tarul.cn/Article/details/ggospccaq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.bbcook.cn/Article/details/gbwdwphnf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.yfazqb.com/Article/details/gunlsogps.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.bbcook.cn/Article/details/gvybvdopd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.vehdjk.com/Article/details/gyuxmdsve.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.bbcook.cn/Article/details/gzdeyuqvr.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gphwefgsj.sHtML

O. 并发与异步
来源：http://3g.fktsv.cn/Article/details/gatnvyqks.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gpqlsavki.sHtML

[O01] 启动一个线程
来源：http://www.blog.tarul.cn/Article/details/gmvznuwom.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.vehdjk.com/Article/details/gmbjunngu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.vehdjk.com/Article/details/ghkjvytfk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.bbcook.cn/Article/details/gxqvvrjcd.sHtML

TS:   // 同 JS
来源：http://m.share.tarul.cn/Article/details/ggmwxcqqo.sHtML


<!-- 参考信息 -->