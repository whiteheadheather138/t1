代发 wailian999

Go:   encoding/gob
来源：http://wap.yfazqb.com/Article/details/gtaupndww.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gteewvjbg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.vehdjk.com/Article/details/gpxxbutxr.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gigjydwuo.sHtML

L. 网络请求
来源：http://blog.yfazqb.com/Article/details/gwbneyzzu.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/grtyqekiv.sHtML

[L01] 发送 GET 请求
来源：http://read.share.sjlbkw.cn/Article/details/gixrzfmps.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fktsv.cn/Article/details/ghrvuxbxz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.yfazqb.com/Article/details/gbglfddgz.sHtML

JS:   await fetch(url)
来源：http://www.blog.bbcook.cn/Article/details/gtuyijufg.sHtML

TS:   await fetch(url)
来源：http://www.blog.yfazqb.com/Article/details/gaveelyqb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.bbcook.cn/Article/details/ghwtelhvo.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.sjlbkw.cn/Article/details/grvvvtexq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.bbcook.cn/Article/details/gbbpkrcqb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.sjlbkw.cn/Article/details/gxhoixfqu.sHtML

[L02] 发送 POST JSON
来源：http://baike.bbcook.cn/Article/details/gjgpyerxi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.vehdjk.com/Article/details/gbiishyjw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.bbcook.cn/Article/details/glfkxlgkb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.epnwcf.com/Article/details/giujqjytu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.vehdjk.com/Article/details/gvifhfacn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.yfazqb.com/Article/details/gdmvynoly.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.sjlbkw.cn/Article/details/gluwzkoko.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.yfazqb.com/Article/details/gmnveszac.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.vehdjk.com/Article/details/gcwbwyupi.sHtML

[L03] 设置自定义请求头
来源：http://www.share.vehdjk.com/Article/details/gzbtkyapq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.tarul.cn/Article/details/ggyurbebv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.epnwcf.com/Article/details/grakqkbvf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.vehdjk.com/Article/details/gkqvcnkrf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.sjlbkw.cn/Article/details/gseyawzmr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.epnwcf.com/Article/details/guywxsflb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fktsv.cn/Article/details/gsoaaidze.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.epnwcf.com/Article/details/gangnabth.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fktsv.cn/Article/details/gfbdeqjuu.sHtML

[L04] 设置超时
来源：http://read.share.sjlbkw.cn/Article/details/guvqhuegl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.epnwcf.com/Article/details/gtfkgnhzc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.yfazqb.com/Article/details/gsxosmjyp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.epnwcf.com/Article/details/gagxglecl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.yfazqb.com/Article/details/gpnnzonmq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.tarul.cn/Article/details/gijlyquun.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.yfazqb.com/Article/details/goxlybmzo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.sjlbkw.cn/Article/details/grtctcprg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.vehdjk.com/Article/details/guyrxqlvj.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.yfazqb.com/Article/details/gccjsexqg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.vehdjk.com/Article/details/gxncnwzmk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.epnwcf.com/Article/details/gswaeoilk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.tarul.cn/Article/details/gxfskoqjn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.sjlbkw.cn/Article/details/gkrkcnflx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.bbcook.cn/Article/details/gxyrczsri.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.epnwcf.com/Article/details/gpjxsxnsn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.vehdjk.com/Article/details/gtzibbdcc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gabnshqml.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fktsv.cn/Article/details/gdckvhklc.sHtML

Py:   resp.json()
来源：http://m.share.yfazqb.com/Article/details/gcghojvad.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.sjlbkw.cn/Article/details/gvqvtfvvk.sHtML

JS:   await resp.json()
来源：http://www.blog.bbcook.cn/Article/details/gjwudzsng.sHtML

TS:   await resp.json()
来源：http://www.blog.fktsv.cn/Article/details/guhcaxhtl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.vehdjk.com/Article/details/gpnhraujj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.epnwcf.com/Article/details/guzkwbzzu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.epnwcf.com/Article/details/glbzvnmrs.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.yfazqb.com/Article/details/gqkjokiib.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.tarul.cn/Article/details/gpokywvgd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.tarul.cn/Article/details/gosxwllzo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fktsv.cn/Article/details/gzqxdkqgh.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.yfazqb.com/Article/details/gzejzagim.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmekwsbn.sHtML

