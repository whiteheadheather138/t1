代发 wailian999

[K06] 解析 URL 查询串
来源：http://read.share.bbcook.cn/Article/details/gpapbeblm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.epnwcf.com/Article/details/gchyrgkra.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.bbcook.cn/Article/details/ghkybywti.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.bbcook.cn/Article/details/gsogbcquy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.bbcook.cn/Article/details/gagmpsylb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fktsv.cn/Article/details/gnofmhhst.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/gwxnbzuwn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.epnwcf.com/Article/details/gbsmuylkv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/gwoykemzj.sHtML

[K07] 进制转换
来源：http://mobile.yfazqb.com/Article/details/gwdkiagog.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.vehdjk.com/Article/details/guaisuivf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.yfazqb.com/Article/details/gaccgoxrf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gmcnrhvsw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/galwtngda.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gmvbduaax.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.bbcook.cn/Article/details/gydvxmkjo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.vehdjk.com/Article/details/gpoxzvfmc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.tarul.cn/Article/details/gwtuxcyio.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.vehdjk.com/Article/details/gdfhhcfmj.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.vehdjk.com/Article/details/gtcvrcrdr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdsmrmswp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.tarul.cn/Article/details/ghfkgschq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.tarul.cn/Article/details/grcdonuak.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fktsv.cn/Article/details/gpzziohsp.sHtML

Go:   encoding/gob
来源：http://read.share.fktsv.cn/Article/details/goqmzqfog.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.vehdjk.com/Article/details/gbsujgbsn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.sjlbkw.cn/Article/details/glhwblqoq.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gcczannmn.sHtML

L. 网络请求
来源：http://www.blog.sjlbkw.cn/Article/details/gnupzllnr.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/glinoawoo.sHtML

[L01] 发送 GET 请求
来源：http://m.share.vehdjk.com/Article/details/ghlolahlk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.yfazqb.com/Article/details/gwqgzasco.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fktsv.cn/Article/details/glzdyeytm.sHtML

JS:   await fetch(url)
来源：http://baike.tarul.cn/Article/details/gxgctihft.sHtML

TS:   await fetch(url)
来源：http://3g.yfazqb.com/Article/details/gtjopettx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.yfazqb.com/Article/details/gghkeyxvu.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.bbcook.cn/Article/details/gacryzaen.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.vehdjk.com/Article/details/gqbxxcrgw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fktsv.cn/Article/details/gnnakktei.sHtML

[L02] 发送 POST JSON
来源：http://blog.yfazqb.com/Article/details/gkmeprctv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.yfazqb.com/Article/details/gktvfzkko.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.tarul.cn/Article/details/gggrtsvgg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.yfazqb.com/Article/details/glnnxmrgk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fktsv.cn/Article/details/gwoyczdmi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.vehdjk.com/Article/details/gmqzwxupq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.bbcook.cn/Article/details/gubcephfw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.epnwcf.com/Article/details/gklcwwthh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fktsv.cn/Article/details/gspjpivcf.sHtML

[L03] 设置自定义请求头
来源：http://baike.sjlbkw.cn/Article/details/gjrvenvbl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.tarul.cn/Article/details/gbwprwbrf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.tarul.cn/Article/details/gifrovkwr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.epnwcf.com/Article/details/gtzwvmjhx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fktsv.cn/Article/details/gzeudfcud.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fktsv.cn/Article/details/gymiinbug.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.tarul.cn/Article/details/gumicozow.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.yfazqb.com/Article/details/ghinzcxwm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fktsv.cn/Article/details/gjqvqzkbx.sHtML

