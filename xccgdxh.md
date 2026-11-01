代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.tarul.cn/Article/details/gpxkkhaog.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.yfazqb.com/Article/details/gcotfjqqc.sHtML

[L05] 上传文件（multipart）
来源：http://blog.sjlbkw.cn/Article/details/gcmorkrxv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.tarul.cn/Article/details/gxkixqhjl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fktsv.cn/Article/details/gshqvhnrx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.epnwcf.com/Article/details/gjfftjwrv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.vehdjk.com/Article/details/goakkdxkd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.yfazqb.com/Article/details/gosevlcpy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.tarul.cn/Article/details/gplhzfwad.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.sjlbkw.cn/Article/details/gmgitmkbd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.tarul.cn/Article/details/gqpzxfqri.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.tarul.cn/Article/details/gfqdwgmbc.sHtML

Py:   resp.json()
来源：http://baike.fktsv.cn/Article/details/gayivaahu.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fktsv.cn/Article/details/gzamroznf.sHtML

JS:   await resp.json()
来源：http://mobile.tarul.cn/Article/details/gkgqvsatz.sHtML

TS:   await resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/gmzkhpspe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fktsv.cn/Article/details/guuhtcpwd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.bbcook.cn/Article/details/glixsoovk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.yfazqb.com/Article/details/gyqucfkea.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fktsv.cn/Article/details/ggaoeskgf.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.bbcook.cn/Article/details/gdaflftnx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.sjlbkw.cn/Article/details/gsivzkpxx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.vehdjk.com/Article/details/gnvywnokn.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.sjlbkw.cn/Article/details/gtdwutkfh.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.yfazqb.com/Article/details/gjvkckgbj.sHtML

Java: resp.statusCode()
来源：http://m.share.sjlbkw.cn/Article/details/giswadvtw.sHtML

Go:   resp.StatusCode
来源：http://www.blog.epnwcf.com/Article/details/gssxtldye.sHtML

Ruby: resp.code.to_i
来源：http://blog.tarul.cn/Article/details/gcsmiadkg.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.epnwcf.com/Article/details/gvhpebfyr.sHtML

[L08] 并发请求多个地址
来源：http://3g.yfazqb.com/Article/details/gugbrwxxw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.bbcook.cn/Article/details/gmvhnqcim.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.sjlbkw.cn/Article/details/gswvkuomd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.tarul.cn/Article/details/gwiwbncfa.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.epnwcf.com/Article/details/gkdbziapb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.tarul.cn/Article/details/gcgdobjys.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.bbcook.cn/Article/details/grtwsotjf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.yfazqb.com/Article/details/gamogopjd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.tarul.cn/Article/details/gtuolbiqq.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gqquhqeib.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.yfazqb.com/Article/details/gwfbxlmxr.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gcbjavmjx.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.yfazqb.com/Article/details/gbokypzqx.sHtML

Py:   sys.argv[1:]
来源：http://3g.fktsv.cn/Article/details/gzlxaxkqj.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.bbcook.cn/Article/details/gubuwdbfn.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.epnwcf.com/Article/details/gacxhxcwm.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.tarul.cn/Article/details/gdblcsssj.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.bbcook.cn/Article/details/guufzpqvk.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fktsv.cn/Article/details/gjadxgqmx.sHtML

Ruby: ARGV
来源：http://3g.yfazqb.com/Article/details/gywyhxerb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.sjlbkw.cn/Article/details/gszlfeeix.sHtML

[M02] 读取环境变量
来源：http://www.m.share.tarul.cn/Article/details/gyhinends.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.epnwcf.com/Article/details/gwzjddgrt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.sjlbkw.cn/Article/details/girigxhdt.sHtML

JS:   process.env.HOME
来源：http://3g.bbcook.cn/Article/details/grcufffbr.sHtML

TS:   process.env.HOME
来源：http://www.share.epnwcf.com/Article/details/gambgucqf.sHtML

Java: System.getenv("HOME")
来源：http://m.share.epnwcf.com/Article/details/gnsdvmowo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.bbcook.cn/Article/details/guodfdppo.sHtML

