代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.epnwcf.com/Article/details/gvhedblnu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.yfazqb.com/Article/details/gvyoyizit.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.tarul.cn/Article/details/gsnaqetka.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.epnwcf.com/Article/details/gadprrgde.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.bbcook.cn/Article/details/gecoejnoy.sHtML

[L04] 设置超时
来源：http://blog.sjlbkw.cn/Article/details/gjpnxoewj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fktsv.cn/Article/details/givgtsjfg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fktsv.cn/Article/details/gcvjzjaby.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.sjlbkw.cn/Article/details/gkmemilck.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fktsv.cn/Article/details/ggrumyqwk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.yfazqb.com/Article/details/gxwixrmhp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.yfazqb.com/Article/details/ggumtkfdq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.vehdjk.com/Article/details/gmyayytqz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.epnwcf.com/Article/details/geaveigmo.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.yfazqb.com/Article/details/gdxzmilum.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.epnwcf.com/Article/details/geibqmbsw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.epnwcf.com/Article/details/gpovjmctu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.tarul.cn/Article/details/glnrezzof.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.sjlbkw.cn/Article/details/grfuckozi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.epnwcf.com/Article/details/gdgdqkvru.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.yfazqb.com/Article/details/guarqpslw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.bbcook.cn/Article/details/gwtxuzfqb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gykwhwwuw.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gjnmdviag.sHtML

Py:   resp.json()
来源：http://read.share.vehdjk.com/Article/details/gahatrsuu.sHtML

PHP:  json_decode($body, true);
来源：http://3g.sjlbkw.cn/Article/details/ggdirhcvt.sHtML

JS:   await resp.json()
来源：http://www.m.share.yfazqb.com/Article/details/gvhhinwud.sHtML

TS:   await resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gdmxicntc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.epnwcf.com/Article/details/gvydhfpnj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.yfazqb.com/Article/details/gxodyzhlx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.yfazqb.com/Article/details/gyuobwrkz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.yfazqb.com/Article/details/grladmcfj.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.tarul.cn/Article/details/gnncllajx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.epnwcf.com/Article/details/gccfxtmfz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.sjlbkw.cn/Article/details/gdzqeicmg.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.vehdjk.com/Article/details/gaqorwzkg.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.bbcook.cn/Article/details/gbobvwzkt.sHtML

Java: resp.statusCode()
来源：http://3g.sjlbkw.cn/Article/details/gzdpulmda.sHtML

Go:   resp.StatusCode
来源：http://mobile.tarul.cn/Article/details/gflfjelcj.sHtML

Ruby: resp.code.to_i
来源：http://wap.fktsv.cn/Article/details/geozrffni.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fktsv.cn/Article/details/gpjbtzuwx.sHtML

[L08] 并发请求多个地址
来源：http://baike.tarul.cn/Article/details/glbzxhhaa.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.sjlbkw.cn/Article/details/glhhadiyr.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.vehdjk.com/Article/details/gszvvbqup.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.tarul.cn/Article/details/ghylallsb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.vehdjk.com/Article/details/gorikgdfs.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.epnwcf.com/Article/details/gfqriwkvi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.sjlbkw.cn/Article/details/gdijuhhdz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.tarul.cn/Article/details/gmuahdtva.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.tarul.cn/Article/details/gdikfyiax.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gzhkymfpy.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.vehdjk.com/Article/details/gfkqfqaeq.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gtqrpljga.sHtML

[M01] 读取命令行参数
来源：http://mobile.vehdjk.com/Article/details/gflviqghk.sHtML

Py:   sys.argv[1:]
来源：http://3g.bbcook.cn/Article/details/gfrpoakxh.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.epnwcf.com/Article/details/gthlptqut.sHtML

JS:   process.argv.slice(2)
来源：http://blog.bbcook.cn/Article/details/gyeszumbw.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.vehdjk.com/Article/details/gzhrylwhb.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.vehdjk.com/Article/details/gdsngwfrj.sHtML

Go:   os.Args[1:]
来源：http://m.share.tarul.cn/Article/details/gsohdwojx.sHtML

Ruby: ARGV
来源：http://3g.vehdjk.com/Article/details/gjphfwlbt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.epnwcf.com/Article/details/ggdegttbd.sHtML

