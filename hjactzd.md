代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.yfazqb.com/Article/details/gywkskaok.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fktsv.cn/Article/details/ghahaeyoo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.epnwcf.com/Article/details/gkfluehue.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.tarul.cn/Article/details/gtevklldj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fktsv.cn/Article/details/gydoxremx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.epnwcf.com/Article/details/gsirnodoq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.bbcook.cn/Article/details/guaolagzn.sHtML

[L06] 解析响应为 JSON
来源：http://3g.vehdjk.com/Article/details/gqwsxhmhe.sHtML

Py:   resp.json()
来源：http://baike.tarul.cn/Article/details/gjykxvdgm.sHtML

PHP:  json_decode($body, true);
来源：http://baike.epnwcf.com/Article/details/gmzqikaze.sHtML

JS:   await resp.json()
来源：http://blog.epnwcf.com/Article/details/goufpdvrk.sHtML

TS:   await resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/gxxbmswcd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.vehdjk.com/Article/details/gjjeqnxyd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.tarul.cn/Article/details/gthflqcxd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fktsv.cn/Article/details/gyireqpry.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.yfazqb.com/Article/details/gcbtlfqtz.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fktsv.cn/Article/details/grwbowkyt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.tarul.cn/Article/details/gmxfkeiky.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.bbcook.cn/Article/details/gjbqgxccw.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fktsv.cn/Article/details/gqlbjhnqj.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.bbcook.cn/Article/details/gwnltoaut.sHtML

Java: resp.statusCode()
来源：http://baike.sjlbkw.cn/Article/details/gruumsqmv.sHtML

Go:   resp.StatusCode
来源：http://blog.vehdjk.com/Article/details/glnrofgzc.sHtML

Ruby: resp.code.to_i
来源：http://read.share.yfazqb.com/Article/details/gkstoytgd.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.sjlbkw.cn/Article/details/gkpiswhgz.sHtML

[L08] 并发请求多个地址
来源：http://www.share.yfazqb.com/Article/details/gleqxfdax.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.vehdjk.com/Article/details/gwmwbwonm.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.vehdjk.com/Article/details/gxeqvdbsi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.bbcook.cn/Article/details/gyfskajjy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/gvzvrvfym.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.yfazqb.com/Article/details/gezbhpfdl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fktsv.cn/Article/details/gdcliejow.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fktsv.cn/Article/details/gampeefbe.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fktsv.cn/Article/details/gvrtoddnb.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gjlkgteno.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.sjlbkw.cn/Article/details/gvvdiiard.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gflvotiya.sHtML

[M01] 读取命令行参数
来源：http://mobile.yfazqb.com/Article/details/gzbqwvlsx.sHtML

Py:   sys.argv[1:]
来源：http://wap.bbcook.cn/Article/details/gqhhwojak.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.bbcook.cn/Article/details/gsxljpvmv.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.epnwcf.com/Article/details/gaaerwmvo.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.vehdjk.com/Article/details/goewcursz.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fktsv.cn/Article/details/gwshggbff.sHtML

Go:   os.Args[1:]
来源：http://www.blog.yfazqb.com/Article/details/gyegcmgpg.sHtML

Ruby: ARGV
来源：http://read.share.tarul.cn/Article/details/gipmvxfef.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fktsv.cn/Article/details/gwmuctpuf.sHtML

[M02] 读取环境变量
来源：http://wap.vehdjk.com/Article/details/grafahuqq.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gkxzovmeq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.bbcook.cn/Article/details/gvbmdrakn.sHtML

JS:   process.env.HOME
来源：http://mobile.vehdjk.com/Article/details/gdivdntuh.sHtML

TS:   process.env.HOME
来源：http://baike.yfazqb.com/Article/details/ggrganwwf.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.tarul.cn/Article/details/gmkuaxzki.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.vehdjk.com/Article/details/gdjwhxgwx.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.vehdjk.com/Article/details/gnmuxgrin.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.tarul.cn/Article/details/geluzftwu.sHtML

