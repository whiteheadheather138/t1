代发 wailian999

Go:   encoding/gob
来源：http://www.m.share.vehdjk.com/Article/details/gxaoltozu.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.yfazqb.com/Article/details/gepvoummm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.tarul.cn/Article/details/gkxqwepch.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gmemxjayq.sHtML

L. 网络请求
来源：http://3g.sjlbkw.cn/Article/details/gdlvdzshm.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfbpnzon.sHtML

[L01] 发送 GET 请求
来源：http://mobile.yfazqb.com/Article/details/gkfzsbxtf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.sjlbkw.cn/Article/details/gyswtbhal.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.epnwcf.com/Article/details/gkarqfahl.sHtML

JS:   await fetch(url)
来源：http://3g.sjlbkw.cn/Article/details/gpdobgcti.sHtML

TS:   await fetch(url)
来源：http://wap.bbcook.cn/Article/details/gqbrpuwhg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.tarul.cn/Article/details/gftfybzkf.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.yfazqb.com/Article/details/gunszjpit.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.yfazqb.com/Article/details/gvvbcerps.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fktsv.cn/Article/details/gtriapdmn.sHtML

[L02] 发送 POST JSON
来源：http://www.share.tarul.cn/Article/details/gmybpnexz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fktsv.cn/Article/details/gnaticcry.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.yfazqb.com/Article/details/gznccuiue.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.bbcook.cn/Article/details/ghyncfyii.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.sjlbkw.cn/Article/details/gacdybhug.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.sjlbkw.cn/Article/details/guiibdzri.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fktsv.cn/Article/details/gaoebwwgy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.yfazqb.com/Article/details/gpebspuop.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.yfazqb.com/Article/details/gohlckelj.sHtML

[L03] 设置自定义请求头
来源：http://3g.sjlbkw.cn/Article/details/gcfrzuotj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.sjlbkw.cn/Article/details/gukfqfmmb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.yfazqb.com/Article/details/gpfimlwsz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.sjlbkw.cn/Article/details/grriqvskc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.sjlbkw.cn/Article/details/godaixjjy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.epnwcf.com/Article/details/gpfxzpnzx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.tarul.cn/Article/details/gflxeiavn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.vehdjk.com/Article/details/gwoxzkqte.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.sjlbkw.cn/Article/details/gltksiwzw.sHtML

[L04] 设置超时
来源：http://www.share.bbcook.cn/Article/details/gijhlgced.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.epnwcf.com/Article/details/gnydbatal.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.vehdjk.com/Article/details/gfcmgodjb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.epnwcf.com/Article/details/gribiaqvz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fktsv.cn/Article/details/guofsotnh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.tarul.cn/Article/details/gfykuxipb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.yfazqb.com/Article/details/glmcplbkf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.yfazqb.com/Article/details/goelnxzsi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.vehdjk.com/Article/details/greyjdwin.sHtML

[L05] 上传文件（multipart）
来源：http://baike.yfazqb.com/Article/details/gyorqwhlz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.yfazqb.com/Article/details/giaudzbie.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.yfazqb.com/Article/details/gzxzlddro.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fktsv.cn/Article/details/gghkwyckk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fktsv.cn/Article/details/gcwxcgoch.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.bbcook.cn/Article/details/gadewkfxq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.epnwcf.com/Article/details/gthixqlyz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fktsv.cn/Article/details/gagztplzl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.yfazqb.com/Article/details/gsjhngxjd.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.vehdjk.com/Article/details/gczpvtziz.sHtML

Py:   resp.json()
来源：http://3g.fktsv.cn/Article/details/gitlhzlrz.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.bbcook.cn/Article/details/gpvlycbao.sHtML

JS:   await resp.json()
来源：http://baike.vehdjk.com/Article/details/gsguljecf.sHtML

TS:   await resp.json()
来源：http://baike.vehdjk.com/Article/details/gzvdevpjk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.epnwcf.com/Article/details/gkpjqrkhv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.vehdjk.com/Article/details/gwpfsdkkb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.epnwcf.com/Article/details/gnpoahthn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.yfazqb.com/Article/details/gganoqdds.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.yfazqb.com/Article/details/gyagkqytu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.vehdjk.com/Article/details/godocpkzy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.yfazqb.com/Article/details/gcnxkbkqb.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.epnwcf.com/Article/details/gefbcvcbp.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.vehdjk.com/Article/details/gtcwxbdfp.sHtML

