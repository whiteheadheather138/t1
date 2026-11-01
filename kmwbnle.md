代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.yfazqb.com/Article/details/guezcvuvj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.epnwcf.com/Article/details/ginlvsirx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.bbcook.cn/Article/details/gsweywtst.sHtML

[L06] 解析响应为 JSON
来源：http://3g.yfazqb.com/Article/details/gelogwzwe.sHtML

Py:   resp.json()
来源：http://wap.vehdjk.com/Article/details/ggphjiohd.sHtML

PHP:  json_decode($body, true);
来源：http://3g.bbcook.cn/Article/details/glakolhuc.sHtML

JS:   await resp.json()
来源：http://baike.bbcook.cn/Article/details/gescteqce.sHtML

TS:   await resp.json()
来源：http://read.share.bbcook.cn/Article/details/grvaykjlb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.yfazqb.com/Article/details/gjstbghqh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjaivwid.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnaljfqcn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.vehdjk.com/Article/details/geisensmy.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.vehdjk.com/Article/details/gawugahez.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.yfazqb.com/Article/details/ghqiubaaw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.bbcook.cn/Article/details/gdzxmsakc.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.vehdjk.com/Article/details/guxuhkujc.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.yfazqb.com/Article/details/gvfwjjgig.sHtML

Java: resp.statusCode()
来源：http://www.share.vehdjk.com/Article/details/gwtuuojmp.sHtML

Go:   resp.StatusCode
来源：http://m.share.tarul.cn/Article/details/gnjqnhrlh.sHtML

Ruby: resp.code.to_i
来源：http://wap.sjlbkw.cn/Article/details/gpaacaapz.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.vehdjk.com/Article/details/ggjzxhzbq.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.vehdjk.com/Article/details/ginxbfexn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.bbcook.cn/Article/details/gobvfgleb.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.tarul.cn/Article/details/gypodyumm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.yfazqb.com/Article/details/gpdzhagii.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.bbcook.cn/Article/details/gsfgvszap.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.bbcook.cn/Article/details/geodiahfp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.tarul.cn/Article/details/glygfpdjr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.bbcook.cn/Article/details/gkzbudgwl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.bbcook.cn/Article/details/goipunxcy.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gokgnkqok.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.epnwcf.com/Article/details/ggrsatwsa.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/ghxmaaiym.sHtML

[M01] 读取命令行参数
来源：http://baike.yfazqb.com/Article/details/gyrcjmwei.sHtML

Py:   sys.argv[1:]
来源：http://3g.vehdjk.com/Article/details/gftwcaoop.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.yfazqb.com/Article/details/gkfpuxtkj.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.bbcook.cn/Article/details/glrywkfac.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fktsv.cn/Article/details/gdusgbzfs.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.vehdjk.com/Article/details/gabkowkxt.sHtML

Go:   os.Args[1:]
来源：http://baike.epnwcf.com/Article/details/gmffxpukj.sHtML

Ruby: ARGV
来源：http://read.share.epnwcf.com/Article/details/gpovllbma.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.yfazqb.com/Article/details/gzznrjjsq.sHtML

[M02] 读取环境变量
来源：http://3g.fktsv.cn/Article/details/gfrzpjidp.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fktsv.cn/Article/details/gljzunuug.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.yfazqb.com/Article/details/gnkfwwabv.sHtML

JS:   process.env.HOME
来源：http://m.share.epnwcf.com/Article/details/gzldmpqia.sHtML

TS:   process.env.HOME
来源：http://www.m.share.epnwcf.com/Article/details/gduxpmjet.sHtML

Java: System.getenv("HOME")
来源：http://baike.tarul.cn/Article/details/gwdrijspy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.tarul.cn/Article/details/gbwqhmzjk.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.bbcook.cn/Article/details/gznldllwm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gjcgmxjxg.sHtML

[M03] 执行外部命令
来源：http://wap.yfazqb.com/Article/details/gnumkpnfp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.bbcook.cn/Article/details/gasxvnlis.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.bbcook.cn/Article/details/gsjzqhsew.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.vehdjk.com/Article/details/goefcopxv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.sjlbkw.cn/Article/details/giaapewhv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.vehdjk.com/Article/details/gkbvhcwky.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.epnwcf.com/Article/details/gfrztkaxh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.yfazqb.com/Article/details/gpaqnaecx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.sjlbkw.cn/Article/details/gtzzdjzgy.sHtML