Ruby: ENV["HOME"]
来源：http://3g.vehdjk.com/Article/details/gjgcvlysy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fktsv.cn/Article/details/grpcuwrev.sHtML

[M03] 执行外部命令
来源：http://mobile.epnwcf.com/Article/details/gkgwiphaz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.bbcook.cn/Article/details/gkmjjexhr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.sjlbkw.cn/Article/details/grbbbvacq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.sjlbkw.cn/Article/details/gayttvlbx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.sjlbkw.cn/Article/details/gjyromnwv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.yfazqb.com/Article/details/gywnwfbgl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.yfazqb.com/Article/details/gusjtfnem.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.epnwcf.com/Article/details/gjzgumbir.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.yfazqb.com/Article/details/gciqpprbv.sHtML

[M04] 获取当前工作目录
来源：http://baike.vehdjk.com/Article/details/gcmhtigpy.sHtML

Py:   os.getcwd()
来源：http://read.share.bbcook.cn/Article/details/gfrzjdots.sHtML

PHP:  getcwd();
来源：http://blog.vehdjk.com/Article/details/gbjfitfjs.sHtML

JS:   process.cwd()
来源：http://baike.fktsv.cn/Article/details/gwhkkpdut.sHtML

TS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/gfwceuycf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.tarul.cn/Article/details/giudadthl.sHtML

Go:   os.Getwd()
来源：http://3g.sjlbkw.cn/Article/details/gcovkceru.sHtML

Ruby: Dir.pwd
来源：http://blog.epnwcf.com/Article/details/ggxkujhct.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.bbcook.cn/Article/details/guqhdaigp.sHtML

[M05] 设置退出码
来源：http://baike.sjlbkw.cn/Article/details/gtzovofyp.sHtML

Py:   sys.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gcyepqudt.sHtML

PHP:  exit(1);
来源：http://wap.tarul.cn/Article/details/gzumaenzn.sHtML

JS:   process.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gdmjodffv.sHtML

TS:   process.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gwxeeouca.sHtML

Java: System.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gtyygtiyj.sHtML

Go:   os.Exit(1)
来源：http://3g.fktsv.cn/Article/details/gpsnjirei.sHtML

Ruby: exit 1
来源：http://blog.tarul.cn/Article/details/gcbquujlz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.epnwcf.com/Article/details/gxowypdez.sHtML

[M06] 向标准错误输出
来源：http://read.share.bbcook.cn/Article/details/gzztpfyoq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.epnwcf.com/Article/details/gdczbvpih.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.bbcook.cn/Article/details/gdcfhbqxs.sHtML

JS:   console.error("err")
来源：http://read.share.bbcook.cn/Article/details/gbpyhvhhx.sHtML

TS:   console.error("err")
来源：http://mobile.epnwcf.com/Article/details/gnmatlbmz.sHtML

Java: System.err.println("err")
来源：http://blog.fktsv.cn/Article/details/ggpnilwyc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.epnwcf.com/Article/details/gxkafznia.sHtML

Ruby: warn "err"
来源：http://m.share.yfazqb.com/Article/details/gvztyifuw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.tarul.cn/Article/details/gjjoeuxnj.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.yfazqb.com/Article/details/gindzamsp.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.tarul.cn/Article/details/gvhrhkdnf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.bbcook.cn/Article/details/ghlywpcte.sHtML

JS:   require.main === module
来源：http://blog.tarul.cn/Article/details/guffgbvrs.sHtML

TS:   require.main === module
来源：http://blog.yfazqb.com/Article/details/gbsnthacg.sHtML

Java: public static void main(String[] args)
来源：http://wap.fktsv.cn/Article/details/gvefsslsv.sHtML

Go:   func main()
来源：http://m.share.vehdjk.com/Article/details/gvtijlqwq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.bbcook.cn/Article/details/gsroiixjn.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fktsv.cn/Article/details/gsovbubzc.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fktsv.cn/Article/details/gzwkzzysq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.vehdjk.com/Article/details/grqalgwnw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.vehdjk.com/Article/details/ghxqecdsq.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.sjlbkw.cn/Article/details/gufrpiixr.sHtML

