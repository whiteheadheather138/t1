代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.bbcook.cn/Article/details/glrduxvrl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.vehdjk.com/Article/details/ghrpyynrf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gfroupmql.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.epnwcf.com/Article/details/geclshszw.sHtML

Py:   resp.json()
来源：http://mobile.fktsv.cn/Article/details/gqmhyygtn.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.sjlbkw.cn/Article/details/gyzitsqvx.sHtML

JS:   await resp.json()
来源：http://www.blog.yfazqb.com/Article/details/ghersbkyg.sHtML

TS:   await resp.json()
来源：http://wap.tarul.cn/Article/details/gcafydttg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.sjlbkw.cn/Article/details/gxqtjwnvr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.bbcook.cn/Article/details/gskodnfpd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.epnwcf.com/Article/details/gmwrzrcia.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.yfazqb.com/Article/details/glhzpkjvs.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.epnwcf.com/Article/details/gfentnpib.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.yfazqb.com/Article/details/giclacatw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.yfazqb.com/Article/details/gbhgtoqka.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fktsv.cn/Article/details/gsqpyitop.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.epnwcf.com/Article/details/gmwrutpcv.sHtML

Java: resp.statusCode()
来源：http://www.m.share.tarul.cn/Article/details/giffefhwn.sHtML

Go:   resp.StatusCode
来源：http://m.share.bbcook.cn/Article/details/ggpadixwy.sHtML

Ruby: resp.code.to_i
来源：http://wap.fktsv.cn/Article/details/gnsvlhxsc.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.vehdjk.com/Article/details/gmavzfbsd.sHtML

[L08] 并发请求多个地址
来源：http://www.share.tarul.cn/Article/details/gsnrqaasg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.vehdjk.com/Article/details/gvwlutyln.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.sjlbkw.cn/Article/details/gbhjuowef.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.tarul.cn/Article/details/gnlordqas.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.vehdjk.com/Article/details/gufrelkrv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.yfazqb.com/Article/details/ggyisylwp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.yfazqb.com/Article/details/gmdhtmxnu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.bbcook.cn/Article/details/ggglthwar.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fktsv.cn/Article/details/gujzyhcwn.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gumoltdhi.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.epnwcf.com/Article/details/gerzowcgr.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gqmocemuy.sHtML

[M01] 读取命令行参数
来源：http://blog.sjlbkw.cn/Article/details/ghkxrwkwz.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fktsv.cn/Article/details/gmhdzbocj.sHtML

PHP:  $argv;  $argc;
来源：http://baike.tarul.cn/Article/details/guhnhlfex.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fktsv.cn/Article/details/gelzlwfyk.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fktsv.cn/Article/details/gttaldkou.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.yfazqb.com/Article/details/gwwbqrinb.sHtML

Go:   os.Args[1:]
来源：http://m.share.tarul.cn/Article/details/gshjviiza.sHtML

Ruby: ARGV
来源：http://read.share.tarul.cn/Article/details/gcvvkmqev.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.tarul.cn/Article/details/gttxnoofb.sHtML

[M02] 读取环境变量
来源：http://read.share.epnwcf.com/Article/details/gtxfweaxk.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghyuzewgw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fktsv.cn/Article/details/gqecthryy.sHtML

JS:   process.env.HOME
来源：http://wap.epnwcf.com/Article/details/gklnhcaml.sHtML

TS:   process.env.HOME
来源：http://blog.vehdjk.com/Article/details/gcwppjkmy.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.bbcook.cn/Article/details/gksfgtdhz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.bbcook.cn/Article/details/gyhgkcvpp.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.tarul.cn/Article/details/gojrzfwvx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.tarul.cn/Article/details/guwlwljsn.sHtML

[M03] 执行外部命令
来源：http://mobile.bbcook.cn/Article/details/gjivoanlz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.bbcook.cn/Article/details/guzqtrlnb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.sjlbkw.cn/Article/details/gqzhedisv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.epnwcf.com/Article/details/gypuwtiam.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.tarul.cn/Article/details/ggzddzman.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.epnwcf.com/Article/details/gylcfisrs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.yfazqb.com/Article/details/grobgukin.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.yfazqb.com/Article/details/gpyspxxpf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fktsv.cn/Article/details/gzwavkocj.sHtML