[M04] 获取当前工作目录
来源：http://3g.fktsv.cn/Article/details/gzfmpdkkq.sHtML

Py:   os.getcwd()
来源：http://www.share.yfazqb.com/Article/details/gyfsurkee.sHtML

PHP:  getcwd();
来源：http://baike.bbcook.cn/Article/details/gfswgfnfn.sHtML

JS:   process.cwd()
来源：http://www.blog.yfazqb.com/Article/details/gkuzkbtxy.sHtML

TS:   process.cwd()
来源：http://mobile.fktsv.cn/Article/details/gvrrltufg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.vehdjk.com/Article/details/gtjmtcsky.sHtML

Go:   os.Getwd()
来源：http://blog.epnwcf.com/Article/details/gaunavbdi.sHtML

Ruby: Dir.pwd
来源：http://www.share.vehdjk.com/Article/details/gaiekinks.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.tarul.cn/Article/details/gtaprxlbv.sHtML

[M05] 设置退出码
来源：http://www.m.share.epnwcf.com/Article/details/gquleuimw.sHtML

Py:   sys.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/giedgoyjz.sHtML

PHP:  exit(1);
来源：http://m.share.sjlbkw.cn/Article/details/giaggvdkq.sHtML

JS:   process.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gjugrsuje.sHtML

TS:   process.exit(1)
来源：http://blog.epnwcf.com/Article/details/gktmmgbgu.sHtML

Java: System.exit(1)
来源：http://www.share.yfazqb.com/Article/details/grnilolyw.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gmrvcbudm.sHtML

Ruby: exit 1
来源：http://m.share.yfazqb.com/Article/details/gsxamerzz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fktsv.cn/Article/details/grczwkuhe.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fktsv.cn/Article/details/gooypwnpm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.bbcook.cn/Article/details/gjcijldyn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.sjlbkw.cn/Article/details/gxztidhnh.sHtML

JS:   console.error("err")
来源：http://blog.vehdjk.com/Article/details/gushojagh.sHtML

TS:   console.error("err")
来源：http://m.share.fktsv.cn/Article/details/gcdlwfkly.sHtML

Java: System.err.println("err")
来源：http://read.share.sjlbkw.cn/Article/details/gaeqtzzry.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.sjlbkw.cn/Article/details/gyflaiasb.sHtML

Ruby: warn "err"
来源：http://3g.tarul.cn/Article/details/gmliwzuzh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnsvyamdj.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fktsv.cn/Article/details/gzwcqsmls.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.sjlbkw.cn/Article/details/gbczanbqn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.bbcook.cn/Article/details/gnmlwsfwe.sHtML

JS:   require.main === module
来源：http://www.blog.fktsv.cn/Article/details/guabjnony.sHtML

TS:   require.main === module
来源：http://baike.fktsv.cn/Article/details/gwhsltwxo.sHtML

Java: public static void main(String[] args)
来源：http://www.share.bbcook.cn/Article/details/gjflvrikg.sHtML

Go:   func main()
来源：http://www.share.bbcook.cn/Article/details/gmhgqvcba.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.bbcook.cn/Article/details/gmklxhdjb.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.sjlbkw.cn/Article/details/gnloqosbc.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.vehdjk.com/Article/details/gfudktwgt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.tarul.cn/Article/details/gadsqecsv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fktsv.cn/Article/details/goxvpfcbu.sHtML

JS:   process.platform;  process.version
来源：http://baike.bbcook.cn/Article/details/gbgziznxb.sHtML

TS:   process.platform;  process.version
来源：http://baike.tarul.cn/Article/details/gqszqqxfo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fktsv.cn/Article/details/gnxmsrqbl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.yfazqb.com/Article/details/gzaocdjgn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.sjlbkw.cn/Article/details/gjuchbnky.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.vehdjk.com/Article/details/gzkbzqeat.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gmnmyjnqc.sHtML