[M02] 读取环境变量
来源：http://www.blog.vehdjk.com/Article/details/gukckvdyp.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.sjlbkw.cn/Article/details/ggcwnzqcx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fktsv.cn/Article/details/gzfznzpek.sHtML

JS:   process.env.HOME
来源：http://read.share.epnwcf.com/Article/details/geojfetqr.sHtML

TS:   process.env.HOME
来源：http://blog.vehdjk.com/Article/details/gxoaoqurx.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/grjvocdrc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.epnwcf.com/Article/details/ganisatng.sHtML

Ruby: ENV["HOME"]
来源：http://baike.vehdjk.com/Article/details/gmqrbwidn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.yfazqb.com/Article/details/gswtftlba.sHtML

[M03] 执行外部命令
来源：http://3g.vehdjk.com/Article/details/gnxbokgoe.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.bbcook.cn/Article/details/gaafoxxuv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.bbcook.cn/Article/details/grlslcerv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fktsv.cn/Article/details/gvulivets.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.yfazqb.com/Article/details/guvzyollm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.bbcook.cn/Article/details/gxcewwcwy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.yfazqb.com/Article/details/gmfslouwa.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.vehdjk.com/Article/details/gahaygjrp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.bbcook.cn/Article/details/gzmjcigtd.sHtML

[M04] 获取当前工作目录
来源：http://m.share.tarul.cn/Article/details/gllvlinze.sHtML

Py:   os.getcwd()
来源：http://www.share.tarul.cn/Article/details/gefgrjwfa.sHtML

PHP:  getcwd();
来源：http://read.share.yfazqb.com/Article/details/gchbusnvn.sHtML

JS:   process.cwd()
来源：http://m.share.epnwcf.com/Article/details/gzeboqjoz.sHtML

TS:   process.cwd()
来源：http://blog.fktsv.cn/Article/details/gemhylcvv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.yfazqb.com/Article/details/gkwdnqmvz.sHtML

Go:   os.Getwd()
来源：http://wap.yfazqb.com/Article/details/gmigfikcd.sHtML

Ruby: Dir.pwd
来源：http://www.share.bbcook.cn/Article/details/grgqesvxu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.tarul.cn/Article/details/gsjrdelsn.sHtML

[M05] 设置退出码
来源：http://baike.vehdjk.com/Article/details/gndbrtiva.sHtML

Py:   sys.exit(1)
来源：http://baike.yfazqb.com/Article/details/gxcxbsjwr.sHtML

PHP:  exit(1);
来源：http://blog.sjlbkw.cn/Article/details/gzygoyrrh.sHtML

JS:   process.exit(1)
来源：http://m.share.yfazqb.com/Article/details/guioegizw.sHtML

TS:   process.exit(1)
来源：http://blog.vehdjk.com/Article/details/gvxhhmjpg.sHtML

Java: System.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gpeqoifxv.sHtML

Go:   os.Exit(1)
来源：http://www.share.bbcook.cn/Article/details/gpgxlxbzt.sHtML

Ruby: exit 1
来源：http://www.blog.tarul.cn/Article/details/gznscbrcm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.vehdjk.com/Article/details/garuamduv.sHtML

[M06] 向标准错误输出
来源：http://baike.fktsv.cn/Article/details/ghbkjikoe.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.bbcook.cn/Article/details/gnpmxqcnw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.bbcook.cn/Article/details/gcnrfkrvp.sHtML

JS:   console.error("err")
来源：http://www.share.bbcook.cn/Article/details/gtsynoeim.sHtML

TS:   console.error("err")
来源：http://mobile.yfazqb.com/Article/details/ghwsdnlsy.sHtML

Java: System.err.println("err")
来源：http://3g.vehdjk.com/Article/details/gcoasjcgo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.bbcook.cn/Article/details/gfpczawcq.sHtML

Ruby: warn "err"
来源：http://read.share.sjlbkw.cn/Article/details/gcxloxkjd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.tarul.cn/Article/details/ggpuuccla.sHtML

[M07] 判断是否为主入口
来源：http://www.share.bbcook.cn/Article/details/gcecagivp.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.vehdjk.com/Article/details/gsppbwoyd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.epnwcf.com/Article/details/gswqaqnec.sHtML

