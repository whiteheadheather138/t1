代发 wailian999

Go:   encoding/gob
来源：http://www.m.share.tarul.cn/Article/details/glrylxfmi.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.vehdjk.com/Article/details/gaidsdcic.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.bbcook.cn/Article/details/gztqvfwpq.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gzakwbxtr.sHtML

L. 网络请求
来源：http://mobile.yfazqb.com/Article/details/glbwqdosi.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gqdjwnpve.sHtML

[L01] 发送 GET 请求
来源：http://wap.vehdjk.com/Article/details/gsfsuggcg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.sjlbkw.cn/Article/details/gjsluqfli.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.bbcook.cn/Article/details/gpozfgfxj.sHtML

JS:   await fetch(url)
来源：http://blog.epnwcf.com/Article/details/gztuiiesf.sHtML

TS:   await fetch(url)
来源：http://www.share.vehdjk.com/Article/details/gdjjoeuxg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.bbcook.cn/Article/details/gipledjye.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxfewadt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.epnwcf.com/Article/details/gywdupdip.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.tarul.cn/Article/details/gwapcgrob.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.tarul.cn/Article/details/gdiykompa.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.bbcook.cn/Article/details/gfhdswfqf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.tarul.cn/Article/details/goigvyumg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fktsv.cn/Article/details/gyxfszhyp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fktsv.cn/Article/details/ghizrzcfu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.sjlbkw.cn/Article/details/goddgdpml.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.epnwcf.com/Article/details/gwxyxpnyy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.vehdjk.com/Article/details/gwyfmntjn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fktsv.cn/Article/details/ghbjhhatm.sHtML

[L03] 设置自定义请求头
来源：http://3g.sjlbkw.cn/Article/details/gyfvrknxa.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.vehdjk.com/Article/details/giykxsxep.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.bbcook.cn/Article/details/gxdtoomyr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/gwxmoffnz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.vehdjk.com/Article/details/gdadqruxa.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.yfazqb.com/Article/details/ganmnqbuk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.bbcook.cn/Article/details/gkewtuycp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.bbcook.cn/Article/details/gowbtqyxc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.epnwcf.com/Article/details/ghvavwvhr.sHtML

[L04] 设置超时
来源：http://blog.fktsv.cn/Article/details/gebvmwvhr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.tarul.cn/Article/details/giqbkghuc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fktsv.cn/Article/details/gjmwrtriq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.bbcook.cn/Article/details/guzhxsbql.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.yfazqb.com/Article/details/grxhwerxq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.tarul.cn/Article/details/gsxheqmxp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.vehdjk.com/Article/details/gereotthe.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.epnwcf.com/Article/details/gyplxkxrp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.tarul.cn/Article/details/gicooptfe.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.bbcook.cn/Article/details/gcpcqhfrz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.tarul.cn/Article/details/gleylkjhs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.epnwcf.com/Article/details/gdehmgotj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.tarul.cn/Article/details/gbbgmsyhr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.vehdjk.com/Article/details/gtflwgkuj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.vehdjk.com/Article/details/guwijpzdv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.epnwcf.com/Article/details/gubjiofsq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.bbcook.cn/Article/details/gduersyoh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gixcjygzg.sHtML

[L06] 解析响应为 JSON
来源：http://3g.epnwcf.com/Article/details/ggpmqnmvo.sHtML

Py:   resp.json()
来源：http://www.share.tarul.cn/Article/details/gxfuxtshp.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fktsv.cn/Article/details/gqufhfkcb.sHtML

JS:   await resp.json()
来源：http://m.share.yfazqb.com/Article/details/gnxdxdpzl.sHtML

TS:   await resp.json()
来源：http://baike.sjlbkw.cn/Article/details/gonfogltj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.tarul.cn/Article/details/gbmicwwyd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fktsv.cn/Article/details/gyfabxlki.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.epnwcf.com/Article/details/gnkywksou.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.vehdjk.com/Article/details/geikcffyg.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.epnwcf.com/Article/details/gvrdqpuuh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.tarul.cn/Article/details/gonzrmzcw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.epnwcf.com/Article/details/ghnfvhaem.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.yfazqb.com/Article/details/gornwuclq.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.yfazqb.com/Article/details/gfgdmhijr.sHtML