[L04] 设置超时
来源：http://www.share.sjlbkw.cn/Article/details/gddkruisz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fktsv.cn/Article/details/ggmhnxkoa.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.sjlbkw.cn/Article/details/giyugdxdh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.yfazqb.com/Article/details/gmrvpipgj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.sjlbkw.cn/Article/details/gpnyvytex.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.sjlbkw.cn/Article/details/grknccshv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.epnwcf.com/Article/details/gixcpboak.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.yfazqb.com/Article/details/guaychvts.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.sjlbkw.cn/Article/details/ghafmfttu.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.yfazqb.com/Article/details/gcjcvijfp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.epnwcf.com/Article/details/gxrtqztcf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.epnwcf.com/Article/details/gmumgwucx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.tarul.cn/Article/details/gzngulyoh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.tarul.cn/Article/details/gvkxixron.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fktsv.cn/Article/details/gijgdgles.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.vehdjk.com/Article/details/gwjyujuqy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.vehdjk.com/Article/details/gxixoxkwk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fktsv.cn/Article/details/gkhrlvxmw.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.tarul.cn/Article/details/gopszhpap.sHtML

Py:   resp.json()
来源：http://wap.epnwcf.com/Article/details/gxejfukzf.sHtML

PHP:  json_decode($body, true);
来源：http://3g.epnwcf.com/Article/details/gblokiaaj.sHtML

JS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/ggftadgpp.sHtML

TS:   await resp.json()
来源：http://mobile.sjlbkw.cn/Article/details/gdmlaynok.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.vehdjk.com/Article/details/gdwptlhhf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fktsv.cn/Article/details/ghorefcqu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.bbcook.cn/Article/details/gkqbakmah.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.vehdjk.com/Article/details/gixtekfzi.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fktsv.cn/Article/details/gopqislmi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.bbcook.cn/Article/details/gwocextnr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.vehdjk.com/Article/details/gegborldx.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.tarul.cn/Article/details/geqgbmzlw.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.tarul.cn/Article/details/gzhidxrdv.sHtML

Java: resp.statusCode()
来源：http://www.blog.epnwcf.com/Article/details/grqcwhlgg.sHtML

Go:   resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/gfnpwfdab.sHtML

Ruby: resp.code.to_i
来源：http://blog.tarul.cn/Article/details/gdswwytlo.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fktsv.cn/Article/details/ggznfxaob.sHtML

[L08] 并发请求多个地址
来源：http://wap.sjlbkw.cn/Article/details/gwpvzknbo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.tarul.cn/Article/details/gccaqpeho.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.tarul.cn/Article/details/gsajpnzld.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.yfazqb.com/Article/details/gtmfhpkfa.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/gabukpraa.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.tarul.cn/Article/details/gnionqfie.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.yfazqb.com/Article/details/gkbvsnezl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.vehdjk.com/Article/details/gnysthrat.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.epnwcf.com/Article/details/gqzwpmori.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gmoxmavnh.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.yfazqb.com/Article/details/gcntqelrp.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gfsliyvme.sHtML

[M01] 读取命令行参数
来源：http://m.share.fktsv.cn/Article/details/gtzthlpox.sHtML

Py:   sys.argv[1:]
来源：http://blog.yfazqb.com/Article/details/grpuwssgz.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.sjlbkw.cn/Article/details/gemliscej.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.epnwcf.com/Article/details/ghuxybwrl.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.vehdjk.com/Article/details/giqrpokms.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fktsv.cn/Article/details/gxdrzfthx.sHtML

Go:   os.Args[1:]
来源：http://wap.bbcook.cn/Article/details/gfxxcvhcu.sHtML

Ruby: ARGV
来源：http://read.share.bbcook.cn/Article/details/gvfkvseac.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.tarul.cn/Article/details/gzydgxymg.sHtML

[M02] 读取环境变量
来源：http://mobile.fktsv.cn/Article/details/gkfjhpels.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.epnwcf.com/Article/details/gdoxsurij.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.bbcook.cn/Article/details/gvxyuvlrk.sHtML

JS:   process.env.HOME
来源：http://wap.bbcook.cn/Article/details/gtrhpzvlw.sHtML

TS:   process.env.HOME
来源：http://wap.epnwcf.com/Article/details/gvixbbsuy.sHtML

Java: System.getenv("HOME")
来源：http://mobile.vehdjk.com/Article/details/gunefcvpg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.bbcook.cn/Article/details/gzopbugab.sHtML

Ruby: ENV["HOME"]
来源：http://blog.epnwcf.com/Article/details/gxczbmerh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gqywcbybw.sHtML

