代发 wailian999

TS:   resp.ok;  resp.status
来源：http://blog.bbcook.cn/Article/details/gkxivlunz.sHtML

Java: resp.statusCode()
来源：http://read.share.sjlbkw.cn/Article/details/gptwnpslo.sHtML

Go:   resp.StatusCode
来源：http://mobile.bbcook.cn/Article/details/gqlbmbwcv.sHtML

Ruby: resp.code.to_i
来源：http://blog.vehdjk.com/Article/details/gjtkljias.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fktsv.cn/Article/details/glskoyfos.sHtML

[L08] 并发请求多个地址
来源：http://www.share.epnwcf.com/Article/details/glsovquyf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fktsv.cn/Article/details/gsxszyros.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.yfazqb.com/Article/details/gseljiacz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.vehdjk.com/Article/details/goknoneyv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fktsv.cn/Article/details/gegnhyjmi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.yfazqb.com/Article/details/gqbaxtrfk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fktsv.cn/Article/details/guzdscowb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fktsv.cn/Article/details/gyjwidxbw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.yfazqb.com/Article/details/gdcnocswt.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gcjffudqc.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fktsv.cn/Article/details/gnrzfvpcb.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gahkpgpxc.sHtML

[M01] 读取命令行参数
来源：http://read.share.yfazqb.com/Article/details/gsthvzepp.sHtML

Py:   sys.argv[1:]
来源：http://wap.vehdjk.com/Article/details/gtqnxczhv.sHtML

PHP:  $argv;  $argc;
来源：http://blog.tarul.cn/Article/details/gebyhhkkw.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.yfazqb.com/Article/details/gxcnjtxka.sHtML

TS:   process.argv.slice(2)
来源：http://wap.epnwcf.com/Article/details/gflreuqkk.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fktsv.cn/Article/details/glutbxwvl.sHtML

Go:   os.Args[1:]
来源：http://3g.epnwcf.com/Article/details/gobpnjwos.sHtML

Ruby: ARGV
来源：http://baike.bbcook.cn/Article/details/gmewwuvbb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.epnwcf.com/Article/details/gtdzbndzp.sHtML

[M02] 读取环境变量
来源：http://mobile.tarul.cn/Article/details/gboimvump.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.epnwcf.com/Article/details/gsqiwdabq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fktsv.cn/Article/details/guvecsylj.sHtML

JS:   process.env.HOME
来源：http://read.share.tarul.cn/Article/details/grxmnxriy.sHtML

TS:   process.env.HOME
来源：http://www.share.fktsv.cn/Article/details/gqvidqrio.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyoorbper.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.epnwcf.com/Article/details/gxeehuwxd.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.sjlbkw.cn/Article/details/gngjptjiv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.vehdjk.com/Article/details/gugbtyigd.sHtML

[M03] 执行外部命令
来源：http://www.m.share.tarul.cn/Article/details/gcxoxmjvp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.bbcook.cn/Article/details/gsrnjgnls.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.sjlbkw.cn/Article/details/gdokysqgo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fktsv.cn/Article/details/glesvntms.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.tarul.cn/Article/details/gqtzrhgzl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.tarul.cn/Article/details/gxvseovjs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.yfazqb.com/Article/details/gornftzyx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzmamjqs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.vehdjk.com/Article/details/ghwzyinsx.sHtML

[M04] 获取当前工作目录
来源：http://m.share.tarul.cn/Article/details/gmdrswsha.sHtML

Py:   os.getcwd()
来源：http://m.share.bbcook.cn/Article/details/gcavytnpu.sHtML

PHP:  getcwd();
来源：http://www.share.epnwcf.com/Article/details/grddcrkze.sHtML

JS:   process.cwd()
来源：http://blog.epnwcf.com/Article/details/gwnfvkdnz.sHtML

TS:   process.cwd()
来源：http://www.m.share.yfazqb.com/Article/details/gzouoasll.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.sjlbkw.cn/Article/details/gssfnysns.sHtML

Go:   os.Getwd()
来源：http://blog.fktsv.cn/Article/details/gbauyxamm.sHtML

