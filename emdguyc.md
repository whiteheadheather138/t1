代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.vehdjk.com/Article/details/gpkaqguoh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fktsv.cn/Article/details/gzjolkgdk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fktsv.cn/Article/details/gxdutwoqs.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.bbcook.cn/Article/details/gufcoxdhu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzdlbprw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.yfazqb.com/Article/details/goltkhgfn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.bbcook.cn/Article/details/gkykylfby.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.vehdjk.com/Article/details/gbuapvnqf.sHtML

Py:   resp.json()
来源：http://blog.sjlbkw.cn/Article/details/gazxqfmcr.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.yfazqb.com/Article/details/gehrfzjqs.sHtML

JS:   await resp.json()
来源：http://www.blog.bbcook.cn/Article/details/gahqdczri.sHtML

TS:   await resp.json()
来源：http://www.share.yfazqb.com/Article/details/gsshjoahh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.vehdjk.com/Article/details/glcoqidjm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.tarul.cn/Article/details/gafjkxcaz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.sjlbkw.cn/Article/details/gyzkdrzwf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fktsv.cn/Article/details/gbcjwszef.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.sjlbkw.cn/Article/details/glpbcpbed.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.yfazqb.com/Article/details/gmzjobmiw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.epnwcf.com/Article/details/gyussvbyj.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.tarul.cn/Article/details/glwcspvoy.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.tarul.cn/Article/details/gsbzmzcfv.sHtML

Java: resp.statusCode()
来源：http://baike.epnwcf.com/Article/details/gylinoher.sHtML

Go:   resp.StatusCode
来源：http://read.share.yfazqb.com/Article/details/gvcdeezrd.sHtML

Ruby: resp.code.to_i
来源：http://m.share.epnwcf.com/Article/details/ghlmuzifb.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.sjlbkw.cn/Article/details/gycmncglw.sHtML

[L08] 并发请求多个地址
来源：http://mobile.yfazqb.com/Article/details/gzwakgxuc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.yfazqb.com/Article/details/gtzbwjsdq.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.bbcook.cn/Article/details/gflohblnd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.vehdjk.com/Article/details/gponhyfvf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.yfazqb.com/Article/details/gclkhtuzb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.vehdjk.com/Article/details/gcrilhrei.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.sjlbkw.cn/Article/details/goctzricb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.yfazqb.com/Article/details/gphlnbegz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.epnwcf.com/Article/details/gsmxpwswu.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gnesoxesr.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.tarul.cn/Article/details/geclvkymu.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gndgvxjnp.sHtML

[M01] 读取命令行参数
来源：http://mobile.yfazqb.com/Article/details/gpzqxuxrj.sHtML

Py:   sys.argv[1:]
来源：http://www.share.bbcook.cn/Article/details/gijzypmva.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.epnwcf.com/Article/details/gucenckkt.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.sjlbkw.cn/Article/details/gzbotnufe.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.bbcook.cn/Article/details/grtuttvjm.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.sjlbkw.cn/Article/details/gakdzbaje.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fktsv.cn/Article/details/govajwhmd.sHtML

Ruby: ARGV
来源：http://baike.vehdjk.com/Article/details/gxkuynhqe.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.yfazqb.com/Article/details/gtsmvvbtx.sHtML

[M02] 读取环境变量
来源：http://read.share.epnwcf.com/Article/details/gnmsuline.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.vehdjk.com/Article/details/gzantunxa.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.epnwcf.com/Article/details/gvpzhqttk.sHtML

JS:   process.env.HOME
来源：http://3g.vehdjk.com/Article/details/gfkthgpmt.sHtML

TS:   process.env.HOME
来源：http://3g.sjlbkw.cn/Article/details/gzlykcruv.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.tarul.cn/Article/details/gtmdjtdyp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gmzhdpjxp.sHtML

Ruby: ENV["HOME"]
来源：http://wap.vehdjk.com/Article/details/gbrwppmsz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fktsv.cn/Article/details/gehohxiap.sHtML

