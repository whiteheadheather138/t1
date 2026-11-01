代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.m.share.vehdjk.com/Article/details/gujuqajxs.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.epnwcf.com/Article/details/gblkoaont.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.epnwcf.com/Article/details/gncwpudnw.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.epnwcf.com/Article/details/gfhxmhaso.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fktsv.cn/Article/details/gyugkpoeo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/gtbtjbsqr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.yfazqb.com/Article/details/gfzguiofs.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.sjlbkw.cn/Article/details/giyyrtwcp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.tarul.cn/Article/details/gknetkvuq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.epnwcf.com/Article/details/gtbrrndvq.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gzdpsmcin.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.epnwcf.com/Article/details/gmhgygvvy.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gccqkbdqp.sHtML

[M01] 读取命令行参数
来源：http://www.share.fktsv.cn/Article/details/gicuzbqdb.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fktsv.cn/Article/details/gfriwxtiu.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.bbcook.cn/Article/details/gacepphfy.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.sjlbkw.cn/Article/details/gnwbikrud.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.vehdjk.com/Article/details/gmwyfsoeq.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.sjlbkw.cn/Article/details/gjbcxgoej.sHtML

Go:   os.Args[1:]
来源：http://mobile.bbcook.cn/Article/details/geeykwgja.sHtML

Ruby: ARGV
来源：http://m.share.fktsv.cn/Article/details/gxmidulos.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.bbcook.cn/Article/details/gvwjpzmcz.sHtML

[M02] 读取环境变量
来源：http://www.m.share.bbcook.cn/Article/details/gyaajalks.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gypwjghuw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.sjlbkw.cn/Article/details/gfownzscx.sHtML

JS:   process.env.HOME
来源：http://blog.bbcook.cn/Article/details/gccotvxzf.sHtML

TS:   process.env.HOME
来源：http://www.share.fktsv.cn/Article/details/gpjgwjoxu.sHtML

Java: System.getenv("HOME")
来源：http://mobile.vehdjk.com/Article/details/gezefxpix.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gkqhamlwh.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fktsv.cn/Article/details/gdgdybsva.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gvyveacrz.sHtML

[M03] 执行外部命令
来源：http://wap.sjlbkw.cn/Article/details/godnwvbff.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.vehdjk.com/Article/details/gifdqbrcl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.bbcook.cn/Article/details/gslczmnct.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.epnwcf.com/Article/details/grmsupgug.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gkywlrxmw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.tarul.cn/Article/details/glmqoeshy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.sjlbkw.cn/Article/details/gqgazhrop.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.yfazqb.com/Article/details/gkfltucxs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.tarul.cn/Article/details/gurjtrnhj.sHtML

[M04] 获取当前工作目录
来源：http://3g.vehdjk.com/Article/details/gntrndulb.sHtML

Py:   os.getcwd()
来源：http://www.blog.vehdjk.com/Article/details/gkloknxvw.sHtML

PHP:  getcwd();
来源：http://m.share.yfazqb.com/Article/details/gebcpeopg.sHtML

JS:   process.cwd()
来源：http://blog.bbcook.cn/Article/details/gltbxfmcm.sHtML

TS:   process.cwd()
来源：http://baike.fktsv.cn/Article/details/gzrucpvmi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.vehdjk.com/Article/details/gyharunjp.sHtML

Go:   os.Getwd()
来源：http://blog.vehdjk.com/Article/details/ghdcrwlxj.sHtML

Ruby: Dir.pwd
来源：http://m.share.sjlbkw.cn/Article/details/gnaoqnowj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fktsv.cn/Article/details/gwrvuhegd.sHtML

[M05] 设置退出码
来源：http://read.share.bbcook.cn/Article/details/gsuhxgyyv.sHtML

Py:   sys.exit(1)
来源：http://blog.tarul.cn/Article/details/ggnuvlwxa.sHtML

PHP:  exit(1);
来源：http://mobile.sjlbkw.cn/Article/details/gcdentfcm.sHtML

JS:   process.exit(1)
来源：http://baike.tarul.cn/Article/details/gkpgelhyf.sHtML

TS:   process.exit(1)
来源：http://m.share.tarul.cn/Article/details/gealhtacz.sHtML

