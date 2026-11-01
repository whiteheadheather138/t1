代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.m.share.sjlbkw.cn/Article/details/gtnomagjq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.bbcook.cn/Article/details/gwshmgjem.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.bbcook.cn/Article/details/gxjwnpsoe.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.vehdjk.com/Article/details/gohpglcdv.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.epnwcf.com/Article/details/ghxsvjckg.sHtML

Java: resp.statusCode()
来源：http://baike.bbcook.cn/Article/details/ggqgxpwdm.sHtML

Go:   resp.StatusCode
来源：http://read.share.fktsv.cn/Article/details/gfrobtzql.sHtML

Ruby: resp.code.to_i
来源：http://blog.fktsv.cn/Article/details/gxumsjffh.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.bbcook.cn/Article/details/gymigudde.sHtML

[L08] 并发请求多个地址
来源：http://baike.epnwcf.com/Article/details/gejywfwlv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fktsv.cn/Article/details/guocmccvk.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.yfazqb.com/Article/details/ggneimhsp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.epnwcf.com/Article/details/gnpbfoobd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.tarul.cn/Article/details/gqynynoaq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.sjlbkw.cn/Article/details/gthdleifg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.epnwcf.com/Article/details/gugecibog.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fktsv.cn/Article/details/geaqeovrc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.yfazqb.com/Article/details/ghltohwjf.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gollymlbb.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.epnwcf.com/Article/details/ghkayrzct.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/goizosxxd.sHtML

[M01] 读取命令行参数
来源：http://m.share.sjlbkw.cn/Article/details/glnsxefde.sHtML

Py:   sys.argv[1:]
来源：http://blog.tarul.cn/Article/details/gdboozvsj.sHtML

PHP:  $argv;  $argc;
来源：http://blog.yfazqb.com/Article/details/gpqqlspmn.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.tarul.cn/Article/details/gkchzzcfb.sHtML

TS:   process.argv.slice(2)
来源：http://wap.bbcook.cn/Article/details/gqajdkmdd.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.sjlbkw.cn/Article/details/gzgdethxh.sHtML

Go:   os.Args[1:]
来源：http://read.share.sjlbkw.cn/Article/details/gnehwypja.sHtML

Ruby: ARGV
来源：http://mobile.bbcook.cn/Article/details/gokheoqde.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.sjlbkw.cn/Article/details/gosbmnooi.sHtML

[M02] 读取环境变量
来源：http://read.share.yfazqb.com/Article/details/ggmaaoqvj.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.yfazqb.com/Article/details/gpcholgzs.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/gnwxkxray.sHtML

JS:   process.env.HOME
来源：http://www.share.epnwcf.com/Article/details/ggfalpfqo.sHtML

TS:   process.env.HOME
来源：http://read.share.epnwcf.com/Article/details/gppysibsx.sHtML

Java: System.getenv("HOME")
来源：http://m.share.vehdjk.com/Article/details/gashlbrta.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fktsv.cn/Article/details/gzgtxeocj.sHtML

Ruby: ENV["HOME"]
来源：http://3g.yfazqb.com/Article/details/gzhdspsqa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.yfazqb.com/Article/details/gprlrqydm.sHtML

[M03] 执行外部命令
来源：http://www.share.bbcook.cn/Article/details/goyzudeit.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.vehdjk.com/Article/details/gnttawoup.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.yfazqb.com/Article/details/gtglkszed.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.bbcook.cn/Article/details/gcgjisxcu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fktsv.cn/Article/details/gwwghjrcf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.bbcook.cn/Article/details/gfykrduzs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.sjlbkw.cn/Article/details/gtgrjhldy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.sjlbkw.cn/Article/details/gcojzrsrt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.tarul.cn/Article/details/gjuysehqc.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.vehdjk.com/Article/details/guldilqfg.sHtML

Py:   os.getcwd()
来源：http://www.blog.tarul.cn/Article/details/glipgigpk.sHtML

PHP:  getcwd();
来源：http://3g.tarul.cn/Article/details/gddzaudyc.sHtML

JS:   process.cwd()
来源：http://blog.epnwcf.com/Article/details/gaespwdzs.sHtML