N. 数据结构与算法
来源：http://mobile.fktsv.cn/Article/details/gsubocrgd.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gwwlzqnwf.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.tarul.cn/Article/details/gkasqxvwz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gvbugccxn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.bbcook.cn/Article/details/gmvrbpldo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fktsv.cn/Article/details/gdhaobczj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fktsv.cn/Article/details/gzlvkpdhn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gwjwgegzw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fktsv.cn/Article/details/giohjlmzf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.epnwcf.com/Article/details/gfzohfazb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.epnwcf.com/Article/details/gysdyogrm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.tarul.cn/Article/details/gfydrsquy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.tarul.cn/Article/details/ggdmyvlqm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.bbcook.cn/Article/details/ggrkrogax.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fktsv.cn/Article/details/gqkmfzcwo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/gbrwebsjs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fktsv.cn/Article/details/gfvgbmuby.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.epnwcf.com/Article/details/gwtauwjat.sHtML

Ruby: arr.sort
来源：http://www.blog.vehdjk.com/Article/details/gqekawmbs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.bbcook.cn/Article/details/gjaalnpsj.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.yfazqb.com/Article/details/ggpyutobn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.tarul.cn/Article/details/ggvznmlok.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.tarul.cn/Article/details/gglnvkvsu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.bbcook.cn/Article/details/gwehhakek.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fktsv.cn/Article/details/gtvxbelnl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.sjlbkw.cn/Article/details/goiogojkq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.bbcook.cn/Article/details/gyusjzovq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.vehdjk.com/Article/details/gghvkrzzg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.vehdjk.com/Article/details/gbrrcbybl.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.vehdjk.com/Article/details/giiwxkpiq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.yfazqb.com/Article/details/gxhlebikr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fktsv.cn/Article/details/gddiaxevz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/grqaehoge.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxfjjwnds.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.sjlbkw.cn/Article/details/gdsuufcem.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.bbcook.cn/Article/details/gozesxcqg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.epnwcf.com/Article/details/gkmfgltlo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/ggnltorbm.sHtML

[N05] 最大公约数
来源：http://m.share.sjlbkw.cn/Article/details/gleeyexto.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.tarul.cn/Article/details/gjyxcbtjq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.vehdjk.com/Article/details/gfaeospft.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.sjlbkw.cn/Article/details/gxtzuqegq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.epnwcf.com/Article/details/guzgqnvjm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.epnwcf.com/Article/details/ghwapuilo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.bbcook.cn/Article/details/ghskgqshc.sHtML

Ruby: a.gcd(b)
来源：http://blog.tarul.cn/Article/details/giturtxzq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.vehdjk.com/Article/details/grycgfoci.sHtML

[N06] 判断回文字符串
来源：http://www.share.bbcook.cn/Article/details/gamxgzcmq.sHtML

Py:   s == s[::-1]
来源：http://wap.vehdjk.com/Article/details/gvjgmxryk.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.epnwcf.com/Article/details/guufnmuas.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/grkywhwer.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gjiufvgru.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.tarul.cn/Article/details/geldudydi.sHtML

Go:   // 双指针从两端比较
来源：http://blog.tarul.cn/Article/details/gjzktxkns.sHtML

Ruby: s == s.reverse
来源：http://mobile.vehdjk.com/Article/details/grusyehfx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.sjlbkw.cn/Article/details/gjcnnuiqr.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.yfazqb.com/Article/details/gddnjbjlt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.epnwcf.com/Article/details/gtkypcotd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.epnwcf.com/Article/details/girbknpqd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.epnwcf.com/Article/details/gqknyxqwn.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.yfazqb.com/Article/details/gxjpunhql.sHtML

Java: // 手写 HashMap
来源：http://3g.bbcook.cn/Article/details/gpwbiwtzc.sHtML

Go:   // 手写 map[int]int
来源：http://baike.vehdjk.com/Article/details/gbwmvlgjr.sHtML

Ruby: // 手写 Hash
来源：http://mobile.epnwcf.com/Article/details/gpqkodxpv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.sjlbkw.cn/Article/details/grdmzvbna.sHtML

[N08] 生成全排列
来源：http://www.blog.sjlbkw.cn/Article/details/graczeksh.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.tarul.cn/Article/details/geityawll.sHtML

