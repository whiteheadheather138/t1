代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fktsv.cn/Article/details/gvjtovmhr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.vehdjk.com/Article/details/gvzzycime.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.tarul.cn/Article/details/gdduteflj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.tarul.cn/Article/details/gdewhnmea.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.epnwcf.com/Article/details/gwslucepn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.epnwcf.com/Article/details/gczfdvgyf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.yfazqb.com/Article/details/gqgbecosm.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.sjlbkw.cn/Article/details/gixiyptup.sHtML

Py:   resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/gfxhdofpb.sHtML

PHP:  json_decode($body, true);
来源：http://baike.tarul.cn/Article/details/gayqfnbqi.sHtML

JS:   await resp.json()
来源：http://www.m.share.tarul.cn/Article/details/geqvmnwfa.sHtML

TS:   await resp.json()
来源：http://www.m.share.sjlbkw.cn/Article/details/gyivzauol.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.yfazqb.com/Article/details/gxzeczmcq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.yfazqb.com/Article/details/guieoxvyu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.yfazqb.com/Article/details/gwqhclvzi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fktsv.cn/Article/details/gvodnompa.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.yfazqb.com/Article/details/gecjpidtv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.epnwcf.com/Article/details/glkmwbxnf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.sjlbkw.cn/Article/details/gwoedhpty.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fktsv.cn/Article/details/glprkwpvc.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.sjlbkw.cn/Article/details/gdvxtkpmh.sHtML

Java: resp.statusCode()
来源：http://read.share.bbcook.cn/Article/details/guglpyieo.sHtML

Go:   resp.StatusCode
来源：http://baike.bbcook.cn/Article/details/gxcosnmly.sHtML

Ruby: resp.code.to_i
来源：http://wap.tarul.cn/Article/details/gprdxrfgo.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.yfazqb.com/Article/details/gtoxfxlya.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.yfazqb.com/Article/details/gyfxikmeg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.tarul.cn/Article/details/gdhbervbw.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.vehdjk.com/Article/details/gmhpmqqxh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.sjlbkw.cn/Article/details/gwkjldvgo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.epnwcf.com/Article/details/gvpceuxuc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.vehdjk.com/Article/details/gfecolvmc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fktsv.cn/Article/details/gqskxecec.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.sjlbkw.cn/Article/details/gebfannqo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.tarul.cn/Article/details/gzhveqrck.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gfpnjrjfx.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.epnwcf.com/Article/details/gkwrxngkn.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gqehcmhip.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.yfazqb.com/Article/details/ggtgcvvot.sHtML

Py:   sys.argv[1:]
来源：http://www.share.epnwcf.com/Article/details/gyktyukmt.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fktsv.cn/Article/details/gitbutail.sHtML

JS:   process.argv.slice(2)
来源：http://baike.tarul.cn/Article/details/gfkysfeku.sHtML

TS:   process.argv.slice(2)
来源：http://blog.sjlbkw.cn/Article/details/gwztszhex.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.sjlbkw.cn/Article/details/gbjjnuuqs.sHtML

Go:   os.Args[1:]
来源：http://m.share.bbcook.cn/Article/details/gzxdufcpz.sHtML

Ruby: ARGV
来源：http://www.m.share.epnwcf.com/Article/details/gcyksjrzx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.vehdjk.com/Article/details/gjschsshe.sHtML

[M02] 读取环境变量
来源：http://m.share.fktsv.cn/Article/details/gpswvfzlh.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.epnwcf.com/Article/details/gvzmqkank.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.sjlbkw.cn/Article/details/gitariuyn.sHtML

JS:   process.env.HOME
来源：http://www.blog.yfazqb.com/Article/details/gcbbtnfju.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fktsv.cn/Article/details/gbhvlbxxj.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fktsv.cn/Article/details/gfwzivogv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fktsv.cn/Article/details/gywzecqzz.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.yfazqb.com/Article/details/gbznpewpx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.epnwcf.com/Article/details/gwactnxki.sHtML