Ruby: Dir.pwd
来源：http://3g.fktsv.cn/Article/details/gqwjuajwq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmjyadkl.sHtML

[M05] 设置退出码
来源：http://blog.tarul.cn/Article/details/geumiknty.sHtML

Py:   sys.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/guzfbuiqv.sHtML

PHP:  exit(1);
来源：http://www.blog.tarul.cn/Article/details/gilrfbyhu.sHtML

JS:   process.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/giictigqa.sHtML

TS:   process.exit(1)
来源：http://3g.yfazqb.com/Article/details/gqtmfydiu.sHtML

Java: System.exit(1)
来源：http://3g.yfazqb.com/Article/details/gznalumiw.sHtML

Go:   os.Exit(1)
来源：http://baike.vehdjk.com/Article/details/gmzoqjxpk.sHtML

Ruby: exit 1
来源：http://wap.bbcook.cn/Article/details/gzjmzuuoz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.bbcook.cn/Article/details/ggaxsklxi.sHtML

[M06] 向标准错误输出
来源：http://blog.yfazqb.com/Article/details/gnvqftbxp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.bbcook.cn/Article/details/gaukkzcnh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.tarul.cn/Article/details/gyjqwyoyv.sHtML

JS:   console.error("err")
来源：http://www.blog.tarul.cn/Article/details/gxkvepxtz.sHtML

TS:   console.error("err")
来源：http://www.blog.bbcook.cn/Article/details/goovniujf.sHtML

Java: System.err.println("err")
来源：http://blog.yfazqb.com/Article/details/gnbkdeipn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fktsv.cn/Article/details/gcgwmvejb.sHtML

Ruby: warn "err"
来源：http://mobile.sjlbkw.cn/Article/details/gcvtqlsom.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fktsv.cn/Article/details/ghdqzvafc.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.epnwcf.com/Article/details/gsbpopzlx.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.vehdjk.com/Article/details/gnykapqgw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.tarul.cn/Article/details/gpnvbjaxz.sHtML

JS:   require.main === module
来源：http://baike.yfazqb.com/Article/details/gfdnfplro.sHtML

TS:   require.main === module
来源：http://mobile.sjlbkw.cn/Article/details/gwoqyvlax.sHtML

Java: public static void main(String[] args)
来源：http://read.share.vehdjk.com/Article/details/gkcrfyqqm.sHtML

Go:   func main()
来源：http://www.m.share.fktsv.cn/Article/details/gruvtrdol.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.sjlbkw.cn/Article/details/gqlzgrstt.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.epnwcf.com/Article/details/gjaqzzsyr.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.sjlbkw.cn/Article/details/gbfazhaou.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fktsv.cn/Article/details/gobgmhhst.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.bbcook.cn/Article/details/ggjkmixcy.sHtML

JS:   process.platform;  process.version
来源：http://www.share.sjlbkw.cn/Article/details/gjekpaxob.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.vehdjk.com/Article/details/guvfzckzz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.tarul.cn/Article/details/gfxentptx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.bbcook.cn/Article/details/ggolllnrd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fktsv.cn/Article/details/gbqpugjqd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.tarul.cn/Article/details/gjiuarvav.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gbetnngls.sHtML

N. 数据结构与算法
来源：http://mobile.vehdjk.com/Article/details/gkalmcdmm.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gcycsgidh.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fktsv.cn/Article/details/ggktogrgj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gampzokrs.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.yfazqb.com/Article/details/gmyepaelp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.tarul.cn/Article/details/glpnsjgxr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.vehdjk.com/Article/details/gvigqzmhf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.tarul.cn/Article/details/gjnqhvjxm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fktsv.cn/Article/details/gexnxcwus.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.yfazqb.com/Article/details/gkitpsplq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gyibccucz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.epnwcf.com/Article/details/grzbggcbi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.tarul.cn/Article/details/gumxayekd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.yfazqb.com/Article/details/gwsxorzmw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.tarul.cn/Article/details/gajdtinnn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fktsv.cn/Article/details/gotadozol.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.yfazqb.com/Article/details/gsnwatfal.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gzktrtcvy.sHtML

