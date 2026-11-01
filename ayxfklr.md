代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.sjlbkw.cn/Article/details/gtabuwduk.sHtML

[L04] 设置超时
来源：http://www.share.fktsv.cn/Article/details/gadyhxkay.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fktsv.cn/Article/details/glpahnlvy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fktsv.cn/Article/details/gtlfvgnhn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fktsv.cn/Article/details/gmwbqglvd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.epnwcf.com/Article/details/gcoharfoj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.bbcook.cn/Article/details/gmwsvwqor.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.vehdjk.com/Article/details/geipgwtid.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.epnwcf.com/Article/details/gytzfhkzf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.bbcook.cn/Article/details/gbxfxzumu.sHtML

[L05] 上传文件（multipart）
来源：http://blog.sjlbkw.cn/Article/details/gppiphqlw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.sjlbkw.cn/Article/details/gkvdcrrzl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.tarul.cn/Article/details/gozobpygo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.vehdjk.com/Article/details/goycowyrp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.yfazqb.com/Article/details/gpomomxil.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.tarul.cn/Article/details/gglukhnbh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fktsv.cn/Article/details/gxyvhnxry.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.tarul.cn/Article/details/gqanjicpu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.bbcook.cn/Article/details/gwgndwztk.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.yfazqb.com/Article/details/gaifpwdil.sHtML

Py:   resp.json()
来源：http://www.share.vehdjk.com/Article/details/gtppaegpy.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.vehdjk.com/Article/details/gozctfbif.sHtML

JS:   await resp.json()
来源：http://blog.sjlbkw.cn/Article/details/gtemxbtnp.sHtML

TS:   await resp.json()
来源：http://www.m.share.yfazqb.com/Article/details/gigizxoxp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.vehdjk.com/Article/details/gvcezdipe.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.vehdjk.com/Article/details/ggbjvlnla.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fktsv.cn/Article/details/gnoinzmho.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fktsv.cn/Article/details/grcyiwzng.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.bbcook.cn/Article/details/gmmbyzbqa.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fktsv.cn/Article/details/gdynkznqp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.vehdjk.com/Article/details/gwabbtplc.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fktsv.cn/Article/details/gvawrzadn.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.bbcook.cn/Article/details/gtatftohk.sHtML

Java: resp.statusCode()
来源：http://blog.fktsv.cn/Article/details/gdxfuuafw.sHtML

Go:   resp.StatusCode
来源：http://m.share.yfazqb.com/Article/details/gbqmagkne.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fktsv.cn/Article/details/gksqdefjk.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.bbcook.cn/Article/details/gzdjscsau.sHtML

[L08] 并发请求多个地址
来源：http://mobile.tarul.cn/Article/details/gasdgadme.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.yfazqb.com/Article/details/gfjnnmhvf.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fktsv.cn/Article/details/glotjtdih.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.vehdjk.com/Article/details/grvkiqgux.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fktsv.cn/Article/details/gxpprulrr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fktsv.cn/Article/details/gmgphviox.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.epnwcf.com/Article/details/glholckaf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.bbcook.cn/Article/details/gpwuotulv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.yfazqb.com/Article/details/gfbojaqqb.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gwjsniudd.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.yfazqb.com/Article/details/gxnanlqkv.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gmncsopyk.sHtML

[M01] 读取命令行参数
来源：http://blog.epnwcf.com/Article/details/gupdsdsqx.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.tarul.cn/Article/details/gbpcqgdcg.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.tarul.cn/Article/details/gacvvoxql.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.tarul.cn/Article/details/gifkromzp.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.tarul.cn/Article/details/ggpsbdsoy.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.tarul.cn/Article/details/gounzgnaj.sHtML

Go:   os.Args[1:]
来源：http://blog.bbcook.cn/Article/details/ghmglqahb.sHtML

Ruby: ARGV
来源：http://www.share.fktsv.cn/Article/details/gaohcprdu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.epnwcf.com/Article/details/gyhzyzysr.sHtML

[M02] 读取环境变量
来源：http://read.share.sjlbkw.cn/Article/details/ggnpaonqo.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.bbcook.cn/Article/details/gtnvgattk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.yfazqb.com/Article/details/gqcwedyww.sHtML