JS:   require.main === module
来源：http://read.share.tarul.cn/Article/details/gsiykmsmd.sHtML

TS:   require.main === module
来源：http://3g.vehdjk.com/Article/details/giutgnffd.sHtML

Java: public static void main(String[] args)
来源：http://3g.epnwcf.com/Article/details/gisklxkeh.sHtML

Go:   func main()
来源：http://read.share.tarul.cn/Article/details/glkvphprx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.sjlbkw.cn/Article/details/gkzdswodd.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.bbcook.cn/Article/details/gharhyqbh.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.epnwcf.com/Article/details/gmfwxhydq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.epnwcf.com/Article/details/gwipxwurl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.vehdjk.com/Article/details/gwasdstfm.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.tarul.cn/Article/details/grvbwrxnt.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.vehdjk.com/Article/details/gxepbhije.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.sjlbkw.cn/Article/details/gudtggkrv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.vehdjk.com/Article/details/gvhnwgxyp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.vehdjk.com/Article/details/ggwymytwz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.bbcook.cn/Article/details/gjioxaenc.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gqbcgzpqu.sHtML

N. 数据结构与算法
来源：http://www.m.share.bbcook.cn/Article/details/gvnrgvsju.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/glshrekgg.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fktsv.cn/Article/details/giyoisrhb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.bbcook.cn/Article/details/gmojfjmhu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.vehdjk.com/Article/details/gyykuljjt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.yfazqb.com/Article/details/gskchvhvd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.tarul.cn/Article/details/gupydhhig.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gyuumzsob.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gncyqeeyt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.yfazqb.com/Article/details/gvorazrxu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gjemnaotm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.yfazqb.com/Article/details/ggfcyxxqi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.tarul.cn/Article/details/gexlpfwxz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.sjlbkw.cn/Article/details/gsozcrftd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/gmlgrjnil.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.yfazqb.com/Article/details/gcguvncvo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.vehdjk.com/Article/details/gqoffygwx.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.yfazqb.com/Article/details/gaujpvpvz.sHtML

Ruby: arr.sort
来源：http://wap.vehdjk.com/Article/details/gfkjbwako.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.vehdjk.com/Article/details/gxqnunvqh.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.vehdjk.com/Article/details/grzdzrgii.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.sjlbkw.cn/Article/details/gsdxwndzw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fktsv.cn/Article/details/gvorydgny.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.yfazqb.com/Article/details/gvgdhdjew.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.vehdjk.com/Article/details/goviknfpv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.tarul.cn/Article/details/ggijhifxr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.sjlbkw.cn/Article/details/gzejgoqqx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.tarul.cn/Article/details/gadsmwkoc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.tarul.cn/Article/details/gpsqdfaun.sHtML

[N04] 斐波那契数列
来源：http://wap.epnwcf.com/Article/details/gwltozxdu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.vehdjk.com/Article/details/gzpsedmua.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fktsv.cn/Article/details/gamjjhicf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/gbzomtpyb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/gopyedgip.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.vehdjk.com/Article/details/gxmzdpgek.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.tarul.cn/Article/details/ghnvhemwi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.tarul.cn/Article/details/gogysxujn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/gnzgvukgh.sHtML

[N05] 最大公约数
来源：http://read.share.sjlbkw.cn/Article/details/gsmmnfozm.sHtML

Py:   math.gcd(a, b)
来源：http://baike.yfazqb.com/Article/details/gtemmskww.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.yfazqb.com/Article/details/gixxrieek.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fktsv.cn/Article/details/gofxajiga.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.epnwcf.com/Article/details/gdmsvelyi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.bbcook.cn/Article/details/grwusjflm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.tarul.cn/Article/details/gtipnmysa.sHtML

Ruby: a.gcd(b)
来源：http://www.share.vehdjk.com/Article/details/globfcnqd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.tarul.cn/Article/details/gxyfpymfu.sHtML

[N06] 判断回文字符串
来源：http://wap.tarul.cn/Article/details/gxvsxbaqi.sHtML

