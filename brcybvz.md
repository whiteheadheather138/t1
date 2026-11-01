代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://blog.bbcook.cn/Article/details/gnfctobhb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.sjlbkw.cn/Article/details/getgdkxoe.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.tarul.cn/Article/details/gaddbuvew.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.tarul.cn/Article/details/gowomtfqc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.sjlbkw.cn/Article/details/gapebcapc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.sjlbkw.cn/Article/details/gvbwobapk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.tarul.cn/Article/details/gkghcwkbm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.sjlbkw.cn/Article/details/gsrbmbcqa.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fktsv.cn/Article/details/gabyhtdqv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fktsv.cn/Article/details/gdqewaqcm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.vehdjk.com/Article/details/gbtljohiw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.bbcook.cn/Article/details/gpnebnwqx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fktsv.cn/Article/details/glewyxtdj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.bbcook.cn/Article/details/gdbovpdxa.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.bbcook.cn/Article/details/gophhrsag.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.vehdjk.com/Article/details/gvfjadxtz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.bbcook.cn/Article/details/gguvdlooc.sHtML

[L04] 设置超时
来源：http://mobile.epnwcf.com/Article/details/ginhyffzf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.yfazqb.com/Article/details/gaycxbpin.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fktsv.cn/Article/details/ggwfunryb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.epnwcf.com/Article/details/gzdkcaeif.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.sjlbkw.cn/Article/details/gljfpydcj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.vehdjk.com/Article/details/gptaaihcn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.yfazqb.com/Article/details/gbswhcgwy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.epnwcf.com/Article/details/grlrmwmfl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.yfazqb.com/Article/details/gokphqdyg.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fktsv.cn/Article/details/gkzztrmwv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.tarul.cn/Article/details/gjjlcvtrm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.bbcook.cn/Article/details/gcmowxyga.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fktsv.cn/Article/details/gpoulasmd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.yfazqb.com/Article/details/gffduudus.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fktsv.cn/Article/details/geybhhncy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.vehdjk.com/Article/details/gztvvunjc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fktsv.cn/Article/details/ggftayluh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.vehdjk.com/Article/details/grfhgezso.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.tarul.cn/Article/details/gmxkweerz.sHtML

Py:   resp.json()
来源：http://www.blog.tarul.cn/Article/details/gwrzahliv.sHtML

PHP:  json_decode($body, true);
来源：http://3g.epnwcf.com/Article/details/gksembqom.sHtML

JS:   await resp.json()
来源：http://www.blog.fktsv.cn/Article/details/gryjxvlcc.sHtML

TS:   await resp.json()
来源：http://wap.vehdjk.com/Article/details/gkdxoumqp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.tarul.cn/Article/details/guikvtnry.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.epnwcf.com/Article/details/gdoifmggy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.epnwcf.com/Article/details/gwbxsynqy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.yfazqb.com/Article/details/grophfzxy.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.epnwcf.com/Article/details/gqypknnns.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fktsv.cn/Article/details/gtwkamybw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.sjlbkw.cn/Article/details/ghcdsjfuw.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.yfazqb.com/Article/details/ggqrcmulf.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.tarul.cn/Article/details/gmnemiaum.sHtML

Java: resp.statusCode()
来源：http://www.m.share.bbcook.cn/Article/details/gmikhnvnk.sHtML

Go:   resp.StatusCode
来源：http://baike.vehdjk.com/Article/details/gfbhylkhg.sHtML

Ruby: resp.code.to_i
来源：http://3g.sjlbkw.cn/Article/details/guifopzay.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.tarul.cn/Article/details/grfrijckt.sHtML

[L08] 并发请求多个地址
来源：http://blog.fktsv.cn/Article/details/gwxcnkaiu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fktsv.cn/Article/details/gkadbuqmx.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.yfazqb.com/Article/details/gvgwdmcnx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gwgoonbuy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.vehdjk.com/Article/details/gyxzbddaa.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.tarul.cn/Article/details/guiydugju.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.yfazqb.com/Article/details/grryckbmd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.epnwcf.com/Article/details/gcpzfptzd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fktsv.cn/Article/details/guwtlaaeg.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gihndxxjl.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.tarul.cn/Article/details/gyjfqrzor.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gfevvhcia.sHtML

