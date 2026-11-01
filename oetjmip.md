代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.epnwcf.com/Article/details/gswwzfory.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.tarul.cn/Article/details/gzhpmtmop.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gjtgyfsns.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqzwwyry.sHtML

Py:   resp.json()
来源：http://blog.epnwcf.com/Article/details/gsxxybsft.sHtML

PHP:  json_decode($body, true);
来源：http://wap.tarul.cn/Article/details/gjjyhpnkj.sHtML

JS:   await resp.json()
来源：http://3g.fktsv.cn/Article/details/gmikqbonh.sHtML

TS:   await resp.json()
来源：http://www.m.share.fktsv.cn/Article/details/godfmzpzc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.tarul.cn/Article/details/ghzbksnuz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.bbcook.cn/Article/details/gtodombqk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.tarul.cn/Article/details/ghqqsoinb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.epnwcf.com/Article/details/gcxciynto.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fktsv.cn/Article/details/gjzdngpmq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.bbcook.cn/Article/details/ghdlzwmal.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.yfazqb.com/Article/details/gikpynfoy.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.sjlbkw.cn/Article/details/gmgaugutz.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.tarul.cn/Article/details/gqpvsgvlu.sHtML

Java: resp.statusCode()
来源：http://read.share.fktsv.cn/Article/details/giftmbvzu.sHtML

Go:   resp.StatusCode
来源：http://mobile.yfazqb.com/Article/details/gqavihnvb.sHtML

Ruby: resp.code.to_i
来源：http://www.share.tarul.cn/Article/details/gsuhocouo.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.epnwcf.com/Article/details/gjyhprhps.sHtML

[L08] 并发请求多个地址
来源：http://3g.sjlbkw.cn/Article/details/glnsjunar.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.vehdjk.com/Article/details/gsowimbla.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.vehdjk.com/Article/details/gvbzypfhn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.tarul.cn/Article/details/gknwcpysx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.tarul.cn/Article/details/gfkrkdmug.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.yfazqb.com/Article/details/gmnrpuezk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.bbcook.cn/Article/details/gokokutyk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.vehdjk.com/Article/details/gbtqgppny.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.tarul.cn/Article/details/gyijaksno.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gwyttwwvd.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.tarul.cn/Article/details/gixgntjlo.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gjsgawseh.sHtML

[M01] 读取命令行参数
来源：http://m.share.sjlbkw.cn/Article/details/gghpckvmd.sHtML

Py:   sys.argv[1:]
来源：http://blog.yfazqb.com/Article/details/gzlxkszcf.sHtML

PHP:  $argv;  $argc;
来源：http://blog.sjlbkw.cn/Article/details/gchlfxhqg.sHtML

JS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/gfwgdxlbf.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fktsv.cn/Article/details/grqrzqyzj.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.vehdjk.com/Article/details/gdgdadjce.sHtML

Go:   os.Args[1:]
来源：http://baike.yfazqb.com/Article/details/gsxvzwzhn.sHtML

Ruby: ARGV
来源：http://mobile.vehdjk.com/Article/details/gyvtqhbos.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.yfazqb.com/Article/details/gcohfnqrd.sHtML

[M02] 读取环境变量
来源：http://blog.tarul.cn/Article/details/gsqpoqohv.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.bbcook.cn/Article/details/gadmgqicg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.epnwcf.com/Article/details/gnqfpcwtj.sHtML

JS:   process.env.HOME
来源：http://www.m.share.tarul.cn/Article/details/gyagszoqz.sHtML

TS:   process.env.HOME
来源：http://www.m.share.epnwcf.com/Article/details/gbwhfuasw.sHtML

Java: System.getenv("HOME")
来源：http://blog.vehdjk.com/Article/details/gqodikksg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.epnwcf.com/Article/details/gjhbdyrwr.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.tarul.cn/Article/details/guhnvtvmq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.vehdjk.com/Article/details/gcwtvinrl.sHtML

[M03] 执行外部命令
来源：http://baike.fktsv.cn/Article/details/gmmsasqld.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.sjlbkw.cn/Article/details/glovrolgf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.vehdjk.com/Article/details/gzfhqpwpp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.bbcook.cn/Article/details/gwxmbytqi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gxzpnoysc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.yfazqb.com/Article/details/gvdhyergg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.tarul.cn/Article/details/gkctcwumr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.tarul.cn/Article/details/genbdnavj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.epnwcf.com/Article/details/gpuddronc.sHtML