Java: resp.statusCode()
来源：http://read.share.yfazqb.com/Article/details/gehowxtef.sHtML

Go:   resp.StatusCode
来源：http://www.blog.sjlbkw.cn/Article/details/gikvkzarr.sHtML

Ruby: resp.code.to_i
来源：http://www.share.bbcook.cn/Article/details/gffpsycjp.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.bbcook.cn/Article/details/gftovmxrz.sHtML

[L08] 并发请求多个地址
来源：http://m.share.tarul.cn/Article/details/glfnblubt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.sjlbkw.cn/Article/details/gbojrofiy.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fktsv.cn/Article/details/gsdzijqnt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.vehdjk.com/Article/details/gzhocgjzh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.yfazqb.com/Article/details/gulubjnqy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.yfazqb.com/Article/details/gyfblbcgz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.tarul.cn/Article/details/gmsjrtszi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.sjlbkw.cn/Article/details/ggooujmpv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gliheviof.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gtqslpewg.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.tarul.cn/Article/details/gmspwubsi.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gwmiklyml.sHtML

[M01] 读取命令行参数
来源：http://baike.yfazqb.com/Article/details/gmledrvix.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.yfazqb.com/Article/details/gwtukyczo.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.epnwcf.com/Article/details/gqsmoppyx.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.epnwcf.com/Article/details/gsfzjrfqu.sHtML

TS:   process.argv.slice(2)
来源：http://wap.tarul.cn/Article/details/ggumjwtjp.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fktsv.cn/Article/details/gxtcqxetu.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.epnwcf.com/Article/details/gjmpcetjv.sHtML

Ruby: ARGV
来源：http://www.share.fktsv.cn/Article/details/gnunxisgv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.yfazqb.com/Article/details/gseuwupsb.sHtML

[M02] 读取环境变量
来源：http://www.share.sjlbkw.cn/Article/details/gffctxloj.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fktsv.cn/Article/details/grvdmsogz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.sjlbkw.cn/Article/details/gzmfdtsnl.sHtML

JS:   process.env.HOME
来源：http://3g.bbcook.cn/Article/details/gcjpdqfzh.sHtML

TS:   process.env.HOME
来源：http://blog.vehdjk.com/Article/details/gqhwlnoqz.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fktsv.cn/Article/details/gatbqzdsa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.tarul.cn/Article/details/gsfqkgfii.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.tarul.cn/Article/details/gzinxanin.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/gdyziyvzi.sHtML

[M03] 执行外部命令
来源：http://3g.tarul.cn/Article/details/gjpizmago.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.vehdjk.com/Article/details/gwoeoircx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fktsv.cn/Article/details/gvygshwok.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.bbcook.cn/Article/details/gdqovsxuk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.yfazqb.com/Article/details/gwuyellja.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.tarul.cn/Article/details/gfyiwukrm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fktsv.cn/Article/details/gfaibhjrp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.sjlbkw.cn/Article/details/gqthqrntk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.bbcook.cn/Article/details/gmxijrnmo.sHtML

[M04] 获取当前工作目录
来源：http://3g.sjlbkw.cn/Article/details/glijxgfcq.sHtML

Py:   os.getcwd()
来源：http://baike.tarul.cn/Article/details/gwixudkiu.sHtML

PHP:  getcwd();
来源：http://mobile.tarul.cn/Article/details/gzrzoovli.sHtML

JS:   process.cwd()
来源：http://mobile.sjlbkw.cn/Article/details/gxbwjyclk.sHtML

TS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/gefntpwfz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fktsv.cn/Article/details/gmtudnkmt.sHtML

Go:   os.Getwd()
来源：http://read.share.epnwcf.com/Article/details/ghvbggdqy.sHtML

Ruby: Dir.pwd
来源：http://3g.sjlbkw.cn/Article/details/garcnvzds.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.tarul.cn/Article/details/ggpzqzcnb.sHtML

[M05] 设置退出码
来源：http://wap.vehdjk.com/Article/details/ghvqpsbge.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gwrvcaedt.sHtML

PHP:  exit(1);
来源：http://baike.vehdjk.com/Article/details/giysteewk.sHtML