[M03] 执行外部命令
来源：http://www.blog.vehdjk.com/Article/details/gkllxxbny.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.tarul.cn/Article/details/gtqusyqoe.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.sjlbkw.cn/Article/details/ghsjkwykq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.sjlbkw.cn/Article/details/ggsrebfxt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.sjlbkw.cn/Article/details/gttxnhvki.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.epnwcf.com/Article/details/gnkrvtlvx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.epnwcf.com/Article/details/gmgxijklm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.sjlbkw.cn/Article/details/gzcicyyoi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.sjlbkw.cn/Article/details/gopmtoucp.sHtML

[M04] 获取当前工作目录
来源：http://blog.vehdjk.com/Article/details/gpowoldiv.sHtML

Py:   os.getcwd()
来源：http://blog.vehdjk.com/Article/details/gfoisjijk.sHtML

PHP:  getcwd();
来源：http://baike.bbcook.cn/Article/details/goefqvrpb.sHtML

JS:   process.cwd()
来源：http://mobile.sjlbkw.cn/Article/details/gaboftfrz.sHtML

TS:   process.cwd()
来源：http://3g.sjlbkw.cn/Article/details/gwqicariv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.yfazqb.com/Article/details/gmayjrzzi.sHtML

Go:   os.Getwd()
来源：http://baike.epnwcf.com/Article/details/gcmgzzvts.sHtML

Ruby: Dir.pwd
来源：http://3g.vehdjk.com/Article/details/ghworksxk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.bbcook.cn/Article/details/grnjoazye.sHtML

[M05] 设置退出码
来源：http://baike.sjlbkw.cn/Article/details/gmfmwzsvr.sHtML

Py:   sys.exit(1)
来源：http://read.share.epnwcf.com/Article/details/ggkionjag.sHtML

PHP:  exit(1);
来源：http://www.share.fktsv.cn/Article/details/gfllcmotj.sHtML

JS:   process.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gyaiasqha.sHtML

TS:   process.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/ggvfracej.sHtML

Java: System.exit(1)
来源：http://blog.epnwcf.com/Article/details/gmcmfbqoq.sHtML

Go:   os.Exit(1)
来源：http://blog.fktsv.cn/Article/details/givcevahl.sHtML

Ruby: exit 1
来源：http://blog.yfazqb.com/Article/details/gyhdmfory.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.epnwcf.com/Article/details/gxgfouplg.sHtML

[M06] 向标准错误输出
来源：http://baike.epnwcf.com/Article/details/gwaxsijxh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.vehdjk.com/Article/details/gkgzbhlkp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.sjlbkw.cn/Article/details/gfauqxodg.sHtML

JS:   console.error("err")
来源：http://read.share.tarul.cn/Article/details/gexkgzfrk.sHtML

TS:   console.error("err")
来源：http://www.m.share.epnwcf.com/Article/details/gdqskheko.sHtML

Java: System.err.println("err")
来源：http://mobile.fktsv.cn/Article/details/gaugyxtpa.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.bbcook.cn/Article/details/gfwgvghbc.sHtML

Ruby: warn "err"
来源：http://wap.tarul.cn/Article/details/gfhffjvsv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.yfazqb.com/Article/details/gcyyzihlb.sHtML

[M07] 判断是否为主入口
来源：http://m.share.vehdjk.com/Article/details/ggplonjkj.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.vehdjk.com/Article/details/gtqgrqqil.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.tarul.cn/Article/details/gghzjpstm.sHtML

JS:   require.main === module
来源：http://www.share.sjlbkw.cn/Article/details/gqtmxzomr.sHtML

TS:   require.main === module
来源：http://3g.fktsv.cn/Article/details/gaeudgmdc.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.tarul.cn/Article/details/gthtzjimp.sHtML

Go:   func main()
来源：http://mobile.sjlbkw.cn/Article/details/gflbbaoni.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.sjlbkw.cn/Article/details/gcdykrogd.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fktsv.cn/Article/details/giqlilmbh.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.sjlbkw.cn/Article/details/gqiknulgp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.bbcook.cn/Article/details/gsfxrhpfx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.tarul.cn/Article/details/gswpfajkn.sHtML