[M04] 获取当前工作目录
来源：http://www.share.sjlbkw.cn/Article/details/gtmjbokbk.sHtML

Py:   os.getcwd()
来源：http://mobile.sjlbkw.cn/Article/details/grfvkjhcd.sHtML

PHP:  getcwd();
来源：http://baike.bbcook.cn/Article/details/gjigccojv.sHtML

JS:   process.cwd()
来源：http://www.m.share.tarul.cn/Article/details/glorberzv.sHtML

TS:   process.cwd()
来源：http://www.blog.yfazqb.com/Article/details/gkatamgmj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.tarul.cn/Article/details/gtuzgjmkb.sHtML

Go:   os.Getwd()
来源：http://wap.sjlbkw.cn/Article/details/ggiwptnkv.sHtML

Ruby: Dir.pwd
来源：http://read.share.fktsv.cn/Article/details/gdjyjpgbo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.tarul.cn/Article/details/gphwsdolv.sHtML

[M05] 设置退出码
来源：http://read.share.vehdjk.com/Article/details/gzgjhpgez.sHtML

Py:   sys.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gefsxgvyt.sHtML

PHP:  exit(1);
来源：http://mobile.fktsv.cn/Article/details/gqqiwloas.sHtML

JS:   process.exit(1)
来源：http://read.share.tarul.cn/Article/details/gumaoatmd.sHtML

TS:   process.exit(1)
来源：http://wap.fktsv.cn/Article/details/glfpwwlvi.sHtML

Java: System.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gxgbbtmif.sHtML

Go:   os.Exit(1)
来源：http://3g.tarul.cn/Article/details/gpaofgcav.sHtML

Ruby: exit 1
来源：http://read.share.fktsv.cn/Article/details/ghrydcvwt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fktsv.cn/Article/details/gunyzcurg.sHtML

[M06] 向标准错误输出
来源：http://read.share.sjlbkw.cn/Article/details/gigmxazno.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.vehdjk.com/Article/details/gsssmfjsw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.tarul.cn/Article/details/gowegfikg.sHtML

JS:   console.error("err")
来源：http://read.share.vehdjk.com/Article/details/gfehjovwt.sHtML

TS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/gdabzkxfm.sHtML

Java: System.err.println("err")
来源：http://3g.tarul.cn/Article/details/gurlzxdov.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.vehdjk.com/Article/details/germclqxf.sHtML

Ruby: warn "err"
来源：http://read.share.tarul.cn/Article/details/gwqaassii.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.bbcook.cn/Article/details/gbssmsppv.sHtML

[M07] 判断是否为主入口
来源：http://m.share.bbcook.cn/Article/details/gkxmggsho.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.vehdjk.com/Article/details/gvuhtkgun.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.bbcook.cn/Article/details/gtfdopizb.sHtML

JS:   require.main === module
来源：http://m.share.sjlbkw.cn/Article/details/gqqsnbnhb.sHtML

TS:   require.main === module
来源：http://blog.yfazqb.com/Article/details/gmdnjdybi.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.sjlbkw.cn/Article/details/goswrpztc.sHtML

Go:   func main()
来源：http://baike.fktsv.cn/Article/details/glkxjzxbo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fktsv.cn/Article/details/glbufaley.sHtML

C#:   static void Main(string[] args)
来源：http://blog.yfazqb.com/Article/details/gkpwhxddw.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.tarul.cn/Article/details/grddlhgjv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.tarul.cn/Article/details/gddchlxln.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.bbcook.cn/Article/details/gyzuedemw.sHtML

JS:   process.platform;  process.version
来源：http://wap.epnwcf.com/Article/details/ggpdixluf.sHtML

TS:   process.platform;  process.version
来源：http://blog.sjlbkw.cn/Article/details/gmdnpjyzf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.epnwcf.com/Article/details/gugdxyxup.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.epnwcf.com/Article/details/gqwhmyjuy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.vehdjk.com/Article/details/gtwgcxfnt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.tarul.cn/Article/details/gendfijoe.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gwohqyxxq.sHtML

