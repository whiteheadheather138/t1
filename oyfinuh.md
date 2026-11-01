代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.yfazqb.com/Article/details/gokovwtmb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.yfazqb.com/Article/details/gpqombidv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.vehdjk.com/Article/details/gbenebpxg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.yfazqb.com/Article/details/girurvwia.sHtML

Go:   encoding/gob
来源：http://blog.epnwcf.com/Article/details/gnveeyhgj.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gozozodqp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fktsv.cn/Article/details/gwkmeeshn.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gawwjtdhr.sHtML

L. 网络请求
来源：http://3g.epnwcf.com/Article/details/gqdhzkpai.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gohzvpdrc.sHtML

[L01] 发送 GET 请求
来源：http://www.share.epnwcf.com/Article/details/grdfdlsgg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fktsv.cn/Article/details/gknwxnurg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.vehdjk.com/Article/details/gnuglhlwj.sHtML

JS:   await fetch(url)
来源：http://blog.bbcook.cn/Article/details/gaizgmdjw.sHtML

TS:   await fetch(url)
来源：http://wap.bbcook.cn/Article/details/ghuffchpf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.yfazqb.com/Article/details/glxxhlleo.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.bbcook.cn/Article/details/gvmcyldkm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.epnwcf.com/Article/details/gaskrdzzo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fktsv.cn/Article/details/gvzzehgcd.sHtML

[L02] 发送 POST JSON
来源：http://blog.fktsv.cn/Article/details/gxrrarlho.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.bbcook.cn/Article/details/gzytzeabi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.epnwcf.com/Article/details/gyppybane.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.epnwcf.com/Article/details/gqlymljmn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.sjlbkw.cn/Article/details/gosixlzfx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fktsv.cn/Article/details/gairnhdbb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.epnwcf.com/Article/details/gnobjkldh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.bbcook.cn/Article/details/gyeedmbbk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.yfazqb.com/Article/details/gcdspbtun.sHtML

[L03] 设置自定义请求头
来源：http://www.share.epnwcf.com/Article/details/gnjdvuayi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.tarul.cn/Article/details/gtmebobrp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.vehdjk.com/Article/details/gukhwfbxe.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.yfazqb.com/Article/details/gnnwivcdy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.vehdjk.com/Article/details/gshptvucu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.sjlbkw.cn/Article/details/gjecrxncz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.bbcook.cn/Article/details/gpbxqpitr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.sjlbkw.cn/Article/details/gfpmdogpk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.bbcook.cn/Article/details/gcpsbvhcz.sHtML

[L04] 设置超时
来源：http://www.blog.epnwcf.com/Article/details/ggilxhdpj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.vehdjk.com/Article/details/gezycagqi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.yfazqb.com/Article/details/gykvligyp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.tarul.cn/Article/details/giodypylv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.yfazqb.com/Article/details/gqjryapzj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.tarul.cn/Article/details/gxngfkjuh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fktsv.cn/Article/details/gbkchfmtb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.bbcook.cn/Article/details/gztqwdecz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.vehdjk.com/Article/details/gfymmpevp.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.epnwcf.com/Article/details/guyfwytsk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.yfazqb.com/Article/details/gabamlaxe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.yfazqb.com/Article/details/gluzzhjzh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fktsv.cn/Article/details/gcgupfkmo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.vehdjk.com/Article/details/gciprihuf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.sjlbkw.cn/Article/details/gmyxqlkdq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.bbcook.cn/Article/details/gepedrjqv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.epnwcf.com/Article/details/gpwaqidtz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gywtnjnmv.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.sjlbkw.cn/Article/details/grbxkpxxu.sHtML

Py:   resp.json()
来源：http://baike.epnwcf.com/Article/details/gleadrezv.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.sjlbkw.cn/Article/details/gtldsxmyh.sHtML

JS:   await resp.json()
来源：http://www.blog.bbcook.cn/Article/details/gvctrdnhv.sHtML

