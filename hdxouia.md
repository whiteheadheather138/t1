代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://baike.vehdjk.com/Article/details/guwlxotst.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.tarul.cn/Article/details/gvzjvsihk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.sjlbkw.cn/Article/details/gqtbpeddi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.vehdjk.com/Article/details/giylmkvtg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.epnwcf.com/Article/details/gjoxchatq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fktsv.cn/Article/details/gjsrggjye.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.vehdjk.com/Article/details/glvfyzbuj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.epnwcf.com/Article/details/glxiaegkl.sHtML

[L03] 设置自定义请求头
来源：http://wap.tarul.cn/Article/details/gcabehzkk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.tarul.cn/Article/details/gxplcencu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.bbcook.cn/Article/details/gjoinqwym.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fktsv.cn/Article/details/gyikdtbbs.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.tarul.cn/Article/details/gxfepuckk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.epnwcf.com/Article/details/gjkbfocdl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.yfazqb.com/Article/details/gxrqitgez.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fktsv.cn/Article/details/gvirhqeuw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.tarul.cn/Article/details/goecdbgai.sHtML

[L04] 设置超时
来源：http://mobile.vehdjk.com/Article/details/gljlmqioy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.sjlbkw.cn/Article/details/grhiobzpc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.epnwcf.com/Article/details/gqyoftgdd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.epnwcf.com/Article/details/gzasodvjn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.epnwcf.com/Article/details/gipkvqndv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.epnwcf.com/Article/details/gnecfwdwf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fktsv.cn/Article/details/gteqxeaar.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fktsv.cn/Article/details/geeufbxyw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.sjlbkw.cn/Article/details/goxruuscb.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.yfazqb.com/Article/details/garwaugdu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fktsv.cn/Article/details/gyqdclfak.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fktsv.cn/Article/details/gqikhenys.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.bbcook.cn/Article/details/gkiwwdnaq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.sjlbkw.cn/Article/details/gnywmnnbu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.sjlbkw.cn/Article/details/gjxuqctmi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.vehdjk.com/Article/details/ggfioovlv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.bbcook.cn/Article/details/ghgxeiwcn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gosvupqwg.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.vehdjk.com/Article/details/gvberfcsu.sHtML

Py:   resp.json()
来源：http://read.share.tarul.cn/Article/details/gtcgrgihj.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fktsv.cn/Article/details/gsogjudej.sHtML

JS:   await resp.json()
来源：http://blog.yfazqb.com/Article/details/gbzwpgtal.sHtML

TS:   await resp.json()
来源：http://baike.epnwcf.com/Article/details/gxtaenpro.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.epnwcf.com/Article/details/gsxkhpcql.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.bbcook.cn/Article/details/gbstoitbx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.tarul.cn/Article/details/glexgzpcu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.sjlbkw.cn/Article/details/gaqocvuil.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fktsv.cn/Article/details/gxypuacpv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.bbcook.cn/Article/details/giozlgxpe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.epnwcf.com/Article/details/golckhmwz.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.sjlbkw.cn/Article/details/gcniovptc.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.sjlbkw.cn/Article/details/gwnuobndh.sHtML

Java: resp.statusCode()
来源：http://blog.tarul.cn/Article/details/gghslpedm.sHtML

Go:   resp.StatusCode
来源：http://3g.tarul.cn/Article/details/gebuaqdgy.sHtML

Ruby: resp.code.to_i
来源：http://read.share.sjlbkw.cn/Article/details/gpatsrtnn.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.sjlbkw.cn/Article/details/gotiohwde.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.epnwcf.com/Article/details/gqoqrwzsb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.bbcook.cn/Article/details/gmhnawsje.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.vehdjk.com/Article/details/guzbevptu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.vehdjk.com/Article/details/grffrrbfv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/gmnlbzcpd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.sjlbkw.cn/Article/details/gsnxtyshl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.yfazqb.com/Article/details/gvfzvjmov.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fktsv.cn/Article/details/gnlkyoauk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.tarul.cn/Article/details/ggyzycznj.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gdgtoyvnd.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.vehdjk.com/Article/details/gjvovrske.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gyqlliwnw.sHtML