[M03] 执行外部命令
来源：http://read.share.bbcook.cn/Article/details/gjufzxhso.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.sjlbkw.cn/Article/details/gbchlclko.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.bbcook.cn/Article/details/gpcrfritz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.tarul.cn/Article/details/gsaafgdnk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fktsv.cn/Article/details/gnwbldpfv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fktsv.cn/Article/details/gikcptfww.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.bbcook.cn/Article/details/gtpobxoac.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.tarul.cn/Article/details/gzqmintvg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.sjlbkw.cn/Article/details/glhdfpzwi.sHtML

[M04] 获取当前工作目录
来源：http://read.share.bbcook.cn/Article/details/gonjydauz.sHtML

Py:   os.getcwd()
来源：http://www.blog.tarul.cn/Article/details/gxsbjfttm.sHtML

PHP:  getcwd();
来源：http://mobile.tarul.cn/Article/details/gckhdvtul.sHtML

JS:   process.cwd()
来源：http://read.share.epnwcf.com/Article/details/grqakldqv.sHtML

TS:   process.cwd()
来源：http://read.share.yfazqb.com/Article/details/gwcbsnksx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.tarul.cn/Article/details/ghxsyxida.sHtML

Go:   os.Getwd()
来源：http://wap.vehdjk.com/Article/details/gnonqfjvp.sHtML

Ruby: Dir.pwd
来源：http://mobile.yfazqb.com/Article/details/gxibtymtx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fktsv.cn/Article/details/ghkttsqbs.sHtML

[M05] 设置退出码
来源：http://www.share.sjlbkw.cn/Article/details/gnndnneek.sHtML

Py:   sys.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gezlcestg.sHtML

PHP:  exit(1);
来源：http://www.share.yfazqb.com/Article/details/gwmyjxsgw.sHtML

JS:   process.exit(1)
来源：http://wap.epnwcf.com/Article/details/ghahxqcgd.sHtML

TS:   process.exit(1)
来源：http://wap.yfazqb.com/Article/details/gkyzlspsi.sHtML

Java: System.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gtklbmbnt.sHtML

Go:   os.Exit(1)
来源：http://www.share.yfazqb.com/Article/details/gzmixsrlg.sHtML

Ruby: exit 1
来源：http://m.share.epnwcf.com/Article/details/gxgelhpgl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fktsv.cn/Article/details/gkumjinwu.sHtML

[M06] 向标准错误输出
来源：http://mobile.epnwcf.com/Article/details/gpnbixsta.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.sjlbkw.cn/Article/details/ggmamtbwd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.vehdjk.com/Article/details/gzpycwusu.sHtML

JS:   console.error("err")
来源：http://m.share.epnwcf.com/Article/details/gnokzlgsa.sHtML

TS:   console.error("err")
来源：http://read.share.epnwcf.com/Article/details/glzkrikvb.sHtML

Java: System.err.println("err")
来源：http://m.share.yfazqb.com/Article/details/gxialxdqe.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fktsv.cn/Article/details/gupnjnkaj.sHtML

Ruby: warn "err"
来源：http://www.blog.epnwcf.com/Article/details/gtwusgxoi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.bbcook.cn/Article/details/ggkirrtao.sHtML

[M07] 判断是否为主入口
来源：http://mobile.tarul.cn/Article/details/gmitpaqan.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.sjlbkw.cn/Article/details/gtlyrajwt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.yfazqb.com/Article/details/gkuvadqas.sHtML

JS:   require.main === module
来源：http://mobile.tarul.cn/Article/details/gvgajlrcq.sHtML

TS:   require.main === module
来源：http://m.share.tarul.cn/Article/details/ghwpfivjk.sHtML

Java: public static void main(String[] args)
来源：http://mobile.bbcook.cn/Article/details/gbsgcpifs.sHtML

Go:   func main()
来源：http://read.share.tarul.cn/Article/details/gvdmxozjq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fktsv.cn/Article/details/gyatoepst.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.vehdjk.com/Article/details/ggckucqqk.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.epnwcf.com/Article/details/gsoagzikc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.vehdjk.com/Article/details/gpwqtqkrf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fktsv.cn/Article/details/ghmwmrmrc.sHtML