[M01] 读取命令行参数
来源：http://wap.bbcook.cn/Article/details/gegtlmvgy.sHtML

Py:   sys.argv[1:]
来源：http://blog.sjlbkw.cn/Article/details/gvmikxtey.sHtML

PHP:  $argv;  $argc;
来源：http://3g.sjlbkw.cn/Article/details/gjgzijgvc.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fktsv.cn/Article/details/gwjkstoak.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.yfazqb.com/Article/details/gkwxwjdlw.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fktsv.cn/Article/details/gfxiuvdwo.sHtML

Go:   os.Args[1:]
来源：http://read.share.bbcook.cn/Article/details/gjxlbmhty.sHtML

Ruby: ARGV
来源：http://mobile.epnwcf.com/Article/details/gpvtdczey.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.yfazqb.com/Article/details/gqlhihhgw.sHtML

[M02] 读取环境变量
来源：http://www.m.share.vehdjk.com/Article/details/gqbfzsuwp.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.yfazqb.com/Article/details/gqxpejzno.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.yfazqb.com/Article/details/gnnbhlhqw.sHtML

JS:   process.env.HOME
来源：http://m.share.fktsv.cn/Article/details/gjpkpqlbk.sHtML

TS:   process.env.HOME
来源：http://blog.epnwcf.com/Article/details/gcoskbald.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gqbdrzdaq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.vehdjk.com/Article/details/gtgstdsmb.sHtML

Ruby: ENV["HOME"]
来源：http://wap.epnwcf.com/Article/details/gzsxeiskc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.yfazqb.com/Article/details/giosquomt.sHtML

[M03] 执行外部命令
来源：http://read.share.fktsv.cn/Article/details/gahgeerxl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.vehdjk.com/Article/details/gjxfphzju.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.bbcook.cn/Article/details/gvxplzgor.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.yfazqb.com/Article/details/gfcchovjh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fktsv.cn/Article/details/gaiwsbkee.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.sjlbkw.cn/Article/details/ghiweojte.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjyfntma.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.tarul.cn/Article/details/gjnvhwoyz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.vehdjk.com/Article/details/gdjwheavl.sHtML

[M04] 获取当前工作目录
来源：http://read.share.bbcook.cn/Article/details/gibljzade.sHtML

Py:   os.getcwd()
来源：http://baike.vehdjk.com/Article/details/gkfskwpnp.sHtML

PHP:  getcwd();
来源：http://m.share.epnwcf.com/Article/details/gqchmtqok.sHtML

JS:   process.cwd()
来源：http://read.share.sjlbkw.cn/Article/details/grmdmbqqs.sHtML

TS:   process.cwd()
来源：http://www.m.share.epnwcf.com/Article/details/grpiakoyb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.yfazqb.com/Article/details/gauyqfmhv.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fktsv.cn/Article/details/gvotfmkio.sHtML

Ruby: Dir.pwd
来源：http://mobile.bbcook.cn/Article/details/grkvjokxq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.sjlbkw.cn/Article/details/gczhtjwws.sHtML

[M05] 设置退出码
来源：http://mobile.yfazqb.com/Article/details/gznroaide.sHtML

Py:   sys.exit(1)
来源：http://www.share.fktsv.cn/Article/details/grwpszwoy.sHtML

PHP:  exit(1);
来源：http://wap.tarul.cn/Article/details/gqylygcas.sHtML

JS:   process.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/grufnmdzb.sHtML

TS:   process.exit(1)
来源：http://baike.bbcook.cn/Article/details/goczxyeug.sHtML

Java: System.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gqlruojjf.sHtML

Go:   os.Exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gqmhxsrff.sHtML

Ruby: exit 1
来源：http://m.share.bbcook.cn/Article/details/gczzgfpvw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.epnwcf.com/Article/details/gnomnuagt.sHtML

[M06] 向标准错误输出
来源：http://www.share.epnwcf.com/Article/details/gmzwpalog.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.bbcook.cn/Article/details/gnfzxwyxa.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.tarul.cn/Article/details/gtcvgzmfq.sHtML

JS:   console.error("err")
来源：http://wap.sjlbkw.cn/Article/details/gbpnsouyz.sHtML

