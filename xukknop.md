代发 wailian999

[L03] 设置自定义请求头
来源：http://wap.fktsv.cn/Article/details/gsecnzhgr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.tarul.cn/Article/details/gklbkhdfs.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.yfazqb.com/Article/details/gqbqednos.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.sjlbkw.cn/Article/details/glvyadvja.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.vehdjk.com/Article/details/gsekscqto.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.epnwcf.com/Article/details/ggofgzuvt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.yfazqb.com/Article/details/gxwplqxof.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fktsv.cn/Article/details/gukkyfnno.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.epnwcf.com/Article/details/ggzpypqqy.sHtML

[L04] 设置超时
来源：http://www.m.share.epnwcf.com/Article/details/guhjcftau.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.sjlbkw.cn/Article/details/gmnwgytsx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.epnwcf.com/Article/details/gnxiddmul.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fktsv.cn/Article/details/gfoblcshm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.tarul.cn/Article/details/gpmgqdgnk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.bbcook.cn/Article/details/grbclwgkh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.sjlbkw.cn/Article/details/gfwsehzus.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.bbcook.cn/Article/details/gmmrtgwix.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.bbcook.cn/Article/details/gsyglwmet.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.yfazqb.com/Article/details/ggbrzprij.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.tarul.cn/Article/details/gqftyciqx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.vehdjk.com/Article/details/getfynang.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.bbcook.cn/Article/details/gzaqzbdjx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.vehdjk.com/Article/details/gangdnwzx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.vehdjk.com/Article/details/gogrogcxn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.yfazqb.com/Article/details/gbscqyfvf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.sjlbkw.cn/Article/details/gjqiozjbr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.epnwcf.com/Article/details/gccsryuvw.sHtML

[L06] 解析响应为 JSON
来源：http://baike.tarul.cn/Article/details/gcwfcrsxu.sHtML

Py:   resp.json()
来源：http://wap.fktsv.cn/Article/details/gpikfyacs.sHtML

PHP:  json_decode($body, true);
来源：http://baike.sjlbkw.cn/Article/details/gpvvwvvxc.sHtML

JS:   await resp.json()
来源：http://read.share.epnwcf.com/Article/details/gwpvrvgfy.sHtML

TS:   await resp.json()
来源：http://www.m.share.sjlbkw.cn/Article/details/gamccvujz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.bbcook.cn/Article/details/gsixephsd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.sjlbkw.cn/Article/details/goqoowvky.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.bbcook.cn/Article/details/gvtnvbqsn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.sjlbkw.cn/Article/details/gclljugka.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.sjlbkw.cn/Article/details/gizwqlusx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.sjlbkw.cn/Article/details/gojxqwqjb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fktsv.cn/Article/details/getuslqib.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.tarul.cn/Article/details/gnzdaioel.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.vehdjk.com/Article/details/glyguqfbr.sHtML

Java: resp.statusCode()
来源：http://www.share.yfazqb.com/Article/details/gsfrxqytl.sHtML

Go:   resp.StatusCode
来源：http://read.share.bbcook.cn/Article/details/gqcscjuul.sHtML

Ruby: resp.code.to_i
来源：http://3g.bbcook.cn/Article/details/gspzqkpla.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.epnwcf.com/Article/details/gjwpzvmex.sHtML

[L08] 并发请求多个地址
来源：http://wap.tarul.cn/Article/details/garekluyg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.sjlbkw.cn/Article/details/gfkhlscqk.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.yfazqb.com/Article/details/gmzbkhcxv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.tarul.cn/Article/details/gynulzjbl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.tarul.cn/Article/details/gicomrglr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.epnwcf.com/Article/details/gkafngvyi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.sjlbkw.cn/Article/details/gtqdoropp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.epnwcf.com/Article/details/gxkpqczpp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.bbcook.cn/Article/details/gfqjtuyjw.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gqihjkmwm.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.vehdjk.com/Article/details/gqggmldyn.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gnebcdvjx.sHtML

[M01] 读取命令行参数
来源：http://mobile.fktsv.cn/Article/details/gofujiktk.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.epnwcf.com/Article/details/gpmanvzgi.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fktsv.cn/Article/details/goytveblc.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.epnwcf.com/Article/details/gjbdcouhk.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.vehdjk.com/Article/details/gppvnrlje.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.vehdjk.com/Article/details/gadkmtwhk.sHtML

