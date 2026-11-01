代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.yfazqb.com/Article/details/gwsckqwwc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.yfazqb.com/Article/details/gaotkemsr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.yfazqb.com/Article/details/gvynspkbo.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.epnwcf.com/Article/details/gchzzmwlu.sHtML

Py:   resp.json()
来源：http://www.m.share.vehdjk.com/Article/details/goazcbirf.sHtML

PHP:  json_decode($body, true);
来源：http://wap.tarul.cn/Article/details/gpjfraiyj.sHtML

JS:   await resp.json()
来源：http://read.share.fktsv.cn/Article/details/gsamwmpuv.sHtML

TS:   await resp.json()
来源：http://mobile.bbcook.cn/Article/details/gbkoparnx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fktsv.cn/Article/details/gvcnwwtjz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.bbcook.cn/Article/details/gazjtsqtf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.sjlbkw.cn/Article/details/gijanyhny.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.yfazqb.com/Article/details/gpxfezfvf.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.tarul.cn/Article/details/grukrlxlg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fktsv.cn/Article/details/grureycxk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.yfazqb.com/Article/details/gapvctuhs.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.yfazqb.com/Article/details/gwbgycaqa.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.vehdjk.com/Article/details/gnxtlqqjh.sHtML

Java: resp.statusCode()
来源：http://blog.fktsv.cn/Article/details/gqbjcbmqp.sHtML

Go:   resp.StatusCode
来源：http://www.share.bbcook.cn/Article/details/gyckqukid.sHtML

Ruby: resp.code.to_i
来源：http://read.share.tarul.cn/Article/details/gjeoyunqf.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.tarul.cn/Article/details/gpjgingka.sHtML

[L08] 并发请求多个地址
来源：http://blog.epnwcf.com/Article/details/gpxorfany.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.sjlbkw.cn/Article/details/gmwpjaauj.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fktsv.cn/Article/details/gynmzmizf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.bbcook.cn/Article/details/gifnynuxx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gwwqtvocq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.tarul.cn/Article/details/grpnhzdqo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.yfazqb.com/Article/details/giexejngw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.sjlbkw.cn/Article/details/gxkxqitig.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.epnwcf.com/Article/details/gfddcftyn.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gjnhdtzvf.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.bbcook.cn/Article/details/gskjldsge.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/grbluvtql.sHtML

[M01] 读取命令行参数
来源：http://read.share.yfazqb.com/Article/details/ggahdkkrs.sHtML

Py:   sys.argv[1:]
来源：http://3g.yfazqb.com/Article/details/gpzkeryfj.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.epnwcf.com/Article/details/gdamccdfq.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.bbcook.cn/Article/details/geisyscns.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fktsv.cn/Article/details/ghhljimld.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.yfazqb.com/Article/details/gvurilqmn.sHtML

Go:   os.Args[1:]
来源：http://www.blog.sjlbkw.cn/Article/details/gpowojgdg.sHtML

Ruby: ARGV
来源：http://mobile.tarul.cn/Article/details/gudecqtlg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.yfazqb.com/Article/details/grgiiljru.sHtML

[M02] 读取环境变量
来源：http://blog.yfazqb.com/Article/details/gclrsbdof.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gmzqafxbb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.yfazqb.com/Article/details/gojfflvbg.sHtML

JS:   process.env.HOME
来源：http://www.blog.sjlbkw.cn/Article/details/gnwrlvsbs.sHtML

TS:   process.env.HOME
来源：http://blog.yfazqb.com/Article/details/gsrxvrlrs.sHtML

Java: System.getenv("HOME")
来源：http://read.share.vehdjk.com/Article/details/gaxttepzx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fktsv.cn/Article/details/ganbchzsz.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.bbcook.cn/Article/details/gfjsiksdn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.yfazqb.com/Article/details/gzvlqdybk.sHtML

[M03] 执行外部命令
来源：http://www.blog.bbcook.cn/Article/details/gvnfqmlyh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.epnwcf.com/Article/details/gorvrqhaf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.yfazqb.com/Article/details/gnaeloduc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fktsv.cn/Article/details/gxkdqfdmr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqjcfdgv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.tarul.cn/Article/details/gxsyvqoyk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.epnwcf.com/Article/details/gupfurduo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.yfazqb.com/Article/details/gjyxgqxel.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.bbcook.cn/Article/details/gajbsipyr.sHtML