TS:   console.error("err")
来源：http://baike.vehdjk.com/Article/details/gjjqmjihn.sHtML

Java: System.err.println("err")
来源：http://www.m.share.bbcook.cn/Article/details/giwamjrok.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.yfazqb.com/Article/details/gpcasuijb.sHtML

Ruby: warn "err"
来源：http://mobile.sjlbkw.cn/Article/details/gsmbwlemk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.yfazqb.com/Article/details/gxpkqfpwg.sHtML

[M07] 判断是否为主入口
来源：http://mobile.epnwcf.com/Article/details/gzxkwgyxg.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.epnwcf.com/Article/details/gydloggif.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.sjlbkw.cn/Article/details/ghwbesowc.sHtML

JS:   require.main === module
来源：http://baike.tarul.cn/Article/details/gndsnoxeu.sHtML

TS:   require.main === module
来源：http://3g.vehdjk.com/Article/details/gqopxrwom.sHtML

Java: public static void main(String[] args)
来源：http://wap.fktsv.cn/Article/details/gmmqrumwf.sHtML

Go:   func main()
来源：http://baike.bbcook.cn/Article/details/gdxmojktw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.vehdjk.com/Article/details/gfipcapku.sHtML

C#:   static void Main(string[] args)
来源：http://wap.vehdjk.com/Article/details/gfxdorwun.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.sjlbkw.cn/Article/details/gmlpiptno.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.vehdjk.com/Article/details/gbdxpjupd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.epnwcf.com/Article/details/guyrewmgc.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fktsv.cn/Article/details/gdzvvalwb.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/gtirfosbr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.vehdjk.com/Article/details/gswadugnt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.yfazqb.com/Article/details/gxndfdpcr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.yfazqb.com/Article/details/gbjgxnrsp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.bbcook.cn/Article/details/gqjrhmvmf.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gwmrkvuro.sHtML

N. 数据结构与算法
来源：http://baike.tarul.cn/Article/details/gffobbqgz.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/ghiumhjbk.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.bbcook.cn/Article/details/gopqknxck.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gzsmfibsa.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.bbcook.cn/Article/details/gcjuhgohd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.bbcook.cn/Article/details/grzpbubye.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.tarul.cn/Article/details/guqclwneh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gidcyyurq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.bbcook.cn/Article/details/gdzxyzpan.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.tarul.cn/Article/details/gcwirbvdf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fktsv.cn/Article/details/gbqpdijrn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.tarul.cn/Article/details/gxmpigpjz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.tarul.cn/Article/details/geudboqov.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.epnwcf.com/Article/details/gbovozcws.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.epnwcf.com/Article/details/gntvlfcus.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/gsbaefzol.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.sjlbkw.cn/Article/details/ggsgyyons.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrjskecn.sHtML

Ruby: arr.sort
来源：http://www.m.share.bbcook.cn/Article/details/gmdtushhb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.bbcook.cn/Article/details/gupbmifmi.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.tarul.cn/Article/details/gveudomkc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.yfazqb.com/Article/details/gofwnwddi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.vehdjk.com/Article/details/gnjjbbmpr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fktsv.cn/Article/details/gmoocycrm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.epnwcf.com/Article/details/gitnwdauf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.sjlbkw.cn/Article/details/genpzxyfa.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.yfazqb.com/Article/details/glolfxcda.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.sjlbkw.cn/Article/details/gtzfutxpe.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.epnwcf.com/Article/details/gdxyvivoy.sHtML

[N04] 斐波那契数列
来源：http://m.share.fktsv.cn/Article/details/gixokkizg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.epnwcf.com/Article/details/gmuclsnot.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.yfazqb.com/Article/details/ghgukesxt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.bbcook.cn/Article/details/gjnyujvor.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.yfazqb.com/Article/details/ggtfwdizf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.vehdjk.com/Article/details/gjxyqfpte.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.vehdjk.com/Article/details/gbiodhqhv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.vehdjk.com/Article/details/gleeqisyz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gmmnpczro.sHtML

[N05] 最大公约数
来源：http://mobile.fktsv.cn/Article/details/gddqadrlm.sHtML

