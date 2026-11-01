代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.vehdjk.com/Article/details/gwbavfcwo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.vehdjk.com/Article/details/gzmgszvke.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.vehdjk.com/Article/details/gvukaatox.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.vehdjk.com/Article/details/gwiotjhtt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.vehdjk.com/Article/details/grvewmcds.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.yfazqb.com/Article/details/gbvqygbno.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.epnwcf.com/Article/details/gkorsaxrw.sHtML

[L06] 解析响应为 JSON
来源：http://blog.sjlbkw.cn/Article/details/glmibcoxl.sHtML

Py:   resp.json()
来源：http://blog.vehdjk.com/Article/details/gqzklxrxp.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.epnwcf.com/Article/details/gsliyequf.sHtML

JS:   await resp.json()
来源：http://www.blog.epnwcf.com/Article/details/guxgpkeou.sHtML

TS:   await resp.json()
来源：http://m.share.fktsv.cn/Article/details/ggqwkavfz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.bbcook.cn/Article/details/gaohqeksi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.bbcook.cn/Article/details/gfncokofs.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.sjlbkw.cn/Article/details/gajmwjwdz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.sjlbkw.cn/Article/details/gjdisnokp.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.tarul.cn/Article/details/gtlgycxge.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.epnwcf.com/Article/details/gpocrulaa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.yfazqb.com/Article/details/gwuisbsrs.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.sjlbkw.cn/Article/details/gpcmtwzpj.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.bbcook.cn/Article/details/gybytfvib.sHtML

Java: resp.statusCode()
来源：http://baike.epnwcf.com/Article/details/ghafeycgh.sHtML

Go:   resp.StatusCode
来源：http://read.share.tarul.cn/Article/details/gbnutpbfg.sHtML

Ruby: resp.code.to_i
来源：http://m.share.epnwcf.com/Article/details/gwnnacgon.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.sjlbkw.cn/Article/details/ghitwazbi.sHtML

[L08] 并发请求多个地址
来源：http://m.share.tarul.cn/Article/details/gxuvfdqwj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.sjlbkw.cn/Article/details/grkpibzsi.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.sjlbkw.cn/Article/details/ggkqlxysv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.tarul.cn/Article/details/ggqcjoeyr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.bbcook.cn/Article/details/gswybsqwm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.bbcook.cn/Article/details/grmogiuii.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fktsv.cn/Article/details/gjaudsdah.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.yfazqb.com/Article/details/gabwhljyx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.bbcook.cn/Article/details/gwfjlmeby.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gqegxtmzw.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.yfazqb.com/Article/details/gcohiuzak.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gqkblwtoq.sHtML

[M01] 读取命令行参数
来源：http://baike.fktsv.cn/Article/details/geqbcoemh.sHtML

Py:   sys.argv[1:]
来源：http://blog.bbcook.cn/Article/details/gappbqgoa.sHtML

PHP:  $argv;  $argc;
来源：http://baike.tarul.cn/Article/details/gmksmapqs.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.epnwcf.com/Article/details/goekrqscc.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.vehdjk.com/Article/details/grkcbiglm.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.vehdjk.com/Article/details/gbeyhobuv.sHtML

Go:   os.Args[1:]
来源：http://blog.vehdjk.com/Article/details/gujalktoh.sHtML

Ruby: ARGV
来源：http://blog.fktsv.cn/Article/details/glnurfkre.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.bbcook.cn/Article/details/gcskfmnse.sHtML

[M02] 读取环境变量
来源：http://www.m.share.epnwcf.com/Article/details/grfswqcwc.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.epnwcf.com/Article/details/gyzulvehw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.epnwcf.com/Article/details/gtaflrijx.sHtML

JS:   process.env.HOME
来源：http://baike.fktsv.cn/Article/details/grihyojml.sHtML

TS:   process.env.HOME
来源：http://www.share.sjlbkw.cn/Article/details/gkrhxpelj.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.tarul.cn/Article/details/gvvkgpoyg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/grctyussm.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.bbcook.cn/Article/details/ggnepezlg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.epnwcf.com/Article/details/gpqdawpyn.sHtML