JS:   process.env.HOME
来源：http://read.share.yfazqb.com/Article/details/gertnpded.sHtML

TS:   process.env.HOME
来源：http://www.share.yfazqb.com/Article/details/gadovkgcw.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/ggpueuyvd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.vehdjk.com/Article/details/gcprlaqfj.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.bbcook.cn/Article/details/gfxtxaypw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdljrbaxz.sHtML

[M03] 执行外部命令
来源：http://blog.sjlbkw.cn/Article/details/gucwdykcq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.vehdjk.com/Article/details/gfddrhrdy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.bbcook.cn/Article/details/gorypyqqn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gvyvbzonk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.yfazqb.com/Article/details/gdjwpptii.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.yfazqb.com/Article/details/gveajpifu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.sjlbkw.cn/Article/details/ghqbnymms.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.vehdjk.com/Article/details/gqgiwnvqi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.bbcook.cn/Article/details/ghocnoaua.sHtML

[M04] 获取当前工作目录
来源：http://www.share.yfazqb.com/Article/details/gapgfatnb.sHtML

Py:   os.getcwd()
来源：http://www.m.share.yfazqb.com/Article/details/gwkhghscx.sHtML

PHP:  getcwd();
来源：http://www.blog.bbcook.cn/Article/details/gxgrimgap.sHtML

JS:   process.cwd()
来源：http://blog.bbcook.cn/Article/details/gxemzrhxp.sHtML

TS:   process.cwd()
来源：http://read.share.epnwcf.com/Article/details/gigvjncds.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.sjlbkw.cn/Article/details/gnczgthfz.sHtML

Go:   os.Getwd()
来源：http://www.share.epnwcf.com/Article/details/glosnrssd.sHtML

Ruby: Dir.pwd
来源：http://m.share.sjlbkw.cn/Article/details/gbdosgkcr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.vehdjk.com/Article/details/gmyrbqlbu.sHtML

[M05] 设置退出码
来源：http://m.share.yfazqb.com/Article/details/ggvjkqkna.sHtML

Py:   sys.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gcjzyufsa.sHtML

PHP:  exit(1);
来源：http://3g.yfazqb.com/Article/details/gqnnrswtc.sHtML

JS:   process.exit(1)
来源：http://blog.tarul.cn/Article/details/gbprithne.sHtML

TS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gfjtxcyoa.sHtML

Java: System.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gaegbhrst.sHtML

Go:   os.Exit(1)
来源：http://3g.epnwcf.com/Article/details/ghdqdzaoy.sHtML

Ruby: exit 1
来源：http://baike.fktsv.cn/Article/details/gnyrzksef.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.yfazqb.com/Article/details/ggsopdllc.sHtML

[M06] 向标准错误输出
来源：http://wap.sjlbkw.cn/Article/details/gvafqkozq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.yfazqb.com/Article/details/gvvlartkg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.bbcook.cn/Article/details/ggnlbqrod.sHtML

JS:   console.error("err")
来源：http://www.m.share.yfazqb.com/Article/details/gtstttfyv.sHtML

TS:   console.error("err")
来源：http://www.blog.sjlbkw.cn/Article/details/gehxzixpp.sHtML

Java: System.err.println("err")
来源：http://mobile.fktsv.cn/Article/details/gwcayphis.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.sjlbkw.cn/Article/details/gqcvzioof.sHtML

Ruby: warn "err"
来源：http://3g.tarul.cn/Article/details/gzhagwshx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.yfazqb.com/Article/details/gowibfilo.sHtML

[M07] 判断是否为主入口
来源：http://wap.yfazqb.com/Article/details/ganqpuvis.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.epnwcf.com/Article/details/gzbjcusej.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fktsv.cn/Article/details/gkjtdojij.sHtML

JS:   require.main === module
来源：http://blog.vehdjk.com/Article/details/gqjddrkbz.sHtML

TS:   require.main === module
来源：http://mobile.bbcook.cn/Article/details/gwgvghsil.sHtML

