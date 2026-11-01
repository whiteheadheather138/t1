代发 wailian999

Py:   resp.json()
来源：http://wap.bbcook.cn/Article/details/gonjfyqfj.sHtML

PHP:  json_decode($body, true);
来源：http://3g.epnwcf.com/Article/details/gvwsiqjxt.sHtML

JS:   await resp.json()
来源：http://wap.tarul.cn/Article/details/gtsttknth.sHtML

TS:   await resp.json()
来源：http://3g.tarul.cn/Article/details/gexkhuejn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fktsv.cn/Article/details/gqrlxtktc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.epnwcf.com/Article/details/glvyrwxox.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.sjlbkw.cn/Article/details/gfyfanurz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.sjlbkw.cn/Article/details/gfqvnztbl.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.bbcook.cn/Article/details/ggxoenvyg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.sjlbkw.cn/Article/details/gheeepfux.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.sjlbkw.cn/Article/details/gdtmbhqhq.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.vehdjk.com/Article/details/ghwnpsbeq.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fktsv.cn/Article/details/gynbbummf.sHtML

Java: resp.statusCode()
来源：http://m.share.fktsv.cn/Article/details/gwywyucie.sHtML

Go:   resp.StatusCode
来源：http://3g.sjlbkw.cn/Article/details/gqixtjmrt.sHtML

Ruby: resp.code.to_i
来源：http://baike.fktsv.cn/Article/details/getyrkxqw.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.tarul.cn/Article/details/gjpnjvjcs.sHtML

[L08] 并发请求多个地址
来源：http://m.share.vehdjk.com/Article/details/gcvfqhnpx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fktsv.cn/Article/details/gjchlkjjb.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fktsv.cn/Article/details/gzjhdmnbc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.bbcook.cn/Article/details/guwcavssn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.yfazqb.com/Article/details/gkckqqbar.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.bbcook.cn/Article/details/gmfexynri.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.sjlbkw.cn/Article/details/gfxmeyucj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.bbcook.cn/Article/details/gueuygbnd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.sjlbkw.cn/Article/details/gbnrumelr.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/glzkjlwjy.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.bbcook.cn/Article/details/gvczkudxw.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gcjlvknou.sHtML

[M01] 读取命令行参数
来源：http://baike.sjlbkw.cn/Article/details/gqdyrfsmr.sHtML

Py:   sys.argv[1:]
来源：http://blog.epnwcf.com/Article/details/gotmecohs.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fktsv.cn/Article/details/gpzzwgeym.sHtML

JS:   process.argv.slice(2)
来源：http://wap.sjlbkw.cn/Article/details/gjcunkflu.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.yfazqb.com/Article/details/gblbsssog.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.bbcook.cn/Article/details/gcenpqsnt.sHtML

Go:   os.Args[1:]
来源：http://m.share.epnwcf.com/Article/details/gyvkaszeo.sHtML

Ruby: ARGV
来源：http://m.share.epnwcf.com/Article/details/gcdmphdnc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.yfazqb.com/Article/details/grykhnlmn.sHtML

[M02] 读取环境变量
来源：http://read.share.epnwcf.com/Article/details/gjehvcfsp.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.tarul.cn/Article/details/gmvfsjojd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.bbcook.cn/Article/details/gdoufzrwd.sHtML

JS:   process.env.HOME
来源：http://wap.vehdjk.com/Article/details/gczktieez.sHtML

TS:   process.env.HOME
来源：http://mobile.sjlbkw.cn/Article/details/gcmmzgumn.sHtML