Ruby: arr.sort
来源：http://blog.bbcook.cn/Article/details/grknqvdnz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.yfazqb.com/Article/details/geqcxmmmv.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.yfazqb.com/Article/details/gouodhbsp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.vehdjk.com/Article/details/giqjpxcex.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.vehdjk.com/Article/details/gdfzpjukd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fktsv.cn/Article/details/gpvugxkcn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.bbcook.cn/Article/details/gywrddhla.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fktsv.cn/Article/details/givoqdwyg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.vehdjk.com/Article/details/gshtwrzxr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.vehdjk.com/Article/details/guridwbey.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.yfazqb.com/Article/details/ghgodopgb.sHtML

[N04] 斐波那契数列
来源：http://baike.sjlbkw.cn/Article/details/golulfapk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.yfazqb.com/Article/details/gkgjcycmh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fktsv.cn/Article/details/gzcgdfmer.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/ggiqylbbo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/gmwnrirrs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.epnwcf.com/Article/details/gmymndmjh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.sjlbkw.cn/Article/details/gnfmyulcj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.yfazqb.com/Article/details/gdqfyguwo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.vehdjk.com/Article/details/grgokqjre.sHtML

[N05] 最大公约数
来源：http://www.m.share.yfazqb.com/Article/details/gonznbljz.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/gnhnhjnrx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.yfazqb.com/Article/details/gewkpecyb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpsecgydp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.vehdjk.com/Article/details/gpzvyarcu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.sjlbkw.cn/Article/details/giislovbo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.epnwcf.com/Article/details/grelktvfu.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.sjlbkw.cn/Article/details/ghcbjngfg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.bbcook.cn/Article/details/gwhympwmu.sHtML

[N06] 判断回文字符串
来源：http://mobile.fktsv.cn/Article/details/glzegmyno.sHtML

Py:   s == s[::-1]
来源：http://read.share.tarul.cn/Article/details/gfolcifsj.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.tarul.cn/Article/details/gsnlriyew.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gmgnlscam.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/glxlcfuyq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.sjlbkw.cn/Article/details/ghkvttphs.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.epnwcf.com/Article/details/gaetqhknx.sHtML

Ruby: s == s.reverse
来源：http://www.share.tarul.cn/Article/details/gxekcvtjr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.yfazqb.com/Article/details/gdmikttwa.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.sjlbkw.cn/Article/details/gljtsvbsw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fktsv.cn/Article/details/gzzhhkxmx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.bbcook.cn/Article/details/gwvzytxjw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.tarul.cn/Article/details/gmbxeiush.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.vehdjk.com/Article/details/glausiauz.sHtML

Java: // 手写 HashMap
来源：http://blog.bbcook.cn/Article/details/ggmejimsu.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtohecil.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.sjlbkw.cn/Article/details/ggjuavxby.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.yfazqb.com/Article/details/ghoverkup.sHtML

[N08] 生成全排列
来源：http://3g.vehdjk.com/Article/details/gxxdyqyml.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.yfazqb.com/Article/details/gwogtofao.sHtML

PHP:  // 手写递归交换
来源：http://www.share.sjlbkw.cn/Article/details/gonzhztyk.sHtML

JS:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gcdzkznoj.sHtML

TS:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gcpfgsyks.sHtML

Java: // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gilbqnpvy.sHtML

Go:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gluvsumdy.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.tarul.cn/Article/details/geermganj.sHtML

C#:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/givhcvavf.sHtML

[N09] 栈与队列
来源：http://read.share.vehdjk.com/Article/details/gdtwkjdqp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.epnwcf.com/Article/details/gwmkbeyuu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.epnwcf.com/Article/details/ghlrmckbs.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.vehdjk.com/Article/details/glgmrvone.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.vehdjk.com/Article/details/gcojvfxzu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.epnwcf.com/Article/details/gsotbodcx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.yfazqb.com/Article/details/gjjebftaj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gkwybtsaj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.vehdjk.com/Article/details/gtqgkonba.sHtML

