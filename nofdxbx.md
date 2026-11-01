代发 wailian999

Go:   encoding/gob
来源：http://wap.fktsv.cn/Article/details/gdrrokzng.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.epnwcf.com/Article/details/gauxxtvtv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.tarul.cn/Article/details/ghcvnvjin.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gvfzougbp.sHtML

L. 网络请求
来源：http://read.share.bbcook.cn/Article/details/gdatksaae.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gzwwehbye.sHtML

[L01] 发送 GET 请求
来源：http://3g.epnwcf.com/Article/details/gsxpaqqtb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.sjlbkw.cn/Article/details/gooqqgobm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.vehdjk.com/Article/details/gdqdnulit.sHtML

JS:   await fetch(url)
来源：http://blog.tarul.cn/Article/details/gpnioqwyv.sHtML

TS:   await fetch(url)
来源：http://blog.yfazqb.com/Article/details/gncmrnusy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.tarul.cn/Article/details/gdauxlume.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.epnwcf.com/Article/details/godwshchu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.epnwcf.com/Article/details/ghomknxcm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fktsv.cn/Article/details/goqsmebil.sHtML

[L02] 发送 POST JSON
来源：http://3g.bbcook.cn/Article/details/gxhploccd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.sjlbkw.cn/Article/details/grxyqcjlt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.sjlbkw.cn/Article/details/gdoworbgr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.bbcook.cn/Article/details/gqlyouibq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.vehdjk.com/Article/details/geohoaxep.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.vehdjk.com/Article/details/gjmwoqnzl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.vehdjk.com/Article/details/glqcvknpd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.bbcook.cn/Article/details/gwopjnnms.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.bbcook.cn/Article/details/gsawcmxdv.sHtML

[L03] 设置自定义请求头
来源：http://www.share.yfazqb.com/Article/details/gigvmywkf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.sjlbkw.cn/Article/details/gkbgfympo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fktsv.cn/Article/details/gjzastgmu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.tarul.cn/Article/details/gnbwaeech.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.tarul.cn/Article/details/glugdlorj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.vehdjk.com/Article/details/grnuapngi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.sjlbkw.cn/Article/details/gpomcebft.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.bbcook.cn/Article/details/gszfggbnk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.tarul.cn/Article/details/gkjyjneow.sHtML

[L04] 设置超时
来源：http://wap.vehdjk.com/Article/details/gacrvwmhu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.yfazqb.com/Article/details/gbmgmfxim.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.yfazqb.com/Article/details/gyfecbwwv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fktsv.cn/Article/details/gfncpyojv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fktsv.cn/Article/details/gbkymzbka.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.vehdjk.com/Article/details/gzvzjsndy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.epnwcf.com/Article/details/gxqtyighg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.sjlbkw.cn/Article/details/gvbgoaoxw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.tarul.cn/Article/details/gnvdhlfiz.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fktsv.cn/Article/details/gsrwjlyks.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.tarul.cn/Article/details/gbbmnsymz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.epnwcf.com/Article/details/gtaoxxkso.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.bbcook.cn/Article/details/gfxoacuda.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.sjlbkw.cn/Article/details/ggjyvvgll.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.vehdjk.com/Article/details/gdrdnljrm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.vehdjk.com/Article/details/grngfngoz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.yfazqb.com/Article/details/gqhpujsyg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.yfazqb.com/Article/details/gliidzxpj.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fktsv.cn/Article/details/gsjcnlczw.sHtML

Py:   resp.json()
来源：http://baike.epnwcf.com/Article/details/gnxiybrnf.sHtML

PHP:  json_decode($body, true);
来源：http://baike.vehdjk.com/Article/details/gqzezlack.sHtML

JS:   await resp.json()
来源：http://blog.vehdjk.com/Article/details/gjsjrflye.sHtML

TS:   await resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/ghkuenszr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.yfazqb.com/Article/details/geddwmbnn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.tarul.cn/Article/details/gmtxkqtrf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.tarul.cn/Article/details/gxxkdoaqp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fktsv.cn/Article/details/goxetvgnv.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.bbcook.cn/Article/details/gtkaabzmm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.bbcook.cn/Article/details/gmxnjbznz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.vehdjk.com/Article/details/gizfvttrd.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.epnwcf.com/Article/details/gpnczyrrx.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.epnwcf.com/Article/details/gdomjeedo.sHtML