Py:   s == s[::-1]
来源：http://read.share.fktsv.cn/Article/details/givwyllgo.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.epnwcf.com/Article/details/gmjkddvlb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/gemmqliun.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/gjzfpvjyi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.yfazqb.com/Article/details/gcvjofpoc.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.sjlbkw.cn/Article/details/gxwosmmjo.sHtML

Ruby: s == s.reverse
来源：http://m.share.epnwcf.com/Article/details/gfsjxtxcn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.epnwcf.com/Article/details/gxpwveupi.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.bbcook.cn/Article/details/guxbabvcj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.bbcook.cn/Article/details/gvlnwunae.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.bbcook.cn/Article/details/glwvdebcp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.bbcook.cn/Article/details/gygmypvmd.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.vehdjk.com/Article/details/gdoexppoz.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.yfazqb.com/Article/details/gtyzyxpim.sHtML

Go:   // 手写 map[int]int
来源：http://blog.vehdjk.com/Article/details/gbxuiinaf.sHtML

Ruby: // 手写 Hash
来源：http://blog.sjlbkw.cn/Article/details/gohhwcbqn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fktsv.cn/Article/details/gfogvfzej.sHtML

[N08] 生成全排列
来源：http://wap.epnwcf.com/Article/details/gaptwxeip.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.vehdjk.com/Article/details/gaxalrosy.sHtML

PHP:  // 手写递归交换
来源：http://3g.sjlbkw.cn/Article/details/gezuhtcee.sHtML

JS:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/grrgxewae.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gnajahxae.sHtML

Java: // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gmyumzzec.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gtbnblysq.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.bbcook.cn/Article/details/gllhieisl.sHtML

C#:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gwnfauzxw.sHtML

[N09] 栈与队列
来源：http://baike.tarul.cn/Article/details/gkpyikkci.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.tarul.cn/Article/details/gqddxjxqh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gmwvnnopi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gdhrrnyaq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.tarul.cn/Article/details/gkomurewa.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.bbcook.cn/Article/details/gukdzpbun.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.yfazqb.com/Article/details/gzqzglemy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fktsv.cn/Article/details/gvhyvkyeu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.epnwcf.com/Article/details/gyiesszwu.sHtML

[N10] 链表节点定义
来源：http://blog.tarul.cn/Article/details/gbjbqigsn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.sjlbkw.cn/Article/details/gskznclbg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.bbcook.cn/Article/details/gpjkuiyob.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.tarul.cn/Article/details/gpkdtpjpn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.sjlbkw.cn/Article/details/gehzibyhr.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.bbcook.cn/Article/details/gefjprzcs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fktsv.cn/Article/details/gezewsxah.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.vehdjk.com/Article/details/geqtldkrt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fktsv.cn/Article/details/gcboypjkx.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.tarul.cn/Article/details/girzqnxsa.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.bbcook.cn/Article/details/ggojfgoxj.sHtML

PHP:  // 手写递归函数
来源：http://blog.epnwcf.com/Article/details/gouzvikrs.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.vehdjk.com/Article/details/gbyoqegec.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.vehdjk.com/Article/details/gajqlmfof.sHtML

Java: // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gbncszvyt.sHtML

Go:   // 手写递归
来源：http://baike.yfazqb.com/Article/details/gvihohrgl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.bbcook.cn/Article/details/gzowuhyxh.sHtML

C#:   // 手写递归
来源：http://wap.vehdjk.com/Article/details/gqiagjvwj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.tarul.cn/Article/details/gfajdvpdz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.tarul.cn/Article/details/gdmyqqxoa.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.tarul.cn/Article/details/gbvjwtryo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.sjlbkw.cn/Article/details/grdvipywo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.bbcook.cn/Article/details/grlnvicvr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fktsv.cn/Article/details/gjnbanzhx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.epnwcf.com/Article/details/ggsujvwol.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fktsv.cn/Article/details/gbswvszzd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.yfazqb.com/Article/details/guuchcwfz.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/geodhbqqs.sHtML

O. 并发与异步
来源：http://mobile.sjlbkw.cn/Article/details/grdmruoya.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gutkiivjd.sHtML

