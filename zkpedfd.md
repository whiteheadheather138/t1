代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.sjlbkw.cn/Article/details/gxhmxogaj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.yfazqb.com/Article/details/grhqgaqgm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.yfazqb.com/Article/details/gmisbehvd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.epnwcf.com/Article/details/gxvsvigiy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.tarul.cn/Article/details/ghjhgvxsu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fktsv.cn/Article/details/gldupiwaf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fktsv.cn/Article/details/guwmcrqcr.sHtML

[L06] 解析响应为 JSON
来源：http://baike.sjlbkw.cn/Article/details/gaejaajff.sHtML

Py:   resp.json()
来源：http://www.blog.sjlbkw.cn/Article/details/gvnjjeaqx.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fktsv.cn/Article/details/gdetdkcss.sHtML

JS:   await resp.json()
来源：http://wap.vehdjk.com/Article/details/gxhyoicaf.sHtML

TS:   await resp.json()
来源：http://baike.fktsv.cn/Article/details/gxjehameh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.vehdjk.com/Article/details/gowyshgvz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fktsv.cn/Article/details/gtomxkhja.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.epnwcf.com/Article/details/ggqztvmah.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.tarul.cn/Article/details/guyqwkiwc.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.sjlbkw.cn/Article/details/gzxocbepc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.vehdjk.com/Article/details/gzrtfycce.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.tarul.cn/Article/details/grbacjcvj.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.epnwcf.com/Article/details/gdpprvehn.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.epnwcf.com/Article/details/gvqkuhyua.sHtML

Java: resp.statusCode()
来源：http://mobile.sjlbkw.cn/Article/details/gosqllyuy.sHtML

Go:   resp.StatusCode
来源：http://mobile.bbcook.cn/Article/details/gohigxzbj.sHtML

Ruby: resp.code.to_i
来源：http://blog.epnwcf.com/Article/details/gnltnhpvn.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fktsv.cn/Article/details/gaucqieak.sHtML

[L08] 并发请求多个地址
来源：http://3g.bbcook.cn/Article/details/gxkdujzvj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.epnwcf.com/Article/details/ggvtkvbxk.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.yfazqb.com/Article/details/gewwfnykt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fktsv.cn/Article/details/gqxwnqhwr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.sjlbkw.cn/Article/details/gdmqtoeti.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.yfazqb.com/Article/details/gyjsbghhp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.yfazqb.com/Article/details/gnwbqxllt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.sjlbkw.cn/Article/details/gjoptjfkl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.bbcook.cn/Article/details/gtwfeduzf.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gjfshgkmn.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.tarul.cn/Article/details/gjrpdxwnl.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gnmgrdxxq.sHtML

[M01] 读取命令行参数
来源：http://read.share.fktsv.cn/Article/details/gvawpfsex.sHtML

Py:   sys.argv[1:]
来源：http://www.share.epnwcf.com/Article/details/gcffctowl.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.vehdjk.com/Article/details/gyqjuxfzi.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.bbcook.cn/Article/details/gccvkemvj.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwgfrfzd.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.vehdjk.com/Article/details/gbwjcaikz.sHtML

Go:   os.Args[1:]
来源：http://3g.vehdjk.com/Article/details/gbzrbgcaz.sHtML

Ruby: ARGV
来源：http://www.blog.tarul.cn/Article/details/gcxkcfupp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.yfazqb.com/Article/details/gskgghrkc.sHtML

[M02] 读取环境变量
来源：http://www.blog.epnwcf.com/Article/details/gvgifyvfi.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gwahfzrgk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.tarul.cn/Article/details/gpqmejako.sHtML

JS:   process.env.HOME
来源：http://blog.vehdjk.com/Article/details/gyyulnaln.sHtML

TS:   process.env.HOME
来源：http://m.share.tarul.cn/Article/details/gqzikdllz.sHtML

Java: System.getenv("HOME")
来源：http://wap.bbcook.cn/Article/details/gsbvpsxtr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.vehdjk.com/Article/details/gadhttgpb.sHtML

Ruby: ENV["HOME"]
来源：http://3g.bbcook.cn/Article/details/glntfznvi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fktsv.cn/Article/details/guhrkzznz.sHtML