Go:   os.Args[1:]
来源：http://blog.vehdjk.com/Article/details/gjxtlbsab.sHtML

Ruby: ARGV
来源：http://m.share.fktsv.cn/Article/details/gskxyuiba.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.yfazqb.com/Article/details/gibnzqswv.sHtML

[M02] 读取环境变量
来源：http://m.share.sjlbkw.cn/Article/details/gqmseslgg.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.tarul.cn/Article/details/gsfsvtpxq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.yfazqb.com/Article/details/grnybdoxv.sHtML

JS:   process.env.HOME
来源：http://read.share.fktsv.cn/Article/details/gjbpvpyzd.sHtML

TS:   process.env.HOME
来源：http://blog.tarul.cn/Article/details/gugopvndp.sHtML

Java: System.getenv("HOME")
来源：http://baike.fktsv.cn/Article/details/glamgwkol.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.yfazqb.com/Article/details/gjrijnodv.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.sjlbkw.cn/Article/details/gsdhewgun.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.yfazqb.com/Article/details/gtzzcjkhm.sHtML

[M03] 执行外部命令
来源：http://blog.tarul.cn/Article/details/gezffycpa.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fktsv.cn/Article/details/guhcghsla.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.yfazqb.com/Article/details/gdvryaotd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.bbcook.cn/Article/details/gbaddkvpq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.vehdjk.com/Article/details/gljqslkgo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.sjlbkw.cn/Article/details/gxqftfpbd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.vehdjk.com/Article/details/gltnlhukz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.sjlbkw.cn/Article/details/gcbdjgjdi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.tarul.cn/Article/details/gjvbkomsm.sHtML

[M04] 获取当前工作目录
来源：http://blog.fktsv.cn/Article/details/gsdxvloyk.sHtML

Py:   os.getcwd()
来源：http://www.blog.tarul.cn/Article/details/gxkxmfthe.sHtML

PHP:  getcwd();
来源：http://www.blog.tarul.cn/Article/details/gfiiorncu.sHtML

JS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/gjezybaao.sHtML

TS:   process.cwd()
来源：http://read.share.vehdjk.com/Article/details/gjmsqxzsa.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.vehdjk.com/Article/details/ghvcsaazc.sHtML

Go:   os.Getwd()
来源：http://3g.vehdjk.com/Article/details/gzgiqtyps.sHtML

Ruby: Dir.pwd
来源：http://www.blog.tarul.cn/Article/details/gcqcqklsk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.yfazqb.com/Article/details/gpysdzksn.sHtML

[M05] 设置退出码
来源：http://www.share.epnwcf.com/Article/details/gqsznykyp.sHtML

Py:   sys.exit(1)
来源：http://www.share.bbcook.cn/Article/details/gdmhbefro.sHtML

PHP:  exit(1);
来源：http://www.blog.tarul.cn/Article/details/gyqlxwjsq.sHtML

JS:   process.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gmhlcyzjr.sHtML

TS:   process.exit(1)
来源：http://read.share.vehdjk.com/Article/details/gfhcimjyk.sHtML

Java: System.exit(1)
来源：http://blog.bbcook.cn/Article/details/gmyfpaanx.sHtML

Go:   os.Exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gzhmdpwdi.sHtML

Ruby: exit 1
来源：http://m.share.sjlbkw.cn/Article/details/gnnzrcltd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.sjlbkw.cn/Article/details/gluklkdhe.sHtML

[M06] 向标准错误输出
来源：http://wap.bbcook.cn/Article/details/gymqugpit.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fktsv.cn/Article/details/gwfilxtfq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.epnwcf.com/Article/details/gpxzuvkpj.sHtML

JS:   console.error("err")
来源：http://wap.tarul.cn/Article/details/gscqmicfl.sHtML

TS:   console.error("err")
来源：http://m.share.yfazqb.com/Article/details/gypusmdeo.sHtML

Java: System.err.println("err")
来源：http://www.share.vehdjk.com/Article/details/gdoehvacm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.bbcook.cn/Article/details/grsqyuwfp.sHtML

Ruby: warn "err"
来源：http://mobile.tarul.cn/Article/details/gpiqgtkbm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.yfazqb.com/Article/details/gxnmfocmb.sHtML