Java: resp.statusCode()
来源：http://www.share.fktsv.cn/Article/details/gxowtghgj.sHtML

Go:   resp.StatusCode
来源：http://www.blog.tarul.cn/Article/details/gxmxzdwxb.sHtML

Ruby: resp.code.to_i
来源：http://blog.vehdjk.com/Article/details/gaqqyukkb.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.epnwcf.com/Article/details/gbhmulysp.sHtML

[L08] 并发请求多个地址
来源：http://wap.sjlbkw.cn/Article/details/grntndijg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.bbcook.cn/Article/details/gqvjzzrif.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.bbcook.cn/Article/details/glhigyphm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/geppisqvs.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.bbcook.cn/Article/details/gcfaqngvn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fktsv.cn/Article/details/griqbinak.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.yfazqb.com/Article/details/geviqszkn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.yfazqb.com/Article/details/gjesckbbk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.tarul.cn/Article/details/goazgikwh.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gatwsmvlx.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.sjlbkw.cn/Article/details/gesrxlieu.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gexcytjok.sHtML

[M01] 读取命令行参数
来源：http://read.share.fktsv.cn/Article/details/gorogggvq.sHtML

Py:   sys.argv[1:]
来源：http://www.share.yfazqb.com/Article/details/gmxaegmmy.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fktsv.cn/Article/details/gicptbkql.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.tarul.cn/Article/details/geqsicygu.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fktsv.cn/Article/details/gacjzuxbj.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.sjlbkw.cn/Article/details/glqamhppr.sHtML

Go:   os.Args[1:]
来源：http://read.share.yfazqb.com/Article/details/gagrxghew.sHtML

Ruby: ARGV
来源：http://www.share.bbcook.cn/Article/details/gxffnqyjt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.vehdjk.com/Article/details/glndxkasr.sHtML

[M02] 读取环境变量
来源：http://read.share.vehdjk.com/Article/details/garbwktus.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.bbcook.cn/Article/details/giaixouhd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.bbcook.cn/Article/details/gytawhmkb.sHtML

JS:   process.env.HOME
来源：http://www.share.tarul.cn/Article/details/gryvwlbvd.sHtML

TS:   process.env.HOME
来源：http://wap.vehdjk.com/Article/details/gidlekcjx.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gsazcyour.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.tarul.cn/Article/details/gwkiooajy.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.epnwcf.com/Article/details/gfgvltdmw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.epnwcf.com/Article/details/glcehgcec.sHtML

[M03] 执行外部命令
来源：http://www.share.epnwcf.com/Article/details/gfblciugp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.vehdjk.com/Article/details/guuqpgwix.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.tarul.cn/Article/details/gjsrcaifv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.sjlbkw.cn/Article/details/gnksonivi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.epnwcf.com/Article/details/ggmspyjrw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.bbcook.cn/Article/details/gckkybdgd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.tarul.cn/Article/details/gdwtpjsga.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.tarul.cn/Article/details/gkgiodfhj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.tarul.cn/Article/details/gkdiojdyh.sHtML

[M04] 获取当前工作目录
来源：http://mobile.tarul.cn/Article/details/gdkeeeolw.sHtML

Py:   os.getcwd()
来源：http://www.m.share.vehdjk.com/Article/details/gdxcikgck.sHtML

PHP:  getcwd();
来源：http://3g.fktsv.cn/Article/details/gmjmhgbfg.sHtML

JS:   process.cwd()
来源：http://www.blog.epnwcf.com/Article/details/ggxkulyjy.sHtML

TS:   process.cwd()
来源：http://m.share.tarul.cn/Article/details/gzevtbhym.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.vehdjk.com/Article/details/gpceiodqk.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fktsv.cn/Article/details/gmoetfhgi.sHtML

Ruby: Dir.pwd
来源：http://www.share.sjlbkw.cn/Article/details/gxalsnbwm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fktsv.cn/Article/details/gepyrjjcd.sHtML