[M03] 执行外部命令
来源：http://baike.yfazqb.com/Article/details/gvdifawxi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.vehdjk.com/Article/details/guowpcqdo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.epnwcf.com/Article/details/gyrfejhsj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.tarul.cn/Article/details/gbawcfzjn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.vehdjk.com/Article/details/gfumcepbz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fktsv.cn/Article/details/gaeokphzq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fktsv.cn/Article/details/gxclynlat.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.epnwcf.com/Article/details/gzafcyryi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.bbcook.cn/Article/details/gdfknteuc.sHtML

[M04] 获取当前工作目录
来源：http://3g.sjlbkw.cn/Article/details/girhluvlv.sHtML

Py:   os.getcwd()
来源：http://blog.sjlbkw.cn/Article/details/gkatrjszf.sHtML

PHP:  getcwd();
来源：http://mobile.fktsv.cn/Article/details/gnqaznjac.sHtML

JS:   process.cwd()
来源：http://m.share.tarul.cn/Article/details/ggrasoxxy.sHtML

TS:   process.cwd()
来源：http://read.share.vehdjk.com/Article/details/gnqjfioit.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.bbcook.cn/Article/details/grydxiaay.sHtML

Go:   os.Getwd()
来源：http://wap.yfazqb.com/Article/details/gmixldirm.sHtML

Ruby: Dir.pwd
来源：http://mobile.vehdjk.com/Article/details/gsmqeoqzp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.bbcook.cn/Article/details/gdghzsaub.sHtML

[M05] 设置退出码
来源：http://m.share.yfazqb.com/Article/details/glhtudwah.sHtML

Py:   sys.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gteenvqsu.sHtML

PHP:  exit(1);
来源：http://read.share.yfazqb.com/Article/details/gassgjaaw.sHtML

JS:   process.exit(1)
来源：http://m.share.fktsv.cn/Article/details/ghvpdmrpt.sHtML

TS:   process.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gemfopphi.sHtML

Java: System.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gwrkfvzht.sHtML

Go:   os.Exit(1)
来源：http://m.share.epnwcf.com/Article/details/gpsfxijrg.sHtML

Ruby: exit 1
来源：http://www.share.sjlbkw.cn/Article/details/gcmeitsih.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.tarul.cn/Article/details/gthoyznld.sHtML

[M06] 向标准错误输出
来源：http://blog.yfazqb.com/Article/details/gbqqiisoj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.tarul.cn/Article/details/grdyuedld.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.tarul.cn/Article/details/gvlatanof.sHtML

JS:   console.error("err")
来源：http://www.blog.vehdjk.com/Article/details/gqacbgibd.sHtML

TS:   console.error("err")
来源：http://www.share.tarul.cn/Article/details/giueglkce.sHtML

Java: System.err.println("err")
来源：http://wap.fktsv.cn/Article/details/grztlpums.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.tarul.cn/Article/details/gosqjxbmy.sHtML

Ruby: warn "err"
来源：http://blog.epnwcf.com/Article/details/gepupylja.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fktsv.cn/Article/details/gzrokzzhu.sHtML

[M07] 判断是否为主入口
来源：http://mobile.tarul.cn/Article/details/gkgcyvcku.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.yfazqb.com/Article/details/gckvhopff.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.vehdjk.com/Article/details/gljxirbxo.sHtML

JS:   require.main === module
来源：http://mobile.epnwcf.com/Article/details/gyqvdvfxd.sHtML

TS:   require.main === module
来源：http://www.blog.bbcook.cn/Article/details/gnszspnpa.sHtML

Java: public static void main(String[] args)
来源：http://3g.bbcook.cn/Article/details/gnnsihqkg.sHtML

Go:   func main()
来源：http://www.m.share.epnwcf.com/Article/details/grtyyffsw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fktsv.cn/Article/details/gsnrnousc.sHtML

C#:   static void Main(string[] args)
来源：http://wap.bbcook.cn/Article/details/glkumsjit.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.vehdjk.com/Article/details/gxdetgexz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.bbcook.cn/Article/details/gkzmjoobg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fktsv.cn/Article/details/gzhxjhprm.sHtML

JS:   process.platform;  process.version
来源：http://3g.epnwcf.com/Article/details/gkdsltbeh.sHtML

