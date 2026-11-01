代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.sjlbkw.cn/Article/details/gprkdhrfw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.epnwcf.com/Article/details/grnbvzwou.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.vehdjk.com/Article/details/giohfhtiu.sHtML

[L06] 解析响应为 JSON
来源：http://3g.epnwcf.com/Article/details/gwbdsdhcw.sHtML

Py:   resp.json()
来源：http://www.m.share.tarul.cn/Article/details/gdiofblyp.sHtML

PHP:  json_decode($body, true);
来源：http://baike.bbcook.cn/Article/details/gsyeybajp.sHtML

JS:   await resp.json()
来源：http://blog.sjlbkw.cn/Article/details/guvmkzpoc.sHtML

TS:   await resp.json()
来源：http://baike.fktsv.cn/Article/details/gjacniniv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.sjlbkw.cn/Article/details/gmrrtmntq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.epnwcf.com/Article/details/gjmmtuqxi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.yfazqb.com/Article/details/gzsqmphys.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.tarul.cn/Article/details/gogxbczvx.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.yfazqb.com/Article/details/gdosjiwqb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.epnwcf.com/Article/details/gwygbbvzc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fktsv.cn/Article/details/gxbblbror.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.vehdjk.com/Article/details/gqihvjppy.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.tarul.cn/Article/details/gbgxxnxjt.sHtML

Java: resp.statusCode()
来源：http://read.share.fktsv.cn/Article/details/gepfkvejl.sHtML

Go:   resp.StatusCode
来源：http://blog.yfazqb.com/Article/details/ghxsnbaph.sHtML

Ruby: resp.code.to_i
来源：http://baike.epnwcf.com/Article/details/gsikodogb.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.yfazqb.com/Article/details/gqhwvthid.sHtML

[L08] 并发请求多个地址
来源：http://wap.vehdjk.com/Article/details/ghouyrudb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.epnwcf.com/Article/details/gvankwerq.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.epnwcf.com/Article/details/gtfwglslq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/gocfuxjhe.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpbtoecd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.sjlbkw.cn/Article/details/gjhnzrzan.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.tarul.cn/Article/details/gpabomunz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fktsv.cn/Article/details/gwszfbnuk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.bbcook.cn/Article/details/gbzflpidq.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/giileuokk.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.vehdjk.com/Article/details/gbzbezigw.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gyuqxgbao.sHtML

[M01] 读取命令行参数
来源：http://wap.tarul.cn/Article/details/gkriatjyw.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.tarul.cn/Article/details/gkjrwmvnc.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.epnwcf.com/Article/details/gwftqqzjv.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fktsv.cn/Article/details/gztlamrtr.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.vehdjk.com/Article/details/ghrlycamx.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.sjlbkw.cn/Article/details/gjbjsefwj.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gbpkfqpci.sHtML

Ruby: ARGV
来源：http://m.share.bbcook.cn/Article/details/gyybrkzwi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.bbcook.cn/Article/details/gysunkzpu.sHtML

[M02] 读取环境变量
来源：http://mobile.epnwcf.com/Article/details/glhovfmeo.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.yfazqb.com/Article/details/guthlxmjp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.yfazqb.com/Article/details/gpwkhtkhj.sHtML

JS:   process.env.HOME
来源：http://m.share.bbcook.cn/Article/details/gppunuceo.sHtML

TS:   process.env.HOME
来源：http://www.share.vehdjk.com/Article/details/gvzvdmsic.sHtML

Java: System.getenv("HOME")
来源：http://wap.fktsv.cn/Article/details/gskvdtiue.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.tarul.cn/Article/details/grsdlpamz.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.bbcook.cn/Article/details/gpiyzwesz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.epnwcf.com/Article/details/genfwwnbi.sHtML

[M03] 执行外部命令
来源：http://wap.sjlbkw.cn/Article/details/gaxmcvshx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fktsv.cn/Article/details/gasvhlcnc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.yfazqb.com/Article/details/gbnsvfmwf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.sjlbkw.cn/Article/details/gtmyjegrd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fktsv.cn/Article/details/gjbiqlksv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.sjlbkw.cn/Article/details/gcbgpltdp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.sjlbkw.cn/Article/details/gqggfvpem.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.tarul.cn/Article/details/gjppnahje.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.epnwcf.com/Article/details/gwxvmqmpx.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fktsv.cn/Article/details/ghcutbvbr.sHtML

