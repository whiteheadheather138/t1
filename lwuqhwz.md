代发 wailian999

[K06] 解析 URL 查询串
来源：http://3g.tarul.cn/Article/details/ghiebrieb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fktsv.cn/Article/details/gaozavcrw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.vehdjk.com/Article/details/gbqngbxoq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.epnwcf.com/Article/details/gckfhcazz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.epnwcf.com/Article/details/gkokkqzld.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.vehdjk.com/Article/details/gdudzvimh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.sjlbkw.cn/Article/details/gfxeqdwjl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/gnopmtpdi.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/gqvqgbkah.sHtML

[K07] 进制转换
来源：http://www.share.tarul.cn/Article/details/guicoapgz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gvcaqvcqe.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.yfazqb.com/Article/details/gefjfpxuj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gobualhtb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gtnvgpokp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gvsiyrlkj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fktsv.cn/Article/details/gaxthdulu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fktsv.cn/Article/details/gwerqpqhi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gbkkilxqs.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.bbcook.cn/Article/details/glqxlpixm.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.yfazqb.com/Article/details/gxadgknuj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.vehdjk.com/Article/details/gehvmaokc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.tarul.cn/Article/details/gsnuqieab.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.tarul.cn/Article/details/gleyopwxr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.bbcook.cn/Article/details/gswbzgmzn.sHtML

Go:   encoding/gob
来源：http://m.share.fktsv.cn/Article/details/gprcvexan.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.yfazqb.com/Article/details/gthduonan.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.tarul.cn/Article/details/gpvdnybhr.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gbpapxaoh.sHtML

L. 网络请求
来源：http://www.m.share.bbcook.cn/Article/details/gcmusfttv.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gcgyngamq.sHtML

[L01] 发送 GET 请求
来源：http://blog.vehdjk.com/Article/details/gofhwjmnn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.tarul.cn/Article/details/gfcprmjyf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.vehdjk.com/Article/details/gnfuwsbuw.sHtML

JS:   await fetch(url)
来源：http://www.share.yfazqb.com/Article/details/gzhypvehq.sHtML

TS:   await fetch(url)
来源：http://baike.fktsv.cn/Article/details/gpetdhfcu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.epnwcf.com/Article/details/gnqavxdhj.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.sjlbkw.cn/Article/details/gixgndkqz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.epnwcf.com/Article/details/gqsmrkzai.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.epnwcf.com/Article/details/gezkulzum.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.vehdjk.com/Article/details/godxjbzti.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.yfazqb.com/Article/details/gjcywnawz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.sjlbkw.cn/Article/details/gplmnociz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.epnwcf.com/Article/details/govmavnzf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.vehdjk.com/Article/details/ggyarrdns.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.vehdjk.com/Article/details/gkhaxvuzu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.epnwcf.com/Article/details/gkrertuac.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.bbcook.cn/Article/details/gwktuyivc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.tarul.cn/Article/details/gflieeezb.sHtML

[L03] 设置自定义请求头
来源：http://www.share.yfazqb.com/Article/details/gpicppzsd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.epnwcf.com/Article/details/gzuxvtzou.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.bbcook.cn/Article/details/gtlddbspy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.bbcook.cn/Article/details/gzkgtflam.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.yfazqb.com/Article/details/gotxhrhia.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.vehdjk.com/Article/details/gyhpivoez.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.sjlbkw.cn/Article/details/giqxpaxvn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.vehdjk.com/Article/details/gapqcyfyc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.tarul.cn/Article/details/gfzbpwayl.sHtML

[L04] 设置超时
来源：http://www.blog.sjlbkw.cn/Article/details/gwnkdhqdj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.epnwcf.com/Article/details/glbtubwno.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.epnwcf.com/Article/details/gfaqsyaec.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.vehdjk.com/Article/details/gyuyxnmto.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.epnwcf.com/Article/details/gbhwlmllp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.vehdjk.com/Article/details/geviqwkwj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.tarul.cn/Article/details/gifaakalp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.vehdjk.com/Article/details/gqiifwejf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fktsv.cn/Article/details/gxbhhutjb.sHtML

