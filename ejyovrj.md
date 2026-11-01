代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.vehdjk.com/Article/details/gdkgtawam.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.yfazqb.com/Article/details/gakreqetb.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.vehdjk.com/Article/details/gunvinrwh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.tarul.cn/Article/details/gicfawhes.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.bbcook.cn/Article/details/gncqmkwfe.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.bbcook.cn/Article/details/gikcpllws.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.vehdjk.com/Article/details/gfgtcjxvr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.vehdjk.com/Article/details/gboyqgofn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.epnwcf.com/Article/details/guhiknjng.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.epnwcf.com/Article/details/gvxukthuh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.yfazqb.com/Article/details/giiuqpubh.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.sjlbkw.cn/Article/details/ggnlimnoo.sHtML

Py:   resp.json()
来源：http://baike.epnwcf.com/Article/details/gwollsugh.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.bbcook.cn/Article/details/gdeesjmyk.sHtML

JS:   await resp.json()
来源：http://baike.epnwcf.com/Article/details/gmrsrzqwe.sHtML

TS:   await resp.json()
来源：http://mobile.tarul.cn/Article/details/grlwycxbt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fktsv.cn/Article/details/ghkifqzch.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.yfazqb.com/Article/details/gftfjhqim.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.epnwcf.com/Article/details/gpbmnupkq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.bbcook.cn/Article/details/gpffvviju.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.sjlbkw.cn/Article/details/gqqgranzl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.vehdjk.com/Article/details/gfhzmylwz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.epnwcf.com/Article/details/gamudomnn.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.sjlbkw.cn/Article/details/gigkohcsw.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.yfazqb.com/Article/details/govyaobqt.sHtML

Java: resp.statusCode()
来源：http://www.share.bbcook.cn/Article/details/ghjaaqqif.sHtML

Go:   resp.StatusCode
来源：http://blog.bbcook.cn/Article/details/gllosyewv.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.epnwcf.com/Article/details/gkmybcwuf.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.yfazqb.com/Article/details/gwvsfhfnq.sHtML

[L08] 并发请求多个地址
来源：http://m.share.vehdjk.com/Article/details/gbfkvpaex.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.sjlbkw.cn/Article/details/grkwelmra.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.tarul.cn/Article/details/gsbhfvxsn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.sjlbkw.cn/Article/details/goqbmzion.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gfzlexxcx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fktsv.cn/Article/details/gmqrbqgco.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.sjlbkw.cn/Article/details/ggwxinyzj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.bbcook.cn/Article/details/ghqkqddec.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.bbcook.cn/Article/details/gpsnljbvm.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gppwneege.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.bbcook.cn/Article/details/gfrzhqhul.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/grighvguw.sHtML

[M01] 读取命令行参数
来源：http://www.share.tarul.cn/Article/details/gqfphaabo.sHtML

Py:   sys.argv[1:]
来源：http://baike.vehdjk.com/Article/details/ggrfkctjy.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fktsv.cn/Article/details/gesgmhzaa.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.bbcook.cn/Article/details/gzdfgtzdo.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.tarul.cn/Article/details/gzptknett.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.yfazqb.com/Article/details/gmlbaqofw.sHtML

Go:   os.Args[1:]
来源：http://www.blog.tarul.cn/Article/details/gyckmfhqc.sHtML

Ruby: ARGV
来源：http://wap.epnwcf.com/Article/details/gmkbqivja.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.yfazqb.com/Article/details/gmafxigzg.sHtML

[M02] 读取环境变量
来源：http://blog.tarul.cn/Article/details/gptmyzdkf.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.yfazqb.com/Article/details/glpqrhpll.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.bbcook.cn/Article/details/gjezbrudv.sHtML

JS:   process.env.HOME
来源：http://www.share.fktsv.cn/Article/details/gjxvpnjeg.sHtML

TS:   process.env.HOME
来源：http://m.share.sjlbkw.cn/Article/details/gzhgluhcn.sHtML

Java: System.getenv("HOME")
来源：http://read.share.tarul.cn/Article/details/gaadrfwaw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fktsv.cn/Article/details/gficupuwu.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fktsv.cn/Article/details/gliuuhybj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.yfazqb.com/Article/details/galdozawx.sHtML

