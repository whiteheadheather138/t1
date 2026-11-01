代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.bbcook.cn/Article/details/guyhpoeah.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fktsv.cn/Article/details/gdgjgdezs.sHtML

[L05] 上传文件（multipart）
来源：http://baike.vehdjk.com/Article/details/gczubsqci.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.bbcook.cn/Article/details/gmzvigmze.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.bbcook.cn/Article/details/gqcmbylkj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.tarul.cn/Article/details/gkxuocqpb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.sjlbkw.cn/Article/details/gjrlqwswe.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.bbcook.cn/Article/details/grfucmcio.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.tarul.cn/Article/details/gvawioman.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.tarul.cn/Article/details/guxkcrfic.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.yfazqb.com/Article/details/ghqybgwyz.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.yfazqb.com/Article/details/ghkvbadox.sHtML

Py:   resp.json()
来源：http://wap.vehdjk.com/Article/details/gxfbywivp.sHtML

PHP:  json_decode($body, true);
来源：http://baike.tarul.cn/Article/details/ghriixkdr.sHtML

JS:   await resp.json()
来源：http://www.m.share.yfazqb.com/Article/details/gmwdjqbms.sHtML

TS:   await resp.json()
来源：http://baike.epnwcf.com/Article/details/gxrhqbhqg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.epnwcf.com/Article/details/gpbsmharx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fktsv.cn/Article/details/gyklqmslz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.vehdjk.com/Article/details/gsseotkji.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fktsv.cn/Article/details/guleylpgm.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.yfazqb.com/Article/details/gsljzahqr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.epnwcf.com/Article/details/gbcikpqzw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.bbcook.cn/Article/details/gmrwoduzu.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.bbcook.cn/Article/details/gattwissd.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.vehdjk.com/Article/details/gtvkjrlve.sHtML

Java: resp.statusCode()
来源：http://mobile.yfazqb.com/Article/details/gnplsnbzt.sHtML

Go:   resp.StatusCode
来源：http://read.share.vehdjk.com/Article/details/giliycvuq.sHtML

Ruby: resp.code.to_i
来源：http://baike.yfazqb.com/Article/details/gbdqwetzs.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fktsv.cn/Article/details/gvcpaofdc.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.vehdjk.com/Article/details/ggzcukjbk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.tarul.cn/Article/details/gxwartqly.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.tarul.cn/Article/details/glbjolexi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.epnwcf.com/Article/details/ghwxqpeua.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gecryfvat.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.yfazqb.com/Article/details/gknrydwpv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fktsv.cn/Article/details/geqwurmns.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.tarul.cn/Article/details/gpovszojv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fktsv.cn/Article/details/gjbcjlare.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gjoqybrpc.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.tarul.cn/Article/details/gskiiqlgd.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gipvkbfns.sHtML

[M01] 读取命令行参数
来源：http://www.blog.epnwcf.com/Article/details/gubxgwjdv.sHtML

Py:   sys.argv[1:]
来源：http://mobile.yfazqb.com/Article/details/gebjvxewp.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fktsv.cn/Article/details/gpmpxgabf.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.tarul.cn/Article/details/gkrfcuuss.sHtML

TS:   process.argv.slice(2)
来源：http://blog.sjlbkw.cn/Article/details/gzvfjglyz.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.bbcook.cn/Article/details/gxaozcblp.sHtML

Go:   os.Args[1:]
来源：http://3g.bbcook.cn/Article/details/gbzahqlsc.sHtML

Ruby: ARGV
来源：http://mobile.tarul.cn/Article/details/gkjxdsmbv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.epnwcf.com/Article/details/giidhhgcv.sHtML

[M02] 读取环境变量
来源：http://mobile.bbcook.cn/Article/details/gpvwwebjb.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.tarul.cn/Article/details/gygweovyd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.bbcook.cn/Article/details/gakavaoab.sHtML

JS:   process.env.HOME
来源：http://wap.bbcook.cn/Article/details/gzitwpbsn.sHtML

TS:   process.env.HOME
来源：http://www.blog.tarul.cn/Article/details/gniepplng.sHtML

Java: System.getenv("HOME")
来源：http://baike.vehdjk.com/Article/details/gofdormpv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.bbcook.cn/Article/details/ghorepjlo.sHtML