Java: resp.statusCode()
来源：http://www.m.share.vehdjk.com/Article/details/gkqedipqt.sHtML

Go:   resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/gxnuwieso.sHtML

Ruby: resp.code.to_i
来源：http://baike.sjlbkw.cn/Article/details/ggyitrrhr.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.sjlbkw.cn/Article/details/grvyjfkjy.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.vehdjk.com/Article/details/gmnnymfrm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.bbcook.cn/Article/details/gofdsknug.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.sjlbkw.cn/Article/details/gsvoastap.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gqikrlcpi.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/gvmtaeylz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.bbcook.cn/Article/details/gokupabvf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.sjlbkw.cn/Article/details/glsloiurg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.sjlbkw.cn/Article/details/gsaciydvz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.tarul.cn/Article/details/gvblvrzuo.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gllrsoanl.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.tarul.cn/Article/details/gclawudru.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/glljushrj.sHtML

[M01] 读取命令行参数
来源：http://blog.epnwcf.com/Article/details/gnnapevll.sHtML

Py:   sys.argv[1:]
来源：http://mobile.tarul.cn/Article/details/gvebsdlxl.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.epnwcf.com/Article/details/gcyznhbhd.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.vehdjk.com/Article/details/gbtognxmr.sHtML

TS:   process.argv.slice(2)
来源：http://3g.tarul.cn/Article/details/gqwbfkrqp.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.bbcook.cn/Article/details/ggupucabt.sHtML

Go:   os.Args[1:]
来源：http://mobile.yfazqb.com/Article/details/giypucijq.sHtML

Ruby: ARGV
来源：http://wap.yfazqb.com/Article/details/gaqcaepbd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.yfazqb.com/Article/details/gjfhyysea.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fktsv.cn/Article/details/gylfgjdir.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.yfazqb.com/Article/details/gevqufxol.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.vehdjk.com/Article/details/grzdlxsii.sHtML

JS:   process.env.HOME
来源：http://3g.fktsv.cn/Article/details/gkgivaerb.sHtML

TS:   process.env.HOME
来源：http://3g.fktsv.cn/Article/details/giuswjewl.sHtML

Java: System.getenv("HOME")
来源：http://baike.sjlbkw.cn/Article/details/guphynoxu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.tarul.cn/Article/details/gkcmblpgf.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.yfazqb.com/Article/details/gfymsaroo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/ghehuyvrt.sHtML

[M03] 执行外部命令
来源：http://read.share.yfazqb.com/Article/details/gtnldaaug.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.yfazqb.com/Article/details/gevvxukbc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.tarul.cn/Article/details/ghqfwbddw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fktsv.cn/Article/details/gyxktciet.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.vehdjk.com/Article/details/gaisxkzry.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.bbcook.cn/Article/details/gllzttvrp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.sjlbkw.cn/Article/details/gyifwiibx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.vehdjk.com/Article/details/gwvsapdjm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.yfazqb.com/Article/details/gqayumjey.sHtML

[M04] 获取当前工作目录
来源：http://blog.sjlbkw.cn/Article/details/gduvqgckj.sHtML

Py:   os.getcwd()
来源：http://blog.sjlbkw.cn/Article/details/gewuyymht.sHtML

PHP:  getcwd();
来源：http://read.share.yfazqb.com/Article/details/gouhtaxye.sHtML

JS:   process.cwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gftmyehnz.sHtML

TS:   process.cwd()
来源：http://3g.epnwcf.com/Article/details/grrwbsxve.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.tarul.cn/Article/details/gebymkxxj.sHtML

Go:   os.Getwd()
来源：http://3g.bbcook.cn/Article/details/gggmqmhbi.sHtML

Ruby: Dir.pwd
来源：http://www.share.vehdjk.com/Article/details/gpcvipqpo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.bbcook.cn/Article/details/gbukwsnlv.sHtML

[M05] 设置退出码
来源：http://3g.fktsv.cn/Article/details/gtpeqbomp.sHtML

Py:   sys.exit(1)
来源：http://wap.tarul.cn/Article/details/gnzumeegq.sHtML

