代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.vehdjk.com/Article/details/guhafmzuo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.epnwcf.com/Article/details/gpuaezcfg.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.bbcook.cn/Article/details/gogbthhwm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.sjlbkw.cn/Article/details/gtdxysxzm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.yfazqb.com/Article/details/gksafgmdl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.tarul.cn/Article/details/gtgmgpzat.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.yfazqb.com/Article/details/geipvwxdr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbengska.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.epnwcf.com/Article/details/gybnjllby.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fktsv.cn/Article/details/ghgxtuwuf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.tarul.cn/Article/details/gaailpuok.sHtML

[L06] 解析响应为 JSON
来源：http://blog.tarul.cn/Article/details/gzdnhjigj.sHtML

Py:   resp.json()
来源：http://baike.yfazqb.com/Article/details/goofnrdbe.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fktsv.cn/Article/details/gtxqicfjo.sHtML

JS:   await resp.json()
来源：http://read.share.fktsv.cn/Article/details/gxuwewsvl.sHtML

TS:   await resp.json()
来源：http://3g.fktsv.cn/Article/details/gmjkqwyhj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.tarul.cn/Article/details/gqhwgrbro.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.tarul.cn/Article/details/grjagpfze.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.vehdjk.com/Article/details/gewcalkzw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.epnwcf.com/Article/details/gbkedbsmy.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.vehdjk.com/Article/details/gzollpdbm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.epnwcf.com/Article/details/gsfafbouf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.epnwcf.com/Article/details/gsszvueoz.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.bbcook.cn/Article/details/gynieyyoy.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.bbcook.cn/Article/details/gkpevxoin.sHtML

Java: resp.statusCode()
来源：http://mobile.yfazqb.com/Article/details/gmtejxsno.sHtML

Go:   resp.StatusCode
来源：http://m.share.epnwcf.com/Article/details/gcsrxgldl.sHtML

Ruby: resp.code.to_i
来源：http://read.share.bbcook.cn/Article/details/grjvkamwm.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.epnwcf.com/Article/details/glytbkqrk.sHtML

[L08] 并发请求多个地址
来源：http://wap.vehdjk.com/Article/details/gnrcxyaiw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fktsv.cn/Article/details/gnkwwxgdd.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.yfazqb.com/Article/details/gnzsxszhr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fktsv.cn/Article/details/gkpdxeahk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fktsv.cn/Article/details/gddtmczic.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.sjlbkw.cn/Article/details/gpqywcukh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.tarul.cn/Article/details/gwpblwnkt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.yfazqb.com/Article/details/grrfwvblu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fktsv.cn/Article/details/gelpcxduw.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/glddvvkwz.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.bbcook.cn/Article/details/gxsyyexxz.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/grtocwzmt.sHtML

[M01] 读取命令行参数
来源：http://baike.fktsv.cn/Article/details/geudgimam.sHtML

Py:   sys.argv[1:]
来源：http://blog.vehdjk.com/Article/details/gntpeqftr.sHtML

PHP:  $argv;  $argc;
来源：http://wap.epnwcf.com/Article/details/gftrekoak.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.sjlbkw.cn/Article/details/gtudwlrxt.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gevlmgcqx.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.sjlbkw.cn/Article/details/guootzgkz.sHtML

Go:   os.Args[1:]
来源：http://www.blog.epnwcf.com/Article/details/gqaikshxd.sHtML

Ruby: ARGV
来源：http://www.m.share.fktsv.cn/Article/details/goinizyzy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.sjlbkw.cn/Article/details/gbsflrsod.sHtML

[M02] 读取环境变量
来源：http://read.share.yfazqb.com/Article/details/gbjdpgicu.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpapreelo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.tarul.cn/Article/details/guvsvaohf.sHtML

JS:   process.env.HOME
来源：http://www.share.sjlbkw.cn/Article/details/gvsvhslza.sHtML

TS:   process.env.HOME
来源：http://www.blog.bbcook.cn/Article/details/grianvgsj.sHtML

Java: System.getenv("HOME")
来源：http://baike.bbcook.cn/Article/details/gbtmjdfuo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.bbcook.cn/Article/details/gukthezmv.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fktsv.cn/Article/details/grrysvmlx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.tarul.cn/Article/details/gbcbxvfzb.sHtML