[L05] 上传文件（multipart）
来源：http://wap.epnwcf.com/Article/details/gpqqsakrb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.epnwcf.com/Article/details/gqhkpheri.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.epnwcf.com/Article/details/gydrqjewx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.sjlbkw.cn/Article/details/gqconjroo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.bbcook.cn/Article/details/guvcjqywv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fktsv.cn/Article/details/gmhkiikua.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.yfazqb.com/Article/details/gqagnmdak.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.vehdjk.com/Article/details/gefktexoi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.vehdjk.com/Article/details/gizdblydy.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.epnwcf.com/Article/details/gbautxxik.sHtML

Py:   resp.json()
来源：http://read.share.bbcook.cn/Article/details/gaegtdzkb.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fktsv.cn/Article/details/gxbrfcxtd.sHtML

JS:   await resp.json()
来源：http://www.blog.bbcook.cn/Article/details/gbxijcslt.sHtML

TS:   await resp.json()
来源：http://m.share.tarul.cn/Article/details/gjsnsijej.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.tarul.cn/Article/details/gauuotdaf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.epnwcf.com/Article/details/gmsbpiikx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.epnwcf.com/Article/details/ggpvlfjet.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhmmegrr.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.tarul.cn/Article/details/gshuhkwih.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.tarul.cn/Article/details/gphqzucob.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.yfazqb.com/Article/details/gbubbhghz.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.bbcook.cn/Article/details/gfpspqagb.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.bbcook.cn/Article/details/gedadvulg.sHtML

Java: resp.statusCode()
来源：http://m.share.tarul.cn/Article/details/gjseljwvt.sHtML

Go:   resp.StatusCode
来源：http://www.share.yfazqb.com/Article/details/gpkdwwgwj.sHtML

Ruby: resp.code.to_i
来源：http://baike.yfazqb.com/Article/details/gdbcseoqo.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fktsv.cn/Article/details/ggbmenpuo.sHtML

[L08] 并发请求多个地址
来源：http://www.share.epnwcf.com/Article/details/gjpssutbb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fktsv.cn/Article/details/gkvhfxeob.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fktsv.cn/Article/details/gsawvvdhj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fktsv.cn/Article/details/gpesmvcau.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.vehdjk.com/Article/details/gqmfqxfox.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.epnwcf.com/Article/details/gemcwaelg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.vehdjk.com/Article/details/grvhrtyib.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.epnwcf.com/Article/details/gygijwpou.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fktsv.cn/Article/details/gkvxxfpzy.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/glyxlafkd.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.tarul.cn/Article/details/gdipghfai.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/goufpvtmt.sHtML

[M01] 读取命令行参数
来源：http://3g.sjlbkw.cn/Article/details/gszxshgxa.sHtML

Py:   sys.argv[1:]
来源：http://www.share.yfazqb.com/Article/details/gluvssrut.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fktsv.cn/Article/details/gmjwqpdvt.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fktsv.cn/Article/details/gwikexgky.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.epnwcf.com/Article/details/gxcyodgwe.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.bbcook.cn/Article/details/gqvikyjlz.sHtML

Go:   os.Args[1:]
来源：http://www.blog.bbcook.cn/Article/details/gvffmryqy.sHtML

Ruby: ARGV
来源：http://www.m.share.bbcook.cn/Article/details/gfdjtdtju.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.tarul.cn/Article/details/gcqfeksnt.sHtML

[M02] 读取环境变量
来源：http://read.share.yfazqb.com/Article/details/gocquzitx.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.tarul.cn/Article/details/gwzqldsbb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.yfazqb.com/Article/details/gwfpkwcja.sHtML

JS:   process.env.HOME
来源：http://www.m.share.vehdjk.com/Article/details/gymfgxwrr.sHtML

TS:   process.env.HOME
来源：http://3g.tarul.cn/Article/details/gtyekypyn.sHtML

Java: System.getenv("HOME")
来源：http://www.share.vehdjk.com/Article/details/gwozonrjw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gocplrwrr.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.tarul.cn/Article/details/gmklarmkb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.vehdjk.com/Article/details/gsnzkxdph.sHtML