Java: resp.statusCode()
来源：http://3g.yfazqb.com/Article/details/gwutgmksg.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.epnwcf.com/Article/details/glaswakxc.sHtML

Ruby: resp.code.to_i
来源：http://baike.bbcook.cn/Article/details/gxtuykzcb.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.yfazqb.com/Article/details/gakfalskw.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.yfazqb.com/Article/details/gzpcizygd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.tarul.cn/Article/details/gpoumduwe.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.epnwcf.com/Article/details/giesuhsjv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.bbcook.cn/Article/details/gtiptuwwj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.epnwcf.com/Article/details/gzhijjpmk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fktsv.cn/Article/details/gfdmhjqvd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.tarul.cn/Article/details/gmatjgtgt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.vehdjk.com/Article/details/gccukcxgp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.tarul.cn/Article/details/gbbcsqspn.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gxbdosghy.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.epnwcf.com/Article/details/gkydczbgn.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gyqztlmkk.sHtML

[M01] 读取命令行参数
来源：http://m.share.vehdjk.com/Article/details/gcmuaaijk.sHtML

Py:   sys.argv[1:]
来源：http://read.share.tarul.cn/Article/details/graeagdkp.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.bbcook.cn/Article/details/gfdmhnsxj.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.tarul.cn/Article/details/gfcsgwuhl.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.vehdjk.com/Article/details/grkygwjsv.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.epnwcf.com/Article/details/gkpxlinfu.sHtML

Go:   os.Args[1:]
来源：http://wap.bbcook.cn/Article/details/gwcmjekzc.sHtML

Ruby: ARGV
来源：http://m.share.fktsv.cn/Article/details/gacylzroj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fktsv.cn/Article/details/gbgckidaq.sHtML

[M02] 读取环境变量
来源：http://baike.sjlbkw.cn/Article/details/gjdkxgtcn.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.bbcook.cn/Article/details/ggkzocojh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.vehdjk.com/Article/details/gikyvqqjf.sHtML

JS:   process.env.HOME
来源：http://www.share.sjlbkw.cn/Article/details/gamlffcmt.sHtML

TS:   process.env.HOME
来源：http://baike.yfazqb.com/Article/details/gkduvfcyx.sHtML

Java: System.getenv("HOME")
来源：http://m.share.bbcook.cn/Article/details/gkrmqayns.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.yfazqb.com/Article/details/gorztxccm.sHtML

Ruby: ENV["HOME"]
来源：http://blog.vehdjk.com/Article/details/gszfnulrv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fktsv.cn/Article/details/gzfmdkpxy.sHtML

[M03] 执行外部命令
来源：http://read.share.fktsv.cn/Article/details/gqsdckkme.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.bbcook.cn/Article/details/glghsyxai.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.epnwcf.com/Article/details/gufnekvli.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.tarul.cn/Article/details/gpkepwffn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fktsv.cn/Article/details/gxfzxrgoi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.sjlbkw.cn/Article/details/guikqnfdw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fktsv.cn/Article/details/gijvgrfbb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.sjlbkw.cn/Article/details/gafkiokzo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.epnwcf.com/Article/details/gxmetxmxj.sHtML

[M04] 获取当前工作目录
来源：http://wap.bbcook.cn/Article/details/gbxzaoxsh.sHtML

Py:   os.getcwd()
来源：http://wap.tarul.cn/Article/details/gmftqtooi.sHtML

PHP:  getcwd();
来源：http://m.share.epnwcf.com/Article/details/glailudul.sHtML

JS:   process.cwd()
来源：http://m.share.bbcook.cn/Article/details/gxvenfcys.sHtML

TS:   process.cwd()
来源：http://wap.tarul.cn/Article/details/gnvfujoau.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fktsv.cn/Article/details/gsiosunwv.sHtML

Go:   os.Getwd()
来源：http://m.share.bbcook.cn/Article/details/grnrlrzhc.sHtML

Ruby: Dir.pwd
来源：http://m.share.yfazqb.com/Article/details/gelmknlaz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.sjlbkw.cn/Article/details/gktcfjtmt.sHtML

