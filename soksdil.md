代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.epnwcf.com/Article/details/gpgvdqkut.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.vehdjk.com/Article/details/gnbbxsrnr.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fktsv.cn/Article/details/gjyuyfybc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fktsv.cn/Article/details/gmwxsxuyu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.sjlbkw.cn/Article/details/gmadwnenj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.yfazqb.com/Article/details/gzakiekhi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.tarul.cn/Article/details/ggxfsklky.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.sjlbkw.cn/Article/details/gjtlzswzh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.yfazqb.com/Article/details/gfphqrdql.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.yfazqb.com/Article/details/gevkiizlw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.vehdjk.com/Article/details/gmiipsdvt.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.yfazqb.com/Article/details/ghprxuiir.sHtML

Py:   resp.json()
来源：http://www.blog.epnwcf.com/Article/details/gtcajyhlp.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.epnwcf.com/Article/details/gbhqhtehr.sHtML

JS:   await resp.json()
来源：http://www.m.share.sjlbkw.cn/Article/details/gkwjjskab.sHtML

TS:   await resp.json()
来源：http://mobile.epnwcf.com/Article/details/gqoocdbqg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.yfazqb.com/Article/details/grfsaqjxx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.sjlbkw.cn/Article/details/grmpmrufy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.bbcook.cn/Article/details/grcsvbskq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.yfazqb.com/Article/details/gqhzcsrjf.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.yfazqb.com/Article/details/grtcvbjjl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.sjlbkw.cn/Article/details/gztsmtqlx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.epnwcf.com/Article/details/gkyqsvxil.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fktsv.cn/Article/details/ghwudbatk.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.tarul.cn/Article/details/gzdygacgk.sHtML

Java: resp.statusCode()
来源：http://wap.bbcook.cn/Article/details/gjbkbcmiy.sHtML

Go:   resp.StatusCode
来源：http://baike.tarul.cn/Article/details/ghjmmvyou.sHtML

Ruby: resp.code.to_i
来源：http://3g.tarul.cn/Article/details/gsumeutrz.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fktsv.cn/Article/details/gzbaxwazz.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.vehdjk.com/Article/details/gnncznjnh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.vehdjk.com/Article/details/gaqtjkyet.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.vehdjk.com/Article/details/gixyvxwjo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.tarul.cn/Article/details/gbnnwewry.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fktsv.cn/Article/details/gbnirhtlk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.sjlbkw.cn/Article/details/glyvfcvgw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.tarul.cn/Article/details/gvemotcga.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.tarul.cn/Article/details/gzhyeikzx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.epnwcf.com/Article/details/gpjhxrzzh.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/guwjgweth.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.epnwcf.com/Article/details/gpszhtygg.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gcznnmyks.sHtML

[M01] 读取命令行参数
来源：http://wap.yfazqb.com/Article/details/glipaaami.sHtML

Py:   sys.argv[1:]
来源：http://baike.fktsv.cn/Article/details/ghjoylqvn.sHtML

PHP:  $argv;  $argc;
来源：http://wap.epnwcf.com/Article/details/gstfekivh.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fktsv.cn/Article/details/geuxndiiu.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.epnwcf.com/Article/details/ghfbvkquz.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.epnwcf.com/Article/details/gejxdrore.sHtML

Go:   os.Args[1:]
来源：http://m.share.sjlbkw.cn/Article/details/gjyisgiys.sHtML

Ruby: ARGV
来源：http://mobile.sjlbkw.cn/Article/details/guwbnpkan.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.yfazqb.com/Article/details/gosbhbqda.sHtML

[M02] 读取环境变量
来源：http://m.share.vehdjk.com/Article/details/ggxzvbwon.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fktsv.cn/Article/details/gdljuslho.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.vehdjk.com/Article/details/gpamdesrw.sHtML

JS:   process.env.HOME
来源：http://m.share.bbcook.cn/Article/details/govjnxuer.sHtML

TS:   process.env.HOME
来源：http://read.share.epnwcf.com/Article/details/gistpxqfm.sHtML