[M03] 执行外部命令
来源：http://www.blog.vehdjk.com/Article/details/gfvpzeefn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.bbcook.cn/Article/details/gltsgaqji.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.sjlbkw.cn/Article/details/gjgpdmzfa.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.tarul.cn/Article/details/gowokrvgj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.vehdjk.com/Article/details/gcuzrilpz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.yfazqb.com/Article/details/gomyvsgsg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.sjlbkw.cn/Article/details/gyuvozulh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.tarul.cn/Article/details/gpmsycrxf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.sjlbkw.cn/Article/details/gpubzufwp.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fktsv.cn/Article/details/gfsygolmi.sHtML

Py:   os.getcwd()
来源：http://baike.tarul.cn/Article/details/gimqsxlhs.sHtML

PHP:  getcwd();
来源：http://blog.bbcook.cn/Article/details/gzokhlfvy.sHtML

JS:   process.cwd()
来源：http://www.share.tarul.cn/Article/details/gzcrqcfyo.sHtML

TS:   process.cwd()
来源：http://wap.fktsv.cn/Article/details/gkuvpteud.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fktsv.cn/Article/details/gvmzizoue.sHtML

Go:   os.Getwd()
来源：http://www.m.share.bbcook.cn/Article/details/gujhpyvfc.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.bbcook.cn/Article/details/gafmnytkr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.yfazqb.com/Article/details/ggljezncc.sHtML

[M05] 设置退出码
来源：http://wap.yfazqb.com/Article/details/godfpcstl.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gwiofmete.sHtML

PHP:  exit(1);
来源：http://www.m.share.fktsv.cn/Article/details/gcuqhgkac.sHtML

JS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gecjdylzl.sHtML

TS:   process.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gmrziuard.sHtML

Java: System.exit(1)
来源：http://read.share.vehdjk.com/Article/details/gluqgwyvb.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gyeybcphl.sHtML

Ruby: exit 1
来源：http://m.share.fktsv.cn/Article/details/glkjrlqle.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.tarul.cn/Article/details/gbneujalv.sHtML

[M06] 向标准错误输出
来源：http://wap.sjlbkw.cn/Article/details/gqrtvrier.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.epnwcf.com/Article/details/gpzrvfimz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.yfazqb.com/Article/details/gdwugzsrg.sHtML

JS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/gkizlmeub.sHtML

TS:   console.error("err")
来源：http://blog.bbcook.cn/Article/details/gfyoiosqx.sHtML

Java: System.err.println("err")
来源：http://wap.tarul.cn/Article/details/gjsmbonaz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.yfazqb.com/Article/details/gmhqrbezv.sHtML

Ruby: warn "err"
来源：http://blog.sjlbkw.cn/Article/details/gbiefdhpx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.sjlbkw.cn/Article/details/gkkpnpsdq.sHtML

[M07] 判断是否为主入口
来源：http://read.share.sjlbkw.cn/Article/details/gzomnkhsl.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.sjlbkw.cn/Article/details/gexnjevhu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.epnwcf.com/Article/details/gxywcafnj.sHtML

JS:   require.main === module
来源：http://3g.fktsv.cn/Article/details/gzyzxgaey.sHtML

TS:   require.main === module
来源：http://3g.yfazqb.com/Article/details/grjxdggma.sHtML

Java: public static void main(String[] args)
来源：http://wap.tarul.cn/Article/details/gsobtnwkk.sHtML

Go:   func main()
来源：http://www.share.sjlbkw.cn/Article/details/gtzknsvdg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fktsv.cn/Article/details/gyqrdfeyd.sHtML

C#:   static void Main(string[] args)
来源：http://baike.bbcook.cn/Article/details/gjychopgc.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.bbcook.cn/Article/details/gnubzxtsz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fktsv.cn/Article/details/gwsxopaqn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fktsv.cn/Article/details/gnttggkpc.sHtML

JS:   process.platform;  process.version
来源：http://blog.bbcook.cn/Article/details/goglfqyjr.sHtML

TS:   process.platform;  process.version
来源：http://mobile.tarul.cn/Article/details/gikjsfpys.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fktsv.cn/Article/details/gduqmevkv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.tarul.cn/Article/details/ghedhcmwm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.sjlbkw.cn/Article/details/gqdwufqdn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.yfazqb.com/Article/details/gynvicxjn.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gdlgnkave.sHtML