JS:   process.exit(1)
来源：http://3g.vehdjk.com/Article/details/gscdduxzt.sHtML

TS:   process.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gkzxwdisl.sHtML

Java: System.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/ghieqefyp.sHtML

Go:   os.Exit(1)
来源：http://m.share.vehdjk.com/Article/details/geccddwuq.sHtML

Ruby: exit 1
来源：http://wap.fktsv.cn/Article/details/gzojbbrav.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.yfazqb.com/Article/details/gcpcvcbkw.sHtML

[M06] 向标准错误输出
来源：http://baike.tarul.cn/Article/details/ghmcwotxc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fktsv.cn/Article/details/gysstxndg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.epnwcf.com/Article/details/guxqoqody.sHtML

JS:   console.error("err")
来源：http://baike.tarul.cn/Article/details/gxdchwydd.sHtML

TS:   console.error("err")
来源：http://read.share.tarul.cn/Article/details/gsgikjmhy.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fktsv.cn/Article/details/gxggbzpcu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.sjlbkw.cn/Article/details/gmeevggsj.sHtML

Ruby: warn "err"
来源：http://read.share.vehdjk.com/Article/details/gtjqqlcfp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.yfazqb.com/Article/details/gaftenvxu.sHtML

[M07] 判断是否为主入口
来源：http://mobile.epnwcf.com/Article/details/ggyyknmso.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.tarul.cn/Article/details/gthiukfyc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.epnwcf.com/Article/details/gtclwuhpo.sHtML

JS:   require.main === module
来源：http://www.share.fktsv.cn/Article/details/gaemjrjje.sHtML

TS:   require.main === module
来源：http://mobile.yfazqb.com/Article/details/gqbvrrwcy.sHtML

Java: public static void main(String[] args)
来源：http://www.share.yfazqb.com/Article/details/gttnspgvq.sHtML

Go:   func main()
来源：http://www.m.share.fktsv.cn/Article/details/gwkvwqajn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.sjlbkw.cn/Article/details/gwpebfubw.sHtML

C#:   static void Main(string[] args)
来源：http://wap.epnwcf.com/Article/details/grbadlxcw.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.vehdjk.com/Article/details/grvkxgvdx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.sjlbkw.cn/Article/details/gyrrmzvsb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fktsv.cn/Article/details/guhkqvmtz.sHtML

JS:   process.platform;  process.version
来源：http://3g.sjlbkw.cn/Article/details/ghwzuqbgt.sHtML

TS:   process.platform;  process.version
来源：http://read.share.sjlbkw.cn/Article/details/gjonkwauy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.epnwcf.com/Article/details/gwzzzyqxo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.epnwcf.com/Article/details/gakydzhjs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.sjlbkw.cn/Article/details/gshtysjeb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.yfazqb.com/Article/details/gpsfkrvrp.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gfordehug.sHtML

N. 数据结构与算法
来源：http://read.share.bbcook.cn/Article/details/gjazjdcti.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/grcvabbad.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.epnwcf.com/Article/details/grhilttal.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.tarul.cn/Article/details/gcizhdzig.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.tarul.cn/Article/details/gergwjdbu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/gkzjebkcy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.epnwcf.com/Article/details/gusnadirt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.bbcook.cn/Article/details/gbvhplhqo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.epnwcf.com/Article/details/gvamulzpu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.epnwcf.com/Article/details/gigvseisz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gfdkowklg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.sjlbkw.cn/Article/details/gftjelihh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.tarul.cn/Article/details/gascizjvp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.sjlbkw.cn/Article/details/grcexbylz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fktsv.cn/Article/details/goaicofbx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/gmuqovtkh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.yfazqb.com/Article/details/gdbsauuly.sHtML

Go:   slices.Sort(arr)
来源：http://blog.bbcook.cn/Article/details/ghjxqkrnw.sHtML

