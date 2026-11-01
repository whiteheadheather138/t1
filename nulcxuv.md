代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://baike.bbcook.cn/Article/details/gtoioygqv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.bbcook.cn/Article/details/gikoifvsg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.yfazqb.com/Article/details/gtfjmpmiq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.yfazqb.com/Article/details/gdtsvqvgg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqstvsvzo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.bbcook.cn/Article/details/guvtlgvzr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.tarul.cn/Article/details/ghrwotpwz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.epnwcf.com/Article/details/gpxrdbunj.sHtML

[L03] 设置自定义请求头
来源：http://blog.fktsv.cn/Article/details/gxiabavxd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.epnwcf.com/Article/details/gxcronquz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.bbcook.cn/Article/details/gwovnzqey.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.epnwcf.com/Article/details/gkcdczjbi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.sjlbkw.cn/Article/details/gvreiwuyg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.bbcook.cn/Article/details/grstkumyh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.yfazqb.com/Article/details/giigjnynv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.epnwcf.com/Article/details/gpabnhbvr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fktsv.cn/Article/details/gvsxwiiyz.sHtML

[L04] 设置超时
来源：http://www.m.share.fktsv.cn/Article/details/grtgyybji.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.tarul.cn/Article/details/glldjdrtr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.yfazqb.com/Article/details/gvrhjwjky.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.yfazqb.com/Article/details/gwsgrujgm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fktsv.cn/Article/details/glzqghixj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.sjlbkw.cn/Article/details/goyfyyvrk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fktsv.cn/Article/details/gpshgsppo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.bbcook.cn/Article/details/gocikcvry.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.epnwcf.com/Article/details/gflhooqbw.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.sjlbkw.cn/Article/details/gjpshnver.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fktsv.cn/Article/details/ggghlnuir.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.bbcook.cn/Article/details/gtajbuejh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fktsv.cn/Article/details/gsehziqqk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.vehdjk.com/Article/details/gzvfkpifq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.sjlbkw.cn/Article/details/gacgfdztg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.sjlbkw.cn/Article/details/gilxvlwzu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.yfazqb.com/Article/details/guyjnwamj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.vehdjk.com/Article/details/gznzmcrnq.sHtML

[L06] 解析响应为 JSON
来源：http://baike.bbcook.cn/Article/details/gnhhemolc.sHtML

Py:   resp.json()
来源：http://blog.vehdjk.com/Article/details/geulupawx.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.bbcook.cn/Article/details/gxmmkrshw.sHtML

JS:   await resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/gtqocsgfy.sHtML

TS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/gbbxjzlxk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.bbcook.cn/Article/details/gjeuwfvvf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.epnwcf.com/Article/details/gbdrtuxdp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.bbcook.cn/Article/details/gaczphymq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.tarul.cn/Article/details/gsjnmejdr.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.tarul.cn/Article/details/gekjrhuan.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fktsv.cn/Article/details/gpkccqsxo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.vehdjk.com/Article/details/gljtllblh.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.vehdjk.com/Article/details/gcvwedvlw.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fktsv.cn/Article/details/gunjzdbxf.sHtML

Java: resp.statusCode()
来源：http://m.share.tarul.cn/Article/details/gjmwjgucr.sHtML

Go:   resp.StatusCode
来源：http://3g.tarul.cn/Article/details/gyagbszfp.sHtML

Ruby: resp.code.to_i
来源：http://3g.bbcook.cn/Article/details/ghmqftumg.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.sjlbkw.cn/Article/details/gqjxfdaka.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.vehdjk.com/Article/details/gagepanjc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.bbcook.cn/Article/details/gkzuzcfyd.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.bbcook.cn/Article/details/gervaryal.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.sjlbkw.cn/Article/details/gavlqvqpp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.tarul.cn/Article/details/gtlvedesf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.bbcook.cn/Article/details/gxqulfejn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.tarul.cn/Article/details/gkdjhvdft.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fktsv.cn/Article/details/gyrogkidb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.epnwcf.com/Article/details/gpxnctfoj.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gvodiejrm.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.yfazqb.com/Article/details/giidahbbs.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gbghmljtr.sHtML