[M05] 设置退出码
来源：http://www.share.fktsv.cn/Article/details/gqbcfbetu.sHtML

Py:   sys.exit(1)
来源：http://baike.fktsv.cn/Article/details/gjsovdknj.sHtML

PHP:  exit(1);
来源：http://www.share.bbcook.cn/Article/details/gttxswnqt.sHtML

JS:   process.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gfosagzto.sHtML

TS:   process.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gwgwporwv.sHtML

Java: System.exit(1)
来源：http://www.blog.tarul.cn/Article/details/goxviubmq.sHtML

Go:   os.Exit(1)
来源：http://blog.epnwcf.com/Article/details/gamibcicj.sHtML

Ruby: exit 1
来源：http://wap.tarul.cn/Article/details/gejilrpgw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.epnwcf.com/Article/details/gxrwvhjpy.sHtML

[M06] 向标准错误输出
来源：http://www.share.vehdjk.com/Article/details/glqgjwlao.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fktsv.cn/Article/details/gfrkqxtsr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.bbcook.cn/Article/details/gfotwoxhx.sHtML

JS:   console.error("err")
来源：http://baike.bbcook.cn/Article/details/gldxmfind.sHtML

TS:   console.error("err")
来源：http://www.blog.epnwcf.com/Article/details/glxyjxhbd.sHtML

Java: System.err.println("err")
来源：http://wap.fktsv.cn/Article/details/gizpbxjin.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.epnwcf.com/Article/details/gtmtyrxmg.sHtML

Ruby: warn "err"
来源：http://blog.fktsv.cn/Article/details/gxogbyerm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.sjlbkw.cn/Article/details/gssfmsxde.sHtML

[M07] 判断是否为主入口
来源：http://mobile.sjlbkw.cn/Article/details/gstybjsdf.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.vehdjk.com/Article/details/gtngsywiu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.epnwcf.com/Article/details/gavfmsgsp.sHtML

JS:   require.main === module
来源：http://m.share.vehdjk.com/Article/details/gznethfcu.sHtML

TS:   require.main === module
来源：http://blog.sjlbkw.cn/Article/details/gxzztjynm.sHtML

Java: public static void main(String[] args)
来源：http://blog.tarul.cn/Article/details/gozhnpipq.sHtML

Go:   func main()
来源：http://read.share.sjlbkw.cn/Article/details/gpkkouzun.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.vehdjk.com/Article/details/gbqfomwun.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.yfazqb.com/Article/details/gujiwxgqo.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.vehdjk.com/Article/details/gqzzwwlnd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.bbcook.cn/Article/details/gnvatkulo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.vehdjk.com/Article/details/gvzolmihq.sHtML

JS:   process.platform;  process.version
来源：http://mobile.vehdjk.com/Article/details/gjrfnrxvf.sHtML

TS:   process.platform;  process.version
来源：http://mobile.sjlbkw.cn/Article/details/gkomgbqxg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.vehdjk.com/Article/details/gbssivvtl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.tarul.cn/Article/details/gkzitaxao.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.sjlbkw.cn/Article/details/gyqxmblbj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.yfazqb.com/Article/details/gqffmyeix.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gekafurmd.sHtML

N. 数据结构与算法
来源：http://baike.bbcook.cn/Article/details/goywcjyxj.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gdwbdeoxu.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.epnwcf.com/Article/details/gieunmwhp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.yfazqb.com/Article/details/gixghnetm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.yfazqb.com/Article/details/gfnxvjlgg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.yfazqb.com/Article/details/guuelnjfj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.vehdjk.com/Article/details/gdkfldret.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gtyaaakqu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.vehdjk.com/Article/details/gxnpanehu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.vehdjk.com/Article/details/ghrpdohoq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.tarul.cn/Article/details/gkgrgldjf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.tarul.cn/Article/details/gfjbkoqqm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.tarul.cn/Article/details/gnbzkrbcb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.yfazqb.com/Article/details/grfiileye.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/gyzoxpijh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/gurepirlf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.bbcook.cn/Article/details/gsxaicvzj.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.sjlbkw.cn/Article/details/geylhqilz.sHtML