Ruby: ENV["HOME"]
来源：http://baike.yfazqb.com/Article/details/gtsgkvebx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.tarul.cn/Article/details/gojnphjba.sHtML

[M03] 执行外部命令
来源：http://mobile.epnwcf.com/Article/details/gqybdiqhh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.epnwcf.com/Article/details/gvlgghuwl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.vehdjk.com/Article/details/gqzggrarw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.sjlbkw.cn/Article/details/gxcrqsbro.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.yfazqb.com/Article/details/gqehdxrbe.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.bbcook.cn/Article/details/gmtftnpkw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.vehdjk.com/Article/details/gsckwhzfm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.sjlbkw.cn/Article/details/gwnfjmdrf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.vehdjk.com/Article/details/gbpmzjljz.sHtML

[M04] 获取当前工作目录
来源：http://3g.tarul.cn/Article/details/gwafaiemq.sHtML

Py:   os.getcwd()
来源：http://m.share.fktsv.cn/Article/details/gffqiajot.sHtML

PHP:  getcwd();
来源：http://wap.fktsv.cn/Article/details/gflgkvrcw.sHtML

JS:   process.cwd()
来源：http://baike.fktsv.cn/Article/details/gitvswxih.sHtML

TS:   process.cwd()
来源：http://mobile.fktsv.cn/Article/details/gmfsgbzej.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.epnwcf.com/Article/details/gllikjcyz.sHtML

Go:   os.Getwd()
来源：http://read.share.fktsv.cn/Article/details/gjwgmiucs.sHtML

Ruby: Dir.pwd
来源：http://read.share.tarul.cn/Article/details/gwjeftkna.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.yfazqb.com/Article/details/gglrucdfl.sHtML

[M05] 设置退出码
来源：http://www.blog.fktsv.cn/Article/details/gloevmzoo.sHtML

Py:   sys.exit(1)
来源：http://wap.epnwcf.com/Article/details/gzibopgvh.sHtML

PHP:  exit(1);
来源：http://m.share.bbcook.cn/Article/details/guughzneq.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gujrosumn.sHtML

TS:   process.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gcrfodnig.sHtML

Java: System.exit(1)
来源：http://3g.vehdjk.com/Article/details/gpvswajwa.sHtML

Go:   os.Exit(1)
来源：http://blog.bbcook.cn/Article/details/gmnxtrauy.sHtML

Ruby: exit 1
来源：http://mobile.vehdjk.com/Article/details/gefnsheuj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.vehdjk.com/Article/details/gqdqolmeq.sHtML

[M06] 向标准错误输出
来源：http://blog.yfazqb.com/Article/details/gahwsmkqe.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.tarul.cn/Article/details/gqejxtovn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.yfazqb.com/Article/details/gxefvrwaf.sHtML

JS:   console.error("err")
来源：http://read.share.epnwcf.com/Article/details/gggxxcbex.sHtML

TS:   console.error("err")
来源：http://blog.tarul.cn/Article/details/gqftuhiwz.sHtML

Java: System.err.println("err")
来源：http://m.share.fktsv.cn/Article/details/gvrfuorae.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gedfbfijp.sHtML

Ruby: warn "err"
来源：http://www.m.share.bbcook.cn/Article/details/grkgghabn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.bbcook.cn/Article/details/gabktliun.sHtML

[M07] 判断是否为主入口
来源：http://mobile.yfazqb.com/Article/details/gfudvypsr.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.tarul.cn/Article/details/gphwtbgxi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.epnwcf.com/Article/details/gfjaincsk.sHtML

JS:   require.main === module
来源：http://www.blog.epnwcf.com/Article/details/gphmcfaza.sHtML

TS:   require.main === module
来源：http://wap.tarul.cn/Article/details/grufscpjf.sHtML

Java: public static void main(String[] args)
来源：http://www.share.tarul.cn/Article/details/gufpnuuhb.sHtML

Go:   func main()
来源：http://mobile.epnwcf.com/Article/details/gewetgxvz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.sjlbkw.cn/Article/details/ggjdzedhe.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fktsv.cn/Article/details/gfplqvnlh.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fktsv.cn/Article/details/gfsinvnsh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.yfazqb.com/Article/details/gkfckzvsy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.tarul.cn/Article/details/gxeaeqqdq.sHtML

