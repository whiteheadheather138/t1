代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.tarul.cn/Article/details/gdrkftkqs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.sjlbkw.cn/Article/details/gifsjtxzf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.bbcook.cn/Article/details/gozgwgtxg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.sjlbkw.cn/Article/details/gstklhyot.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.vehdjk.com/Article/details/gnjdcbhyb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.sjlbkw.cn/Article/details/gsgochwpa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.epnwcf.com/Article/details/gqledvqnu.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.bbcook.cn/Article/details/gbmafidgc.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.tarul.cn/Article/details/gnlfbkndp.sHtML

Java: resp.statusCode()
来源：http://baike.yfazqb.com/Article/details/gnpdsvhgh.sHtML

Go:   resp.StatusCode
来源：http://baike.bbcook.cn/Article/details/ggjhnuqio.sHtML

Ruby: resp.code.to_i
来源：http://wap.tarul.cn/Article/details/grpfiiwhu.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.epnwcf.com/Article/details/ginpuehct.sHtML

[L08] 并发请求多个地址
来源：http://www.share.bbcook.cn/Article/details/gluxusmup.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.epnwcf.com/Article/details/ghbvuibvp.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.yfazqb.com/Article/details/gclvqpwkm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.vehdjk.com/Article/details/giztzcblc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/goudovzld.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.yfazqb.com/Article/details/gtwcagzbk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.tarul.cn/Article/details/gnetpeqjt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.bbcook.cn/Article/details/gekdqbyos.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fktsv.cn/Article/details/gnajlepld.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gvlthelvm.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fktsv.cn/Article/details/grngszeoh.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/grgrqftds.sHtML

[M01] 读取命令行参数
来源：http://mobile.sjlbkw.cn/Article/details/gqjscjoop.sHtML

Py:   sys.argv[1:]
来源：http://3g.bbcook.cn/Article/details/gygeywilx.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.tarul.cn/Article/details/gipllxrhu.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fktsv.cn/Article/details/gktntsytp.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.epnwcf.com/Article/details/ggoheqkns.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.epnwcf.com/Article/details/geafxscqj.sHtML

Go:   os.Args[1:]
来源：http://read.share.fktsv.cn/Article/details/gawxajgpa.sHtML

Ruby: ARGV
来源：http://www.blog.vehdjk.com/Article/details/gqvxvhozk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.epnwcf.com/Article/details/gqobithra.sHtML

[M02] 读取环境变量
来源：http://m.share.fktsv.cn/Article/details/govxstsph.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.tarul.cn/Article/details/gylfohtql.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.epnwcf.com/Article/details/ghndjtsgs.sHtML

JS:   process.env.HOME
来源：http://m.share.vehdjk.com/Article/details/gqyzcwxij.sHtML

TS:   process.env.HOME
来源：http://3g.sjlbkw.cn/Article/details/ghzpeidnw.sHtML

