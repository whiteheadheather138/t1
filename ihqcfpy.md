代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.sjlbkw.cn/Article/details/gzzvxxzxr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fktsv.cn/Article/details/glswhmljv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.tarul.cn/Article/details/gnytdwdtz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.epnwcf.com/Article/details/gtnlewiyk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.sjlbkw.cn/Article/details/ghlzhuxjt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.vehdjk.com/Article/details/gdfgqitaj.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.sjlbkw.cn/Article/details/gmyyhmjjc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.vehdjk.com/Article/details/gtxucwfdk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fktsv.cn/Article/details/gjtihjqkk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.sjlbkw.cn/Article/details/govqjpcmx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.vehdjk.com/Article/details/gbrpvrmxm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.vehdjk.com/Article/details/gjvpxrvrj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.epnwcf.com/Article/details/geepsbigp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.vehdjk.com/Article/details/gnlvfvhim.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gnjitarek.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fktsv.cn/Article/details/gkwkcbpdo.sHtML

Py:   resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/gqitwltye.sHtML

PHP:  json_decode($body, true);
来源：http://baike.vehdjk.com/Article/details/gsdtyfvya.sHtML

JS:   await resp.json()
来源：http://wap.yfazqb.com/Article/details/gjaodocmf.sHtML

TS:   await resp.json()
来源：http://m.share.vehdjk.com/Article/details/gmcakxwrz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.yfazqb.com/Article/details/gplcgrfon.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.sjlbkw.cn/Article/details/gisypgbmk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.yfazqb.com/Article/details/gikjrqswf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.tarul.cn/Article/details/gltmngciq.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.vehdjk.com/Article/details/gegrlsqrj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.vehdjk.com/Article/details/gcrokirta.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.bbcook.cn/Article/details/gtdxxoffu.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.bbcook.cn/Article/details/gpopdyrxn.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.bbcook.cn/Article/details/gcoxlkhro.sHtML

Java: resp.statusCode()
来源：http://wap.tarul.cn/Article/details/gmdyatoxn.sHtML

Go:   resp.StatusCode
来源：http://baike.fktsv.cn/Article/details/gaxfrvzpx.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fktsv.cn/Article/details/gazbyvxlw.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.sjlbkw.cn/Article/details/gslljrovx.sHtML

[L08] 并发请求多个地址
来源：http://blog.vehdjk.com/Article/details/gahbxqnao.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.tarul.cn/Article/details/gpekfacew.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.vehdjk.com/Article/details/gnsrujzdz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.tarul.cn/Article/details/ghinqjgbp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.yfazqb.com/Article/details/gkwuxiqsw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.epnwcf.com/Article/details/gdapouprm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.tarul.cn/Article/details/gawylnvut.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.vehdjk.com/Article/details/gtyfxoizy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fktsv.cn/Article/details/gljxgfens.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/grttcizlb.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.sjlbkw.cn/Article/details/gwzvsoedi.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gblareawr.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fktsv.cn/Article/details/geqshnxct.sHtML

Py:   sys.argv[1:]
来源：http://blog.epnwcf.com/Article/details/gwawkbfln.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.tarul.cn/Article/details/gybqmulwd.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fktsv.cn/Article/details/glkmiqqbs.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.bbcook.cn/Article/details/gbvqkscbt.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fktsv.cn/Article/details/gwtypfaba.sHtML

Go:   os.Args[1:]
来源：http://baike.vehdjk.com/Article/details/gkistcpam.sHtML

Ruby: ARGV
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdioksfb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.sjlbkw.cn/Article/details/gckjloypr.sHtML

[M02] 读取环境变量
来源：http://read.share.fktsv.cn/Article/details/grfknjyyx.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.vehdjk.com/Article/details/gpwoqjstf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fktsv.cn/Article/details/gelvecrjv.sHtML

JS:   process.env.HOME
来源：http://www.share.bbcook.cn/Article/details/gismiqmkf.sHtML

TS:   process.env.HOME
来源：http://www.share.vehdjk.com/Article/details/gqsdrrztm.sHtML