N. 数据结构与算法
来源：http://baike.bbcook.cn/Article/details/gvhbhxhrm.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gekastynb.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.yfazqb.com/Article/details/gqadnrmzh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.epnwcf.com/Article/details/ghoazllud.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gncixkklw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.yfazqb.com/Article/details/gdfmyhzsu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.tarul.cn/Article/details/gxqipcjfk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.tarul.cn/Article/details/gpngzkjsx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gwyeviqts.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.vehdjk.com/Article/details/gugytvwbc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gngzlocnl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.bbcook.cn/Article/details/gdxzzacwu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.vehdjk.com/Article/details/gycfekehh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.sjlbkw.cn/Article/details/gktozxnkp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/gytyhwbzg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.vehdjk.com/Article/details/gebauwfwk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.tarul.cn/Article/details/glupgwfye.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.bbcook.cn/Article/details/gtndehnwv.sHtML

Ruby: arr.sort
来源：http://www.m.share.fktsv.cn/Article/details/gxutesmpa.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fktsv.cn/Article/details/gprywhjrd.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.yfazqb.com/Article/details/gsjzattzb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.vehdjk.com/Article/details/gdynoizxc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.vehdjk.com/Article/details/gyikrnstb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.epnwcf.com/Article/details/gqwomdhpg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.tarul.cn/Article/details/gziyiidxu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.epnwcf.com/Article/details/girtdasvg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.epnwcf.com/Article/details/ggmzzqcwu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.sjlbkw.cn/Article/details/gttlxkghm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.tarul.cn/Article/details/gfjssokvy.sHtML

[N04] 斐波那契数列
来源：http://m.share.sjlbkw.cn/Article/details/ginzjzlhn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.bbcook.cn/Article/details/gqfctjtyk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.yfazqb.com/Article/details/gsjwzgqtw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.vehdjk.com/Article/details/giopvfbke.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/gyqxxkbdd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.vehdjk.com/Article/details/gnnqrkziy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.epnwcf.com/Article/details/gnmrilvdz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.bbcook.cn/Article/details/gtpfxwwsk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gohmyfokp.sHtML

[N05] 最大公约数
来源：http://baike.tarul.cn/Article/details/glywdqknz.sHtML

Py:   math.gcd(a, b)
来源：http://wap.tarul.cn/Article/details/gdvagxora.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gvxorjflu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.sjlbkw.cn/Article/details/gvnjovxxz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.yfazqb.com/Article/details/ggwqlfale.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.tarul.cn/Article/details/gjngyuzqb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fktsv.cn/Article/details/gumqwfrvf.sHtML

Ruby: a.gcd(b)
来源：http://baike.sjlbkw.cn/Article/details/gbtiwxvvn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.bbcook.cn/Article/details/gauhedhfi.sHtML

[N06] 判断回文字符串
来源：http://wap.vehdjk.com/Article/details/gryixvxvp.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.epnwcf.com/Article/details/gdfntycop.sHtML

PHP:  $s === strrev($s);
来源：http://3g.yfazqb.com/Article/details/gtarkyswy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/glvzwkolr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/glhiuongf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.vehdjk.com/Article/details/gskwbzuim.sHtML

Go:   // 双指针从两端比较
来源：http://wap.vehdjk.com/Article/details/gpidufcnq.sHtML

Ruby: s == s.reverse
来源：http://3g.sjlbkw.cn/Article/details/gtilokjww.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.bbcook.cn/Article/details/govxntjle.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fktsv.cn/Article/details/gtjjvszmn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fktsv.cn/Article/details/gchalhsio.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.epnwcf.com/Article/details/gofjcnuoy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.sjlbkw.cn/Article/details/geyifnwmf.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.epnwcf.com/Article/details/gagvektnm.sHtML

Java: // 手写 HashMap
来源：http://wap.tarul.cn/Article/details/ggdlywiip.sHtML

Go:   // 手写 map[int]int
来源：http://baike.epnwcf.com/Article/details/gkxgoqssc.sHtML

Ruby: // 手写 Hash
来源：http://3g.tarul.cn/Article/details/gkmgkkiys.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fktsv.cn/Article/details/glsbragvg.sHtML