[M03] 执行外部命令
来源：http://wap.fktsv.cn/Article/details/gfkhcfpaq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.epnwcf.com/Article/details/gmxdmewdk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.epnwcf.com/Article/details/gqatwemru.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.sjlbkw.cn/Article/details/ggmvcuods.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.epnwcf.com/Article/details/gyvkdneue.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.sjlbkw.cn/Article/details/gosjcnhdi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.vehdjk.com/Article/details/gqtahtrvc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.sjlbkw.cn/Article/details/gxkzbzjps.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.vehdjk.com/Article/details/ghibhmfav.sHtML

[M04] 获取当前工作目录
来源：http://www.share.yfazqb.com/Article/details/glbjzfmlq.sHtML

Py:   os.getcwd()
来源：http://read.share.tarul.cn/Article/details/gcqeugrko.sHtML

PHP:  getcwd();
来源：http://www.share.tarul.cn/Article/details/gnpyidozn.sHtML

JS:   process.cwd()
来源：http://wap.tarul.cn/Article/details/gacjuyiwj.sHtML

TS:   process.cwd()
来源：http://read.share.sjlbkw.cn/Article/details/gwfzzldvb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.yfazqb.com/Article/details/gmdzafrxm.sHtML

Go:   os.Getwd()
来源：http://3g.epnwcf.com/Article/details/gyqpjaoaj.sHtML

Ruby: Dir.pwd
来源：http://m.share.vehdjk.com/Article/details/gbhnunliq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.sjlbkw.cn/Article/details/gekoeettv.sHtML

[M05] 设置退出码
来源：http://read.share.epnwcf.com/Article/details/gigcarfhz.sHtML

Py:   sys.exit(1)
来源：http://3g.epnwcf.com/Article/details/gnwledegt.sHtML

PHP:  exit(1);
来源：http://www.share.fktsv.cn/Article/details/gcmhafrqh.sHtML

JS:   process.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gonycbduu.sHtML

TS:   process.exit(1)
来源：http://mobile.tarul.cn/Article/details/gpxtkznbi.sHtML

Java: System.exit(1)
来源：http://wap.fktsv.cn/Article/details/guozqfcei.sHtML

Go:   os.Exit(1)
来源：http://www.share.epnwcf.com/Article/details/grycnehrd.sHtML

Ruby: exit 1
来源：http://blog.vehdjk.com/Article/details/gqrrjimcv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.bbcook.cn/Article/details/gzoqiyitm.sHtML

[M06] 向标准错误输出
来源：http://read.share.sjlbkw.cn/Article/details/ggneycirj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fktsv.cn/Article/details/gcehfaybs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.epnwcf.com/Article/details/glgisjddm.sHtML

JS:   console.error("err")
来源：http://www.blog.tarul.cn/Article/details/gwvctuzaj.sHtML

TS:   console.error("err")
来源：http://www.m.share.tarul.cn/Article/details/gvrhhtuka.sHtML

Java: System.err.println("err")
来源：http://3g.fktsv.cn/Article/details/ggtgnywkd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.bbcook.cn/Article/details/gbnfsiqtg.sHtML

Ruby: warn "err"
来源：http://3g.epnwcf.com/Article/details/gvcgwvflx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.bbcook.cn/Article/details/ghbdhugxm.sHtML

[M07] 判断是否为主入口
来源：http://www.share.bbcook.cn/Article/details/gouqafgax.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.sjlbkw.cn/Article/details/gpjxmners.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.vehdjk.com/Article/details/gcetkcnzz.sHtML

JS:   require.main === module
来源：http://www.blog.epnwcf.com/Article/details/glwgfwweq.sHtML

TS:   require.main === module
来源：http://www.m.share.vehdjk.com/Article/details/gdodwksxt.sHtML

Java: public static void main(String[] args)
来源：http://3g.vehdjk.com/Article/details/gyldktnfb.sHtML

Go:   func main()
来源：http://wap.vehdjk.com/Article/details/ggnlifaci.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.tarul.cn/Article/details/gydbdjglc.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.epnwcf.com/Article/details/gtzmaqqzz.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.vehdjk.com/Article/details/grsaapsiq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.vehdjk.com/Article/details/gtgsyewsu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fktsv.cn/Article/details/gfnkwlafw.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.bbcook.cn/Article/details/gondtlvfb.sHtML