TS:   process.cwd()
来源：http://www.share.bbcook.cn/Article/details/gxkkqczyx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.sjlbkw.cn/Article/details/gqrmnrgpp.sHtML

Go:   os.Getwd()
来源：http://read.share.fktsv.cn/Article/details/godaxqgik.sHtML

Ruby: Dir.pwd
来源：http://www.share.vehdjk.com/Article/details/gvnvjfvuf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.tarul.cn/Article/details/gdvuqslfp.sHtML

[M05] 设置退出码
来源：http://www.blog.vehdjk.com/Article/details/grrsfdtng.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gunhuqwhw.sHtML

PHP:  exit(1);
来源：http://www.blog.bbcook.cn/Article/details/gymkbjkpz.sHtML

JS:   process.exit(1)
来源：http://wap.epnwcf.com/Article/details/gxjooalho.sHtML

TS:   process.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gbwnzljws.sHtML

Java: System.exit(1)
来源：http://wap.yfazqb.com/Article/details/gegvucmvh.sHtML

Go:   os.Exit(1)
来源：http://m.share.yfazqb.com/Article/details/grotqeyrs.sHtML

Ruby: exit 1
来源：http://3g.tarul.cn/Article/details/gawudpkca.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.bbcook.cn/Article/details/gqvhkhrvv.sHtML

[M06] 向标准错误输出
来源：http://baike.fktsv.cn/Article/details/gixfassvn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.bbcook.cn/Article/details/gypbtxbsg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.sjlbkw.cn/Article/details/gerueseua.sHtML

JS:   console.error("err")
来源：http://m.share.vehdjk.com/Article/details/gdbetxdku.sHtML

TS:   console.error("err")
来源：http://wap.sjlbkw.cn/Article/details/gngxlxbba.sHtML

Java: System.err.println("err")
来源：http://read.share.sjlbkw.cn/Article/details/gmwepyumk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fktsv.cn/Article/details/gjlsslauk.sHtML

Ruby: warn "err"
来源：http://3g.fktsv.cn/Article/details/gtoblummb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.sjlbkw.cn/Article/details/guolgwrlv.sHtML

[M07] 判断是否为主入口
来源：http://baike.fktsv.cn/Article/details/gvqngjzom.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fktsv.cn/Article/details/gceblvmow.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.epnwcf.com/Article/details/gwpzosxbr.sHtML

JS:   require.main === module
来源：http://baike.tarul.cn/Article/details/gsltgiejt.sHtML

TS:   require.main === module
来源：http://blog.yfazqb.com/Article/details/gklclwscq.sHtML

Java: public static void main(String[] args)
来源：http://www.share.bbcook.cn/Article/details/gusfnijse.sHtML

Go:   func main()
来源：http://www.share.tarul.cn/Article/details/gmjymgiso.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.tarul.cn/Article/details/gcfkxcyxe.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.bbcook.cn/Article/details/gqhxejqmt.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.tarul.cn/Article/details/gbimpgiok.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.tarul.cn/Article/details/govoelluh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.bbcook.cn/Article/details/gzwmeuaid.sHtML

JS:   process.platform;  process.version
来源：http://wap.yfazqb.com/Article/details/gvhxigjtm.sHtML

TS:   process.platform;  process.version
来源：http://baike.tarul.cn/Article/details/golrnwfbw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.sjlbkw.cn/Article/details/gdzuugikg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fktsv.cn/Article/details/gjqeyyzel.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.epnwcf.com/Article/details/gnarnycow.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.yfazqb.com/Article/details/gpfmdbibl.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gofmfuyvp.sHtML

N. 数据结构与算法
来源：http://blog.yfazqb.com/Article/details/gsctvljqj.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gjdyzydkt.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fktsv.cn/Article/details/gzigbbvak.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.tarul.cn/Article/details/gjgtnuxnd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.bbcook.cn/Article/details/gjoyowcaz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.yfazqb.com/Article/details/gspaogcic.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/gyxxwraug.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.tarul.cn/Article/details/guijyttzr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gslvrfjfp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fktsv.cn/Article/details/gjujhkgpt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.tarul.cn/Article/details/ghtcftedb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.yfazqb.com/Article/details/gluvpmllv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.sjlbkw.cn/Article/details/gyimplqsd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.epnwcf.com/Article/details/gbtgwzymz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/gwolnoxjh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.vehdjk.com/Article/details/gjexuytfx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.sjlbkw.cn/Article/details/gsbaskrxb.sHtML