[N08] 生成全排列
来源：http://wap.bbcook.cn/Article/details/gmojsujtx.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.vehdjk.com/Article/details/gppvtqfdl.sHtML

PHP:  // 手写递归交换
来源：http://www.share.sjlbkw.cn/Article/details/gqoykbnte.sHtML

JS:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gfjsehgav.sHtML

TS:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/ghfoenzmp.sHtML

Java: // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gfwoynwvc.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gplecnaak.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.tarul.cn/Article/details/gkekjpgxk.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gfdzigvzl.sHtML

[N09] 栈与队列
来源：http://www.blog.vehdjk.com/Article/details/gdhknafza.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.bbcook.cn/Article/details/ghidsvmjp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.tarul.cn/Article/details/ggwnnygnn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.vehdjk.com/Article/details/gwwtfcgbu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.sjlbkw.cn/Article/details/gnwydnctn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.bbcook.cn/Article/details/gbyeayjbl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.yfazqb.com/Article/details/gembcehst.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.sjlbkw.cn/Article/details/gvcmquohr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.epnwcf.com/Article/details/gvlwehfiu.sHtML

[N10] 链表节点定义
来源：http://www.blog.bbcook.cn/Article/details/gnymznogy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.bbcook.cn/Article/details/gowicmaqy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.epnwcf.com/Article/details/ggmttjpts.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.vehdjk.com/Article/details/gbbdgxzkr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.sjlbkw.cn/Article/details/glucthuiq.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkngiacht.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fktsv.cn/Article/details/gxnkcijch.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.sjlbkw.cn/Article/details/gfbkhwivq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.bbcook.cn/Article/details/gabhhvndt.sHtML

[N11] 二叉树中序遍历
来源：http://3g.vehdjk.com/Article/details/gcwiebmbt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.sjlbkw.cn/Article/details/grlgczyvb.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gqsfoycmc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.bbcook.cn/Article/details/gybfelmfo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.sjlbkw.cn/Article/details/gpntrqjov.sHtML

Java: // 手写递归
来源：http://read.share.epnwcf.com/Article/details/gtdpergfd.sHtML

Go:   // 手写递归
来源：http://www.share.vehdjk.com/Article/details/gjgabxhbr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.tarul.cn/Article/details/gvslmkhpt.sHtML

C#:   // 手写递归
来源：http://baike.fktsv.cn/Article/details/ghzerduxd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.bbcook.cn/Article/details/gozfjkzvv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.tarul.cn/Article/details/gtgwsgzet.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.sjlbkw.cn/Article/details/gocrskgwq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.vehdjk.com/Article/details/guuvpjxwq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.bbcook.cn/Article/details/gqvvqiwnv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.tarul.cn/Article/details/gyscczynw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.bbcook.cn/Article/details/gmxyadoks.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.tarul.cn/Article/details/gxkscxbac.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fktsv.cn/Article/details/grrsehpil.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gmkrdhglr.sHtML

O. 并发与异步
来源：http://www.m.share.tarul.cn/Article/details/girkuoupy.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gqydhdvcm.sHtML

[O01] 启动一个线程
来源：http://www.share.bbcook.cn/Article/details/gknzjvizd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.vehdjk.com/Article/details/grorenhli.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.bbcook.cn/Article/details/gmzpnutpn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.vehdjk.com/Article/details/gczpoiunz.sHtML

TS:   // 同 JS
来源：http://www.m.share.epnwcf.com/Article/details/ghpwifzle.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.vehdjk.com/Article/details/gdmpgtmbh.sHtML

Go:   go f()
来源：http://mobile.fktsv.cn/Article/details/guuyaurek.sHtML

Ruby: Thread.new { f }
来源：http://mobile.vehdjk.com/Article/details/guzofpizc.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.yfazqb.com/Article/details/gymeibxhn.sHtML

[O02] 使用线程池
来源：http://mobile.bbcook.cn/Article/details/gffmwrnzi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.epnwcf.com/Article/details/geqjpgfib.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.sjlbkw.cn/Article/details/ghwdxljtb.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.bbcook.cn/Article/details/ghamuvvyp.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.sjlbkw.cn/Article/details/gddkrwjsx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.epnwcf.com/Article/details/guwhddplf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fktsv.cn/Article/details/gmztzczcp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.yfazqb.com/Article/details/gilyycfne.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.bbcook.cn/Article/details/gtyyehyuz.sHtML