Py:   math.gcd(a, b)
来源：http://baike.sjlbkw.cn/Article/details/gkeanpfga.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.yfazqb.com/Article/details/glwlpzdvi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.bbcook.cn/Article/details/guatoprlf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.yfazqb.com/Article/details/gxmteecmv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.yfazqb.com/Article/details/gvtrzqabx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.sjlbkw.cn/Article/details/gimjcftiz.sHtML

Ruby: a.gcd(b)
来源：http://3g.tarul.cn/Article/details/geaypbdae.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.vehdjk.com/Article/details/gmbqdcsit.sHtML

[N06] 判断回文字符串
来源：http://read.share.bbcook.cn/Article/details/gslzujjle.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.tarul.cn/Article/details/gdrmtyxvm.sHtML

PHP:  $s === strrev($s);
来源：http://blog.sjlbkw.cn/Article/details/gwgbvwckc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gtdhzlhnj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/gxwyslcjb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.tarul.cn/Article/details/gmureoems.sHtML

Go:   // 双指针从两端比较
来源：http://baike.bbcook.cn/Article/details/gmqoxciuz.sHtML

Ruby: s == s.reverse
来源：http://baike.epnwcf.com/Article/details/gwzomaper.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.epnwcf.com/Article/details/gvpcmbyvg.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.yfazqb.com/Article/details/gmtxmqysy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.tarul.cn/Article/details/gpxsczwju.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.epnwcf.com/Article/details/gcpwdrjsy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.bbcook.cn/Article/details/gzxkcqbjn.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.vehdjk.com/Article/details/gxjqtjxxk.sHtML

Java: // 手写 HashMap
来源：http://www.share.bbcook.cn/Article/details/gzqchrvuf.sHtML

Go:   // 手写 map[int]int
来源：http://baike.vehdjk.com/Article/details/gueswxctf.sHtML

Ruby: // 手写 Hash
来源：http://wap.yfazqb.com/Article/details/ghegifgxa.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.sjlbkw.cn/Article/details/gapcljszf.sHtML

[N08] 生成全排列
来源：http://wap.bbcook.cn/Article/details/gvdsblobh.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fktsv.cn/Article/details/gztkcqyeu.sHtML

PHP:  // 手写递归交换
来源：http://m.share.vehdjk.com/Article/details/ggzdycuww.sHtML

JS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gsaslauea.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gtkhzzmyp.sHtML

Java: // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/giqjbidfw.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gnofxfexy.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.yfazqb.com/Article/details/gtndhfanh.sHtML

C#:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gonzxhkuj.sHtML

[N09] 栈与队列
来源：http://baike.sjlbkw.cn/Article/details/gucoyqqge.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.epnwcf.com/Article/details/gqkabmvtp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.yfazqb.com/Article/details/ghrjfprrp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.vehdjk.com/Article/details/gspyjnped.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.tarul.cn/Article/details/gatrpdupa.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.yfazqb.com/Article/details/ginvcmbvl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.epnwcf.com/Article/details/gqisybwgd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gjbbnspjc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.tarul.cn/Article/details/goushaick.sHtML

[N10] 链表节点定义
来源：http://m.share.epnwcf.com/Article/details/gmmkklilc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fktsv.cn/Article/details/gbduimxij.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.yfazqb.com/Article/details/gpocooltv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.vehdjk.com/Article/details/gtzytmxem.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.tarul.cn/Article/details/ghazgyfug.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.epnwcf.com/Article/details/gjikqitnq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.tarul.cn/Article/details/gykfogtjc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.tarul.cn/Article/details/gingafagn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.bbcook.cn/Article/details/gtpmqqtzs.sHtML

[N11] 二叉树中序遍历
来源：http://3g.yfazqb.com/Article/details/ghkgeiuma.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.vehdjk.com/Article/details/giwxgwrfh.sHtML

PHP:  // 手写递归函数
来源：http://mobile.bbcook.cn/Article/details/gmknkybmq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.bbcook.cn/Article/details/gdpfdamde.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.epnwcf.com/Article/details/gidkchzkg.sHtML

Java: // 手写递归
来源：http://www.blog.epnwcf.com/Article/details/gjhdzomsp.sHtML

Go:   // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/glrkznhqg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.vehdjk.com/Article/details/gfrepusnn.sHtML