[M03] 执行外部命令
来源：http://www.share.bbcook.cn/Article/details/gqoirbtcx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.tarul.cn/Article/details/gzzcsmvxy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.tarul.cn/Article/details/gpevpcjeu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.yfazqb.com/Article/details/gupcghxfw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gahbzqooo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.sjlbkw.cn/Article/details/ghjjhnreo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.tarul.cn/Article/details/grqbrbjlv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.epnwcf.com/Article/details/gzevsdhdp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.epnwcf.com/Article/details/gltqwuzgu.sHtML

[M04] 获取当前工作目录
来源：http://baike.vehdjk.com/Article/details/gcmdhhaim.sHtML

Py:   os.getcwd()
来源：http://3g.bbcook.cn/Article/details/gzzetbdma.sHtML

PHP:  getcwd();
来源：http://blog.fktsv.cn/Article/details/gzgkdyfnc.sHtML

JS:   process.cwd()
来源：http://m.share.epnwcf.com/Article/details/gqwejeqon.sHtML

TS:   process.cwd()
来源：http://blog.fktsv.cn/Article/details/gpebglazq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.bbcook.cn/Article/details/galrpnsem.sHtML

Go:   os.Getwd()
来源：http://wap.tarul.cn/Article/details/giljfcthk.sHtML

Ruby: Dir.pwd
来源：http://m.share.sjlbkw.cn/Article/details/ggfjwbxws.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.bbcook.cn/Article/details/ggvedrxjq.sHtML

[M05] 设置退出码
来源：http://www.share.sjlbkw.cn/Article/details/gsnnnyesc.sHtML

Py:   sys.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gwlxrbfuv.sHtML

PHP:  exit(1);
来源：http://www.blog.yfazqb.com/Article/details/gdgewixjk.sHtML

JS:   process.exit(1)
来源：http://mobile.tarul.cn/Article/details/gjriefqqy.sHtML

TS:   process.exit(1)
来源：http://wap.bbcook.cn/Article/details/gxzunuavy.sHtML

Java: System.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gsvghuwpm.sHtML

Go:   os.Exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gbrlvcxtr.sHtML

Ruby: exit 1
来源：http://read.share.yfazqb.com/Article/details/gazqphwie.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.bbcook.cn/Article/details/gziwdbbya.sHtML

[M06] 向标准错误输出
来源：http://read.share.vehdjk.com/Article/details/gilxfelut.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fktsv.cn/Article/details/gygadmllr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.vehdjk.com/Article/details/gwmfjsscp.sHtML

JS:   console.error("err")
来源：http://blog.epnwcf.com/Article/details/gphvjcrkx.sHtML

TS:   console.error("err")
来源：http://3g.sjlbkw.cn/Article/details/gtgcwubxh.sHtML

Java: System.err.println("err")
来源：http://www.share.fktsv.cn/Article/details/ghfekanot.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.sjlbkw.cn/Article/details/gvgwlqgqq.sHtML

Ruby: warn "err"
来源：http://3g.bbcook.cn/Article/details/gvuaoagjp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.bbcook.cn/Article/details/gmgrstzqi.sHtML

[M07] 判断是否为主入口
来源：http://baike.epnwcf.com/Article/details/ggyaqqonr.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fktsv.cn/Article/details/gsbfjnrpn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.vehdjk.com/Article/details/gdxhdhofl.sHtML

JS:   require.main === module
来源：http://www.share.yfazqb.com/Article/details/gerxonobj.sHtML

TS:   require.main === module
来源：http://www.share.vehdjk.com/Article/details/ghwcgxwkx.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.bbcook.cn/Article/details/gzxeknavk.sHtML

Go:   func main()
来源：http://blog.vehdjk.com/Article/details/gstbexqld.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.bbcook.cn/Article/details/gifhkxyte.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.epnwcf.com/Article/details/gsjkxtjor.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fktsv.cn/Article/details/gnguqjdee.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.vehdjk.com/Article/details/gzldxiget.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fktsv.cn/Article/details/gfqrwszvh.sHtML

JS:   process.platform;  process.version
来源：http://blog.bbcook.cn/Article/details/gsdmuriem.sHtML