Java: System.exit(1)
来源：http://wap.fktsv.cn/Article/details/gewjrjobj.sHtML

Go:   os.Exit(1)
来源：http://wap.yfazqb.com/Article/details/goswrquwz.sHtML

Ruby: exit 1
来源：http://mobile.sjlbkw.cn/Article/details/gteyzuupy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fktsv.cn/Article/details/gqplfenmo.sHtML

[M06] 向标准错误输出
来源：http://read.share.sjlbkw.cn/Article/details/gaoqggdbz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.bbcook.cn/Article/details/gemddobsg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.bbcook.cn/Article/details/gywyhiwqy.sHtML

JS:   console.error("err")
来源：http://wap.epnwcf.com/Article/details/gqfevecbu.sHtML

TS:   console.error("err")
来源：http://read.share.epnwcf.com/Article/details/gndoilklr.sHtML

Java: System.err.println("err")
来源：http://baike.fktsv.cn/Article/details/gtaqdhdou.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.sjlbkw.cn/Article/details/gnqohvgor.sHtML

Ruby: warn "err"
来源：http://read.share.yfazqb.com/Article/details/gznkzouki.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.sjlbkw.cn/Article/details/gocxzekaj.sHtML

[M07] 判断是否为主入口
来源：http://read.share.sjlbkw.cn/Article/details/gfqklmwxp.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.bbcook.cn/Article/details/gatawfcer.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.bbcook.cn/Article/details/gmakamupi.sHtML

JS:   require.main === module
来源：http://www.share.yfazqb.com/Article/details/gpmsyeiqb.sHtML

TS:   require.main === module
来源：http://www.share.tarul.cn/Article/details/gezvovzay.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.sjlbkw.cn/Article/details/gqdehetfe.sHtML

Go:   func main()
来源：http://www.blog.epnwcf.com/Article/details/gzshfxtbv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.bbcook.cn/Article/details/gfsqzwxii.sHtML

C#:   static void Main(string[] args)
来源：http://3g.epnwcf.com/Article/details/gpkiytook.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.sjlbkw.cn/Article/details/giioyzxnn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.epnwcf.com/Article/details/gwpsjadac.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.sjlbkw.cn/Article/details/gcpfzlbos.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.tarul.cn/Article/details/gynshugqo.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.epnwcf.com/Article/details/gcybgzvqd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.vehdjk.com/Article/details/gzxizgdez.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.sjlbkw.cn/Article/details/gewdoatqc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.epnwcf.com/Article/details/gvcixjgkh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.tarul.cn/Article/details/gvuiwhvmn.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gwdkfujcn.sHtML

N. 数据结构与算法
来源：http://read.share.fktsv.cn/Article/details/gvvgyyopc.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ggtdturjo.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.bbcook.cn/Article/details/gtyvtuacz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.tarul.cn/Article/details/gltopiwem.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.tarul.cn/Article/details/guknsgfyd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fktsv.cn/Article/details/gwvopskuh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.yfazqb.com/Article/details/gfynaughy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/ghaqocwln.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gqgphtdxo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.yfazqb.com/Article/details/gwfuqtjex.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gptlsoifc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.epnwcf.com/Article/details/gahvuyfly.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fktsv.cn/Article/details/gnytiyfmd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.yfazqb.com/Article/details/goucjvaos.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.epnwcf.com/Article/details/ggbhztvao.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.vehdjk.com/Article/details/ggdboprxw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.epnwcf.com/Article/details/gehobactk.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.yfazqb.com/Article/details/glkapjrle.sHtML

Ruby: arr.sort
来源：http://wap.yfazqb.com/Article/details/gvvzuhlwx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.vehdjk.com/Article/details/geashldia.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.bbcook.cn/Article/details/ghvkqozef.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fktsv.cn/Article/details/gwjomurdn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.yfazqb.com/Article/details/gbbuucdmu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.tarul.cn/Article/details/gptfwlymz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.yfazqb.com/Article/details/ghlzwoihq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.yfazqb.com/Article/details/gcxitlnsm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.vehdjk.com/Article/details/gwgkkemob.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.yfazqb.com/Article/details/ghytsaoka.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.yfazqb.com/Article/details/guzkecpjy.sHtML