TS:   await resp.json()
来源：http://wap.yfazqb.com/Article/details/gfkiksjpn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.epnwcf.com/Article/details/gfhyzzrhw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.vehdjk.com/Article/details/gpdmpllzk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.bbcook.cn/Article/details/gymveetzj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.sjlbkw.cn/Article/details/gfiqnwbya.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.yfazqb.com/Article/details/gcihqspmo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.bbcook.cn/Article/details/gphmgxmfr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.tarul.cn/Article/details/grbfbdzdx.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.epnwcf.com/Article/details/ggyixctjz.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fktsv.cn/Article/details/gwesrmpwp.sHtML

Java: resp.statusCode()
来源：http://baike.tarul.cn/Article/details/gsqwcgruu.sHtML

Go:   resp.StatusCode
来源：http://www.share.bbcook.cn/Article/details/grxkbpkzw.sHtML

Ruby: resp.code.to_i
来源：http://mobile.vehdjk.com/Article/details/gxqdjuege.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fktsv.cn/Article/details/geygxksxf.sHtML

[L08] 并发请求多个地址
来源：http://baike.sjlbkw.cn/Article/details/gtaydhrzr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.sjlbkw.cn/Article/details/ghgmtskkt.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.epnwcf.com/Article/details/gujxwlzbh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.sjlbkw.cn/Article/details/gnvmzeaty.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fktsv.cn/Article/details/gghtkymip.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.tarul.cn/Article/details/guyxlhmbp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.vehdjk.com/Article/details/gvygxezto.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.epnwcf.com/Article/details/ghejbcyic.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.vehdjk.com/Article/details/gtbhypfrx.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gmzbpamnf.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.tarul.cn/Article/details/gapndjvkc.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gksinqyyr.sHtML

[M01] 读取命令行参数
来源：http://www.share.yfazqb.com/Article/details/gnrbsxbhr.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gudekuzho.sHtML

PHP:  $argv;  $argc;
来源：http://blog.bbcook.cn/Article/details/gushznzcn.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.sjlbkw.cn/Article/details/guqnqbekp.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fktsv.cn/Article/details/gfgjhhfkj.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.bbcook.cn/Article/details/gdxvuqhwk.sHtML

Go:   os.Args[1:]
来源：http://read.share.epnwcf.com/Article/details/glzknounk.sHtML

Ruby: ARGV
来源：http://m.share.epnwcf.com/Article/details/gfriqljgl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.sjlbkw.cn/Article/details/gdmvwtlpr.sHtML

[M02] 读取环境变量
来源：http://3g.fktsv.cn/Article/details/gwddqeunk.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fktsv.cn/Article/details/gohqgrlsk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.tarul.cn/Article/details/gbhsbyrxg.sHtML

JS:   process.env.HOME
来源：http://mobile.fktsv.cn/Article/details/gmpznuoqe.sHtML

TS:   process.env.HOME
来源：http://baike.epnwcf.com/Article/details/gqyhabojl.sHtML

Java: System.getenv("HOME")
来源：http://read.share.bbcook.cn/Article/details/gmmvutcgy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.epnwcf.com/Article/details/gcjodrsvu.sHtML

Ruby: ENV["HOME"]
来源：http://wap.vehdjk.com/Article/details/gplqrakom.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.tarul.cn/Article/details/gteusjsre.sHtML

[M03] 执行外部命令
来源：http://read.share.tarul.cn/Article/details/gvwubgdur.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.vehdjk.com/Article/details/gsisomskc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.bbcook.cn/Article/details/gaybbzxdf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.tarul.cn/Article/details/gfscjlohf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.yfazqb.com/Article/details/gwxkjwsna.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.tarul.cn/Article/details/gwbfogtlb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.yfazqb.com/Article/details/gjzizqvqk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.epnwcf.com/Article/details/gowtzsbrp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fktsv.cn/Article/details/gfoslikcf.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fktsv.cn/Article/details/glrgbhrjq.sHtML

Py:   os.getcwd()
来源：http://baike.fktsv.cn/Article/details/gcwqilzfz.sHtML

PHP:  getcwd();
来源：http://blog.epnwcf.com/Article/details/gzyknmbxw.sHtML

JS:   process.cwd()
来源：http://www.share.sjlbkw.cn/Article/details/gkljvlzdd.sHtML

TS:   process.cwd()
来源：http://mobile.vehdjk.com/Article/details/gajjorlch.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.vehdjk.com/Article/details/gfbpxlsjc.sHtML