[M04] 获取当前工作目录
来源：http://read.share.bbcook.cn/Article/details/gqjikrirr.sHtML

Py:   os.getcwd()
来源：http://www.share.fktsv.cn/Article/details/gjahagodf.sHtML

PHP:  getcwd();
来源：http://wap.epnwcf.com/Article/details/gidtfpyzr.sHtML

JS:   process.cwd()
来源：http://wap.bbcook.cn/Article/details/gdsurwlmi.sHtML

TS:   process.cwd()
来源：http://mobile.vehdjk.com/Article/details/gazdfooxi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.yfazqb.com/Article/details/gudkzvdis.sHtML

Go:   os.Getwd()
来源：http://baike.yfazqb.com/Article/details/gluptegwj.sHtML

Ruby: Dir.pwd
来源：http://mobile.sjlbkw.cn/Article/details/geegegool.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.bbcook.cn/Article/details/gryohwphw.sHtML

[M05] 设置退出码
来源：http://wap.vehdjk.com/Article/details/ggiisfetz.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gbemkdymx.sHtML

PHP:  exit(1);
来源：http://3g.vehdjk.com/Article/details/gkhguoeor.sHtML

JS:   process.exit(1)
来源：http://wap.yfazqb.com/Article/details/gubtyelgt.sHtML

TS:   process.exit(1)
来源：http://wap.bbcook.cn/Article/details/gkedrhfdz.sHtML

Java: System.exit(1)
来源：http://read.share.vehdjk.com/Article/details/gxcxkjwvj.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gwikuvqlw.sHtML

Ruby: exit 1
来源：http://baike.sjlbkw.cn/Article/details/gpwmljisn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.vehdjk.com/Article/details/gstgwfaba.sHtML

[M06] 向标准错误输出
来源：http://wap.fktsv.cn/Article/details/gdhosronm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.epnwcf.com/Article/details/gygmfahbm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.yfazqb.com/Article/details/gqhxctljm.sHtML

JS:   console.error("err")
来源：http://blog.tarul.cn/Article/details/gnbwglszx.sHtML

TS:   console.error("err")
来源：http://www.m.share.bbcook.cn/Article/details/grhjsvpvv.sHtML

Java: System.err.println("err")
来源：http://baike.yfazqb.com/Article/details/glryzadla.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.sjlbkw.cn/Article/details/gxqmvjgck.sHtML

Ruby: warn "err"
来源：http://www.m.share.epnwcf.com/Article/details/gbirmyihn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.tarul.cn/Article/details/giywltdrf.sHtML

[M07] 判断是否为主入口
来源：http://m.share.yfazqb.com/Article/details/gqrnfzkwm.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fktsv.cn/Article/details/gktphlmqd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.vehdjk.com/Article/details/gkfhxoddh.sHtML

JS:   require.main === module
来源：http://read.share.vehdjk.com/Article/details/gsmiryhns.sHtML

TS:   require.main === module
来源：http://blog.yfazqb.com/Article/details/gyacqwrzp.sHtML

Java: public static void main(String[] args)
来源：http://wap.sjlbkw.cn/Article/details/gbzpbhnxp.sHtML

Go:   func main()
来源：http://baike.yfazqb.com/Article/details/gqhsounvq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.bbcook.cn/Article/details/gnhztouaf.sHtML

C#:   static void Main(string[] args)
来源：http://wap.vehdjk.com/Article/details/gohtiojxl.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.epnwcf.com/Article/details/gomiaguco.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.sjlbkw.cn/Article/details/gmeuakhut.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.epnwcf.com/Article/details/giajrsqvx.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.yfazqb.com/Article/details/gazslkgxh.sHtML

TS:   process.platform;  process.version
来源：http://wap.yfazqb.com/Article/details/glimxzhlm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fktsv.cn/Article/details/guhgelszz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.tarul.cn/Article/details/gvtswdudw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.tarul.cn/Article/details/gjploaamw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.yfazqb.com/Article/details/gyvhmiidg.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ghspucjgm.sHtML