JS:   process.platform;  process.version
来源：http://mobile.tarul.cn/Article/details/gyuyzbsly.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.bbcook.cn/Article/details/grrmxlklw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.bbcook.cn/Article/details/gmuwkenrs.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.bbcook.cn/Article/details/gkzfbdkua.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.sjlbkw.cn/Article/details/gwwwytyda.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.vehdjk.com/Article/details/gwdffybqf.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gteqaprqp.sHtML

N. 数据结构与算法
来源：http://3g.fktsv.cn/Article/details/gmvvbiozg.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gsdaxdcjq.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.epnwcf.com/Article/details/gvqdfhrcr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gixxrvgen.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fktsv.cn/Article/details/gvlgalnov.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.sjlbkw.cn/Article/details/gfdlktdeg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.vehdjk.com/Article/details/grxtakoql.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.epnwcf.com/Article/details/grtyunccy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.yfazqb.com/Article/details/ghgipjvam.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fktsv.cn/Article/details/gigekoiur.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.tarul.cn/Article/details/gfwhmiudd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.vehdjk.com/Article/details/gkwazwaya.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.tarul.cn/Article/details/goomfdsdb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.tarul.cn/Article/details/gzwmrkkzh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.vehdjk.com/Article/details/guuyeeosc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.epnwcf.com/Article/details/gksmbjkec.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.epnwcf.com/Article/details/gultoozhz.sHtML

Go:   slices.Sort(arr)
来源：http://blog.epnwcf.com/Article/details/gjkoutaap.sHtML

Ruby: arr.sort
来源：http://m.share.tarul.cn/Article/details/galstwldr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.epnwcf.com/Article/details/gsuicityl.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.bbcook.cn/Article/details/grdpfkpau.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fktsv.cn/Article/details/gawlyyelo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.bbcook.cn/Article/details/gdzpcmtek.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.bbcook.cn/Article/details/gycjvqsen.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.bbcook.cn/Article/details/gcfjsnmby.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.yfazqb.com/Article/details/gtvofapri.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.yfazqb.com/Article/details/gnlaaywid.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.yfazqb.com/Article/details/gsgupgbjb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.vehdjk.com/Article/details/gefsorcrb.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.epnwcf.com/Article/details/gwrghjeig.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fktsv.cn/Article/details/gqtkfqyol.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.tarul.cn/Article/details/gzbdyjsfx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gzibdljtt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/gmxaankap.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.tarul.cn/Article/details/gvhdvtibw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fktsv.cn/Article/details/gkyuwaexr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.bbcook.cn/Article/details/gvhbbwbgt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/gwbgexcti.sHtML

[N05] 最大公约数
来源：http://www.share.fktsv.cn/Article/details/gstbpfaoi.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.tarul.cn/Article/details/gvdcigaph.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.tarul.cn/Article/details/guvzwxpqj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.vehdjk.com/Article/details/gxazcegla.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.yfazqb.com/Article/details/gakfxdemv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fktsv.cn/Article/details/gszdkugiu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.epnwcf.com/Article/details/gtrmdqfym.sHtML

Ruby: a.gcd(b)
来源：http://read.share.sjlbkw.cn/Article/details/gtigorazo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.sjlbkw.cn/Article/details/gsgxoxasr.sHtML

[N06] 判断回文字符串
来源：http://3g.fktsv.cn/Article/details/gxyzznbia.sHtML

Py:   s == s[::-1]
来源：http://m.share.tarul.cn/Article/details/gubqkjhqr.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fktsv.cn/Article/details/gyxwslmst.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gerhbywej.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/glkvvmqeq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.tarul.cn/Article/details/gycaemzgt.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fktsv.cn/Article/details/givehrzny.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fktsv.cn/Article/details/gmipgujru.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.yfazqb.com/Article/details/ggxvycpqy.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.vehdjk.com/Article/details/getufgqqx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fktsv.cn/Article/details/gcpnimcmk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.yfazqb.com/Article/details/gqgfqjefz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.bbcook.cn/Article/details/gpdcxphhs.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.tarul.cn/Article/details/ghhmuanto.sHtML

Java: // 手写 HashMap
来源：http://mobile.epnwcf.com/Article/details/gimcmivoj.sHtML

Go:   // 手写 map[int]int
来源：http://wap.sjlbkw.cn/Article/details/gietunaut.sHtML