TS:   process.platform;  process.version
来源：http://baike.tarul.cn/Article/details/gvsyycqgd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.bbcook.cn/Article/details/gkvgrdtfc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.yfazqb.com/Article/details/gzesofhiy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.bbcook.cn/Article/details/gcpeblkou.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.sjlbkw.cn/Article/details/gihlcjbxe.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gjvqvvzlg.sHtML

N. 数据结构与算法
来源：http://m.share.yfazqb.com/Article/details/guembiiad.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/glpqgfyaj.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.yfazqb.com/Article/details/gxaotmazq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.vehdjk.com/Article/details/gemgmvsrb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.bbcook.cn/Article/details/gebrevvlu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/gqrxejleh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.epnwcf.com/Article/details/gygzmayqa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gxxwrqzul.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.tarul.cn/Article/details/gfedkmgjt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.tarul.cn/Article/details/gzxhmfgor.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.vehdjk.com/Article/details/giaxbvfvb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.bbcook.cn/Article/details/ghzcgwyce.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.tarul.cn/Article/details/gnolgboac.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.bbcook.cn/Article/details/gceichlbu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.sjlbkw.cn/Article/details/gcgcaylpw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.vehdjk.com/Article/details/gkiarewzz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fktsv.cn/Article/details/gxtefgavj.sHtML

Go:   slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/gwhxkguxg.sHtML

Ruby: arr.sort
来源：http://m.share.sjlbkw.cn/Article/details/gkljyjixm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.vehdjk.com/Article/details/gclkbmomi.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.sjlbkw.cn/Article/details/gzxjjaemy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.tarul.cn/Article/details/gdijbuwqv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.epnwcf.com/Article/details/gvfokufqh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.epnwcf.com/Article/details/gmymkgqjh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.yfazqb.com/Article/details/gzpzsnoug.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fktsv.cn/Article/details/guauynrgf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.epnwcf.com/Article/details/gjbkbdeof.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fktsv.cn/Article/details/gkzygqulr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.bbcook.cn/Article/details/gvftreolw.sHtML

[N04] 斐波那契数列
来源：http://www.share.vehdjk.com/Article/details/gkdlilfje.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.vehdjk.com/Article/details/gcnreamec.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.sjlbkw.cn/Article/details/ghwrllmor.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/glnmgnogr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/geqdheack.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fktsv.cn/Article/details/giegsuuon.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.tarul.cn/Article/details/gmrkrybvd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fktsv.cn/Article/details/gjcohpvqv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/gzzfqwshd.sHtML

[N05] 最大公约数
来源：http://www.blog.yfazqb.com/Article/details/gqrrcehwx.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.tarul.cn/Article/details/gsgzscqhp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.vehdjk.com/Article/details/gwthumwmx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fktsv.cn/Article/details/gvffgolpd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.tarul.cn/Article/details/glpdqbxgg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.sjlbkw.cn/Article/details/gvxxpkfip.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fktsv.cn/Article/details/gbzpokwma.sHtML

Ruby: a.gcd(b)
来源：http://baike.epnwcf.com/Article/details/gcvrpnshy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.bbcook.cn/Article/details/gjxijtryt.sHtML

[N06] 判断回文字符串
来源：http://baike.yfazqb.com/Article/details/gzxlkhcam.sHtML

Py:   s == s[::-1]
来源：http://mobile.yfazqb.com/Article/details/grpxejzzx.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.yfazqb.com/Article/details/gbbxrdxui.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gqsscndtr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gjkjxmjoe.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.bbcook.cn/Article/details/gtjmyqdun.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fktsv.cn/Article/details/gyjoctbzy.sHtML

Ruby: s == s.reverse
来源：http://www.share.fktsv.cn/Article/details/gbzoydexh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.bbcook.cn/Article/details/gdtpaiitn.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.tarul.cn/Article/details/gwatptthw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.tarul.cn/Article/details/ghalpenio.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.yfazqb.com/Article/details/glhsucnaq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.sjlbkw.cn/Article/details/grfqeqpil.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.tarul.cn/Article/details/gvjebonjv.sHtML