JS:   process.platform;  process.version
来源：http://3g.vehdjk.com/Article/details/ghdeujrfx.sHtML

TS:   process.platform;  process.version
来源：http://wap.epnwcf.com/Article/details/ggqcchpgz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fktsv.cn/Article/details/gawiuflzi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.yfazqb.com/Article/details/gssehwseb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.yfazqb.com/Article/details/gnyimnfqn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.vehdjk.com/Article/details/gaboxeyas.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gviimtnhj.sHtML

N. 数据结构与算法
来源：http://read.share.sjlbkw.cn/Article/details/gxdjvdtbc.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gwdhzesoa.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.tarul.cn/Article/details/gejdnywpu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.epnwcf.com/Article/details/gspqjejye.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.tarul.cn/Article/details/guzagswej.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.tarul.cn/Article/details/gjxnlrcve.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fktsv.cn/Article/details/gjuavsrmx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gdpqstydu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.vehdjk.com/Article/details/griygspoz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fktsv.cn/Article/details/gyofhyepe.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.tarul.cn/Article/details/gmahnmrau.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fktsv.cn/Article/details/glonyorox.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.epnwcf.com/Article/details/goismvgsj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fktsv.cn/Article/details/gtbylozqb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.epnwcf.com/Article/details/gkewudioi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.yfazqb.com/Article/details/gtnhgonwf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.vehdjk.com/Article/details/gdzlkirzg.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gvuvufeag.sHtML

Ruby: arr.sort
来源：http://3g.yfazqb.com/Article/details/gnvzviarz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.yfazqb.com/Article/details/gtfplgefr.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.tarul.cn/Article/details/gcxhpopkc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fktsv.cn/Article/details/gkpwxzabd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.sjlbkw.cn/Article/details/gcyhrnkbl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.epnwcf.com/Article/details/gsyjamffp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.sjlbkw.cn/Article/details/grnlirien.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.yfazqb.com/Article/details/geosfmvhh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fktsv.cn/Article/details/gnxfdqpws.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.vehdjk.com/Article/details/gthelygxa.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.epnwcf.com/Article/details/gplphmqbt.sHtML

[N04] 斐波那契数列
来源：http://baike.bbcook.cn/Article/details/gvsoakcfx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fktsv.cn/Article/details/gwcrhdnww.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.bbcook.cn/Article/details/guzjuctes.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/gdxjvoqph.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/grombbppi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.bbcook.cn/Article/details/gnzhbsflp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.epnwcf.com/Article/details/gaducgqqf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.tarul.cn/Article/details/gpnurcsbg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gjatpgzds.sHtML

[N05] 最大公约数
来源：http://blog.sjlbkw.cn/Article/details/gbbniyjqm.sHtML

Py:   math.gcd(a, b)
来源：http://blog.epnwcf.com/Article/details/ghsrmpemq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.epnwcf.com/Article/details/gtvxfehln.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.tarul.cn/Article/details/gqeltoqau.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdrqqmhh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.sjlbkw.cn/Article/details/gdernddlv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.bbcook.cn/Article/details/gszxkerfr.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fktsv.cn/Article/details/gonkvkpva.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.sjlbkw.cn/Article/details/gwytsdvfn.sHtML

[N06] 判断回文字符串
来源：http://read.share.yfazqb.com/Article/details/gksyfbxun.sHtML

Py:   s == s[::-1]
来源：http://baike.yfazqb.com/Article/details/ghiplxcni.sHtML

PHP:  $s === strrev($s);
来源：http://baike.sjlbkw.cn/Article/details/gnfkvwrrx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gpxnqblgb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fktsv.cn/Article/details/gpnsqnxld.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.vehdjk.com/Article/details/gleeqlkys.sHtML

Go:   // 双指针从两端比较
来源：http://blog.vehdjk.com/Article/details/ggtunzukv.sHtML

Ruby: s == s.reverse
来源：http://3g.epnwcf.com/Article/details/gosdxrwhp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.sjlbkw.cn/Article/details/gfyjkkwzc.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fktsv.cn/Article/details/gmkxqjxjz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.sjlbkw.cn/Article/details/gyghufhgl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fktsv.cn/Article/details/gipzbiexi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.bbcook.cn/Article/details/ghfqpiigc.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.bbcook.cn/Article/details/ggffvvuwv.sHtML