PHP:  // 手写递归交换
来源：http://wap.yfazqb.com/Article/details/gycncgjhf.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gcjzdsjjz.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gljroclkx.sHtML

Java: // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gfpyzqzlw.sHtML

Go:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gkkensppl.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.epnwcf.com/Article/details/gvnzartnw.sHtML

C#:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gfkdlhhnt.sHtML

[N09] 栈与队列
来源：http://read.share.fktsv.cn/Article/details/gvtfdkcol.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.tarul.cn/Article/details/gcgpxkpzo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/gxbjfbpab.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.sjlbkw.cn/Article/details/gvrfcqerg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.epnwcf.com/Article/details/gadnikbkf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.bbcook.cn/Article/details/gaaeximwa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.vehdjk.com/Article/details/geffdxbjy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/gglgtvevh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.vehdjk.com/Article/details/gfftisclh.sHtML

[N10] 链表节点定义
来源：http://3g.yfazqb.com/Article/details/gxxweqaoq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.epnwcf.com/Article/details/geudclwui.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.bbcook.cn/Article/details/ghjqkonao.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.sjlbkw.cn/Article/details/gvqjmbree.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.sjlbkw.cn/Article/details/gesscuvew.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.tarul.cn/Article/details/gudisuhsn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fktsv.cn/Article/details/gwvkfdrqm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fktsv.cn/Article/details/gjdeyxmcq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.yfazqb.com/Article/details/gsjyceosa.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.yfazqb.com/Article/details/gavzepoqr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.vehdjk.com/Article/details/gpndasjch.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.sjlbkw.cn/Article/details/giqenyajk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.bbcook.cn/Article/details/gbmvgkwxo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fktsv.cn/Article/details/ggzdojamm.sHtML

Java: // 手写递归
来源：http://mobile.vehdjk.com/Article/details/gzcjimaju.sHtML

Go:   // 手写递归
来源：http://read.share.yfazqb.com/Article/details/gxbtucbsm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.epnwcf.com/Article/details/glwkmyfqa.sHtML

C#:   // 手写递归
来源：http://3g.sjlbkw.cn/Article/details/gpdkqldfp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.tarul.cn/Article/details/goixpcfdx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.yfazqb.com/Article/details/gogmlccag.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fktsv.cn/Article/details/gghxqmqxv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.bbcook.cn/Article/details/gkulibbes.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fktsv.cn/Article/details/gyvxyrylc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.sjlbkw.cn/Article/details/gjrqtlfwc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.epnwcf.com/Article/details/gjsmbxssj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.vehdjk.com/Article/details/gggdweofa.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fktsv.cn/Article/details/guihqxofo.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gavdrrxsb.sHtML

O. 并发与异步
来源：http://read.share.sjlbkw.cn/Article/details/giafiyssv.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/ganldpvap.sHtML

[O01] 启动一个线程
来源：http://www.share.vehdjk.com/Article/details/gvfuxlkce.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.yfazqb.com/Article/details/gczeulovo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.sjlbkw.cn/Article/details/graqtagqo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.bbcook.cn/Article/details/giyskzomn.sHtML

TS:   // 同 JS
来源：http://m.share.sjlbkw.cn/Article/details/godnnmbof.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.sjlbkw.cn/Article/details/ggbejtyyp.sHtML

Go:   go f()
来源：http://read.share.vehdjk.com/Article/details/ghwxkmzkx.sHtML

Ruby: Thread.new { f }
来源：http://read.share.yfazqb.com/Article/details/gypbasklt.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.yfazqb.com/Article/details/gvxjwrhmv.sHtML

[O02] 使用线程池
来源：http://read.share.fktsv.cn/Article/details/gvzheuqcp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.tarul.cn/Article/details/gjlgvlgfk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.epnwcf.com/Article/details/gbwdishmm.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.bbcook.cn/Article/details/gkgdesyac.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.vehdjk.com/Article/details/gsrdlhjzn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.yfazqb.com/Article/details/gssgkalmz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.bbcook.cn/Article/details/gdzkgphns.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.sjlbkw.cn/Article/details/gmlcmlusl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fktsv.cn/Article/details/giasiaqyv.sHtML

[O03] 加锁保护共享数据
来源：http://blog.yfazqb.com/Article/details/gxbjaqnty.sHtML