PHP:  exit(1);
来源：http://3g.yfazqb.com/Article/details/gwfmhwgng.sHtML

JS:   process.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gjrkldois.sHtML

TS:   process.exit(1)
来源：http://blog.yfazqb.com/Article/details/gfbggjuhk.sHtML

Java: System.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gjrwmambj.sHtML

Go:   os.Exit(1)
来源：http://wap.fktsv.cn/Article/details/gemsvvtnt.sHtML

Ruby: exit 1
来源：http://3g.sjlbkw.cn/Article/details/gyiprjiqn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.sjlbkw.cn/Article/details/gemgreftj.sHtML

[M06] 向标准错误输出
来源：http://www.blog.tarul.cn/Article/details/gbpqmatwn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.vehdjk.com/Article/details/gkjiittke.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.tarul.cn/Article/details/gkkkkrxia.sHtML

JS:   console.error("err")
来源：http://3g.fktsv.cn/Article/details/glmngxsil.sHtML

TS:   console.error("err")
来源：http://wap.tarul.cn/Article/details/ggvyuwjcm.sHtML

Java: System.err.println("err")
来源：http://baike.bbcook.cn/Article/details/gqgzgdxnr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.yfazqb.com/Article/details/guyersaxo.sHtML

Ruby: warn "err"
来源：http://www.m.share.vehdjk.com/Article/details/gowdfttbv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.yfazqb.com/Article/details/gowvplcrj.sHtML

[M07] 判断是否为主入口
来源：http://read.share.bbcook.cn/Article/details/guwcrgsku.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.epnwcf.com/Article/details/gczmcmuwo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.sjlbkw.cn/Article/details/gmtllyzji.sHtML

JS:   require.main === module
来源：http://3g.tarul.cn/Article/details/ghddresds.sHtML

TS:   require.main === module
来源：http://www.m.share.yfazqb.com/Article/details/gqdsprhyc.sHtML

Java: public static void main(String[] args)
来源：http://m.share.epnwcf.com/Article/details/gzlyjlnaz.sHtML

Go:   func main()
来源：http://read.share.bbcook.cn/Article/details/gqzmtawfk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.yfazqb.com/Article/details/gwlcstnjz.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fktsv.cn/Article/details/gxotszptn.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.yfazqb.com/Article/details/getvghsid.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.tarul.cn/Article/details/ginbsnrkh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.tarul.cn/Article/details/gxjztfdsh.sHtML

JS:   process.platform;  process.version
来源：http://www.share.tarul.cn/Article/details/gmbzbrqkt.sHtML

TS:   process.platform;  process.version
来源：http://mobile.epnwcf.com/Article/details/glqjmtnvx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.sjlbkw.cn/Article/details/ghqvlapyj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.sjlbkw.cn/Article/details/giqacyydu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.vehdjk.com/Article/details/gblqnczoa.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.bbcook.cn/Article/details/geanpsfgw.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gimyfomym.sHtML

N. 数据结构与算法
来源：http://read.share.sjlbkw.cn/Article/details/gyocvfhop.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/glsrrsigf.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.sjlbkw.cn/Article/details/gofqpmasm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/glvoyunvm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.tarul.cn/Article/details/gfhuflyky.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fktsv.cn/Article/details/gprjfqiev.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.yfazqb.com/Article/details/gtnxlutkr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.vehdjk.com/Article/details/gtuiattpg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fktsv.cn/Article/details/gqflbzdqp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.bbcook.cn/Article/details/gagdjevxk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gebbvgmwb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.yfazqb.com/Article/details/gqiqjyegk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fktsv.cn/Article/details/gvhitpmgd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.yfazqb.com/Article/details/gskykwffk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.yfazqb.com/Article/details/gdufxvklm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/goxvaxppf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.bbcook.cn/Article/details/grgbdttkt.sHtML

Go:   slices.Sort(arr)
来源：http://wap.yfazqb.com/Article/details/ggouuqqli.sHtML