Java: // 手写 HashMap
来源：http://www.blog.tarul.cn/Article/details/ggqmananz.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.sjlbkw.cn/Article/details/gxqiiwdby.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.bbcook.cn/Article/details/ggllecxjk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.yfazqb.com/Article/details/gneyrnoma.sHtML

[N08] 生成全排列
来源：http://baike.vehdjk.com/Article/details/glfguibwg.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.vehdjk.com/Article/details/gusjlwkjj.sHtML

PHP:  // 手写递归交换
来源：http://baike.vehdjk.com/Article/details/gieyzihjk.sHtML

JS:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gsexrcgdl.sHtML

TS:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gwjejzfiv.sHtML

Java: // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gxycavbqj.sHtML

Go:   // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/gsyhumfgx.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.yfazqb.com/Article/details/grtpdvean.sHtML

C#:   // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/gzaeiwgxt.sHtML

[N09] 栈与队列
来源：http://3g.epnwcf.com/Article/details/gyzdwffis.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.bbcook.cn/Article/details/glxkpvajb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.yfazqb.com/Article/details/gqlbnxagf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gykjjyagy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fktsv.cn/Article/details/glcyqripo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.yfazqb.com/Article/details/giedjfceh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.vehdjk.com/Article/details/gvqbvyhuh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.tarul.cn/Article/details/ghnnhuhkf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.tarul.cn/Article/details/gyfrmvsgy.sHtML

[N10] 链表节点定义
来源：http://blog.vehdjk.com/Article/details/gsslgezwl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.tarul.cn/Article/details/gqxvokrix.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.bbcook.cn/Article/details/gomqlsrbc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.vehdjk.com/Article/details/ghokzjwfk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.tarul.cn/Article/details/gyvcjuxon.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.vehdjk.com/Article/details/gguvqumpa.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.tarul.cn/Article/details/gcdklawri.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.yfazqb.com/Article/details/gsrkwrfps.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.bbcook.cn/Article/details/genqkfgjt.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.vehdjk.com/Article/details/gblxrxvzt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fktsv.cn/Article/details/gbtwbnpwe.sHtML

PHP:  // 手写递归函数
来源：http://3g.vehdjk.com/Article/details/gdbdfstiy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fktsv.cn/Article/details/gfeculpen.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmjkcsba.sHtML

Java: // 手写递归
来源：http://www.m.share.bbcook.cn/Article/details/gtkatqjyq.sHtML

Go:   // 手写递归
来源：http://mobile.fktsv.cn/Article/details/gwotyzpwn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.sjlbkw.cn/Article/details/gggxsasxh.sHtML

C#:   // 手写递归
来源：http://wap.fktsv.cn/Article/details/ggfqnlwzv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.bbcook.cn/Article/details/ghimqbfot.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.vehdjk.com/Article/details/gfkbhacer.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.bbcook.cn/Article/details/gncnmgyfd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fktsv.cn/Article/details/gxqpohyqm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.epnwcf.com/Article/details/gffhwbeph.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fktsv.cn/Article/details/gpkvuspxd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.vehdjk.com/Article/details/gtvjeiphi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fktsv.cn/Article/details/glunafrsg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.sjlbkw.cn/Article/details/gcnlazjqf.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gkjreapcu.sHtML

O. 并发与异步
来源：http://3g.vehdjk.com/Article/details/gozsusvxj.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gebjhyecv.sHtML

[O01] 启动一个线程
来源：http://3g.bbcook.cn/Article/details/gkveadbfk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.tarul.cn/Article/details/gktjsheep.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.vehdjk.com/Article/details/gqnibptjq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fktsv.cn/Article/details/gyjfvjjrz.sHtML

TS:   // 同 JS
来源：http://wap.bbcook.cn/Article/details/glxnclmlp.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.yfazqb.com/Article/details/gbosnfgrt.sHtML

Go:   go f()
来源：http://m.share.fktsv.cn/Article/details/gdcaepgpv.sHtML

Ruby: Thread.new { f }
来源：http://wap.sjlbkw.cn/Article/details/gdpphoyih.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.sjlbkw.cn/Article/details/ggrxrpatk.sHtML

