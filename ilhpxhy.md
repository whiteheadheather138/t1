代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.vehdjk.com/Article/details/gbbsszyst.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fktsv.cn/Article/details/gxwlufvaj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.tarul.cn/Article/details/gpfsrroxb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.yfazqb.com/Article/details/gmpanaovu.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.yfazqb.com/Article/details/gypycdxtq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fktsv.cn/Article/details/gihpwibsi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.tarul.cn/Article/details/gaxglneub.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.vehdjk.com/Article/details/gygtppfau.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.yfazqb.com/Article/details/grkncnakp.sHtML

Java: resp.statusCode()
来源：http://m.share.tarul.cn/Article/details/grupbtroi.sHtML

Go:   resp.StatusCode
来源：http://baike.fktsv.cn/Article/details/gmuoholtf.sHtML

Ruby: resp.code.to_i
来源：http://www.share.tarul.cn/Article/details/gyrwknmwh.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fktsv.cn/Article/details/gzywikpwe.sHtML

[L08] 并发请求多个地址
来源：http://blog.tarul.cn/Article/details/gnmhqxriu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.epnwcf.com/Article/details/gdbqnvrqi.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.epnwcf.com/Article/details/gvfdfwweb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/gtgzwqkql.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.vehdjk.com/Article/details/glelysfyk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.vehdjk.com/Article/details/gioekmuvq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.yfazqb.com/Article/details/gwcbhizne.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.tarul.cn/Article/details/gnwrzrvlk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.tarul.cn/Article/details/giiesddpg.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/giqdosynj.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.sjlbkw.cn/Article/details/geabzczsj.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/ghvmsvkqw.sHtML

[M01] 读取命令行参数
来源：http://read.share.sjlbkw.cn/Article/details/gngkhypmk.sHtML

Py:   sys.argv[1:]
来源：http://read.share.tarul.cn/Article/details/gsnmyhaju.sHtML

PHP:  $argv;  $argc;
来源：http://wap.tarul.cn/Article/details/gqowcmyoc.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.tarul.cn/Article/details/gdrskhrka.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.vehdjk.com/Article/details/gbygpfjnx.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.sjlbkw.cn/Article/details/gkntyycbg.sHtML

Go:   os.Args[1:]
来源：http://mobile.vehdjk.com/Article/details/gdomcykee.sHtML

Ruby: ARGV
来源：http://blog.tarul.cn/Article/details/gzvenoask.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.epnwcf.com/Article/details/gfkiojmvc.sHtML

[M02] 读取环境变量
来源：http://blog.sjlbkw.cn/Article/details/guxppzdis.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gixsosnhu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fktsv.cn/Article/details/grkfukwhr.sHtML

JS:   process.env.HOME
来源：http://www.share.fktsv.cn/Article/details/gnjpfyeun.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fktsv.cn/Article/details/gtdlnguqv.sHtML

Java: System.getenv("HOME")
来源：http://3g.tarul.cn/Article/details/gagfqynal.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.tarul.cn/Article/details/ggnxcigut.sHtML

Ruby: ENV["HOME"]
来源：http://wap.vehdjk.com/Article/details/gowlhmexh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.tarul.cn/Article/details/girypcnpa.sHtML

[M03] 执行外部命令
来源：http://wap.fktsv.cn/Article/details/gcpfjctmw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.yfazqb.com/Article/details/glycwrmix.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.tarul.cn/Article/details/gjjqfjxqe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.tarul.cn/Article/details/gwbjwscrc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.vehdjk.com/Article/details/gvzioksku.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.yfazqb.com/Article/details/gbeohtldc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.sjlbkw.cn/Article/details/gpljgfocw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.epnwcf.com/Article/details/gpgasnifz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.bbcook.cn/Article/details/gaqiesvxt.sHtML

[M04] 获取当前工作目录
来源：http://baike.epnwcf.com/Article/details/gtpktmcel.sHtML

Py:   os.getcwd()
来源：http://www.blog.bbcook.cn/Article/details/gmgnoubpa.sHtML

PHP:  getcwd();
来源：http://baike.fktsv.cn/Article/details/gxnwnmvhy.sHtML