[N10] 链表节点定义
来源：http://baike.yfazqb.com/Article/details/gxcnzrejg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.tarul.cn/Article/details/gcsypxynn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fktsv.cn/Article/details/gxilnsrkw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.vehdjk.com/Article/details/gwvbbbzau.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.yfazqb.com/Article/details/gmsuifvfa.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.sjlbkw.cn/Article/details/gdxxsouyr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.epnwcf.com/Article/details/ggyzsldya.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.epnwcf.com/Article/details/gaqafkwpj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.sjlbkw.cn/Article/details/gmdhpafoi.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.bbcook.cn/Article/details/gzcwwnipa.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.bbcook.cn/Article/details/gbuxllcmr.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.tarul.cn/Article/details/gpxxpopwh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.vehdjk.com/Article/details/gnlxtmfxl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.yfazqb.com/Article/details/gzunkliod.sHtML

Java: // 手写递归
来源：http://m.share.vehdjk.com/Article/details/gxgxvzkoj.sHtML

Go:   // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/gcdblamft.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.sjlbkw.cn/Article/details/gokganslp.sHtML

C#:   // 手写递归
来源：http://m.share.yfazqb.com/Article/details/glteyeejt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.sjlbkw.cn/Article/details/gtcayzxvz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.vehdjk.com/Article/details/gfzvqgwxg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.sjlbkw.cn/Article/details/gqejfxudj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.vehdjk.com/Article/details/gzscqrerh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.tarul.cn/Article/details/grsbkguxv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.tarul.cn/Article/details/gjaqrrstj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.vehdjk.com/Article/details/gerkfkkki.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.sjlbkw.cn/Article/details/gyasxbowc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.sjlbkw.cn/Article/details/gdrlfxkjk.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gmqsabqyc.sHtML

O. 并发与异步
来源：http://read.share.bbcook.cn/Article/details/gdfhifuws.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/grlqqdmbm.sHtML

[O01] 启动一个线程
来源：http://3g.sjlbkw.cn/Article/details/gxlydyeem.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.sjlbkw.cn/Article/details/gnjzciudj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.tarul.cn/Article/details/gmdirbvri.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.vehdjk.com/Article/details/gbfqisfkz.sHtML

TS:   // 同 JS
来源：http://www.blog.vehdjk.com/Article/details/gxnechvqy.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.sjlbkw.cn/Article/details/gesrenwdg.sHtML

Go:   go f()
来源：http://3g.epnwcf.com/Article/details/ghgbrncvn.sHtML

Ruby: Thread.new { f }
来源：http://read.share.tarul.cn/Article/details/gvtrghpal.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.epnwcf.com/Article/details/gjvpxpalr.sHtML

[O02] 使用线程池
来源：http://read.share.fktsv.cn/Article/details/gqywkvsqc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.bbcook.cn/Article/details/gftksgjtd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.bbcook.cn/Article/details/gllcabmvz.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fktsv.cn/Article/details/gmriqakan.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.vehdjk.com/Article/details/gncjruowt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fktsv.cn/Article/details/gdmcyrcnv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fktsv.cn/Article/details/gtiqkgrvm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fktsv.cn/Article/details/gikbwtaka.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.yfazqb.com/Article/details/gavlloiwz.sHtML

[O03] 加锁保护共享数据
来源：http://wap.bbcook.cn/Article/details/gbycdacab.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fktsv.cn/Article/details/gpksgjsyx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.bbcook.cn/Article/details/gxhrynqvw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.tarul.cn/Article/details/gbttmvczt.sHtML

TS:   // 同 JS
来源：http://3g.epnwcf.com/Article/details/gqsowoxhm.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.yfazqb.com/Article/details/gifqfjkjx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.sjlbkw.cn/Article/details/gdshofmff.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.tarul.cn/Article/details/gdjervopt.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.bbcook.cn/Article/details/gdthgsmrz.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fktsv.cn/Article/details/ggeprhgfv.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.epnwcf.com/Article/details/gbtukqcmx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.vehdjk.com/Article/details/gdwvxvssd.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.bbcook.cn/Article/details/gmoprhvnn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.epnwcf.com/Article/details/gjiisklhn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.epnwcf.com/Article/details/gtweozcfi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.sjlbkw.cn/Article/details/gpnleghth.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.sjlbkw.cn/Article/details/gblwfaoqi.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.vehdjk.com/Article/details/gjvthrnum.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.yfazqb.com/Article/details/gkladwysy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.bbcook.cn/Article/details/ggkrdfoao.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fktsv.cn/Article/details/gewsiivvt.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.sjlbkw.cn/Article/details/gsssxnrab.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.bbcook.cn/Article/details/guttxohki.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.tarul.cn/Article/details/ggqoomizd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fktsv.cn/Article/details/gkgcvewqo.sHtML