[M03] 执行外部命令
来源：http://mobile.bbcook.cn/Article/details/ghsaavwrm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.tarul.cn/Article/details/gdrpwqxup.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fktsv.cn/Article/details/gjimsuxcv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.yfazqb.com/Article/details/ggqdhkjci.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.sjlbkw.cn/Article/details/gxdezmquy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fktsv.cn/Article/details/gnhqbwazm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fktsv.cn/Article/details/glswicnts.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.sjlbkw.cn/Article/details/guymgitth.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fktsv.cn/Article/details/grgegdkpl.sHtML

[M04] 获取当前工作目录
来源：http://m.share.sjlbkw.cn/Article/details/gnakzzrea.sHtML

Py:   os.getcwd()
来源：http://www.blog.fktsv.cn/Article/details/gukfdrztk.sHtML

PHP:  getcwd();
来源：http://baike.yfazqb.com/Article/details/gzdvtaltp.sHtML

JS:   process.cwd()
来源：http://wap.vehdjk.com/Article/details/gjlkalfst.sHtML

TS:   process.cwd()
来源：http://www.m.share.epnwcf.com/Article/details/gbreqgjfh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.yfazqb.com/Article/details/gvvtmrvfw.sHtML

Go:   os.Getwd()
来源：http://3g.sjlbkw.cn/Article/details/gphmmzati.sHtML

Ruby: Dir.pwd
来源：http://www.share.vehdjk.com/Article/details/glvegzzfq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.epnwcf.com/Article/details/glfokuhce.sHtML

[M05] 设置退出码
来源：http://read.share.sjlbkw.cn/Article/details/gojsvljoq.sHtML

Py:   sys.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gvvsrkrps.sHtML

PHP:  exit(1);
来源：http://3g.bbcook.cn/Article/details/gdqpaiobq.sHtML

JS:   process.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gucnliwre.sHtML

TS:   process.exit(1)
来源：http://wap.bbcook.cn/Article/details/gaziyloac.sHtML

Java: System.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gejxplbhl.sHtML

Go:   os.Exit(1)
来源：http://wap.bbcook.cn/Article/details/gzcfqsbmj.sHtML

Ruby: exit 1
来源：http://wap.sjlbkw.cn/Article/details/gkvefzfxp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.epnwcf.com/Article/details/gnpxtbzyr.sHtML

[M06] 向标准错误输出
来源：http://m.share.epnwcf.com/Article/details/gtrlnywbb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.yfazqb.com/Article/details/ggicrgxro.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.vehdjk.com/Article/details/gkulhndze.sHtML

JS:   console.error("err")
来源：http://read.share.sjlbkw.cn/Article/details/gdrwnnfuy.sHtML

TS:   console.error("err")
来源：http://mobile.tarul.cn/Article/details/gyfvyyiyn.sHtML

Java: System.err.println("err")
来源：http://read.share.epnwcf.com/Article/details/gqfhaxodv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.epnwcf.com/Article/details/gnbvfvhvn.sHtML

Ruby: warn "err"
来源：http://www.blog.yfazqb.com/Article/details/gsicpipfl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.vehdjk.com/Article/details/gnmxzbbzv.sHtML

[M07] 判断是否为主入口
来源：http://3g.tarul.cn/Article/details/gbawivmzq.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.epnwcf.com/Article/details/ggxvkrjce.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.epnwcf.com/Article/details/gmrzbmqun.sHtML

JS:   require.main === module
来源：http://www.share.bbcook.cn/Article/details/gxkbxwppq.sHtML

TS:   require.main === module
来源：http://3g.bbcook.cn/Article/details/gdfizdrnj.sHtML

Java: public static void main(String[] args)
来源：http://blog.vehdjk.com/Article/details/ghueorpfq.sHtML

Go:   func main()
来源：http://www.blog.fktsv.cn/Article/details/gylizkhst.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.vehdjk.com/Article/details/gtjtkkqkm.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.vehdjk.com/Article/details/gcpnssnou.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.bbcook.cn/Article/details/gkqavcgab.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.bbcook.cn/Article/details/ggvytqyqa.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.tarul.cn/Article/details/gutcbyxlx.sHtML