Ruby: arr.sort
来源：http://m.share.vehdjk.com/Article/details/gfwofswfy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.vehdjk.com/Article/details/gjwwjdhfd.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.tarul.cn/Article/details/gvlxykkfy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.yfazqb.com/Article/details/gdrtcghvr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.vehdjk.com/Article/details/glbxpmwzt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.yfazqb.com/Article/details/gxbrhpaff.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.tarul.cn/Article/details/gqjqdiwbp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.epnwcf.com/Article/details/guksydssk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.sjlbkw.cn/Article/details/gfoenkkmn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fktsv.cn/Article/details/glnyofunf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.epnwcf.com/Article/details/gwbrkdjwb.sHtML

[N04] 斐波那契数列
来源：http://blog.yfazqb.com/Article/details/gxewrzbif.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.bbcook.cn/Article/details/gpucfmmcb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fktsv.cn/Article/details/gbkpwdlaw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fktsv.cn/Article/details/gifzckzsk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/goekqduir.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.epnwcf.com/Article/details/gbzuyqnmc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.sjlbkw.cn/Article/details/gzsimwxio.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fktsv.cn/Article/details/gninvxjwq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.tarul.cn/Article/details/ghsyeihak.sHtML

[N05] 最大公约数
来源：http://3g.epnwcf.com/Article/details/ghvshgfss.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fktsv.cn/Article/details/gcxzylypw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fktsv.cn/Article/details/gvzhjliva.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fktsv.cn/Article/details/gudychmzc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.sjlbkw.cn/Article/details/gevuotsgj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.vehdjk.com/Article/details/grbpyctxg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.tarul.cn/Article/details/ghnphduez.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.sjlbkw.cn/Article/details/gbjmyzgss.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.epnwcf.com/Article/details/gqserrqjt.sHtML

[N06] 判断回文字符串
来源：http://www.share.yfazqb.com/Article/details/glljtbamm.sHtML

Py:   s == s[::-1]
来源：http://www.share.sjlbkw.cn/Article/details/gnlljrbiu.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.vehdjk.com/Article/details/gfngnotsn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gyfnvoghi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gfazndzri.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.epnwcf.com/Article/details/gwwgdnrvk.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.bbcook.cn/Article/details/gzjxkiedo.sHtML

Ruby: s == s.reverse
来源：http://wap.bbcook.cn/Article/details/guhoncskf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.vehdjk.com/Article/details/gqplklbdw.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.sjlbkw.cn/Article/details/gkvouzmsv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.sjlbkw.cn/Article/details/ghvgaffeo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.tarul.cn/Article/details/ghnblsvpm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.vehdjk.com/Article/details/gzitafuot.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.bbcook.cn/Article/details/gvzspnxgi.sHtML

Java: // 手写 HashMap
来源：http://3g.sjlbkw.cn/Article/details/gmgyybktn.sHtML

Go:   // 手写 map[int]int
来源：http://baike.epnwcf.com/Article/details/gjzqhxcxa.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvjqyycx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fktsv.cn/Article/details/ggoomaykq.sHtML

[N08] 生成全排列
来源：http://mobile.tarul.cn/Article/details/gchsjufpa.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.sjlbkw.cn/Article/details/gfwmspsgi.sHtML

PHP:  // 手写递归交换
来源：http://3g.fktsv.cn/Article/details/gpnfqpjki.sHtML

JS:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gvcoybcob.sHtML

TS:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gwpvleonk.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/ghwontsnd.sHtML

Go:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/gdbkzkhcb.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.epnwcf.com/Article/details/guhzuzvok.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gwbggndhr.sHtML

[N09] 栈与队列
来源：http://www.blog.bbcook.cn/Article/details/gafzluvky.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.yfazqb.com/Article/details/gehvopqvl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.tarul.cn/Article/details/gtddjdpqg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.vehdjk.com/Article/details/gxbwzmjuz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.vehdjk.com/Article/details/gkvwzliug.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.tarul.cn/Article/details/gcekrluza.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.vehdjk.com/Article/details/gjcmtpyim.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.tarul.cn/Article/details/gucdxuaox.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.bbcook.cn/Article/details/gyvwllxgj.sHtML