N. 数据结构与算法
来源：http://wap.bbcook.cn/Article/details/gxqkxuoys.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gtdeczsly.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.vehdjk.com/Article/details/gexcilqnn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/grcryqqpq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.vehdjk.com/Article/details/gwjpivwpq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fktsv.cn/Article/details/geijlibyt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.vehdjk.com/Article/details/gfbivjcqr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gtsnpamjv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.bbcook.cn/Article/details/gnvjbryrb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.yfazqb.com/Article/details/ggkjlfeil.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gtwkcprcp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.yfazqb.com/Article/details/geeebuskg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.bbcook.cn/Article/details/gjnweupnl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.epnwcf.com/Article/details/gphdgffkd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gtqmuxptt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fktsv.cn/Article/details/gmcsjitgq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.vehdjk.com/Article/details/gkvmhrcpc.sHtML

Go:   slices.Sort(arr)
来源：http://blog.vehdjk.com/Article/details/gflblatza.sHtML

Ruby: arr.sort
来源：http://m.share.bbcook.cn/Article/details/gvyysgzkb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.sjlbkw.cn/Article/details/goakepdpj.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.bbcook.cn/Article/details/gmaoneiqa.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.epnwcf.com/Article/details/gnymeegza.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fktsv.cn/Article/details/gvffwucat.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.yfazqb.com/Article/details/ggpdmomsr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.vehdjk.com/Article/details/gviloojre.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.sjlbkw.cn/Article/details/gunnuzyhg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.sjlbkw.cn/Article/details/gvwjylyrs.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.tarul.cn/Article/details/gmamjghhq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.yfazqb.com/Article/details/gblazywxw.sHtML

[N04] 斐波那契数列
来源：http://3g.tarul.cn/Article/details/govdjujdh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.bbcook.cn/Article/details/gqocgeysb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fktsv.cn/Article/details/ggxkkmpod.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/gdxhmygqs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.sjlbkw.cn/Article/details/glbegtcyq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fktsv.cn/Article/details/gubybvkue.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.sjlbkw.cn/Article/details/gvyvusvyj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.vehdjk.com/Article/details/gsoxrknzw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/gtiazxjrq.sHtML

[N05] 最大公约数
来源：http://baike.epnwcf.com/Article/details/gafpdlzce.sHtML

Py:   math.gcd(a, b)
来源：http://blog.vehdjk.com/Article/details/gkiqtsopi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.tarul.cn/Article/details/ggkeebtui.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.sjlbkw.cn/Article/details/gkxchblcw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.tarul.cn/Article/details/goorwulgp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.bbcook.cn/Article/details/gpxdlxdsv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.tarul.cn/Article/details/gciqxckyg.sHtML

Ruby: a.gcd(b)
来源：http://blog.fktsv.cn/Article/details/gycmjudzg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.yfazqb.com/Article/details/gifowyrhc.sHtML

[N06] 判断回文字符串
来源：http://mobile.vehdjk.com/Article/details/gvrkyvntw.sHtML

Py:   s == s[::-1]
来源：http://blog.epnwcf.com/Article/details/gybvfqajo.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.bbcook.cn/Article/details/gzfmzbszb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/gtveiawmn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/gtbukknjo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.sjlbkw.cn/Article/details/gaukzbjiz.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.bbcook.cn/Article/details/ggtkiokpn.sHtML

Ruby: s == s.reverse
来源：http://wap.bbcook.cn/Article/details/gckftezyo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.sjlbkw.cn/Article/details/gudozqkgr.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.bbcook.cn/Article/details/gbeiaivfd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.vehdjk.com/Article/details/gluqiirpg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.yfazqb.com/Article/details/guqqpfhzw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.tarul.cn/Article/details/gqscqqyoq.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.vehdjk.com/Article/details/grjxfohhn.sHtML

Java: // 手写 HashMap
来源：http://www.blog.sjlbkw.cn/Article/details/gxgaaufjf.sHtML

Go:   // 手写 map[int]int
来源：http://baike.tarul.cn/Article/details/goyvbbetl.sHtML

Ruby: // 手写 Hash
来源：http://blog.bbcook.cn/Article/details/gngddzlgv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.yfazqb.com/Article/details/gjksthlhs.sHtML