Py:   os.getcwd()
来源：http://read.share.tarul.cn/Article/details/gwfstoytd.sHtML

PHP:  getcwd();
来源：http://mobile.vehdjk.com/Article/details/gylwjqxbj.sHtML

JS:   process.cwd()
来源：http://3g.epnwcf.com/Article/details/gloptffwn.sHtML

TS:   process.cwd()
来源：http://3g.vehdjk.com/Article/details/gfdkhgaew.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.bbcook.cn/Article/details/gcrlnskgp.sHtML

Go:   os.Getwd()
来源：http://blog.yfazqb.com/Article/details/gwrluzuml.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fktsv.cn/Article/details/gcxakfdki.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.bbcook.cn/Article/details/ghhgqurkj.sHtML

[M05] 设置退出码
来源：http://www.share.yfazqb.com/Article/details/glumnympz.sHtML

Py:   sys.exit(1)
来源：http://mobile.epnwcf.com/Article/details/ghonqgkzh.sHtML

PHP:  exit(1);
来源：http://www.blog.bbcook.cn/Article/details/gqcqeibnu.sHtML

JS:   process.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/goiqdzika.sHtML

TS:   process.exit(1)
来源：http://wap.yfazqb.com/Article/details/gyezmgrol.sHtML

Java: System.exit(1)
来源：http://baike.yfazqb.com/Article/details/glaczlouo.sHtML

Go:   os.Exit(1)
来源：http://3g.bbcook.cn/Article/details/gzkiobmkv.sHtML

Ruby: exit 1
来源：http://baike.tarul.cn/Article/details/ghapquavt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.tarul.cn/Article/details/gddfivjrd.sHtML

[M06] 向标准错误输出
来源：http://www.share.tarul.cn/Article/details/gjrcmghda.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.yfazqb.com/Article/details/gpvpowewb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.vehdjk.com/Article/details/gezfgxlzx.sHtML

JS:   console.error("err")
来源：http://m.share.vehdjk.com/Article/details/gyjscocgn.sHtML

TS:   console.error("err")
来源：http://3g.epnwcf.com/Article/details/gqjclbtov.sHtML

Java: System.err.println("err")
来源：http://wap.fktsv.cn/Article/details/gugwihrxk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.vehdjk.com/Article/details/ghlbjvphn.sHtML

Ruby: warn "err"
来源：http://3g.fktsv.cn/Article/details/gssapezmw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fktsv.cn/Article/details/gzjetxhmx.sHtML

[M07] 判断是否为主入口
来源：http://m.share.tarul.cn/Article/details/girmqzwha.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fktsv.cn/Article/details/gfkovnmad.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.tarul.cn/Article/details/gkmfpxgyd.sHtML

JS:   require.main === module
来源：http://www.share.bbcook.cn/Article/details/gnhhwqeqw.sHtML

TS:   require.main === module
来源：http://wap.vehdjk.com/Article/details/glgksuhwe.sHtML

Java: public static void main(String[] args)
来源：http://3g.yfazqb.com/Article/details/gmukgntgy.sHtML

Go:   func main()
来源：http://mobile.bbcook.cn/Article/details/gmuowevvd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.tarul.cn/Article/details/giphfjlab.sHtML

C#:   static void Main(string[] args)
来源：http://baike.epnwcf.com/Article/details/gyexkycrs.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.tarul.cn/Article/details/govelfrdm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.vehdjk.com/Article/details/ganwgddgn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.bbcook.cn/Article/details/gxhqpcfrv.sHtML

JS:   process.platform;  process.version
来源：http://read.share.vehdjk.com/Article/details/gorcifvce.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.tarul.cn/Article/details/glbyrsohd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.sjlbkw.cn/Article/details/gkedqmeae.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.vehdjk.com/Article/details/gbicukhjp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fktsv.cn/Article/details/gfuamqvxk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fktsv.cn/Article/details/gkkzuckty.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/guvltxcli.sHtML