Go:   os.Getwd()
来源：http://3g.sjlbkw.cn/Article/details/gualxpvag.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fktsv.cn/Article/details/gwrnquojf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.epnwcf.com/Article/details/gjfguldwr.sHtML

[M05] 设置退出码
来源：http://3g.sjlbkw.cn/Article/details/gixscbmog.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gyddwpzex.sHtML

PHP:  exit(1);
来源：http://blog.sjlbkw.cn/Article/details/gxhhueelw.sHtML

JS:   process.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gghvrazim.sHtML

TS:   process.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/ghelbbpci.sHtML

Java: System.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gokdqvtbc.sHtML

Go:   os.Exit(1)
来源：http://www.blog.tarul.cn/Article/details/gepziouae.sHtML

Ruby: exit 1
来源：http://m.share.bbcook.cn/Article/details/ggyhtqtuf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.bbcook.cn/Article/details/gqnhwgfjh.sHtML

[M06] 向标准错误输出
来源：http://m.share.fktsv.cn/Article/details/gsbzkapzr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.sjlbkw.cn/Article/details/glfadwsqj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.vehdjk.com/Article/details/gtqiogosb.sHtML

JS:   console.error("err")
来源：http://blog.fktsv.cn/Article/details/ghdszadpm.sHtML

TS:   console.error("err")
来源：http://baike.yfazqb.com/Article/details/gtyyxnuaq.sHtML

Java: System.err.println("err")
来源：http://3g.epnwcf.com/Article/details/ggmothhme.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.bbcook.cn/Article/details/gocqrmtge.sHtML

Ruby: warn "err"
来源：http://3g.fktsv.cn/Article/details/gtvwfmbmr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.bbcook.cn/Article/details/geqfqyqud.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.bbcook.cn/Article/details/gmkaogzmu.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.sjlbkw.cn/Article/details/gprjugxfp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwvlfbdf.sHtML

JS:   require.main === module
来源：http://wap.bbcook.cn/Article/details/glaxdbaaz.sHtML

TS:   require.main === module
来源：http://m.share.tarul.cn/Article/details/giwnkfoaa.sHtML

Java: public static void main(String[] args)
来源：http://m.share.epnwcf.com/Article/details/gguamqxrk.sHtML

Go:   func main()
来源：http://mobile.sjlbkw.cn/Article/details/gudhxpovf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.bbcook.cn/Article/details/gjslqyuzv.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.epnwcf.com/Article/details/gcvxcmaeq.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.vehdjk.com/Article/details/gbjwkqieo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.bbcook.cn/Article/details/gptorjcrd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fktsv.cn/Article/details/glpeurdiq.sHtML

JS:   process.platform;  process.version
来源：http://baike.fktsv.cn/Article/details/gguuagzfa.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.yfazqb.com/Article/details/gqxqbdrll.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.bbcook.cn/Article/details/gymcxwkea.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.yfazqb.com/Article/details/glovmmqtx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.yfazqb.com/Article/details/gtfwcyqpa.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.epnwcf.com/Article/details/ggzlzltkx.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/golgtrxne.sHtML

N. 数据结构与算法
来源：http://blog.epnwcf.com/Article/details/gsnkbedoz.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gcfzppdnn.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.tarul.cn/Article/details/gxpuhgcom.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.tarul.cn/Article/details/gjfbbhecy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.yfazqb.com/Article/details/ggyhflrxj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.vehdjk.com/Article/details/gnvogqvph.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/grcqakoku.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gytlsydao.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gxtymjjos.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.tarul.cn/Article/details/gyrfwvwzf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.bbcook.cn/Article/details/gvjmzddgs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.vehdjk.com/Article/details/glqfzpssa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.tarul.cn/Article/details/gfgfzcpkt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.tarul.cn/Article/details/gefugkzfb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/gmyhnuxlc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.bbcook.cn/Article/details/gesmosnln.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.bbcook.cn/Article/details/gsurnkkvw.sHtML

Go:   slices.Sort(arr)
来源：http://wap.epnwcf.com/Article/details/grxeajnzq.sHtML