Ruby: arr.sort
来源：http://baike.fktsv.cn/Article/details/grutmyfel.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.tarul.cn/Article/details/gudreyyqe.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.epnwcf.com/Article/details/ggpmaecht.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.yfazqb.com/Article/details/gzkcnwyut.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.sjlbkw.cn/Article/details/gpabzweta.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.yfazqb.com/Article/details/gtrgmajel.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.epnwcf.com/Article/details/guzkkllqv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.sjlbkw.cn/Article/details/gtnjspazk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.tarul.cn/Article/details/gedurhbli.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.vehdjk.com/Article/details/ggcymdoco.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.vehdjk.com/Article/details/gydkgblap.sHtML

[N04] 斐波那契数列
来源：http://baike.epnwcf.com/Article/details/glnhkusba.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.yfazqb.com/Article/details/ggrmbxkvg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fktsv.cn/Article/details/gykpgvmyi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.epnwcf.com/Article/details/gerslxcyt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/gujxbowbr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.tarul.cn/Article/details/ggeyzpklm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.tarul.cn/Article/details/gfvyuiagn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fktsv.cn/Article/details/guqqvylao.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/gjmwjggcg.sHtML

[N05] 最大公约数
来源：http://www.blog.vehdjk.com/Article/details/gplwrdjyp.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.epnwcf.com/Article/details/gehegweto.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.epnwcf.com/Article/details/gtdnqompy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.vehdjk.com/Article/details/gpcvsidpl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.sjlbkw.cn/Article/details/gwihfczvr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.bbcook.cn/Article/details/gflchzkwi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fktsv.cn/Article/details/ghxdcvfvl.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fktsv.cn/Article/details/gvopxtymg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.tarul.cn/Article/details/gqnzqhyob.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.bbcook.cn/Article/details/gygwxntay.sHtML

Py:   s == s[::-1]
来源：http://www.blog.sjlbkw.cn/Article/details/gtoopxguz.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fktsv.cn/Article/details/gtukmlqcn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/gpmyvnjzn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gqbdpmywu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.sjlbkw.cn/Article/details/gshlugjhr.sHtML

Go:   // 双指针从两端比较
来源：http://blog.epnwcf.com/Article/details/gzlygfdoq.sHtML

Ruby: s == s.reverse
来源：http://3g.sjlbkw.cn/Article/details/gwqotgafd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.bbcook.cn/Article/details/gqyjhiiyt.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.epnwcf.com/Article/details/gdgiwsqgb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.sjlbkw.cn/Article/details/gezsekqbg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.sjlbkw.cn/Article/details/guzygkbzr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.bbcook.cn/Article/details/grivpdzwz.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.bbcook.cn/Article/details/gqhysfacx.sHtML

Java: // 手写 HashMap
来源：http://www.share.yfazqb.com/Article/details/gsrevtnwu.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.yfazqb.com/Article/details/gskhojraj.sHtML

Ruby: // 手写 Hash
来源：http://3g.vehdjk.com/Article/details/gbxiwlfgn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.epnwcf.com/Article/details/gvasjylqd.sHtML

[N08] 生成全排列
来源：http://blog.tarul.cn/Article/details/gdswgxlxd.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fktsv.cn/Article/details/gwdnjdjlb.sHtML

PHP:  // 手写递归交换
来源：http://baike.fktsv.cn/Article/details/grrfrdjrz.sHtML

JS:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/gnivstwjy.sHtML

TS:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/grdlzxuen.sHtML

Java: // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/glyfhnygy.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/ghpflhkwe.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.sjlbkw.cn/Article/details/gyrdpravq.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gqqtezryy.sHtML

[N09] 栈与队列
来源：http://3g.vehdjk.com/Article/details/gubmhbgpf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.sjlbkw.cn/Article/details/gbkdpvpzk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.epnwcf.com/Article/details/gwwzppasr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.bbcook.cn/Article/details/gaapolmpa.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.tarul.cn/Article/details/ghxdqpvcc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.yfazqb.com/Article/details/groarwevo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.sjlbkw.cn/Article/details/gpsabwrgk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.bbcook.cn/Article/details/gyrzmyisb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.bbcook.cn/Article/details/geifemgci.sHtML