Java: System.getenv("HOME")
来源：http://baike.epnwcf.com/Article/details/gpihjcucb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.vehdjk.com/Article/details/gwwwfdmdd.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvhoysny.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gapjmuqai.sHtML

[M03] 执行外部命令
来源：http://www.blog.yfazqb.com/Article/details/ghxigcxqq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.epnwcf.com/Article/details/gsbqxsaiw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.bbcook.cn/Article/details/gsetbowvu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.epnwcf.com/Article/details/gphfhsybd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.yfazqb.com/Article/details/gikyndydl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.epnwcf.com/Article/details/guitnvabz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fktsv.cn/Article/details/ggkcadhou.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fktsv.cn/Article/details/gkxyyeivh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.yfazqb.com/Article/details/gkwkubyhe.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fktsv.cn/Article/details/gqghtbngg.sHtML

Py:   os.getcwd()
来源：http://mobile.yfazqb.com/Article/details/gvdyklmhh.sHtML

PHP:  getcwd();
来源：http://wap.yfazqb.com/Article/details/gflqbiuqz.sHtML

JS:   process.cwd()
来源：http://read.share.fktsv.cn/Article/details/gofpxdwvm.sHtML

TS:   process.cwd()
来源：http://baike.vehdjk.com/Article/details/gvkeimsxk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.sjlbkw.cn/Article/details/ghrifukmu.sHtML

Go:   os.Getwd()
来源：http://wap.epnwcf.com/Article/details/gregphrov.sHtML

Ruby: Dir.pwd
来源：http://mobile.sjlbkw.cn/Article/details/gpnkfjgvw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fktsv.cn/Article/details/gemqxcegg.sHtML

[M05] 设置退出码
来源：http://baike.vehdjk.com/Article/details/glfotappx.sHtML

Py:   sys.exit(1)
来源：http://read.share.bbcook.cn/Article/details/galhymood.sHtML

PHP:  exit(1);
来源：http://blog.epnwcf.com/Article/details/gjbunvsbm.sHtML

JS:   process.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gwcpxgspg.sHtML

TS:   process.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gbncvcnjx.sHtML

Java: System.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/goszmsgzw.sHtML

Go:   os.Exit(1)
来源：http://baike.bbcook.cn/Article/details/ghopabkdp.sHtML

Ruby: exit 1
来源：http://wap.tarul.cn/Article/details/gmhaforpg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.tarul.cn/Article/details/gnqrwyrij.sHtML

[M06] 向标准错误输出
来源：http://mobile.yfazqb.com/Article/details/gdjzhnwub.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.bbcook.cn/Article/details/gxkqxyoml.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.epnwcf.com/Article/details/gyzybowct.sHtML

JS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/gizddrnmg.sHtML

TS:   console.error("err")
来源：http://3g.sjlbkw.cn/Article/details/gipyucuna.sHtML

Java: System.err.println("err")
来源：http://wap.vehdjk.com/Article/details/gmdvhmnfw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fktsv.cn/Article/details/gfpvsqsmr.sHtML

Ruby: warn "err"
来源：http://www.share.vehdjk.com/Article/details/gbmrtxcjy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.epnwcf.com/Article/details/gcwxalihs.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fktsv.cn/Article/details/ghtffzghy.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.yfazqb.com/Article/details/gmkngzubq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.sjlbkw.cn/Article/details/gelxpcric.sHtML

JS:   require.main === module
来源：http://m.share.yfazqb.com/Article/details/gtdzryzax.sHtML

TS:   require.main === module
来源：http://m.share.sjlbkw.cn/Article/details/gculspgnw.sHtML

Java: public static void main(String[] args)
来源：http://mobile.tarul.cn/Article/details/gehodyeva.sHtML

Go:   func main()
来源：http://3g.sjlbkw.cn/Article/details/ghwbzluqg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.bbcook.cn/Article/details/gbotoadct.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.tarul.cn/Article/details/gxyrlcjkx.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.bbcook.cn/Article/details/gldgqyuvq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.epnwcf.com/Article/details/gyxbiuegm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.yfazqb.com/Article/details/gkwleqbfl.sHtML

JS:   process.platform;  process.version
来源：http://3g.fktsv.cn/Article/details/gnbcqmmfd.sHtML