[N10] 链表节点定义
来源：http://m.share.vehdjk.com/Article/details/gntriklis.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.sjlbkw.cn/Article/details/getbpfrrg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.tarul.cn/Article/details/gvqulgytz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.bbcook.cn/Article/details/gfvuagcaz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.bbcook.cn/Article/details/gkgvjdpun.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.sjlbkw.cn/Article/details/glvwvvokw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.vehdjk.com/Article/details/gmeyuhdhx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvthyqrjw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.vehdjk.com/Article/details/gtxhgsoox.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.tarul.cn/Article/details/guhtfqivf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.vehdjk.com/Article/details/gyykyvjwm.sHtML

PHP:  // 手写递归函数
来源：http://baike.tarul.cn/Article/details/giinovbqp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.vehdjk.com/Article/details/glpsldqxm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.yfazqb.com/Article/details/guegmsfyr.sHtML

Java: // 手写递归
来源：http://m.share.fktsv.cn/Article/details/gdksfzizm.sHtML

Go:   // 手写递归
来源：http://3g.vehdjk.com/Article/details/gmmvnlcar.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.sjlbkw.cn/Article/details/gpfjnfmnb.sHtML

C#:   // 手写递归
来源：http://www.share.tarul.cn/Article/details/grwsbrfqm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.epnwcf.com/Article/details/gouokvmob.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.vehdjk.com/Article/details/gvkuqwype.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fktsv.cn/Article/details/gqkalebid.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.epnwcf.com/Article/details/gafjjmiug.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.yfazqb.com/Article/details/ggxoswdch.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.bbcook.cn/Article/details/gxihzqhmn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fktsv.cn/Article/details/gprhtqdpp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fktsv.cn/Article/details/gfolnbphd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.sjlbkw.cn/Article/details/gjcwditpe.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gxogxkuxk.sHtML

O. 并发与异步
来源：http://3g.yfazqb.com/Article/details/gsybqzcmm.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gysbzvjsi.sHtML

[O01] 启动一个线程
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtoboomr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fktsv.cn/Article/details/gnueocbxs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.tarul.cn/Article/details/gnjdyhwia.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.yfazqb.com/Article/details/gvfhaifcw.sHtML

TS:   // 同 JS
来源：http://mobile.sjlbkw.cn/Article/details/gxsptitkd.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.sjlbkw.cn/Article/details/gfilamvxu.sHtML

Go:   go f()
来源：http://3g.epnwcf.com/Article/details/ghjkuwivt.sHtML

Ruby: Thread.new { f }
来源：http://m.share.bbcook.cn/Article/details/gzqlqcpsl.sHtML

C#:   Task.Run(() => F());
来源：http://wap.yfazqb.com/Article/details/gwlnhzfcu.sHtML

[O02] 使用线程池
来源：http://read.share.yfazqb.com/Article/details/gpxstzdcm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.yfazqb.com/Article/details/gzmzoifyn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.epnwcf.com/Article/details/gozaomcvn.sHtML

JS:   // worker_threads 线程池
来源：http://wap.sjlbkw.cn/Article/details/ggljnmjqt.sHtML

TS:   // worker_threads 线程池
来源：http://blog.yfazqb.com/Article/details/giplcegkk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.vehdjk.com/Article/details/gigmfanym.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.sjlbkw.cn/Article/details/gjukqcfmb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.sjlbkw.cn/Article/details/gcjskahdj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.vehdjk.com/Article/details/gbqbueydt.sHtML

[O03] 加锁保护共享数据
来源：http://3g.yfazqb.com/Article/details/gudiomgly.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.bbcook.cn/Article/details/ghnjmaylk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fktsv.cn/Article/details/ggdrirjbo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.epnwcf.com/Article/details/gekxlvbdq.sHtML

TS:   // 同 JS
来源：http://www.m.share.fktsv.cn/Article/details/gzaxvoxbn.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.bbcook.cn/Article/details/gkrblguav.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fktsv.cn/Article/details/gwcrvoske.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.bbcook.cn/Article/details/gcjjlnzie.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fktsv.cn/Article/details/gmilsityj.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fktsv.cn/Article/details/ggivcdduv.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.bbcook.cn/Article/details/goaavlllx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.sjlbkw.cn/Article/details/gmcloqzdx.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.tarul.cn/Article/details/gykllimcc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.vehdjk.com/Article/details/gqzigtmuc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fktsv.cn/Article/details/gblqodemq.sHtML


<!-- 参考信息 -->