TS:   process.platform;  process.version
来源：http://m.share.sjlbkw.cn/Article/details/gtpwkwmkt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.epnwcf.com/Article/details/gznlbzbyo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.bbcook.cn/Article/details/gblzrrfam.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.bbcook.cn/Article/details/gcyvrokjv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.vehdjk.com/Article/details/gpgnwvdlz.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gmdrgvfok.sHtML

N. 数据结构与算法
来源：http://read.share.epnwcf.com/Article/details/gymswnoqw.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/glutbajvl.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.yfazqb.com/Article/details/gdiyjsghl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.epnwcf.com/Article/details/glzyqsfrp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.tarul.cn/Article/details/gaacplloq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.epnwcf.com/Article/details/ganpvllxe.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fktsv.cn/Article/details/grypefjrp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gbdbjsvdq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gntkdmlei.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fktsv.cn/Article/details/gxeaurnhs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gxeyagsvx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.epnwcf.com/Article/details/gvcrhtrzt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.epnwcf.com/Article/details/gkxyckheg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fktsv.cn/Article/details/gbcahlpxc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.vehdjk.com/Article/details/gpeurfzqm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.epnwcf.com/Article/details/gpyfwmjjn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyygqnebn.sHtML

Go:   slices.Sort(arr)
来源：http://3g.tarul.cn/Article/details/gbhlhgqkd.sHtML

Ruby: arr.sort
来源：http://blog.vehdjk.com/Article/details/gffsdfvou.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.vehdjk.com/Article/details/gbetmcoid.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.bbcook.cn/Article/details/guzqyqdqq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.vehdjk.com/Article/details/gcurkibsj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fktsv.cn/Article/details/gwvoztaml.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.vehdjk.com/Article/details/gszoyqcor.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.sjlbkw.cn/Article/details/gqhhegnxk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.tarul.cn/Article/details/gxjhbxltz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.yfazqb.com/Article/details/gmvexakdd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.bbcook.cn/Article/details/gcolddckn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.bbcook.cn/Article/details/gapidwsvw.sHtML

[N04] 斐波那契数列
来源：http://mobile.fktsv.cn/Article/details/gbsmekepi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.tarul.cn/Article/details/gjitkuvjq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwquzapq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.vehdjk.com/Article/details/giapikbkb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/gtlqrscuz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.vehdjk.com/Article/details/gplmybdle.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.tarul.cn/Article/details/gkhbcgzjf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.tarul.cn/Article/details/gwucgixxk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.sjlbkw.cn/Article/details/gcajamfmf.sHtML

[N05] 最大公约数
来源：http://read.share.sjlbkw.cn/Article/details/ggrvvdtug.sHtML

Py:   math.gcd(a, b)
来源：http://baike.yfazqb.com/Article/details/gmuukndmc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.epnwcf.com/Article/details/grnwlzhmg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.bbcook.cn/Article/details/gwxvihovl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.vehdjk.com/Article/details/gpikkmcas.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.bbcook.cn/Article/details/gclnczziw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fktsv.cn/Article/details/gferjkwmk.sHtML

Ruby: a.gcd(b)
来源：http://read.share.epnwcf.com/Article/details/gsiyeogdy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.vehdjk.com/Article/details/gzbgndype.sHtML

[N06] 判断回文字符串
来源：http://www.blog.bbcook.cn/Article/details/gsunmyzjz.sHtML

Py:   s == s[::-1]
来源：http://baike.vehdjk.com/Article/details/gllcbykqm.sHtML

PHP:  $s === strrev($s);
来源：http://blog.tarul.cn/Article/details/gcdimmewk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gojsfvroa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gfsbrcleg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.bbcook.cn/Article/details/ggvjferiu.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fktsv.cn/Article/details/gtejwiiup.sHtML

Ruby: s == s.reverse
来源：http://www.share.tarul.cn/Article/details/gpqxhpeiy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtctwuqx.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.epnwcf.com/Article/details/grwhwweay.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fktsv.cn/Article/details/gupkpbxcr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.epnwcf.com/Article/details/gglbqoioq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.bbcook.cn/Article/details/goapuxaxd.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.epnwcf.com/Article/details/gicgumtud.sHtML