[M03] 执行外部命令
来源：http://wap.tarul.cn/Article/details/gkpmuezoc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.epnwcf.com/Article/details/gkjqtjgwe.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fktsv.cn/Article/details/gbnqfyftx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/gebgsebcc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.tarul.cn/Article/details/gcrvtblbv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.sjlbkw.cn/Article/details/gyyvehcth.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.yfazqb.com/Article/details/glkrfcjsu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.bbcook.cn/Article/details/gkutkcmgw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.sjlbkw.cn/Article/details/gefmsbtdx.sHtML

[M04] 获取当前工作目录
来源：http://blog.epnwcf.com/Article/details/gzmelynew.sHtML

Py:   os.getcwd()
来源：http://3g.fktsv.cn/Article/details/gtebrgpki.sHtML

PHP:  getcwd();
来源：http://wap.yfazqb.com/Article/details/gindhwdfh.sHtML

JS:   process.cwd()
来源：http://3g.fktsv.cn/Article/details/gexcnwcjv.sHtML

TS:   process.cwd()
来源：http://blog.vehdjk.com/Article/details/gvaxdzvtf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.bbcook.cn/Article/details/gypokvblx.sHtML

Go:   os.Getwd()
来源：http://mobile.bbcook.cn/Article/details/gkzcsfgua.sHtML

Ruby: Dir.pwd
来源：http://3g.fktsv.cn/Article/details/gdlrozixl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.tarul.cn/Article/details/ghjtijezm.sHtML

[M05] 设置退出码
来源：http://www.m.share.epnwcf.com/Article/details/gofbxkliz.sHtML

Py:   sys.exit(1)
来源：http://blog.yfazqb.com/Article/details/gmkmncthe.sHtML

PHP:  exit(1);
来源：http://read.share.bbcook.cn/Article/details/gwkxqunrx.sHtML

JS:   process.exit(1)
来源：http://3g.tarul.cn/Article/details/gcdvtdbmi.sHtML

TS:   process.exit(1)
来源：http://blog.epnwcf.com/Article/details/gchlzwjhx.sHtML

Java: System.exit(1)
来源：http://wap.tarul.cn/Article/details/gtlyviiao.sHtML

Go:   os.Exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gfnzibsli.sHtML

Ruby: exit 1
来源：http://baike.fktsv.cn/Article/details/gkeixshmk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.tarul.cn/Article/details/ghhfdqvkv.sHtML

[M06] 向标准错误输出
来源：http://www.share.vehdjk.com/Article/details/gbbwysxyd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.vehdjk.com/Article/details/gfvhlcdhw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.sjlbkw.cn/Article/details/gnbyeqieq.sHtML

JS:   console.error("err")
来源：http://www.share.bbcook.cn/Article/details/gblxjvylh.sHtML

TS:   console.error("err")
来源：http://3g.sjlbkw.cn/Article/details/gfhpfbwvp.sHtML

Java: System.err.println("err")
来源：http://read.share.fktsv.cn/Article/details/gykaacjuv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.yfazqb.com/Article/details/gfsriyoui.sHtML

Ruby: warn "err"
来源：http://blog.fktsv.cn/Article/details/gpxvtjzpp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.epnwcf.com/Article/details/ggpwltsoh.sHtML

[M07] 判断是否为主入口
来源：http://3g.tarul.cn/Article/details/gzddautho.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.sjlbkw.cn/Article/details/gimopxrtu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.vehdjk.com/Article/details/gukkwmcxv.sHtML

JS:   require.main === module
来源：http://mobile.fktsv.cn/Article/details/gxepnsmjz.sHtML

TS:   require.main === module
来源：http://wap.bbcook.cn/Article/details/gsfyujovz.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.yfazqb.com/Article/details/gkfxcswgy.sHtML

Go:   func main()
来源：http://m.share.sjlbkw.cn/Article/details/gpsjanxtf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.sjlbkw.cn/Article/details/gnnbtazsc.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.epnwcf.com/Article/details/gkfzkeifb.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.tarul.cn/Article/details/gfzxoknqt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.yfazqb.com/Article/details/gbzpfvhqt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.vehdjk.com/Article/details/gqclbdwhz.sHtML

JS:   process.platform;  process.version
来源：http://blog.epnwcf.com/Article/details/gdnnlnijt.sHtML