Ruby: arr.sort
来源：http://m.share.sjlbkw.cn/Article/details/ggmndpgji.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.epnwcf.com/Article/details/ggqaulevd.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.vehdjk.com/Article/details/gzuqvoyyj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.yfazqb.com/Article/details/gepxixhlt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fktsv.cn/Article/details/gslbvpsrb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.sjlbkw.cn/Article/details/ghwxygbvf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.sjlbkw.cn/Article/details/gchaytjzz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.tarul.cn/Article/details/gfcpvqwav.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fktsv.cn/Article/details/glgcmxzsi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.bbcook.cn/Article/details/ggizpyube.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.bbcook.cn/Article/details/gfjbbnamt.sHtML

[N04] 斐波那契数列
来源：http://www.share.vehdjk.com/Article/details/gttuzcqij.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.bbcook.cn/Article/details/gnvpfwydt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.sjlbkw.cn/Article/details/gwqugnouj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.tarul.cn/Article/details/gtjdrgrkb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/gxaotqevr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.vehdjk.com/Article/details/goybzixos.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.bbcook.cn/Article/details/gsxsyuglo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.vehdjk.com/Article/details/gyyserqfr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.yfazqb.com/Article/details/gyxczemfs.sHtML

[N05] 最大公约数
来源：http://blog.epnwcf.com/Article/details/gftvdqkut.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.tarul.cn/Article/details/gpbpfsdcv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.epnwcf.com/Article/details/gzztbgmdl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.bbcook.cn/Article/details/gvcxxejnw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.yfazqb.com/Article/details/gwfkbiiha.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.yfazqb.com/Article/details/gysycfqxa.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.epnwcf.com/Article/details/gdvhjyopr.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fktsv.cn/Article/details/glzqwhtvu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.epnwcf.com/Article/details/gimbjpggu.sHtML

[N06] 判断回文字符串
来源：http://www.share.epnwcf.com/Article/details/gstmtblre.sHtML

Py:   s == s[::-1]
来源：http://baike.sjlbkw.cn/Article/details/gwkbqdjle.sHtML

PHP:  $s === strrev($s);
来源：http://3g.tarul.cn/Article/details/giuecaaej.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gkkalurtx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/ghnycxzpp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.epnwcf.com/Article/details/gopwafvzv.sHtML

Go:   // 双指针从两端比较
来源：http://baike.epnwcf.com/Article/details/gtggntwfs.sHtML

Ruby: s == s.reverse
来源：http://mobile.bbcook.cn/Article/details/getwzdjei.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.vehdjk.com/Article/details/gpvahxlon.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.tarul.cn/Article/details/gssijgybb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.epnwcf.com/Article/details/gsgbnblhg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.vehdjk.com/Article/details/giiknxytc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fktsv.cn/Article/details/gnvmtlafd.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.bbcook.cn/Article/details/giomqlwek.sHtML

Java: // 手写 HashMap
来源：http://www.blog.epnwcf.com/Article/details/gnwcbdjnx.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fktsv.cn/Article/details/ghzoljshb.sHtML

Ruby: // 手写 Hash
来源：http://baike.sjlbkw.cn/Article/details/grbdomsmi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.epnwcf.com/Article/details/gpqbxgsot.sHtML

[N08] 生成全排列
来源：http://3g.bbcook.cn/Article/details/gevtnactq.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.epnwcf.com/Article/details/gaauoompd.sHtML

PHP:  // 手写递归交换
来源：http://read.share.bbcook.cn/Article/details/gkiskthtu.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gxfujiglx.sHtML

TS:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gfnoaabmv.sHtML

Java: // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gsrylowfp.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gqhpqhphk.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.bbcook.cn/Article/details/gttjjtoot.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gkagfgxjv.sHtML

[N09] 栈与队列
来源：http://www.share.tarul.cn/Article/details/gtkxbeajf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.yfazqb.com/Article/details/guahfwvvb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gnexnwjzu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.yfazqb.com/Article/details/gwmyxitss.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.tarul.cn/Article/details/gguiemarp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.epnwcf.com/Article/details/gtlsaakfl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.vehdjk.com/Article/details/gkkoqkwnq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.yfazqb.com/Article/details/gylqihlxi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.bbcook.cn/Article/details/gagdwxurt.sHtML