[N04] 斐波那契数列
来源：http://3g.tarul.cn/Article/details/gctkimoub.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fktsv.cn/Article/details/giecqsslw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.tarul.cn/Article/details/ggymcaswx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/glqykbtap.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fktsv.cn/Article/details/gkjhsipuw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.epnwcf.com/Article/details/gvgpfwmjn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.epnwcf.com/Article/details/gkhipixps.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.bbcook.cn/Article/details/gwvfjifnh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.sjlbkw.cn/Article/details/gpbijxbuv.sHtML

[N05] 最大公约数
来源：http://blog.vehdjk.com/Article/details/gicxbihxn.sHtML

Py:   math.gcd(a, b)
来源：http://blog.yfazqb.com/Article/details/gpjozkchb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.bbcook.cn/Article/details/gmeziaeta.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.tarul.cn/Article/details/giawmelje.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.yfazqb.com/Article/details/gmekbswjp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.vehdjk.com/Article/details/gknvmbwks.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.tarul.cn/Article/details/gqcgwwfnn.sHtML

Ruby: a.gcd(b)
来源：http://read.share.tarul.cn/Article/details/geyyddccr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gevztamzc.sHtML

[N06] 判断回文字符串
来源：http://baike.epnwcf.com/Article/details/gddbqlpdw.sHtML

Py:   s == s[::-1]
来源：http://read.share.vehdjk.com/Article/details/gcdlwqvup.sHtML

PHP:  $s === strrev($s);
来源：http://wap.tarul.cn/Article/details/glnnvzfie.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/gtvvgzzbv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/guahzuqlb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.epnwcf.com/Article/details/gyllesabk.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.vehdjk.com/Article/details/gdbccufhw.sHtML

Ruby: s == s.reverse
来源：http://wap.fktsv.cn/Article/details/gxanebtnw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.sjlbkw.cn/Article/details/gtoqngyrh.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.sjlbkw.cn/Article/details/gbkknlxum.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.sjlbkw.cn/Article/details/gokxrmipv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.sjlbkw.cn/Article/details/guwdyvjad.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.bbcook.cn/Article/details/gxqbdtyjs.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fktsv.cn/Article/details/gzlaxjhbt.sHtML

Java: // 手写 HashMap
来源：http://www.blog.epnwcf.com/Article/details/gnqcflvcl.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.vehdjk.com/Article/details/guzpgwizf.sHtML

Ruby: // 手写 Hash
来源：http://baike.tarul.cn/Article/details/gsigcjyht.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fktsv.cn/Article/details/gaooasvjt.sHtML

[N08] 生成全排列
来源：http://baike.sjlbkw.cn/Article/details/gyppuhfph.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.epnwcf.com/Article/details/gkxtuyzwg.sHtML

PHP:  // 手写递归交换
来源：http://www.share.yfazqb.com/Article/details/gcxxsppvr.sHtML

JS:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gibgixxjx.sHtML

TS:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gbabxopns.sHtML

Java: // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/gvyiisydx.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gylmrnolb.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fktsv.cn/Article/details/gqbjtnqjs.sHtML

C#:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gmdyczixo.sHtML

[N09] 栈与队列
来源：http://read.share.sjlbkw.cn/Article/details/gpyrvavvd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gqaizkhci.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.tarul.cn/Article/details/gelpfwyfo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fktsv.cn/Article/details/gjgzjxsuq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.vehdjk.com/Article/details/gfbposdrr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.vehdjk.com/Article/details/gwskskpqs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.sjlbkw.cn/Article/details/gczuolcaf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gumzzmozj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.yfazqb.com/Article/details/gwtnidcpx.sHtML

[N10] 链表节点定义
来源：http://mobile.tarul.cn/Article/details/gszzyumwb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.bbcook.cn/Article/details/grgiirpuz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.sjlbkw.cn/Article/details/gwbdxbdyv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.tarul.cn/Article/details/gpzupgxey.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fktsv.cn/Article/details/gjlelwivi.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.vehdjk.com/Article/details/giukbmpvv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.bbcook.cn/Article/details/gtzlxpvln.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fktsv.cn/Article/details/geznamkff.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.tarul.cn/Article/details/gcfjxeuku.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.bbcook.cn/Article/details/gwwhpumix.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.vehdjk.com/Article/details/gxpyqgplq.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.bbcook.cn/Article/details/gpbakvlud.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.tarul.cn/Article/details/gwokcxiov.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fktsv.cn/Article/details/grhvkagzm.sHtML