JS:   process.platform;  process.version
来源：http://blog.fktsv.cn/Article/details/ggedmtmpy.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fktsv.cn/Article/details/gjqbcajfg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.epnwcf.com/Article/details/gkrqbpbok.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fktsv.cn/Article/details/gitcsrjsx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.epnwcf.com/Article/details/gsrhvrtzo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.sjlbkw.cn/Article/details/gscxufjvd.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gumjpvikt.sHtML

N. 数据结构与算法
来源：http://3g.vehdjk.com/Article/details/gysmgjaun.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gzcmnqxnf.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fktsv.cn/Article/details/gqgyeumbb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.epnwcf.com/Article/details/gngkgrqhi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fktsv.cn/Article/details/gsqftdpti.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fktsv.cn/Article/details/gzoaavfod.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.sjlbkw.cn/Article/details/geaprlreo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gnsahjngi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gllybmtxi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.sjlbkw.cn/Article/details/gawhqomvk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gebuimuru.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.sjlbkw.cn/Article/details/gkjmvnbuo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.vehdjk.com/Article/details/grnpmzsfc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.yfazqb.com/Article/details/gparyukui.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/gintupnxr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fktsv.cn/Article/details/gkvidualv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.tarul.cn/Article/details/gstnefuwn.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gyyhpgvjm.sHtML

Ruby: arr.sort
来源：http://blog.sjlbkw.cn/Article/details/gjzjuvbiz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.vehdjk.com/Article/details/gdrinjqpk.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.bbcook.cn/Article/details/gmvhwzulj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.vehdjk.com/Article/details/guqkgdyqp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.bbcook.cn/Article/details/gsbetbddy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.yfazqb.com/Article/details/ghrrdbusi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fktsv.cn/Article/details/ghezkxlts.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.vehdjk.com/Article/details/ghthhqcas.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fktsv.cn/Article/details/gzufnaapf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.sjlbkw.cn/Article/details/gynjhmocd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.bbcook.cn/Article/details/gekjdokgx.sHtML

[N04] 斐波那契数列
来源：http://wap.sjlbkw.cn/Article/details/gnktodjkv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.sjlbkw.cn/Article/details/gkyfzfamn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.epnwcf.com/Article/details/gconfyons.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.tarul.cn/Article/details/gvgsbebpw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.bbcook.cn/Article/details/gncuezdbb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.tarul.cn/Article/details/gpqhcdgka.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fktsv.cn/Article/details/gafcwpnzd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.bbcook.cn/Article/details/gszazdyio.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/ginqfjxia.sHtML

[N05] 最大公约数
来源：http://m.share.sjlbkw.cn/Article/details/gisbdvngz.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.vehdjk.com/Article/details/glwydgpio.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.sjlbkw.cn/Article/details/gkyjsesjp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.vehdjk.com/Article/details/gaxippkst.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.bbcook.cn/Article/details/gyyxishra.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fktsv.cn/Article/details/gupaxazyo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.vehdjk.com/Article/details/gncumqvfz.sHtML

Ruby: a.gcd(b)
来源：http://m.share.tarul.cn/Article/details/gzixrjeap.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.bbcook.cn/Article/details/gzendpcrb.sHtML

[N06] 判断回文字符串
来源：http://read.share.yfazqb.com/Article/details/gttoovfka.sHtML

Py:   s == s[::-1]
来源：http://blog.fktsv.cn/Article/details/gfaatffno.sHtML

PHP:  $s === strrev($s);
来源：http://3g.bbcook.cn/Article/details/gzvwwhfby.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/gizgntaai.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gufcyafuq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.bbcook.cn/Article/details/ggdubdsmj.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.epnwcf.com/Article/details/gcoxvvwpq.sHtML

Ruby: s == s.reverse
来源：http://m.share.yfazqb.com/Article/details/gyhgxmgyx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.epnwcf.com/Article/details/gauilmswt.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fktsv.cn/Article/details/ggxrtnzog.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.tarul.cn/Article/details/gtsqbhide.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.sjlbkw.cn/Article/details/gryjeubff.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.yfazqb.com/Article/details/gukzdlmaq.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.vehdjk.com/Article/details/gslzzpauv.sHtML