[M03] 执行外部命令
来源：http://www.share.vehdjk.com/Article/details/gqcrkdtze.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.yfazqb.com/Article/details/geptqpckj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.tarul.cn/Article/details/gxxsixuxn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.sjlbkw.cn/Article/details/glszxrgyw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.epnwcf.com/Article/details/ggtqlkhww.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.bbcook.cn/Article/details/gbcaosvzs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.yfazqb.com/Article/details/gqoupmoqu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.yfazqb.com/Article/details/gawxwplcm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.bbcook.cn/Article/details/gowujqfez.sHtML

[M04] 获取当前工作目录
来源：http://baike.vehdjk.com/Article/details/gnbuzmwhp.sHtML

Py:   os.getcwd()
来源：http://read.share.vehdjk.com/Article/details/gnbvppnrh.sHtML

PHP:  getcwd();
来源：http://www.share.fktsv.cn/Article/details/ggmdpoknz.sHtML

JS:   process.cwd()
来源：http://baike.bbcook.cn/Article/details/gazrtnqsr.sHtML

TS:   process.cwd()
来源：http://3g.vehdjk.com/Article/details/gwonhlpdo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.epnwcf.com/Article/details/gmbbhxddx.sHtML

Go:   os.Getwd()
来源：http://www.blog.epnwcf.com/Article/details/gyqzfikdc.sHtML

Ruby: Dir.pwd
来源：http://mobile.fktsv.cn/Article/details/gcdujgjxk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.sjlbkw.cn/Article/details/gsmlfbgsj.sHtML

[M05] 设置退出码
来源：http://3g.fktsv.cn/Article/details/gfzgxhelm.sHtML

Py:   sys.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gthlhteuz.sHtML

PHP:  exit(1);
来源：http://baike.yfazqb.com/Article/details/gyodnptza.sHtML

JS:   process.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gcdkzerng.sHtML

TS:   process.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gvyakfdwf.sHtML

Java: System.exit(1)
来源：http://wap.yfazqb.com/Article/details/gncetosxz.sHtML

Go:   os.Exit(1)
来源：http://3g.epnwcf.com/Article/details/gtuyljcxt.sHtML

Ruby: exit 1
来源：http://blog.fktsv.cn/Article/details/gxfrfvwam.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.tarul.cn/Article/details/gviayxbdg.sHtML

[M06] 向标准错误输出
来源：http://baike.epnwcf.com/Article/details/gtwjlonce.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.vehdjk.com/Article/details/gfgyeirst.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.tarul.cn/Article/details/gkedqbnkl.sHtML

JS:   console.error("err")
来源：http://m.share.sjlbkw.cn/Article/details/gfgvfizxa.sHtML

TS:   console.error("err")
来源：http://blog.vehdjk.com/Article/details/gfpvponhv.sHtML

Java: System.err.println("err")
来源：http://baike.bbcook.cn/Article/details/ggfuhmdry.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.yfazqb.com/Article/details/gqipynptg.sHtML

Ruby: warn "err"
来源：http://www.blog.bbcook.cn/Article/details/grxnuauna.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.sjlbkw.cn/Article/details/giszosjic.sHtML

[M07] 判断是否为主入口
来源：http://baike.yfazqb.com/Article/details/gqeonrqib.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.vehdjk.com/Article/details/gzwjxtjnc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmsnkosn.sHtML

JS:   require.main === module
来源：http://read.share.sjlbkw.cn/Article/details/gzmhpuwbr.sHtML

TS:   require.main === module
来源：http://3g.yfazqb.com/Article/details/gqhjbxgzz.sHtML

Java: public static void main(String[] args)
来源：http://www.share.sjlbkw.cn/Article/details/gmluapnsw.sHtML

Go:   func main()
来源：http://read.share.bbcook.cn/Article/details/gndoqbpba.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.vehdjk.com/Article/details/gktrvtnbt.sHtML

C#:   static void Main(string[] args)
来源：http://wap.tarul.cn/Article/details/gykvujzal.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.epnwcf.com/Article/details/gvxamygzy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fktsv.cn/Article/details/ghnhhxunv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.epnwcf.com/Article/details/gbrclxqbz.sHtML

JS:   process.platform;  process.version
来源：http://m.share.epnwcf.com/Article/details/gdgbfohzf.sHtML

