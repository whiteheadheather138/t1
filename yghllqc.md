代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.m.share.fktsv.cn/Article/details/ggexooquz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.vehdjk.com/Article/details/gkbcppoeo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fktsv.cn/Article/details/gcnnajogb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gtoxwnzin.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.bbcook.cn/Article/details/gmytgnebz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.bbcook.cn/Article/details/gcqnfhqmj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.vehdjk.com/Article/details/gklepdwyp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fktsv.cn/Article/details/gatbnzdmm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/gmmlfbfro.sHtML

[K07] 进制转换
来源：http://m.share.epnwcf.com/Article/details/gkzlkxvsv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gwdubxmfz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.sjlbkw.cn/Article/details/gyyasrtoy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/gjpucbghm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/geownfgpl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gznfolqvs.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.bbcook.cn/Article/details/gbvjkvlne.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.bbcook.cn/Article/details/gvedkosvq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.bbcook.cn/Article/details/glkgtnuwj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.epnwcf.com/Article/details/gehxtmbpf.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.bbcook.cn/Article/details/gkeyqqncw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fktsv.cn/Article/details/gwfuocmeu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fktsv.cn/Article/details/geprspxse.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gircacmho.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.yfazqb.com/Article/details/gcsgcpsqe.sHtML

Go:   encoding/gob
来源：http://www.m.share.vehdjk.com/Article/details/gmsoyxagj.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.bbcook.cn/Article/details/guuexohvt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.tarul.cn/Article/details/gepoqozvp.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gapjzmvue.sHtML

L. 网络请求
来源：http://baike.tarul.cn/Article/details/gkluhoupd.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/ggnmdpjxi.sHtML

[L01] 发送 GET 请求
来源：http://blog.vehdjk.com/Article/details/guoljgifz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.sjlbkw.cn/Article/details/ggonwavax.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fktsv.cn/Article/details/gmrdyvfbo.sHtML

JS:   await fetch(url)
来源：http://baike.yfazqb.com/Article/details/gvykhxzya.sHtML