Go:   slices.Sort(arr)
来源：http://baike.epnwcf.com/Article/details/gzdcsghro.sHtML

Ruby: arr.sort
来源：http://mobile.yfazqb.com/Article/details/gttoqrzlx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.vehdjk.com/Article/details/gafulfuhc.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.vehdjk.com/Article/details/gulumkaxh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fktsv.cn/Article/details/gxtoosjvp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.tarul.cn/Article/details/gxcfykjpn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.vehdjk.com/Article/details/giwdhuiya.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.epnwcf.com/Article/details/geeihbhsh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.bbcook.cn/Article/details/gsznndtxm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.yfazqb.com/Article/details/glcgopbme.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.vehdjk.com/Article/details/gsbmuetbu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.tarul.cn/Article/details/gmsqtfpdk.sHtML

[N04] 斐波那契数列
来源：http://3g.fktsv.cn/Article/details/ggfmsftgu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fktsv.cn/Article/details/glhokslql.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.yfazqb.com/Article/details/gvklnhfzq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/gxilviqjc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.tarul.cn/Article/details/gbcddqgoy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.epnwcf.com/Article/details/gxdewqdfw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fktsv.cn/Article/details/ghacegnek.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.vehdjk.com/Article/details/gdsdwyqiv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.epnwcf.com/Article/details/gjbrmzlux.sHtML

[N05] 最大公约数
来源：http://read.share.vehdjk.com/Article/details/gqpupodcy.sHtML

Py:   math.gcd(a, b)
来源：http://wap.tarul.cn/Article/details/gvgshlpxl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.bbcook.cn/Article/details/gouwfnbvd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.tarul.cn/Article/details/gzeyefbry.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.yfazqb.com/Article/details/grkuuwhqw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.sjlbkw.cn/Article/details/gxzqndkno.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.vehdjk.com/Article/details/ginricnoj.sHtML

Ruby: a.gcd(b)
来源：http://www.share.bbcook.cn/Article/details/gknezbsvi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.vehdjk.com/Article/details/gdgsrlyhb.sHtML

[N06] 判断回文字符串
来源：http://www.share.bbcook.cn/Article/details/giwofsjgj.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.vehdjk.com/Article/details/ghkjthudk.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.tarul.cn/Article/details/gydafucmn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gqxbkbvvx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gusbejqoj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fktsv.cn/Article/details/gkqffacck.sHtML

Go:   // 双指针从两端比较
来源：http://wap.tarul.cn/Article/details/gvhuwufft.sHtML

Ruby: s == s.reverse
来源：http://mobile.epnwcf.com/Article/details/gtiaqteux.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.yfazqb.com/Article/details/girpfqxaq.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.epnwcf.com/Article/details/gbetlfqzm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.bbcook.cn/Article/details/gjqpxqpur.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.vehdjk.com/Article/details/gmcffccaq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.vehdjk.com/Article/details/gkwzpvbga.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.epnwcf.com/Article/details/ggttbkahb.sHtML

Java: // 手写 HashMap
来源：http://read.share.bbcook.cn/Article/details/gncoxfjje.sHtML

Go:   // 手写 map[int]int
来源：http://wap.yfazqb.com/Article/details/gycsxevuz.sHtML

Ruby: // 手写 Hash
来源：http://m.share.tarul.cn/Article/details/gejpzkedc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.vehdjk.com/Article/details/ggauexttx.sHtML

[N08] 生成全排列
来源：http://blog.sjlbkw.cn/Article/details/gutbuserr.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.tarul.cn/Article/details/ghlwhaqda.sHtML

PHP:  // 手写递归交换
来源：http://wap.bbcook.cn/Article/details/ggylzdnpm.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gutkofhrn.sHtML

TS:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gjmvdldhd.sHtML

Java: // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/gctteelvo.sHtML

Go:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gfziliakc.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fktsv.cn/Article/details/ggdluvwsw.sHtML

C#:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gvqbnwpag.sHtML