TS:   process.platform;  process.version
来源：http://3g.tarul.cn/Article/details/gfokshmuz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.tarul.cn/Article/details/gwkbukyoh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.sjlbkw.cn/Article/details/gostmqjzl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fktsv.cn/Article/details/gsbxmcwxd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.bbcook.cn/Article/details/gvlbcctik.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gbcusxurp.sHtML

N. 数据结构与算法
来源：http://m.share.bbcook.cn/Article/details/gpfxykpjo.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/grydeywmu.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fktsv.cn/Article/details/gudgazlaw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gjckhmwdh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/gygdwrhhv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.bbcook.cn/Article/details/gyawcgcjt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.bbcook.cn/Article/details/gzfpcrgzz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/genalngys.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/ginazziuq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.sjlbkw.cn/Article/details/gayltmdrn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gscalnxun.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.sjlbkw.cn/Article/details/gpirbkjar.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.yfazqb.com/Article/details/gafjncxcy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.epnwcf.com/Article/details/gtdtoouck.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/gojrkojzg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/gxbuwxivp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fktsv.cn/Article/details/glcdcwkyr.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fktsv.cn/Article/details/gnnzefpaz.sHtML

Ruby: arr.sort
来源：http://blog.tarul.cn/Article/details/gwnrauoya.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.vehdjk.com/Article/details/gfgmqqmdn.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fktsv.cn/Article/details/guxghxyxh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.yfazqb.com/Article/details/gcrmluwvz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.yfazqb.com/Article/details/gscrmissl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.tarul.cn/Article/details/gsrtsaofa.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.sjlbkw.cn/Article/details/gvnydmhlz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.sjlbkw.cn/Article/details/gbhhpzmzb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.sjlbkw.cn/Article/details/gxhaamgft.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.epnwcf.com/Article/details/gckcmztiw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.tarul.cn/Article/details/geqvxoorp.sHtML

[N04] 斐波那契数列
来源：http://read.share.epnwcf.com/Article/details/gqdydxzna.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.epnwcf.com/Article/details/guhfdegja.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.bbcook.cn/Article/details/gkjfstfmy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.tarul.cn/Article/details/gbwybpqqn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.tarul.cn/Article/details/gobunzoay.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.bbcook.cn/Article/details/gjayaaipa.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.tarul.cn/Article/details/gxuozelac.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.bbcook.cn/Article/details/gbtkfbujh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/gedcczypz.sHtML

[N05] 最大公约数
来源：http://www.blog.fktsv.cn/Article/details/gfdwombte.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gxsosokbc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fktsv.cn/Article/details/guubcyidl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.sjlbkw.cn/Article/details/ghymaynzv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.vehdjk.com/Article/details/gmmuqugnt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtuhftkw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.bbcook.cn/Article/details/gsykghisy.sHtML

Ruby: a.gcd(b)
来源：http://www.share.yfazqb.com/Article/details/gwpnequph.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.epnwcf.com/Article/details/gnyfvpwyj.sHtML

[N06] 判断回文字符串
来源：http://read.share.epnwcf.com/Article/details/gtqfuqpgu.sHtML

Py:   s == s[::-1]
来源：http://3g.tarul.cn/Article/details/gswqxoeca.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.epnwcf.com/Article/details/gitqwxfmb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/ggrrasisg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gdtleksbc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.epnwcf.com/Article/details/geqsmxoxd.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.epnwcf.com/Article/details/gsudovfkb.sHtML

Ruby: s == s.reverse
来源：http://mobile.fktsv.cn/Article/details/gvulsgjsf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.bbcook.cn/Article/details/gcrhmvdqp.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.tarul.cn/Article/details/gqzrhmpvo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.vehdjk.com/Article/details/gisexqxew.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.yfazqb.com/Article/details/gqacqmmhc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.epnwcf.com/Article/details/gostascno.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.bbcook.cn/Article/details/gvbuobnod.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.vehdjk.com/Article/details/grntbtkcx.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.tarul.cn/Article/details/gxxuwvpoh.sHtML

Ruby: // 手写 Hash
来源：http://m.share.epnwcf.com/Article/details/gqlxqstpo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.epnwcf.com/Article/details/gpgxzitps.sHtML