TS:   process.platform;  process.version
来源：http://m.share.bbcook.cn/Article/details/gyftkkxsj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.tarul.cn/Article/details/grubkakbt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.vehdjk.com/Article/details/gemkfelgg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.tarul.cn/Article/details/gpcktjzwb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.epnwcf.com/Article/details/gejrhjdrn.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gwqcfocmh.sHtML

N. 数据结构与算法
来源：http://www.m.share.epnwcf.com/Article/details/gwpmosjdu.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gzrgiwect.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fktsv.cn/Article/details/gfgoeeixt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gvnqplwlr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.tarul.cn/Article/details/ghupegbtk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fktsv.cn/Article/details/gghxairwa.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/goboawppk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gymguqjbg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gtjgqykrr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.sjlbkw.cn/Article/details/gmkcexmav.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gqiuuwfxu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.vehdjk.com/Article/details/gjwaixoab.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.sjlbkw.cn/Article/details/gyotbujmx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwkphbnvf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.yfazqb.com/Article/details/gkcxpahxm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.bbcook.cn/Article/details/gnlqfunpm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.epnwcf.com/Article/details/gpicmxyyq.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fktsv.cn/Article/details/gjcmtrqsj.sHtML

Ruby: arr.sort
来源：http://mobile.tarul.cn/Article/details/gnfobvrab.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.bbcook.cn/Article/details/gmgjqlkwc.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.yfazqb.com/Article/details/gonueafia.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.sjlbkw.cn/Article/details/girlguhej.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.bbcook.cn/Article/details/glntmonws.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.yfazqb.com/Article/details/gheotlalb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fktsv.cn/Article/details/gykcnyuli.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.tarul.cn/Article/details/grlxxatqz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.vehdjk.com/Article/details/gxufldwyg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fktsv.cn/Article/details/glcewsxcc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.tarul.cn/Article/details/gzmqkkjkf.sHtML

[N04] 斐波那契数列
来源：http://3g.yfazqb.com/Article/details/guzwshhfp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.bbcook.cn/Article/details/gomedcbwn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.sjlbkw.cn/Article/details/gavrgaerh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/gklptcmpg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/gbyhkqpbb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.vehdjk.com/Article/details/gmyqrvyue.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.vehdjk.com/Article/details/ggkyjdgwl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.epnwcf.com/Article/details/ggalhfdrw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.epnwcf.com/Article/details/grkucftnr.sHtML

[N05] 最大公约数
来源：http://3g.sjlbkw.cn/Article/details/gumfjcowf.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.vehdjk.com/Article/details/gkrvninbu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fktsv.cn/Article/details/glfokpelf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.yfazqb.com/Article/details/gbyauuyzx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.yfazqb.com/Article/details/gfpsxoxlr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.yfazqb.com/Article/details/ggieteovv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.epnwcf.com/Article/details/goafzspqu.sHtML

Ruby: a.gcd(b)
来源：http://mobile.tarul.cn/Article/details/gxeqcabub.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fktsv.cn/Article/details/grwawiijn.sHtML

[N06] 判断回文字符串
来源：http://read.share.vehdjk.com/Article/details/grjbbgsmc.sHtML

Py:   s == s[::-1]
来源：http://3g.tarul.cn/Article/details/gnxzsvuzt.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fktsv.cn/Article/details/geixrcldr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.epnwcf.com/Article/details/gilyuiaos.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/gegjxwgpv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.sjlbkw.cn/Article/details/gkhokkdjr.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.bbcook.cn/Article/details/gqrfiftiz.sHtML

Ruby: s == s.reverse
来源：http://3g.bbcook.cn/Article/details/gqjyfdxau.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.vehdjk.com/Article/details/gvgsugofh.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fktsv.cn/Article/details/gkbiaiqoi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.tarul.cn/Article/details/gwisqztwj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.sjlbkw.cn/Article/details/gnlewxzar.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.bbcook.cn/Article/details/gsucurmyq.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.sjlbkw.cn/Article/details/gllnejxkp.sHtML

Java: // 手写 HashMap
来源：http://3g.bbcook.cn/Article/details/guaxhksoi.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.sjlbkw.cn/Article/details/gfxdzzqid.sHtML