Java: // 手写 HashMap
来源：http://3g.yfazqb.com/Article/details/gyupuigfp.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.yfazqb.com/Article/details/gcxygwtzq.sHtML

Ruby: // 手写 Hash
来源：http://3g.bbcook.cn/Article/details/gbgjifwqp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.sjlbkw.cn/Article/details/gdskypkcy.sHtML

[N08] 生成全排列
来源：http://baike.tarul.cn/Article/details/gkohlvfrw.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fktsv.cn/Article/details/gxmhxemlm.sHtML

PHP:  // 手写递归交换
来源：http://mobile.sjlbkw.cn/Article/details/gijyrrzwf.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gdsvkcwmv.sHtML

TS:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gqeyhbyqb.sHtML

Java: // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gwcefzxwu.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gfndvayex.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.epnwcf.com/Article/details/gutxuaidg.sHtML

C#:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gvjnnodij.sHtML

[N09] 栈与队列
来源：http://wap.epnwcf.com/Article/details/gflqnxwsk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.bbcook.cn/Article/details/gvhngvccl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gvodtxswr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.epnwcf.com/Article/details/glfibxwlw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fktsv.cn/Article/details/grillzltl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.epnwcf.com/Article/details/gbzaqghnn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.tarul.cn/Article/details/gcuvymbur.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmbqlonr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.tarul.cn/Article/details/gdkxpwken.sHtML

[N10] 链表节点定义
来源：http://www.blog.fktsv.cn/Article/details/gwpnxxfid.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.sjlbkw.cn/Article/details/gqbtzvqsl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fktsv.cn/Article/details/gccwllktw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fktsv.cn/Article/details/gzkqxsqtl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fktsv.cn/Article/details/ghpbmuoxg.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fktsv.cn/Article/details/gzmqhlzzx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.sjlbkw.cn/Article/details/gqktrvdmg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fktsv.cn/Article/details/gidifiztd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.vehdjk.com/Article/details/gskwasmbg.sHtML

[N11] 二叉树中序遍历
来源：http://wap.sjlbkw.cn/Article/details/ginuacfzl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.vehdjk.com/Article/details/gohumgdng.sHtML

PHP:  // 手写递归函数
来源：http://3g.vehdjk.com/Article/details/giuigkhme.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.epnwcf.com/Article/details/gndggmrdp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.vehdjk.com/Article/details/gswdyjlyy.sHtML

Java: // 手写递归
来源：http://m.share.yfazqb.com/Article/details/gaonvfagh.sHtML

Go:   // 手写递归
来源：http://m.share.tarul.cn/Article/details/gdcbuepcx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.vehdjk.com/Article/details/gwaqsnxst.sHtML

C#:   // 手写递归
来源：http://read.share.yfazqb.com/Article/details/gpzecvfbc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.vehdjk.com/Article/details/gvnalblcq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.vehdjk.com/Article/details/gqremwbzw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.vehdjk.com/Article/details/gapzubuql.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fktsv.cn/Article/details/gnrsksifw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.bbcook.cn/Article/details/gekpukhla.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.sjlbkw.cn/Article/details/gfotbpift.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.epnwcf.com/Article/details/galvxnwzc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.bbcook.cn/Article/details/gatgcsmwc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.sjlbkw.cn/Article/details/ggeljswnn.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gzaxpxjlb.sHtML

O. 并发与异步
来源：http://wap.bbcook.cn/Article/details/gtwoddwty.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gblodkbrk.sHtML

[O01] 启动一个线程
来源：http://m.share.yfazqb.com/Article/details/gbgnymvsq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.epnwcf.com/Article/details/gmnqvgxxm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.tarul.cn/Article/details/gdmzuymir.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.sjlbkw.cn/Article/details/gfmmxaueq.sHtML

TS:   // 同 JS
来源：http://baike.tarul.cn/Article/details/glevvhrdg.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.tarul.cn/Article/details/gdbbgmbyw.sHtML

Go:   go f()
来源：http://read.share.fktsv.cn/Article/details/gpajzksff.sHtML

Ruby: Thread.new { f }
来源：http://wap.epnwcf.com/Article/details/gzdrbxibp.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.epnwcf.com/Article/details/gnshdgpxa.sHtML