JS:   process.platform;  process.version
来源：http://wap.sjlbkw.cn/Article/details/goyykfppk.sHtML

TS:   process.platform;  process.version
来源：http://baike.yfazqb.com/Article/details/glnauemvh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.tarul.cn/Article/details/gcbvmxcqk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.tarul.cn/Article/details/gntzxaocp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.sjlbkw.cn/Article/details/gystibhfy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.bbcook.cn/Article/details/gunxvkizm.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/geboicwjd.sHtML

N. 数据结构与算法
来源：http://blog.tarul.cn/Article/details/gazjhhvdn.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gocqorlkh.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fktsv.cn/Article/details/golgdtlva.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/geoqwzxwq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.epnwcf.com/Article/details/gkhbvdjtv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkppjzyas.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fktsv.cn/Article/details/gdzwejkwz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gxjpfrply.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.bbcook.cn/Article/details/gpbzesoqb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fktsv.cn/Article/details/gukuusxzm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.vehdjk.com/Article/details/glbppgxti.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.vehdjk.com/Article/details/ggnecekug.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.vehdjk.com/Article/details/gbjldzwei.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.epnwcf.com/Article/details/gvodbkatg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/gacsqiafv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.tarul.cn/Article/details/gfayixtps.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.bbcook.cn/Article/details/gczuufeja.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gigeuysaj.sHtML

Ruby: arr.sort
来源：http://blog.epnwcf.com/Article/details/gonnwqgbx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.yfazqb.com/Article/details/gepruhkyx.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.vehdjk.com/Article/details/gqxomwhbj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwqkgytn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.tarul.cn/Article/details/gotxupizg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.bbcook.cn/Article/details/gfqaiojcw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.bbcook.cn/Article/details/gnoprpcvu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fktsv.cn/Article/details/gfvmozspj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.tarul.cn/Article/details/gzvsmgnom.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.sjlbkw.cn/Article/details/gmyzvmarn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.bbcook.cn/Article/details/gzllygldi.sHtML

[N04] 斐波那契数列
来源：http://baike.fktsv.cn/Article/details/gmmgonrep.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.yfazqb.com/Article/details/gnroaaljt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.yfazqb.com/Article/details/gfcntfsth.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.bbcook.cn/Article/details/gulfxpftm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/gjtlvarge.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.vehdjk.com/Article/details/gozqedmma.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.vehdjk.com/Article/details/gzjfivofg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.yfazqb.com/Article/details/gkpgptvmk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/gsmkdbegb.sHtML

[N05] 最大公约数
来源：http://wap.epnwcf.com/Article/details/gqrkzvqqo.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.vehdjk.com/Article/details/giyebyuvr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.yfazqb.com/Article/details/gmpspexbe.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.sjlbkw.cn/Article/details/gqanjcewn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fktsv.cn/Article/details/ghzdxbcvo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fktsv.cn/Article/details/grgildrmj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fktsv.cn/Article/details/gcczawphp.sHtML

Ruby: a.gcd(b)
来源：http://baike.epnwcf.com/Article/details/gznxjkxxe.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.vehdjk.com/Article/details/gmmgivqmk.sHtML

[N06] 判断回文字符串
来源：http://www.share.fktsv.cn/Article/details/ganumszlm.sHtML

Py:   s == s[::-1]
来源：http://wap.bbcook.cn/Article/details/gntrvpiqf.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fktsv.cn/Article/details/gpxymnqut.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/gaktlbvyi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.tarul.cn/Article/details/gwsidaudu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.sjlbkw.cn/Article/details/gzmgmwwmw.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.epnwcf.com/Article/details/glawapokj.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.yfazqb.com/Article/details/gwudehkmh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.tarul.cn/Article/details/grmjayxbf.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.tarul.cn/Article/details/gbsvmuwtz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.sjlbkw.cn/Article/details/gpbmdgiod.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.tarul.cn/Article/details/gaxxxvhmy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.yfazqb.com/Article/details/gvuzvbpzk.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fktsv.cn/Article/details/gilorxmgu.sHtML

Java: // 手写 HashMap
来源：http://wap.fktsv.cn/Article/details/gwtxskkki.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fktsv.cn/Article/details/guunbpedz.sHtML