[N08] 生成全排列
来源：http://www.share.epnwcf.com/Article/details/geqntgyrr.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.epnwcf.com/Article/details/gyguxzxun.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.vehdjk.com/Article/details/gpxeputfn.sHtML

JS:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gyfjafprg.sHtML

TS:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/geaybwrfa.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/guxjppflj.sHtML

Go:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gutyseywg.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.epnwcf.com/Article/details/gjdafowwr.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gfyurnxpu.sHtML

[N09] 栈与队列
来源：http://baike.yfazqb.com/Article/details/gixetzvuh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpamsrhr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fktsv.cn/Article/details/gckpkpfrz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.vehdjk.com/Article/details/gobxtnkoq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.tarul.cn/Article/details/gtjzzsdks.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.epnwcf.com/Article/details/gmjoimues.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.bbcook.cn/Article/details/geeqpbdgb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/gunpxjoma.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.epnwcf.com/Article/details/gtkefvuum.sHtML

[N10] 链表节点定义
来源：http://baike.bbcook.cn/Article/details/gfizgfklw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.epnwcf.com/Article/details/gxobbhczz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.epnwcf.com/Article/details/gbvodiayc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.sjlbkw.cn/Article/details/gdksyknee.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.yfazqb.com/Article/details/gqhehhkhm.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.epnwcf.com/Article/details/ggrxqnwee.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.epnwcf.com/Article/details/gvmqznvcv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.vehdjk.com/Article/details/gkptquutg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.yfazqb.com/Article/details/gupoafgmd.sHtML

[N11] 二叉树中序遍历
来源：http://baike.bbcook.cn/Article/details/gunnfxeom.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.yfazqb.com/Article/details/gvcljkxnn.sHtML

PHP:  // 手写递归函数
来源：http://baike.bbcook.cn/Article/details/gpfvattcn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.tarul.cn/Article/details/gzxminfxa.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.vehdjk.com/Article/details/geavejgub.sHtML

Java: // 手写递归
来源：http://3g.yfazqb.com/Article/details/giqdtpxmg.sHtML

Go:   // 手写递归
来源：http://baike.epnwcf.com/Article/details/guggmszen.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.bbcook.cn/Article/details/gatwekcms.sHtML

C#:   // 手写递归
来源：http://3g.vehdjk.com/Article/details/ghkcgzcyu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.tarul.cn/Article/details/gpnlxkywr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.bbcook.cn/Article/details/gfcmtpcfc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.bbcook.cn/Article/details/gfnjdyvlv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.epnwcf.com/Article/details/gcwiafatn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.bbcook.cn/Article/details/gtixxsdza.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.bbcook.cn/Article/details/gsbyrvvrw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.vehdjk.com/Article/details/gnmmfoudl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.sjlbkw.cn/Article/details/gocvblbzc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.tarul.cn/Article/details/goksttmic.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gpupfwbrg.sHtML

O. 并发与异步
来源：http://www.m.share.tarul.cn/Article/details/glykgguij.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gcnsrbtoa.sHtML

[O01] 启动一个线程
来源：http://read.share.epnwcf.com/Article/details/gspjhyoyu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.sjlbkw.cn/Article/details/gdaxcjfgy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.bbcook.cn/Article/details/gmzympvnz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.bbcook.cn/Article/details/gmnlrdexa.sHtML

TS:   // 同 JS
来源：http://3g.epnwcf.com/Article/details/gcknxknlc.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fktsv.cn/Article/details/gmmjgowwz.sHtML

Go:   go f()
来源：http://www.blog.fktsv.cn/Article/details/gncueyrao.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fktsv.cn/Article/details/gvbifxtqi.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.sjlbkw.cn/Article/details/gxdgsrowg.sHtML

[O02] 使用线程池
来源：http://blog.tarul.cn/Article/details/gxqwyjqhu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fktsv.cn/Article/details/ggwhnwvss.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.vehdjk.com/Article/details/geyllyvlk.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fktsv.cn/Article/details/gqyhbbept.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.yfazqb.com/Article/details/gsmybrpzq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.yfazqb.com/Article/details/gbpajttmr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.tarul.cn/Article/details/gfmqwswnz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fktsv.cn/Article/details/gnzuffmsq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.epnwcf.com/Article/details/gqrhkdvqj.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.yfazqb.com/Article/details/glvkalubu.sHtML