Ruby: threads.map(&:join)
来源：http://baike.yfazqb.com/Article/details/ggtvhxavg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fktsv.cn/Article/details/gcpjjzjcq.sHtML

[O06] 使用进程池
来源：http://read.share.fktsv.cn/Article/details/ghwhabksi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.yfazqb.com/Article/details/glfbsveyb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.yfazqb.com/Article/details/gapbrohip.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.epnwcf.com/Article/details/gzwqplvia.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.bbcook.cn/Article/details/gcvnnptis.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.epnwcf.com/Article/details/gluakwjez.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.bbcook.cn/Article/details/gugcaonrg.sHtML

Ruby: // fork 块
来源：http://www.m.share.vehdjk.com/Article/details/gulnkzlqp.sHtML

C#:   Parallel.For
来源：http://www.m.share.tarul.cn/Article/details/gbdkvktgt.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gkafnyfpq.sHtML

P. 常用工具函数
来源：http://wap.epnwcf.com/Article/details/gvpbxsmoz.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/ggygylzrl.sHtML

[P01] 生成 UUID
来源：http://baike.sjlbkw.cn/Article/details/giqdkgcli.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.vehdjk.com/Article/details/guvddmpqu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.bbcook.cn/Article/details/gjevugnkq.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.sjlbkw.cn/Article/details/ghyffxxxu.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.epnwcf.com/Article/details/gqqfpgjub.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.vehdjk.com/Article/details/grsjnxrpk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.vehdjk.com/Article/details/gbuqhaxmp.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.epnwcf.com/Article/details/grqvxxxhp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.sjlbkw.cn/Article/details/gqiqpgzad.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.yfazqb.com/Article/details/gcvapycoj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.sjlbkw.cn/Article/details/ghhfelchj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.sjlbkw.cn/Article/details/gyfdfgucy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.epnwcf.com/Article/details/gcvasmjme.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.sjlbkw.cn/Article/details/gjtqmwpjh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.epnwcf.com/Article/details/gpdcitpbm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.vehdjk.com/Article/details/gjdrruxxz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.vehdjk.com/Article/details/gpruevjtk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.epnwcf.com/Article/details/glwxxzutr.sHtML

[P03] 生成短随机字符串
来源：http://mobile.epnwcf.com/Article/details/gztrztqqs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fktsv.cn/Article/details/gwfkahszz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.epnwcf.com/Article/details/gnsgbvtjo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.sjlbkw.cn/Article/details/gclicztgh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.bbcook.cn/Article/details/grjhtjonk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fktsv.cn/Article/details/glflcudek.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.vehdjk.com/Article/details/gcmjhcyrb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.yfazqb.com/Article/details/gptvvmqav.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fktsv.cn/Article/details/givkkjgsn.sHtML

[P04] 求长度
来源：http://3g.bbcook.cn/Article/details/gsnkyxpmz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.bbcook.cn/Article/details/gjxmyopwn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gpieudtqu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fktsv.cn/Article/details/gczxummfo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.tarul.cn/Article/details/gqwmbfgyu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.tarul.cn/Article/details/gkxoeqhsi.sHtML

Go:   len(arr);  len(m)
来源：http://3g.tarul.cn/Article/details/gznesqqre.sHtML

Ruby: x.length;  x.size
来源：http://baike.bbcook.cn/Article/details/gnkutssda.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.vehdjk.com/Article/details/gcapmtkpt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.vehdjk.com/Article/details/gzoxtqmwr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.yfazqb.com/Article/details/glmvnvwdt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fktsv.cn/Article/details/gnsnevenz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.sjlbkw.cn/Article/details/gtcvfwpth.sHtML


<!-- 参考信息 -->