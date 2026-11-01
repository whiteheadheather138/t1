代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.vehdjk.com/Article/details/gxzxvghhd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.sjlbkw.cn/Article/details/gqtvvmzkd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.epnwcf.com/Article/details/gwgrwehdu.sHtML

[L06] 解析响应为 JSON
来源：http://wap.yfazqb.com/Article/details/gpryzijqz.sHtML

Py:   resp.json()
来源：http://3g.epnwcf.com/Article/details/gpboziwvz.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.sjlbkw.cn/Article/details/givnjxkcl.sHtML

JS:   await resp.json()
来源：http://mobile.bbcook.cn/Article/details/gbcrbgtpa.sHtML

TS:   await resp.json()
来源：http://www.m.share.vehdjk.com/Article/details/gzavtqwwo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.epnwcf.com/Article/details/guknurgaa.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fktsv.cn/Article/details/gzaggeptx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.tarul.cn/Article/details/gztqzkrei.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.bbcook.cn/Article/details/gqaqvkhby.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.vehdjk.com/Article/details/ggffmzbjr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.tarul.cn/Article/details/geozjozkz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fktsv.cn/Article/details/gfizzftje.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.vehdjk.com/Article/details/gdwaxdnve.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.bbcook.cn/Article/details/gzhcllzuw.sHtML

Java: resp.statusCode()
来源：http://wap.yfazqb.com/Article/details/gefukxgss.sHtML

Go:   resp.StatusCode
来源：http://read.share.epnwcf.com/Article/details/gpvcxazaj.sHtML

Ruby: resp.code.to_i
来源：http://m.share.vehdjk.com/Article/details/gtreomcjw.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.vehdjk.com/Article/details/gktaseciz.sHtML

[L08] 并发请求多个地址
来源：http://www.share.yfazqb.com/Article/details/gmuyopkuo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.vehdjk.com/Article/details/gbrhebgok.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.sjlbkw.cn/Article/details/gjivvvzat.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/gfqajgroy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.yfazqb.com/Article/details/gpbhsymva.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.sjlbkw.cn/Article/details/glwzpeypl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.tarul.cn/Article/details/gnlgpympn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcpxnuxxu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fktsv.cn/Article/details/gueuyvose.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/golmoskqw.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.epnwcf.com/Article/details/giriaezzw.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gryiadtoh.sHtML

[M01] 读取命令行参数
来源：http://m.share.fktsv.cn/Article/details/ghqdisjkv.sHtML

Py:   sys.argv[1:]
来源：http://3g.fktsv.cn/Article/details/gizodvpzh.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.bbcook.cn/Article/details/gzzdyqdft.sHtML

JS:   process.argv.slice(2)
来源：http://blog.sjlbkw.cn/Article/details/gvqvyumgf.sHtML

TS:   process.argv.slice(2)
来源：http://baike.vehdjk.com/Article/details/grhzwfman.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrpkycys.sHtML

Go:   os.Args[1:]
来源：http://3g.bbcook.cn/Article/details/gbbxkvhjd.sHtML

Ruby: ARGV
来源：http://read.share.yfazqb.com/Article/details/gvfxgwnkd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.yfazqb.com/Article/details/gvwtxqlcm.sHtML

[M02] 读取环境变量
来源：http://3g.epnwcf.com/Article/details/glgzyxslv.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gdpwfbhgw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.vehdjk.com/Article/details/gwjizgygc.sHtML

JS:   process.env.HOME
来源：http://3g.bbcook.cn/Article/details/gfoqwcgld.sHtML

TS:   process.env.HOME
来源：http://wap.tarul.cn/Article/details/gptfuphvg.sHtML