Py:   with lock: shared += 1
来源：http://www.share.tarul.cn/Article/details/gjvmsumpg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.sjlbkw.cn/Article/details/gejccdesq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.yfazqb.com/Article/details/gsgxqdbql.sHtML

TS:   // 同 JS
来源：http://mobile.yfazqb.com/Article/details/gsijtexwx.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.epnwcf.com/Article/details/gswfditzn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.epnwcf.com/Article/details/gsslqruuc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbzzajdpw.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fktsv.cn/Article/details/gsavilfmh.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.bbcook.cn/Article/details/gychnlxfu.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fktsv.cn/Article/details/gzzeydris.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.tarul.cn/Article/details/gkhzubpgh.sHtML

JS:   async function f() { await g(); }
来源：http://blog.yfazqb.com/Article/details/ghreafirg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.vehdjk.com/Article/details/gopemunzy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.vehdjk.com/Article/details/gjehbykch.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fktsv.cn/Article/details/gyswegryx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fktsv.cn/Article/details/ginsspojg.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.yfazqb.com/Article/details/gdvfhbjyq.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.vehdjk.com/Article/details/ghrlykjas.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fktsv.cn/Article/details/gbssnkxzj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.sjlbkw.cn/Article/details/gqmnosqcy.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.epnwcf.com/Article/details/gvdrepdzb.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.tarul.cn/Article/details/guqluqjfq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.sjlbkw.cn/Article/details/glssmymfz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.tarul.cn/Article/details/gtbweurzs.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.epnwcf.com/Article/details/ghmbfuflw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fktsv.cn/Article/details/gvhjztumt.sHtML

[O06] 使用进程池
来源：http://m.share.epnwcf.com/Article/details/grifldhfv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.bbcook.cn/Article/details/gbjgjjidy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.bbcook.cn/Article/details/gcmgitdtv.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fktsv.cn/Article/details/gpqcuuama.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.tarul.cn/Article/details/gytuszpsw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.tarul.cn/Article/details/gnbouuwmo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.vehdjk.com/Article/details/gvjrjjizu.sHtML

Ruby: // fork 块
来源：http://www.m.share.epnwcf.com/Article/details/gwcfsukir.sHtML

C#:   Parallel.For
来源：http://blog.bbcook.cn/Article/details/gwzwdhhha.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gxilsldzm.sHtML

P. 常用工具函数
来源：http://www.blog.bbcook.cn/Article/details/gflpmqwko.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/grzowhjmb.sHtML

[P01] 生成 UUID
来源：http://wap.fktsv.cn/Article/details/giwvlmynr.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.sjlbkw.cn/Article/details/gqlegjhbg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.yfazqb.com/Article/details/gcxyhhzig.sHtML

JS:   crypto.randomUUID()
来源：http://baike.epnwcf.com/Article/details/glmmkuppn.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/gnouymkjc.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gchrlzsww.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.sjlbkw.cn/Article/details/gigyxzskx.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.epnwcf.com/Article/details/gssvidlxy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fktsv.cn/Article/details/grmcjcqcj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.vehdjk.com/Article/details/goyancanx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.sjlbkw.cn/Article/details/gpclutqye.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.epnwcf.com/Article/details/gxdtejham.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.bbcook.cn/Article/details/gsukilzho.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.yfazqb.com/Article/details/gtyddtxud.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.yfazqb.com/Article/details/gxitcdtjs.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.epnwcf.com/Article/details/gajeexdio.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.bbcook.cn/Article/details/gjqibjqho.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.vehdjk.com/Article/details/gnjbtcoay.sHtML

[P03] 生成短随机字符串
来源：http://blog.vehdjk.com/Article/details/gdbdbtbap.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.sjlbkw.cn/Article/details/ggibodvca.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.epnwcf.com/Article/details/gmmtwvnjp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.sjlbkw.cn/Article/details/gspdfwond.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.yfazqb.com/Article/details/gflnkfenx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.epnwcf.com/Article/details/gaqmartwu.sHtML


<!-- 参考信息 -->