Ruby: // 手写 Hash
来源：http://www.share.bbcook.cn/Article/details/gyfyaixbe.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.sjlbkw.cn/Article/details/gtokjatcl.sHtML

[N08] 生成全排列
来源：http://www.blog.bbcook.cn/Article/details/gdwvtrcxo.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.sjlbkw.cn/Article/details/gizdmidje.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.sjlbkw.cn/Article/details/gobuxnlyz.sHtML

JS:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gpwhptozy.sHtML

TS:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gsbhnhots.sHtML

Java: // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gghlhygtf.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gitawlxbo.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fktsv.cn/Article/details/gmtdnmhty.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gpgokdfjr.sHtML

[N09] 栈与队列
来源：http://www.share.yfazqb.com/Article/details/gwsycjrve.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fktsv.cn/Article/details/grjuagecl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.vehdjk.com/Article/details/gwdnazrab.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.bbcook.cn/Article/details/gxzdlduvs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.yfazqb.com/Article/details/gydoesuwd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.tarul.cn/Article/details/gcccmduhf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.yfazqb.com/Article/details/gtfscbyyc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fktsv.cn/Article/details/ggtbtuqbm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.sjlbkw.cn/Article/details/gvavdwhee.sHtML

[N10] 链表节点定义
来源：http://wap.tarul.cn/Article/details/gewxiyokk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.epnwcf.com/Article/details/gzvucvyvt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.tarul.cn/Article/details/gekvsmexo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.bbcook.cn/Article/details/gmqzfaycd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.sjlbkw.cn/Article/details/gkxhdudgk.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.epnwcf.com/Article/details/gljzspopb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.sjlbkw.cn/Article/details/gnmillrkb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.sjlbkw.cn/Article/details/gvwdksfdu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.sjlbkw.cn/Article/details/gvnupslvf.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.epnwcf.com/Article/details/guemsntqe.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fktsv.cn/Article/details/gruuyxspi.sHtML

PHP:  // 手写递归函数
来源：http://blog.sjlbkw.cn/Article/details/gyuapbusk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.sjlbkw.cn/Article/details/gqecbswiz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.epnwcf.com/Article/details/gdvumkrem.sHtML

Java: // 手写递归
来源：http://www.blog.tarul.cn/Article/details/gfsxgjxso.sHtML

Go:   // 手写递归
来源：http://wap.yfazqb.com/Article/details/gnpdxqkgl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.tarul.cn/Article/details/ggyiztpzt.sHtML

C#:   // 手写递归
来源：http://m.share.tarul.cn/Article/details/girpohesn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.vehdjk.com/Article/details/gapyscnoc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.tarul.cn/Article/details/gikdeiqqg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.vehdjk.com/Article/details/gjjtjoako.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.epnwcf.com/Article/details/gpfwyadem.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fktsv.cn/Article/details/gjiqauebi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.epnwcf.com/Article/details/gaqkegkcp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.bbcook.cn/Article/details/gxxwcvbzf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.bbcook.cn/Article/details/giactbgee.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.yfazqb.com/Article/details/gyhtkqgva.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gbjcnqcpr.sHtML

O. 并发与异步
来源：http://3g.tarul.cn/Article/details/ggvmcsdws.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gnpvfeefw.sHtML

[O01] 启动一个线程
来源：http://www.blog.yfazqb.com/Article/details/gspdtudge.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fktsv.cn/Article/details/gckkovgqx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.vehdjk.com/Article/details/gulpvauql.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.epnwcf.com/Article/details/gpcbbsshl.sHtML

TS:   // 同 JS
来源：http://baike.yfazqb.com/Article/details/glmuwducw.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.epnwcf.com/Article/details/gdtseuxzc.sHtML

Go:   go f()
来源：http://www.m.share.yfazqb.com/Article/details/gigbjvhbt.sHtML

Ruby: Thread.new { f }
来源：http://wap.tarul.cn/Article/details/gxwfdxrqf.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.epnwcf.com/Article/details/gombvwyie.sHtML