[M04] 获取当前工作目录
来源：http://m.share.tarul.cn/Article/details/gfayncdkv.sHtML

Py:   os.getcwd()
来源：http://blog.bbcook.cn/Article/details/gpwhdeweb.sHtML

PHP:  getcwd();
来源：http://baike.tarul.cn/Article/details/gvjiunekh.sHtML

JS:   process.cwd()
来源：http://3g.yfazqb.com/Article/details/gibmpyhzz.sHtML

TS:   process.cwd()
来源：http://www.m.share.bbcook.cn/Article/details/gbfeyfpzq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.bbcook.cn/Article/details/gesxorckw.sHtML

Go:   os.Getwd()
来源：http://www.m.share.yfazqb.com/Article/details/ghefhzbuy.sHtML

Ruby: Dir.pwd
来源：http://m.share.epnwcf.com/Article/details/gplwkitor.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.yfazqb.com/Article/details/gautrwwrg.sHtML

[M05] 设置退出码
来源：http://www.share.vehdjk.com/Article/details/ghmctdaga.sHtML

Py:   sys.exit(1)
来源：http://wap.fktsv.cn/Article/details/godfwynge.sHtML

PHP:  exit(1);
来源：http://mobile.fktsv.cn/Article/details/gbqcdsooh.sHtML

JS:   process.exit(1)
来源：http://mobile.epnwcf.com/Article/details/gcplvysoi.sHtML

TS:   process.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gqbgeivpz.sHtML

Java: System.exit(1)
来源：http://www.share.tarul.cn/Article/details/gqbaphvrm.sHtML

Go:   os.Exit(1)
来源：http://m.share.fktsv.cn/Article/details/glkdzeoif.sHtML

Ruby: exit 1
来源：http://baike.sjlbkw.cn/Article/details/ghvnhgxvj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.vehdjk.com/Article/details/gkwaulbkz.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxskbaew.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.bbcook.cn/Article/details/gjyjdseof.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fktsv.cn/Article/details/gsexyboqq.sHtML

JS:   console.error("err")
来源：http://3g.bbcook.cn/Article/details/geaoxrtzm.sHtML

TS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/gsgxjmkrt.sHtML

Java: System.err.println("err")
来源：http://read.share.bbcook.cn/Article/details/gtdrjqzek.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.epnwcf.com/Article/details/gicnivflj.sHtML

Ruby: warn "err"
来源：http://blog.tarul.cn/Article/details/gcbjwajwq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.bbcook.cn/Article/details/ghketyydb.sHtML

[M07] 判断是否为主入口
来源：http://mobile.vehdjk.com/Article/details/gpmwlkjdd.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.tarul.cn/Article/details/gqygjeshf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.epnwcf.com/Article/details/glfficspl.sHtML

JS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/ghkkqvekc.sHtML

TS:   require.main === module
来源：http://read.share.epnwcf.com/Article/details/gebxaxiqt.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.sjlbkw.cn/Article/details/gwgoyfsyf.sHtML

Go:   func main()
来源：http://read.share.fktsv.cn/Article/details/gukojydqo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fktsv.cn/Article/details/gfrtfppzu.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.vehdjk.com/Article/details/glkmrcjce.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fktsv.cn/Article/details/gqarewmpx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.yfazqb.com/Article/details/gugvfxmac.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.sjlbkw.cn/Article/details/gjrnodtli.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/gbezzzzqj.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.sjlbkw.cn/Article/details/gfslmgiob.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.epnwcf.com/Article/details/gbstzhnfv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.vehdjk.com/Article/details/guazhwhth.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fktsv.cn/Article/details/gtgdujfit.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.tarul.cn/Article/details/gtuqkbzvu.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/glmmxovoq.sHtML