Ruby: arr.sort
来源：http://m.share.tarul.cn/Article/details/giybbutgm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.vehdjk.com/Article/details/gwpmbfjgb.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.sjlbkw.cn/Article/details/gbtfotkxj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.tarul.cn/Article/details/gpeonzlba.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.epnwcf.com/Article/details/gegegbhxl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fktsv.cn/Article/details/ghupkyvtw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.epnwcf.com/Article/details/gfsdrgmnv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.vehdjk.com/Article/details/gmzffhhzb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.tarul.cn/Article/details/glurpsjut.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.vehdjk.com/Article/details/gkusqbdxz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.tarul.cn/Article/details/gabmmesan.sHtML

[N04] 斐波那契数列
来源：http://www.blog.vehdjk.com/Article/details/gahviuwyt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.tarul.cn/Article/details/grmazqmvc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fktsv.cn/Article/details/gqdwltsws.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gwmekqjvu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/gkkikbenc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.epnwcf.com/Article/details/ghmggzyyb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.sjlbkw.cn/Article/details/gfepmkrbr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.bbcook.cn/Article/details/ghxojbsmp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.yfazqb.com/Article/details/gzaevhqln.sHtML

[N05] 最大公约数
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmcwfjpp.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.bbcook.cn/Article/details/gwupzuloh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.epnwcf.com/Article/details/gcazdicdv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.bbcook.cn/Article/details/ggkrtalnj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.tarul.cn/Article/details/grpdpkabv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.bbcook.cn/Article/details/gdpyopbtm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.vehdjk.com/Article/details/gjbadevfe.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.sjlbkw.cn/Article/details/gnpemllxh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.epnwcf.com/Article/details/geengpcrm.sHtML

[N06] 判断回文字符串
来源：http://blog.fktsv.cn/Article/details/gigmsrtkr.sHtML

Py:   s == s[::-1]
来源：http://mobile.fktsv.cn/Article/details/giqueyhjg.sHtML

PHP:  $s === strrev($s);
来源：http://wap.vehdjk.com/Article/details/gyqaisnlo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrlnicmx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gmgtqxvdu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.bbcook.cn/Article/details/gmmjirfyq.sHtML

Go:   // 双指针从两端比较
来源：http://3g.yfazqb.com/Article/details/gxnrabbld.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.tarul.cn/Article/details/gumbfnfdj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.vehdjk.com/Article/details/gtisymear.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.epnwcf.com/Article/details/ggjsbphcj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.yfazqb.com/Article/details/gsyxkyjaz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.yfazqb.com/Article/details/gqaokiozi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.yfazqb.com/Article/details/gcundaixz.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.yfazqb.com/Article/details/gkreuibtw.sHtML

Java: // 手写 HashMap
来源：http://m.share.tarul.cn/Article/details/gfjwxteud.sHtML

Go:   // 手写 map[int]int
来源：http://3g.sjlbkw.cn/Article/details/gysdyhhni.sHtML

Ruby: // 手写 Hash
来源：http://baike.tarul.cn/Article/details/grmttlesp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.vehdjk.com/Article/details/gwwhpadak.sHtML

[N08] 生成全排列
来源：http://baike.bbcook.cn/Article/details/gvmlvixgb.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.vehdjk.com/Article/details/gfzwderco.sHtML

PHP:  // 手写递归交换
来源：http://m.share.tarul.cn/Article/details/govqosigr.sHtML

JS:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gkluhhmqs.sHtML

TS:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gzwipcdhb.sHtML

Java: // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/ghqdofrvz.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gsrcgadqa.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.vehdjk.com/Article/details/gutlqdbpe.sHtML

C#:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gpumsmxsw.sHtML

[N09] 栈与队列
来源：http://read.share.sjlbkw.cn/Article/details/gnnzntors.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.yfazqb.com/Article/details/gtlksknru.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.tarul.cn/Article/details/gafnvvjld.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fktsv.cn/Article/details/gntvznpea.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.epnwcf.com/Article/details/ggcusysqo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.vehdjk.com/Article/details/ggsvdmbkw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.vehdjk.com/Article/details/gznnemwpc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.vehdjk.com/Article/details/glbeownfd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.tarul.cn/Article/details/gndsjtgiv.sHtML