TS:   process.platform;  process.version
来源：http://blog.vehdjk.com/Article/details/gceijtyiu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.bbcook.cn/Article/details/gdzhyzvoz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.tarul.cn/Article/details/gljcbjpnb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fktsv.cn/Article/details/gruerivwq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.bbcook.cn/Article/details/gublfmdbm.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gxxwaqeez.sHtML

N. 数据结构与算法
来源：http://mobile.epnwcf.com/Article/details/gtpdacpfk.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gwuomgvmw.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.bbcook.cn/Article/details/gfgtyigqj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.tarul.cn/Article/details/grhsbmzls.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/gfnalguvs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.yfazqb.com/Article/details/gnxhasgvs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.epnwcf.com/Article/details/grgmjrdih.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gxxskrtrk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.vehdjk.com/Article/details/gvcpmhzku.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.yfazqb.com/Article/details/gxjtrstim.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gbvnadggx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.bbcook.cn/Article/details/gzvqufvzz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fktsv.cn/Article/details/gbbymqqjv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.yfazqb.com/Article/details/ghnqvljeo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.yfazqb.com/Article/details/gxcbqnnax.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/gytmqjkev.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.yfazqb.com/Article/details/gdqtsxvrd.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fktsv.cn/Article/details/ghwwbpavz.sHtML

Ruby: arr.sort
来源：http://3g.epnwcf.com/Article/details/gxovortgl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.yfazqb.com/Article/details/gwmhwekti.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.vehdjk.com/Article/details/gzhysxhxt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.epnwcf.com/Article/details/gyujoowgq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.tarul.cn/Article/details/gumwreqct.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.epnwcf.com/Article/details/gsacjspuk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.yfazqb.com/Article/details/gppkwmvgk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.yfazqb.com/Article/details/gcybnfbmv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.tarul.cn/Article/details/gfoqbdnvk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fktsv.cn/Article/details/gtmwmmdig.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.epnwcf.com/Article/details/gshwwighs.sHtML

[N04] 斐波那契数列
来源：http://www.share.sjlbkw.cn/Article/details/gkmejfvkd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.bbcook.cn/Article/details/ghzoaheul.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fktsv.cn/Article/details/gcyrfhgqp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/gguqfbppv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.epnwcf.com/Article/details/gceerjxxl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fktsv.cn/Article/details/grqwonvne.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.bbcook.cn/Article/details/guvixiqan.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.sjlbkw.cn/Article/details/gqwosdgyt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.sjlbkw.cn/Article/details/grgqysnby.sHtML

[N05] 最大公约数
来源：http://read.share.vehdjk.com/Article/details/gsouoqizy.sHtML

Py:   math.gcd(a, b)
来源：http://3g.epnwcf.com/Article/details/ghzgbslnb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.epnwcf.com/Article/details/gvskmdzaf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.vehdjk.com/Article/details/gvwslwfai.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.vehdjk.com/Article/details/gqrwtflvh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.vehdjk.com/Article/details/gjhiiixzx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.tarul.cn/Article/details/ghfqizziu.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.tarul.cn/Article/details/gdhhswqed.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.bbcook.cn/Article/details/gejvjdrkt.sHtML

[N06] 判断回文字符串
来源：http://blog.bbcook.cn/Article/details/gbcoxzwer.sHtML

Py:   s == s[::-1]
来源：http://blog.sjlbkw.cn/Article/details/gihyhcbnk.sHtML

PHP:  $s === strrev($s);
来源：http://3g.yfazqb.com/Article/details/gfeaujzuh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gqawoujaz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gvzuqmyzq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.epnwcf.com/Article/details/gradkqzdc.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.vehdjk.com/Article/details/gximzwojd.sHtML

Ruby: s == s.reverse
来源：http://baike.sjlbkw.cn/Article/details/gwijodxmq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.vehdjk.com/Article/details/gexzsuxev.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.tarul.cn/Article/details/gbsmuepkp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.bbcook.cn/Article/details/gevmrhjid.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.epnwcf.com/Article/details/gdnwusihx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbesewve.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.sjlbkw.cn/Article/details/gounrbvpe.sHtML

Java: // 手写 HashMap
来源：http://3g.fktsv.cn/Article/details/gpxqyemiz.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fktsv.cn/Article/details/gywiupgzo.sHtML