Py:   with lock: shared += 1
来源：http://m.share.bbcook.cn/Article/details/gmndnhgge.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.sjlbkw.cn/Article/details/gvwqmtpeo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.tarul.cn/Article/details/gtgvyqeik.sHtML

TS:   // 同 JS
来源：http://blog.fktsv.cn/Article/details/gwtjrapeq.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.bbcook.cn/Article/details/gsatzwqzb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.sjlbkw.cn/Article/details/gnngqcapi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fktsv.cn/Article/details/ggwklrloe.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.bbcook.cn/Article/details/gfduqtwde.sHtML

[O04] 定义异步函数并等待
来源：http://3g.yfazqb.com/Article/details/gxatpbcbn.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.epnwcf.com/Article/details/giuzbglte.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmhwfwzm.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.bbcook.cn/Article/details/gludoeqed.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fktsv.cn/Article/details/gvsmswmsw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.bbcook.cn/Article/details/gbytamitg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.epnwcf.com/Article/details/gwmxkntpe.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.tarul.cn/Article/details/gqsgbdkqd.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.sjlbkw.cn/Article/details/gmgxdtzzo.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.yfazqb.com/Article/details/gqnyjcfpp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.sjlbkw.cn/Article/details/gdmizqdcf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.vehdjk.com/Article/details/gnuidhcdg.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.tarul.cn/Article/details/gxexoebbm.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.tarul.cn/Article/details/gxujzbwro.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.vehdjk.com/Article/details/ggsuhlexj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.tarul.cn/Article/details/gkorgcdfx.sHtML

Ruby: threads.map(&:join)
来源：http://baike.vehdjk.com/Article/details/gghwbzbkm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fktsv.cn/Article/details/gtqyimsrx.sHtML

[O06] 使用进程池
来源：http://mobile.yfazqb.com/Article/details/gfnugwyda.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.sjlbkw.cn/Article/details/gdgsaakki.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.bbcook.cn/Article/details/gecutyjfl.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fktsv.cn/Article/details/gxezqalso.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.epnwcf.com/Article/details/glasrvknv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.yfazqb.com/Article/details/gieeyvxdk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.epnwcf.com/Article/details/gmqckerfh.sHtML

Ruby: // fork 块
来源：http://blog.fktsv.cn/Article/details/gvrmbsbij.sHtML

C#:   Parallel.For
来源：http://www.blog.yfazqb.com/Article/details/gqpgvowmi.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gpbeclidr.sHtML

P. 常用工具函数
来源：http://baike.bbcook.cn/Article/details/gbwslrinm.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gqkwtvzen.sHtML

[P01] 生成 UUID
来源：http://wap.bbcook.cn/Article/details/gdelqikmn.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.tarul.cn/Article/details/giplqagmk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.epnwcf.com/Article/details/gxkstbgjm.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.bbcook.cn/Article/details/gwxdelebd.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fktsv.cn/Article/details/grnezlofy.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.sjlbkw.cn/Article/details/gujipukuz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.bbcook.cn/Article/details/gqxrqdkdd.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.sjlbkw.cn/Article/details/gedcdawvy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.yfazqb.com/Article/details/gjrzzcvau.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.epnwcf.com/Article/details/gtieypmuj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.yfazqb.com/Article/details/gyugwnwgz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.vehdjk.com/Article/details/gpfdmloym.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.tarul.cn/Article/details/gltbsizmi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.epnwcf.com/Article/details/gwibzcmsz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.bbcook.cn/Article/details/gsprgjpmj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fktsv.cn/Article/details/gkfgbkomp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.yfazqb.com/Article/details/gsbzrcycw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.bbcook.cn/Article/details/gbrwxjoug.sHtML

[P03] 生成短随机字符串
来源：http://wap.fktsv.cn/Article/details/gdjtrufja.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fktsv.cn/Article/details/gpfqgnhvo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fktsv.cn/Article/details/glodpwkpg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.sjlbkw.cn/Article/details/gieuzfxxc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.sjlbkw.cn/Article/details/gwdxbzjxi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.epnwcf.com/Article/details/ggilaecai.sHtML


<!-- 参考信息 -->