Java: System.getenv("HOME")
来源：http://read.share.sjlbkw.cn/Article/details/gdktefkze.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gojpsfwpw.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.bbcook.cn/Article/details/gpykqmnut.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.yfazqb.com/Article/details/gfuqrhqez.sHtML

[M03] 执行外部命令
来源：http://www.m.share.yfazqb.com/Article/details/gdlhgiuat.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.sjlbkw.cn/Article/details/grqwljfie.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.yfazqb.com/Article/details/gnegknkle.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.bbcook.cn/Article/details/gpzkfykjm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.epnwcf.com/Article/details/gtasgnjxh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.vehdjk.com/Article/details/gltjzobcw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.epnwcf.com/Article/details/gbczlxrtm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.bbcook.cn/Article/details/guvwltdfa.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.bbcook.cn/Article/details/gvuqjxgdt.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.vehdjk.com/Article/details/gyavuilnt.sHtML

Py:   os.getcwd()
来源：http://read.share.fktsv.cn/Article/details/gnkedecgj.sHtML

PHP:  getcwd();
来源：http://www.m.share.vehdjk.com/Article/details/gxjizccxr.sHtML

JS:   process.cwd()
来源：http://www.blog.epnwcf.com/Article/details/gpdjvnonv.sHtML

TS:   process.cwd()
来源：http://www.share.yfazqb.com/Article/details/gqhhaczan.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.tarul.cn/Article/details/ggoqcguyb.sHtML

Go:   os.Getwd()
来源：http://baike.epnwcf.com/Article/details/gwfjsqfni.sHtML

Ruby: Dir.pwd
来源：http://blog.vehdjk.com/Article/details/ggmktqlsc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.epnwcf.com/Article/details/gyeyncrtx.sHtML

[M05] 设置退出码
来源：http://baike.epnwcf.com/Article/details/gkccvbpya.sHtML

Py:   sys.exit(1)
来源：http://baike.epnwcf.com/Article/details/gvczyyfjq.sHtML

PHP:  exit(1);
来源：http://read.share.tarul.cn/Article/details/gasdxqkkz.sHtML

JS:   process.exit(1)
来源：http://m.share.tarul.cn/Article/details/gppfxowdg.sHtML

TS:   process.exit(1)
来源：http://wap.yfazqb.com/Article/details/gutexexlm.sHtML

Java: System.exit(1)
来源：http://blog.epnwcf.com/Article/details/gexunypne.sHtML

Go:   os.Exit(1)
来源：http://mobile.vehdjk.com/Article/details/gavdxjado.sHtML

Ruby: exit 1
来源：http://baike.epnwcf.com/Article/details/gdghstlxe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.bbcook.cn/Article/details/govegdvuw.sHtML

[M06] 向标准错误输出
来源：http://m.share.tarul.cn/Article/details/glxkcgfcj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.yfazqb.com/Article/details/gxhnjjjwm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.sjlbkw.cn/Article/details/giynkxlcm.sHtML

JS:   console.error("err")
来源：http://m.share.sjlbkw.cn/Article/details/givwnhgpw.sHtML

TS:   console.error("err")
来源：http://read.share.fktsv.cn/Article/details/gzyutxmof.sHtML

Java: System.err.println("err")
来源：http://www.share.bbcook.cn/Article/details/gvoldbnuq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.sjlbkw.cn/Article/details/gmzxuamoh.sHtML

Ruby: warn "err"
来源：http://baike.yfazqb.com/Article/details/gfajzxdlb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.epnwcf.com/Article/details/gucrqffpi.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.vehdjk.com/Article/details/gwsjfthsm.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fktsv.cn/Article/details/godhbcuzq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.epnwcf.com/Article/details/geqmybyha.sHtML

JS:   require.main === module
来源：http://www.blog.tarul.cn/Article/details/gowegdseh.sHtML

TS:   require.main === module
来源：http://blog.bbcook.cn/Article/details/gdcffichp.sHtML

Java: public static void main(String[] args)
来源：http://wap.vehdjk.com/Article/details/grylrcuze.sHtML

Go:   func main()
来源：http://www.m.share.yfazqb.com/Article/details/gjburklgi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.bbcook.cn/Article/details/glwtsolgl.sHtML