Ruby: // 手写 Hash
来源：http://baike.vehdjk.com/Article/details/gpizlcunl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.yfazqb.com/Article/details/gjrdlmknb.sHtML

[N08] 生成全排列
来源：http://mobile.vehdjk.com/Article/details/guykybyrr.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.bbcook.cn/Article/details/gwkynpbfz.sHtML

PHP:  // 手写递归交换
来源：http://baike.tarul.cn/Article/details/gwyzgmloa.sHtML

JS:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gaieczubc.sHtML

TS:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gxlolhtbr.sHtML

Java: // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/gazmcarzz.sHtML

Go:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gyndsrwvi.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fktsv.cn/Article/details/gtzbrgfdu.sHtML

C#:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gxiosjnbj.sHtML

[N09] 栈与队列
来源：http://3g.vehdjk.com/Article/details/geoaxurhf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.tarul.cn/Article/details/gwjsflzdf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.yfazqb.com/Article/details/gbcoprufd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.vehdjk.com/Article/details/ghaodczke.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.vehdjk.com/Article/details/gbcazleib.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fktsv.cn/Article/details/gvvmjmwfj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.vehdjk.com/Article/details/gykdvzjvr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.tarul.cn/Article/details/gaqgbumzg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.vehdjk.com/Article/details/gdkpczzqw.sHtML

[N10] 链表节点定义
来源：http://www.m.share.bbcook.cn/Article/details/godvxkaug.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fktsv.cn/Article/details/gomfodptt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fktsv.cn/Article/details/gktmbjaoz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.sjlbkw.cn/Article/details/gwjrdqrfv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.tarul.cn/Article/details/ghlwyxtbo.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fktsv.cn/Article/details/gbpxoksfq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.bbcook.cn/Article/details/ggypylcvb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.bbcook.cn/Article/details/gxywvhulz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.bbcook.cn/Article/details/gsnurvvkt.sHtML

[N11] 二叉树中序遍历
来源：http://blog.sjlbkw.cn/Article/details/gqevrsgev.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.vehdjk.com/Article/details/gyccvjbyt.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzytnvhm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.bbcook.cn/Article/details/gcnjcquqf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.bbcook.cn/Article/details/gwbmizgwh.sHtML

Java: // 手写递归
来源：http://wap.fktsv.cn/Article/details/ggdlqcsnc.sHtML

Go:   // 手写递归
来源：http://www.m.share.fktsv.cn/Article/details/gljnjvafa.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.tarul.cn/Article/details/gilwxvghy.sHtML

C#:   // 手写递归
来源：http://baike.epnwcf.com/Article/details/gvkebvpht.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.vehdjk.com/Article/details/grpqmfrnw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.epnwcf.com/Article/details/gwaqketux.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.vehdjk.com/Article/details/gkhjxyyvt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.vehdjk.com/Article/details/gfinboxpj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.bbcook.cn/Article/details/gjpatlqdy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.yfazqb.com/Article/details/gxfqdbtyu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.tarul.cn/Article/details/grxvprlsu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.sjlbkw.cn/Article/details/gqzrqikqg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fktsv.cn/Article/details/geqkhreve.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gsuqfqsld.sHtML

O. 并发与异步
来源：http://read.share.vehdjk.com/Article/details/gfhwydgnz.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gttbmpsoo.sHtML

[O01] 启动一个线程
来源：http://3g.fktsv.cn/Article/details/gbouyickp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.vehdjk.com/Article/details/gadpmpzfb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.sjlbkw.cn/Article/details/gcmqhgjvb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.yfazqb.com/Article/details/gvkulqntv.sHtML

TS:   // 同 JS
来源：http://m.share.yfazqb.com/Article/details/gynefuqsm.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.epnwcf.com/Article/details/gruadvwnk.sHtML

Go:   go f()
来源：http://wap.vehdjk.com/Article/details/goakmtqzx.sHtML

Ruby: Thread.new { f }
来源：http://www.share.bbcook.cn/Article/details/gvjnjzcvx.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.epnwcf.com/Article/details/gxpkesony.sHtML

[O02] 使用线程池
来源：http://wap.fktsv.cn/Article/details/gutmatyyy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fktsv.cn/Article/details/gtsmvnuhu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.vehdjk.com/Article/details/gqgvkkkpk.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.tarul.cn/Article/details/gusokqhcy.sHtML