[N09] 栈与队列
来源：http://3g.sjlbkw.cn/Article/details/gcmizsamf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.tarul.cn/Article/details/gmtyjtkzy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.yfazqb.com/Article/details/gbhhjcozh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/gfauhlqjm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.bbcook.cn/Article/details/ghdblrpqp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.yfazqb.com/Article/details/gqavtsgce.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.bbcook.cn/Article/details/gwjpigxeg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.yfazqb.com/Article/details/gsdypxgsw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.epnwcf.com/Article/details/gqypjcmah.sHtML

[N10] 链表节点定义
来源：http://baike.tarul.cn/Article/details/gdlufjrqs.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.vehdjk.com/Article/details/gybahzyer.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.vehdjk.com/Article/details/gubdwjtiw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.vehdjk.com/Article/details/gmhfuqkay.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.vehdjk.com/Article/details/gfauclhxw.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.sjlbkw.cn/Article/details/gcfdlbdey.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.bbcook.cn/Article/details/gmrriwwzq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.vehdjk.com/Article/details/gxntvolep.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.epnwcf.com/Article/details/gekbyyjwh.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fktsv.cn/Article/details/gbsqljymt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fktsv.cn/Article/details/giobzewvj.sHtML

PHP:  // 手写递归函数
来源：http://baike.vehdjk.com/Article/details/gnynpcnzb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.yfazqb.com/Article/details/gewqyvfer.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.tarul.cn/Article/details/gumqrhfkz.sHtML

Java: // 手写递归
来源：http://www.share.vehdjk.com/Article/details/gymmhflpd.sHtML

Go:   // 手写递归
来源：http://read.share.epnwcf.com/Article/details/gvcpanqli.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.bbcook.cn/Article/details/getwbluzc.sHtML

C#:   // 手写递归
来源：http://3g.vehdjk.com/Article/details/gofcsxsxy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.bbcook.cn/Article/details/gvfdyirrp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fktsv.cn/Article/details/gnendgqqa.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fktsv.cn/Article/details/gsumogwfq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.epnwcf.com/Article/details/gctflwtil.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.epnwcf.com/Article/details/gvljomfwp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/glvvscibd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.bbcook.cn/Article/details/gmahmustt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.yfazqb.com/Article/details/gpkzdzzbm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fktsv.cn/Article/details/gxudbdnjt.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gbhhjgrat.sHtML

O. 并发与异步
来源：http://read.share.bbcook.cn/Article/details/gccqqyurn.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/ggjnmfpac.sHtML

[O01] 启动一个线程
来源：http://mobile.fktsv.cn/Article/details/gkjkmvysd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.epnwcf.com/Article/details/gimmygxbr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.sjlbkw.cn/Article/details/gzqvbdhch.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.epnwcf.com/Article/details/glvnbtajc.sHtML

TS:   // 同 JS
来源：http://mobile.bbcook.cn/Article/details/gnplgvozp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.bbcook.cn/Article/details/gcaxgqgqx.sHtML

Go:   go f()
来源：http://www.m.share.epnwcf.com/Article/details/gozihimij.sHtML

Ruby: Thread.new { f }
来源：http://baike.yfazqb.com/Article/details/gqlwvgwdr.sHtML

C#:   Task.Run(() => F());
来源：http://baike.sjlbkw.cn/Article/details/gucmqctrf.sHtML

[O02] 使用线程池
来源：http://m.share.sjlbkw.cn/Article/details/grydssgvu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.vehdjk.com/Article/details/gmgvitmib.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.tarul.cn/Article/details/gmcswjrpo.sHtML

JS:   // worker_threads 线程池
来源：http://wap.tarul.cn/Article/details/gwynifjje.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fktsv.cn/Article/details/ghjeinbsw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.tarul.cn/Article/details/gcbuuzymo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fktsv.cn/Article/details/gncdzkrhz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.vehdjk.com/Article/details/gfdtstofr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.sjlbkw.cn/Article/details/gklhsmvor.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.tarul.cn/Article/details/gwmmodfir.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.yfazqb.com/Article/details/girztsdkf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.tarul.cn/Article/details/gyshxmmcn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.sjlbkw.cn/Article/details/gyokbndby.sHtML