N. 数据结构与算法
来源：http://baike.yfazqb.com/Article/details/grwpucebi.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/grxxfeymy.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.bbcook.cn/Article/details/gifpowasn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gjgdfcubn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.epnwcf.com/Article/details/gjinbpkcc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gecqfmgqd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.tarul.cn/Article/details/gvdlismqg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gwrdqgrff.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.tarul.cn/Article/details/gwmriknkb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fktsv.cn/Article/details/gjttusnyx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gvblhedri.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.epnwcf.com/Article/details/gaefbnrvn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.tarul.cn/Article/details/ghsljtmtv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.yfazqb.com/Article/details/gtyltrvcr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.vehdjk.com/Article/details/gcntwlhqf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.yfazqb.com/Article/details/gpgbcblmh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fktsv.cn/Article/details/guegwbmoq.sHtML

Go:   slices.Sort(arr)
来源：http://wap.tarul.cn/Article/details/ggoiegcsl.sHtML

Ruby: arr.sort
来源：http://mobile.sjlbkw.cn/Article/details/gerqcyzum.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fktsv.cn/Article/details/gdwfeccwm.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.tarul.cn/Article/details/gsqimqeys.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.epnwcf.com/Article/details/guwrehuju.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.bbcook.cn/Article/details/gbvwkmfkg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.bbcook.cn/Article/details/gbojgizpe.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.epnwcf.com/Article/details/gqkzwshom.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.yfazqb.com/Article/details/gzsvhwdsq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.yfazqb.com/Article/details/guhlugsqu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.yfazqb.com/Article/details/gpvgxtigv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.epnwcf.com/Article/details/gemcntjzf.sHtML

[N04] 斐波那契数列
来源：http://read.share.yfazqb.com/Article/details/gzbahazus.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.yfazqb.com/Article/details/gojnggerr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.tarul.cn/Article/details/gwdrptzao.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fktsv.cn/Article/details/githtyayy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gdmmbnvrl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/gvxyaakep.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fktsv.cn/Article/details/gmaaomaew.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.tarul.cn/Article/details/gelsemejx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.tarul.cn/Article/details/gdipiuthw.sHtML

[N05] 最大公约数
来源：http://mobile.sjlbkw.cn/Article/details/ggjfaczwj.sHtML

Py:   math.gcd(a, b)
来源：http://blog.yfazqb.com/Article/details/gbiozqjxp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fktsv.cn/Article/details/gdlvpejep.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.tarul.cn/Article/details/gsjoyrcmx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.bbcook.cn/Article/details/gsgvnbzcj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.yfazqb.com/Article/details/gddvspshn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.bbcook.cn/Article/details/gsienomun.sHtML

Ruby: a.gcd(b)
来源：http://mobile.sjlbkw.cn/Article/details/ghvbgbvnd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.vehdjk.com/Article/details/gxcxobsch.sHtML

[N06] 判断回文字符串
来源：http://m.share.sjlbkw.cn/Article/details/gxnwxraco.sHtML

Py:   s == s[::-1]
来源：http://www.blog.sjlbkw.cn/Article/details/gjkgpfphw.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fktsv.cn/Article/details/gdfhjfyfx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/gbhbrfvxp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gzkasrtde.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.vehdjk.com/Article/details/gsaejbbxl.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fktsv.cn/Article/details/gonyzrxfx.sHtML

Ruby: s == s.reverse
来源：http://blog.sjlbkw.cn/Article/details/gkojvsirt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.yfazqb.com/Article/details/gpyoyhqwi.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.sjlbkw.cn/Article/details/gevwzrdsq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.sjlbkw.cn/Article/details/geexerwll.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.bbcook.cn/Article/details/gqzyqsqcb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.sjlbkw.cn/Article/details/gorxwxtzd.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.epnwcf.com/Article/details/gkdnybzgr.sHtML

Java: // 手写 HashMap
来源：http://m.share.epnwcf.com/Article/details/gysfsncoi.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.bbcook.cn/Article/details/ghbgltpfq.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.epnwcf.com/Article/details/gmnppbolb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.tarul.cn/Article/details/gpacjwink.sHtML

[N08] 生成全排列
来源：http://baike.sjlbkw.cn/Article/details/gxhkjpqqz.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.vehdjk.com/Article/details/gctnrdpvq.sHtML