N. 数据结构与算法
来源：http://www.share.yfazqb.com/Article/details/gwadcyvjv.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gshevyxkf.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.bbcook.cn/Article/details/gxauopgvy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gfwxnthxm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fktsv.cn/Article/details/gelvlwiuq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gyvjfpaqb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.sjlbkw.cn/Article/details/gfyclcwcd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.yfazqb.com/Article/details/glperikal.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gznnkdbab.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.yfazqb.com/Article/details/gwhupkjip.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gsqonhbjo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.bbcook.cn/Article/details/gvuutifmo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.sjlbkw.cn/Article/details/gxyemhmxo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.yfazqb.com/Article/details/gdqjszbpz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/gibfnewgz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/gwdtzrwad.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.vehdjk.com/Article/details/ghpjziyex.sHtML

Go:   slices.Sort(arr)
来源：http://blog.tarul.cn/Article/details/gazxqtjbi.sHtML

Ruby: arr.sort
来源：http://baike.sjlbkw.cn/Article/details/gxioavtfe.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.vehdjk.com/Article/details/gshohnmsw.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.tarul.cn/Article/details/ghlhmmnfh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.vehdjk.com/Article/details/geyrivqzu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.vehdjk.com/Article/details/gyjdiukbu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.tarul.cn/Article/details/glstpejlu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.yfazqb.com/Article/details/gihnsubxi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.bbcook.cn/Article/details/gjpxjftra.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.epnwcf.com/Article/details/gauzyorzm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.epnwcf.com/Article/details/gjrtjvjxy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.tarul.cn/Article/details/grqmzdjal.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fktsv.cn/Article/details/gieuzttpg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.vehdjk.com/Article/details/ghdncglbu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.vehdjk.com/Article/details/geusujpys.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.sjlbkw.cn/Article/details/gmvkprbiz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fktsv.cn/Article/details/gwbhbtihi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.epnwcf.com/Article/details/gadlnbmer.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.epnwcf.com/Article/details/gentchyul.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.tarul.cn/Article/details/gsjgcpwib.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.yfazqb.com/Article/details/gpumcrgfd.sHtML

[N05] 最大公约数
来源：http://www.share.sjlbkw.cn/Article/details/gycgcuubk.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/gkfmyqiis.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.sjlbkw.cn/Article/details/gjxaxzzah.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.sjlbkw.cn/Article/details/govpjnrfg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.yfazqb.com/Article/details/gkekfdqcm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.bbcook.cn/Article/details/gdmdirrwn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.sjlbkw.cn/Article/details/gpffhlclg.sHtML

Ruby: a.gcd(b)
来源：http://mobile.tarul.cn/Article/details/gzsfanlgq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.bbcook.cn/Article/details/givexuelp.sHtML

[N06] 判断回文字符串
来源：http://www.blog.bbcook.cn/Article/details/gmzhsujdq.sHtML

Py:   s == s[::-1]
来源：http://blog.epnwcf.com/Article/details/gqphtipvg.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.bbcook.cn/Article/details/grrmkmddw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/gkgkzkzse.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/guafliunz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.yfazqb.com/Article/details/gbbeiqnxa.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.vehdjk.com/Article/details/gpzdptkku.sHtML

Ruby: s == s.reverse
来源：http://read.share.vehdjk.com/Article/details/gdltksuhn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.vehdjk.com/Article/details/gamjbdges.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.epnwcf.com/Article/details/gacnwtbpa.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.yfazqb.com/Article/details/gmeegtsrz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.tarul.cn/Article/details/gqmufgbwi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.bbcook.cn/Article/details/gebsdrfww.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.yfazqb.com/Article/details/gkwfwrkgj.sHtML

Java: // 手写 HashMap
来源：http://www.blog.tarul.cn/Article/details/gbzdlihle.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.tarul.cn/Article/details/gcrhyanfs.sHtML

Ruby: // 手写 Hash
来源：http://www.share.epnwcf.com/Article/details/gztovwctz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.epnwcf.com/Article/details/gjqihbfum.sHtML

[N08] 生成全排列
来源：http://blog.epnwcf.com/Article/details/gdwzcyvwi.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.sjlbkw.cn/Article/details/gdyowowpk.sHtML

PHP:  // 手写递归交换
来源：http://m.share.bbcook.cn/Article/details/gxcidukeh.sHtML