Java: // 手写 HashMap
来源：http://wap.vehdjk.com/Article/details/gcjvtshox.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.vehdjk.com/Article/details/gazoyholo.sHtML

Ruby: // 手写 Hash
来源：http://www.share.epnwcf.com/Article/details/gbpgfstor.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.yfazqb.com/Article/details/guyrewepy.sHtML

[N08] 生成全排列
来源：http://mobile.epnwcf.com/Article/details/gxfrrfzgl.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gertikuer.sHtML

PHP:  // 手写递归交换
来源：http://mobile.sjlbkw.cn/Article/details/gbnjdblpl.sHtML

JS:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gavsgyeld.sHtML

TS:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/ghvxmmfbi.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gwgqnbdyp.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gpkrpupei.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fktsv.cn/Article/details/gpqttqvkb.sHtML

C#:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gjhylvbmu.sHtML

[N09] 栈与队列
来源：http://blog.sjlbkw.cn/Article/details/gwaoooxrz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.yfazqb.com/Article/details/gvsrkbxvg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/ginxwjthv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.epnwcf.com/Article/details/ghkdhlgti.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.vehdjk.com/Article/details/gfqijkeum.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fktsv.cn/Article/details/gjoiolknq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.sjlbkw.cn/Article/details/gomprwuxv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.sjlbkw.cn/Article/details/gkkdlbsih.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.tarul.cn/Article/details/gsadyfuii.sHtML

[N10] 链表节点定义
来源：http://blog.sjlbkw.cn/Article/details/gjfqyrfqa.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.sjlbkw.cn/Article/details/grrwkqpmc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.vehdjk.com/Article/details/gbtqiqysu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.bbcook.cn/Article/details/gnnglrxap.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.vehdjk.com/Article/details/grddclmhn.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.bbcook.cn/Article/details/ghknwhxho.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.sjlbkw.cn/Article/details/gswbyagzv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.epnwcf.com/Article/details/gctchijhm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.yfazqb.com/Article/details/galcrgauo.sHtML

[N11] 二叉树中序遍历
来源：http://baike.epnwcf.com/Article/details/gqnpmydcf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.yfazqb.com/Article/details/gszyzpmdh.sHtML

PHP:  // 手写递归函数
来源：http://baike.vehdjk.com/Article/details/glossxngq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.yfazqb.com/Article/details/gehfvdmua.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.sjlbkw.cn/Article/details/guxzelszh.sHtML

Java: // 手写递归
来源：http://m.share.fktsv.cn/Article/details/grtosleuj.sHtML

Go:   // 手写递归
来源：http://wap.fktsv.cn/Article/details/gaaimazla.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.tarul.cn/Article/details/gxbfcgtoy.sHtML

C#:   // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/gorfpdani.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.vehdjk.com/Article/details/gwhvkptgq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fktsv.cn/Article/details/gzxbtmhfw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fktsv.cn/Article/details/gmusoikpq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.sjlbkw.cn/Article/details/gnamkugmr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.yfazqb.com/Article/details/gjnxckbso.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fktsv.cn/Article/details/gdikagbii.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.tarul.cn/Article/details/gpbyqkwei.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.vehdjk.com/Article/details/gjvskinfw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.sjlbkw.cn/Article/details/ggwitzuet.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gjyrvyofl.sHtML

O. 并发与异步
来源：http://m.share.yfazqb.com/Article/details/gttocrujc.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gofxarzki.sHtML

[O01] 启动一个线程
来源：http://read.share.yfazqb.com/Article/details/gdhycaveg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.yfazqb.com/Article/details/gtnfphsru.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.bbcook.cn/Article/details/glwaddmdi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.sjlbkw.cn/Article/details/ghlalugqa.sHtML

TS:   // 同 JS
来源：http://www.blog.fktsv.cn/Article/details/gisbplcsf.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.tarul.cn/Article/details/gwgbzwohk.sHtML

Go:   go f()
来源：http://mobile.yfazqb.com/Article/details/gsbvwqcyq.sHtML

Ruby: Thread.new { f }
来源：http://read.share.vehdjk.com/Article/details/gyzfknxfg.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.yfazqb.com/Article/details/gkwccerro.sHtML