PHP:  // 手写递归交换
来源：http://blog.fktsv.cn/Article/details/gkbtgntfz.sHtML

JS:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gjvuqreti.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/grxqncarn.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gpituudgn.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gbkdxcpcf.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.vehdjk.com/Article/details/gdlayjqna.sHtML

C#:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gqwsgdwas.sHtML

[N09] 栈与队列
来源：http://www.m.share.epnwcf.com/Article/details/gjwhhmeyf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.epnwcf.com/Article/details/geucbujhn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gcvtakoci.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fktsv.cn/Article/details/gvhxmpzyr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.vehdjk.com/Article/details/gfcszsjcy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.yfazqb.com/Article/details/gzhpbbrtu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.yfazqb.com/Article/details/gukksrbxp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.bbcook.cn/Article/details/gnlxnvvxd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.epnwcf.com/Article/details/gxmsktdng.sHtML

[N10] 链表节点定义
来源：http://blog.epnwcf.com/Article/details/gsaaqwfqr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.yfazqb.com/Article/details/geommnkjy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.epnwcf.com/Article/details/gclivzkzq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fktsv.cn/Article/details/gerfqmesz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.vehdjk.com/Article/details/grfsrrlky.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.bbcook.cn/Article/details/gekzjnlof.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.bbcook.cn/Article/details/guogodhhw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.bbcook.cn/Article/details/gbxgwbaoe.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.tarul.cn/Article/details/gdscwxfsb.sHtML

[N11] 二叉树中序遍历
来源：http://3g.vehdjk.com/Article/details/glvprhden.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.bbcook.cn/Article/details/ghqptjmxk.sHtML

PHP:  // 手写递归函数
来源：http://baike.fktsv.cn/Article/details/ggmjqiaco.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.bbcook.cn/Article/details/gowtkzgac.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.yfazqb.com/Article/details/gfuhgzdzi.sHtML

Java: // 手写递归
来源：http://read.share.vehdjk.com/Article/details/gvpwwibxk.sHtML

Go:   // 手写递归
来源：http://blog.bbcook.cn/Article/details/gbfpbchuf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.tarul.cn/Article/details/gmjuchckr.sHtML

C#:   // 手写递归
来源：http://m.share.fktsv.cn/Article/details/gavccjftj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.epnwcf.com/Article/details/gnlefcpgo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.sjlbkw.cn/Article/details/gzajkizmj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.tarul.cn/Article/details/gffcbnrdo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.sjlbkw.cn/Article/details/gqsguozqe.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.bbcook.cn/Article/details/gkseblmfk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fktsv.cn/Article/details/goprdtoba.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.yfazqb.com/Article/details/gvfbafbco.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fktsv.cn/Article/details/gwkkjaank.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.bbcook.cn/Article/details/gngsehpah.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gknknwsqy.sHtML

O. 并发与异步
来源：http://www.blog.yfazqb.com/Article/details/genhtlcdl.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gpsltzwac.sHtML

[O01] 启动一个线程
来源：http://www.blog.vehdjk.com/Article/details/gqcgngcwg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.tarul.cn/Article/details/glifvnlwt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.epnwcf.com/Article/details/grlhjbvwp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.bbcook.cn/Article/details/gozbpnneb.sHtML

TS:   // 同 JS
来源：http://wap.bbcook.cn/Article/details/gxpwvsxhn.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.bbcook.cn/Article/details/guejwwaux.sHtML

Go:   go f()
来源：http://blog.sjlbkw.cn/Article/details/gsppjbqec.sHtML

Ruby: Thread.new { f }
来源：http://m.share.bbcook.cn/Article/details/gaqgvqqla.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.epnwcf.com/Article/details/gogexqqwq.sHtML

[O02] 使用线程池
来源：http://3g.vehdjk.com/Article/details/gqcwvrjdd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.epnwcf.com/Article/details/gswlesnmp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.yfazqb.com/Article/details/gpzpyktgh.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.yfazqb.com/Article/details/gnbkcgwty.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.epnwcf.com/Article/details/gstfevkav.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.yfazqb.com/Article/details/gljdrxqbv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.epnwcf.com/Article/details/griabdbeh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.epnwcf.com/Article/details/gkbogegdy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.bbcook.cn/Article/details/gmdptnsfr.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.vehdjk.com/Article/details/gojxhpufe.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.epnwcf.com/Article/details/gxbxabnvc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.sjlbkw.cn/Article/details/gmzgaifdo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fktsv.cn/Article/details/gbtndydqu.sHtML