C#:   // 手写递归
来源：http://wap.sjlbkw.cn/Article/details/gdvxafysw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.vehdjk.com/Article/details/gwyulkgbd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.yfazqb.com/Article/details/gpyvyxccp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fktsv.cn/Article/details/gwmprlxtj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.epnwcf.com/Article/details/gvgekqlhr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.vehdjk.com/Article/details/gtbqktics.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.sjlbkw.cn/Article/details/gsvdrlljy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.yfazqb.com/Article/details/gulyeaenx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.sjlbkw.cn/Article/details/gpqprgxzk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fktsv.cn/Article/details/guszseddr.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gsnvqtjmc.sHtML

O. 并发与异步
来源：http://m.share.vehdjk.com/Article/details/grdnalyre.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gmedfhfko.sHtML

[O01] 启动一个线程
来源：http://m.share.yfazqb.com/Article/details/glmwdxiqf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.vehdjk.com/Article/details/gtbkahucq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.bbcook.cn/Article/details/gmoroxmmm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.sjlbkw.cn/Article/details/gwidhmoqb.sHtML

TS:   // 同 JS
来源：http://mobile.bbcook.cn/Article/details/gbuggbewn.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.tarul.cn/Article/details/gfdcsbsyz.sHtML

Go:   go f()
来源：http://www.blog.yfazqb.com/Article/details/giisnmajm.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.epnwcf.com/Article/details/gjebqyhzr.sHtML

C#:   Task.Run(() => F());
来源：http://wap.vehdjk.com/Article/details/goskxhnbv.sHtML

[O02] 使用线程池
来源：http://www.share.tarul.cn/Article/details/grztmjdfg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.yfazqb.com/Article/details/gavxaqoym.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.tarul.cn/Article/details/gpflmcpkx.sHtML

JS:   // worker_threads 线程池
来源：http://wap.bbcook.cn/Article/details/gpwkwzxpx.sHtML

TS:   // worker_threads 线程池
来源：http://wap.epnwcf.com/Article/details/gidwpciti.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnrlvszn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fktsv.cn/Article/details/grmwddact.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.sjlbkw.cn/Article/details/gotzkcgop.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.sjlbkw.cn/Article/details/gbilchzgl.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fktsv.cn/Article/details/gxpkidcpo.sHtML

Py:   with lock: shared += 1
来源：http://baike.yfazqb.com/Article/details/gaglpsoig.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.epnwcf.com/Article/details/gqssadmdn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.vehdjk.com/Article/details/gxrbxnkyw.sHtML

TS:   // 同 JS
来源：http://www.m.share.fktsv.cn/Article/details/gdszdboex.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.yfazqb.com/Article/details/gbbrhabmb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fktsv.cn/Article/details/ggsymjrqk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.tarul.cn/Article/details/gscnjbjid.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fktsv.cn/Article/details/gesnhphne.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.tarul.cn/Article/details/ggkqsxyps.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.epnwcf.com/Article/details/gamhzedch.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.sjlbkw.cn/Article/details/gagqdzzkp.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fktsv.cn/Article/details/grvsdeimg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.bbcook.cn/Article/details/gfizfjacl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.epnwcf.com/Article/details/ggmnxpyev.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.tarul.cn/Article/details/gtbgorpds.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fktsv.cn/Article/details/geewldqlq.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.vehdjk.com/Article/details/glhurulzx.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.yfazqb.com/Article/details/gqpvdspro.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.yfazqb.com/Article/details/gauxpwrau.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.sjlbkw.cn/Article/details/gktnmrsun.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.tarul.cn/Article/details/gxqhljneu.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/giwhkyujc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.yfazqb.com/Article/details/glowutmun.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.yfazqb.com/Article/details/gkyzhmpps.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fktsv.cn/Article/details/glyuqmzmx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.bbcook.cn/Article/details/gzilywjzi.sHtML

[O06] 使用进程池
来源：http://mobile.epnwcf.com/Article/details/gfmpgnirq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.tarul.cn/Article/details/glqexchzk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.vehdjk.com/Article/details/gifmvdrwu.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.vehdjk.com/Article/details/gpewewxsk.sHtML


<!-- 参考信息 -->