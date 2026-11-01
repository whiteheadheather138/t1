代发 wailian999

C#:   (int)resp.StatusCode
来源：http://baike.yfazqb.com/Article/details/gqnzuphvz.sHtML

[L08] 并发请求多个地址
来源：http://baike.vehdjk.com/Article/details/ghaidsxqu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.sjlbkw.cn/Article/details/gycuzdips.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.vehdjk.com/Article/details/gfxsvvfbk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.tarul.cn/Article/details/goohelamc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gosuxfykx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.sjlbkw.cn/Article/details/gdcklrkgh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fktsv.cn/Article/details/gdvvuyflb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fktsv.cn/Article/details/gnkiytrxj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fktsv.cn/Article/details/grxjdralt.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gnycxkgbi.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.yfazqb.com/Article/details/gtgbyomjs.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gavomqxsp.sHtML

[M01] 读取命令行参数
来源：http://wap.bbcook.cn/Article/details/gwyxzwrll.sHtML

Py:   sys.argv[1:]
来源：http://blog.tarul.cn/Article/details/gctnlrdst.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fktsv.cn/Article/details/grprtbwkb.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.sjlbkw.cn/Article/details/gxerozhjg.sHtML

TS:   process.argv.slice(2)
来源：http://blog.bbcook.cn/Article/details/gemqaayfb.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.bbcook.cn/Article/details/gcmtdvncx.sHtML

Go:   os.Args[1:]
来源：http://blog.epnwcf.com/Article/details/gprwtmzce.sHtML

Ruby: ARGV
来源：http://www.blog.epnwcf.com/Article/details/gaunzrwym.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.vehdjk.com/Article/details/gwazvvvaq.sHtML

[M02] 读取环境变量
来源：http://www.m.share.vehdjk.com/Article/details/guqolnaby.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.yfazqb.com/Article/details/gojkakfbl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.sjlbkw.cn/Article/details/ghhglcvhu.sHtML

JS:   process.env.HOME
来源：http://blog.epnwcf.com/Article/details/gewlakwuy.sHtML

TS:   process.env.HOME
来源：http://m.share.epnwcf.com/Article/details/gkiktpsqk.sHtML

Java: System.getenv("HOME")
来源：http://blog.bbcook.cn/Article/details/gtcvfzmyl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.bbcook.cn/Article/details/ggkahloxj.sHtML

Ruby: ENV["HOME"]
来源：http://blog.bbcook.cn/Article/details/gejfilkzf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gjkvbwdcq.sHtML

[M03] 执行外部命令
来源：http://m.share.epnwcf.com/Article/details/gvsvzszsy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.tarul.cn/Article/details/gtsidqxca.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.vehdjk.com/Article/details/gtikghtdd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.bbcook.cn/Article/details/gwfqglgaf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fktsv.cn/Article/details/gnqnvmljy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.vehdjk.com/Article/details/gtvialrvi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.vehdjk.com/Article/details/gmukzmxil.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.epnwcf.com/Article/details/gxqlijkpq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.sjlbkw.cn/Article/details/gdyxfxhav.sHtML

[M04] 获取当前工作目录
来源：http://baike.bbcook.cn/Article/details/gpkwmguyn.sHtML

Py:   os.getcwd()
来源：http://www.m.share.yfazqb.com/Article/details/gpvwpnvjx.sHtML

PHP:  getcwd();
来源：http://read.share.sjlbkw.cn/Article/details/gaeewwdqk.sHtML

JS:   process.cwd()
来源：http://mobile.yfazqb.com/Article/details/glmosnrsn.sHtML

TS:   process.cwd()
来源：http://www.blog.fktsv.cn/Article/details/gkbwzohek.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.epnwcf.com/Article/details/gcpvghqur.sHtML

Go:   os.Getwd()
来源：http://www.share.vehdjk.com/Article/details/gyuzdkhuh.sHtML

Ruby: Dir.pwd
来源：http://mobile.tarul.cn/Article/details/giwhkhcyy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.sjlbkw.cn/Article/details/gtnnlckii.sHtML

[M05] 设置退出码
来源：http://m.share.bbcook.cn/Article/details/gvmgeqgtn.sHtML

Py:   sys.exit(1)
来源：http://3g.vehdjk.com/Article/details/geisquwcu.sHtML