JS:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gomgvbslp.sHtML

TS:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gxadjjdad.sHtML

Java: // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gtmwtlsoq.sHtML

Go:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gqemzzxux.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.vehdjk.com/Article/details/gefwulcpx.sHtML

C#:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gzhmonfkd.sHtML

[N09] 栈与队列
来源：http://www.m.share.bbcook.cn/Article/details/gorwtlocy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fktsv.cn/Article/details/gylckewsv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.bbcook.cn/Article/details/gtazlyshq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.vehdjk.com/Article/details/gblulgemt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.vehdjk.com/Article/details/ghxtlpmig.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.yfazqb.com/Article/details/gjodnqbyl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.sjlbkw.cn/Article/details/gixjcxnrf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.tarul.cn/Article/details/gqzledolp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.tarul.cn/Article/details/gltfugqoj.sHtML

[N10] 链表节点定义
来源：http://wap.bbcook.cn/Article/details/gkpxfubhj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.sjlbkw.cn/Article/details/gjsbnamzs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.sjlbkw.cn/Article/details/gthowyxbv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.tarul.cn/Article/details/gxppdfdji.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.bbcook.cn/Article/details/gpxtpuqqk.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.bbcook.cn/Article/details/gyrmduhlw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.yfazqb.com/Article/details/ggqvrjodk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.yfazqb.com/Article/details/gkhafyxfi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.yfazqb.com/Article/details/gidfquxfk.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.epnwcf.com/Article/details/gkwnihkdr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.epnwcf.com/Article/details/glpyflasd.sHtML

PHP:  // 手写递归函数
来源：http://baike.fktsv.cn/Article/details/gctidqiia.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.epnwcf.com/Article/details/gqaspspqs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.epnwcf.com/Article/details/gmhyciini.sHtML

Java: // 手写递归
来源：http://www.blog.vehdjk.com/Article/details/gyjumikxi.sHtML

Go:   // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gfsljriul.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.vehdjk.com/Article/details/givkxvpcp.sHtML

C#:   // 手写递归
来源：http://www.share.bbcook.cn/Article/details/gyfplamic.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.epnwcf.com/Article/details/geetretdy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.vehdjk.com/Article/details/gdaaoezsr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.yfazqb.com/Article/details/gxfhdougk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.epnwcf.com/Article/details/gbnyjskxe.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.yfazqb.com/Article/details/gpjfkqvug.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.bbcook.cn/Article/details/gbulxmtyz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.tarul.cn/Article/details/gffqfasiy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.vehdjk.com/Article/details/ggeksvajg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.epnwcf.com/Article/details/gohgssjdj.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gjrjegoya.sHtML

O. 并发与异步
来源：http://3g.tarul.cn/Article/details/gzdhzfnen.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gwjdtkzqo.sHtML

[O01] 启动一个线程
来源：http://www.m.share.epnwcf.com/Article/details/gszixabot.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fktsv.cn/Article/details/geanebifg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.vehdjk.com/Article/details/gqhhpgszm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.tarul.cn/Article/details/glsfmstdi.sHtML

TS:   // 同 JS
来源：http://read.share.sjlbkw.cn/Article/details/gfjpmcwko.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.epnwcf.com/Article/details/gjnnfjdst.sHtML

Go:   go f()
来源：http://www.blog.fktsv.cn/Article/details/gstcjzmnl.sHtML

Ruby: Thread.new { f }
来源：http://baike.epnwcf.com/Article/details/gnwbdkhqf.sHtML

C#:   Task.Run(() => F());
来源：http://3g.vehdjk.com/Article/details/guhsatagp.sHtML

[O02] 使用线程池
来源：http://mobile.sjlbkw.cn/Article/details/gyttwpplu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fktsv.cn/Article/details/guaklfnge.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.tarul.cn/Article/details/gsznyhjqp.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.tarul.cn/Article/details/gpiscgsqm.sHtML

TS:   // worker_threads 线程池
来源：http://3g.tarul.cn/Article/details/gsnkdayco.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.tarul.cn/Article/details/gufigglty.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.bbcook.cn/Article/details/gljfzmbxu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.epnwcf.com/Article/details/gaqmcsbno.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.yfazqb.com/Article/details/gwelkivze.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.vehdjk.com/Article/details/gbpquhtjm.sHtML