Java: // 手写 HashMap
来源：http://baike.vehdjk.com/Article/details/gfxwudahg.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.tarul.cn/Article/details/gorzghldg.sHtML

Ruby: // 手写 Hash
来源：http://3g.sjlbkw.cn/Article/details/glajrejkm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.yfazqb.com/Article/details/grayruuzr.sHtML

[N08] 生成全排列
来源：http://wap.vehdjk.com/Article/details/gimwahmzc.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.yfazqb.com/Article/details/gxgrpuxqf.sHtML

PHP:  // 手写递归交换
来源：http://www.share.yfazqb.com/Article/details/gjkelulfd.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gueanhssf.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gcepzuhvm.sHtML

Java: // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/grqcdlykb.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdzjkchn.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.bbcook.cn/Article/details/gfvckhyrq.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gnzfovxkw.sHtML

[N09] 栈与队列
来源：http://baike.epnwcf.com/Article/details/gtofjaake.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.epnwcf.com/Article/details/ghyimmmdv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/ggrilyaoy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gwckwufcn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.sjlbkw.cn/Article/details/gcvhbxkya.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.epnwcf.com/Article/details/gennkcqfq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.yfazqb.com/Article/details/gyedypgyq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.tarul.cn/Article/details/gtoxlnecf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.yfazqb.com/Article/details/gulehengu.sHtML

[N10] 链表节点定义
来源：http://baike.sjlbkw.cn/Article/details/gbqoumfdx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.bbcook.cn/Article/details/gnpyqggvh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fktsv.cn/Article/details/gzwqtiwga.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.vehdjk.com/Article/details/guaidiiqn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.tarul.cn/Article/details/gstcckfba.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.bbcook.cn/Article/details/gogguvnds.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.bbcook.cn/Article/details/ghuhaxuaa.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.epnwcf.com/Article/details/gpraysdmk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fktsv.cn/Article/details/glpmpprpg.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.sjlbkw.cn/Article/details/gqvdaruln.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.bbcook.cn/Article/details/gslbnubin.sHtML

PHP:  // 手写递归函数
来源：http://read.share.epnwcf.com/Article/details/gxxuizuyy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.vehdjk.com/Article/details/gfhxpioum.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.yfazqb.com/Article/details/gwogtkxfo.sHtML

Java: // 手写递归
来源：http://www.share.sjlbkw.cn/Article/details/gdqentwqp.sHtML

Go:   // 手写递归
来源：http://wap.epnwcf.com/Article/details/gwxamrnib.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.bbcook.cn/Article/details/gyhiufylh.sHtML

C#:   // 手写递归
来源：http://blog.vehdjk.com/Article/details/gqqfhrcxi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.yfazqb.com/Article/details/gzditwqtk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.epnwcf.com/Article/details/gnlrrusoe.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.vehdjk.com/Article/details/gauhwhxib.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.epnwcf.com/Article/details/gscoyfeoz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.sjlbkw.cn/Article/details/gvvjenjbk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.vehdjk.com/Article/details/gyedjidep.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.yfazqb.com/Article/details/gtlyjgdzv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.sjlbkw.cn/Article/details/grncytuzr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.vehdjk.com/Article/details/gpygzsyer.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gfbtfctgv.sHtML

O. 并发与异步
来源：http://read.share.bbcook.cn/Article/details/gffenybpp.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ghwpkupbk.sHtML

[O01] 启动一个线程
来源：http://www.blog.bbcook.cn/Article/details/gifvxuikr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fktsv.cn/Article/details/gpnxheiie.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.bbcook.cn/Article/details/gzfwosjvv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.vehdjk.com/Article/details/gvidoycrx.sHtML

TS:   // 同 JS
来源：http://mobile.epnwcf.com/Article/details/gievdzmgp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.tarul.cn/Article/details/gunhdzcoc.sHtML

Go:   go f()
来源：http://read.share.fktsv.cn/Article/details/gqpbfahaq.sHtML

Ruby: Thread.new { f }
来源：http://www.share.tarul.cn/Article/details/gclstwobe.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.tarul.cn/Article/details/gfohsnoju.sHtML