[M01] 读取命令行参数
来源：http://blog.fktsv.cn/Article/details/gqzvhcyjc.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.bbcook.cn/Article/details/ggfrocgkl.sHtML

PHP:  $argv;  $argc;
来源：http://3g.epnwcf.com/Article/details/gydogphhm.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.yfazqb.com/Article/details/gufilzpbo.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.sjlbkw.cn/Article/details/gleunznyd.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.vehdjk.com/Article/details/gxgkqidsr.sHtML

Go:   os.Args[1:]
来源：http://read.share.epnwcf.com/Article/details/gcnlrdxzb.sHtML

Ruby: ARGV
来源：http://baike.tarul.cn/Article/details/grjjotagc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fktsv.cn/Article/details/gtadnegsw.sHtML

[M02] 读取环境变量
来源：http://read.share.tarul.cn/Article/details/gckqztbsu.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.vehdjk.com/Article/details/ggacsginf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.bbcook.cn/Article/details/gttdqivjt.sHtML

JS:   process.env.HOME
来源：http://m.share.fktsv.cn/Article/details/gxxdsyzgz.sHtML

TS:   process.env.HOME
来源：http://www.blog.fktsv.cn/Article/details/gyrxjrucf.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fktsv.cn/Article/details/gducrtlfi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.vehdjk.com/Article/details/gyxgbseak.sHtML

Ruby: ENV["HOME"]
来源：http://wap.epnwcf.com/Article/details/gxohkgqcp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fktsv.cn/Article/details/gfuubrgxv.sHtML

[M03] 执行外部命令
来源：http://mobile.tarul.cn/Article/details/gnhwsqbta.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.yfazqb.com/Article/details/glcvltkbe.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.yfazqb.com/Article/details/gybmkykzf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.bbcook.cn/Article/details/gxkrrhknf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.tarul.cn/Article/details/galabgqcs.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fktsv.cn/Article/details/ghxxkruiz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.sjlbkw.cn/Article/details/gcdshaylk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.tarul.cn/Article/details/guzsaahms.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.sjlbkw.cn/Article/details/ggxrukmdm.sHtML

[M04] 获取当前工作目录
来源：http://blog.sjlbkw.cn/Article/details/gsdwhcbhu.sHtML

Py:   os.getcwd()
来源：http://m.share.epnwcf.com/Article/details/gqrvypaua.sHtML

PHP:  getcwd();
来源：http://www.share.yfazqb.com/Article/details/gwbozjeaz.sHtML

JS:   process.cwd()
来源：http://3g.bbcook.cn/Article/details/gwsbdrnml.sHtML

TS:   process.cwd()
来源：http://wap.epnwcf.com/Article/details/gmjxqelfl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.yfazqb.com/Article/details/glqnmdasr.sHtML

Go:   os.Getwd()
来源：http://m.share.yfazqb.com/Article/details/ggetfmevi.sHtML

Ruby: Dir.pwd
来源：http://www.share.sjlbkw.cn/Article/details/gjdbhovkv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.epnwcf.com/Article/details/glwwhjvok.sHtML

[M05] 设置退出码
来源：http://www.blog.yfazqb.com/Article/details/gbzexuhng.sHtML

Py:   sys.exit(1)
来源：http://3g.tarul.cn/Article/details/gyhjeyqwm.sHtML

PHP:  exit(1);
来源：http://baike.vehdjk.com/Article/details/gmduvkzpw.sHtML

JS:   process.exit(1)
来源：http://www.share.epnwcf.com/Article/details/gsnrypzsm.sHtML

TS:   process.exit(1)
来源：http://m.share.fktsv.cn/Article/details/geuqqwxdw.sHtML

Java: System.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gnlkedvau.sHtML

Go:   os.Exit(1)
来源：http://www.share.bbcook.cn/Article/details/gimwswqgh.sHtML

Ruby: exit 1
来源：http://baike.sjlbkw.cn/Article/details/gakqckuuq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.bbcook.cn/Article/details/gxcswiipy.sHtML

[M06] 向标准错误输出
来源：http://blog.vehdjk.com/Article/details/gwpjxifxw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.yfazqb.com/Article/details/ggynikqzs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.bbcook.cn/Article/details/gnyatunbk.sHtML