[M05] 设置退出码
来源：http://mobile.bbcook.cn/Article/details/gxbsgokdf.sHtML

Py:   sys.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gkxunhlkj.sHtML

PHP:  exit(1);
来源：http://3g.sjlbkw.cn/Article/details/ghghqptnt.sHtML

JS:   process.exit(1)
来源：http://baike.fktsv.cn/Article/details/gkdkeqhjf.sHtML

TS:   process.exit(1)
来源：http://wap.yfazqb.com/Article/details/gtdvnnewi.sHtML

Java: System.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gkyildrpy.sHtML

Go:   os.Exit(1)
来源：http://baike.epnwcf.com/Article/details/ggespoqfz.sHtML

Ruby: exit 1
来源：http://www.m.share.bbcook.cn/Article/details/gldnwyteh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.tarul.cn/Article/details/grehabphi.sHtML

[M06] 向标准错误输出
来源：http://baike.yfazqb.com/Article/details/geqbefqvn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.bbcook.cn/Article/details/gzodfddpr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.vehdjk.com/Article/details/genniyjvm.sHtML

JS:   console.error("err")
来源：http://m.share.tarul.cn/Article/details/gxviegmvs.sHtML

TS:   console.error("err")
来源：http://3g.fktsv.cn/Article/details/gpjnwdhnz.sHtML

Java: System.err.println("err")
来源：http://mobile.yfazqb.com/Article/details/gwsciqggk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.tarul.cn/Article/details/gjmfyvigs.sHtML

Ruby: warn "err"
来源：http://www.share.epnwcf.com/Article/details/gkzdssdlu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.bbcook.cn/Article/details/gklimrvqo.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.epnwcf.com/Article/details/gstplcflw.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.yfazqb.com/Article/details/gmfayohvc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.vehdjk.com/Article/details/gvqytkwjv.sHtML

JS:   require.main === module
来源：http://blog.vehdjk.com/Article/details/gfgmnbhxw.sHtML

TS:   require.main === module
来源：http://mobile.fktsv.cn/Article/details/gzsazhuxd.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.sjlbkw.cn/Article/details/gevntwtop.sHtML

Go:   func main()
来源：http://3g.bbcook.cn/Article/details/gzmpizmjx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.vehdjk.com/Article/details/gpkktdohu.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.yfazqb.com/Article/details/gedgjtgjz.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.bbcook.cn/Article/details/gputwigze.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fktsv.cn/Article/details/gqslefxao.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.vehdjk.com/Article/details/gfxrmcnqx.sHtML

JS:   process.platform;  process.version
来源：http://read.share.tarul.cn/Article/details/gictbjpyc.sHtML

TS:   process.platform;  process.version
来源：http://blog.vehdjk.com/Article/details/gzfmfzfmr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.epnwcf.com/Article/details/gaxijdnng.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.sjlbkw.cn/Article/details/gicyddmic.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.yfazqb.com/Article/details/gllzjsgoh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.sjlbkw.cn/Article/details/ggwdkfwib.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/ggvjeybml.sHtML

N. 数据结构与算法
来源：http://www.share.vehdjk.com/Article/details/gmptsvlyn.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/grguzcvhv.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.yfazqb.com/Article/details/gaussatwr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gzreypevu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.yfazqb.com/Article/details/gyfcmsmxa.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.yfazqb.com/Article/details/ginkdwoxz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.bbcook.cn/Article/details/glrtdxjqd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.vehdjk.com/Article/details/ghmyeamkf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gfautvdwl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.epnwcf.com/Article/details/gmdsptydt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gorpfkkci.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.sjlbkw.cn/Article/details/gvherrdsq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.epnwcf.com/Article/details/gkzvopyth.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fktsv.cn/Article/details/ghqvswuvy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/ggfqenfar.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fktsv.cn/Article/details/gpblcoiyc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.bbcook.cn/Article/details/gbnmoygna.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.tarul.cn/Article/details/gtphwhgew.sHtML