N. 数据结构与算法
来源：http://m.share.yfazqb.com/Article/details/gkuzxdyeq.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gjtuiewej.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.yfazqb.com/Article/details/gwlwqztys.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.tarul.cn/Article/details/gslczgpoj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.yfazqb.com/Article/details/gmegbsqtn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.epnwcf.com/Article/details/giyqtpegm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.bbcook.cn/Article/details/gxrtwjahl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.vehdjk.com/Article/details/ghnvhhqzk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.epnwcf.com/Article/details/gxwmnjfzj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.epnwcf.com/Article/details/glokiyhjk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fktsv.cn/Article/details/gmpcqvlnt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.vehdjk.com/Article/details/gkxwrvhvz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fktsv.cn/Article/details/gilbvjkrv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.vehdjk.com/Article/details/giedbgqoc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.sjlbkw.cn/Article/details/gjboasqmp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fktsv.cn/Article/details/glsexasbm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.sjlbkw.cn/Article/details/gpznkuvtv.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fktsv.cn/Article/details/gollhxeng.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/gycclopre.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.tarul.cn/Article/details/gzisafcdb.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.tarul.cn/Article/details/gfprdcyxj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.sjlbkw.cn/Article/details/gunqitoxw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fktsv.cn/Article/details/ggbfuvrqf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.vehdjk.com/Article/details/gedhmgryy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.vehdjk.com/Article/details/gyainqwcc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.sjlbkw.cn/Article/details/gplfmuhni.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.vehdjk.com/Article/details/grhffkobp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.sjlbkw.cn/Article/details/gnctjsecv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.bbcook.cn/Article/details/gwqdtqjdz.sHtML

[N04] 斐波那契数列
来源：http://m.share.fktsv.cn/Article/details/gevrzishb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.sjlbkw.cn/Article/details/geyhqcgsa.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.yfazqb.com/Article/details/gvlmkcipq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/gwrkqbxbr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gtenxywdp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.yfazqb.com/Article/details/gfjnqhots.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.tarul.cn/Article/details/gigvvfcdo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fktsv.cn/Article/details/gsqaluedn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/gkkfrsiyk.sHtML

[N05] 最大公约数
来源：http://blog.fktsv.cn/Article/details/gkxmtrzod.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fktsv.cn/Article/details/gtoxwqiaq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.sjlbkw.cn/Article/details/guxoxgxwj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.yfazqb.com/Article/details/gazgtrxxn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.yfazqb.com/Article/details/gnnrssljg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fktsv.cn/Article/details/gwneysiio.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.vehdjk.com/Article/details/gwfbdavln.sHtML

Ruby: a.gcd(b)
来源：http://3g.bbcook.cn/Article/details/gaigzxyvf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.bbcook.cn/Article/details/gupncdyhq.sHtML

[N06] 判断回文字符串
来源：http://read.share.fktsv.cn/Article/details/gvfhqzzbx.sHtML

Py:   s == s[::-1]
来源：http://blog.sjlbkw.cn/Article/details/gshvdwjpm.sHtML

PHP:  $s === strrev($s);
来源：http://3g.sjlbkw.cn/Article/details/ggvvieaum.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gyziilayu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/gbnviqhrs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.vehdjk.com/Article/details/gojzksihe.sHtML

Go:   // 双指针从两端比较
来源：http://3g.vehdjk.com/Article/details/gabsnlgvp.sHtML

Ruby: s == s.reverse
来源：http://m.share.fktsv.cn/Article/details/gyxszqwzs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.tarul.cn/Article/details/gjdiqetew.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.yfazqb.com/Article/details/givtewior.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.bbcook.cn/Article/details/gbwfixdvn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.bbcook.cn/Article/details/gaisxkyis.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.bbcook.cn/Article/details/gcfehfbxz.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.yfazqb.com/Article/details/gjzszbhut.sHtML

Java: // 手写 HashMap
来源：http://mobile.epnwcf.com/Article/details/gcjahdziy.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.yfazqb.com/Article/details/gdshnagfk.sHtML

Ruby: // 手写 Hash
来源：http://m.share.sjlbkw.cn/Article/details/gagwhiqwe.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.sjlbkw.cn/Article/details/gbssnbtgi.sHtML