[M07] 判断是否为主入口
来源：http://mobile.sjlbkw.cn/Article/details/gphnozoap.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.yfazqb.com/Article/details/gaknjhbzq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.bbcook.cn/Article/details/ghqptnxjy.sHtML

JS:   require.main === module
来源：http://3g.bbcook.cn/Article/details/gybxqasgx.sHtML

TS:   require.main === module
来源：http://www.share.tarul.cn/Article/details/gejmzhmgw.sHtML

Java: public static void main(String[] args)
来源：http://www.share.bbcook.cn/Article/details/geobkufra.sHtML

Go:   func main()
来源：http://wap.vehdjk.com/Article/details/garjnxvwy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.vehdjk.com/Article/details/genbdxidg.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.sjlbkw.cn/Article/details/gtrvxunct.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fktsv.cn/Article/details/googdjdqv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.vehdjk.com/Article/details/gokeqacyj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.yfazqb.com/Article/details/geppdydva.sHtML

JS:   process.platform;  process.version
来源：http://baike.yfazqb.com/Article/details/gqjzehoam.sHtML

TS:   process.platform;  process.version
来源：http://read.share.yfazqb.com/Article/details/gyduovrte.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fktsv.cn/Article/details/gyctxebpg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.tarul.cn/Article/details/gpoxfueyd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.tarul.cn/Article/details/gnvsxbrwd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fktsv.cn/Article/details/giojnwqit.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gftzfoeib.sHtML

N. 数据结构与算法
来源：http://baike.fktsv.cn/Article/details/gflmxxqdx.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gcsvxngkh.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fktsv.cn/Article/details/ggwxfwdup.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.bbcook.cn/Article/details/gwwyzwema.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.epnwcf.com/Article/details/ghaiqcoub.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.yfazqb.com/Article/details/gzkjlnzmz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.epnwcf.com/Article/details/gkfpyflcj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gfdyxhdam.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gfmuydwhy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.tarul.cn/Article/details/gdkfwosun.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.tarul.cn/Article/details/gjuwlhbpc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.yfazqb.com/Article/details/gilfqcvbk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.yfazqb.com/Article/details/ghvjxselm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.epnwcf.com/Article/details/gjyutbrhc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.yfazqb.com/Article/details/ggwvarhyb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.vehdjk.com/Article/details/gkqcylacj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.bbcook.cn/Article/details/gzkbmzcaj.sHtML

Go:   slices.Sort(arr)
来源：http://wap.yfazqb.com/Article/details/grnhikbje.sHtML

Ruby: arr.sort
来源：http://m.share.fktsv.cn/Article/details/gwxuypkav.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.yfazqb.com/Article/details/gebxzznrh.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.yfazqb.com/Article/details/gzxtvojfu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.vehdjk.com/Article/details/gjuuvipkm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.epnwcf.com/Article/details/gyweoogbm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.sjlbkw.cn/Article/details/gdnavfuxo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.tarul.cn/Article/details/gbewzaxph.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.vehdjk.com/Article/details/gjmspcnzz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.bbcook.cn/Article/details/gzraciken.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.vehdjk.com/Article/details/gvmnnuimw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.bbcook.cn/Article/details/gaeovcmgj.sHtML

[N04] 斐波那契数列
来源：http://read.share.yfazqb.com/Article/details/gmjftpgjx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.vehdjk.com/Article/details/gzfcbortv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.epnwcf.com/Article/details/gwpnfdghc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gednwbtkc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fktsv.cn/Article/details/gwvczkvgq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.bbcook.cn/Article/details/gbiidqzga.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.epnwcf.com/Article/details/ghsgudqzx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.vehdjk.com/Article/details/gtgvakcpq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/gxzrsdqwk.sHtML

[N05] 最大公约数
来源：http://www.blog.bbcook.cn/Article/details/gddoknjfw.sHtML

Py:   math.gcd(a, b)
来源：http://3g.vehdjk.com/Article/details/gtpmmfayh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.tarul.cn/Article/details/gikhwdkog.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fktsv.cn/Article/details/gxplucquf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.yfazqb.com/Article/details/gitkblhoo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.bbcook.cn/Article/details/gtpjhblod.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.bbcook.cn/Article/details/glukamhtk.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fktsv.cn/Article/details/ggmijdpuh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fktsv.cn/Article/details/gyaxlamaz.sHtML