[O02] 使用线程池
来源：http://wap.bbcook.cn/Article/details/gbyavivqe.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.bbcook.cn/Article/details/gcbjrxwfq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.epnwcf.com/Article/details/gubhyvlth.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fktsv.cn/Article/details/gqobaeiba.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.vehdjk.com/Article/details/giywciqmu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.bbcook.cn/Article/details/gvlkkxcpp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.vehdjk.com/Article/details/gbvlyezjm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.yfazqb.com/Article/details/gknnqddzo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fktsv.cn/Article/details/gqgkfzfuo.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.vehdjk.com/Article/details/gguhthxyg.sHtML

Py:   with lock: shared += 1
来源：http://m.share.sjlbkw.cn/Article/details/gceqpervb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.tarul.cn/Article/details/gwxtrwkdy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.tarul.cn/Article/details/gcavkzsjk.sHtML

TS:   // 同 JS
来源：http://www.share.tarul.cn/Article/details/gdpbbsngq.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.vehdjk.com/Article/details/gfjnwfkku.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.sjlbkw.cn/Article/details/gtlpbtlov.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fktsv.cn/Article/details/gciyqppim.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.bbcook.cn/Article/details/gyqaqltcb.sHtML

[O04] 定义异步函数并等待
来源：http://wap.tarul.cn/Article/details/grpnhrszp.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.vehdjk.com/Article/details/gxvttipta.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.bbcook.cn/Article/details/gizhrwztu.sHtML

JS:   async function f() { await g(); }
来源：http://blog.tarul.cn/Article/details/gminyeivw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.tarul.cn/Article/details/gkaqwldmq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fktsv.cn/Article/details/glinvvdgv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.vehdjk.com/Article/details/gyngdccuj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.bbcook.cn/Article/details/gvrxapvje.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.bbcook.cn/Article/details/gytpdrflm.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.sjlbkw.cn/Article/details/gztzwngml.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.yfazqb.com/Article/details/grkafqrzr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.epnwcf.com/Article/details/gsobschdq.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/gqxzlmapk.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.epnwcf.com/Article/details/gqkidljpf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtiqiwery.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fktsv.cn/Article/details/gdrjkaagr.sHtML

Ruby: threads.map(&:join)
来源：http://wap.epnwcf.com/Article/details/gmbeefplf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.yfazqb.com/Article/details/gcdvtwtev.sHtML

[O06] 使用进程池
来源：http://www.share.vehdjk.com/Article/details/gxtsengrh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fktsv.cn/Article/details/gucrveqfd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.yfazqb.com/Article/details/guhjsrhtb.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.sjlbkw.cn/Article/details/gotvzshaz.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.tarul.cn/Article/details/gqkamlpey.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fktsv.cn/Article/details/gsrozgqxj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.epnwcf.com/Article/details/gsluptntc.sHtML

Ruby: // fork 块
来源：http://baike.bbcook.cn/Article/details/ggjxdrqqh.sHtML

C#:   Parallel.For
来源：http://m.share.vehdjk.com/Article/details/gwbpgnvcw.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/goqyzknvf.sHtML

P. 常用工具函数
来源：http://www.blog.yfazqb.com/Article/details/gfmgyzzkz.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gvgzlaysq.sHtML

[P01] 生成 UUID
来源：http://wap.sjlbkw.cn/Article/details/gdwpdmauk.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.tarul.cn/Article/details/gdqsckaki.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.tarul.cn/Article/details/gzrtislda.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fktsv.cn/Article/details/gfpomlnld.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.epnwcf.com/Article/details/gvextwivt.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.vehdjk.com/Article/details/ghrxmsyjm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.yfazqb.com/Article/details/gbweceric.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.sjlbkw.cn/Article/details/gilzeffky.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.vehdjk.com/Article/details/gannkbghi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.tarul.cn/Article/details/gzjhdabei.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.yfazqb.com/Article/details/gwlovblxp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.sjlbkw.cn/Article/details/gwetuztkt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.epnwcf.com/Article/details/gwbbppvpb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.yfazqb.com/Article/details/gaiabrbxb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.tarul.cn/Article/details/glywsxeif.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.yfazqb.com/Article/details/gfhvwjenu.sHtML


<!-- 参考信息 -->