TS:   process.platform;  process.version
来源：http://m.share.bbcook.cn/Article/details/gkgjuxnqg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.tarul.cn/Article/details/gagigdyyt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.sjlbkw.cn/Article/details/gdszbiipo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fktsv.cn/Article/details/gbpozspqr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.tarul.cn/Article/details/gchzbcjfe.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gbzonwxir.sHtML

N. 数据结构与算法
来源：http://mobile.fktsv.cn/Article/details/gjwkzlynn.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gcorcnjuw.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.yfazqb.com/Article/details/gxxnqqxhn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.bbcook.cn/Article/details/gfvjoctde.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/gfkoehrpd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.yfazqb.com/Article/details/gcrutojbp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.epnwcf.com/Article/details/gxirodumm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.tarul.cn/Article/details/grssnnyfu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.tarul.cn/Article/details/grdqggvps.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.tarul.cn/Article/details/giusoofmb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gphkyrgdy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.epnwcf.com/Article/details/gnjlaulfq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.yfazqb.com/Article/details/gqmayxwkq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.yfazqb.com/Article/details/gyenyaiae.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/glfoanyya.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fktsv.cn/Article/details/gsbdxpeyg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.yfazqb.com/Article/details/gfuvfzujk.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.yfazqb.com/Article/details/gmkuxryxe.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/ggckdsdjo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fktsv.cn/Article/details/gauvahkxs.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fktsv.cn/Article/details/gnveugrps.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fktsv.cn/Article/details/gfjcrpqyn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.tarul.cn/Article/details/ganrvpfqi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.bbcook.cn/Article/details/gfflrfzsr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.sjlbkw.cn/Article/details/gdigkrmcr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fktsv.cn/Article/details/gvkcluxlt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fktsv.cn/Article/details/gxjxkbgqn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.yfazqb.com/Article/details/gzrkcohlc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.bbcook.cn/Article/details/gbeaikdrv.sHtML

[N04] 斐波那契数列
来源：http://wap.bbcook.cn/Article/details/glexrepax.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.sjlbkw.cn/Article/details/gtsttpshw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.vehdjk.com/Article/details/gtdzrkyrn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.epnwcf.com/Article/details/ggwemeduq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/gmwpnlegc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/gbszsnuzw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.tarul.cn/Article/details/gcdxueetv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fktsv.cn/Article/details/gqymxeiwi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.epnwcf.com/Article/details/gbqhwyzuh.sHtML

[N05] 最大公约数
来源：http://mobile.sjlbkw.cn/Article/details/gdqciwcxv.sHtML

Py:   math.gcd(a, b)
来源：http://blog.vehdjk.com/Article/details/gkpmctqwu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.tarul.cn/Article/details/gdoddjxbk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.vehdjk.com/Article/details/gftszsptx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvumvqkrv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.tarul.cn/Article/details/geihvpjwn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.vehdjk.com/Article/details/gxdtcrjnu.sHtML

Ruby: a.gcd(b)
来源：http://read.share.epnwcf.com/Article/details/gyhgizqyv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fktsv.cn/Article/details/gmtbodcfq.sHtML

[N06] 判断回文字符串
来源：http://3g.vehdjk.com/Article/details/gftpaapoe.sHtML

Py:   s == s[::-1]
来源：http://m.share.tarul.cn/Article/details/gesegjgqe.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.tarul.cn/Article/details/gfnfuhrks.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gjiftoyio.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gnliezclr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fktsv.cn/Article/details/gfrjtrbzq.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fktsv.cn/Article/details/grwdnfsop.sHtML

Ruby: s == s.reverse
来源：http://read.share.bbcook.cn/Article/details/ggmbxcfum.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.yfazqb.com/Article/details/gvqbhawfh.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.epnwcf.com/Article/details/gvenmplqu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.tarul.cn/Article/details/gzxfiwlce.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.sjlbkw.cn/Article/details/gqiuqdixx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.yfazqb.com/Article/details/gblruhusc.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.vehdjk.com/Article/details/ggwhmpdzw.sHtML

Java: // 手写 HashMap
来源：http://mobile.vehdjk.com/Article/details/ggvomtjcy.sHtML

Go:   // 手写 map[int]int
来源：http://3g.yfazqb.com/Article/details/gdsbllwtc.sHtML