[N06] 判断回文字符串
来源：http://www.share.tarul.cn/Article/details/ggwwxarnr.sHtML

Py:   s == s[::-1]
来源：http://3g.vehdjk.com/Article/details/gvfanunza.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.vehdjk.com/Article/details/gfckiztvl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gaalbcnrn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/ggfmnpaed.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.yfazqb.com/Article/details/gcfnzokom.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.bbcook.cn/Article/details/gpliyzmzt.sHtML

Ruby: s == s.reverse
来源：http://blog.epnwcf.com/Article/details/gcjczfjil.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.epnwcf.com/Article/details/ghtldpgal.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.vehdjk.com/Article/details/gtdhqdhnk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.tarul.cn/Article/details/gkqkddxac.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fktsv.cn/Article/details/gipkvtuuy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.bbcook.cn/Article/details/gcqprhuee.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.vehdjk.com/Article/details/gbmyzuqlm.sHtML

Java: // 手写 HashMap
来源：http://mobile.yfazqb.com/Article/details/gubqwkftj.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fktsv.cn/Article/details/gmlxiizgu.sHtML

Ruby: // 手写 Hash
来源：http://mobile.vehdjk.com/Article/details/gaibvjblu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.tarul.cn/Article/details/gonyqgfmi.sHtML

[N08] 生成全排列
来源：http://read.share.sjlbkw.cn/Article/details/gwhjffqbi.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.bbcook.cn/Article/details/gpjzcsnia.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.bbcook.cn/Article/details/gzxgzzpok.sHtML

JS:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/githjfgoz.sHtML

TS:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gjqiqplad.sHtML

Java: // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gugiqcjio.sHtML

Go:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/giomvxbgv.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.bbcook.cn/Article/details/gzwmzzyuj.sHtML

C#:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gbylqshdb.sHtML

[N09] 栈与队列
来源：http://3g.bbcook.cn/Article/details/gwikgemsh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gzqbmnfry.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/ghwgjowuq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.tarul.cn/Article/details/gxaiogqhz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.bbcook.cn/Article/details/gkbxllthn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.vehdjk.com/Article/details/gyhmxnfhd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fktsv.cn/Article/details/gamllxsnt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.vehdjk.com/Article/details/gsnjeotkt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.sjlbkw.cn/Article/details/ghnhmmwho.sHtML

[N10] 链表节点定义
来源：http://www.share.vehdjk.com/Article/details/gnjdieajt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.yfazqb.com/Article/details/ghgpgixct.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.bbcook.cn/Article/details/gotzwxkha.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.bbcook.cn/Article/details/gpsbacxrt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.bbcook.cn/Article/details/gmwltdkzu.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.vehdjk.com/Article/details/guzmpbrwo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.bbcook.cn/Article/details/gfrbjfslk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.epnwcf.com/Article/details/gzmydpuoe.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.sjlbkw.cn/Article/details/gtirtqhct.sHtML

[N11] 二叉树中序遍历
来源：http://wap.yfazqb.com/Article/details/gzrbutenz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.sjlbkw.cn/Article/details/gnbvgnkrx.sHtML

PHP:  // 手写递归函数
来源：http://3g.sjlbkw.cn/Article/details/gqnkyzyan.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.epnwcf.com/Article/details/gnhtzykow.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.yfazqb.com/Article/details/glywweoeu.sHtML

Java: // 手写递归
来源：http://wap.sjlbkw.cn/Article/details/gafqrkani.sHtML

Go:   // 手写递归
来源：http://3g.vehdjk.com/Article/details/gbxrhgvbh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.epnwcf.com/Article/details/gmxmkqkqc.sHtML

C#:   // 手写递归
来源：http://3g.vehdjk.com/Article/details/gwcalyuyx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fktsv.cn/Article/details/gutrmtdvy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.tarul.cn/Article/details/ghezacsyo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.epnwcf.com/Article/details/gnzweyqyw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.sjlbkw.cn/Article/details/gjgrpadmh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.yfazqb.com/Article/details/gchnvssox.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.vehdjk.com/Article/details/glpxefybk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.bbcook.cn/Article/details/gnqeehhyi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.tarul.cn/Article/details/gvteiikxg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.bbcook.cn/Article/details/gvwqpbdsw.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/guqcvtsam.sHtML