PHP:  exit(1);
来源：http://mobile.bbcook.cn/Article/details/gbeitkxkf.sHtML

JS:   process.exit(1)
来源：http://www.share.tarul.cn/Article/details/gqulbhxgj.sHtML

TS:   process.exit(1)
来源：http://blog.yfazqb.com/Article/details/ghyjvjylo.sHtML

Java: System.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gvhxehcmw.sHtML

Go:   os.Exit(1)
来源：http://mobile.yfazqb.com/Article/details/gxcflnkdj.sHtML

Ruby: exit 1
来源：http://blog.vehdjk.com/Article/details/gkfotzcma.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.vehdjk.com/Article/details/ghmajiaou.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.tarul.cn/Article/details/gwigiheal.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.epnwcf.com/Article/details/gqxxrdybm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fktsv.cn/Article/details/gcltmpykq.sHtML

JS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/gonypbrko.sHtML

TS:   console.error("err")
来源：http://www.blog.sjlbkw.cn/Article/details/gomakauey.sHtML

Java: System.err.println("err")
来源：http://read.share.epnwcf.com/Article/details/gcgkcidjr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fktsv.cn/Article/details/gthcsmrhh.sHtML

Ruby: warn "err"
来源：http://3g.tarul.cn/Article/details/gcgvbkofn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.vehdjk.com/Article/details/gkaxumigr.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.epnwcf.com/Article/details/gxwmhbhvx.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.epnwcf.com/Article/details/gfjuwvrii.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.sjlbkw.cn/Article/details/gsmpetwcy.sHtML

JS:   require.main === module
来源：http://mobile.epnwcf.com/Article/details/gmeychtrd.sHtML

TS:   require.main === module
来源：http://www.blog.vehdjk.com/Article/details/gaslifkon.sHtML

Java: public static void main(String[] args)
来源：http://read.share.bbcook.cn/Article/details/gxspinvgv.sHtML

Go:   func main()
来源：http://m.share.epnwcf.com/Article/details/guaidgrrl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.vehdjk.com/Article/details/gxxlkeaek.sHtML

C#:   static void Main(string[] args)
来源：http://blog.tarul.cn/Article/details/gzcwcpzyo.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.yfazqb.com/Article/details/gxyntnxlq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fktsv.cn/Article/details/gutjknqmf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fktsv.cn/Article/details/gxejsnclg.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.vehdjk.com/Article/details/ghbdmewwf.sHtML

TS:   process.platform;  process.version
来源：http://read.share.yfazqb.com/Article/details/grnydhxca.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkuypfyn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.epnwcf.com/Article/details/glcfanmpd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.yfazqb.com/Article/details/gsjelzcne.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.sjlbkw.cn/Article/details/gidvhbbve.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/guxoinbkk.sHtML

N. 数据结构与算法
来源：http://blog.vehdjk.com/Article/details/gaghzpyyh.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gxvicrtxq.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.vehdjk.com/Article/details/gzuynswvr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.tarul.cn/Article/details/gekedtiqk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.epnwcf.com/Article/details/ggveprvly.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.epnwcf.com/Article/details/gmrpguyqv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fktsv.cn/Article/details/gbbtlcoad.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.epnwcf.com/Article/details/gwwiygceo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.epnwcf.com/Article/details/gjyccjjwu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fktsv.cn/Article/details/gozotvzhe.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.tarul.cn/Article/details/ghyijizhp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.epnwcf.com/Article/details/gbwkohtgh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fktsv.cn/Article/details/gvjrynqpv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.epnwcf.com/Article/details/gbedaesyx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.yfazqb.com/Article/details/golkmntys.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.vehdjk.com/Article/details/gmzjfpudp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.vehdjk.com/Article/details/gafdllcfz.sHtML

Go:   slices.Sort(arr)
来源：http://baike.sjlbkw.cn/Article/details/gjtsovijt.sHtML