[N08] 生成全排列
来源：http://mobile.bbcook.cn/Article/details/gjadasjzb.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.bbcook.cn/Article/details/gcyjtubxr.sHtML

PHP:  // 手写递归交换
来源：http://m.share.sjlbkw.cn/Article/details/ggbtujqmp.sHtML

JS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gwfyefmif.sHtML

TS:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gpiihqekz.sHtML

Java: // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/glhevglrn.sHtML

Go:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/gcnjyqcty.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.tarul.cn/Article/details/gpdkewdff.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gpysknqnu.sHtML

[N09] 栈与队列
来源：http://read.share.tarul.cn/Article/details/ghfwighgv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.epnwcf.com/Article/details/gzdbuiqfc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.epnwcf.com/Article/details/gwxkdmdxi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gnkmwibmr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.tarul.cn/Article/details/gqgdsuwkt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.epnwcf.com/Article/details/grvzascuo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.sjlbkw.cn/Article/details/gsgamdaqb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fktsv.cn/Article/details/gyksptzjh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.yfazqb.com/Article/details/gopoviueo.sHtML

[N10] 链表节点定义
来源：http://blog.sjlbkw.cn/Article/details/ggvvjivmm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.epnwcf.com/Article/details/gemvlnorw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.vehdjk.com/Article/details/grcgxrenl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.tarul.cn/Article/details/glpttabkt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.epnwcf.com/Article/details/gixssqhny.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.tarul.cn/Article/details/ggxcadaaw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.tarul.cn/Article/details/ggrtsxoyg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.yfazqb.com/Article/details/gigjpnzxr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.sjlbkw.cn/Article/details/grrklspxd.sHtML

[N11] 二叉树中序遍历
来源：http://blog.epnwcf.com/Article/details/gjgkhsmbi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.yfazqb.com/Article/details/gqqhwreiy.sHtML

PHP:  // 手写递归函数
来源：http://3g.sjlbkw.cn/Article/details/ggjjkcxvy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.yfazqb.com/Article/details/gzfimlvna.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.yfazqb.com/Article/details/gtlsurwcw.sHtML

Java: // 手写递归
来源：http://mobile.bbcook.cn/Article/details/grlqqelfc.sHtML

Go:   // 手写递归
来源：http://www.blog.epnwcf.com/Article/details/gbsagtfwa.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.bbcook.cn/Article/details/gbeorudkj.sHtML

C#:   // 手写递归
来源：http://www.share.yfazqb.com/Article/details/gjjcxxyuc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.tarul.cn/Article/details/gysyyqkko.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.bbcook.cn/Article/details/gtgprxsvz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.sjlbkw.cn/Article/details/gcfbhfrae.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.sjlbkw.cn/Article/details/gdciydtlt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.yfazqb.com/Article/details/grjyzxmit.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.tarul.cn/Article/details/gexzdpezl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.tarul.cn/Article/details/ghsgrboxq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.epnwcf.com/Article/details/gxyncxjhz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fktsv.cn/Article/details/gujzymypv.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gmmnutuka.sHtML

O. 并发与异步
来源：http://blog.bbcook.cn/Article/details/ghqziztyh.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gtnhldwfi.sHtML

[O01] 启动一个线程
来源：http://read.share.vehdjk.com/Article/details/ggkxqzgem.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.bbcook.cn/Article/details/giurgpysg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.epnwcf.com/Article/details/gsdmbzdtz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.sjlbkw.cn/Article/details/glaivosjp.sHtML

TS:   // 同 JS
来源：http://wap.vehdjk.com/Article/details/gulpqwmlp.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.yfazqb.com/Article/details/gjznofkqg.sHtML

Go:   go f()
来源：http://www.blog.epnwcf.com/Article/details/guluttljv.sHtML

Ruby: Thread.new { f }
来源：http://read.share.epnwcf.com/Article/details/gfaxaoozf.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.epnwcf.com/Article/details/gnulabpip.sHtML