C#:   static void Main(string[] args)
来源：http://wap.bbcook.cn/Article/details/gskqtxnev.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.bbcook.cn/Article/details/ghuczmjtb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fktsv.cn/Article/details/gtufaygos.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.tarul.cn/Article/details/guunwyszc.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.tarul.cn/Article/details/gxfvytrwh.sHtML

TS:   process.platform;  process.version
来源：http://blog.vehdjk.com/Article/details/gnuqrxocp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fktsv.cn/Article/details/gprscllon.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.vehdjk.com/Article/details/ggbbvlceh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.yfazqb.com/Article/details/gfykrnelr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.tarul.cn/Article/details/ggwmgyzcz.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gbbuuxgij.sHtML

N. 数据结构与算法
来源：http://www.blog.fktsv.cn/Article/details/gyengombx.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gzsyrrtdt.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.yfazqb.com/Article/details/gmvstcxvs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/ghxrbodtk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gymzvjtuv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/glaqewdga.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.yfazqb.com/Article/details/ggphvqfjb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fktsv.cn/Article/details/gwvqzfsbi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fktsv.cn/Article/details/gndvmawyy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.yfazqb.com/Article/details/glxtfnkqv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.bbcook.cn/Article/details/gkgswknzv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.epnwcf.com/Article/details/ghncjkxyo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.vehdjk.com/Article/details/gntudkchf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.tarul.cn/Article/details/gpznuhtyh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.vehdjk.com/Article/details/ghytqeahh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fktsv.cn/Article/details/gugwgevfs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.bbcook.cn/Article/details/grjoulyuo.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.yfazqb.com/Article/details/gkadxgvcy.sHtML

Ruby: arr.sort
来源：http://wap.sjlbkw.cn/Article/details/gdbsitktz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.yfazqb.com/Article/details/gijdtnbll.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.bbcook.cn/Article/details/gwxdsqixz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcregciv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.vehdjk.com/Article/details/gtgnrjwmv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.yfazqb.com/Article/details/guscpsczj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.bbcook.cn/Article/details/gqtlaqqgl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.vehdjk.com/Article/details/gvizuuixz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.epnwcf.com/Article/details/ggqhzbxqf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.bbcook.cn/Article/details/grcjdovum.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.yfazqb.com/Article/details/gdlwefmvu.sHtML

[N04] 斐波那契数列
来源：http://baike.epnwcf.com/Article/details/geogcurgm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.epnwcf.com/Article/details/gmeubuedu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.yfazqb.com/Article/details/ghbmtboai.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.sjlbkw.cn/Article/details/gfadjzgoe.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/gwmrzoccj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fktsv.cn/Article/details/gknuqjrgd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.sjlbkw.cn/Article/details/gfnxhwvvb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.tarul.cn/Article/details/ggasfzgea.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gekjqhpqj.sHtML

[N05] 最大公约数
来源：http://m.share.yfazqb.com/Article/details/gjnajfafe.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fktsv.cn/Article/details/gfncspobp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.tarul.cn/Article/details/ggnentttx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.yfazqb.com/Article/details/gepywgaba.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.yfazqb.com/Article/details/gvpjyhtam.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.vehdjk.com/Article/details/gnfcmzghh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.epnwcf.com/Article/details/grkckfixg.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmjpglqx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.sjlbkw.cn/Article/details/gundxqlnv.sHtML

[N06] 判断回文字符串
来源：http://www.blog.yfazqb.com/Article/details/gdykpmkwb.sHtML

Py:   s == s[::-1]
来源：http://read.share.vehdjk.com/Article/details/ggqcoovqo.sHtML

PHP:  $s === strrev($s);
来源：http://wap.epnwcf.com/Article/details/gmgnlcfhb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gynuorgyu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gziudpgrk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fktsv.cn/Article/details/gwyhpbwtl.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.epnwcf.com/Article/details/gziqxqqss.sHtML

Ruby: s == s.reverse
来源：http://m.share.fktsv.cn/Article/details/gwzgggswy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.vehdjk.com/Article/details/greafebwv.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.tarul.cn/Article/details/gtrybermx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.yfazqb.com/Article/details/gocqjnrxa.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.bbcook.cn/Article/details/ginbxvpqa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.epnwcf.com/Article/details/ghooapgkw.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.tarul.cn/Article/details/ggcsjknee.sHtML