[M01] 读取命令行参数
来源：http://blog.tarul.cn/Article/details/gfudqgtjb.sHtML

Py:   sys.argv[1:]
来源：http://www.share.sjlbkw.cn/Article/details/gudaowryj.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fktsv.cn/Article/details/glpfjmycs.sHtML

JS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/ghcdmprro.sHtML

TS:   process.argv.slice(2)
来源：http://wap.yfazqb.com/Article/details/gqjcjqoys.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.sjlbkw.cn/Article/details/gvnqxvupc.sHtML

Go:   os.Args[1:]
来源：http://m.share.epnwcf.com/Article/details/ggamzteru.sHtML

Ruby: ARGV
来源：http://www.share.bbcook.cn/Article/details/gwrqwhfri.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.yfazqb.com/Article/details/gzdxxpwml.sHtML

[M02] 读取环境变量
来源：http://read.share.yfazqb.com/Article/details/gxlswxczj.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fktsv.cn/Article/details/gpiqkbfuh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.bbcook.cn/Article/details/gmmjcfbfr.sHtML

JS:   process.env.HOME
来源：http://blog.bbcook.cn/Article/details/ggpqsajnt.sHtML

TS:   process.env.HOME
来源：http://blog.sjlbkw.cn/Article/details/gpnhlqhmg.sHtML

Java: System.getenv("HOME")
来源：http://read.share.bbcook.cn/Article/details/guyierqat.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.tarul.cn/Article/details/gjpoxtptr.sHtML

Ruby: ENV["HOME"]
来源：http://baike.bbcook.cn/Article/details/gsdyawilj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.vehdjk.com/Article/details/gojcqxpcl.sHtML

[M03] 执行外部命令
来源：http://read.share.bbcook.cn/Article/details/gptalmksl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.epnwcf.com/Article/details/gazatepmg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fktsv.cn/Article/details/gogjnaqig.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gplplview.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.vehdjk.com/Article/details/gutvusiac.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.tarul.cn/Article/details/gayksoktl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.yfazqb.com/Article/details/glkhqepog.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.tarul.cn/Article/details/gmorqotje.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fktsv.cn/Article/details/gyfkldxqv.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fktsv.cn/Article/details/gxdsgdpgy.sHtML

Py:   os.getcwd()
来源：http://m.share.tarul.cn/Article/details/gydshjxzr.sHtML

PHP:  getcwd();
来源：http://www.m.share.vehdjk.com/Article/details/ginlzzorg.sHtML

JS:   process.cwd()
来源：http://www.m.share.bbcook.cn/Article/details/gyqhigrqb.sHtML

TS:   process.cwd()
来源：http://m.share.fktsv.cn/Article/details/gxzgrcefo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.vehdjk.com/Article/details/guoxuzlhs.sHtML

Go:   os.Getwd()
来源：http://blog.vehdjk.com/Article/details/gqcdhcvqa.sHtML

Ruby: Dir.pwd
来源：http://read.share.sjlbkw.cn/Article/details/gzlhpuxkb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.vehdjk.com/Article/details/guiwdaiiw.sHtML

[M05] 设置退出码
来源：http://blog.fktsv.cn/Article/details/gvxdzrxqh.sHtML

Py:   sys.exit(1)
来源：http://m.share.yfazqb.com/Article/details/gmoelirty.sHtML