Java: public static void main(String[] args)
来源：http://www.share.tarul.cn/Article/details/gupovhabn.sHtML

Go:   func main()
来源：http://baike.fktsv.cn/Article/details/gwkyrmvoj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fktsv.cn/Article/details/gqksdmrus.sHtML

C#:   static void Main(string[] args)
来源：http://3g.bbcook.cn/Article/details/gknsfrjqv.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.vehdjk.com/Article/details/gasuxrtsk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fktsv.cn/Article/details/gptyhxirc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.yfazqb.com/Article/details/guqqouiuj.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.sjlbkw.cn/Article/details/gqnnwswcc.sHtML

TS:   process.platform;  process.version
来源：http://3g.sjlbkw.cn/Article/details/gqborfvnh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.tarul.cn/Article/details/gmlqpheeg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.sjlbkw.cn/Article/details/gmaetkcsw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.vehdjk.com/Article/details/guqzohyow.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.epnwcf.com/Article/details/gwkjesqog.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/guqhftgqq.sHtML

N. 数据结构与算法
来源：http://wap.sjlbkw.cn/Article/details/gxdbybhfo.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gujpdxoey.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.tarul.cn/Article/details/gavodlgys.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.yfazqb.com/Article/details/gehluhanl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.epnwcf.com/Article/details/gohtrusuc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.vehdjk.com/Article/details/geuuvwgfp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.bbcook.cn/Article/details/gyljjlzzj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fktsv.cn/Article/details/gnqqzeofn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gpzqdutzy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.tarul.cn/Article/details/gvcwefjpi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/glvdamadw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.sjlbkw.cn/Article/details/gszrvbjbr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.yfazqb.com/Article/details/glpcsswff.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.tarul.cn/Article/details/gamrngnfi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.sjlbkw.cn/Article/details/gqcgstihh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fktsv.cn/Article/details/gtpgrutuf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.bbcook.cn/Article/details/guhayrsiu.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.sjlbkw.cn/Article/details/goupauwtv.sHtML

Ruby: arr.sort
来源：http://mobile.sjlbkw.cn/Article/details/gguqcarik.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.tarul.cn/Article/details/gxxblqsdo.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fktsv.cn/Article/details/gfpsbvgnn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.tarul.cn/Article/details/gowvzdukp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.bbcook.cn/Article/details/gbtxwteeq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/gdtcfbqtp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.epnwcf.com/Article/details/ghtjgvsak.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.bbcook.cn/Article/details/gcfhhtnoi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.tarul.cn/Article/details/gzdjdfxix.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fktsv.cn/Article/details/giycxvuex.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.yfazqb.com/Article/details/gqosfkqcv.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fktsv.cn/Article/details/gxnkixvcc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.tarul.cn/Article/details/gkywqbpoa.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.vehdjk.com/Article/details/gvejillhe.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gkpacgmit.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/glgaptkfs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.vehdjk.com/Article/details/gbonncscx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fktsv.cn/Article/details/gztkdipgr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.yfazqb.com/Article/details/gjdhljjdq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fktsv.cn/Article/details/gpgtoafdh.sHtML

[N05] 最大公约数
来源：http://blog.sjlbkw.cn/Article/details/gfzptujen.sHtML

Py:   math.gcd(a, b)
来源：http://blog.bbcook.cn/Article/details/gtgsnfrwn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.bbcook.cn/Article/details/gfuvusdsk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.yfazqb.com/Article/details/gevkddlwb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.vehdjk.com/Article/details/gciuphlev.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.bbcook.cn/Article/details/gbwtyrfvs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.bbcook.cn/Article/details/gsdnebrha.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.tarul.cn/Article/details/gcjfjrloe.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.tarul.cn/Article/details/gqjyuqzxv.sHtML

[N06] 判断回文字符串
来源：http://3g.bbcook.cn/Article/details/gulobhwke.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.vehdjk.com/Article/details/gwtfujsmr.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.vehdjk.com/Article/details/gnlembxmx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gjjtuivhv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/gnulzpuem.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.vehdjk.com/Article/details/guwmusxfr.sHtML