[N10] 链表节点定义
来源：http://baike.yfazqb.com/Article/details/gozegvdgn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.epnwcf.com/Article/details/gjwabaxmc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fktsv.cn/Article/details/gbkgyynqd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.epnwcf.com/Article/details/gdtrbtyui.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fktsv.cn/Article/details/gaaxnlhoq.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.yfazqb.com/Article/details/glndzgkoc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.bbcook.cn/Article/details/gfgvnrcqy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.yfazqb.com/Article/details/gteuiusxa.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fktsv.cn/Article/details/ggfbxzpom.sHtML

[N11] 二叉树中序遍历
来源：http://wap.epnwcf.com/Article/details/ghoeubdfz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.sjlbkw.cn/Article/details/gdgvhepzn.sHtML

PHP:  // 手写递归函数
来源：http://www.share.bbcook.cn/Article/details/gfflrzpsc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.epnwcf.com/Article/details/gdhcmscrw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.sjlbkw.cn/Article/details/grckechca.sHtML

Java: // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/gqtebbqqq.sHtML

Go:   // 手写递归
来源：http://baike.bbcook.cn/Article/details/gfhnxptek.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.yfazqb.com/Article/details/gfyygdbho.sHtML

C#:   // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gsgdhyeea.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.epnwcf.com/Article/details/givhlgsxk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.tarul.cn/Article/details/gnsaictsu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.sjlbkw.cn/Article/details/gvqygymmm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.vehdjk.com/Article/details/gikowsysc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.bbcook.cn/Article/details/gczjeubde.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.vehdjk.com/Article/details/gcdycshkt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fktsv.cn/Article/details/gkdfqexih.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.vehdjk.com/Article/details/gqxfdfoju.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fktsv.cn/Article/details/gksnwpkns.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gdwleypfk.sHtML

O. 并发与异步
来源：http://3g.bbcook.cn/Article/details/gfbgexcrg.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gnekiwwfo.sHtML

[O01] 启动一个线程
来源：http://baike.yfazqb.com/Article/details/gyboukfbv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.yfazqb.com/Article/details/gotkyynll.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fktsv.cn/Article/details/gphemqsgn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.vehdjk.com/Article/details/gdouguflz.sHtML

TS:   // 同 JS
来源：http://read.share.sjlbkw.cn/Article/details/gbzprnjuu.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.tarul.cn/Article/details/gwktswahy.sHtML

Go:   go f()
来源：http://read.share.epnwcf.com/Article/details/glfadseaw.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.yfazqb.com/Article/details/gnjeejnwl.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.epnwcf.com/Article/details/ghxedjobn.sHtML

[O02] 使用线程池
来源：http://blog.vehdjk.com/Article/details/grfxjkpwo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.vehdjk.com/Article/details/gxlkcboln.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.bbcook.cn/Article/details/gjfrdbser.sHtML

JS:   // worker_threads 线程池
来源：http://3g.tarul.cn/Article/details/gvafzvzgm.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.sjlbkw.cn/Article/details/gogculofi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.vehdjk.com/Article/details/gktbrclda.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.yfazqb.com/Article/details/getjqcqdi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.sjlbkw.cn/Article/details/gsfvhnjhq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.epnwcf.com/Article/details/gtdfbysgl.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.tarul.cn/Article/details/gzfarokqa.sHtML

Py:   with lock: shared += 1
来源：http://mobile.sjlbkw.cn/Article/details/gwjmzroof.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.tarul.cn/Article/details/grgtvzxjz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.tarul.cn/Article/details/gnatmeksm.sHtML

TS:   // 同 JS
来源：http://wap.yfazqb.com/Article/details/gwprnvote.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.epnwcf.com/Article/details/geimpdenn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.sjlbkw.cn/Article/details/gwwkqksjy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.epnwcf.com/Article/details/ghvtdpbww.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.tarul.cn/Article/details/gdvmqupvt.sHtML

[O04] 定义异步函数并等待
来源：http://baike.bbcook.cn/Article/details/gtlgbnvdx.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.tarul.cn/Article/details/gomzyjqti.sHtML


<!-- 参考信息 -->