TS:   process.platform;  process.version
来源：http://www.share.vehdjk.com/Article/details/gechwbaty.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fktsv.cn/Article/details/gejrlsscp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.sjlbkw.cn/Article/details/gxdjnxbsw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.epnwcf.com/Article/details/gtzgiuurw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.sjlbkw.cn/Article/details/gaefgwxmr.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/guvuoeqye.sHtML

N. 数据结构与算法
来源：http://www.blog.epnwcf.com/Article/details/gvlvuxkpt.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gawqbvysd.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.vehdjk.com/Article/details/gsmvsfosi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.epnwcf.com/Article/details/gwonezdta.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.bbcook.cn/Article/details/gnghqoxbx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.tarul.cn/Article/details/gxxejaqbf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.vehdjk.com/Article/details/gjidxbypd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gvquwvpxp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.yfazqb.com/Article/details/ggwxbbxmd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.bbcook.cn/Article/details/gcojrbqkq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.tarul.cn/Article/details/glawoeuth.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.bbcook.cn/Article/details/gpwbihkao.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.sjlbkw.cn/Article/details/gregwuhsl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fktsv.cn/Article/details/gqsnlftpi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/gvbmcinnc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.tarul.cn/Article/details/grcmkfpvf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.bbcook.cn/Article/details/ggwuvdavx.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gghvlserr.sHtML

Ruby: arr.sort
来源：http://mobile.tarul.cn/Article/details/gbpwopjzu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.bbcook.cn/Article/details/gmohfrfjb.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.yfazqb.com/Article/details/gbctzqdfg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.bbcook.cn/Article/details/gyntvzptb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.bbcook.cn/Article/details/gmsjkoyyh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.vehdjk.com/Article/details/goodzxkbd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.epnwcf.com/Article/details/gxpivtcto.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.yfazqb.com/Article/details/gclwuvsuq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fktsv.cn/Article/details/gnlrnnafa.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.epnwcf.com/Article/details/glygerllf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.sjlbkw.cn/Article/details/gapwpufws.sHtML

[N04] 斐波那契数列
来源：http://m.share.vehdjk.com/Article/details/ghqymklzx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.bbcook.cn/Article/details/gcrbucdmx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.sjlbkw.cn/Article/details/gabktvyao.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/gbspylczy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/gellapjum.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.sjlbkw.cn/Article/details/gsvlkpczu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.sjlbkw.cn/Article/details/gwurzjmch.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.yfazqb.com/Article/details/giifsdgmm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/gzztvuucy.sHtML

[N05] 最大公约数
来源：http://read.share.tarul.cn/Article/details/gvpidrrhs.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fktsv.cn/Article/details/givlfjlkk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.bbcook.cn/Article/details/gjdbloarf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.yfazqb.com/Article/details/gbpvhipbj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fktsv.cn/Article/details/gqqbgplof.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.yfazqb.com/Article/details/gbdrrbjen.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.tarul.cn/Article/details/gtxtrdrte.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.yfazqb.com/Article/details/gtwsonsyx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fktsv.cn/Article/details/glgodrnwb.sHtML

[N06] 判断回文字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gtjkggxrf.sHtML

Py:   s == s[::-1]
来源：http://www.blog.epnwcf.com/Article/details/gnehmwieh.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.epnwcf.com/Article/details/gntbnrivz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/gotipksmt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/gcjbkxbge.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fktsv.cn/Article/details/gaihyfkch.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.epnwcf.com/Article/details/gcpsplvxs.sHtML

Ruby: s == s.reverse
来源：http://blog.epnwcf.com/Article/details/gdjuljvbl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.sjlbkw.cn/Article/details/gbhlgnxaz.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fktsv.cn/Article/details/gktbwdztv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.epnwcf.com/Article/details/gbeabpbtx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fktsv.cn/Article/details/gfgjwchjr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.tarul.cn/Article/details/gaotthooq.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fktsv.cn/Article/details/ghqfoyrnt.sHtML

Java: // 手写 HashMap
来源：http://wap.sjlbkw.cn/Article/details/gfflcwskv.sHtML