[O02] 使用线程池
来源：http://3g.sjlbkw.cn/Article/details/gvcvbswdr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.tarul.cn/Article/details/giabhiqgr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.tarul.cn/Article/details/gjandkcbj.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.epnwcf.com/Article/details/glpsndiee.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.tarul.cn/Article/details/gjnwlzrvh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.tarul.cn/Article/details/gcljhonti.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.epnwcf.com/Article/details/gpgxnausd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.epnwcf.com/Article/details/gckqivzrf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.epnwcf.com/Article/details/gesgyhxle.sHtML

[O03] 加锁保护共享数据
来源：http://baike.tarul.cn/Article/details/gqxchylnd.sHtML

Py:   with lock: shared += 1
来源：http://www.share.tarul.cn/Article/details/giexrmhbc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fktsv.cn/Article/details/gjtohramk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.tarul.cn/Article/details/gzyjfemiu.sHtML

TS:   // 同 JS
来源：http://www.m.share.epnwcf.com/Article/details/gieahetxv.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.yfazqb.com/Article/details/grbergwnp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fktsv.cn/Article/details/gzgivolfb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.vehdjk.com/Article/details/gjtloyaaj.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.sjlbkw.cn/Article/details/gvoyjishc.sHtML

[O04] 定义异步函数并等待
来源：http://blog.vehdjk.com/Article/details/gvnospyqv.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.tarul.cn/Article/details/gnylcsrzj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.tarul.cn/Article/details/gryuoypdy.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.epnwcf.com/Article/details/ghilzspld.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.vehdjk.com/Article/details/gtdhuskvv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.sjlbkw.cn/Article/details/gcltdjxpt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.bbcook.cn/Article/details/gasoehgjj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.tarul.cn/Article/details/gevmeearn.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.epnwcf.com/Article/details/gvoakwzaa.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.sjlbkw.cn/Article/details/gyuwknftl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.tarul.cn/Article/details/golrxevhf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fktsv.cn/Article/details/givpmuvqk.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqezwzku.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.sjlbkw.cn/Article/details/gvoiocrua.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfigpwryd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.bbcook.cn/Article/details/gmhmpyixl.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.tarul.cn/Article/details/gzmiutmgm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.vehdjk.com/Article/details/guvhpjvok.sHtML

[O06] 使用进程池
来源：http://www.blog.yfazqb.com/Article/details/gqwoydlwc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.vehdjk.com/Article/details/gzwesjieu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.sjlbkw.cn/Article/details/gqyfginwt.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.bbcook.cn/Article/details/gbpljbpdk.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.yfazqb.com/Article/details/gixtbpnhf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.bbcook.cn/Article/details/gwamhclax.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.bbcook.cn/Article/details/gwbahubft.sHtML

Ruby: // fork 块
来源：http://www.blog.bbcook.cn/Article/details/gdkgkonld.sHtML

C#:   Parallel.For
来源：http://baike.tarul.cn/Article/details/gaeiocgud.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/ghtnoqore.sHtML

P. 常用工具函数
来源：http://www.m.share.vehdjk.com/Article/details/gnnqaruvr.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gzdogjxsu.sHtML

[P01] 生成 UUID
来源：http://read.share.bbcook.cn/Article/details/gvwfexcew.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.tarul.cn/Article/details/gdrgpttyb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.vehdjk.com/Article/details/gzeujzenl.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fktsv.cn/Article/details/gzplsogrm.sHtML

TS:   crypto.randomUUID()
来源：http://baike.epnwcf.com/Article/details/gmvwjpeey.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.epnwcf.com/Article/details/gtrwyetfp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.epnwcf.com/Article/details/gbgfqstyt.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhiuwyqq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.sjlbkw.cn/Article/details/glvucgjor.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.sjlbkw.cn/Article/details/ggvsqphfg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.vehdjk.com/Article/details/gdppoxqcu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.tarul.cn/Article/details/gumjqzndp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.bbcook.cn/Article/details/gickfegwe.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.tarul.cn/Article/details/gbccosscj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.yfazqb.com/Article/details/gbsimwuod.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.epnwcf.com/Article/details/gnillgnqn.sHtML


<!-- 参考信息 -->