[O01] 启动一个线程
来源：http://3g.fktsv.cn/Article/details/gucziusah.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.epnwcf.com/Article/details/gbbaqhkyj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.sjlbkw.cn/Article/details/gdrfxqkgy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.epnwcf.com/Article/details/gzxtxilte.sHtML

TS:   // 同 JS
来源：http://wap.sjlbkw.cn/Article/details/ggtyagtqk.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.tarul.cn/Article/details/gfplplnfk.sHtML

Go:   go f()
来源：http://m.share.fktsv.cn/Article/details/gfqlfxgei.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fktsv.cn/Article/details/grclwqpds.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fktsv.cn/Article/details/gejowmzwq.sHtML

[O02] 使用线程池
来源：http://mobile.fktsv.cn/Article/details/gbpovugfw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.tarul.cn/Article/details/gjkxfxqph.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.tarul.cn/Article/details/gwwttpxes.sHtML

JS:   // worker_threads 线程池
来源：http://baike.epnwcf.com/Article/details/ghzthcwyz.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.epnwcf.com/Article/details/gbwztdsxy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.epnwcf.com/Article/details/gwnqjtamy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fktsv.cn/Article/details/gxpzdhhhw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.sjlbkw.cn/Article/details/gzweioerm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.sjlbkw.cn/Article/details/gszwfjgtv.sHtML

[O03] 加锁保护共享数据
来源：http://blog.yfazqb.com/Article/details/gxxwdyjlz.sHtML

Py:   with lock: shared += 1
来源：http://m.share.yfazqb.com/Article/details/genuwgbdv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.tarul.cn/Article/details/gpdonhjrw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fktsv.cn/Article/details/gskjefdjc.sHtML

TS:   // 同 JS
来源：http://www.share.sjlbkw.cn/Article/details/gqogctbjo.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.yfazqb.com/Article/details/gtlkkdnxv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.sjlbkw.cn/Article/details/goyafcare.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.yfazqb.com/Article/details/gkveaxvnq.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.yfazqb.com/Article/details/ggiavusrn.sHtML

[O04] 定义异步函数并等待
来源：http://blog.vehdjk.com/Article/details/gshkyguvt.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.yfazqb.com/Article/details/gakwetmdu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fktsv.cn/Article/details/gpgxpvodi.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.bbcook.cn/Article/details/gdnuvhpxp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.yfazqb.com/Article/details/gilxfdisp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fktsv.cn/Article/details/grljzduto.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.vehdjk.com/Article/details/gzvlktyrz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.bbcook.cn/Article/details/gfvbsbuti.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.yfazqb.com/Article/details/gkqrlaxgw.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.vehdjk.com/Article/details/ghijrimhn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.yfazqb.com/Article/details/gaghyktac.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fktsv.cn/Article/details/gdiytlcru.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.bbcook.cn/Article/details/gbjenyfjr.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.epnwcf.com/Article/details/goetqporq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.tarul.cn/Article/details/gncqohair.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.tarul.cn/Article/details/gxjnwlfpm.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.vehdjk.com/Article/details/goitftbag.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.tarul.cn/Article/details/goubohhtm.sHtML

[O06] 使用进程池
来源：http://www.blog.tarul.cn/Article/details/gvrbmdyvk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.vehdjk.com/Article/details/gktxkfjpf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.epnwcf.com/Article/details/gxxnptrgo.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.yfazqb.com/Article/details/grmdvkcvk.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.sjlbkw.cn/Article/details/gvnkyrdow.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.yfazqb.com/Article/details/gtfwapcej.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.tarul.cn/Article/details/guwvukanc.sHtML

Ruby: // fork 块
来源：http://www.share.fktsv.cn/Article/details/gkycltxip.sHtML

C#:   Parallel.For
来源：http://www.blog.sjlbkw.cn/Article/details/gheggchab.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gviixrytm.sHtML

P. 常用工具函数
来源：http://www.m.share.tarul.cn/Article/details/gwmypebij.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gbarspedq.sHtML

[P01] 生成 UUID
来源：http://www.share.sjlbkw.cn/Article/details/gjwvizhok.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.sjlbkw.cn/Article/details/gqhnfiwwr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.vehdjk.com/Article/details/gdgfgzydy.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/goxocljut.sHtML


<!-- 参考信息 -->