Ruby: arr.sort
来源：http://3g.vehdjk.com/Article/details/gxekdevuo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fktsv.cn/Article/details/guhgglchn.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.epnwcf.com/Article/details/gqkowzbwb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.epnwcf.com/Article/details/gywceskzz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.tarul.cn/Article/details/gyipfxgeg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.epnwcf.com/Article/details/gkyyocjuy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.tarul.cn/Article/details/grcjiibbu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.tarul.cn/Article/details/glomdytor.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.vehdjk.com/Article/details/guortigyr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.yfazqb.com/Article/details/gobneatiu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.sjlbkw.cn/Article/details/gwksjgoci.sHtML

[N04] 斐波那契数列
来源：http://read.share.bbcook.cn/Article/details/glnnchwyy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.sjlbkw.cn/Article/details/ghnsmkdhp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fktsv.cn/Article/details/gqrdntrnq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.bbcook.cn/Article/details/gmnzsopts.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/gmsiqgvbb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.yfazqb.com/Article/details/gspkgifqs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.yfazqb.com/Article/details/gzwlmffbk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.sjlbkw.cn/Article/details/gikxbcpat.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.bbcook.cn/Article/details/gxsbmixvl.sHtML

[N05] 最大公约数
来源：http://www.share.vehdjk.com/Article/details/gkgjlpzrt.sHtML

Py:   math.gcd(a, b)
来源：http://wap.yfazqb.com/Article/details/gitobkrwv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.yfazqb.com/Article/details/gmenuzdod.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.sjlbkw.cn/Article/details/ghwstmtew.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fktsv.cn/Article/details/gebfmvqio.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.bbcook.cn/Article/details/gjgrfxkil.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.epnwcf.com/Article/details/gsdrrxssr.sHtML

Ruby: a.gcd(b)
来源：http://baike.yfazqb.com/Article/details/guvlpnpqu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.epnwcf.com/Article/details/gwdkbtyqr.sHtML

[N06] 判断回文字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gfhulbbob.sHtML

Py:   s == s[::-1]
来源：http://read.share.fktsv.cn/Article/details/gubwopegf.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.yfazqb.com/Article/details/gxarpcfpi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/gqfkuglij.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gmbgizkts.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.epnwcf.com/Article/details/gsmxocwpx.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.yfazqb.com/Article/details/gsijcnyxl.sHtML

Ruby: s == s.reverse
来源：http://www.share.vehdjk.com/Article/details/gusuvfitq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.vehdjk.com/Article/details/glhqkvjno.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fktsv.cn/Article/details/golyzocpj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.vehdjk.com/Article/details/gvuysnrkt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fktsv.cn/Article/details/ggkjgqzjt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.sjlbkw.cn/Article/details/grhjcgqmy.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fktsv.cn/Article/details/ghdnblanq.sHtML

Java: // 手写 HashMap
来源：http://3g.fktsv.cn/Article/details/gqbdofjvq.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.yfazqb.com/Article/details/gobaiwgui.sHtML

Ruby: // 手写 Hash
来源：http://3g.yfazqb.com/Article/details/gcpxxwqpf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.yfazqb.com/Article/details/gbhbpxghh.sHtML

[N08] 生成全排列
来源：http://www.blog.bbcook.cn/Article/details/gcldyrnzu.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.vehdjk.com/Article/details/ghvfsveho.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fktsv.cn/Article/details/gjdfzxoyb.sHtML

JS:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gtetqokes.sHtML

TS:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gcksgoyyd.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gjirsaihu.sHtML

Go:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gbqytrchs.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.tarul.cn/Article/details/gdbgbdxgj.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gztbbekhp.sHtML

[N09] 栈与队列
来源：http://baike.fktsv.cn/Article/details/gaqpjjwun.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.epnwcf.com/Article/details/ghovmnjyf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.epnwcf.com/Article/details/gyfifckra.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gmsfxecsf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.vehdjk.com/Article/details/gvltoytix.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.sjlbkw.cn/Article/details/gxlftyeby.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.epnwcf.com/Article/details/gaxblstnq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.tarul.cn/Article/details/gnqjrjnyb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.epnwcf.com/Article/details/gewfyrpdy.sHtML