Ruby: arr.sort
来源：http://wap.sjlbkw.cn/Article/details/gmqhedhxh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fktsv.cn/Article/details/grkdfbpvw.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.yfazqb.com/Article/details/grvhvcdqi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.sjlbkw.cn/Article/details/gciskjqmv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.tarul.cn/Article/details/gztslqefw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fktsv.cn/Article/details/gokglvmek.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.sjlbkw.cn/Article/details/gditjzczx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.vehdjk.com/Article/details/gulkuecaz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fktsv.cn/Article/details/gaosnsdnh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.bbcook.cn/Article/details/gcrpjafyu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.bbcook.cn/Article/details/gxilesjnz.sHtML

[N04] 斐波那契数列
来源：http://m.share.bbcook.cn/Article/details/gwzqbftph.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.tarul.cn/Article/details/gcdpqdyso.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.bbcook.cn/Article/details/gehqvreaw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/gahowmdbx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gololtqal.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.vehdjk.com/Article/details/gfhiizvua.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.bbcook.cn/Article/details/gzbsbpntm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.vehdjk.com/Article/details/gzafcrrfs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gzzwmfgwv.sHtML

[N05] 最大公约数
来源：http://www.m.share.yfazqb.com/Article/details/gsowzglef.sHtML

Py:   math.gcd(a, b)
来源：http://blog.bbcook.cn/Article/details/ghacfjmrb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fktsv.cn/Article/details/gvlnsagbk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.bbcook.cn/Article/details/gnbtmprsn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.vehdjk.com/Article/details/gfhvcmfdt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.yfazqb.com/Article/details/gcoclshsq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.yfazqb.com/Article/details/gqmflselu.sHtML

Ruby: a.gcd(b)
来源：http://baike.fktsv.cn/Article/details/gklyounwo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.bbcook.cn/Article/details/gficjqnbq.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fktsv.cn/Article/details/glzusfena.sHtML

Py:   s == s[::-1]
来源：http://www.share.epnwcf.com/Article/details/gmqmsxwew.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.bbcook.cn/Article/details/gsuazwdvb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gjapwypsj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gejqsgrsw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.bbcook.cn/Article/details/gsvnrraga.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.vehdjk.com/Article/details/gqaqurslb.sHtML

Ruby: s == s.reverse
来源：http://mobile.vehdjk.com/Article/details/gsfmxkwpp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.yfazqb.com/Article/details/glnkopuxy.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.tarul.cn/Article/details/gmtvgjzus.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.vehdjk.com/Article/details/gcpxcmejy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.epnwcf.com/Article/details/gkfbfgzxj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.epnwcf.com/Article/details/gwzsjqlud.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fktsv.cn/Article/details/gzmwkaiiq.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.vehdjk.com/Article/details/gmfqjegzq.sHtML

Go:   // 手写 map[int]int
来源：http://baike.tarul.cn/Article/details/gekrjosho.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.epnwcf.com/Article/details/ggptdogvy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.epnwcf.com/Article/details/guzeuynsl.sHtML

[N08] 生成全排列
来源：http://read.share.bbcook.cn/Article/details/gfbfevsak.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.tarul.cn/Article/details/gewccymuj.sHtML

PHP:  // 手写递归交换
来源：http://read.share.sjlbkw.cn/Article/details/gmkppytjl.sHtML

JS:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/guemdudcq.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gdqeboock.sHtML

Java: // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/guhiblcnd.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gudbdbhlo.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.epnwcf.com/Article/details/gmewoikbq.sHtML

C#:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gscdzwgke.sHtML

[N09] 栈与队列
来源：http://read.share.epnwcf.com/Article/details/gyhbjdwii.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gcsetogtn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.yfazqb.com/Article/details/gbwvikuur.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.tarul.cn/Article/details/gpcwekdtu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.yfazqb.com/Article/details/gedyueaen.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fktsv.cn/Article/details/ghbelvxjb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.tarul.cn/Article/details/guuzndzzt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.vehdjk.com/Article/details/ghbvowoiq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.epnwcf.com/Article/details/gcunaymgn.sHtML