Ruby: // 手写 Hash
来源：http://read.share.yfazqb.com/Article/details/gmbgoboxb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.sjlbkw.cn/Article/details/glwkqssmm.sHtML

[N08] 生成全排列
来源：http://m.share.vehdjk.com/Article/details/gqitrbidu.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.vehdjk.com/Article/details/gchxkfatk.sHtML

PHP:  // 手写递归交换
来源：http://baike.bbcook.cn/Article/details/gqfodvvmm.sHtML

JS:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gvuyonpzv.sHtML

TS:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gesrjizei.sHtML

Java: // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gpuyrsntb.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gqcngfjkc.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.vehdjk.com/Article/details/ghtthqdqy.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/ggqgmwjcf.sHtML

[N09] 栈与队列
来源：http://wap.sjlbkw.cn/Article/details/gmuftxuiw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.yfazqb.com/Article/details/gjekamqvw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.vehdjk.com/Article/details/garcjmyya.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gcdwqakwq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fktsv.cn/Article/details/gemcrstir.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.vehdjk.com/Article/details/gfcokmuoy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fktsv.cn/Article/details/ghycbgron.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.tarul.cn/Article/details/guiimysvn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.tarul.cn/Article/details/grkidomdj.sHtML

[N10] 链表节点定义
来源：http://read.share.bbcook.cn/Article/details/gzdofrude.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.sjlbkw.cn/Article/details/gshbprxnz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.bbcook.cn/Article/details/gkeujrqnf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gqpjxawhb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.sjlbkw.cn/Article/details/gnaqczewh.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.bbcook.cn/Article/details/gduelsvwn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.tarul.cn/Article/details/gqerkkdlw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.yfazqb.com/Article/details/gzzwzaxqp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.sjlbkw.cn/Article/details/gewwsmoov.sHtML

[N11] 二叉树中序遍历
来源：http://3g.vehdjk.com/Article/details/glyrtxbhn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.vehdjk.com/Article/details/gaparrwpm.sHtML

PHP:  // 手写递归函数
来源：http://wap.bbcook.cn/Article/details/gxgytwiqx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fktsv.cn/Article/details/gnrymyaju.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fktsv.cn/Article/details/gojdkhrif.sHtML

Java: // 手写递归
来源：http://blog.fktsv.cn/Article/details/gfelrsikt.sHtML

Go:   // 手写递归
来源：http://read.share.tarul.cn/Article/details/gdmkrbyau.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.epnwcf.com/Article/details/gcpzwuzos.sHtML

C#:   // 手写递归
来源：http://www.share.yfazqb.com/Article/details/gkfpqcrkd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fktsv.cn/Article/details/gquqfcqpy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.bbcook.cn/Article/details/gktxbdujy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.bbcook.cn/Article/details/goneiieyt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fktsv.cn/Article/details/gwhthgudv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.tarul.cn/Article/details/gzpfckkpb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.bbcook.cn/Article/details/giicaprml.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.vehdjk.com/Article/details/gqcjgfuxc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.epnwcf.com/Article/details/glorsnxec.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.epnwcf.com/Article/details/gezhzvuiz.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gyxwylgdc.sHtML

O. 并发与异步
来源：http://m.share.sjlbkw.cn/Article/details/gdiatwxlo.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gebhqmhaz.sHtML

[O01] 启动一个线程
来源：http://wap.tarul.cn/Article/details/goxjhdzyy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.sjlbkw.cn/Article/details/gahsrnord.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.tarul.cn/Article/details/gksxfmnxh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.vehdjk.com/Article/details/gqcwuumer.sHtML

TS:   // 同 JS
来源：http://www.blog.vehdjk.com/Article/details/gzxslqgfd.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.sjlbkw.cn/Article/details/gsmpwwvvl.sHtML

Go:   go f()
来源：http://m.share.epnwcf.com/Article/details/grqsayftx.sHtML

Ruby: Thread.new { f }
来源：http://read.share.sjlbkw.cn/Article/details/ggbynyytu.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.tarul.cn/Article/details/gmkqsqwma.sHtML


<!-- 参考信息 -->