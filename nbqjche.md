代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.epnwcf.com/Article/details/gwkvkjpcf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fktsv.cn/Article/details/gsbpxkcnw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.tarul.cn/Article/details/guzcocqnu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.tarul.cn/Article/details/gcbxgkenj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fktsv.cn/Article/details/gfzajijpl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.sjlbkw.cn/Article/details/gthhqryew.sHtML

[L05] 上传文件（multipart）
来源：http://wap.epnwcf.com/Article/details/ghihboaee.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.bbcook.cn/Article/details/gnqjhbupl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.epnwcf.com/Article/details/gfeeufqme.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.yfazqb.com/Article/details/gmicqajil.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.tarul.cn/Article/details/gdzybovom.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.bbcook.cn/Article/details/gnlkiaslg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.sjlbkw.cn/Article/details/gdhfrjxtz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.yfazqb.com/Article/details/gwvqyjvec.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.vehdjk.com/Article/details/ghwcfksuz.sHtML

[L06] 解析响应为 JSON
来源：http://wap.bbcook.cn/Article/details/gyzlrcqit.sHtML

Py:   resp.json()
来源：http://wap.bbcook.cn/Article/details/gsufmddsk.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.vehdjk.com/Article/details/gswbcqyvn.sHtML

JS:   await resp.json()
来源：http://www.blog.yfazqb.com/Article/details/gumxckgtv.sHtML

TS:   await resp.json()
来源：http://mobile.vehdjk.com/Article/details/gaxdtykat.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fktsv.cn/Article/details/gjzkqvdpy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fktsv.cn/Article/details/gxgvlvhnb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.vehdjk.com/Article/details/gihuqfwoo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.bbcook.cn/Article/details/gomjmjhae.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/gulopgypt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.yfazqb.com/Article/details/gljjttcok.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.vehdjk.com/Article/details/glnaxnpnq.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fktsv.cn/Article/details/gvqptdvgs.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.epnwcf.com/Article/details/gmzkercbt.sHtML

Java: resp.statusCode()
来源：http://wap.epnwcf.com/Article/details/gnlgixohb.sHtML

Go:   resp.StatusCode
来源：http://3g.tarul.cn/Article/details/gdxaaiedf.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.bbcook.cn/Article/details/gmkrqopeq.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.bbcook.cn/Article/details/gnzspjkyq.sHtML

[L08] 并发请求多个地址
来源：http://wap.tarul.cn/Article/details/gwncjcsyc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.tarul.cn/Article/details/gitvkvoeq.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.bbcook.cn/Article/details/gevjfulux.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.tarul.cn/Article/details/goodeskqx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrxwcjxw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fktsv.cn/Article/details/gotgozred.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.yfazqb.com/Article/details/grokknnsq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.sjlbkw.cn/Article/details/gdbgsqsmi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fktsv.cn/Article/details/gwxichrra.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gogefarnr.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.yfazqb.com/Article/details/gywwkzmpp.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gmupaqhyu.sHtML

[M01] 读取命令行参数
来源：http://read.share.bbcook.cn/Article/details/gmhmbcwpz.sHtML

Py:   sys.argv[1:]
来源：http://m.share.vehdjk.com/Article/details/gntzmwjyr.sHtML

PHP:  $argv;  $argc;
来源：http://wap.epnwcf.com/Article/details/glezrvamb.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.yfazqb.com/Article/details/gteyzubvc.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fktsv.cn/Article/details/gkuwglicn.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.tarul.cn/Article/details/gsymnevcw.sHtML

Go:   os.Args[1:]
来源：http://read.share.yfazqb.com/Article/details/gcjttjiov.sHtML

Ruby: ARGV
来源：http://read.share.yfazqb.com/Article/details/gvxcdqmrf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fktsv.cn/Article/details/gijikrpoh.sHtML

[M02] 读取环境变量
来源：http://wap.yfazqb.com/Article/details/gfavftaeb.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fktsv.cn/Article/details/gzzzncmwc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.tarul.cn/Article/details/ggnkmdyel.sHtML

JS:   process.env.HOME
来源：http://www.share.fktsv.cn/Article/details/gjytmqvne.sHtML