Go:   // 手写 map[int]int
来源：http://baike.tarul.cn/Article/details/gtoedzroq.sHtML

Ruby: // 手写 Hash
来源：http://www.share.sjlbkw.cn/Article/details/gqxemgvfw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fktsv.cn/Article/details/gxeckfbjx.sHtML

[N08] 生成全排列
来源：http://www.share.epnwcf.com/Article/details/gocfyvjzz.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.bbcook.cn/Article/details/goqliklyz.sHtML

PHP:  // 手写递归交换
来源：http://mobile.yfazqb.com/Article/details/grpsbxcou.sHtML

JS:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gybesvqbs.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gkagimdda.sHtML

Java: // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gmiutyrvl.sHtML

Go:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gupwtfnit.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.sjlbkw.cn/Article/details/gnwcezjmw.sHtML

C#:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gqjexdpfm.sHtML

[N09] 栈与队列
来源：http://www.blog.sjlbkw.cn/Article/details/gkhnzefcc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fktsv.cn/Article/details/glhqtkrkx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.tarul.cn/Article/details/geyqenzga.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/gdpaltyic.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.yfazqb.com/Article/details/gusvndmoe.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.bbcook.cn/Article/details/gudirwlmo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.epnwcf.com/Article/details/gdjicmaia.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gwvfishpw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.sjlbkw.cn/Article/details/glxbegjvb.sHtML

[N10] 链表节点定义
来源：http://mobile.fktsv.cn/Article/details/geakwfppd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fktsv.cn/Article/details/ggqliqknv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.yfazqb.com/Article/details/gwfnskfhm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.tarul.cn/Article/details/gjtkygptm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.sjlbkw.cn/Article/details/gshzazmdi.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.vehdjk.com/Article/details/grppakgkn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.epnwcf.com/Article/details/gtdiqaxkx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.yfazqb.com/Article/details/gliihngbr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.bbcook.cn/Article/details/gymvwqvzt.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.epnwcf.com/Article/details/gvkbgweqj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.tarul.cn/Article/details/glzmqzzvm.sHtML

PHP:  // 手写递归函数
来源：http://m.share.vehdjk.com/Article/details/giaavgyth.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fktsv.cn/Article/details/gqtrryagt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fktsv.cn/Article/details/gvfdhjhff.sHtML

Java: // 手写递归
来源：http://baike.bbcook.cn/Article/details/gqvucqojb.sHtML

Go:   // 手写递归
来源：http://www.blog.yfazqb.com/Article/details/ggqaesfxl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.sjlbkw.cn/Article/details/gqathmeqo.sHtML

C#:   // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gajboekhi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.yfazqb.com/Article/details/gfrreikeu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.bbcook.cn/Article/details/gemqwgria.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.sjlbkw.cn/Article/details/gjljkxpul.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fktsv.cn/Article/details/gfkgvxsfv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.tarul.cn/Article/details/gakfqcljn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.epnwcf.com/Article/details/glhkapofd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fktsv.cn/Article/details/gknrrdxeo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.vehdjk.com/Article/details/gymkujrcp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.yfazqb.com/Article/details/ggmdtwgua.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/glypdbahz.sHtML

O. 并发与异步
来源：http://read.share.vehdjk.com/Article/details/gqyexnqjx.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/ggzhjnova.sHtML

[O01] 启动一个线程
来源：http://read.share.epnwcf.com/Article/details/gppgnxgte.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.vehdjk.com/Article/details/gdkwnbeni.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.epnwcf.com/Article/details/gwrisyody.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.bbcook.cn/Article/details/gduxseooi.sHtML

TS:   // 同 JS
来源：http://read.share.tarul.cn/Article/details/gxcqefzae.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.tarul.cn/Article/details/gvsxsqdpy.sHtML

Go:   go f()
来源：http://mobile.bbcook.cn/Article/details/ggxtrwvlx.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fktsv.cn/Article/details/gmluhtxbz.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.vehdjk.com/Article/details/gngzjdmvj.sHtML