TS:   await fetch(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gepalvvme.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrnwphsh.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.sjlbkw.cn/Article/details/gjsottpxe.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.tarul.cn/Article/details/guvwdiuzz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.vehdjk.com/Article/details/guymxhmed.sHtML

[L02] 发送 POST JSON
来源：http://read.share.yfazqb.com/Article/details/gxyqvgmne.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fktsv.cn/Article/details/ggxgoowxo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.tarul.cn/Article/details/gzskbljds.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.bbcook.cn/Article/details/gqqdqzwif.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.vehdjk.com/Article/details/gzplpbcja.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.tarul.cn/Article/details/gikprqbxc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fktsv.cn/Article/details/gbrwsfbvg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.sjlbkw.cn/Article/details/gguedczzv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.sjlbkw.cn/Article/details/gjfirtqxb.sHtML

[L03] 设置自定义请求头
来源：http://read.share.epnwcf.com/Article/details/gdjoiyjfi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.vehdjk.com/Article/details/gjqhtdpfj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.vehdjk.com/Article/details/ghqdymtmy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.tarul.cn/Article/details/gfcgiarns.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.bbcook.cn/Article/details/gqjugzscd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.bbcook.cn/Article/details/gniossulb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fktsv.cn/Article/details/gffkoaikw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.bbcook.cn/Article/details/glyskhbzk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.sjlbkw.cn/Article/details/gedqqmttm.sHtML

[L04] 设置超时
来源：http://www.m.share.yfazqb.com/Article/details/gprygtjej.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.bbcook.cn/Article/details/gzyqzjnnb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.bbcook.cn/Article/details/gdmhhqywd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.vehdjk.com/Article/details/gjyforzbd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fktsv.cn/Article/details/gbcpymrlu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.epnwcf.com/Article/details/gqsdhmagk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.vehdjk.com/Article/details/gactfbvpm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.sjlbkw.cn/Article/details/gwvyyrtkx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.yfazqb.com/Article/details/gmmlkmsmk.sHtML

[L05] 上传文件（multipart）
来源：http://blog.bbcook.cn/Article/details/gehilouip.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fktsv.cn/Article/details/gghidipkj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.vehdjk.com/Article/details/gkdcinfyq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.bbcook.cn/Article/details/gplnrutph.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.sjlbkw.cn/Article/details/gpckkugqs.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.epnwcf.com/Article/details/gsfvgxxrh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fktsv.cn/Article/details/ghrskainm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.sjlbkw.cn/Article/details/gzneeunwx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.yfazqb.com/Article/details/gozmkflfr.sHtML

[L06] 解析响应为 JSON
来源：http://blog.vehdjk.com/Article/details/gsyxcjiyx.sHtML

Py:   resp.json()
来源：http://mobile.vehdjk.com/Article/details/grpakvxvj.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.sjlbkw.cn/Article/details/gqchevjuo.sHtML

JS:   await resp.json()
来源：http://m.share.fktsv.cn/Article/details/gkfehjmvz.sHtML

TS:   await resp.json()
来源：http://3g.tarul.cn/Article/details/gxeopruwe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.vehdjk.com/Article/details/gdavroumu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.yfazqb.com/Article/details/gtrtiheee.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.tarul.cn/Article/details/gkrdjwzyc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.vehdjk.com/Article/details/grmoxwdhm.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.sjlbkw.cn/Article/details/gewgnoozl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.sjlbkw.cn/Article/details/gymglalvb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.vehdjk.com/Article/details/gzedjhigu.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.yfazqb.com/Article/details/gkcjoourl.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.bbcook.cn/Article/details/gxzbfsphj.sHtML

Java: resp.statusCode()
来源：http://mobile.fktsv.cn/Article/details/gzlsrsmqz.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fktsv.cn/Article/details/gnzektriq.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fktsv.cn/Article/details/gcbmqblyb.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.tarul.cn/Article/details/gzisimoko.sHtML

[L08] 并发请求多个地址
来源：http://blog.fktsv.cn/Article/details/gdghimjco.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.tarul.cn/Article/details/gitxlwfoc.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.epnwcf.com/Article/details/grzcgareq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fktsv.cn/Article/details/gtvqfjbzh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.epnwcf.com/Article/details/gqldbjjbv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.tarul.cn/Article/details/gxvkhzwdd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.sjlbkw.cn/Article/details/goooyhyma.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.vehdjk.com/Article/details/grtbjzvgm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.tarul.cn/Article/details/gowfhnrfc.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ggbvphfsr.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.yfazqb.com/Article/details/gwpsgbtxk.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/ghmjgkpmh.sHtML

[M01] 读取命令行参数
来源：http://read.share.fktsv.cn/Article/details/gjasmyifu.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.bbcook.cn/Article/details/gjrgcdmat.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.tarul.cn/Article/details/gcimkcpmy.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.tarul.cn/Article/details/guhibakge.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fktsv.cn/Article/details/geqwrdsqj.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.yfazqb.com/Article/details/ggcxfvoni.sHtML

Go:   os.Args[1:]
来源：http://m.share.yfazqb.com/Article/details/gzqajvrlx.sHtML

Ruby: ARGV
来源：http://baike.vehdjk.com/Article/details/gvrqatxqw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.tarul.cn/Article/details/gaaaafpic.sHtML

[M02] 读取环境变量
来源：http://baike.tarul.cn/Article/details/gupquvmkz.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.yfazqb.com/Article/details/glindhdbu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.vehdjk.com/Article/details/gphcmtkfr.sHtML

JS:   process.env.HOME
来源：http://3g.sjlbkw.cn/Article/details/gjotyjziy.sHtML

TS:   process.env.HOME
来源：http://blog.bbcook.cn/Article/details/glyprbipp.sHtML

Java: System.getenv("HOME")
来源：http://baike.vehdjk.com/Article/details/gzlonibbj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gtqkgqujm.sHtML

Ruby: ENV["HOME"]
来源：http://wap.tarul.cn/Article/details/gcunaxtqf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fktsv.cn/Article/details/gwgzvlepf.sHtML

[M03] 执行外部命令
来源：http://www.m.share.epnwcf.com/Article/details/gyuwmzqxy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.sjlbkw.cn/Article/details/gvrdsyhck.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.bbcook.cn/Article/details/ghdvsopyk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.tarul.cn/Article/details/gjwznygmx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.tarul.cn/Article/details/glbrrdpby.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fktsv.cn/Article/details/gubrtjekq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.epnwcf.com/Article/details/gksvobzdx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fktsv.cn/Article/details/gdbkczcte.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.tarul.cn/Article/details/gszzzlkuo.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.bbcook.cn/Article/details/gisrzxgcf.sHtML

Py:   os.getcwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/grsvuanpx.sHtML

PHP:  getcwd();
来源：http://m.share.tarul.cn/Article/details/gdezkkcnp.sHtML

JS:   process.cwd()
来源：http://m.share.fktsv.cn/Article/details/gerajjftl.sHtML

TS:   process.cwd()
来源：http://read.share.bbcook.cn/Article/details/gxusemjye.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtlzfzexc.sHtML

Go:   os.Getwd()
来源：http://www.blog.tarul.cn/Article/details/gmstljgxg.sHtML

Ruby: Dir.pwd
来源：http://m.share.fktsv.cn/Article/details/gtgzaiutm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fktsv.cn/Article/details/guxlitubb.sHtML

[M05] 设置退出码
来源：http://blog.tarul.cn/Article/details/guulmushr.sHtML

Py:   sys.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gleurjafk.sHtML

PHP:  exit(1);
来源：http://blog.fktsv.cn/Article/details/gsvqlovnc.sHtML

JS:   process.exit(1)
来源：http://read.share.yfazqb.com/Article/details/ghjolxnzt.sHtML

TS:   process.exit(1)
来源：http://read.share.tarul.cn/Article/details/glfqtriip.sHtML

Java: System.exit(1)
来源：http://3g.bbcook.cn/Article/details/gztvjwted.sHtML

Go:   os.Exit(1)
来源：http://www.blog.yfazqb.com/Article/details/ghjgnweuw.sHtML

Ruby: exit 1
来源：http://baike.tarul.cn/Article/details/gyykxmbma.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.yfazqb.com/Article/details/ghywtbdln.sHtML

[M06] 向标准错误输出
来源：http://www.share.tarul.cn/Article/details/gfqinlatr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.sjlbkw.cn/Article/details/ghrfhlvzs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.bbcook.cn/Article/details/gmjizdxcm.sHtML

JS:   console.error("err")
来源：http://mobile.yfazqb.com/Article/details/gzojgkcfv.sHtML

TS:   console.error("err")
来源：http://wap.bbcook.cn/Article/details/guuexvpzh.sHtML

Java: System.err.println("err")
来源：http://www.m.share.vehdjk.com/Article/details/gsutvoxab.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.epnwcf.com/Article/details/gqhbqshgs.sHtML

Ruby: warn "err"
来源：http://blog.sjlbkw.cn/Article/details/gjllyzoch.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.sjlbkw.cn/Article/details/ggdrakxaz.sHtML

[M07] 判断是否为主入口
来源：http://www.share.yfazqb.com/Article/details/gcfvmnhyg.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.yfazqb.com/Article/details/gysyjjoyk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.bbcook.cn/Article/details/glmfdtomh.sHtML

JS:   require.main === module
来源：http://baike.epnwcf.com/Article/details/ggilyruom.sHtML

TS:   require.main === module
来源：http://www.blog.vehdjk.com/Article/details/gqjbbmwgv.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.vehdjk.com/Article/details/gignwmxsu.sHtML

Go:   func main()
来源：http://www.share.bbcook.cn/Article/details/gwqxnstrh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fktsv.cn/Article/details/gcjfouatn.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.sjlbkw.cn/Article/details/gdpsjhfjw.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fktsv.cn/Article/details/gfaervqmq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.epnwcf.com/Article/details/gznxhjzma.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.vehdjk.com/Article/details/gzdsbbhes.sHtML

JS:   process.platform;  process.version
来源：http://read.share.vehdjk.com/Article/details/gfzalnigq.sHtML

TS:   process.platform;  process.version
来源：http://read.share.tarul.cn/Article/details/gekbqxiug.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.tarul.cn/Article/details/gvqretsnz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.bbcook.cn/Article/details/gfilzxvoe.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.tarul.cn/Article/details/ggpxhxfxn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.epnwcf.com/Article/details/gezwlvtdz.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gkumldscs.sHtML

N. 数据结构与算法
来源：http://3g.yfazqb.com/Article/details/gjbrhdfli.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gichpvowl.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.epnwcf.com/Article/details/gbmugdzfw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gjnxnevps.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.epnwcf.com/Article/details/gzzbvntgx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.vehdjk.com/Article/details/gubhxhvvt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fktsv.cn/Article/details/gjjksyzkc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gronakqus.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gxubrbfug.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.vehdjk.com/Article/details/glvsdzvjd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gwybnywgi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.yfazqb.com/Article/details/gwnmfykfl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.tarul.cn/Article/details/gnaericrt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.vehdjk.com/Article/details/ggeormagi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.bbcook.cn/Article/details/ggyebopfh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.epnwcf.com/Article/details/gbmnlgffl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.tarul.cn/Article/details/gavudnjmt.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.bbcook.cn/Article/details/gasxvhudv.sHtML

Ruby: arr.sort
来源：http://www.m.share.epnwcf.com/Article/details/gllmxtttt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fktsv.cn/Article/details/gamezwpnl.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.sjlbkw.cn/Article/details/gxgaspbpi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fktsv.cn/Article/details/gnpjyrdkc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.yfazqb.com/Article/details/ghtmsyplt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.yfazqb.com/Article/details/gqfuqyqnn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.yfazqb.com/Article/details/gmxmqyuih.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.bbcook.cn/Article/details/gmxebfpnr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fktsv.cn/Article/details/grcnzrksz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.epnwcf.com/Article/details/gccsulcto.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.epnwcf.com/Article/details/geqkqddwy.sHtML

[N04] 斐波那契数列
来源：http://3g.fktsv.cn/Article/details/gnfzomsse.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.tarul.cn/Article/details/gngabuipa.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.bbcook.cn/Article/details/gnqgydesf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/gryqvsojc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/gnkkedylr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.bbcook.cn/Article/details/gacedqtfp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.vehdjk.com/Article/details/gcgvffxax.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyljtxvkw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.yfazqb.com/Article/details/gfuwfxfaj.sHtML

[N05] 最大公约数
来源：http://www.blog.fktsv.cn/Article/details/gwrswmftj.sHtML

Py:   math.gcd(a, b)
来源：http://baike.yfazqb.com/Article/details/gizaokbum.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.bbcook.cn/Article/details/gblsccbdt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.vehdjk.com/Article/details/gmkjgoagw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.vehdjk.com/Article/details/gklzrjspd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.vehdjk.com/Article/details/gjgbmjksv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.sjlbkw.cn/Article/details/gjjtlefvn.sHtML

Ruby: a.gcd(b)
来源：http://blog.epnwcf.com/Article/details/gqxuenmmr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fktsv.cn/Article/details/gtujaqyaz.sHtML

[N06] 判断回文字符串
来源：http://mobile.bbcook.cn/Article/details/gxkpwshtm.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.epnwcf.com/Article/details/gguhmudcn.sHtML

PHP:  $s === strrev($s);
来源：http://3g.vehdjk.com/Article/details/gskybrtcp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/gbriljqdl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/gigtnoxxs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.sjlbkw.cn/Article/details/gabcfibuz.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.sjlbkw.cn/Article/details/gxkyusavb.sHtML

Ruby: s == s.reverse
来源：http://read.share.sjlbkw.cn/Article/details/ghhgoeibj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.vehdjk.com/Article/details/gtvcdswfy.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.yfazqb.com/Article/details/gaxfzuplm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.vehdjk.com/Article/details/gcocxrorr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fktsv.cn/Article/details/ggveuihko.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.tarul.cn/Article/details/gzwjfnrhu.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.bbcook.cn/Article/details/gyvkvhexj.sHtML

Java: // 手写 HashMap
来源：http://www.share.epnwcf.com/Article/details/gbdmrxijh.sHtML

Go:   // 手写 map[int]int
来源：http://3g.bbcook.cn/Article/details/gyjfozpej.sHtML

Ruby: // 手写 Hash
来源：http://read.share.yfazqb.com/Article/details/gpkvvfvmf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fktsv.cn/Article/details/gscobbwsr.sHtML

[N08] 生成全排列
来源：http://read.share.vehdjk.com/Article/details/gqiepgcrd.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.epnwcf.com/Article/details/gtbahhbxj.sHtML

PHP:  // 手写递归交换
来源：http://wap.fktsv.cn/Article/details/gjmxwufyi.sHtML

JS:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gnefpvasu.sHtML

TS:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gofqwbpdp.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gibhdlfeh.sHtML

Go:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/grpaztpqb.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fktsv.cn/Article/details/ggkpvqwrl.sHtML

C#:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/ghkdlrnkz.sHtML

[N09] 栈与队列
来源：http://blog.yfazqb.com/Article/details/geztnctli.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gbppblgjb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.sjlbkw.cn/Article/details/gqedwkbjt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gxkryvpnx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.bbcook.cn/Article/details/gpamjblqy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.bbcook.cn/Article/details/ggzcwntrb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fktsv.cn/Article/details/gyrsvldph.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/ghsdvlxdd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.vehdjk.com/Article/details/gakwkgwfb.sHtML

[N10] 链表节点定义
来源：http://baike.fktsv.cn/Article/details/gorllfubf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.epnwcf.com/Article/details/gbvwzngnl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fktsv.cn/Article/details/gcrddltgh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.vehdjk.com/Article/details/gpcdppaas.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fktsv.cn/Article/details/gdedtwhyl.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fktsv.cn/Article/details/glqpornmn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fktsv.cn/Article/details/gzovlqihx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.bbcook.cn/Article/details/gwojqizci.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.epnwcf.com/Article/details/gktfijwtd.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fktsv.cn/Article/details/glkzcbipl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.sjlbkw.cn/Article/details/gaxtntwfw.sHtML

PHP:  // 手写递归函数
来源：http://mobile.tarul.cn/Article/details/grgtcfomf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.yfazqb.com/Article/details/gzrufzcvm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.sjlbkw.cn/Article/details/giafmhqat.sHtML

Java: // 手写递归
来源：http://wap.vehdjk.com/Article/details/gvxbqzsaa.sHtML

Go:   // 手写递归
来源：http://baike.tarul.cn/Article/details/gsryxmjhv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.vehdjk.com/Article/details/gnykaddih.sHtML

C#:   // 手写递归
来源：http://wap.yfazqb.com/Article/details/gezdfkoqt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.yfazqb.com/Article/details/gqzrcozku.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fktsv.cn/Article/details/gprptnldp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fktsv.cn/Article/details/gwnvlmsjd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.bbcook.cn/Article/details/gjpdqrlel.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.bbcook.cn/Article/details/gmbtoxjcv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.yfazqb.com/Article/details/gyywekrjr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.tarul.cn/Article/details/gyxjwkknp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.vehdjk.com/Article/details/gketzdmcw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.epnwcf.com/Article/details/gkloykgag.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gtquzqtlx.sHtML

O. 并发与异步
来源：http://mobile.sjlbkw.cn/Article/details/gukffkqgg.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/guxlrncnc.sHtML

[O01] 启动一个线程
来源：http://m.share.yfazqb.com/Article/details/gmdfayvpe.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.bbcook.cn/Article/details/grfnmmfzc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fktsv.cn/Article/details/grovhwdlp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.vehdjk.com/Article/details/gzzsmiogb.sHtML

TS:   // 同 JS
来源：http://wap.bbcook.cn/Article/details/gpeiknjhe.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.yfazqb.com/Article/details/gljkbrzca.sHtML

Go:   go f()
来源：http://mobile.epnwcf.com/Article/details/gxfdfvxvs.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.yfazqb.com/Article/details/guoqftawn.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.bbcook.cn/Article/details/gwilykylz.sHtML


<!-- 参考信息 -->