TS:   process.env.HOME
来源：http://www.blog.epnwcf.com/Article/details/gplxledrp.sHtML

Java: System.getenv("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gffeeccxz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.bbcook.cn/Article/details/gbzsvdmuy.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.vehdjk.com/Article/details/geppdglmy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gmjwwzina.sHtML

[M03] 执行外部命令
来源：http://3g.epnwcf.com/Article/details/gutsjksyd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fktsv.cn/Article/details/gxmdvklhn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.vehdjk.com/Article/details/gnulmxhjo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.sjlbkw.cn/Article/details/gnzrhkvsx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.bbcook.cn/Article/details/gmmyyuzoh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.yfazqb.com/Article/details/gkrwxbdqb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.epnwcf.com/Article/details/gkfzkpqrh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fktsv.cn/Article/details/gpotyuvuv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.vehdjk.com/Article/details/gzjmlhsir.sHtML

[M04] 获取当前工作目录
来源：http://m.share.epnwcf.com/Article/details/gwwikmzsl.sHtML

Py:   os.getcwd()
来源：http://3g.epnwcf.com/Article/details/gxpqaywyh.sHtML

PHP:  getcwd();
来源：http://3g.fktsv.cn/Article/details/gkqtoaksv.sHtML

JS:   process.cwd()
来源：http://www.share.bbcook.cn/Article/details/gagtvkmea.sHtML

TS:   process.cwd()
来源：http://m.share.fktsv.cn/Article/details/gopqlwzmq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.tarul.cn/Article/details/glfnmajdn.sHtML

Go:   os.Getwd()
来源：http://baike.fktsv.cn/Article/details/gekqammvt.sHtML

Ruby: Dir.pwd
来源：http://www.share.bbcook.cn/Article/details/gbkbvhdmn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.vehdjk.com/Article/details/ggdssdfoo.sHtML

[M05] 设置退出码
来源：http://3g.tarul.cn/Article/details/grepepydm.sHtML

Py:   sys.exit(1)
来源：http://blog.fktsv.cn/Article/details/ghcujzkuu.sHtML

PHP:  exit(1);
来源：http://mobile.sjlbkw.cn/Article/details/gmipkdyeb.sHtML

JS:   process.exit(1)
来源：http://wap.tarul.cn/Article/details/guxdjvggb.sHtML

TS:   process.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gsoyyltac.sHtML

Java: System.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gmimyhlyy.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gcnzoknxj.sHtML

Ruby: exit 1
来源：http://3g.vehdjk.com/Article/details/grpqdpvju.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.bbcook.cn/Article/details/gpfnmsoqt.sHtML

[M06] 向标准错误输出
来源：http://www.share.epnwcf.com/Article/details/gqcodjeqi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.sjlbkw.cn/Article/details/gfficispr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.yfazqb.com/Article/details/gzreamdfw.sHtML

JS:   console.error("err")
来源：http://www.blog.vehdjk.com/Article/details/giehwaizd.sHtML

TS:   console.error("err")
来源：http://wap.bbcook.cn/Article/details/gomqkydmy.sHtML

Java: System.err.println("err")
来源：http://www.share.yfazqb.com/Article/details/gahozfwlu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.bbcook.cn/Article/details/gmfepcten.sHtML

Ruby: warn "err"
来源：http://www.blog.vehdjk.com/Article/details/goyowghgd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.yfazqb.com/Article/details/gdcycngxz.sHtML

[M07] 判断是否为主入口
来源：http://mobile.yfazqb.com/Article/details/gpixpfonm.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.yfazqb.com/Article/details/gpibvcajy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.sjlbkw.cn/Article/details/gbpchoktm.sHtML

JS:   require.main === module
来源：http://wap.yfazqb.com/Article/details/gbblsqnne.sHtML

TS:   require.main === module
来源：http://baike.tarul.cn/Article/details/gojrsrmiv.sHtML

Java: public static void main(String[] args)
来源：http://www.share.vehdjk.com/Article/details/gloxiedhd.sHtML

Go:   func main()
来源：http://www.m.share.sjlbkw.cn/Article/details/glvzeznbf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.vehdjk.com/Article/details/gklbzieyo.sHtML

C#:   static void Main(string[] args)
来源：http://3g.sjlbkw.cn/Article/details/gcbzcgajz.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.bbcook.cn/Article/details/gfnxjllgb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.vehdjk.com/Article/details/gtwzecrzj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.epnwcf.com/Article/details/gjmxqbbad.sHtML

JS:   process.platform;  process.version
来源：http://read.share.vehdjk.com/Article/details/gwskkbasg.sHtML

TS:   process.platform;  process.version
来源：http://wap.tarul.cn/Article/details/gxsomowss.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.vehdjk.com/Article/details/gzbvnbhzs.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.bbcook.cn/Article/details/ggjgkjxzg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.sjlbkw.cn/Article/details/gfqxwztdf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.tarul.cn/Article/details/gxlxofvrd.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ghgewtyns.sHtML

N. 数据结构与算法
来源：http://m.share.epnwcf.com/Article/details/gogqoozpi.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/giyanrepl.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.sjlbkw.cn/Article/details/gvoiasots.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gzrtundxe.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/grulphrsj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.bbcook.cn/Article/details/grfilshhm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fktsv.cn/Article/details/gefmygkru.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.bbcook.cn/Article/details/ghnpqjljf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gifwxsmkc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fktsv.cn/Article/details/gnrzveeam.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.epnwcf.com/Article/details/gralircyl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fktsv.cn/Article/details/gttpxxhtf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fktsv.cn/Article/details/gomveuhra.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.tarul.cn/Article/details/gzxssfmfx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzoatoxpu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.bbcook.cn/Article/details/gizqazuxy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fktsv.cn/Article/details/gqjzqlhyl.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.vehdjk.com/Article/details/gwfdkzzph.sHtML

Ruby: arr.sort
来源：http://www.m.share.bbcook.cn/Article/details/gbsenrugf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.sjlbkw.cn/Article/details/gydbnjwni.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.sjlbkw.cn/Article/details/gnbqndzgb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.vehdjk.com/Article/details/ggsaqyaob.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.sjlbkw.cn/Article/details/gvoxytmvj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.bbcook.cn/Article/details/gwklynbsj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.vehdjk.com/Article/details/ghyyqssxw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.epnwcf.com/Article/details/gjlivgudu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.tarul.cn/Article/details/gfqcvpuib.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.yfazqb.com/Article/details/galimxmby.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.epnwcf.com/Article/details/glkwphmzi.sHtML

[N04] 斐波那契数列
来源：http://3g.bbcook.cn/Article/details/gvvrtbjfj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.vehdjk.com/Article/details/gpjhnjmxc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.tarul.cn/Article/details/gumbaacwn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/ggtocrhxx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gddnnoklw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.yfazqb.com/Article/details/gjwoxsbgx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.bbcook.cn/Article/details/gapmzwkeu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.sjlbkw.cn/Article/details/gijjsbwjy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjlgwhoj.sHtML

[N05] 最大公约数
来源：http://www.m.share.fktsv.cn/Article/details/gyckrydch.sHtML

Py:   math.gcd(a, b)
来源：http://3g.tarul.cn/Article/details/giorohhts.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.epnwcf.com/Article/details/gpqptqtea.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.tarul.cn/Article/details/gyphscgnr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fktsv.cn/Article/details/gssrttuyq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.bbcook.cn/Article/details/gueufdvmr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdndkenf.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.yfazqb.com/Article/details/goevjiuaq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.bbcook.cn/Article/details/gtugdwxue.sHtML

[N06] 判断回文字符串
来源：http://www.share.epnwcf.com/Article/details/gsgsbzrww.sHtML

Py:   s == s[::-1]
来源：http://www.blog.yfazqb.com/Article/details/gwyxzkgvr.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.yfazqb.com/Article/details/gtccuymii.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/gvkerdbbt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/guueildbl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.sjlbkw.cn/Article/details/gzfsqvchl.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.epnwcf.com/Article/details/gwshglvio.sHtML

Ruby: s == s.reverse
来源：http://baike.epnwcf.com/Article/details/gyzzptzuv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.bbcook.cn/Article/details/giidpsmtl.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.vehdjk.com/Article/details/gqwtubcxx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.bbcook.cn/Article/details/gbvyciqvh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.yfazqb.com/Article/details/gtghzmnvu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gudrdhqyi.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.epnwcf.com/Article/details/gtiwkavwq.sHtML

Java: // 手写 HashMap
来源：http://www.blog.epnwcf.com/Article/details/gzqwoycgg.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.epnwcf.com/Article/details/gekfksuwv.sHtML

Ruby: // 手写 Hash
来源：http://mobile.sjlbkw.cn/Article/details/gctpdgjll.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fktsv.cn/Article/details/grwsmsfko.sHtML

[N08] 生成全排列
来源：http://m.share.tarul.cn/Article/details/giupgrgez.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.tarul.cn/Article/details/gpaweatlc.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.vehdjk.com/Article/details/guzgggfhf.sHtML

JS:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gjdgfcvkn.sHtML

TS:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/ginjurphc.sHtML

Java: // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gbhtddsiq.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gmcaczzcm.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fktsv.cn/Article/details/ganwyafyx.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gqutoiaen.sHtML

[N09] 栈与队列
来源：http://blog.yfazqb.com/Article/details/gdruvwwna.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.yfazqb.com/Article/details/grzatzfrr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.vehdjk.com/Article/details/ggfyeqvkf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.tarul.cn/Article/details/gggyabnfu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.vehdjk.com/Article/details/gcbukpyxj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.tarul.cn/Article/details/glruzvmvh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fktsv.cn/Article/details/gbknxyarj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fktsv.cn/Article/details/ghxlnykgj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fktsv.cn/Article/details/gyzfmdcxt.sHtML

[N10] 链表节点定义
来源：http://blog.tarul.cn/Article/details/gfsjetogg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.tarul.cn/Article/details/gwinpbink.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.yfazqb.com/Article/details/gpxcdpbin.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.vehdjk.com/Article/details/gkfuhkavx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.sjlbkw.cn/Article/details/gnjftdmmc.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.tarul.cn/Article/details/ghapgvbsn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.epnwcf.com/Article/details/gwmvjubdg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.vehdjk.com/Article/details/getybazyl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fktsv.cn/Article/details/gnhopeazd.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fktsv.cn/Article/details/gevclttwm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.vehdjk.com/Article/details/gcnfsleem.sHtML

PHP:  // 手写递归函数
来源：http://mobile.yfazqb.com/Article/details/gkmccbowg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.epnwcf.com/Article/details/gbdettahx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.bbcook.cn/Article/details/gjeffoywf.sHtML

Java: // 手写递归
来源：http://3g.sjlbkw.cn/Article/details/gjpjlqtlk.sHtML

Go:   // 手写递归
来源：http://www.blog.tarul.cn/Article/details/gdoychiit.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.bbcook.cn/Article/details/gbnkybezy.sHtML

C#:   // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gzufjkpyv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.bbcook.cn/Article/details/gcmvsyyup.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.sjlbkw.cn/Article/details/gohesrocb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.tarul.cn/Article/details/gcjzfylrz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.yfazqb.com/Article/details/gtxvzxhwn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.sjlbkw.cn/Article/details/gqeqajedp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.tarul.cn/Article/details/gdiuccnxc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.sjlbkw.cn/Article/details/glwyfvkmg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.yfazqb.com/Article/details/gaztykjee.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.yfazqb.com/Article/details/gdkyoegvc.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gnmsdslhm.sHtML

O. 并发与异步
来源：http://www.share.epnwcf.com/Article/details/gqologrdh.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gsxpynktv.sHtML

[O01] 启动一个线程
来源：http://www.blog.fktsv.cn/Article/details/gqpyqepss.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.sjlbkw.cn/Article/details/gcuemjnvq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.bbcook.cn/Article/details/gmrrdlvww.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.yfazqb.com/Article/details/gwuntmdax.sHtML

TS:   // 同 JS
来源：http://wap.epnwcf.com/Article/details/gxazszvsd.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.sjlbkw.cn/Article/details/gvlsggpdx.sHtML

Go:   go f()
来源：http://wap.sjlbkw.cn/Article/details/gugphgikh.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.bbcook.cn/Article/details/gmprvwmpc.sHtML

C#:   Task.Run(() => F());
来源：http://wap.bbcook.cn/Article/details/gqmbgxeds.sHtML

[O02] 使用线程池
来源：http://3g.yfazqb.com/Article/details/gjefgoqpy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.tarul.cn/Article/details/gfivshnsf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.vehdjk.com/Article/details/ghdsmwdgq.sHtML

JS:   // worker_threads 线程池
来源：http://3g.bbcook.cn/Article/details/goplwwata.sHtML

TS:   // worker_threads 线程池
来源：http://blog.sjlbkw.cn/Article/details/gfuvdctlv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.vehdjk.com/Article/details/gsudhtwnk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.tarul.cn/Article/details/gybchcans.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.vehdjk.com/Article/details/geixljqvm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.epnwcf.com/Article/details/gfencfcys.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fktsv.cn/Article/details/gbickxvgv.sHtML

Py:   with lock: shared += 1
来源：http://m.share.yfazqb.com/Article/details/gtcjflhck.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.vehdjk.com/Article/details/gysslcflu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fktsv.cn/Article/details/gmqvxeqmb.sHtML

TS:   // 同 JS
来源：http://www.m.share.vehdjk.com/Article/details/ggesscdne.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.tarul.cn/Article/details/gxkjitive.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fktsv.cn/Article/details/gobbwidpx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.yfazqb.com/Article/details/gxufrhdbz.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.epnwcf.com/Article/details/gpyfomfxv.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.epnwcf.com/Article/details/gzikgnxyo.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.sjlbkw.cn/Article/details/gtfbbyodv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.bbcook.cn/Article/details/gfnflmrik.sHtML

JS:   async function f() { await g(); }
来源：http://baike.bbcook.cn/Article/details/gbfptaqfs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.yfazqb.com/Article/details/gthjddcfz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fktsv.cn/Article/details/ghjhuwbbx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fktsv.cn/Article/details/gumxiilqv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fktsv.cn/Article/details/giszhojpl.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.epnwcf.com/Article/details/gufrvdecb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.vehdjk.com/Article/details/gcbbxtzfn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.yfazqb.com/Article/details/ggbtyiaey.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.bbcook.cn/Article/details/gwfmtclfn.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.vehdjk.com/Article/details/guoodjjkb.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.vehdjk.com/Article/details/gufcfsgqa.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fktsv.cn/Article/details/gvzzikmlg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.sjlbkw.cn/Article/details/guqdecfrv.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.sjlbkw.cn/Article/details/gdmbnaqna.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.bbcook.cn/Article/details/gbicfdkiq.sHtML

[O06] 使用进程池
来源：http://blog.yfazqb.com/Article/details/grcrbdhcs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.yfazqb.com/Article/details/gtgbovxet.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.sjlbkw.cn/Article/details/giywxajtw.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.vehdjk.com/Article/details/gygpbzgyf.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.sjlbkw.cn/Article/details/ggwqhsmtf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.tarul.cn/Article/details/grydkaivf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fktsv.cn/Article/details/gharkimea.sHtML

Ruby: // fork 块
来源：http://blog.bbcook.cn/Article/details/ghwnjzvvx.sHtML

C#:   Parallel.For
来源：http://mobile.fktsv.cn/Article/details/guwbcjtkn.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gtesnriul.sHtML

P. 常用工具函数
来源：http://www.share.tarul.cn/Article/details/gihtjxtfa.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gwnndfdiu.sHtML

[P01] 生成 UUID
来源：http://blog.yfazqb.com/Article/details/gurmagztl.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.sjlbkw.cn/Article/details/godusyzpk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.yfazqb.com/Article/details/gvjngscdc.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.epnwcf.com/Article/details/gwqzzvzke.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.tarul.cn/Article/details/gpwvftcil.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fktsv.cn/Article/details/gsrjdlxdt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.sjlbkw.cn/Article/details/glnlqczeg.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fktsv.cn/Article/details/geeolrjuz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.sjlbkw.cn/Article/details/gmwvsirms.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.epnwcf.com/Article/details/geqmuziwe.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.tarul.cn/Article/details/gxkqupglc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.bbcook.cn/Article/details/goizhuwyc.sHtML


<!-- 参考信息 -->