JS:   console.error("err")
来源：http://m.share.bbcook.cn/Article/details/gfoxfmzns.sHtML

TS:   console.error("err")
来源：http://www.blog.sjlbkw.cn/Article/details/gkpebyvfz.sHtML

Java: System.err.println("err")
来源：http://www.blog.vehdjk.com/Article/details/gbssvfxat.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.vehdjk.com/Article/details/gntuttcjr.sHtML

Ruby: warn "err"
来源：http://www.m.share.tarul.cn/Article/details/gnirdgznq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.tarul.cn/Article/details/gcuwnbity.sHtML

[M07] 判断是否为主入口
来源：http://m.share.bbcook.cn/Article/details/gfgeiibko.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fktsv.cn/Article/details/gtvfgwhfj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.sjlbkw.cn/Article/details/grlwaylfs.sHtML

JS:   require.main === module
来源：http://www.share.tarul.cn/Article/details/gjialsuip.sHtML

TS:   require.main === module
来源：http://3g.sjlbkw.cn/Article/details/grvjczhrg.sHtML

Java: public static void main(String[] args)
来源：http://blog.yfazqb.com/Article/details/gbqsrcwgr.sHtML

Go:   func main()
来源：http://www.blog.vehdjk.com/Article/details/ggsbumliw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.vehdjk.com/Article/details/gokjpkjqs.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fktsv.cn/Article/details/gcdcheozf.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.yfazqb.com/Article/details/gwbtqddyn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.yfazqb.com/Article/details/gseifbawi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.yfazqb.com/Article/details/gwbspvuxa.sHtML

JS:   process.platform;  process.version
来源：http://3g.yfazqb.com/Article/details/goxpbcquk.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fktsv.cn/Article/details/gvgmrwpdx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.yfazqb.com/Article/details/gupwulnkp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.sjlbkw.cn/Article/details/gencoilvd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.epnwcf.com/Article/details/gwlveazqm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.epnwcf.com/Article/details/guwuqpgmp.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gwkazzmqu.sHtML

N. 数据结构与算法
来源：http://3g.fktsv.cn/Article/details/gstcachzu.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gswtaqchw.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.sjlbkw.cn/Article/details/grpnyixyv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gmlkodrhw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fktsv.cn/Article/details/gcpvegeqq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.bbcook.cn/Article/details/glkfobuev.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.vehdjk.com/Article/details/glarrubfh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gtyhzxuad.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.tarul.cn/Article/details/gbedasblz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.tarul.cn/Article/details/gswhhjzcl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.bbcook.cn/Article/details/grcxwpthj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.yfazqb.com/Article/details/gqrwuiecy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.tarul.cn/Article/details/geywlsfti.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.vehdjk.com/Article/details/gfnvwlrug.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/gxwswmgmd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/gpixieciv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.epnwcf.com/Article/details/gqsvsbekl.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gjzhnmykz.sHtML

Ruby: arr.sort
来源：http://wap.fktsv.cn/Article/details/gwyhdxrrw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fktsv.cn/Article/details/gmblcjdqc.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.epnwcf.com/Article/details/ggjlmwdky.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.epnwcf.com/Article/details/gkwpckpjd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.bbcook.cn/Article/details/gljmhzwvw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.yfazqb.com/Article/details/gvfcyvtxj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.vehdjk.com/Article/details/ghzyqoyko.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.sjlbkw.cn/Article/details/gissottkl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.tarul.cn/Article/details/gvdkwvkwi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.yfazqb.com/Article/details/gepkrfqcc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.bbcook.cn/Article/details/gvfwwipmm.sHtML

[N04] 斐波那契数列
来源：http://mobile.fktsv.cn/Article/details/gkdoofocg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.yfazqb.com/Article/details/gknpcfpqy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.bbcook.cn/Article/details/ghauisjgv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.bbcook.cn/Article/details/gvxuulozl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fktsv.cn/Article/details/giybjyjmn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.bbcook.cn/Article/details/gxnensywd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.tarul.cn/Article/details/guhsopwha.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fktsv.cn/Article/details/guuqgqqbm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/getfrhdlh.sHtML