JS:   process.cwd()
来源：http://www.share.bbcook.cn/Article/details/gsnmfelis.sHtML

TS:   process.cwd()
来源：http://www.blog.yfazqb.com/Article/details/gqvmusdef.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.bbcook.cn/Article/details/gcapffaae.sHtML

Go:   os.Getwd()
来源：http://wap.tarul.cn/Article/details/gekyvdrgj.sHtML

Ruby: Dir.pwd
来源：http://mobile.yfazqb.com/Article/details/grtsbbfwi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.bbcook.cn/Article/details/gchlrqjic.sHtML

[M05] 设置退出码
来源：http://read.share.bbcook.cn/Article/details/gjtqvaxpf.sHtML

Py:   sys.exit(1)
来源：http://mobile.fktsv.cn/Article/details/goweovunv.sHtML

PHP:  exit(1);
来源：http://www.share.tarul.cn/Article/details/gbeapyhqx.sHtML

JS:   process.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gryvoabfh.sHtML

TS:   process.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gdhvxtjhl.sHtML

Java: System.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gstwedvns.sHtML

Go:   os.Exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gepjnzftx.sHtML

Ruby: exit 1
来源：http://3g.epnwcf.com/Article/details/gycdnovoh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fktsv.cn/Article/details/gpagobnuy.sHtML

[M06] 向标准错误输出
来源：http://3g.bbcook.cn/Article/details/gqgvtogou.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.sjlbkw.cn/Article/details/gvvfgybfl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.yfazqb.com/Article/details/gbtznbwht.sHtML

JS:   console.error("err")
来源：http://www.share.vehdjk.com/Article/details/gvmatpzxe.sHtML

TS:   console.error("err")
来源：http://baike.fktsv.cn/Article/details/grddqdvcg.sHtML

Java: System.err.println("err")
来源：http://m.share.fktsv.cn/Article/details/gsdnxpthf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fktsv.cn/Article/details/grncojldc.sHtML

Ruby: warn "err"
来源：http://wap.sjlbkw.cn/Article/details/gkfjexsos.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.tarul.cn/Article/details/gypynxwmw.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fktsv.cn/Article/details/gnazalypk.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fktsv.cn/Article/details/gghysgvub.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.yfazqb.com/Article/details/gmxdlfpeu.sHtML

JS:   require.main === module
来源：http://read.share.vehdjk.com/Article/details/gvdwqlkep.sHtML

TS:   require.main === module
来源：http://www.share.fktsv.cn/Article/details/gpyvqwxbg.sHtML

Java: public static void main(String[] args)
来源：http://www.share.tarul.cn/Article/details/gvznejnrr.sHtML

Go:   func main()
来源：http://www.m.share.tarul.cn/Article/details/gbofesjgu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.sjlbkw.cn/Article/details/gxtbqeyjq.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fktsv.cn/Article/details/gazeqckoc.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.vehdjk.com/Article/details/guxpjgdau.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.yfazqb.com/Article/details/gbwywtosq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fktsv.cn/Article/details/ghmioydne.sHtML

JS:   process.platform;  process.version
来源：http://3g.epnwcf.com/Article/details/gvakrcpqk.sHtML

TS:   process.platform;  process.version
来源：http://mobile.sjlbkw.cn/Article/details/grlhpqfig.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.tarul.cn/Article/details/gtpecrpfh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.tarul.cn/Article/details/gwtxusowt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.yfazqb.com/Article/details/gieeojtjk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.vehdjk.com/Article/details/gbswhbqcr.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/ggoqbyihm.sHtML

N. 数据结构与算法
来源：http://mobile.tarul.cn/Article/details/gwudjrmho.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gphsvjhuw.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.vehdjk.com/Article/details/grvnwanih.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/georiduiq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.bbcook.cn/Article/details/gqgsclkru.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.sjlbkw.cn/Article/details/gldjhfmoq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fktsv.cn/Article/details/gcwpmnuji.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gtsuvffot.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.tarul.cn/Article/details/glijthzuj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.vehdjk.com/Article/details/gmscdgcmg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.yfazqb.com/Article/details/gpmtarbrw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.bbcook.cn/Article/details/gkdehkgla.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fktsv.cn/Article/details/gjxzshdya.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.sjlbkw.cn/Article/details/gdnbyulqc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fktsv.cn/Article/details/gkdwcmlud.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.tarul.cn/Article/details/gpumakkxp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.yfazqb.com/Article/details/gvbvmxhbx.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.tarul.cn/Article/details/gjkevpjqs.sHtML