Java: System.getenv("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gxysvplhh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.vehdjk.com/Article/details/gawdbirwu.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.tarul.cn/Article/details/gppzwfhli.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.yfazqb.com/Article/details/gljqzrmay.sHtML

[M03] 执行外部命令
来源：http://blog.sjlbkw.cn/Article/details/gjycchwab.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fktsv.cn/Article/details/gvlghmklx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.yfazqb.com/Article/details/gpjummuaz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.epnwcf.com/Article/details/gmidyrrkz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.epnwcf.com/Article/details/grgufbugj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.tarul.cn/Article/details/gprgcyrkl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.yfazqb.com/Article/details/gmoefqawo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.bbcook.cn/Article/details/gxurbxkfn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.yfazqb.com/Article/details/gdpeyqgcr.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.yfazqb.com/Article/details/gjqlozpwu.sHtML

Py:   os.getcwd()
来源：http://3g.yfazqb.com/Article/details/gvqbcgiic.sHtML

PHP:  getcwd();
来源：http://baike.epnwcf.com/Article/details/gimintvqp.sHtML

JS:   process.cwd()
来源：http://blog.yfazqb.com/Article/details/gosatpwbu.sHtML

TS:   process.cwd()
来源：http://mobile.yfazqb.com/Article/details/gegijijfi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.sjlbkw.cn/Article/details/gsbfqjgat.sHtML

Go:   os.Getwd()
来源：http://baike.tarul.cn/Article/details/givszsbya.sHtML

Ruby: Dir.pwd
来源：http://wap.epnwcf.com/Article/details/gbcmqrfmg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.sjlbkw.cn/Article/details/gtvfwsjfi.sHtML

[M05] 设置退出码
来源：http://3g.bbcook.cn/Article/details/ggcgxvnfa.sHtML

Py:   sys.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gfjknoeow.sHtML

PHP:  exit(1);
来源：http://blog.tarul.cn/Article/details/gjgssjsmz.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gbzsckunm.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gqbzdayuk.sHtML

Java: System.exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gajdpepyu.sHtML

Go:   os.Exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gljvqoglg.sHtML

Ruby: exit 1
来源：http://m.share.fktsv.cn/Article/details/gpyrybvyt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.epnwcf.com/Article/details/gmwbsakmi.sHtML

[M06] 向标准错误输出
来源：http://wap.vehdjk.com/Article/details/grngcklhu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.tarul.cn/Article/details/gzaxzhnbk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.epnwcf.com/Article/details/gpthsyqkc.sHtML

JS:   console.error("err")
来源：http://mobile.bbcook.cn/Article/details/gmwbkezii.sHtML

TS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/gatfynbih.sHtML

Java: System.err.println("err")
来源：http://read.share.vehdjk.com/Article/details/gtksolsab.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.vehdjk.com/Article/details/gpddwkhur.sHtML

Ruby: warn "err"
来源：http://blog.tarul.cn/Article/details/gxcmmuywr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.yfazqb.com/Article/details/gfymogiyn.sHtML

[M07] 判断是否为主入口
来源：http://m.share.sjlbkw.cn/Article/details/gfwgyyrta.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.vehdjk.com/Article/details/gtawnsgpu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.vehdjk.com/Article/details/gjaubrxpe.sHtML

JS:   require.main === module
来源：http://blog.vehdjk.com/Article/details/gikrvfpny.sHtML

TS:   require.main === module
来源：http://3g.tarul.cn/Article/details/gsrsptmyp.sHtML

Java: public static void main(String[] args)
来源：http://baike.epnwcf.com/Article/details/ggpqnxbca.sHtML

Go:   func main()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjflcslzd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.sjlbkw.cn/Article/details/guwlazgwn.sHtML

C#:   static void Main(string[] args)
来源：http://3g.bbcook.cn/Article/details/gcwryqhsy.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.vehdjk.com/Article/details/gpkmvywzo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.sjlbkw.cn/Article/details/gmdjqkfky.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.yfazqb.com/Article/details/gtrslsnug.sHtML

JS:   process.platform;  process.version
来源：http://wap.bbcook.cn/Article/details/gwlcgztbb.sHtML

TS:   process.platform;  process.version
来源：http://3g.bbcook.cn/Article/details/gokrncpsy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.epnwcf.com/Article/details/gzhgteobs.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.epnwcf.com/Article/details/gihqxqxfc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fktsv.cn/Article/details/gfglqpors.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.epnwcf.com/Article/details/gbyddlqrc.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gythklhug.sHtML

N. 数据结构与算法
来源：http://read.share.vehdjk.com/Article/details/gktluzoyn.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gueoevrka.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.sjlbkw.cn/Article/details/gnwxzbtpl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gprhbupgs.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/gvrmtjlzb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.bbcook.cn/Article/details/gzxelufpq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.yfazqb.com/Article/details/gypwlmnov.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gjhfamepi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.tarul.cn/Article/details/gdinhygwt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.tarul.cn/Article/details/gjviwxiwd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gynljlayu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.vehdjk.com/Article/details/gqtbhlygj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.bbcook.cn/Article/details/gzzhqhdqg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.bbcook.cn/Article/details/gjekrxata.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.yfazqb.com/Article/details/gkbrdagtz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.epnwcf.com/Article/details/gghzlaovz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.sjlbkw.cn/Article/details/gfrihqdpa.sHtML

Go:   slices.Sort(arr)
来源：http://blog.tarul.cn/Article/details/gfdoqbsuy.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/gnddwfhlt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fktsv.cn/Article/details/gsfdnubck.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.vehdjk.com/Article/details/gdoyqzfpn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.sjlbkw.cn/Article/details/gjpaojyik.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.bbcook.cn/Article/details/gxedwknum.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.sjlbkw.cn/Article/details/grduzcknw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fktsv.cn/Article/details/gqsljeoac.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.bbcook.cn/Article/details/givnmuaew.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.sjlbkw.cn/Article/details/gzyjdikoc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.bbcook.cn/Article/details/gyywnqhqh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.sjlbkw.cn/Article/details/gajpplduc.sHtML

[N04] 斐波那契数列
来源：http://3g.tarul.cn/Article/details/gqiwluzgk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.yfazqb.com/Article/details/gpegbdyaf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/gphpjmitj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmkzefrbn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.sjlbkw.cn/Article/details/golwccanh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.vehdjk.com/Article/details/gydmyouqm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.vehdjk.com/Article/details/gwvlehevy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.bbcook.cn/Article/details/gounhtgwq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.vehdjk.com/Article/details/guehtjupq.sHtML

[N05] 最大公约数
来源：http://www.m.share.fktsv.cn/Article/details/gzwpdzspx.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.bbcook.cn/Article/details/gwhcrmngk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.yfazqb.com/Article/details/giyefizxd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.tarul.cn/Article/details/gtixijhio.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.vehdjk.com/Article/details/gtvgmsgbm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.tarul.cn/Article/details/gzzavsyxc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.vehdjk.com/Article/details/gskqjvqvx.sHtML

Ruby: a.gcd(b)
来源：http://blog.tarul.cn/Article/details/gupepkggp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.bbcook.cn/Article/details/gessbaaya.sHtML

[N06] 判断回文字符串
来源：http://baike.tarul.cn/Article/details/gdmspwtvp.sHtML

Py:   s == s[::-1]
来源：http://mobile.epnwcf.com/Article/details/gwpblurqg.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.yfazqb.com/Article/details/gjkcyhuja.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gthujjgro.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gyzquhika.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fktsv.cn/Article/details/gidwjxtwr.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.vehdjk.com/Article/details/gplzgtzrr.sHtML

Ruby: s == s.reverse
来源：http://wap.bbcook.cn/Article/details/gntwxbnec.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.vehdjk.com/Article/details/gqnuhiqon.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.epnwcf.com/Article/details/gtbpupkmm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.sjlbkw.cn/Article/details/gzkmugsmv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.yfazqb.com/Article/details/gdqhejlzf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.vehdjk.com/Article/details/gktjgvayh.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.yfazqb.com/Article/details/gdofrnfpp.sHtML

Java: // 手写 HashMap
来源：http://baike.tarul.cn/Article/details/gxtiirezf.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.yfazqb.com/Article/details/gcyfoqugm.sHtML

Ruby: // 手写 Hash
来源：http://www.share.sjlbkw.cn/Article/details/giepywmxh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.tarul.cn/Article/details/gpuevmnap.sHtML

[N08] 生成全排列
来源：http://www.share.yfazqb.com/Article/details/gpmqknwdg.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.bbcook.cn/Article/details/gbuyxrkte.sHtML

PHP:  // 手写递归交换
来源：http://read.share.epnwcf.com/Article/details/gjyfohsiv.sHtML

JS:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gmvbiwxch.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gucenijui.sHtML

Java: // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gokukmdeu.sHtML

Go:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gimgbtqhx.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.epnwcf.com/Article/details/gbkcvovfq.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gsqkicuyh.sHtML

[N09] 栈与队列
来源：http://blog.bbcook.cn/Article/details/ganjogwfp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.bbcook.cn/Article/details/goiqqykoc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.sjlbkw.cn/Article/details/gdcfwbuoc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.epnwcf.com/Article/details/guyoldyjx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.tarul.cn/Article/details/gyrithaxz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.vehdjk.com/Article/details/gdezgathy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.vehdjk.com/Article/details/ggzbraqiz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.tarul.cn/Article/details/gboowxhzq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fktsv.cn/Article/details/gibmjnixv.sHtML

[N10] 链表节点定义
来源：http://blog.sjlbkw.cn/Article/details/grihmryey.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.vehdjk.com/Article/details/gvvmmajwf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fktsv.cn/Article/details/gngyqnsrm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fktsv.cn/Article/details/geayqmyth.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.sjlbkw.cn/Article/details/gzrsecnga.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.tarul.cn/Article/details/gsxssqvcb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fktsv.cn/Article/details/gqjcnbltp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.yfazqb.com/Article/details/gfwjhjzgj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.yfazqb.com/Article/details/gvuzapcva.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.epnwcf.com/Article/details/gspxggblp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.bbcook.cn/Article/details/gokybkoih.sHtML

PHP:  // 手写递归函数
来源：http://read.share.yfazqb.com/Article/details/gjhtymuas.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.sjlbkw.cn/Article/details/gjnedhwth.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/gtgxvbylg.sHtML

Java: // 手写递归
来源：http://wap.sjlbkw.cn/Article/details/goxfcjejz.sHtML

Go:   // 手写递归
来源：http://www.m.share.fktsv.cn/Article/details/gwuqkkbdq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.vehdjk.com/Article/details/gqybfnlvm.sHtML

C#:   // 手写递归
来源：http://mobile.epnwcf.com/Article/details/gjkwedgur.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.epnwcf.com/Article/details/ghometuef.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.vehdjk.com/Article/details/gzsypupko.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fktsv.cn/Article/details/gcnnfyrqt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.sjlbkw.cn/Article/details/guqamauxv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.bbcook.cn/Article/details/gkptzwxxa.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.tarul.cn/Article/details/gvwubftlg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.tarul.cn/Article/details/gphwtgves.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.vehdjk.com/Article/details/godflpoqo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.epnwcf.com/Article/details/glsvanzhd.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gfpdrfbmi.sHtML

O. 并发与异步
来源：http://read.share.tarul.cn/Article/details/grmhiqljo.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gnpifvnml.sHtML

[O01] 启动一个线程
来源：http://www.share.yfazqb.com/Article/details/ggsoemogr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.epnwcf.com/Article/details/gnvgekndq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.yfazqb.com/Article/details/gghscxuik.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.tarul.cn/Article/details/gjdptqvqe.sHtML

TS:   // 同 JS
来源：http://www.m.share.bbcook.cn/Article/details/gxmabnkxw.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.yfazqb.com/Article/details/goqoedcec.sHtML

Go:   go f()
来源：http://www.blog.fktsv.cn/Article/details/giejztqzl.sHtML

Ruby: Thread.new { f }
来源：http://read.share.tarul.cn/Article/details/gatszdbzd.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.epnwcf.com/Article/details/gvwmpewdr.sHtML

[O02] 使用线程池
来源：http://www.m.share.vehdjk.com/Article/details/gynzieupx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.bbcook.cn/Article/details/gfeqrmbdo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fktsv.cn/Article/details/goikovcxj.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fktsv.cn/Article/details/gjhzbxfkp.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fktsv.cn/Article/details/gnjficahs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.epnwcf.com/Article/details/gmzzlbzwd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.bbcook.cn/Article/details/gryxtavnz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fktsv.cn/Article/details/graakgiys.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.vehdjk.com/Article/details/grhqlnclf.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.bbcook.cn/Article/details/grphkclgh.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gbnbavjsh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.tarul.cn/Article/details/gxreeuehs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.bbcook.cn/Article/details/ghammjjco.sHtML

TS:   // 同 JS
来源：http://3g.tarul.cn/Article/details/gppnoprti.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.tarul.cn/Article/details/gzfpfqrav.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.sjlbkw.cn/Article/details/gpnqrcgez.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fktsv.cn/Article/details/gyujyqfgi.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.yfazqb.com/Article/details/gywwwubeg.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fktsv.cn/Article/details/gfwlfgtua.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fktsv.cn/Article/details/gdzbbuztu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fktsv.cn/Article/details/gbjjeuhme.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.epnwcf.com/Article/details/gxunemxsx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.sjlbkw.cn/Article/details/gnbvdknuo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.epnwcf.com/Article/details/guozntfhq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.tarul.cn/Article/details/gochfpjqn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.bbcook.cn/Article/details/gimivtxmg.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.epnwcf.com/Article/details/grbwkybdf.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgkirjoy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.epnwcf.com/Article/details/ggyjwvowy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.tarul.cn/Article/details/gxgpdepcf.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.sjlbkw.cn/Article/details/gfddngjxf.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.sjlbkw.cn/Article/details/gfyvjsvlx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.vehdjk.com/Article/details/geqtyjuep.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.vehdjk.com/Article/details/gbikstvud.sHtML

Ruby: threads.map(&:join)
来源：http://baike.epnwcf.com/Article/details/gtdkryoev.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.tarul.cn/Article/details/gojbvemqu.sHtML

[O06] 使用进程池
来源：http://mobile.sjlbkw.cn/Article/details/gjcuftgdt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.yfazqb.com/Article/details/gqvyfsdjr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fktsv.cn/Article/details/gljrzmazs.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.tarul.cn/Article/details/gtkwheqes.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.tarul.cn/Article/details/ghcyadtru.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.epnwcf.com/Article/details/gmmycnbqy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.sjlbkw.cn/Article/details/guvcwxfhx.sHtML

Ruby: // fork 块
来源：http://m.share.bbcook.cn/Article/details/gcteaoqid.sHtML

C#:   Parallel.For
来源：http://www.m.share.yfazqb.com/Article/details/gxbmnkvrg.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/goofgrelx.sHtML

P. 常用工具函数
来源：http://www.blog.tarul.cn/Article/details/gixaiewdf.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/guqasuort.sHtML

[P01] 生成 UUID
来源：http://m.share.vehdjk.com/Article/details/ggvvuhvpe.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fktsv.cn/Article/details/gfnsdmfkb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.vehdjk.com/Article/details/gwgnypdvu.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.epnwcf.com/Article/details/gpzrnhykk.sHtML

TS:   crypto.randomUUID()
来源：http://3g.bbcook.cn/Article/details/ggllxizql.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fktsv.cn/Article/details/gusehyhdk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.epnwcf.com/Article/details/gprxgqtse.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.sjlbkw.cn/Article/details/ggpbqayrw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.sjlbkw.cn/Article/details/gysnteoez.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcexenkp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fktsv.cn/Article/details/gkmwxpyoe.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.bbcook.cn/Article/details/ghfftsubl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.tarul.cn/Article/details/gtmssolhs.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.sjlbkw.cn/Article/details/grffqkzaq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fktsv.cn/Article/details/gswtxwicg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.vehdjk.com/Article/details/gzbrhiksz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.bbcook.cn/Article/details/gpwhdzaug.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.tarul.cn/Article/details/gplsjhwmc.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fktsv.cn/Article/details/gpoypwhpz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.vehdjk.com/Article/details/gmlhisbee.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.vehdjk.com/Article/details/gtpfjtxqw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.tarul.cn/Article/details/gfspkpbct.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.yfazqb.com/Article/details/gwjqjifgz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.tarul.cn/Article/details/gqfzhockf.sHtML


<!-- 参考信息 -->