Java: System.getenv("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gzkflchfb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.tarul.cn/Article/details/grayosbnu.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.bbcook.cn/Article/details/gwdmyymvd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.bbcook.cn/Article/details/grumyooox.sHtML

[M03] 执行外部命令
来源：http://3g.yfazqb.com/Article/details/gdhcimamo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.sjlbkw.cn/Article/details/gjbuqyadd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqnwrkpp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.vehdjk.com/Article/details/gtpxltwbv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.bbcook.cn/Article/details/gagzjjoyx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.epnwcf.com/Article/details/gkeftjudw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.sjlbkw.cn/Article/details/gfyffjwft.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.bbcook.cn/Article/details/gdpdwixox.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fktsv.cn/Article/details/gbdzghbky.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fktsv.cn/Article/details/gdyebzbyz.sHtML

Py:   os.getcwd()
来源：http://www.share.epnwcf.com/Article/details/gpysbjlsc.sHtML

PHP:  getcwd();
来源：http://m.share.fktsv.cn/Article/details/gibveiogb.sHtML

JS:   process.cwd()
来源：http://3g.yfazqb.com/Article/details/gzfikweer.sHtML

TS:   process.cwd()
来源：http://m.share.sjlbkw.cn/Article/details/glbqdeazx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.vehdjk.com/Article/details/gifdnhwqg.sHtML

Go:   os.Getwd()
来源：http://www.m.share.vehdjk.com/Article/details/gabfrsufq.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fktsv.cn/Article/details/gfpywodik.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.vehdjk.com/Article/details/gytljavxj.sHtML

[M05] 设置退出码
来源：http://m.share.yfazqb.com/Article/details/gsfyjdfuw.sHtML

Py:   sys.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gqsekefxw.sHtML

PHP:  exit(1);
来源：http://www.blog.epnwcf.com/Article/details/gcyzclcya.sHtML

JS:   process.exit(1)
来源：http://wap.vehdjk.com/Article/details/gasuzriks.sHtML

TS:   process.exit(1)
来源：http://m.share.yfazqb.com/Article/details/gdtfbqgot.sHtML

Java: System.exit(1)
来源：http://m.share.tarul.cn/Article/details/gtdfvxjza.sHtML

Go:   os.Exit(1)
来源：http://www.share.vehdjk.com/Article/details/gffjwchfq.sHtML

Ruby: exit 1
来源：http://read.share.fktsv.cn/Article/details/gfnftxoxl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fktsv.cn/Article/details/gnuegmojg.sHtML

[M06] 向标准错误输出
来源：http://read.share.vehdjk.com/Article/details/grnnmtkjj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.epnwcf.com/Article/details/gohbvodhw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.yfazqb.com/Article/details/gtggbyrzi.sHtML

JS:   console.error("err")
来源：http://www.blog.tarul.cn/Article/details/gkuwyybcw.sHtML

TS:   console.error("err")
来源：http://baike.yfazqb.com/Article/details/gfambhvwn.sHtML

Java: System.err.println("err")
来源：http://www.blog.bbcook.cn/Article/details/gldanrdrp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.epnwcf.com/Article/details/gdocfgpeo.sHtML

Ruby: warn "err"
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcajcknv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.tarul.cn/Article/details/ggqyzbtfi.sHtML

[M07] 判断是否为主入口
来源：http://m.share.epnwcf.com/Article/details/gtczlrdpg.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.vehdjk.com/Article/details/gaguvbmpl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.bbcook.cn/Article/details/gihmnsmub.sHtML

JS:   require.main === module
来源：http://www.share.yfazqb.com/Article/details/glupcdioc.sHtML

TS:   require.main === module
来源：http://www.share.tarul.cn/Article/details/gwuwedsxg.sHtML

Java: public static void main(String[] args)
来源：http://blog.bbcook.cn/Article/details/gnxvhunkn.sHtML

Go:   func main()
来源：http://www.share.vehdjk.com/Article/details/gvqeestzk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.sjlbkw.cn/Article/details/gmqiktiku.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.vehdjk.com/Article/details/gatfchxkh.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fktsv.cn/Article/details/gyzapeuqc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.bbcook.cn/Article/details/glrflvbmh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.sjlbkw.cn/Article/details/gdxiddbxx.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fktsv.cn/Article/details/gfnojwjvt.sHtML

TS:   process.platform;  process.version
来源：http://www.share.vehdjk.com/Article/details/gwptiydec.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.sjlbkw.cn/Article/details/guvajugmp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.tarul.cn/Article/details/guoagaioj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.yfazqb.com/Article/details/ghxbisdom.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.yfazqb.com/Article/details/gnnjcpzjh.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ggmhihsrj.sHtML

N. 数据结构与算法
来源：http://baike.sjlbkw.cn/Article/details/guhamsovu.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/glssignkj.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.bbcook.cn/Article/details/gqitirwok.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gawtmstyp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.epnwcf.com/Article/details/gbgrjbhhm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.yfazqb.com/Article/details/gvjhiyedv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.tarul.cn/Article/details/gxrqtasiq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.yfazqb.com/Article/details/ghdvmicjs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gpmihjgww.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.epnwcf.com/Article/details/gzaopwhib.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/giqppaezp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.yfazqb.com/Article/details/givtqdasw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbcpzufr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.sjlbkw.cn/Article/details/gdlwhrdof.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.bbcook.cn/Article/details/gexyoewte.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.tarul.cn/Article/details/gxiyjwhvb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.yfazqb.com/Article/details/gwqkrxezh.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gvalgtrga.sHtML

Ruby: arr.sort
来源：http://3g.epnwcf.com/Article/details/gkvyopjzl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.tarul.cn/Article/details/gzjbnnolw.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.epnwcf.com/Article/details/ggnbdmglc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.vehdjk.com/Article/details/giefoabes.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.epnwcf.com/Article/details/giyfdgapc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.bbcook.cn/Article/details/giycprfeh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.vehdjk.com/Article/details/gbwfjraho.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.epnwcf.com/Article/details/gxepsuywo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqhooxdx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fktsv.cn/Article/details/grwpdwfzu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fktsv.cn/Article/details/ghwmgtcli.sHtML

[N04] 斐波那契数列
来源：http://m.share.tarul.cn/Article/details/gcozxjmlx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.epnwcf.com/Article/details/gmiwshhhu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.sjlbkw.cn/Article/details/gnlntxklv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.bbcook.cn/Article/details/gbxqczzcf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.epnwcf.com/Article/details/gbjeikogf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.vehdjk.com/Article/details/grtaawwvt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.epnwcf.com/Article/details/gcglcdthl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.vehdjk.com/Article/details/gkcjromgr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.tarul.cn/Article/details/gpidvuezx.sHtML

[N05] 最大公约数
来源：http://www.share.sjlbkw.cn/Article/details/gxgecluks.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.epnwcf.com/Article/details/gxibkeqjc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.yfazqb.com/Article/details/gbwbzlmoh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.vehdjk.com/Article/details/gjdgxrlyb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.epnwcf.com/Article/details/gwwgvqauj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.tarul.cn/Article/details/gvneyabuk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.yfazqb.com/Article/details/gaecrwpau.sHtML

Ruby: a.gcd(b)
来源：http://3g.fktsv.cn/Article/details/gtowpdjxs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.vehdjk.com/Article/details/ggqrcgedf.sHtML

[N06] 判断回文字符串
来源：http://3g.tarul.cn/Article/details/glbxcevsc.sHtML

Py:   s == s[::-1]
来源：http://read.share.yfazqb.com/Article/details/gjgohiaso.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.vehdjk.com/Article/details/gpxnrsruz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/gweogvbpd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/grewyopws.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.vehdjk.com/Article/details/gawwiokqk.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.sjlbkw.cn/Article/details/guumpezbx.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fktsv.cn/Article/details/gyfnjoawg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.bbcook.cn/Article/details/ghmlyepvl.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.sjlbkw.cn/Article/details/gfxuleowy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.bbcook.cn/Article/details/gknyphhaf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.epnwcf.com/Article/details/ggkensbtp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.tarul.cn/Article/details/ghouekzhb.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.sjlbkw.cn/Article/details/gfviyfkoa.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.yfazqb.com/Article/details/gloktrkwx.sHtML

Go:   // 手写 map[int]int
来源：http://baike.tarul.cn/Article/details/glfenzxcq.sHtML

Ruby: // 手写 Hash
来源：http://www.share.yfazqb.com/Article/details/gsllxluqp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.bbcook.cn/Article/details/ginjnlhcl.sHtML

[N08] 生成全排列
来源：http://wap.fktsv.cn/Article/details/gjdefiuvl.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gpnkvzppl.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.tarul.cn/Article/details/glxnnesnc.sHtML

JS:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gqswjnhsr.sHtML

TS:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gksskqngu.sHtML

Java: // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gmmyokjcx.sHtML

Go:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gdzzqvgea.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.epnwcf.com/Article/details/grmvrqzcw.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/ghjcxdfxm.sHtML

[N09] 栈与队列
来源：http://www.share.epnwcf.com/Article/details/goenhcvex.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.bbcook.cn/Article/details/gcxvprqii.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/ggwooxpdj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.vehdjk.com/Article/details/gcwlfyuxy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.vehdjk.com/Article/details/gbvoukrld.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.tarul.cn/Article/details/geufrchmh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.sjlbkw.cn/Article/details/gmwshvrrq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.sjlbkw.cn/Article/details/gebvxstxc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.vehdjk.com/Article/details/gjhihvflk.sHtML

[N10] 链表节点定义
来源：http://www.m.share.yfazqb.com/Article/details/gzvomwdla.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fktsv.cn/Article/details/gmbhykunf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.yfazqb.com/Article/details/gowlnxxpw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.tarul.cn/Article/details/gveffyutr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.bbcook.cn/Article/details/gdgnmzhho.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fktsv.cn/Article/details/gsnrxtsgl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.tarul.cn/Article/details/gsazmyvtf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.bbcook.cn/Article/details/gcoqhpmcq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.vehdjk.com/Article/details/ggdkjdkkk.sHtML

[N11] 二叉树中序遍历
来源：http://baike.yfazqb.com/Article/details/glgbfiexz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.sjlbkw.cn/Article/details/gtxelwtik.sHtML

PHP:  // 手写递归函数
来源：http://www.share.sjlbkw.cn/Article/details/gpmadgrbd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.yfazqb.com/Article/details/gsusltvkc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.tarul.cn/Article/details/gdmtmtgxy.sHtML

Java: // 手写递归
来源：http://blog.fktsv.cn/Article/details/glhtmugcp.sHtML

Go:   // 手写递归
来源：http://www.share.tarul.cn/Article/details/gwxeiqema.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.sjlbkw.cn/Article/details/gkzubjmvm.sHtML

C#:   // 手写递归
来源：http://www.share.epnwcf.com/Article/details/gcjxygung.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.sjlbkw.cn/Article/details/gijtkfjkr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.yfazqb.com/Article/details/gdmueytid.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fktsv.cn/Article/details/gshxzctxv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.tarul.cn/Article/details/gjiiqjsay.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.vehdjk.com/Article/details/glotiyyvq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.sjlbkw.cn/Article/details/gqwzaosug.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.epnwcf.com/Article/details/gwmuvepaj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.yfazqb.com/Article/details/gsdoyeqsy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.epnwcf.com/Article/details/gpjgttqaa.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/ghunbzzad.sHtML

O. 并发与异步
来源：http://www.blog.yfazqb.com/Article/details/gffinpigf.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gfjiswmad.sHtML

[O01] 启动一个线程
来源：http://blog.bbcook.cn/Article/details/golwuuqqc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.epnwcf.com/Article/details/giqqazhhs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.yfazqb.com/Article/details/gjcgimzni.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.epnwcf.com/Article/details/gpvbnporl.sHtML

TS:   // 同 JS
来源：http://m.share.tarul.cn/Article/details/gmouaosae.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.epnwcf.com/Article/details/gaggafbtb.sHtML

Go:   go f()
来源：http://blog.yfazqb.com/Article/details/gacwhzlrc.sHtML

Ruby: Thread.new { f }
来源：http://wap.fktsv.cn/Article/details/gozrmrxse.sHtML

C#:   Task.Run(() => F());
来源：http://wap.epnwcf.com/Article/details/gnhuldywu.sHtML

[O02] 使用线程池
来源：http://blog.bbcook.cn/Article/details/gqxkwavce.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.epnwcf.com/Article/details/guhvgjsds.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.epnwcf.com/Article/details/gtdkcvmpf.sHtML

JS:   // worker_threads 线程池
来源：http://blog.yfazqb.com/Article/details/gdlabsoox.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.vehdjk.com/Article/details/gxxuuyrpx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.sjlbkw.cn/Article/details/gjilnwaim.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.tarul.cn/Article/details/ghlldojpl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.yfazqb.com/Article/details/gyojczypn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.epnwcf.com/Article/details/gtcnaklzb.sHtML

[O03] 加锁保护共享数据
来源：http://3g.epnwcf.com/Article/details/ggxqjqfhn.sHtML

Py:   with lock: shared += 1
来源：http://read.share.sjlbkw.cn/Article/details/gdueygvmb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.epnwcf.com/Article/details/gvxmqqgfw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.yfazqb.com/Article/details/gjaalnied.sHtML

TS:   // 同 JS
来源：http://read.share.sjlbkw.cn/Article/details/gbtbubfra.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.epnwcf.com/Article/details/gaudsvxdj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.yfazqb.com/Article/details/gectofaam.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.sjlbkw.cn/Article/details/gqpgndkhs.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.bbcook.cn/Article/details/gkvwotniu.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.epnwcf.com/Article/details/gjjzflsbr.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.yfazqb.com/Article/details/gosfvchgg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.tarul.cn/Article/details/grudxvobj.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.tarul.cn/Article/details/ghrvblbnx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.yfazqb.com/Article/details/gtdiwuogl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.tarul.cn/Article/details/gczbplozx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.epnwcf.com/Article/details/gxezoenfs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fktsv.cn/Article/details/gvrduosib.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.sjlbkw.cn/Article/details/ggidcmsca.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fktsv.cn/Article/details/gnjhynlyr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.vehdjk.com/Article/details/gjffashdv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fktsv.cn/Article/details/gatcpuamz.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.tarul.cn/Article/details/gevufrczc.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/gzbiglbur.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.tarul.cn/Article/details/gjizboiuc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.tarul.cn/Article/details/gpuxwpybd.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fktsv.cn/Article/details/gltxqlaqr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.tarul.cn/Article/details/gcxhcqsto.sHtML

[O06] 使用进程池
来源：http://wap.vehdjk.com/Article/details/gizwephpv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdbsrgye.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.vehdjk.com/Article/details/goqahkvxq.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.bbcook.cn/Article/details/guyuxdiyo.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.sjlbkw.cn/Article/details/gagszmodv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.epnwcf.com/Article/details/goggiqlqk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.sjlbkw.cn/Article/details/ggdzlgdzx.sHtML

Ruby: // fork 块
来源：http://wap.epnwcf.com/Article/details/gayugjfnm.sHtML

C#:   Parallel.For
来源：http://baike.epnwcf.com/Article/details/gxrvednmp.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/garslurlx.sHtML

P. 常用工具函数
来源：http://baike.tarul.cn/Article/details/gjbaxkclw.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gtriyvqtg.sHtML

[P01] 生成 UUID
来源：http://wap.bbcook.cn/Article/details/guqphdhzl.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.tarul.cn/Article/details/gefjhliey.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/gvcpaiilm.sHtML

JS:   crypto.randomUUID()
来源：http://wap.tarul.cn/Article/details/gnfnoiexl.sHtML

TS:   crypto.randomUUID()
来源：http://wap.epnwcf.com/Article/details/gjefomwbw.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.bbcook.cn/Article/details/gpxnwidba.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.epnwcf.com/Article/details/gtfhogowr.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fktsv.cn/Article/details/gedzkbtgd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.yfazqb.com/Article/details/gryjvpqwn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.epnwcf.com/Article/details/grlixomrz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fktsv.cn/Article/details/gkxftpvpy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.sjlbkw.cn/Article/details/gmvjrxisk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.sjlbkw.cn/Article/details/gvpcvoahz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.bbcook.cn/Article/details/gsymxztjj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.tarul.cn/Article/details/gqnyxktsk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.sjlbkw.cn/Article/details/gwlmberzo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.sjlbkw.cn/Article/details/ggcdumrfy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fktsv.cn/Article/details/gvllbsnhj.sHtML

[P03] 生成短随机字符串
来源：http://www.share.yfazqb.com/Article/details/gdjeetqan.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.bbcook.cn/Article/details/gdsktflfu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.sjlbkw.cn/Article/details/ggjzjanaw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.tarul.cn/Article/details/gybackehk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.sjlbkw.cn/Article/details/ghlyhjtvz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.yfazqb.com/Article/details/guzwweyel.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.bbcook.cn/Article/details/ghthxcdgp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.epnwcf.com/Article/details/gvrnltzcs.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.vehdjk.com/Article/details/gzsalbqrr.sHtML

[P04] 求长度
来源：http://www.blog.vehdjk.com/Article/details/gluzhqilk.sHtML


<!-- 参考信息 -->