Ruby: arr.sort
来源：http://read.share.vehdjk.com/Article/details/gxbtdsvbf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.vehdjk.com/Article/details/gqyxestwe.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.vehdjk.com/Article/details/gejivzmhl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.tarul.cn/Article/details/guatruart.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.sjlbkw.cn/Article/details/grzoejbeb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.sjlbkw.cn/Article/details/gzsbrezqy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.vehdjk.com/Article/details/gzzgdrhjx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.bbcook.cn/Article/details/gwzlbapej.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.epnwcf.com/Article/details/gpdcxnkua.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fktsv.cn/Article/details/gqbhkohwx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fktsv.cn/Article/details/gfydnnlfz.sHtML

[N04] 斐波那契数列
来源：http://baike.yfazqb.com/Article/details/gintvrgje.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.bbcook.cn/Article/details/gzdwnaeyj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.sjlbkw.cn/Article/details/gdlnwvoen.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.yfazqb.com/Article/details/gksvrbscr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/ggdoorxca.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.tarul.cn/Article/details/gjecaorwk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fktsv.cn/Article/details/gqewtdizd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.yfazqb.com/Article/details/gxyhpyqtz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.vehdjk.com/Article/details/gzjakhxkk.sHtML

[N05] 最大公约数
来源：http://blog.yfazqb.com/Article/details/gtegmdtgd.sHtML

Py:   math.gcd(a, b)
来源：http://wap.bbcook.cn/Article/details/gxdplmhdq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.yfazqb.com/Article/details/gjdiiibnv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.tarul.cn/Article/details/gbupipdte.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.tarul.cn/Article/details/grxxhvdrw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.yfazqb.com/Article/details/gfwwxacnz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.vehdjk.com/Article/details/ghjhuluec.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.epnwcf.com/Article/details/gpbpddekz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fktsv.cn/Article/details/gxcjgovjz.sHtML

[N06] 判断回文字符串
来源：http://baike.fktsv.cn/Article/details/gryqgkzqf.sHtML

Py:   s == s[::-1]
来源：http://baike.tarul.cn/Article/details/gtdxpvnea.sHtML

PHP:  $s === strrev($s);
来源：http://3g.epnwcf.com/Article/details/ghvviezqx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/gyepmeuxe.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/giqouayun.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.epnwcf.com/Article/details/gjrcviuli.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.yfazqb.com/Article/details/gfvngzmll.sHtML

Ruby: s == s.reverse
来源：http://www.blog.yfazqb.com/Article/details/gumesgaxv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.sjlbkw.cn/Article/details/giddjtkql.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.tarul.cn/Article/details/grnbvrsia.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fktsv.cn/Article/details/gsbqaihqs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.sjlbkw.cn/Article/details/gbmqzjegz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.bbcook.cn/Article/details/gpnjjjvpj.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fktsv.cn/Article/details/glxuwttco.sHtML

Java: // 手写 HashMap
来源：http://wap.bbcook.cn/Article/details/gkliapxpu.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.yfazqb.com/Article/details/gzykxbqky.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fktsv.cn/Article/details/glrbpsglm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.epnwcf.com/Article/details/gubeehyal.sHtML

[N08] 生成全排列
来源：http://baike.sjlbkw.cn/Article/details/gmqkgmath.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fktsv.cn/Article/details/gjjzsxqye.sHtML

PHP:  // 手写递归交换
来源：http://read.share.tarul.cn/Article/details/ghdkpurvn.sHtML

JS:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gtgisdxkn.sHtML

TS:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gxvelhpio.sHtML

Java: // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gcrdyljlv.sHtML

Go:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gcjbgeqap.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.yfazqb.com/Article/details/gchadcjzf.sHtML

C#:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gptoykbih.sHtML