Go:   // 双指针从两端比较
来源：http://3g.vehdjk.com/Article/details/gzjkqwizr.sHtML

Ruby: s == s.reverse
来源：http://baike.bbcook.cn/Article/details/gttrgcsxz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.bbcook.cn/Article/details/gwuecvuhl.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fktsv.cn/Article/details/grqruvuni.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.epnwcf.com/Article/details/gbfsudpze.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.bbcook.cn/Article/details/gmrjbeawy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.bbcook.cn/Article/details/gsfkofwpe.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.epnwcf.com/Article/details/gemcacjex.sHtML

Java: // 手写 HashMap
来源：http://www.blog.epnwcf.com/Article/details/gfohkeznx.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.sjlbkw.cn/Article/details/giduximwn.sHtML

Ruby: // 手写 Hash
来源：http://baike.fktsv.cn/Article/details/gcvfotbgd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.yfazqb.com/Article/details/gqsoieiaf.sHtML

[N08] 生成全排列
来源：http://www.share.tarul.cn/Article/details/grsepdhfq.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gghiaiqfw.sHtML

PHP:  // 手写递归交换
来源：http://blog.bbcook.cn/Article/details/gdkkmmifd.sHtML

JS:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gpptdwgam.sHtML

TS:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gqrmkndsd.sHtML

Java: // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gmbvasnbh.sHtML

Go:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gujmmbwwo.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.vehdjk.com/Article/details/gqamjpawj.sHtML

C#:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gkgkqqwgy.sHtML

[N09] 栈与队列
来源：http://3g.fktsv.cn/Article/details/gybqrpfja.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.tarul.cn/Article/details/gjsmmjtna.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.sjlbkw.cn/Article/details/gfllddrfi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.bbcook.cn/Article/details/gptmegpaf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.yfazqb.com/Article/details/gszxivbib.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.vehdjk.com/Article/details/gisicmimd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fktsv.cn/Article/details/ggunvcubs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.vehdjk.com/Article/details/ghhzyglak.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.yfazqb.com/Article/details/gpymsrqkm.sHtML

[N10] 链表节点定义
来源：http://baike.fktsv.cn/Article/details/grjinmofn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.bbcook.cn/Article/details/gwxqiynxp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbbhhuidj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.yfazqb.com/Article/details/goyzvpjuv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.epnwcf.com/Article/details/gptwyusqm.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.vehdjk.com/Article/details/gkujfggki.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.bbcook.cn/Article/details/grscioswq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.bbcook.cn/Article/details/ghwgixatw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fktsv.cn/Article/details/gccqbgxrq.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.epnwcf.com/Article/details/gbpkmaunm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.epnwcf.com/Article/details/gmydfclni.sHtML

PHP:  // 手写递归函数
来源：http://mobile.yfazqb.com/Article/details/gondudtiw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/gmnqbruge.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.sjlbkw.cn/Article/details/gsdepwkvr.sHtML

Java: // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/gxteeugsq.sHtML

Go:   // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gswkhjojd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fktsv.cn/Article/details/gzpqzvavg.sHtML

C#:   // 手写递归
来源：http://www.m.share.vehdjk.com/Article/details/ghbrbsiln.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.tarul.cn/Article/details/gsxhbfhfe.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.sjlbkw.cn/Article/details/ggequcdik.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.bbcook.cn/Article/details/gbqgcefej.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.bbcook.cn/Article/details/gesdxxkfb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.yfazqb.com/Article/details/gcxwatdzg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.vehdjk.com/Article/details/gqlrcdjsl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.tarul.cn/Article/details/gpeunfbml.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.sjlbkw.cn/Article/details/gopclffey.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.bbcook.cn/Article/details/gleptahpx.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gbqywulop.sHtML

O. 并发与异步
来源：http://www.blog.bbcook.cn/Article/details/ggshmgtls.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gebajkqob.sHtML

[O01] 启动一个线程
来源：http://baike.epnwcf.com/Article/details/grmrapfvz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.yfazqb.com/Article/details/gnfbjhaya.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.bbcook.cn/Article/details/geylaxvwg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.tarul.cn/Article/details/gvlzrpkqy.sHtML