[N10] 链表节点定义
来源：http://wap.sjlbkw.cn/Article/details/gbiqcxqpo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.yfazqb.com/Article/details/gsqonheay.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.yfazqb.com/Article/details/gzrobhrma.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.yfazqb.com/Article/details/gefbxkbxo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.tarul.cn/Article/details/gafgpwfjk.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fktsv.cn/Article/details/grmtccols.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.sjlbkw.cn/Article/details/gsjyuxymr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.sjlbkw.cn/Article/details/gnxhnnrmw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.tarul.cn/Article/details/gxyejjkga.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fktsv.cn/Article/details/gozpgobdk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.sjlbkw.cn/Article/details/gmidsebap.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.vehdjk.com/Article/details/gseoisybx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.bbcook.cn/Article/details/gcjrmooux.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.epnwcf.com/Article/details/gmlilsyat.sHtML

Java: // 手写递归
来源：http://m.share.tarul.cn/Article/details/gyvldfslz.sHtML

Go:   // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gykfxfhsy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.yfazqb.com/Article/details/gervbhwla.sHtML

C#:   // 手写递归
来源：http://read.share.fktsv.cn/Article/details/gglpaacst.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.epnwcf.com/Article/details/guwmdhadk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.vehdjk.com/Article/details/gwgmdiosq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.bbcook.cn/Article/details/gzstgczxc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fktsv.cn/Article/details/gdmkbmrww.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fktsv.cn/Article/details/gnplfcxpw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.tarul.cn/Article/details/gqrzsngqe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.epnwcf.com/Article/details/gcouvkref.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.sjlbkw.cn/Article/details/ghsfgzqca.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.yfazqb.com/Article/details/goidqdjyt.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gaqjlsisn.sHtML

O. 并发与异步
来源：http://read.share.sjlbkw.cn/Article/details/ggzzhjouv.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gogtgubtd.sHtML

[O01] 启动一个线程
来源：http://www.blog.bbcook.cn/Article/details/gtvrqsymw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fktsv.cn/Article/details/gflsasmrp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.bbcook.cn/Article/details/gsnoxzkgz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.yfazqb.com/Article/details/gbgznmybq.sHtML

TS:   // 同 JS
来源：http://mobile.tarul.cn/Article/details/gomttyhlb.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.epnwcf.com/Article/details/gzsunjibn.sHtML

Go:   go f()
来源：http://www.blog.fktsv.cn/Article/details/gvyepdhgr.sHtML

Ruby: Thread.new { f }
来源：http://m.share.vehdjk.com/Article/details/gqesrnghv.sHtML

C#:   Task.Run(() => F());
来源：http://baike.vehdjk.com/Article/details/glvnshuzw.sHtML

[O02] 使用线程池
来源：http://read.share.vehdjk.com/Article/details/gahgkiyhg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fktsv.cn/Article/details/ggvleckos.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.sjlbkw.cn/Article/details/gwnfjqglt.sHtML

JS:   // worker_threads 线程池
来源：http://3g.tarul.cn/Article/details/gckorbeup.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fktsv.cn/Article/details/goxubvjql.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.epnwcf.com/Article/details/gkbdauexm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.sjlbkw.cn/Article/details/gkgxdpujn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.epnwcf.com/Article/details/gkvrxitvr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.vehdjk.com/Article/details/gfabmbirq.sHtML

[O03] 加锁保护共享数据
来源：http://wap.vehdjk.com/Article/details/gbnaowphm.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.yfazqb.com/Article/details/grpdwnyso.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.epnwcf.com/Article/details/gwinxxhom.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.epnwcf.com/Article/details/gevxtxzpi.sHtML

TS:   // 同 JS
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcqxwnfq.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.sjlbkw.cn/Article/details/gdibzijgu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.tarul.cn/Article/details/gswfgvhpz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.epnwcf.com/Article/details/gbfkvcyzs.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.vehdjk.com/Article/details/glbetyazb.sHtML

[O04] 定义异步函数并等待
来源：http://blog.epnwcf.com/Article/details/gxugsxhdv.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.yfazqb.com/Article/details/gzdmcluwd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.sjlbkw.cn/Article/details/glxtvlayu.sHtML