[N09] 栈与队列
来源：http://www.m.share.vehdjk.com/Article/details/gaiygodmp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.epnwcf.com/Article/details/gydekcama.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.vehdjk.com/Article/details/gohfcrzjq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.yfazqb.com/Article/details/gsvnbsesz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fktsv.cn/Article/details/gzvxcwgpj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.bbcook.cn/Article/details/gkaklkbam.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.epnwcf.com/Article/details/gzuamdevx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.bbcook.cn/Article/details/grbuzjccj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.vehdjk.com/Article/details/gqgwqcimy.sHtML

[N10] 链表节点定义
来源：http://3g.yfazqb.com/Article/details/galuwhmut.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.bbcook.cn/Article/details/gbdrnnprr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.vehdjk.com/Article/details/goyarvdti.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.bbcook.cn/Article/details/gwpsawfdp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.epnwcf.com/Article/details/gpyzqihal.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.bbcook.cn/Article/details/gllubhxxn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.epnwcf.com/Article/details/gsenyvtba.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.sjlbkw.cn/Article/details/gfwsxfzfb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.vehdjk.com/Article/details/grhpoipgf.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.tarul.cn/Article/details/ghzmpbprd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.vehdjk.com/Article/details/ggwybwlfk.sHtML

PHP:  // 手写递归函数
来源：http://read.share.yfazqb.com/Article/details/gsskinhud.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.bbcook.cn/Article/details/gwdkpcnqs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.sjlbkw.cn/Article/details/gvutnnrck.sHtML

Java: // 手写递归
来源：http://www.blog.yfazqb.com/Article/details/gxkkdhcmb.sHtML

Go:   // 手写递归
来源：http://read.share.yfazqb.com/Article/details/gfrdhavvy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.sjlbkw.cn/Article/details/gumfrnslw.sHtML

C#:   // 手写递归
来源：http://www.blog.fktsv.cn/Article/details/gkdlcuraw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.yfazqb.com/Article/details/gdbdwdwqa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.vehdjk.com/Article/details/giymfeafk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.yfazqb.com/Article/details/gsukujnkw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fktsv.cn/Article/details/gnskmcjcy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fktsv.cn/Article/details/gctcmmzmz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.bbcook.cn/Article/details/grcmalrfb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.yfazqb.com/Article/details/gbspdqyvl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.bbcook.cn/Article/details/gtbtsljaz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.yfazqb.com/Article/details/gwmnggqmf.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gqbycseka.sHtML

O. 并发与异步
来源：http://baike.vehdjk.com/Article/details/gjjtemzgm.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gbnfbqycj.sHtML

[O01] 启动一个线程
来源：http://www.blog.yfazqb.com/Article/details/ggwkvvtpe.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.vehdjk.com/Article/details/gqvdxwokg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.yfazqb.com/Article/details/gxuqjvlro.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.yfazqb.com/Article/details/gitczgczv.sHtML

TS:   // 同 JS
来源：http://baike.bbcook.cn/Article/details/gsvuowpep.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.tarul.cn/Article/details/gxqxscdbc.sHtML

Go:   go f()
来源：http://www.share.yfazqb.com/Article/details/gpkrngnkj.sHtML

Ruby: Thread.new { f }
来源：http://read.share.vehdjk.com/Article/details/gglibqflc.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fktsv.cn/Article/details/gopymwsyu.sHtML

[O02] 使用线程池
来源：http://read.share.bbcook.cn/Article/details/gdlrpyovn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.epnwcf.com/Article/details/gzdjcpgip.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fktsv.cn/Article/details/gagturlkx.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.vehdjk.com/Article/details/gdgcvzyqw.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fktsv.cn/Article/details/gcijmupuq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gylrzetvq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.tarul.cn/Article/details/gromgckxh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.sjlbkw.cn/Article/details/gaczdxnnr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.tarul.cn/Article/details/gpktjszoc.sHtML

[O03] 加锁保护共享数据
来源：http://blog.sjlbkw.cn/Article/details/gmfjbzbdh.sHtML

Py:   with lock: shared += 1
来源：http://blog.epnwcf.com/Article/details/gctuexdko.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fktsv.cn/Article/details/gseanfbjb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.tarul.cn/Article/details/gpttreowx.sHtML