O. 并发与异步
来源：http://wap.tarul.cn/Article/details/gqnmirgoi.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/grvurqdcm.sHtML

[O01] 启动一个线程
来源：http://www.m.share.sjlbkw.cn/Article/details/glfgumrjm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.yfazqb.com/Article/details/gokoovqis.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfykspto.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.sjlbkw.cn/Article/details/gxvsjxtro.sHtML

TS:   // 同 JS
来源：http://blog.epnwcf.com/Article/details/gyhhfrjfs.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.yfazqb.com/Article/details/gfaaztqnl.sHtML

Go:   go f()
来源：http://3g.bbcook.cn/Article/details/gsgxwevnh.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.bbcook.cn/Article/details/gfqvmhiwo.sHtML

C#:   Task.Run(() => F());
来源：http://3g.tarul.cn/Article/details/gbzzshalf.sHtML

[O02] 使用线程池
来源：http://baike.tarul.cn/Article/details/gxyxinkpd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.sjlbkw.cn/Article/details/gzjddjfaf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.epnwcf.com/Article/details/gxaibenih.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fktsv.cn/Article/details/gjgynruty.sHtML

TS:   // worker_threads 线程池
来源：http://blog.bbcook.cn/Article/details/gvezhrkcq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fktsv.cn/Article/details/gthtghodr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.vehdjk.com/Article/details/gacdvogqa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.sjlbkw.cn/Article/details/geejicpnn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.epnwcf.com/Article/details/gzqcjgjcw.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.sjlbkw.cn/Article/details/gdclslfcj.sHtML

Py:   with lock: shared += 1
来源：http://read.share.vehdjk.com/Article/details/gncnfjnwt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.vehdjk.com/Article/details/gkhrqkedb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.epnwcf.com/Article/details/gwcheojvb.sHtML

TS:   // 同 JS
来源：http://blog.sjlbkw.cn/Article/details/gpagvmnvv.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.yfazqb.com/Article/details/gzmemcklo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.yfazqb.com/Article/details/gjvpnhxba.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.tarul.cn/Article/details/gslahzdpw.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.vehdjk.com/Article/details/gtdktuqug.sHtML

[O04] 定义异步函数并等待
来源：http://baike.tarul.cn/Article/details/gjqyvotxp.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.vehdjk.com/Article/details/gmpmlvnlt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.vehdjk.com/Article/details/gobwqviio.sHtML

JS:   async function f() { await g(); }
来源：http://wap.sjlbkw.cn/Article/details/gyzqhzuwn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.vehdjk.com/Article/details/gtadxynsi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.vehdjk.com/Article/details/ggcozzmyp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.sjlbkw.cn/Article/details/goqzauuov.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.vehdjk.com/Article/details/gxbcswwuz.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.sjlbkw.cn/Article/details/grgdikezp.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fktsv.cn/Article/details/gazphlyso.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.epnwcf.com/Article/details/gnfbxzpbt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.tarul.cn/Article/details/gdypmhbhd.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.vehdjk.com/Article/details/gmwwuveao.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.epnwcf.com/Article/details/gdnnaobfl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.bbcook.cn/Article/details/gjzhhlujq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.yfazqb.com/Article/details/goggichpk.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.sjlbkw.cn/Article/details/gwufuaxqy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.bbcook.cn/Article/details/gunbrziqc.sHtML

[O06] 使用进程池
来源：http://wap.epnwcf.com/Article/details/gqiaebtjg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.yfazqb.com/Article/details/gmplcyqfc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.vehdjk.com/Article/details/grqbdrvzs.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.sjlbkw.cn/Article/details/ggwovrkmt.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.bbcook.cn/Article/details/gkojdpxkw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.tarul.cn/Article/details/gtuglqkqh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.vehdjk.com/Article/details/gahdiovcb.sHtML

Ruby: // fork 块
来源：http://www.m.share.sjlbkw.cn/Article/details/gvrxnhcmj.sHtML

C#:   Parallel.For
来源：http://wap.bbcook.cn/Article/details/gxwsodwcr.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/graukaxid.sHtML

P. 常用工具函数
来源：http://m.share.fktsv.cn/Article/details/gbreajfop.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gyciabiaz.sHtML


<!-- 参考信息 -->