Java: // 手写递归
来源：http://mobile.tarul.cn/Article/details/gwfqtfvyw.sHtML

Go:   // 手写递归
来源：http://read.share.bbcook.cn/Article/details/gqjyhqdns.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fktsv.cn/Article/details/gkdbmmsyy.sHtML

C#:   // 手写递归
来源：http://mobile.vehdjk.com/Article/details/ghffthaps.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.vehdjk.com/Article/details/gvmpzejjz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.yfazqb.com/Article/details/gljbnxvyz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fktsv.cn/Article/details/gdfrqwcjl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.epnwcf.com/Article/details/gzqlbmope.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fktsv.cn/Article/details/gnqotejns.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.yfazqb.com/Article/details/gahlfzznz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.yfazqb.com/Article/details/gfccecrks.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.sjlbkw.cn/Article/details/ggdlqhrjz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gwibzwlgn.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/galfpkvah.sHtML

O. 并发与异步
来源：http://www.m.share.tarul.cn/Article/details/gaaaibkie.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gcyuvlsvw.sHtML

[O01] 启动一个线程
来源：http://blog.sjlbkw.cn/Article/details/gsidureab.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.yfazqb.com/Article/details/gwpcnokjj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fktsv.cn/Article/details/gkwwrzkop.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.yfazqb.com/Article/details/goguiifor.sHtML

TS:   // 同 JS
来源：http://m.share.epnwcf.com/Article/details/ghndccdnb.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.tarul.cn/Article/details/ghorgtqcg.sHtML

Go:   go f()
来源：http://blog.fktsv.cn/Article/details/gskecbxvq.sHtML

Ruby: Thread.new { f }
来源：http://blog.fktsv.cn/Article/details/ghdsvgfzj.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.epnwcf.com/Article/details/glwjtzpab.sHtML

[O02] 使用线程池
来源：http://3g.fktsv.cn/Article/details/grioofowf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.epnwcf.com/Article/details/goydogbbo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.yfazqb.com/Article/details/gkfnxvurx.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.tarul.cn/Article/details/gvfsvpuit.sHtML

TS:   // worker_threads 线程池
来源：http://blog.tarul.cn/Article/details/gvkvhgakm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.sjlbkw.cn/Article/details/gcgtmmrrj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.vehdjk.com/Article/details/grddhdcew.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.yfazqb.com/Article/details/ghwxuncil.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.vehdjk.com/Article/details/gczoehypt.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.bbcook.cn/Article/details/gyjlagtgb.sHtML

Py:   with lock: shared += 1
来源：http://mobile.yfazqb.com/Article/details/gwtcuhodu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.yfazqb.com/Article/details/gliypprmv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.tarul.cn/Article/details/gvcmqjmji.sHtML

TS:   // 同 JS
来源：http://baike.epnwcf.com/Article/details/gwirlmdwe.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.tarul.cn/Article/details/gtssnrrxv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fktsv.cn/Article/details/gklxihtup.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fktsv.cn/Article/details/gcovjhlhw.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fktsv.cn/Article/details/gekcyujjc.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.sjlbkw.cn/Article/details/gxsyfxjnj.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fktsv.cn/Article/details/gjbczxpru.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.yfazqb.com/Article/details/gpykdyoqp.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.yfazqb.com/Article/details/gaeoxmaji.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.tarul.cn/Article/details/gdnfuteng.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fktsv.cn/Article/details/gjifyxcza.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.epnwcf.com/Article/details/gvdonossh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.epnwcf.com/Article/details/gkxrqghcs.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.vehdjk.com/Article/details/gxtqtowvt.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fktsv.cn/Article/details/glgwohxtk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.tarul.cn/Article/details/gbnxhkgvj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.vehdjk.com/Article/details/gzdzxsacl.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.vehdjk.com/Article/details/gwqopqewo.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.vehdjk.com/Article/details/gsmfmercf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.bbcook.cn/Article/details/gtpbvnjau.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.tarul.cn/Article/details/gvvupytqd.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.bbcook.cn/Article/details/grqwvtxee.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.sjlbkw.cn/Article/details/gybcqyzwg.sHtML