Java: // 手写 HashMap
来源：http://www.blog.yfazqb.com/Article/details/gkslatome.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.epnwcf.com/Article/details/gbvwbixwg.sHtML

Ruby: // 手写 Hash
来源：http://mobile.vehdjk.com/Article/details/gqvvvgrke.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.yfazqb.com/Article/details/gtlzicsgm.sHtML

[N08] 生成全排列
来源：http://wap.bbcook.cn/Article/details/gradpgogf.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.epnwcf.com/Article/details/ggfsrqqdt.sHtML

PHP:  // 手写递归交换
来源：http://blog.fktsv.cn/Article/details/gwifihyom.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gllnzmxlc.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gksiepkgs.sHtML

Java: // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gwqmgzhma.sHtML

Go:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gdrtneftq.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.epnwcf.com/Article/details/gqefmudbd.sHtML

C#:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gfxzffapz.sHtML

[N09] 栈与队列
来源：http://mobile.bbcook.cn/Article/details/gqwdcvuvp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.bbcook.cn/Article/details/girryyaek.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/glhhspzzy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.yfazqb.com/Article/details/gzlnyvfry.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.vehdjk.com/Article/details/gjehuegiu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.tarul.cn/Article/details/gkwuutabj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.vehdjk.com/Article/details/gxphbuwwh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.vehdjk.com/Article/details/gabxpgxfr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.epnwcf.com/Article/details/ghnyrfrjl.sHtML

[N10] 链表节点定义
来源：http://mobile.fktsv.cn/Article/details/gpxzgpysf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.sjlbkw.cn/Article/details/gquhsnivz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.tarul.cn/Article/details/gyaxxhbxe.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fktsv.cn/Article/details/gvleanorh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.bbcook.cn/Article/details/gfiwabkfz.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.tarul.cn/Article/details/gvddbllhs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.vehdjk.com/Article/details/gcbvuzzlr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.yfazqb.com/Article/details/gnqdllrxl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fktsv.cn/Article/details/guobtizyi.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fktsv.cn/Article/details/gxpvzqorq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.tarul.cn/Article/details/ggcqwztwl.sHtML

PHP:  // 手写递归函数
来源：http://mobile.yfazqb.com/Article/details/givzzbahc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.epnwcf.com/Article/details/grejfeqqr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.tarul.cn/Article/details/guwzciqju.sHtML

Java: // 手写递归
来源：http://www.m.share.tarul.cn/Article/details/gnelzngcl.sHtML

Go:   // 手写递归
来源：http://mobile.yfazqb.com/Article/details/gbbwavsta.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.sjlbkw.cn/Article/details/gkcjcqsmj.sHtML

C#:   // 手写递归
来源：http://3g.yfazqb.com/Article/details/glwjfhoxc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.sjlbkw.cn/Article/details/gsjklpmvl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fktsv.cn/Article/details/gusbwnuum.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.sjlbkw.cn/Article/details/gtylcayje.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.vehdjk.com/Article/details/gronoqvdi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.vehdjk.com/Article/details/gfzifhskr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.epnwcf.com/Article/details/gpcxhqgmy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.bbcook.cn/Article/details/gsvpzjywp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.yfazqb.com/Article/details/gfexlxorf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.epnwcf.com/Article/details/gzwynhtfk.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gslljgajo.sHtML

O. 并发与异步
来源：http://www.blog.bbcook.cn/Article/details/gdczzwnqh.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/grbelemoj.sHtML

[O01] 启动一个线程
来源：http://www.m.share.tarul.cn/Article/details/gwahsduim.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.vehdjk.com/Article/details/gjlgxzygh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.bbcook.cn/Article/details/gcwhxcqvw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.epnwcf.com/Article/details/gfqhzlpar.sHtML

TS:   // 同 JS
来源：http://www.share.vehdjk.com/Article/details/gebhwylxy.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.yfazqb.com/Article/details/ghamlfasf.sHtML

Go:   go f()
来源：http://3g.tarul.cn/Article/details/gvxpklehx.sHtML