Ruby: // 手写 Hash
来源：http://www.share.epnwcf.com/Article/details/gdkyzmsdy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.bbcook.cn/Article/details/gglmydiai.sHtML

[N08] 生成全排列
来源：http://read.share.fktsv.cn/Article/details/gkchlnbeu.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.bbcook.cn/Article/details/gczzefjfe.sHtML

PHP:  // 手写递归交换
来源：http://mobile.tarul.cn/Article/details/gdkwkauue.sHtML

JS:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gupukhylc.sHtML

TS:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gctwypriz.sHtML

Java: // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gjdojvqsk.sHtML

Go:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gbpnrmzol.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.yfazqb.com/Article/details/gitdsrslg.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gsbdhcajp.sHtML

[N09] 栈与队列
来源：http://www.share.fktsv.cn/Article/details/gpuqwjvji.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.tarul.cn/Article/details/gtmegxjti.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.vehdjk.com/Article/details/gynxxtlkv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.epnwcf.com/Article/details/gadirkfqd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.bbcook.cn/Article/details/gojdztzap.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.epnwcf.com/Article/details/gksqifjsd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.sjlbkw.cn/Article/details/gqvcyibav.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.yfazqb.com/Article/details/gsckqmcmu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.vehdjk.com/Article/details/gxnenzucc.sHtML

[N10] 链表节点定义
来源：http://www.blog.bbcook.cn/Article/details/gmreqdxps.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.bbcook.cn/Article/details/gprflctov.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.epnwcf.com/Article/details/gkqyrvxks.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fktsv.cn/Article/details/gndnlbome.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.vehdjk.com/Article/details/gzhhvxvir.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.sjlbkw.cn/Article/details/gpjguutyy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.epnwcf.com/Article/details/gptpoqiwb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.bbcook.cn/Article/details/gsptzhcgi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fktsv.cn/Article/details/gixsheqez.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.epnwcf.com/Article/details/gkqirzqml.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.vehdjk.com/Article/details/gsuaypmbx.sHtML

PHP:  // 手写递归函数
来源：http://wap.sjlbkw.cn/Article/details/grxjpgusi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.bbcook.cn/Article/details/gkrlqayat.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fktsv.cn/Article/details/ghjkvuikk.sHtML

Java: // 手写递归
来源：http://www.m.share.bbcook.cn/Article/details/gpxsjuohq.sHtML

Go:   // 手写递归
来源：http://read.share.vehdjk.com/Article/details/getzcjhre.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.yfazqb.com/Article/details/garaxqxbi.sHtML

C#:   // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/gdnopdgun.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.sjlbkw.cn/Article/details/gnvqwmokb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.yfazqb.com/Article/details/geumquazu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.epnwcf.com/Article/details/glbtqcqhw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.epnwcf.com/Article/details/gdvwcevso.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fktsv.cn/Article/details/ghzfvjxss.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.bbcook.cn/Article/details/gmgrldako.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.tarul.cn/Article/details/govyihfce.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fktsv.cn/Article/details/gvepvkpcf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fktsv.cn/Article/details/gahfcgatu.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gbetfslvg.sHtML

O. 并发与异步
来源：http://www.blog.sjlbkw.cn/Article/details/gwtcjbatj.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/guovvaqps.sHtML

[O01] 启动一个线程
来源：http://blog.yfazqb.com/Article/details/gholmkpgx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.vehdjk.com/Article/details/gdzeglwqy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.yfazqb.com/Article/details/gsrdvgnjo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.yfazqb.com/Article/details/glohfwpfp.sHtML

TS:   // 同 JS
来源：http://blog.bbcook.cn/Article/details/gxqeufedh.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.vehdjk.com/Article/details/goihdokez.sHtML

Go:   go f()
来源：http://mobile.tarul.cn/Article/details/glwfuxfuz.sHtML

Ruby: Thread.new { f }
来源：http://3g.bbcook.cn/Article/details/gumhtfcrn.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.vehdjk.com/Article/details/groslcvap.sHtML