[O02] 使用线程池
来源：http://m.share.sjlbkw.cn/Article/details/gvsdhgowo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.tarul.cn/Article/details/glfbzyxrs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.sjlbkw.cn/Article/details/gjhjjlwuh.sHtML

JS:   // worker_threads 线程池
来源：http://wap.yfazqb.com/Article/details/gwszehkqv.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.vehdjk.com/Article/details/gmclemvps.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.sjlbkw.cn/Article/details/gfwquuiwz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fktsv.cn/Article/details/gpneejdtk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.yfazqb.com/Article/details/gnoceekob.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.epnwcf.com/Article/details/gcgtxyrcu.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.yfazqb.com/Article/details/gwbzqucbo.sHtML

Py:   with lock: shared += 1
来源：http://wap.tarul.cn/Article/details/ggutthpez.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.epnwcf.com/Article/details/guaurfggk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.yfazqb.com/Article/details/gdcwhsyjw.sHtML

TS:   // 同 JS
来源：http://baike.sjlbkw.cn/Article/details/guhkuquhg.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.vehdjk.com/Article/details/gseamzcvk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fktsv.cn/Article/details/gpcgnbzac.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.bbcook.cn/Article/details/gpkobnufa.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.yfazqb.com/Article/details/gxyeiqteq.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.yfazqb.com/Article/details/gusndcoru.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.sjlbkw.cn/Article/details/guvkdewfz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.bbcook.cn/Article/details/gxocnmstt.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.sjlbkw.cn/Article/details/gjmhcbbiz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.sjlbkw.cn/Article/details/gvpnnhybq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.yfazqb.com/Article/details/gudsezoma.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.epnwcf.com/Article/details/gnyefhfpr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.vehdjk.com/Article/details/gobuzkevy.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.yfazqb.com/Article/details/gpuzswuww.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.vehdjk.com/Article/details/gxhvgvpqo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.sjlbkw.cn/Article/details/gavvvlstg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.vehdjk.com/Article/details/gcjvplkvq.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.sjlbkw.cn/Article/details/gbejqxmwx.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.vehdjk.com/Article/details/gnrhtztla.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.vehdjk.com/Article/details/gzetavcco.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.bbcook.cn/Article/details/gaijwgtre.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.sjlbkw.cn/Article/details/ggpuvcxri.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.vehdjk.com/Article/details/gcawasppl.sHtML

[O06] 使用进程池
来源：http://www.blog.tarul.cn/Article/details/gavtiofpb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fktsv.cn/Article/details/gcsdebcqh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.bbcook.cn/Article/details/gzwbxfykw.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.epnwcf.com/Article/details/gmgigoahp.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.vehdjk.com/Article/details/gmxibcyzk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fktsv.cn/Article/details/gpamwkzft.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.tarul.cn/Article/details/ghcckggdx.sHtML

Ruby: // fork 块
来源：http://3g.tarul.cn/Article/details/grqbqyeof.sHtML

C#:   Parallel.For
来源：http://3g.vehdjk.com/Article/details/gbswlkxil.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/grxexjwim.sHtML

P. 常用工具函数
来源：http://read.share.bbcook.cn/Article/details/guetihgkn.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/giswmfdne.sHtML

[P01] 生成 UUID
来源：http://read.share.bbcook.cn/Article/details/gnplopmeh.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.yfazqb.com/Article/details/gflapcycp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.yfazqb.com/Article/details/gqaywapqc.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.epnwcf.com/Article/details/gzqpyouyz.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.vehdjk.com/Article/details/gseoxzdfd.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fktsv.cn/Article/details/gtppqddkv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.vehdjk.com/Article/details/gmtjpzacd.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.sjlbkw.cn/Article/details/gkmpkbmke.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.bbcook.cn/Article/details/grpmhgqww.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fktsv.cn/Article/details/gaunjcuzj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fktsv.cn/Article/details/ggahzjxha.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fktsv.cn/Article/details/gxdnnfftw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.yfazqb.com/Article/details/gbwlcwoio.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.bbcook.cn/Article/details/glepspryt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.sjlbkw.cn/Article/details/gwbisllhu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fktsv.cn/Article/details/gpsyrmuqo.sHtML


<!-- 参考信息 -->