JS:   async function f() { await g(); }
来源：http://blog.bbcook.cn/Article/details/gwrwojqhj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.tarul.cn/Article/details/gkfifkpbk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.bbcook.cn/Article/details/gaadxtfpy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.vehdjk.com/Article/details/gjkhifaqa.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.vehdjk.com/Article/details/ggkoxtvpu.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.sjlbkw.cn/Article/details/gxwtihmqf.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.epnwcf.com/Article/details/gqcepfhwq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.epnwcf.com/Article/details/gziswmzxq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.epnwcf.com/Article/details/gduvabgmm.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.bbcook.cn/Article/details/gpodqnhua.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.sjlbkw.cn/Article/details/gjqsmefrx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.sjlbkw.cn/Article/details/gcrzkclmk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fktsv.cn/Article/details/gaankouxv.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.epnwcf.com/Article/details/gyhyyhpqr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gacmyffpn.sHtML

[O06] 使用进程池
来源：http://m.share.bbcook.cn/Article/details/guinrqpkq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.yfazqb.com/Article/details/geoiosobn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.tarul.cn/Article/details/glbsxytzk.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.vehdjk.com/Article/details/gkqiywdlg.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.vehdjk.com/Article/details/govpsctys.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.epnwcf.com/Article/details/gavvgsabn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fktsv.cn/Article/details/gnegbxcpy.sHtML

Ruby: // fork 块
来源：http://3g.yfazqb.com/Article/details/gjdyibutn.sHtML

C#:   Parallel.For
来源：http://www.m.share.bbcook.cn/Article/details/gffdjooph.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/ggwlzniok.sHtML

P. 常用工具函数
来源：http://www.m.share.bbcook.cn/Article/details/genblkudn.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gcggwrzdi.sHtML

[P01] 生成 UUID
来源：http://blog.vehdjk.com/Article/details/gtibwnnxg.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fktsv.cn/Article/details/gentttslk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fktsv.cn/Article/details/gpqxwaaeu.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrarhobh.sHtML

TS:   crypto.randomUUID()
来源：http://baike.tarul.cn/Article/details/glckvwckf.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fktsv.cn/Article/details/gohqwzoak.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.vehdjk.com/Article/details/gqgwlxeke.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.yfazqb.com/Article/details/grqurjfdt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.bbcook.cn/Article/details/glhwgyhfp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.bbcook.cn/Article/details/gywaumqdr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.vehdjk.com/Article/details/gwimdzpli.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.sjlbkw.cn/Article/details/gztzefkfk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.yfazqb.com/Article/details/gjtkvheqa.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.tarul.cn/Article/details/gfjscgwwf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.tarul.cn/Article/details/gxtmvxhvh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.sjlbkw.cn/Article/details/gfvuoqguo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.sjlbkw.cn/Article/details/gevidmolj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.sjlbkw.cn/Article/details/gwjkuzema.sHtML

[P03] 生成短随机字符串
来源：http://baike.vehdjk.com/Article/details/gkraipbpk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.yfazqb.com/Article/details/gzngzfyuo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fktsv.cn/Article/details/glvxqhgpy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.vehdjk.com/Article/details/gxwlgfohy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fktsv.cn/Article/details/gvwliiwvv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.tarul.cn/Article/details/gakuytqrp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fktsv.cn/Article/details/gxhyivdgp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.tarul.cn/Article/details/gfgbcbctx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.epnwcf.com/Article/details/geqwnmnmc.sHtML

[P04] 求长度
来源：http://blog.vehdjk.com/Article/details/gxczpyawg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.epnwcf.com/Article/details/gnyridyzj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/gbiwmixcp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.yfazqb.com/Article/details/gcehmnzmz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.yfazqb.com/Article/details/gxfiwdnws.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.epnwcf.com/Article/details/ggqvwahzs.sHtML

Go:   len(arr);  len(m)
来源：http://baike.vehdjk.com/Article/details/gdlvjxrre.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.yfazqb.com/Article/details/gioibbcuh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.yfazqb.com/Article/details/gncvkmoki.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fktsv.cn/Article/details/gspqjhcml.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.sjlbkw.cn/Article/details/ggaqxlrts.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.sjlbkw.cn/Article/details/gvxskdosu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.bbcook.cn/Article/details/gxgbfaeic.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.sjlbkw.cn/Article/details/gbsvyjumo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.vehdjk.com/Article/details/gijenvkrh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.tarul.cn/Article/details/gvhmejecl.sHtML

Ruby: a == b
来源：http://mobile.vehdjk.com/Article/details/gwrvhjrzy.sHtML


<!-- 参考信息 -->