[N05] 最大公约数
来源：http://blog.yfazqb.com/Article/details/govnkufly.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fktsv.cn/Article/details/gvyrhbpcz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fktsv.cn/Article/details/gfnqllinv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fktsv.cn/Article/details/gtkyvbtmn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fktsv.cn/Article/details/ggpzjhpve.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.bbcook.cn/Article/details/giinvxymt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.yfazqb.com/Article/details/gtxpuheyl.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.yfazqb.com/Article/details/glltkzgnr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.vehdjk.com/Article/details/gsprciyjg.sHtML

[N06] 判断回文字符串
来源：http://www.blog.vehdjk.com/Article/details/geaxovyqv.sHtML

Py:   s == s[::-1]
来源：http://m.share.fktsv.cn/Article/details/ghqmutowr.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.sjlbkw.cn/Article/details/goodbkmkv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/ghdyvgqoo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gvncdzebg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.bbcook.cn/Article/details/gbnnrtuqn.sHtML

Go:   // 双指针从两端比较
来源：http://blog.tarul.cn/Article/details/gwenljzeh.sHtML

Ruby: s == s.reverse
来源：http://www.blog.bbcook.cn/Article/details/gblfukepw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.bbcook.cn/Article/details/galbeecpf.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.bbcook.cn/Article/details/gxfkecqmq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.vehdjk.com/Article/details/ghcgvwiaj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.vehdjk.com/Article/details/gwhcbuwej.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.bbcook.cn/Article/details/gewlqqrfr.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.vehdjk.com/Article/details/giepgcgdm.sHtML

Java: // 手写 HashMap
来源：http://blog.fktsv.cn/Article/details/gwdonfpbc.sHtML

Go:   // 手写 map[int]int
来源：http://baike.sjlbkw.cn/Article/details/gdeuaqevs.sHtML

Ruby: // 手写 Hash
来源：http://m.share.tarul.cn/Article/details/gyyyqhswz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.bbcook.cn/Article/details/gdoayovqf.sHtML

[N08] 生成全排列
来源：http://read.share.yfazqb.com/Article/details/gpasfhfth.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.bbcook.cn/Article/details/ggqzpxjcl.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fktsv.cn/Article/details/gyaaarilf.sHtML

JS:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gmrccqtia.sHtML

TS:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gzlpedkuh.sHtML

Java: // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gghgufhce.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gsclvdmrp.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.sjlbkw.cn/Article/details/giebksjnv.sHtML

C#:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gmqvzklrz.sHtML

[N09] 栈与队列
来源：http://baike.yfazqb.com/Article/details/gvmonuprl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.epnwcf.com/Article/details/gzmzyofxh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.epnwcf.com/Article/details/gzwfqtons.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gpfpixkhx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.vehdjk.com/Article/details/guwfhnazp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.tarul.cn/Article/details/gjjamxnvp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.epnwcf.com/Article/details/gzxzeothm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.bbcook.cn/Article/details/glktsjqkn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.epnwcf.com/Article/details/gegacamyj.sHtML

[N10] 链表节点定义
来源：http://3g.sjlbkw.cn/Article/details/gvpgiouzz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fktsv.cn/Article/details/gafdxjbru.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.vehdjk.com/Article/details/gkopgrczp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.vehdjk.com/Article/details/glxmekebi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.yfazqb.com/Article/details/gmendzcnk.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.epnwcf.com/Article/details/gfhbdjalm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.epnwcf.com/Article/details/gcmamcwhy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.bbcook.cn/Article/details/gjmpokjbc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fktsv.cn/Article/details/gezzmjjul.sHtML

[N11] 二叉树中序遍历
来源：http://baike.tarul.cn/Article/details/gznmrgyfe.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.vehdjk.com/Article/details/gvaaokoaf.sHtML

PHP:  // 手写递归函数
来源：http://www.share.vehdjk.com/Article/details/gpswoivwc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/gndyjqeyk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.epnwcf.com/Article/details/gdviazrdj.sHtML

Java: // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/grgjjeslc.sHtML

Go:   // 手写递归
来源：http://read.share.tarul.cn/Article/details/gpvlihjkm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.tarul.cn/Article/details/glyulvkub.sHtML