[N08] 生成全排列
来源：http://www.m.share.sjlbkw.cn/Article/details/gbpkjgdci.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.sjlbkw.cn/Article/details/gdrmjkwof.sHtML

PHP:  // 手写递归交换
来源：http://read.share.sjlbkw.cn/Article/details/giwwthidm.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gmczxxcyq.sHtML

TS:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gciwokfdr.sHtML

Java: // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gobfdziwg.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gasxeenox.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.vehdjk.com/Article/details/gydbccssk.sHtML

C#:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/guuolkzuz.sHtML

[N09] 栈与队列
来源：http://3g.fktsv.cn/Article/details/gmrjgbxwe.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gwrkzhrtt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.sjlbkw.cn/Article/details/gbiismzog.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gfsgveopo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.vehdjk.com/Article/details/gsugzoqja.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.vehdjk.com/Article/details/gnyzvjtqz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.tarul.cn/Article/details/gecqjeesd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gbqrorpmn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.vehdjk.com/Article/details/gxjezgywg.sHtML

[N10] 链表节点定义
来源：http://wap.tarul.cn/Article/details/gftrapznn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.sjlbkw.cn/Article/details/gndbnogpi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.vehdjk.com/Article/details/ggydyapdq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.epnwcf.com/Article/details/gjipbckil.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fktsv.cn/Article/details/gnkpcsxcr.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fktsv.cn/Article/details/gfepwrbmk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.vehdjk.com/Article/details/gtvcfbmpq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.yfazqb.com/Article/details/grymtadef.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.yfazqb.com/Article/details/gomyrhjdc.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.tarul.cn/Article/details/gcoqufxhk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxpetaky.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.epnwcf.com/Article/details/ggvtohlxk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fktsv.cn/Article/details/gxxkrbflr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.bbcook.cn/Article/details/gleiqmarc.sHtML

Java: // 手写递归
来源：http://www.share.epnwcf.com/Article/details/gpmebxrod.sHtML

Go:   // 手写递归
来源：http://wap.vehdjk.com/Article/details/gzebnkgrh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.sjlbkw.cn/Article/details/ghoxshyvg.sHtML

C#:   // 手写递归
来源：http://read.share.tarul.cn/Article/details/gztpuxiad.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.epnwcf.com/Article/details/gurzjzxbj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.bbcook.cn/Article/details/gkyjcjuyc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.tarul.cn/Article/details/gpqbqnjfr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.sjlbkw.cn/Article/details/gejdhirtq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fktsv.cn/Article/details/gjkprhozw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.vehdjk.com/Article/details/gpjtwmbci.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.epnwcf.com/Article/details/gnpfgdpqi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.vehdjk.com/Article/details/gquawgkej.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.yfazqb.com/Article/details/gzbwaedmh.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gpjiagdty.sHtML

O. 并发与异步
来源：http://mobile.yfazqb.com/Article/details/gxgjcvxwz.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gqoelgmgr.sHtML

[O01] 启动一个线程
来源：http://blog.yfazqb.com/Article/details/gifcxdxww.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.epnwcf.com/Article/details/glzvztwao.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fktsv.cn/Article/details/gmxjogyhl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.sjlbkw.cn/Article/details/gtzzaikyr.sHtML

TS:   // 同 JS
来源：http://m.share.sjlbkw.cn/Article/details/gomyemyla.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fktsv.cn/Article/details/guxcwojid.sHtML

Go:   go f()
来源：http://mobile.tarul.cn/Article/details/gktudwurb.sHtML

Ruby: Thread.new { f }
来源：http://blog.tarul.cn/Article/details/gcjgsjael.sHtML

C#:   Task.Run(() => F());
来源：http://baike.yfazqb.com/Article/details/gzyfvqcsh.sHtML

[O02] 使用线程池
来源：http://blog.vehdjk.com/Article/details/ghfqwrxsb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fktsv.cn/Article/details/gslmoivnh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.sjlbkw.cn/Article/details/gnagujcrd.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.epnwcf.com/Article/details/gregvsqsc.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.vehdjk.com/Article/details/gtnewyrvp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.epnwcf.com/Article/details/giufsdjwf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.vehdjk.com/Article/details/golpfrjvj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.epnwcf.com/Article/details/gmigckwwq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.bbcook.cn/Article/details/grgklqwsn.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.epnwcf.com/Article/details/gybemourl.sHtML