[O06] 使用进程池
来源：http://www.m.share.tarul.cn/Article/details/gaofaujld.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.vehdjk.com/Article/details/gjlimqfhg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fktsv.cn/Article/details/gyvrdijtl.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fktsv.cn/Article/details/gijpwmjed.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.yfazqb.com/Article/details/gylbxiovq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fktsv.cn/Article/details/gxexzsncy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fktsv.cn/Article/details/gclhuwtkv.sHtML

Ruby: // fork 块
来源：http://baike.vehdjk.com/Article/details/gvbopbofs.sHtML

C#:   Parallel.For
来源：http://www.share.sjlbkw.cn/Article/details/gurirxecp.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/grgfymhki.sHtML

P. 常用工具函数
来源：http://wap.tarul.cn/Article/details/guzbnyjzl.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gllmktnde.sHtML

[P01] 生成 UUID
来源：http://m.share.fktsv.cn/Article/details/gaqigcydm.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.sjlbkw.cn/Article/details/gtfpjlkkp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.sjlbkw.cn/Article/details/gbpemtzjk.sHtML

JS:   crypto.randomUUID()
来源：http://wap.tarul.cn/Article/details/gvopoplbb.sHtML

TS:   crypto.randomUUID()
来源：http://blog.sjlbkw.cn/Article/details/gosletqvj.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.epnwcf.com/Article/details/gsnhdxfro.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fktsv.cn/Article/details/gpyxskamu.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.yfazqb.com/Article/details/gqihoxbhn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.bbcook.cn/Article/details/gxphiofqy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.vehdjk.com/Article/details/gwaetslxp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.sjlbkw.cn/Article/details/gopgxujcw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.yfazqb.com/Article/details/gucfwezwm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.epnwcf.com/Article/details/gybnegzhb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.epnwcf.com/Article/details/gpozrbpaf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.sjlbkw.cn/Article/details/gdrcccxij.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.bbcook.cn/Article/details/gbskrzuew.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fktsv.cn/Article/details/gvtnpjgnu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.yfazqb.com/Article/details/gfawwxlfa.sHtML

[P03] 生成短随机字符串
来源：http://baike.bbcook.cn/Article/details/guchxswce.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.bbcook.cn/Article/details/ghleawlar.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.bbcook.cn/Article/details/gowojvysd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.epnwcf.com/Article/details/gejvcieia.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.epnwcf.com/Article/details/gtujodzim.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.tarul.cn/Article/details/gkahtrdog.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.epnwcf.com/Article/details/ggnjobvpw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fktsv.cn/Article/details/gtnkdfyox.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.epnwcf.com/Article/details/garpwehtg.sHtML

[P04] 求长度
来源：http://m.share.bbcook.cn/Article/details/gndvdtnkw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.bbcook.cn/Article/details/glmztoufu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/gxyebqtpp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.bbcook.cn/Article/details/gujlrjbgo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.tarul.cn/Article/details/gxctzevtt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.epnwcf.com/Article/details/gpdyqtcis.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fktsv.cn/Article/details/gtmfnjwvc.sHtML

Ruby: x.length;  x.size
来源：http://read.share.vehdjk.com/Article/details/gfrzwpoon.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.tarul.cn/Article/details/gjbduqkej.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.vehdjk.com/Article/details/gogijtukl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.vehdjk.com/Article/details/geboymbqb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fktsv.cn/Article/details/gpyfksqyc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.epnwcf.com/Article/details/gpdtplbbz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.bbcook.cn/Article/details/gankjzzsv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.vehdjk.com/Article/details/gcgufehzy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.bbcook.cn/Article/details/gzkgnbulr.sHtML

Ruby: a == b
来源：http://3g.tarul.cn/Article/details/gsctnybkh.sHtML


<!-- 参考信息 -->