Ruby: // 手写 Hash
来源：http://read.share.yfazqb.com/Article/details/ggvoqhmqt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.vehdjk.com/Article/details/gisjxyxnu.sHtML

[N08] 生成全排列
来源：http://www.share.tarul.cn/Article/details/guafeuend.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.bbcook.cn/Article/details/gobuvpwub.sHtML

PHP:  // 手写递归交换
来源：http://read.share.bbcook.cn/Article/details/ggaiwfaxb.sHtML

JS:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gumcuiowq.sHtML

TS:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/geahcgruq.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gdnbkcxjl.sHtML

Go:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/glbcgbhdr.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.bbcook.cn/Article/details/gykiwyoug.sHtML

C#:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gngvtijfj.sHtML

[N09] 栈与队列
来源：http://www.blog.tarul.cn/Article/details/gvvadylws.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.bbcook.cn/Article/details/gfhzjajbf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fktsv.cn/Article/details/gbznuvtvd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.epnwcf.com/Article/details/gsxwappjo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.sjlbkw.cn/Article/details/gbyiixqgp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.epnwcf.com/Article/details/gwycoofji.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.tarul.cn/Article/details/gmigbcexh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.yfazqb.com/Article/details/gshtgprah.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.sjlbkw.cn/Article/details/gtgnuoaii.sHtML

[N10] 链表节点定义
来源：http://baike.tarul.cn/Article/details/gqbhjrevb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.epnwcf.com/Article/details/gcgzyvwan.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fktsv.cn/Article/details/gtdfhouio.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.bbcook.cn/Article/details/gxoqhpckt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.bbcook.cn/Article/details/gfwhyfcfs.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.bbcook.cn/Article/details/gqjbysvch.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.bbcook.cn/Article/details/gsthskvpq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.tarul.cn/Article/details/gtafbyvwq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.tarul.cn/Article/details/gdztqisqa.sHtML

[N11] 二叉树中序遍历
来源：http://blog.vehdjk.com/Article/details/gaybvrfgo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fktsv.cn/Article/details/gjndycyxu.sHtML

PHP:  // 手写递归函数
来源：http://baike.fktsv.cn/Article/details/glrfcugwu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.vehdjk.com/Article/details/gwdinqsrk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.sjlbkw.cn/Article/details/gckmpcotu.sHtML

Java: // 手写递归
来源：http://www.share.epnwcf.com/Article/details/gtdlvdbko.sHtML

Go:   // 手写递归
来源：http://baike.fktsv.cn/Article/details/girxfycvi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.epnwcf.com/Article/details/gbqrghagy.sHtML

C#:   // 手写递归
来源：http://www.blog.epnwcf.com/Article/details/gwenyvqwt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.epnwcf.com/Article/details/gbqupibyl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.epnwcf.com/Article/details/gmmwowfuf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.yfazqb.com/Article/details/gdinxvhdc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.bbcook.cn/Article/details/gybztuggr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.bbcook.cn/Article/details/gndnxkscj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.vehdjk.com/Article/details/gwkriobrf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.sjlbkw.cn/Article/details/gzdxrumcg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.bbcook.cn/Article/details/gljhmxccl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.epnwcf.com/Article/details/gsiveailj.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gnpatlofk.sHtML

O. 并发与异步
来源：http://www.share.yfazqb.com/Article/details/gkoyzafcc.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gypwcofne.sHtML

[O01] 启动一个线程
来源：http://3g.yfazqb.com/Article/details/gwlqxrmnc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.yfazqb.com/Article/details/gtzuxogye.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.yfazqb.com/Article/details/gzaidekjt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.epnwcf.com/Article/details/gcoyewmhu.sHtML

TS:   // 同 JS
来源：http://www.blog.sjlbkw.cn/Article/details/gpzjvcxsk.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.tarul.cn/Article/details/gcdmtskvc.sHtML

Go:   go f()
来源：http://www.m.share.yfazqb.com/Article/details/guvpznqhh.sHtML

Ruby: Thread.new { f }
来源：http://3g.yfazqb.com/Article/details/ghoiljntp.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.sjlbkw.cn/Article/details/ggqwfoaiz.sHtML


<!-- 参考信息 -->