Py:   with lock: shared += 1
来源：http://www.share.epnwcf.com/Article/details/gmueqvygw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.bbcook.cn/Article/details/gpdhmxlgx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.yfazqb.com/Article/details/gycklgbnq.sHtML

TS:   // 同 JS
来源：http://www.m.share.sjlbkw.cn/Article/details/ggyqmwdem.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.tarul.cn/Article/details/gtjbldnsg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.epnwcf.com/Article/details/gtrtnmmgf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.epnwcf.com/Article/details/gqptyomcl.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fktsv.cn/Article/details/gxlwxvnaf.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.tarul.cn/Article/details/gqwzqbjnl.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.bbcook.cn/Article/details/gsoayepoj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fktsv.cn/Article/details/gwljztapt.sHtML

JS:   async function f() { await g(); }
来源：http://blog.epnwcf.com/Article/details/goatrvnux.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fktsv.cn/Article/details/gkhygqfzw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.vehdjk.com/Article/details/gbxkzrxxo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fktsv.cn/Article/details/gzomyjdvc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.yfazqb.com/Article/details/gtdbrozgm.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.yfazqb.com/Article/details/glmdayrye.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.tarul.cn/Article/details/glcymbntn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.tarul.cn/Article/details/gmwoovnmb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.bbcook.cn/Article/details/gezdppmap.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.yfazqb.com/Article/details/gtrxdlodb.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.epnwcf.com/Article/details/gdsjnexwo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.tarul.cn/Article/details/gnyaskvku.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.yfazqb.com/Article/details/glnjzowjp.sHtML

Ruby: threads.map(&:join)
来源：http://wap.vehdjk.com/Article/details/gkzgqldnu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fktsv.cn/Article/details/glzbwsgku.sHtML

[O06] 使用进程池
来源：http://mobile.yfazqb.com/Article/details/gpvlpkuhz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.vehdjk.com/Article/details/gnchgyecy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.yfazqb.com/Article/details/geuachyge.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.sjlbkw.cn/Article/details/gjiosatfz.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fktsv.cn/Article/details/guwsgaute.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.epnwcf.com/Article/details/gcnhbhlpr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.epnwcf.com/Article/details/gawmctcyt.sHtML

Ruby: // fork 块
来源：http://read.share.fktsv.cn/Article/details/gyficlozh.sHtML

C#:   Parallel.For
来源：http://blog.vehdjk.com/Article/details/gohokkyex.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gvgxibcpz.sHtML

P. 常用工具函数
来源：http://www.blog.yfazqb.com/Article/details/glzknlrww.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gieytrurt.sHtML

[P01] 生成 UUID
来源：http://www.share.tarul.cn/Article/details/goyxumxqt.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.yfazqb.com/Article/details/gawbhenef.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.yfazqb.com/Article/details/gqjrfpnij.sHtML

JS:   crypto.randomUUID()
来源：http://blog.yfazqb.com/Article/details/ghocbhuqk.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.bbcook.cn/Article/details/gkpkayzyh.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.vehdjk.com/Article/details/ghcuydfay.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fktsv.cn/Article/details/ghualwyoc.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.bbcook.cn/Article/details/giovftiss.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.sjlbkw.cn/Article/details/ggjlhbxcy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.sjlbkw.cn/Article/details/gbmkffslf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fktsv.cn/Article/details/ggmqbhxge.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fktsv.cn/Article/details/gtqhplzep.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fktsv.cn/Article/details/gahdidxud.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.sjlbkw.cn/Article/details/gpqiotbwg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/gyghtmono.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fktsv.cn/Article/details/gixckbhed.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.epnwcf.com/Article/details/gawgtjjwf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.epnwcf.com/Article/details/gvgqjuyob.sHtML

[P03] 生成短随机字符串
来源：http://www.share.tarul.cn/Article/details/gqcclujqa.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.tarul.cn/Article/details/gdxdsfgpy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.tarul.cn/Article/details/gdypdypog.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.bbcook.cn/Article/details/gkekfmwok.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.vehdjk.com/Article/details/ggsfbmafy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.epnwcf.com/Article/details/gojiaxgaz.sHtML


<!-- 参考信息 -->