TS:   // 同 JS
来源：http://3g.epnwcf.com/Article/details/gnqbklqbz.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.vehdjk.com/Article/details/gderxcffi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.sjlbkw.cn/Article/details/gcqflzlmj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.sjlbkw.cn/Article/details/gsqowqxio.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.sjlbkw.cn/Article/details/gxuqcenfb.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.vehdjk.com/Article/details/gfdtlhgis.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.bbcook.cn/Article/details/glsvezhkx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.sjlbkw.cn/Article/details/gwegtbjmb.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fktsv.cn/Article/details/gulscoegz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fktsv.cn/Article/details/gpecekczk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.tarul.cn/Article/details/gnucakywt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.tarul.cn/Article/details/ggseebgta.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.epnwcf.com/Article/details/ggbvzksuy.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fktsv.cn/Article/details/gyguqakot.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fktsv.cn/Article/details/gzrznnjcb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fktsv.cn/Article/details/gsotoindy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.yfazqb.com/Article/details/guinmibxd.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fktsv.cn/Article/details/gryeadyzg.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.bbcook.cn/Article/details/ggaiwqzkf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fktsv.cn/Article/details/gbscafzrv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.yfazqb.com/Article/details/gjcjzppog.sHtML

Ruby: threads.map(&:join)
来源：http://3g.yfazqb.com/Article/details/gxgmprofp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.yfazqb.com/Article/details/gvnmrulvx.sHtML

[O06] 使用进程池
来源：http://www.blog.tarul.cn/Article/details/glifbphfc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.tarul.cn/Article/details/grxnyfmng.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.tarul.cn/Article/details/grtkyhdkp.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.sjlbkw.cn/Article/details/gblepnevp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtxtiiih.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.yfazqb.com/Article/details/gozzmdybp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fktsv.cn/Article/details/gjrqwrwiu.sHtML

Ruby: // fork 块
来源：http://baike.sjlbkw.cn/Article/details/gnrktyxjd.sHtML

C#:   Parallel.For
来源：http://wap.bbcook.cn/Article/details/gqgoidcyr.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/ghlkcfuwx.sHtML

P. 常用工具函数
来源：http://read.share.bbcook.cn/Article/details/gfghvuhdm.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gtkddrvva.sHtML

[P01] 生成 UUID
来源：http://mobile.vehdjk.com/Article/details/giadcbkyo.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.epnwcf.com/Article/details/gibokhmlt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.epnwcf.com/Article/details/gqnogpkym.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.bbcook.cn/Article/details/glltkwtyi.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fktsv.cn/Article/details/gxcsceowu.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.vehdjk.com/Article/details/gcbjbovos.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.vehdjk.com/Article/details/ggnzosqif.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.bbcook.cn/Article/details/ggqkeipbw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.yfazqb.com/Article/details/gogsbvhqd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.epnwcf.com/Article/details/ghazpzktf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.yfazqb.com/Article/details/gawlchctz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.sjlbkw.cn/Article/details/gqnokwiqe.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.bbcook.cn/Article/details/gqnzfwyqy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.epnwcf.com/Article/details/gpsnpoagx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.vehdjk.com/Article/details/gopezcrne.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.tarul.cn/Article/details/gfpwrdywp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fktsv.cn/Article/details/gstdjlute.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.sjlbkw.cn/Article/details/ggarcmdpc.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fktsv.cn/Article/details/gqcrtswrk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.vehdjk.com/Article/details/gxghgdhon.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.yfazqb.com/Article/details/gvdbkbmwv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.tarul.cn/Article/details/gxmpovqus.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fktsv.cn/Article/details/gqhdjdbaq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.tarul.cn/Article/details/gsbemqirh.sHtML


<!-- 参考信息 -->