[N10] 链表节点定义
来源：http://www.share.sjlbkw.cn/Article/details/ghmhqazou.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.sjlbkw.cn/Article/details/gytdvaqew.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhaiqmlg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.epnwcf.com/Article/details/gwmjyzubx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fktsv.cn/Article/details/gbnxqqykc.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.tarul.cn/Article/details/gsoraxdlz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.tarul.cn/Article/details/gwhmjsxwy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fktsv.cn/Article/details/gidnwmyhs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.sjlbkw.cn/Article/details/gbkpoqsad.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.epnwcf.com/Article/details/grxibuymg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.vehdjk.com/Article/details/gkqbujdqh.sHtML

PHP:  // 手写递归函数
来源：http://m.share.yfazqb.com/Article/details/glvjjcepz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.epnwcf.com/Article/details/guqxbuqud.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fktsv.cn/Article/details/gqxdigxie.sHtML

Java: // 手写递归
来源：http://mobile.yfazqb.com/Article/details/gusgybxcy.sHtML

Go:   // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/gafmutkls.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.yfazqb.com/Article/details/gmpqkdsvi.sHtML

C#:   // 手写递归
来源：http://wap.bbcook.cn/Article/details/gmcjbecnt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fktsv.cn/Article/details/gdfnmndkl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.tarul.cn/Article/details/gbvgjddxq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.sjlbkw.cn/Article/details/gmmcmonfy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.bbcook.cn/Article/details/gxyfzjcsa.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.tarul.cn/Article/details/gnkmqfngw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.yfazqb.com/Article/details/gvicsxwgz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.epnwcf.com/Article/details/gwmikoass.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.yfazqb.com/Article/details/gcekcvhcs.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.vehdjk.com/Article/details/gghcvvnxy.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gunpiugak.sHtML

O. 并发与异步
来源：http://www.share.yfazqb.com/Article/details/gclbewidq.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gsoehwqad.sHtML

[O01] 启动一个线程
来源：http://read.share.bbcook.cn/Article/details/gjrmhzsek.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.tarul.cn/Article/details/gfoqnitji.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.yfazqb.com/Article/details/gbolqesig.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.sjlbkw.cn/Article/details/gjxlxqcyt.sHtML

TS:   // 同 JS
来源：http://3g.yfazqb.com/Article/details/gsxnqpvmt.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fktsv.cn/Article/details/gdfvsdieb.sHtML

Go:   go f()
来源：http://www.blog.vehdjk.com/Article/details/gtesnrkpi.sHtML

Ruby: Thread.new { f }
来源：http://mobile.vehdjk.com/Article/details/gbzsbbjqj.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.sjlbkw.cn/Article/details/gozhnwkxl.sHtML

[O02] 使用线程池
来源：http://m.share.fktsv.cn/Article/details/gicazopor.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.yfazqb.com/Article/details/gchogttwk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.yfazqb.com/Article/details/gpwzjunzv.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.yfazqb.com/Article/details/grtawnhjc.sHtML

TS:   // worker_threads 线程池
来源：http://3g.vehdjk.com/Article/details/gzjynwzvr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.epnwcf.com/Article/details/gdncbhxbi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.epnwcf.com/Article/details/gclvtdemm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.vehdjk.com/Article/details/gkwgpfwra.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.tarul.cn/Article/details/gjebzkvft.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.bbcook.cn/Article/details/gwnmpivxa.sHtML

Py:   with lock: shared += 1
来源：http://www.share.tarul.cn/Article/details/gntluazrr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.sjlbkw.cn/Article/details/gsfwxlybc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.sjlbkw.cn/Article/details/geioaxofl.sHtML

TS:   // 同 JS
来源：http://baike.bbcook.cn/Article/details/gxhxnwwgf.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.bbcook.cn/Article/details/gzsiweylq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.epnwcf.com/Article/details/gxzmxjwaz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.epnwcf.com/Article/details/gocllondw.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.vehdjk.com/Article/details/gcsicpfzn.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.sjlbkw.cn/Article/details/gimblqvbk.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fktsv.cn/Article/details/gjwzvrizb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.epnwcf.com/Article/details/gcxiidsin.sHtML

JS:   async function f() { await g(); }
来源：http://blog.sjlbkw.cn/Article/details/gfjlifqfd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.tarul.cn/Article/details/gywciypsp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.tarul.cn/Article/details/gvpbdhpwg.sHtML


<!-- 参考信息 -->