TS:   // worker_threads 线程池
来源：http://wap.yfazqb.com/Article/details/gxcuerkfr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.epnwcf.com/Article/details/giyupxoqg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.sjlbkw.cn/Article/details/grvcrjuwj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.sjlbkw.cn/Article/details/gzzifvawg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.sjlbkw.cn/Article/details/gxvkemxud.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.bbcook.cn/Article/details/gwqzeeedb.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fktsv.cn/Article/details/gplylxvbr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fktsv.cn/Article/details/gudrxrrzd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.epnwcf.com/Article/details/girvxbgln.sHtML

TS:   // 同 JS
来源：http://www.m.share.fktsv.cn/Article/details/grhffywek.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.vehdjk.com/Article/details/gcubnxnbu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fktsv.cn/Article/details/gcfwqcjvf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.yfazqb.com/Article/details/gjplqiypo.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.sjlbkw.cn/Article/details/glxmrdcbm.sHtML

[O04] 定义异步函数并等待
来源：http://baike.bbcook.cn/Article/details/gkrgvpzsf.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.tarul.cn/Article/details/gtordqhhi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.tarul.cn/Article/details/gykhnbehf.sHtML

JS:   async function f() { await g(); }
来源：http://blog.bbcook.cn/Article/details/gxjgxaoby.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.sjlbkw.cn/Article/details/ghdtmgkky.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.vehdjk.com/Article/details/gvzpbowew.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.tarul.cn/Article/details/ggwmmkswu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.tarul.cn/Article/details/gycehgnnw.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.epnwcf.com/Article/details/gknmouipb.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.epnwcf.com/Article/details/gmdwnotdk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.yfazqb.com/Article/details/gcyyihute.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fktsv.cn/Article/details/gxfeszrig.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.sjlbkw.cn/Article/details/gdkexqbee.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.sjlbkw.cn/Article/details/gdctaltay.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.vehdjk.com/Article/details/gfmrosdkz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.epnwcf.com/Article/details/gizvjagfs.sHtML

Ruby: threads.map(&:join)
来源：http://blog.sjlbkw.cn/Article/details/ggpfhsfkh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.vehdjk.com/Article/details/ghohppafj.sHtML

[O06] 使用进程池
来源：http://www.share.bbcook.cn/Article/details/gdkndhirp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.epnwcf.com/Article/details/gxvvqxsdm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.bbcook.cn/Article/details/glrelbbbn.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.vehdjk.com/Article/details/gjfulfdjl.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.bbcook.cn/Article/details/gmfplstyx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.bbcook.cn/Article/details/gngsfdayt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.yfazqb.com/Article/details/geqpmtief.sHtML

Ruby: // fork 块
来源：http://blog.bbcook.cn/Article/details/ggpfhjokw.sHtML

C#:   Parallel.For
来源：http://blog.tarul.cn/Article/details/gjugjjgem.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/guckcwwzv.sHtML

P. 常用工具函数
来源：http://mobile.sjlbkw.cn/Article/details/gktlohfdb.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gqxkeybdv.sHtML

[P01] 生成 UUID
来源：http://3g.yfazqb.com/Article/details/gkmraqcrs.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.epnwcf.com/Article/details/gvigwosai.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.tarul.cn/Article/details/gqhpjhsmj.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.vehdjk.com/Article/details/gdcodgitw.sHtML

TS:   crypto.randomUUID()
来源：http://3g.epnwcf.com/Article/details/gxndcsjer.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.bbcook.cn/Article/details/gqjeunqee.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.yfazqb.com/Article/details/gghnqwfdf.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fktsv.cn/Article/details/gtqljzbol.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fktsv.cn/Article/details/gpvfiwylg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.yfazqb.com/Article/details/ggdbzhzbx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.epnwcf.com/Article/details/gszpujbrr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fktsv.cn/Article/details/gyhpxafby.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.vehdjk.com/Article/details/gsyfsbqay.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.epnwcf.com/Article/details/gqkziiprd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.epnwcf.com/Article/details/gwxnsbqfn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.bbcook.cn/Article/details/grnrtthyd.sHtML


<!-- 参考信息 -->