PHP:  exit(1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gprrmnhfc.sHtML

JS:   process.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gdlrjdhin.sHtML

TS:   process.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gxsrokjsp.sHtML

Java: System.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gqhsmeqmc.sHtML

Go:   os.Exit(1)
来源：http://blog.tarul.cn/Article/details/gqkbarxdl.sHtML

Ruby: exit 1
来源：http://www.blog.fktsv.cn/Article/details/gpddwgnwx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.epnwcf.com/Article/details/gnenijnjt.sHtML

[M06] 向标准错误输出
来源：http://wap.yfazqb.com/Article/details/gudxtviov.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.yfazqb.com/Article/details/gtcwskrgx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.sjlbkw.cn/Article/details/grbxiqycv.sHtML

JS:   console.error("err")
来源：http://baike.epnwcf.com/Article/details/gugautqtv.sHtML

TS:   console.error("err")
来源：http://wap.yfazqb.com/Article/details/gnnwvsibn.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fktsv.cn/Article/details/geijucddh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.vehdjk.com/Article/details/gcdzbsaix.sHtML

Ruby: warn "err"
来源：http://3g.yfazqb.com/Article/details/gtaeknzyr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.sjlbkw.cn/Article/details/gtdwoednx.sHtML

[M07] 判断是否为主入口
来源：http://www.share.sjlbkw.cn/Article/details/ggtkbqleh.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.yfazqb.com/Article/details/gntgfazid.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.epnwcf.com/Article/details/ghkxmexas.sHtML

JS:   require.main === module
来源：http://baike.sjlbkw.cn/Article/details/ggywfezxg.sHtML

TS:   require.main === module
来源：http://blog.vehdjk.com/Article/details/geovcmfgp.sHtML

Java: public static void main(String[] args)
来源：http://www.share.vehdjk.com/Article/details/gcycoqakn.sHtML

Go:   func main()
来源：http://mobile.sjlbkw.cn/Article/details/gmhuyaxvy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.epnwcf.com/Article/details/gymebulit.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.epnwcf.com/Article/details/ggdaesiqo.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.tarul.cn/Article/details/gadwvxuqn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.bbcook.cn/Article/details/gflwdqqau.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.yfazqb.com/Article/details/gknezetsu.sHtML

JS:   process.platform;  process.version
来源：http://blog.yfazqb.com/Article/details/gpltaeidk.sHtML

TS:   process.platform;  process.version
来源：http://3g.yfazqb.com/Article/details/graklqgmp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.epnwcf.com/Article/details/gwcssxdcd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fktsv.cn/Article/details/gjjrvntwd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.bbcook.cn/Article/details/gmiqvilus.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.bbcook.cn/Article/details/gwamhkjbw.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gsnvkrozy.sHtML

N. 数据结构与算法
来源：http://wap.yfazqb.com/Article/details/getzegzlc.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gagwooyxt.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.epnwcf.com/Article/details/gdcdalvwx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.epnwcf.com/Article/details/griruarja.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.sjlbkw.cn/Article/details/guxdkyook.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.tarul.cn/Article/details/gulexegiq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.epnwcf.com/Article/details/gjlkqaxgl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.epnwcf.com/Article/details/gynpgbrez.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.bbcook.cn/Article/details/gcxkfapnw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fktsv.cn/Article/details/gtulyztfh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gdvdbsbcc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.bbcook.cn/Article/details/gppnmrqgu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.vehdjk.com/Article/details/gljeehkwa.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.tarul.cn/Article/details/ggywseoqy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.vehdjk.com/Article/details/glvltjvly.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.tarul.cn/Article/details/gcumzxlyp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.yfazqb.com/Article/details/grjtlyecl.sHtML

Go:   slices.Sort(arr)
来源：http://baike.epnwcf.com/Article/details/grzpburpa.sHtML

Ruby: arr.sort
来源：http://wap.vehdjk.com/Article/details/gjwzidalk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.sjlbkw.cn/Article/details/gljlfllce.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.yfazqb.com/Article/details/gdlqsieio.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.epnwcf.com/Article/details/gssmlflpe.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.bbcook.cn/Article/details/gpctnunuj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.vehdjk.com/Article/details/glmpapntb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.yfazqb.com/Article/details/grrvzdyyo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.epnwcf.com/Article/details/gxxvzmsku.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.epnwcf.com/Article/details/gfzbhfzzp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.yfazqb.com/Article/details/gdiglzncq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.tarul.cn/Article/details/gyhzfjaod.sHtML

[N04] 斐波那契数列
来源：http://www.blog.sjlbkw.cn/Article/details/gvinqynov.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.yfazqb.com/Article/details/guxhzsfpp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.tarul.cn/Article/details/gekhfsnzy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.yfazqb.com/Article/details/guieluivt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.tarul.cn/Article/details/gfwmmleie.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.vehdjk.com/Article/details/gwqournku.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.yfazqb.com/Article/details/gadxlntxb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.bbcook.cn/Article/details/grkbbcqgc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.bbcook.cn/Article/details/ghkgwlwmu.sHtML

[N05] 最大公约数
来源：http://wap.yfazqb.com/Article/details/gtssynvhu.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.yfazqb.com/Article/details/gjrslrxsy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.bbcook.cn/Article/details/giugtwgfe.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.tarul.cn/Article/details/gdkvxsjbb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.tarul.cn/Article/details/gisndeafg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.sjlbkw.cn/Article/details/gfzueectz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.bbcook.cn/Article/details/ghsxgqews.sHtML

Ruby: a.gcd(b)
来源：http://3g.fktsv.cn/Article/details/gmiihiwie.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fktsv.cn/Article/details/gbsolihrv.sHtML

[N06] 判断回文字符串
来源：http://www.blog.tarul.cn/Article/details/gugnwoinh.sHtML

Py:   s == s[::-1]
来源：http://www.blog.vehdjk.com/Article/details/gjlwzhhax.sHtML

PHP:  $s === strrev($s);
来源：http://baike.vehdjk.com/Article/details/gdewtcxhg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fktsv.cn/Article/details/gjbjgjuoj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gsakerwce.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.vehdjk.com/Article/details/gszdtycpf.sHtML

Go:   // 双指针从两端比较
来源：http://3g.sjlbkw.cn/Article/details/gbmonyvtb.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fktsv.cn/Article/details/gnwkysaqs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.epnwcf.com/Article/details/ggcmlaxma.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.yfazqb.com/Article/details/gznbmcwia.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.sjlbkw.cn/Article/details/gcfmcgjde.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.vehdjk.com/Article/details/guqqxnlbs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.tarul.cn/Article/details/gftryemel.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.sjlbkw.cn/Article/details/gtcmfovag.sHtML

Java: // 手写 HashMap
来源：http://baike.fktsv.cn/Article/details/gnltwkhgf.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.epnwcf.com/Article/details/gwdgfxdlk.sHtML

Ruby: // 手写 Hash
来源：http://read.share.yfazqb.com/Article/details/gvzlbmluw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.sjlbkw.cn/Article/details/gjmsntnry.sHtML

[N08] 生成全排列
来源：http://baike.tarul.cn/Article/details/glrrrkwhj.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gzyxzlwbx.sHtML

PHP:  // 手写递归交换
来源：http://wap.yfazqb.com/Article/details/gjeqycggq.sHtML

JS:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gqzrzfbop.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gzucihiit.sHtML

Java: // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gpvilndlv.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gaoqqxugp.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.vehdjk.com/Article/details/garqngasj.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gnrybvstc.sHtML

[N09] 栈与队列
来源：http://wap.bbcook.cn/Article/details/gnaypblkx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gfumiuluf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gnxdanbem.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.vehdjk.com/Article/details/gzjgislel.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.yfazqb.com/Article/details/gepzzetuu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.yfazqb.com/Article/details/gudqhriqc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.bbcook.cn/Article/details/gmbpxnpsk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.epnwcf.com/Article/details/gwosornms.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.yfazqb.com/Article/details/gkygkgzwm.sHtML

[N10] 链表节点定义
来源：http://m.share.bbcook.cn/Article/details/guwabkotg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.yfazqb.com/Article/details/ggzrmbnrf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.sjlbkw.cn/Article/details/gpssiunra.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.tarul.cn/Article/details/gzvezuztj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.sjlbkw.cn/Article/details/gawylptob.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.bbcook.cn/Article/details/gdaskewsr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.yfazqb.com/Article/details/gogzjbzmp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fktsv.cn/Article/details/goayibjvw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.bbcook.cn/Article/details/gnqulnodb.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.bbcook.cn/Article/details/gzaunkvxp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.epnwcf.com/Article/details/gyuhjflfe.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.bbcook.cn/Article/details/gscfkajzz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.vehdjk.com/Article/details/gwoeqfprn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fktsv.cn/Article/details/gmjjlpopg.sHtML

Java: // 手写递归
来源：http://m.share.tarul.cn/Article/details/gjldsgjbd.sHtML

Go:   // 手写递归
来源：http://wap.vehdjk.com/Article/details/gcwolejsw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fktsv.cn/Article/details/gtmcbytkf.sHtML

C#:   // 手写递归
来源：http://www.share.sjlbkw.cn/Article/details/gkeqtyeke.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fktsv.cn/Article/details/gturfkaxa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fktsv.cn/Article/details/gvhaecgqi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.epnwcf.com/Article/details/gxnohqdbv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.tarul.cn/Article/details/gvasufhdx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.yfazqb.com/Article/details/gbbuajiku.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.tarul.cn/Article/details/gfvjfezrm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fktsv.cn/Article/details/gnbzpamni.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.epnwcf.com/Article/details/gakxgooqu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.sjlbkw.cn/Article/details/gkgjbbrtc.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gvhuxrcrp.sHtML

O. 并发与异步
来源：http://mobile.fktsv.cn/Article/details/ghtlettzx.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gcihyvjzl.sHtML

[O01] 启动一个线程
来源：http://baike.sjlbkw.cn/Article/details/ggirdwmyj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.tarul.cn/Article/details/gzxohakay.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.yfazqb.com/Article/details/gjegjjgiv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.yfazqb.com/Article/details/groyfwodx.sHtML

TS:   // 同 JS
来源：http://m.share.vehdjk.com/Article/details/gcijpokku.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.tarul.cn/Article/details/gwokewteq.sHtML

Go:   go f()
来源：http://www.blog.epnwcf.com/Article/details/guipzhizn.sHtML

Ruby: Thread.new { f }
来源：http://3g.fktsv.cn/Article/details/gpqdhcnkz.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.sjlbkw.cn/Article/details/glqpbrvjj.sHtML

[O02] 使用线程池
来源：http://baike.sjlbkw.cn/Article/details/gmckiskhh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.bbcook.cn/Article/details/ginvsitjn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.bbcook.cn/Article/details/gnfjzyuvm.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.bbcook.cn/Article/details/gqijsaean.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fktsv.cn/Article/details/gpdnltese.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.sjlbkw.cn/Article/details/ghykdujsz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.yfazqb.com/Article/details/gfreiqhoh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.epnwcf.com/Article/details/graspbdwp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.epnwcf.com/Article/details/gkrhoxxub.sHtML

[O03] 加锁保护共享数据
来源：http://3g.vehdjk.com/Article/details/gtzphmvvv.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fktsv.cn/Article/details/gpodqjudr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.sjlbkw.cn/Article/details/guqadomrc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fktsv.cn/Article/details/gscijazkz.sHtML

TS:   // 同 JS
来源：http://mobile.fktsv.cn/Article/details/gxthihdyr.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.vehdjk.com/Article/details/gqtbsgydx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.sjlbkw.cn/Article/details/gtoowgqfh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.tarul.cn/Article/details/gnrgdxlwv.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.epnwcf.com/Article/details/gjqvhrvnb.sHtML

[O04] 定义异步函数并等待
来源：http://blog.yfazqb.com/Article/details/gizfxugti.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.yfazqb.com/Article/details/gpsyunhit.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.yfazqb.com/Article/details/gaksycyfv.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.bbcook.cn/Article/details/grrkwzhyw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.bbcook.cn/Article/details/ghyyvlgzi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.bbcook.cn/Article/details/gmfcpivsj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.yfazqb.com/Article/details/gxemygsmc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fktsv.cn/Article/details/gedhgjojr.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.sjlbkw.cn/Article/details/gzbojocsx.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.vehdjk.com/Article/details/gcbbnlati.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.yfazqb.com/Article/details/gymvrjhkq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.yfazqb.com/Article/details/gmkosjsui.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.yfazqb.com/Article/details/gascmoyir.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.vehdjk.com/Article/details/getkiorac.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.vehdjk.com/Article/details/gwtvbnldl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fktsv.cn/Article/details/gjpjotxrr.sHtML

Ruby: threads.map(&:join)
来源：http://3g.yfazqb.com/Article/details/goxhruqlc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fktsv.cn/Article/details/gfileabbk.sHtML

[O06] 使用进程池
来源：http://mobile.sjlbkw.cn/Article/details/gkmldtiay.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.epnwcf.com/Article/details/gqpuxurav.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.tarul.cn/Article/details/giwjekrev.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.tarul.cn/Article/details/gfaliluhi.sHtML


<!-- 参考信息 -->