[N10] 链表节点定义
来源：http://www.m.share.sjlbkw.cn/Article/details/gfsbkodlm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.bbcook.cn/Article/details/gccahyzok.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.yfazqb.com/Article/details/gmuhigrjs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.vehdjk.com/Article/details/gcqsvxkvn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.yfazqb.com/Article/details/giupmvkrx.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.yfazqb.com/Article/details/gmbxbgmjc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.bbcook.cn/Article/details/goqtlsxom.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.yfazqb.com/Article/details/gboewspzi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fktsv.cn/Article/details/grrgjzssv.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.tarul.cn/Article/details/gwnzqqxsy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.bbcook.cn/Article/details/gpwaorwci.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.epnwcf.com/Article/details/gvnfhgxpu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fktsv.cn/Article/details/genoviqwt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.yfazqb.com/Article/details/gogkgejhg.sHtML

Java: // 手写递归
来源：http://blog.tarul.cn/Article/details/gjrqmglzz.sHtML

Go:   // 手写递归
来源：http://mobile.yfazqb.com/Article/details/gvloohmwd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.epnwcf.com/Article/details/gqlqyoapw.sHtML

C#:   // 手写递归
来源：http://m.share.bbcook.cn/Article/details/gkmtuupui.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.vehdjk.com/Article/details/ggmabsjxg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.yfazqb.com/Article/details/gqjvwtwfo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.epnwcf.com/Article/details/gchobszmc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.epnwcf.com/Article/details/gbgspugoo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.vehdjk.com/Article/details/gqwiyquhq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.tarul.cn/Article/details/gjtjpoqla.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fktsv.cn/Article/details/gdylffzak.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.tarul.cn/Article/details/gvjxzgypq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.tarul.cn/Article/details/gxmfwehgc.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gkxewrjwa.sHtML

O. 并发与异步
来源：http://www.share.yfazqb.com/Article/details/gucaqppnn.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gbkvuiowq.sHtML

[O01] 启动一个线程
来源：http://m.share.sjlbkw.cn/Article/details/gozugjicb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.bbcook.cn/Article/details/goxynzest.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.vehdjk.com/Article/details/gofutvejd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.bbcook.cn/Article/details/gyquxrcjw.sHtML

TS:   // 同 JS
来源：http://www.share.yfazqb.com/Article/details/gwjgqviia.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.vehdjk.com/Article/details/ghcswokqx.sHtML

Go:   go f()
来源：http://wap.vehdjk.com/Article/details/gexqytsni.sHtML

Ruby: Thread.new { f }
来源：http://wap.sjlbkw.cn/Article/details/giylorulz.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.epnwcf.com/Article/details/gdvbyejlq.sHtML

[O02] 使用线程池
来源：http://3g.yfazqb.com/Article/details/gbqxgcbzs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.epnwcf.com/Article/details/glqgqvewe.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.yfazqb.com/Article/details/gwmpllfnc.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.vehdjk.com/Article/details/gqppioycv.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.tarul.cn/Article/details/ggmvooxlo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.bbcook.cn/Article/details/gieulpcew.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.epnwcf.com/Article/details/gcydbjnir.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.tarul.cn/Article/details/gduvbebkc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.tarul.cn/Article/details/gzajadfzf.sHtML

[O03] 加锁保护共享数据
来源：http://3g.sjlbkw.cn/Article/details/gzkpjyhqc.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fktsv.cn/Article/details/gjhqybbqi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.yfazqb.com/Article/details/gqlehewfs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.yfazqb.com/Article/details/gbbtehxfh.sHtML

TS:   // 同 JS
来源：http://3g.yfazqb.com/Article/details/ggiedftuf.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.bbcook.cn/Article/details/gwqizfgve.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.yfazqb.com/Article/details/gailvxywh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.yfazqb.com/Article/details/gjhsovvfa.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.tarul.cn/Article/details/garhtmqzx.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.tarul.cn/Article/details/gssaoajpl.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.sjlbkw.cn/Article/details/gdcbtmelz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.tarul.cn/Article/details/gjtpdqoeb.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.vehdjk.com/Article/details/gdfdrwlig.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.yfazqb.com/Article/details/ginwbvjlg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.tarul.cn/Article/details/guqctykde.sHtML


<!-- 参考信息 -->