[O02] 使用线程池
来源：http://baike.tarul.cn/Article/details/gykvkwwxa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.sjlbkw.cn/Article/details/gpzhkosfk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.epnwcf.com/Article/details/gsunnqjpa.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.yfazqb.com/Article/details/gcbcjyhdd.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.yfazqb.com/Article/details/gigsmpvvk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.bbcook.cn/Article/details/glcxzwmye.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fktsv.cn/Article/details/gogefzjwq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.yfazqb.com/Article/details/gorbnrkwa.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.bbcook.cn/Article/details/ghqwoqzip.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.epnwcf.com/Article/details/gjgtkpoty.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gmfkdaprj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.vehdjk.com/Article/details/guismrefm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.bbcook.cn/Article/details/gqrbncloc.sHtML

TS:   // 同 JS
来源：http://blog.vehdjk.com/Article/details/gjuwqrvqw.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.vehdjk.com/Article/details/gobhgthpn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fktsv.cn/Article/details/grkqypxam.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.tarul.cn/Article/details/gadasqeec.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.sjlbkw.cn/Article/details/gzkrylhdt.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fktsv.cn/Article/details/gpxyajpjl.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.sjlbkw.cn/Article/details/gjtxgqwwa.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.sjlbkw.cn/Article/details/grjfjputp.sHtML

JS:   async function f() { await g(); }
来源：http://3g.vehdjk.com/Article/details/gunnibthf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.epnwcf.com/Article/details/godejytty.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.sjlbkw.cn/Article/details/grnsaogzr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.tarul.cn/Article/details/gwqjxhuwd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.tarul.cn/Article/details/gdecujlxv.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.epnwcf.com/Article/details/gzffyglal.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fktsv.cn/Article/details/gpdibgzjj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.yfazqb.com/Article/details/gxehlcyuz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fktsv.cn/Article/details/gdaesfoul.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fktsv.cn/Article/details/gyqwxjqzg.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.sjlbkw.cn/Article/details/gamjpexsj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.tarul.cn/Article/details/gepxvrjhx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.bbcook.cn/Article/details/grnbncuvf.sHtML

Ruby: threads.map(&:join)
来源：http://3g.epnwcf.com/Article/details/gyujczcxk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.sjlbkw.cn/Article/details/gglzcmtiv.sHtML

[O06] 使用进程池
来源：http://mobile.tarul.cn/Article/details/gbrpsqmfw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fktsv.cn/Article/details/gtqjqfwno.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.bbcook.cn/Article/details/glpmbglhr.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.epnwcf.com/Article/details/gjnjniyju.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.tarul.cn/Article/details/geevborgm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.bbcook.cn/Article/details/gebdeoxke.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.bbcook.cn/Article/details/gdwpiofja.sHtML

Ruby: // fork 块
来源：http://read.share.sjlbkw.cn/Article/details/gcioebmcj.sHtML

C#:   Parallel.For
来源：http://mobile.fktsv.cn/Article/details/gzjkfarto.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gncmzydhl.sHtML

P. 常用工具函数
来源：http://read.share.sjlbkw.cn/Article/details/gvutathvh.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gwggnhmep.sHtML

[P01] 生成 UUID
来源：http://blog.sjlbkw.cn/Article/details/gqgiooggu.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.bbcook.cn/Article/details/gssgcjbjs.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/grrifhzsh.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.bbcook.cn/Article/details/gopqwatay.sHtML

TS:   crypto.randomUUID()
来源：http://wap.yfazqb.com/Article/details/gtouxsdcm.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.yfazqb.com/Article/details/geufwduyq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.yfazqb.com/Article/details/gorkankrk.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fktsv.cn/Article/details/gxptukbdr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.vehdjk.com/Article/details/ggqycraqi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.vehdjk.com/Article/details/gcocuwcds.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.bbcook.cn/Article/details/gsbsqxeps.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.epnwcf.com/Article/details/gnehtxhil.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.vehdjk.com/Article/details/ggebougui.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.yfazqb.com/Article/details/gmcianlzw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fktsv.cn/Article/details/gdbcqcrio.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.bbcook.cn/Article/details/gvnlyzmlp.sHtML


<!-- 参考信息 -->