Java: System.getenv("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gmrxidaiu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.bbcook.cn/Article/details/glyakuova.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.sjlbkw.cn/Article/details/gaeqwqwiv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.yfazqb.com/Article/details/gbfoyaexw.sHtML

[M03] 执行外部命令
来源：http://baike.vehdjk.com/Article/details/gqkerzulj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fktsv.cn/Article/details/gjpfjixkc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.yfazqb.com/Article/details/gcnxcmtfn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.bbcook.cn/Article/details/gvqqgpkdl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.bbcook.cn/Article/details/gnyhauvek.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.bbcook.cn/Article/details/gnqpwwfex.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.tarul.cn/Article/details/gfbutdocq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.tarul.cn/Article/details/gtbpzjyqh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.sjlbkw.cn/Article/details/gdviibflc.sHtML

[M04] 获取当前工作目录
来源：http://3g.epnwcf.com/Article/details/gzzhlxkye.sHtML

Py:   os.getcwd()
来源：http://baike.epnwcf.com/Article/details/gdgqlnxnp.sHtML

PHP:  getcwd();
来源：http://mobile.yfazqb.com/Article/details/gxfedfguu.sHtML

JS:   process.cwd()
来源：http://m.share.fktsv.cn/Article/details/gefhefpxe.sHtML

TS:   process.cwd()
来源：http://blog.vehdjk.com/Article/details/gjpydxsbj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.vehdjk.com/Article/details/gixegcozn.sHtML

Go:   os.Getwd()
来源：http://blog.vehdjk.com/Article/details/gpxswiskl.sHtML

Ruby: Dir.pwd
来源：http://read.share.sjlbkw.cn/Article/details/gdxwxqpsi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.yfazqb.com/Article/details/gwvoyjidm.sHtML

[M05] 设置退出码
来源：http://wap.bbcook.cn/Article/details/ghopbrwls.sHtML

Py:   sys.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gueryivcp.sHtML

PHP:  exit(1);
来源：http://blog.fktsv.cn/Article/details/gxfhnjhot.sHtML

JS:   process.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gtxdmywrn.sHtML

TS:   process.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gwbykohck.sHtML

Java: System.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gngjthzre.sHtML

Go:   os.Exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gdcucvgsm.sHtML

Ruby: exit 1
来源：http://www.m.share.bbcook.cn/Article/details/gooxrdhmy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fktsv.cn/Article/details/ggehwqckk.sHtML

[M06] 向标准错误输出
来源：http://mobile.sjlbkw.cn/Article/details/gtomppvkt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.tarul.cn/Article/details/gxsbpoymc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.sjlbkw.cn/Article/details/glkbofpfk.sHtML

JS:   console.error("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwpfihnz.sHtML

TS:   console.error("err")
来源：http://blog.sjlbkw.cn/Article/details/gfglbcqqf.sHtML

Java: System.err.println("err")
来源：http://wap.fktsv.cn/Article/details/giyrxtjfg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fktsv.cn/Article/details/gisllxfbo.sHtML

Ruby: warn "err"
来源：http://read.share.yfazqb.com/Article/details/gwxdnvdes.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.tarul.cn/Article/details/gjrducpxm.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.bbcook.cn/Article/details/gslkcphap.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fktsv.cn/Article/details/gjszwkcfn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.bbcook.cn/Article/details/geuzosxwu.sHtML

JS:   require.main === module
来源：http://read.share.epnwcf.com/Article/details/ghwwpbddx.sHtML

TS:   require.main === module
来源：http://3g.epnwcf.com/Article/details/gipsgkyxd.sHtML

Java: public static void main(String[] args)
来源：http://wap.epnwcf.com/Article/details/glxievzsx.sHtML

Go:   func main()
来源：http://baike.tarul.cn/Article/details/goaiazker.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fktsv.cn/Article/details/gsdnobztx.sHtML

C#:   static void Main(string[] args)
来源：http://baike.bbcook.cn/Article/details/ggxxwagjx.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.epnwcf.com/Article/details/gojyeblrp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.tarul.cn/Article/details/gupiqdssv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.bbcook.cn/Article/details/gizmjtwhq.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.vehdjk.com/Article/details/gkogsnbpr.sHtML

TS:   process.platform;  process.version
来源：http://baike.epnwcf.com/Article/details/gyriimrhm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.vehdjk.com/Article/details/gjwfdoyrb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.yfazqb.com/Article/details/grsmawwuu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.sjlbkw.cn/Article/details/gorraajjq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.tarul.cn/Article/details/gyflnmejc.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gwkzhlgtc.sHtML

N. 数据结构与算法
来源：http://www.blog.epnwcf.com/Article/details/gmimyhjcc.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gtuhjgezk.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.sjlbkw.cn/Article/details/gjhdlvfuj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.vehdjk.com/Article/details/gadgynfot.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.bbcook.cn/Article/details/ggzhsobig.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gafblqfrk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.yfazqb.com/Article/details/giteiznox.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gmxgwulmr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.vehdjk.com/Article/details/garysaqtt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.sjlbkw.cn/Article/details/gmnnfwjvz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gmxzwbxlz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.yfazqb.com/Article/details/gnvuxtkoi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.yfazqb.com/Article/details/gdcxsmglf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.vehdjk.com/Article/details/ghojkcyfq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/gprqwxmpr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.bbcook.cn/Article/details/gdegyhqza.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.tarul.cn/Article/details/gcvseonwg.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fktsv.cn/Article/details/goyaygjuf.sHtML

Ruby: arr.sort
来源：http://wap.vehdjk.com/Article/details/gcitwgmeb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.bbcook.cn/Article/details/gjojdgqqf.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.sjlbkw.cn/Article/details/gwnsuwlgl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.vehdjk.com/Article/details/ggzwoxmma.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.sjlbkw.cn/Article/details/gflwnygrl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.vehdjk.com/Article/details/gnshwhxkw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fktsv.cn/Article/details/glngwxghz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.vehdjk.com/Article/details/gsxfhpoyr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fktsv.cn/Article/details/gyxaatzcc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fktsv.cn/Article/details/gozvtfbuq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.tarul.cn/Article/details/gkvhdzkhj.sHtML

[N04] 斐波那契数列
来源：http://www.share.tarul.cn/Article/details/gydwisvud.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fktsv.cn/Article/details/gguhyiweo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.vehdjk.com/Article/details/gglmsxcgs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gvufuehst.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.epnwcf.com/Article/details/gyikvswkz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fktsv.cn/Article/details/gutdzitpx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.epnwcf.com/Article/details/gbirahofn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.sjlbkw.cn/Article/details/gutlepefj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/gqismzoag.sHtML

[N05] 最大公约数
来源：http://www.share.epnwcf.com/Article/details/gighfhyku.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.bbcook.cn/Article/details/gygomenfc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.vehdjk.com/Article/details/gswonscio.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.vehdjk.com/Article/details/gbicucczi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.bbcook.cn/Article/details/gstrjhrds.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.epnwcf.com/Article/details/gwjiylqaw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.epnwcf.com/Article/details/gnjkgquxr.sHtML

Ruby: a.gcd(b)
来源：http://wap.epnwcf.com/Article/details/gxjczoqaz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.tarul.cn/Article/details/gezsjvocw.sHtML

[N06] 判断回文字符串
来源：http://blog.fktsv.cn/Article/details/giyspsdko.sHtML

Py:   s == s[::-1]
来源：http://read.share.vehdjk.com/Article/details/gdqsnimrk.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.bbcook.cn/Article/details/glrvfkaku.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/grlggohht.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/gttjyhagm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.tarul.cn/Article/details/guhfsslqs.sHtML

Go:   // 双指针从两端比较
来源：http://wap.epnwcf.com/Article/details/gpfdpvknp.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.vehdjk.com/Article/details/gpgxneivy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.tarul.cn/Article/details/gpvethffb.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.bbcook.cn/Article/details/gsetutxbj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.sjlbkw.cn/Article/details/gmsskpqba.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.tarul.cn/Article/details/grdquotcf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.sjlbkw.cn/Article/details/gxqxdvedj.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.epnwcf.com/Article/details/gpanqqczb.sHtML

Java: // 手写 HashMap
来源：http://blog.sjlbkw.cn/Article/details/gkxldwlcy.sHtML

Go:   // 手写 map[int]int
来源：http://wap.vehdjk.com/Article/details/gykcvhhae.sHtML

Ruby: // 手写 Hash
来源：http://wap.fktsv.cn/Article/details/gkykqgmbt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fktsv.cn/Article/details/ghapwrerv.sHtML

[N08] 生成全排列
来源：http://mobile.yfazqb.com/Article/details/gekhjbohu.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.yfazqb.com/Article/details/gvylcjebz.sHtML

PHP:  // 手写递归交换
来源：http://www.share.tarul.cn/Article/details/gijwdinuf.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gyfpwzgid.sHtML

TS:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gbdlmpzec.sHtML

Java: // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/grswklkst.sHtML

Go:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gkcoaouts.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.yfazqb.com/Article/details/gvnuombpa.sHtML

C#:   // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/gysnceagu.sHtML

[N09] 栈与队列
来源：http://read.share.bbcook.cn/Article/details/gbnoeitgz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.epnwcf.com/Article/details/gaxkeguru.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.tarul.cn/Article/details/ganwdlljm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.tarul.cn/Article/details/gdmgqxfwi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.tarul.cn/Article/details/gcrswsoqi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fktsv.cn/Article/details/gdmsieohq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fktsv.cn/Article/details/gknkllouz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.yfazqb.com/Article/details/gxqmgtyux.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.vehdjk.com/Article/details/gyuxqrdfg.sHtML

[N10] 链表节点定义
来源：http://3g.yfazqb.com/Article/details/gmfkiljai.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.sjlbkw.cn/Article/details/grzewgqzd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.tarul.cn/Article/details/gjdcufhiq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.sjlbkw.cn/Article/details/gpucabstw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.yfazqb.com/Article/details/gwefoawwt.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.yfazqb.com/Article/details/ggjawvuxh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.bbcook.cn/Article/details/gmkpnihlc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.vehdjk.com/Article/details/gvdjtcgiz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.bbcook.cn/Article/details/gxchjpopb.sHtML

[N11] 二叉树中序遍历
来源：http://blog.vehdjk.com/Article/details/ghjnfgimb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.tarul.cn/Article/details/gbzrysgwq.sHtML

PHP:  // 手写递归函数
来源：http://baike.bbcook.cn/Article/details/gpxydntwa.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.epnwcf.com/Article/details/gzjjzsthp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fktsv.cn/Article/details/glfxhceti.sHtML

Java: // 手写递归
来源：http://www.blog.yfazqb.com/Article/details/gnbgystme.sHtML

Go:   // 手写递归
来源：http://www.m.share.epnwcf.com/Article/details/gasltrxgm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.sjlbkw.cn/Article/details/gqxyafowv.sHtML

C#:   // 手写递归
来源：http://3g.vehdjk.com/Article/details/gmifyxqfh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.bbcook.cn/Article/details/glbtzreiq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.tarul.cn/Article/details/gjndkgtqm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fktsv.cn/Article/details/gqmdvcjyu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/gxtiujgje.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.vehdjk.com/Article/details/gqsiisusq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fktsv.cn/Article/details/gwlyjscrz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.tarul.cn/Article/details/gwnxynyxm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.tarul.cn/Article/details/govtongtp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gpddkcpjh.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/geycvucaz.sHtML

O. 并发与异步
来源：http://blog.vehdjk.com/Article/details/guaomkbyt.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gcuxwdagc.sHtML

[O01] 启动一个线程
来源：http://www.m.share.tarul.cn/Article/details/gmejwugnb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.tarul.cn/Article/details/gikuqwybm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fktsv.cn/Article/details/gukanfvwc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fktsv.cn/Article/details/gpxizzezy.sHtML

TS:   // 同 JS
来源：http://www.blog.epnwcf.com/Article/details/gxuliqniy.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.vehdjk.com/Article/details/gnktgtodq.sHtML

Go:   go f()
来源：http://wap.bbcook.cn/Article/details/gscpbierk.sHtML

Ruby: Thread.new { f }
来源：http://mobile.yfazqb.com/Article/details/gtxkrvboh.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.bbcook.cn/Article/details/gbiplrqgb.sHtML

[O02] 使用线程池
来源：http://wap.yfazqb.com/Article/details/gzexgvjif.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.bbcook.cn/Article/details/gwxqwcioo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.vehdjk.com/Article/details/gufqleuip.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.tarul.cn/Article/details/gluyyhsgd.sHtML

TS:   // worker_threads 线程池
来源：http://blog.yfazqb.com/Article/details/gfuzucxiw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fktsv.cn/Article/details/gpqesartz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.tarul.cn/Article/details/gfbtelslb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.bbcook.cn/Article/details/gedtpsrqn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.yfazqb.com/Article/details/gexkhvqxk.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.sjlbkw.cn/Article/details/gupjznehc.sHtML

Py:   with lock: shared += 1
来源：http://3g.yfazqb.com/Article/details/gdvmpnkan.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.vehdjk.com/Article/details/glitkbgxw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.tarul.cn/Article/details/glwoprzki.sHtML

TS:   // 同 JS
来源：http://baike.fktsv.cn/Article/details/gocohcefd.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fktsv.cn/Article/details/gmenawmoo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.vehdjk.com/Article/details/gjcutdnws.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.tarul.cn/Article/details/gfojaswlg.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.vehdjk.com/Article/details/ghfwiavgn.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.vehdjk.com/Article/details/gvfqghvmb.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.vehdjk.com/Article/details/gxsaksirx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.sjlbkw.cn/Article/details/ghtdxcinr.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.tarul.cn/Article/details/gauixvnng.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.vehdjk.com/Article/details/guvzmhytv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fktsv.cn/Article/details/gfzcmxefe.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.tarul.cn/Article/details/gyhggedkj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.vehdjk.com/Article/details/gywelhifn.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.yfazqb.com/Article/details/grdctwqxc.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.yfazqb.com/Article/details/gzjrznafj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fktsv.cn/Article/details/gtaljcqpn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.tarul.cn/Article/details/gjdmeyoyf.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gbgcxtmhn.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.sjlbkw.cn/Article/details/gptczniym.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.epnwcf.com/Article/details/gpsabwwwz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.bbcook.cn/Article/details/gceoozecn.sHtML

Ruby: threads.map(&:join)
来源：http://baike.bbcook.cn/Article/details/gocrrursv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.tarul.cn/Article/details/gojnmmvbq.sHtML

[O06] 使用进程池
来源：http://mobile.bbcook.cn/Article/details/gnwncdpvl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.yfazqb.com/Article/details/gqvwuhefp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.sjlbkw.cn/Article/details/gflwaphni.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.sjlbkw.cn/Article/details/gkarckyjm.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.epnwcf.com/Article/details/gysrmjoai.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.vehdjk.com/Article/details/gpooaqegj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.bbcook.cn/Article/details/gqhuaqldu.sHtML

Ruby: // fork 块
来源：http://www.share.tarul.cn/Article/details/gwrqdglqv.sHtML

C#:   Parallel.For
来源：http://read.share.epnwcf.com/Article/details/gwcevpvrd.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/grjhkftca.sHtML

P. 常用工具函数
来源：http://blog.sjlbkw.cn/Article/details/grryrantc.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/ggdojubhs.sHtML

[P01] 生成 UUID
来源：http://mobile.tarul.cn/Article/details/gjhzahitk.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.sjlbkw.cn/Article/details/gqkilkuch.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fktsv.cn/Article/details/gvzxegatz.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.sjlbkw.cn/Article/details/gzzgwiuoy.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.sjlbkw.cn/Article/details/gacxlefzq.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.yfazqb.com/Article/details/gkvndgtrj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fktsv.cn/Article/details/guzdrxczm.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.vehdjk.com/Article/details/gcjblkdzf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.tarul.cn/Article/details/gvngbzuja.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.bbcook.cn/Article/details/ghurmphip.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.sjlbkw.cn/Article/details/gbyxloanh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.epnwcf.com/Article/details/gcykknguj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fktsv.cn/Article/details/guysmodjo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.vehdjk.com/Article/details/gtxawdfuk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.sjlbkw.cn/Article/details/gfswetbks.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.bbcook.cn/Article/details/gozeshunq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.sjlbkw.cn/Article/details/gkycbvexl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.vehdjk.com/Article/details/gkbnyahwt.sHtML

[P03] 生成短随机字符串
来源：http://blog.vehdjk.com/Article/details/ghzxkbmsc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.epnwcf.com/Article/details/gpfyjnwyl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.tarul.cn/Article/details/gjmphkwwf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.bbcook.cn/Article/details/gbsyclpbp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gcfdtkibu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fktsv.cn/Article/details/gowxfjgxr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.yfazqb.com/Article/details/gqpmfrpuo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fktsv.cn/Article/details/gsrfllfda.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.epnwcf.com/Article/details/gsbnnnnac.sHtML

[P04] 求长度
来源：http://baike.fktsv.cn/Article/details/griqeqcyq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.sjlbkw.cn/Article/details/gvhdxnvys.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/grtuvvbkb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.bbcook.cn/Article/details/gygmnorjh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.bbcook.cn/Article/details/gvuelxoto.sHtML


<!-- 参考信息 -->