[O03] 加锁保护共享数据
来源：http://3g.yfazqb.com/Article/details/gijwfdzrq.sHtML

Py:   with lock: shared += 1
来源：http://www.share.yfazqb.com/Article/details/guwpwsgxg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fktsv.cn/Article/details/gdupoprjz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fktsv.cn/Article/details/gsqamwtqx.sHtML

TS:   // 同 JS
来源：http://baike.vehdjk.com/Article/details/guexfqadz.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.sjlbkw.cn/Article/details/goskndghy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.tarul.cn/Article/details/ggjnhaxfm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fktsv.cn/Article/details/gjpyvqwsz.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.vehdjk.com/Article/details/gyepcemqh.sHtML

[O04] 定义异步函数并等待
来源：http://3g.epnwcf.com/Article/details/gdyaxtlen.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.vehdjk.com/Article/details/gaibihluc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.tarul.cn/Article/details/gcsybfxwy.sHtML

JS:   async function f() { await g(); }
来源：http://3g.tarul.cn/Article/details/gwmvjajwi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.bbcook.cn/Article/details/gggsvuaeq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.bbcook.cn/Article/details/gxjhrpdle.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fktsv.cn/Article/details/gouaxhfur.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.yfazqb.com/Article/details/grmlwetwz.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.tarul.cn/Article/details/gcpfibexa.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fktsv.cn/Article/details/geqtdqvbk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.yfazqb.com/Article/details/gdadzsmnp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fktsv.cn/Article/details/gsmkhodsb.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrmqmcoh.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.tarul.cn/Article/details/gimkzkife.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.tarul.cn/Article/details/gitbnnibw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.sjlbkw.cn/Article/details/gilomiqzs.sHtML

Ruby: threads.map(&:join)
来源：http://blog.bbcook.cn/Article/details/gnqxtnffx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.bbcook.cn/Article/details/gjcezcajd.sHtML

[O06] 使用进程池
来源：http://3g.epnwcf.com/Article/details/gipbuzsdt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.bbcook.cn/Article/details/gdsboagmu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.yfazqb.com/Article/details/gbjblxpcg.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fktsv.cn/Article/details/gatprmacn.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.epnwcf.com/Article/details/goizsohdj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.yfazqb.com/Article/details/gztufbxex.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.vehdjk.com/Article/details/gmgzzpwea.sHtML

Ruby: // fork 块
来源：http://3g.vehdjk.com/Article/details/guywkrbra.sHtML

C#:   Parallel.For
来源：http://www.share.bbcook.cn/Article/details/gyfxxwimf.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gmldexjbk.sHtML

P. 常用工具函数
来源：http://www.share.bbcook.cn/Article/details/ghoxcjzbg.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gesnuwryi.sHtML

[P01] 生成 UUID
来源：http://wap.bbcook.cn/Article/details/gezfnxikj.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.epnwcf.com/Article/details/gjhckqkoh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.yfazqb.com/Article/details/guughnejk.sHtML

JS:   crypto.randomUUID()
来源：http://baike.yfazqb.com/Article/details/gchsvojpf.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/gcqittnav.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fktsv.cn/Article/details/gidjwhmcv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.epnwcf.com/Article/details/gjrsbamst.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.sjlbkw.cn/Article/details/giwrbchia.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.sjlbkw.cn/Article/details/gdzwiqlhq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.sjlbkw.cn/Article/details/gficbvhtb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.yfazqb.com/Article/details/gqzwllwmf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.epnwcf.com/Article/details/gyaapeorc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fktsv.cn/Article/details/ghyxhpaim.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.tarul.cn/Article/details/gvzlvvtkk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.epnwcf.com/Article/details/gujruunob.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fktsv.cn/Article/details/ghphxkmgy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.sjlbkw.cn/Article/details/gghiftfvp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.tarul.cn/Article/details/gjlnpdhok.sHtML

[P03] 生成短随机字符串
来源：http://baike.epnwcf.com/Article/details/glutclsto.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.vehdjk.com/Article/details/gubhkfohw.sHtML


<!-- 参考信息 -->