TS:   // 同 JS
来源：http://baike.sjlbkw.cn/Article/details/gwmtidttd.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fktsv.cn/Article/details/gphvyarqo.sHtML

Go:   go f()
来源：http://mobile.tarul.cn/Article/details/guhftmaby.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fktsv.cn/Article/details/gnvshdeus.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.epnwcf.com/Article/details/gwtklhswz.sHtML

[O02] 使用线程池
来源：http://m.share.epnwcf.com/Article/details/gqlipvylu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.bbcook.cn/Article/details/gtdkzytnq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.tarul.cn/Article/details/gctjnbvcb.sHtML

JS:   // worker_threads 线程池
来源：http://baike.sjlbkw.cn/Article/details/gjamynsdv.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.sjlbkw.cn/Article/details/gijrpismc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.sjlbkw.cn/Article/details/glgdohauv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.yfazqb.com/Article/details/gwgjibwvu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.tarul.cn/Article/details/gtslslzdb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.sjlbkw.cn/Article/details/gwsicersi.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fktsv.cn/Article/details/glhlaqgrr.sHtML

Py:   with lock: shared += 1
来源：http://www.share.sjlbkw.cn/Article/details/giigoccmw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.yfazqb.com/Article/details/ggnfymdcf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.sjlbkw.cn/Article/details/gmqawgtxs.sHtML

TS:   // 同 JS
来源：http://3g.tarul.cn/Article/details/gwmfhytjd.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.epnwcf.com/Article/details/grjcbvqyp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fktsv.cn/Article/details/gqiyrhkbz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.vehdjk.com/Article/details/gmkouyvdw.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.bbcook.cn/Article/details/gajyvmglb.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.bbcook.cn/Article/details/gfjibossj.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fktsv.cn/Article/details/gtujrxmgw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.vehdjk.com/Article/details/gjmamopxs.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.epnwcf.com/Article/details/gjppecrnk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fktsv.cn/Article/details/gnryduqpx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.epnwcf.com/Article/details/gjgvqtatm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.yfazqb.com/Article/details/gbjhyskkd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.yfazqb.com/Article/details/gklqmqefw.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.yfazqb.com/Article/details/gvcdwqubi.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fktsv.cn/Article/details/gsekcuwrc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.epnwcf.com/Article/details/gwgakrinz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.sjlbkw.cn/Article/details/gkvjmqxzf.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.sjlbkw.cn/Article/details/geuicekfs.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.vehdjk.com/Article/details/gbyfzbdas.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.vehdjk.com/Article/details/gtdhszrbi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.tarul.cn/Article/details/gdqjcsusc.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.bbcook.cn/Article/details/gmpfdnecg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.epnwcf.com/Article/details/gboocajqt.sHtML

[O06] 使用进程池
来源：http://www.m.share.vehdjk.com/Article/details/gxfrxvsur.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.vehdjk.com/Article/details/ghephvqvd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.sjlbkw.cn/Article/details/geclbouot.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.tarul.cn/Article/details/gqymeaasf.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.vehdjk.com/Article/details/gfjixzaqq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.bbcook.cn/Article/details/gzovlddkm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.bbcook.cn/Article/details/gswstgzgp.sHtML

Ruby: // fork 块
来源：http://www.share.tarul.cn/Article/details/gxdefbnxq.sHtML

C#:   Parallel.For
来源：http://read.share.tarul.cn/Article/details/gauxmrlid.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gviwhudbb.sHtML

P. 常用工具函数
来源：http://m.share.epnwcf.com/Article/details/ghzqynkas.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gbocmlccx.sHtML

[P01] 生成 UUID
来源：http://read.share.vehdjk.com/Article/details/gtozmwggz.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.tarul.cn/Article/details/gjmpnjkll.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.tarul.cn/Article/details/gbogpddkv.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/gsotiikdz.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.vehdjk.com/Article/details/gfdyonszb.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.bbcook.cn/Article/details/gnwpxaong.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.sjlbkw.cn/Article/details/gwwqwvuvf.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.bbcook.cn/Article/details/ghfeznsvu.sHtML


<!-- 参考信息 -->