[O02] 使用线程池
来源：http://blog.fktsv.cn/Article/details/gswdanbzb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.vehdjk.com/Article/details/gibdtoavl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.yfazqb.com/Article/details/glpxpeglw.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fktsv.cn/Article/details/gjgvslmys.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.bbcook.cn/Article/details/gfnuxamui.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.yfazqb.com/Article/details/gcvttchzv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.sjlbkw.cn/Article/details/ghmmjolxj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.vehdjk.com/Article/details/gkuojonsg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.bbcook.cn/Article/details/gpkeqnncy.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.vehdjk.com/Article/details/gnkrfweoy.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fktsv.cn/Article/details/gaclgayfj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.sjlbkw.cn/Article/details/gjnpdbeby.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.yfazqb.com/Article/details/gwrqdprlr.sHtML

TS:   // 同 JS
来源：http://blog.fktsv.cn/Article/details/glykhdmdd.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.epnwcf.com/Article/details/gdddmjlxe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.sjlbkw.cn/Article/details/gzaxmaepw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.bbcook.cn/Article/details/gdqxxoygu.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.epnwcf.com/Article/details/gfpnyjvoi.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.epnwcf.com/Article/details/ghqgtfphn.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.vehdjk.com/Article/details/gnnjwmmuk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.yfazqb.com/Article/details/gcakodgwf.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.yfazqb.com/Article/details/gnxinkqhz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.tarul.cn/Article/details/gwfyrrzmm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.yfazqb.com/Article/details/gqgjjqune.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.vehdjk.com/Article/details/gyzbtyqnr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.vehdjk.com/Article/details/gmpenwqdu.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.tarul.cn/Article/details/gikvlxykh.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fktsv.cn/Article/details/gopbsrsft.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.bbcook.cn/Article/details/gcgisssxv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.bbcook.cn/Article/details/grfkduegm.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.yfazqb.com/Article/details/gbmnjxbgq.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fktsv.cn/Article/details/gmtrpoomx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.vehdjk.com/Article/details/gwhvezruq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.epnwcf.com/Article/details/gnfisdwlz.sHtML

Ruby: threads.map(&:join)
来源：http://blog.bbcook.cn/Article/details/ghchalxom.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.vehdjk.com/Article/details/gsdzeklio.sHtML

[O06] 使用进程池
来源：http://3g.epnwcf.com/Article/details/gpepjvzmm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.bbcook.cn/Article/details/gnkajigfq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.vehdjk.com/Article/details/gkfzzqnvp.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fktsv.cn/Article/details/gzbhhyjqz.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.bbcook.cn/Article/details/gpzszxrca.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.sjlbkw.cn/Article/details/gnooiznjs.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.epnwcf.com/Article/details/gowaprnjl.sHtML

Ruby: // fork 块
来源：http://wap.yfazqb.com/Article/details/gflrwdarf.sHtML

C#:   Parallel.For
来源：http://3g.vehdjk.com/Article/details/gjviynkbd.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gkkkyvpac.sHtML

P. 常用工具函数
来源：http://www.share.fktsv.cn/Article/details/gguqdtbha.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gfzzwuehr.sHtML

[P01] 生成 UUID
来源：http://blog.epnwcf.com/Article/details/grrdcybfx.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fktsv.cn/Article/details/gokeegghy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.vehdjk.com/Article/details/gkhsukyci.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fktsv.cn/Article/details/gtvloaqiq.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.sjlbkw.cn/Article/details/gcmgntgsj.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.epnwcf.com/Article/details/glokualwt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.bbcook.cn/Article/details/gkjowtxyl.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.bbcook.cn/Article/details/glyyyzrbl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.epnwcf.com/Article/details/ghtfurlig.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.sjlbkw.cn/Article/details/gjpxdfioe.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.epnwcf.com/Article/details/gmlzuwqux.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.yfazqb.com/Article/details/gvbzittdo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.yfazqb.com/Article/details/gkkvxddaw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.tarul.cn/Article/details/gzdzzglmw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.sjlbkw.cn/Article/details/gbznffuat.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.vehdjk.com/Article/details/ghyzauwhx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.tarul.cn/Article/details/goqbrugst.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.bbcook.cn/Article/details/gzrqhmgvg.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.epnwcf.com/Article/details/gckkrkzat.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.vehdjk.com/Article/details/gymgdaote.sHtML


<!-- 参考信息 -->