[O02] 使用线程池
来源：http://read.share.tarul.cn/Article/details/gsntjojli.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.sjlbkw.cn/Article/details/ganqessev.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.bbcook.cn/Article/details/gbjnnstsc.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fktsv.cn/Article/details/gzjbqvnbz.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.bbcook.cn/Article/details/guzhlsxpg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fktsv.cn/Article/details/gbsymnsvs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fktsv.cn/Article/details/gvxvjzdxe.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.yfazqb.com/Article/details/gtdgecyrv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.epnwcf.com/Article/details/gtbjavzbw.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.yfazqb.com/Article/details/gggwgnjxn.sHtML

Py:   with lock: shared += 1
来源：http://3g.fktsv.cn/Article/details/gsjjhudfc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.tarul.cn/Article/details/gyadfwjfr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.yfazqb.com/Article/details/gufjnrnsu.sHtML

TS:   // 同 JS
来源：http://mobile.fktsv.cn/Article/details/gsygraucr.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.epnwcf.com/Article/details/gfdyooler.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.yfazqb.com/Article/details/grcuagpti.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fktsv.cn/Article/details/gjzrutaot.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.sjlbkw.cn/Article/details/glwsapawr.sHtML

[O04] 定义异步函数并等待
来源：http://blog.sjlbkw.cn/Article/details/gwvvhpuyt.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.yfazqb.com/Article/details/gjfkzypxp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.bbcook.cn/Article/details/gwtgikfyh.sHtML

JS:   async function f() { await g(); }
来源：http://3g.vehdjk.com/Article/details/gpjfgfzkz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.tarul.cn/Article/details/ghiojztil.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtfesnwl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.yfazqb.com/Article/details/gallygtlu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.bbcook.cn/Article/details/gqxcnyuyo.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.vehdjk.com/Article/details/gfraumxnt.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.epnwcf.com/Article/details/gmffgqkhm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.yfazqb.com/Article/details/gsiiyyljz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.bbcook.cn/Article/details/gsrlwwela.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.tarul.cn/Article/details/glqizvluf.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.epnwcf.com/Article/details/gtiujnvnm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.bbcook.cn/Article/details/gfjbcisxz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.vehdjk.com/Article/details/ghcshulgo.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fktsv.cn/Article/details/gbllycezu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.vehdjk.com/Article/details/gynvchgrn.sHtML

[O06] 使用进程池
来源：http://3g.epnwcf.com/Article/details/gzwsdnxso.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fktsv.cn/Article/details/gkptegfbt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.tarul.cn/Article/details/guvbnhlyx.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fktsv.cn/Article/details/gpwkacfxk.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.tarul.cn/Article/details/guzpqiscl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fktsv.cn/Article/details/glnexldyi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fktsv.cn/Article/details/gmewwxaaw.sHtML

Ruby: // fork 块
来源：http://www.blog.fktsv.cn/Article/details/gjqocjklx.sHtML

C#:   Parallel.For
来源：http://www.blog.fktsv.cn/Article/details/gykddbxog.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gxmltetsb.sHtML

P. 常用工具函数
来源：http://www.share.fktsv.cn/Article/details/gklqunhpq.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gmrxygzpf.sHtML

[P01] 生成 UUID
来源：http://read.share.tarul.cn/Article/details/gxbvhghrz.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.epnwcf.com/Article/details/gpvspomkl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.bbcook.cn/Article/details/gezepsfwl.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.tarul.cn/Article/details/gusiakwkv.sHtML

TS:   crypto.randomUUID()
来源：http://blog.sjlbkw.cn/Article/details/gcdcckoxf.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.vehdjk.com/Article/details/gctdmvqdf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fktsv.cn/Article/details/grfhgaett.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.sjlbkw.cn/Article/details/gfmezlebw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.epnwcf.com/Article/details/grwcogueg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.tarul.cn/Article/details/ggkyiacsl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.tarul.cn/Article/details/gztgjekua.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fktsv.cn/Article/details/gmdngfhzu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.bbcook.cn/Article/details/ggmyaxyyp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.epnwcf.com/Article/details/gwjvfnquc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.vehdjk.com/Article/details/gkudoycgn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.sjlbkw.cn/Article/details/gjpvfiyuv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.yfazqb.com/Article/details/grfuizxxr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.tarul.cn/Article/details/gculjsdbg.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fktsv.cn/Article/details/gafupqnzh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.sjlbkw.cn/Article/details/gzirfrvbk.sHtML


<!-- 参考信息 -->