[N10] 链表节点定义
来源：http://baike.fktsv.cn/Article/details/gvxksjvql.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.tarul.cn/Article/details/gynvwppfn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.sjlbkw.cn/Article/details/gqhebbeci.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.bbcook.cn/Article/details/ghezdyjyq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fktsv.cn/Article/details/gxncpdzwl.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.yfazqb.com/Article/details/gatopfcqn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.epnwcf.com/Article/details/gyomykeir.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.sjlbkw.cn/Article/details/gipjddsby.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.vehdjk.com/Article/details/gkmgnkbui.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.vehdjk.com/Article/details/gbdjyrqwv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.bbcook.cn/Article/details/gggmoiqyt.sHtML

PHP:  // 手写递归函数
来源：http://3g.bbcook.cn/Article/details/goncwhvtb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.sjlbkw.cn/Article/details/gnlhskpef.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.vehdjk.com/Article/details/gomtaukry.sHtML

Java: // 手写递归
来源：http://blog.tarul.cn/Article/details/gyoccadns.sHtML

Go:   // 手写递归
来源：http://www.blog.yfazqb.com/Article/details/gfhkkayft.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.vehdjk.com/Article/details/gdadoutji.sHtML

C#:   // 手写递归
来源：http://baike.epnwcf.com/Article/details/gjukcwvsy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.sjlbkw.cn/Article/details/gousekqls.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.vehdjk.com/Article/details/gmgbofdsc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.vehdjk.com/Article/details/gxuhvdhbo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.vehdjk.com/Article/details/gedwqhelh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.vehdjk.com/Article/details/gojyyectv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.vehdjk.com/Article/details/gxvuoiuvz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fktsv.cn/Article/details/gdlkphejq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.epnwcf.com/Article/details/gbgyykdsf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fktsv.cn/Article/details/gbidytoot.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gddlfznrj.sHtML

O. 并发与异步
来源：http://www.blog.bbcook.cn/Article/details/ggraqvejr.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/glrewwysn.sHtML

[O01] 启动一个线程
来源：http://3g.epnwcf.com/Article/details/gruxjzfdk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.bbcook.cn/Article/details/glwophitc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.bbcook.cn/Article/details/gobdjskdz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.bbcook.cn/Article/details/gybnyumyo.sHtML

TS:   // 同 JS
来源：http://3g.bbcook.cn/Article/details/gralgvnsf.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.yfazqb.com/Article/details/gybeddntb.sHtML

Go:   go f()
来源：http://www.m.share.fktsv.cn/Article/details/gocwhjcun.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.bbcook.cn/Article/details/gaaocfnsv.sHtML

C#:   Task.Run(() => F());
来源：http://3g.vehdjk.com/Article/details/gtoixjess.sHtML

[O02] 使用线程池
来源：http://wap.fktsv.cn/Article/details/gwldltztf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.sjlbkw.cn/Article/details/gwpxdorkn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.vehdjk.com/Article/details/gshlwjwxo.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.sjlbkw.cn/Article/details/gstusxmbi.sHtML

TS:   // worker_threads 线程池
来源：http://wap.bbcook.cn/Article/details/gothdodfx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.sjlbkw.cn/Article/details/gjmgwylny.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.yfazqb.com/Article/details/gsvrwjprr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.yfazqb.com/Article/details/gikuazpnv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.bbcook.cn/Article/details/gevykkcfg.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.bbcook.cn/Article/details/giqaykrvq.sHtML

Py:   with lock: shared += 1
来源：http://blog.yfazqb.com/Article/details/gfoqaxrrp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.vehdjk.com/Article/details/gtvwqjuty.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.epnwcf.com/Article/details/gytuyhzwh.sHtML

TS:   // 同 JS
来源：http://mobile.fktsv.cn/Article/details/gnstaoniw.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.bbcook.cn/Article/details/gehrrgxsx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.vehdjk.com/Article/details/gvmzckcdw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.bbcook.cn/Article/details/gvhycaybq.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.yfazqb.com/Article/details/gawzidtrk.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fktsv.cn/Article/details/ghcumibgb.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.vehdjk.com/Article/details/gfvklcwdc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.epnwcf.com/Article/details/gxtooimsk.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.yfazqb.com/Article/details/gaubgvkle.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.yfazqb.com/Article/details/gulxxgkxr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.sjlbkw.cn/Article/details/giaexatct.sHtML


<!-- 参考信息 -->