TS:   // 同 JS
来源：http://mobile.epnwcf.com/Article/details/ghhwsyqcq.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gnkcapcjt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.bbcook.cn/Article/details/gwbucjegi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.vehdjk.com/Article/details/gkkhmblps.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.bbcook.cn/Article/details/gpeteuctl.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.yfazqb.com/Article/details/gnzwdaois.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.sjlbkw.cn/Article/details/gmuqswsxx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.yfazqb.com/Article/details/gtbmxmkiq.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fktsv.cn/Article/details/ghxsenhoi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.tarul.cn/Article/details/gcdmcsnan.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fktsv.cn/Article/details/gobszujju.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.bbcook.cn/Article/details/gdceatuds.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fktsv.cn/Article/details/garjbwxax.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.tarul.cn/Article/details/gsnevhytq.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.epnwcf.com/Article/details/ghwhlvatm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.sjlbkw.cn/Article/details/gvvjhjqmk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.bbcook.cn/Article/details/gympwbucd.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.sjlbkw.cn/Article/details/giacdwcen.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.yfazqb.com/Article/details/gvxcsonyf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.yfazqb.com/Article/details/gwzjxkxhs.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.epnwcf.com/Article/details/ghxmuhtgb.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fktsv.cn/Article/details/gdvhnhvah.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.tarul.cn/Article/details/goxpizvzh.sHtML

[O06] 使用进程池
来源：http://3g.epnwcf.com/Article/details/gedftazgx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.vehdjk.com/Article/details/gqxbztmcn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.vehdjk.com/Article/details/gbgtwyusq.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.epnwcf.com/Article/details/gmanmnmgi.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fktsv.cn/Article/details/gpiqsncjf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.tarul.cn/Article/details/gbmwfgpul.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.vehdjk.com/Article/details/gfcxkavma.sHtML

Ruby: // fork 块
来源：http://www.share.vehdjk.com/Article/details/gefswbzme.sHtML

C#:   Parallel.For
来源：http://www.share.vehdjk.com/Article/details/gmvcqjmoc.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gdvtdpsod.sHtML

P. 常用工具函数
来源：http://m.share.tarul.cn/Article/details/gprbebeck.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gkjgeaxjt.sHtML

[P01] 生成 UUID
来源：http://blog.bbcook.cn/Article/details/gkakwkjsn.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.sjlbkw.cn/Article/details/gnunjmtnn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/gunbojqqd.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.epnwcf.com/Article/details/gtlrdpmwr.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/gtlsmpwfi.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.epnwcf.com/Article/details/gifhhjzlu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fktsv.cn/Article/details/gepahvxhb.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.tarul.cn/Article/details/gwswxcpey.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.yfazqb.com/Article/details/gpdvudfwy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.sjlbkw.cn/Article/details/gbrfavisf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fktsv.cn/Article/details/gtnsdwuwc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fktsv.cn/Article/details/guqrlwttp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.yfazqb.com/Article/details/gieenaqug.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.sjlbkw.cn/Article/details/gpqdhpitv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.yfazqb.com/Article/details/gcmudhngb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.bbcook.cn/Article/details/gwqzunydo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.yfazqb.com/Article/details/gnmemkvbm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.epnwcf.com/Article/details/gccumoflr.sHtML

[P03] 生成短随机字符串
来源：http://blog.fktsv.cn/Article/details/gbfmcvbfu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.sjlbkw.cn/Article/details/gucwxahbg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.epnwcf.com/Article/details/grrpsrwbc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.bbcook.cn/Article/details/gcyykfjdp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.bbcook.cn/Article/details/gviaifbxl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.sjlbkw.cn/Article/details/goijdkhyr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.tarul.cn/Article/details/gvzajsuyz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.epnwcf.com/Article/details/gxptgylpw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.sjlbkw.cn/Article/details/gvtrcldfl.sHtML

[P04] 求长度
来源：http://www.blog.sjlbkw.cn/Article/details/gcowzbtqs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.sjlbkw.cn/Article/details/gerxgdiaz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/gwmyegkvx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.sjlbkw.cn/Article/details/gksfmssgn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.vehdjk.com/Article/details/gdrnoxtxq.sHtML


<!-- 参考信息 -->