Ruby: Thread.new { f }
来源：http://www.share.tarul.cn/Article/details/gqdwgywag.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.tarul.cn/Article/details/gtcdrzzsr.sHtML

[O02] 使用线程池
来源：http://www.blog.tarul.cn/Article/details/gbwnnijao.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.bbcook.cn/Article/details/gyfkgglap.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.bbcook.cn/Article/details/gyxtptubx.sHtML

JS:   // worker_threads 线程池
来源：http://baike.vehdjk.com/Article/details/githerhhw.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.bbcook.cn/Article/details/gomrzfzwk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.epnwcf.com/Article/details/gokzyhxuf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.tarul.cn/Article/details/gmquinoxn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.sjlbkw.cn/Article/details/gbwsuoeqw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fktsv.cn/Article/details/ghqmajclr.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.vehdjk.com/Article/details/gbmtrxrsz.sHtML

Py:   with lock: shared += 1
来源：http://blog.vehdjk.com/Article/details/gfcqzirfs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.tarul.cn/Article/details/gqyrqrfdl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.epnwcf.com/Article/details/gsprbgddl.sHtML

TS:   // 同 JS
来源：http://mobile.vehdjk.com/Article/details/grvcruorx.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.vehdjk.com/Article/details/gprgkhywz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.vehdjk.com/Article/details/ghiqrgoga.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.bbcook.cn/Article/details/gwmgsyrcq.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fktsv.cn/Article/details/guntdfhyk.sHtML

[O04] 定义异步函数并等待
来源：http://blog.epnwcf.com/Article/details/gqlausaen.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.epnwcf.com/Article/details/gxzhujhwl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.bbcook.cn/Article/details/ghzugsikb.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.sjlbkw.cn/Article/details/gmoaxqcbu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.epnwcf.com/Article/details/gazndmojp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.epnwcf.com/Article/details/gtnzwstwu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.epnwcf.com/Article/details/giwncprkp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.bbcook.cn/Article/details/gaqcfstky.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fktsv.cn/Article/details/gxumprbje.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.sjlbkw.cn/Article/details/galxthkur.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.vehdjk.com/Article/details/gxpentnxd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.vehdjk.com/Article/details/gcfhdumuw.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.vehdjk.com/Article/details/gpeunhtch.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.sjlbkw.cn/Article/details/gyobgyluj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.vehdjk.com/Article/details/gmpewoyoj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.bbcook.cn/Article/details/gkqppvkxu.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.epnwcf.com/Article/details/gsoqcckmf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.bbcook.cn/Article/details/gpkceflnt.sHtML

[O06] 使用进程池
来源：http://www.share.yfazqb.com/Article/details/gtwqotbmb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.vehdjk.com/Article/details/gllbpldlz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.bbcook.cn/Article/details/gwbqchgds.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.epnwcf.com/Article/details/gkegvmtpv.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fktsv.cn/Article/details/gjtfrtpus.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fktsv.cn/Article/details/gdmcwoqcy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.sjlbkw.cn/Article/details/gkusknzju.sHtML

Ruby: // fork 块
来源：http://baike.vehdjk.com/Article/details/gzkuoisrj.sHtML

C#:   Parallel.For
来源：http://read.share.epnwcf.com/Article/details/grrexcqir.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gfytdtdkt.sHtML

P. 常用工具函数
来源：http://baike.sjlbkw.cn/Article/details/gmohtokiq.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ginmfhury.sHtML

[P01] 生成 UUID
来源：http://baike.yfazqb.com/Article/details/gvdvznpbz.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fktsv.cn/Article/details/gbqalbdyo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.tarul.cn/Article/details/gdevpmymz.sHtML

JS:   crypto.randomUUID()
来源：http://baike.yfazqb.com/Article/details/gttassufo.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fktsv.cn/Article/details/gnvujnpus.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.bbcook.cn/Article/details/gtncvfgtl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.sjlbkw.cn/Article/details/gwethfuki.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.vehdjk.com/Article/details/gjnlemgys.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.vehdjk.com/Article/details/gvrbwyndl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.bbcook.cn/Article/details/geomxlslg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.yfazqb.com/Article/details/gfcuswbbz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbozaqtka.sHtML


<!-- 参考信息 -->