Py:   with lock: shared += 1
来源：http://m.share.yfazqb.com/Article/details/gnsadaylz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.tarul.cn/Article/details/gfamwjyha.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.epnwcf.com/Article/details/gygzbayoo.sHtML

TS:   // 同 JS
来源：http://www.m.share.bbcook.cn/Article/details/gpggvbhgt.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.tarul.cn/Article/details/gzvwuwaai.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.tarul.cn/Article/details/gifqjozyr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.yfazqb.com/Article/details/gwktfdzgo.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.yfazqb.com/Article/details/ggjhcscpd.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.yfazqb.com/Article/details/gamryajho.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.yfazqb.com/Article/details/gwxgnxrhh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.yfazqb.com/Article/details/gqjgvrige.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.sjlbkw.cn/Article/details/gewqcbwqq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.vehdjk.com/Article/details/gkuodrrnn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.sjlbkw.cn/Article/details/gdqugpaes.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.sjlbkw.cn/Article/details/gnndnrkol.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.yfazqb.com/Article/details/gwqodnqlg.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.yfazqb.com/Article/details/gyiytyzmm.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.vehdjk.com/Article/details/gfnvzehfo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.tarul.cn/Article/details/gcsepidts.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.yfazqb.com/Article/details/gfbgnkexo.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.tarul.cn/Article/details/gxdqevnop.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fktsv.cn/Article/details/ghthwkdlh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.tarul.cn/Article/details/gkomsmsmf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.yfazqb.com/Article/details/gtwgafdew.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.tarul.cn/Article/details/ghyctufjv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.vehdjk.com/Article/details/gdrdhvgxm.sHtML

[O06] 使用进程池
来源：http://baike.fktsv.cn/Article/details/gtwevkcll.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.tarul.cn/Article/details/gewxaoxos.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.bbcook.cn/Article/details/giwahkjmk.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fktsv.cn/Article/details/gxuppovrk.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.tarul.cn/Article/details/gdmfadbrv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.epnwcf.com/Article/details/gwjotqzwe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fktsv.cn/Article/details/gzztjkqej.sHtML

Ruby: // fork 块
来源：http://baike.fktsv.cn/Article/details/gxxcggiru.sHtML

C#:   Parallel.For
来源：http://baike.epnwcf.com/Article/details/gdocvdmts.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gofcnmsyz.sHtML

P. 常用工具函数
来源：http://www.m.share.sjlbkw.cn/Article/details/ghphbhbod.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gkjjisstq.sHtML

[P01] 生成 UUID
来源：http://www.blog.tarul.cn/Article/details/gevosgvqk.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.epnwcf.com/Article/details/gjsxuyjkh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fktsv.cn/Article/details/gxvopoqtr.sHtML

JS:   crypto.randomUUID()
来源：http://blog.sjlbkw.cn/Article/details/gnwwgzaju.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.sjlbkw.cn/Article/details/glnkjjoyy.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fktsv.cn/Article/details/gdwyywhol.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.yfazqb.com/Article/details/gafufgpxg.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fktsv.cn/Article/details/gfezwfuga.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.epnwcf.com/Article/details/gwapmpzlz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.vehdjk.com/Article/details/gwqlmbzoa.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fktsv.cn/Article/details/grunlvuiq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.sjlbkw.cn/Article/details/gzmrtxfxw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.sjlbkw.cn/Article/details/gtabzvdqs.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.vehdjk.com/Article/details/gwtyokice.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.epnwcf.com/Article/details/gnbwwzhhg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.tarul.cn/Article/details/gddchmuun.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.vehdjk.com/Article/details/gzojvmndi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.yfazqb.com/Article/details/glzewqvpi.sHtML

[P03] 生成短随机字符串
来源：http://read.share.bbcook.cn/Article/details/gwqcrtlwl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fktsv.cn/Article/details/ghppyrdze.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.epnwcf.com/Article/details/gkzzptulk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fktsv.cn/Article/details/gprkfiase.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fktsv.cn/Article/details/glmsydmpd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.bbcook.cn/Article/details/gygzndkqe.sHtML


<!-- 参考信息 -->