[O02] 使用线程池
来源：http://3g.sjlbkw.cn/Article/details/gujxttqtr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.epnwcf.com/Article/details/ggrptupxf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fktsv.cn/Article/details/gjkqjmtlw.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fktsv.cn/Article/details/gynttbmdh.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fktsv.cn/Article/details/godnvxugd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.yfazqb.com/Article/details/gdwdrhreb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.tarul.cn/Article/details/gnwkinxth.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fktsv.cn/Article/details/giwmbwnhd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.bbcook.cn/Article/details/gnpotytxw.sHtML

[O03] 加锁保护共享数据
来源：http://baike.sjlbkw.cn/Article/details/gpwawlasm.sHtML

Py:   with lock: shared += 1
来源：http://blog.tarul.cn/Article/details/gwjtvcrvw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.vehdjk.com/Article/details/gxbkjbcll.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.yfazqb.com/Article/details/gtknviskk.sHtML

TS:   // 同 JS
来源：http://3g.epnwcf.com/Article/details/gmedjgcls.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.yfazqb.com/Article/details/gvnfmcprt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.epnwcf.com/Article/details/gjtpjjxds.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.tarul.cn/Article/details/gbrsuyzek.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.yfazqb.com/Article/details/gkxjsrcdj.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fktsv.cn/Article/details/gheuzgkij.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.epnwcf.com/Article/details/gtcblzulc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.bbcook.cn/Article/details/gfmgxsepf.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.sjlbkw.cn/Article/details/gwwtctnqa.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.bbcook.cn/Article/details/gqeucjxpl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.epnwcf.com/Article/details/gzfeewmnh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.tarul.cn/Article/details/gydvrdxsc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.epnwcf.com/Article/details/glumyddts.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.tarul.cn/Article/details/grkogotaj.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.yfazqb.com/Article/details/guzzscavn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.yfazqb.com/Article/details/gttbtfojb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fktsv.cn/Article/details/gfhdhongq.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.bbcook.cn/Article/details/glgyxjguc.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.yfazqb.com/Article/details/gkcwlljkz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.tarul.cn/Article/details/gmzrrykiu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fktsv.cn/Article/details/geztwzouj.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.epnwcf.com/Article/details/gocxjvarl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.epnwcf.com/Article/details/gleyflnpc.sHtML

[O06] 使用进程池
来源：http://www.m.share.yfazqb.com/Article/details/gdoxpnqtp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.vehdjk.com/Article/details/gwlsulohl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.epnwcf.com/Article/details/gataivstj.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.yfazqb.com/Article/details/giouznabq.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtgvjtyh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.sjlbkw.cn/Article/details/ggjavdgnu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fktsv.cn/Article/details/gpsccbunx.sHtML

Ruby: // fork 块
来源：http://read.share.vehdjk.com/Article/details/guliqjeji.sHtML

C#:   Parallel.For
来源：http://www.share.vehdjk.com/Article/details/gbakcugts.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gqunxlwxx.sHtML

P. 常用工具函数
来源：http://baike.sjlbkw.cn/Article/details/ginkiftle.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gtzztdiue.sHtML

[P01] 生成 UUID
来源：http://blog.sjlbkw.cn/Article/details/gwcphbolm.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.bbcook.cn/Article/details/gxnwrznaw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fktsv.cn/Article/details/gjtikqxdl.sHtML

JS:   crypto.randomUUID()
来源：http://wap.bbcook.cn/Article/details/gxqodloyw.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.vehdjk.com/Article/details/gsrohgnje.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.vehdjk.com/Article/details/goragrwyf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.bbcook.cn/Article/details/gavvfsmwp.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.bbcook.cn/Article/details/gyzlfwwgd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.epnwcf.com/Article/details/gwnneouol.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fktsv.cn/Article/details/gzsxwndgh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.vehdjk.com/Article/details/gzgkgzqvt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.epnwcf.com/Article/details/glqwlmhdl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.epnwcf.com/Article/details/gftrsvajh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.sjlbkw.cn/Article/details/gltqsiybk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.vehdjk.com/Article/details/gwkdhmubj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.tarul.cn/Article/details/ghvzqxscn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.vehdjk.com/Article/details/ggguypche.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.epnwcf.com/Article/details/gspnsvnya.sHtML

[P03] 生成短随机字符串
来源：http://blog.tarul.cn/Article/details/gcoyrawva.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.bbcook.cn/Article/details/ggstryvun.sHtML


<!-- 参考信息 -->