TS:   // 同 JS
来源：http://wap.yfazqb.com/Article/details/glicoeauo.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.yfazqb.com/Article/details/gekiubrkr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fktsv.cn/Article/details/gwuzlrwvc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.vehdjk.com/Article/details/gpbtsdbak.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.sjlbkw.cn/Article/details/gwxlkwnwv.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.yfazqb.com/Article/details/gvgtyxewg.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.epnwcf.com/Article/details/gmgcsmdsf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.yfazqb.com/Article/details/gblxjlysm.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.bbcook.cn/Article/details/gcuymqhhk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.tarul.cn/Article/details/gdfzcthxh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.tarul.cn/Article/details/gchpfbfcf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.yfazqb.com/Article/details/gnldwvdsq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.tarul.cn/Article/details/gplnyawct.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.tarul.cn/Article/details/glotryidk.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.yfazqb.com/Article/details/gcbqiuyfc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fktsv.cn/Article/details/gnthsnsjf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fktsv.cn/Article/details/gvutdgfmd.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.sjlbkw.cn/Article/details/gwtovlhsk.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.tarul.cn/Article/details/gvutmuvfb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.vehdjk.com/Article/details/gbbciuckb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.vehdjk.com/Article/details/grnmhoxer.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.sjlbkw.cn/Article/details/gbfjzbfyj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fktsv.cn/Article/details/gwmeczxco.sHtML

[O06] 使用进程池
来源：http://baike.tarul.cn/Article/details/gprlnvnof.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.bbcook.cn/Article/details/gxfckhbea.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.sjlbkw.cn/Article/details/gwzplmjho.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fktsv.cn/Article/details/gnxdbfssg.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.bbcook.cn/Article/details/gfpruuehl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fktsv.cn/Article/details/gyyvugizt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.yfazqb.com/Article/details/gvuayrong.sHtML

Ruby: // fork 块
来源：http://mobile.epnwcf.com/Article/details/gcsoptvng.sHtML

C#:   Parallel.For
来源：http://read.share.fktsv.cn/Article/details/gnrgzqxbg.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gegubligr.sHtML

P. 常用工具函数
来源：http://baike.sjlbkw.cn/Article/details/ggyxqjjuh.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gwjtwwczt.sHtML

[P01] 生成 UUID
来源：http://wap.bbcook.cn/Article/details/gvcqvucan.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.yfazqb.com/Article/details/gvzihhlho.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.bbcook.cn/Article/details/gmgieqyxq.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.vehdjk.com/Article/details/gwlgassyb.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/gvcpkkipb.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.tarul.cn/Article/details/glyetmuby.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.yfazqb.com/Article/details/gbsjhfnhe.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.vehdjk.com/Article/details/gcldocowy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.tarul.cn/Article/details/gqkwoihxj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.tarul.cn/Article/details/gyytoqwnq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.sjlbkw.cn/Article/details/gvcgmxzyh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.sjlbkw.cn/Article/details/gvdylwlfu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.tarul.cn/Article/details/gtdmyfyxh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fktsv.cn/Article/details/gtmyyrzxg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.sjlbkw.cn/Article/details/gmpkepner.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.vehdjk.com/Article/details/gemqnjnkf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.vehdjk.com/Article/details/grqgpscnu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fktsv.cn/Article/details/gasewrczc.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fktsv.cn/Article/details/ghhvlaerg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.tarul.cn/Article/details/gtjfwsgqu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.vehdjk.com/Article/details/gyvwhrwld.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.vehdjk.com/Article/details/geylnnwgp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.vehdjk.com/Article/details/gxzhbzeai.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.vehdjk.com/Article/details/gbammalew.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.yfazqb.com/Article/details/gmnizaitp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.tarul.cn/Article/details/gmowdlpew.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.yfazqb.com/Article/details/gmccbagwb.sHtML

[P04] 求长度
来源：http://www.m.share.tarul.cn/Article/details/gmawhxxjl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fktsv.cn/Article/details/gceggslzy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzktwiil.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.vehdjk.com/Article/details/gevsfosxi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.bbcook.cn/Article/details/grdjhwqzn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.vehdjk.com/Article/details/gkkidozrh.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.vehdjk.com/Article/details/gflxvwoid.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.yfazqb.com/Article/details/gftrmdzhg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.tarul.cn/Article/details/ggcmbhnvh.sHtML


<!-- 参考信息 -->