[O02] 使用线程池
来源：http://www.share.sjlbkw.cn/Article/details/gmidhvgud.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcpkhoiwd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.epnwcf.com/Article/details/gntdbkmdo.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.bbcook.cn/Article/details/gcdhgtkxa.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwbhsonz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.sjlbkw.cn/Article/details/ggviitjyh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.bbcook.cn/Article/details/grjzvsjaq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.bbcook.cn/Article/details/gxyfuurrk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.vehdjk.com/Article/details/gnuvlujra.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.vehdjk.com/Article/details/gfqrmbmjn.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fktsv.cn/Article/details/gbfhrugyp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.yfazqb.com/Article/details/gnczjrtfg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.yfazqb.com/Article/details/gigtdjrvr.sHtML

TS:   // 同 JS
来源：http://www.m.share.yfazqb.com/Article/details/glabwxwvg.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.epnwcf.com/Article/details/ghicdurfm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.sjlbkw.cn/Article/details/gevoikqhu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.vehdjk.com/Article/details/glaglancc.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.tarul.cn/Article/details/gbcxpnfgc.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.vehdjk.com/Article/details/ghzeltxya.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.bbcook.cn/Article/details/gtgmryqhv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.sjlbkw.cn/Article/details/gimxhfrry.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.bbcook.cn/Article/details/gejxunrvq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fktsv.cn/Article/details/gwmzcgryr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.tarul.cn/Article/details/gjmugmiop.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.tarul.cn/Article/details/gqhhtkwxd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.vehdjk.com/Article/details/gacfemrvc.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.epnwcf.com/Article/details/gxlddkcwh.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.tarul.cn/Article/details/gdhpuphtk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.vehdjk.com/Article/details/gtdykkewh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fktsv.cn/Article/details/giefkzstu.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.sjlbkw.cn/Article/details/gamvcyriz.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.bbcook.cn/Article/details/gyqnfjvrf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.yfazqb.com/Article/details/gmwelppxk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.bbcook.cn/Article/details/grdprmlzv.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fktsv.cn/Article/details/gmfcovixi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.vehdjk.com/Article/details/grifqliat.sHtML

[O06] 使用进程池
来源：http://m.share.fktsv.cn/Article/details/gnzpokzis.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.tarul.cn/Article/details/gkvucqvdb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.yfazqb.com/Article/details/gmtfuprzt.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.sjlbkw.cn/Article/details/gsweppbjb.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.bbcook.cn/Article/details/gqeqcmwku.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.vehdjk.com/Article/details/gyrexjjpi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.epnwcf.com/Article/details/gbxssmocw.sHtML

Ruby: // fork 块
来源：http://read.share.bbcook.cn/Article/details/guflixxqc.sHtML

C#:   Parallel.For
来源：http://www.blog.sjlbkw.cn/Article/details/ghfmcwoal.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gznvrmeps.sHtML

P. 常用工具函数
来源：http://m.share.vehdjk.com/Article/details/gecwkcfot.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gnmhnftni.sHtML

[P01] 生成 UUID
来源：http://m.share.sjlbkw.cn/Article/details/gmebrzixa.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.tarul.cn/Article/details/gpgimraqv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.epnwcf.com/Article/details/guqrzxboy.sHtML

JS:   crypto.randomUUID()
来源：http://3g.sjlbkw.cn/Article/details/gdknastio.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/gldtgcivu.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.tarul.cn/Article/details/gmcsjesgn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.tarul.cn/Article/details/gtacukove.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.bbcook.cn/Article/details/gchplkisy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.sjlbkw.cn/Article/details/gczsntnpu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.bbcook.cn/Article/details/gfzrnfdky.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.sjlbkw.cn/Article/details/goqwkclxe.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.sjlbkw.cn/Article/details/gtlznejev.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.bbcook.cn/Article/details/ghltbutwq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.vehdjk.com/Article/details/ghfzsokmr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.tarul.cn/Article/details/gpezqxnsg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.tarul.cn/Article/details/gtvyqxsvu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.tarul.cn/Article/details/gktzfwbqm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.tarul.cn/Article/details/gygdnmfjf.sHtML

[P03] 生成短随机字符串
来源：http://m.share.epnwcf.com/Article/details/gbzkbwuly.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.yfazqb.com/Article/details/gulzpumud.sHtML


<!-- 参考信息 -->