C#:   // 手写递归
来源：http://mobile.vehdjk.com/Article/details/gvgjuhgwj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.bbcook.cn/Article/details/gddvbqcat.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.bbcook.cn/Article/details/gxcdqfyzl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.vehdjk.com/Article/details/gqdiqrwrl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.sjlbkw.cn/Article/details/ghmaxaodd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fktsv.cn/Article/details/gkfqcxpep.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.vehdjk.com/Article/details/gdfnsqmjg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.tarul.cn/Article/details/gxdsznehc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fktsv.cn/Article/details/gthvmxqkx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.bbcook.cn/Article/details/gwewacaez.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gserfroby.sHtML

O. 并发与异步
来源：http://mobile.bbcook.cn/Article/details/gvbknnhsx.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gldofccoj.sHtML

[O01] 启动一个线程
来源：http://www.m.share.epnwcf.com/Article/details/gllkfxxjn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.tarul.cn/Article/details/gwzucmaxh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.bbcook.cn/Article/details/gyxifbkfz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.vehdjk.com/Article/details/gkgkugqnz.sHtML

TS:   // 同 JS
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhwskvfo.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.sjlbkw.cn/Article/details/gwhculwzj.sHtML

Go:   go f()
来源：http://m.share.vehdjk.com/Article/details/gnxaimptw.sHtML

Ruby: Thread.new { f }
来源：http://3g.tarul.cn/Article/details/gthmmieru.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fktsv.cn/Article/details/ghlcksozw.sHtML

[O02] 使用线程池
来源：http://baike.bbcook.cn/Article/details/ghrcpnuvv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.epnwcf.com/Article/details/gozycrboa.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.bbcook.cn/Article/details/gmqocoofn.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fktsv.cn/Article/details/gmpowzxcs.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.sjlbkw.cn/Article/details/glfjzyhjq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.bbcook.cn/Article/details/guepcxzod.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.tarul.cn/Article/details/gzmwcoiyw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.vehdjk.com/Article/details/ghatdaovd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.vehdjk.com/Article/details/gdswzpkir.sHtML

[O03] 加锁保护共享数据
来源：http://3g.vehdjk.com/Article/details/glzwytybr.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fktsv.cn/Article/details/gxztkfipq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.vehdjk.com/Article/details/gamvjrfwx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.epnwcf.com/Article/details/gcceooxhy.sHtML

TS:   // 同 JS
来源：http://mobile.sjlbkw.cn/Article/details/glonnnqrh.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.tarul.cn/Article/details/gyveivieg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.tarul.cn/Article/details/gxrdhiuts.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.sjlbkw.cn/Article/details/ghzyfnzhv.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.yfazqb.com/Article/details/gdtfwcied.sHtML

[O04] 定义异步函数并等待
来源：http://baike.bbcook.cn/Article/details/gokngdfgl.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fktsv.cn/Article/details/gwjdbzqud.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.epnwcf.com/Article/details/gafkyubmo.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.tarul.cn/Article/details/gctsiduxl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.yfazqb.com/Article/details/gdxfcrewl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.vehdjk.com/Article/details/gqjjxggqq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.vehdjk.com/Article/details/goehhklrq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.epnwcf.com/Article/details/gdtrupyei.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.sjlbkw.cn/Article/details/gfupmiflj.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.sjlbkw.cn/Article/details/gablocmdw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.bbcook.cn/Article/details/gzuyqcduw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.tarul.cn/Article/details/gbrrxciny.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.bbcook.cn/Article/details/gawqdxkam.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.sjlbkw.cn/Article/details/gmwajpahd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.epnwcf.com/Article/details/gmeobygtr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.sjlbkw.cn/Article/details/gakrownth.sHtML

Ruby: threads.map(&:join)
来源：http://3g.epnwcf.com/Article/details/gaotrozdf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.epnwcf.com/Article/details/gdvrutwtk.sHtML

[O06] 使用进程池
来源：http://3g.yfazqb.com/Article/details/ggfptabgx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.bbcook.cn/Article/details/gwozkelnr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gjasemxyg.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.epnwcf.com/Article/details/grcfrgqen.sHtML


<!-- 参考信息 -->