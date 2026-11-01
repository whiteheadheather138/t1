代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.yfazqb.com/Article/details/ggsbtzbtc.sHtML

JS:   await fetch(url)
来源：http://baike.tarul.cn/Article/details/gasvuswwk.sHtML

TS:   await fetch(url)
来源：http://www.blog.vehdjk.com/Article/details/ghjoylqaz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.epnwcf.com/Article/details/gwcfhehak.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.bbcook.cn/Article/details/gawtvetfi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fktsv.cn/Article/details/ghqkxzrdi.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.sjlbkw.cn/Article/details/gohdutxww.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fktsv.cn/Article/details/gjbkmiosp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.tarul.cn/Article/details/gqmbbrzmz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.bbcook.cn/Article/details/gqgoebdsm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.yfazqb.com/Article/details/gznzrrszr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.vehdjk.com/Article/details/gcvjidxlh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.sjlbkw.cn/Article/details/gnuusvqlo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.vehdjk.com/Article/details/gofhnludw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.epnwcf.com/Article/details/ghtuvatxa.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.vehdjk.com/Article/details/gudyzndoy.sHtML

[L03] 设置自定义请求头
来源：http://baike.vehdjk.com/Article/details/gxgksznpn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.yfazqb.com/Article/details/gmdkuseet.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fktsv.cn/Article/details/gkhnbtasr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.yfazqb.com/Article/details/gfmalepcw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.yfazqb.com/Article/details/gzvpdnsji.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.sjlbkw.cn/Article/details/gowmnupkc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.tarul.cn/Article/details/gdkuhpfsn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.tarul.cn/Article/details/gnpplfvzx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.bbcook.cn/Article/details/gmytlbcfz.sHtML

[L04] 设置超时
来源：http://mobile.fktsv.cn/Article/details/gjexsaysx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.epnwcf.com/Article/details/glpaxmzwn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.bbcook.cn/Article/details/gopwfhzrr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.yfazqb.com/Article/details/ghmaqxorv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.vehdjk.com/Article/details/gxugljuvr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.bbcook.cn/Article/details/gambnjaqa.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fktsv.cn/Article/details/grxepptcl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.sjlbkw.cn/Article/details/gbthrnnhl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.vehdjk.com/Article/details/gvsdwoivj.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.sjlbkw.cn/Article/details/gbtilivlz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.sjlbkw.cn/Article/details/ghveubyar.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fktsv.cn/Article/details/gosidxrxr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.bbcook.cn/Article/details/gtviohsev.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.vehdjk.com/Article/details/gvuaqnyzv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fktsv.cn/Article/details/ghwhoxxur.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.tarul.cn/Article/details/gfncthdyt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.sjlbkw.cn/Article/details/gezpgggdr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.epnwcf.com/Article/details/gabeilepq.sHtML

[L06] 解析响应为 JSON
来源：http://3g.yfazqb.com/Article/details/guijsxjlw.sHtML

Py:   resp.json()
来源：http://mobile.fktsv.cn/Article/details/ggkuylply.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fktsv.cn/Article/details/gdphsbbdg.sHtML

JS:   await resp.json()
来源：http://3g.sjlbkw.cn/Article/details/gqgpeeeug.sHtML

TS:   await resp.json()
来源：http://mobile.epnwcf.com/Article/details/gdovgexov.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.tarul.cn/Article/details/gsftxxovj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.epnwcf.com/Article/details/gjyfmgqvq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fktsv.cn/Article/details/glwojwbil.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.yfazqb.com/Article/details/gtxhixemg.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.vehdjk.com/Article/details/guihmufla.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.bbcook.cn/Article/details/geqhcczzo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fktsv.cn/Article/details/gwayvabuc.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.tarul.cn/Article/details/gefxcydwa.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fktsv.cn/Article/details/gezfbpsyl.sHtML

Java: resp.statusCode()
来源：http://blog.yfazqb.com/Article/details/ggevnvwpd.sHtML

Go:   resp.StatusCode
来源：http://mobile.yfazqb.com/Article/details/gakjmgwri.sHtML

Ruby: resp.code.to_i
来源：http://read.share.epnwcf.com/Article/details/gbbvjuqfm.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fktsv.cn/Article/details/gcvxiewno.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.epnwcf.com/Article/details/gbknofcey.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.sjlbkw.cn/Article/details/gakbqdszq.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.bbcook.cn/Article/details/gdpgbbskz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.vehdjk.com/Article/details/gytwfokkb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fktsv.cn/Article/details/ghtmdqrco.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fktsv.cn/Article/details/gcaunuhwk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.vehdjk.com/Article/details/gdregqbqh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.bbcook.cn/Article/details/gkokgdatj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.epnwcf.com/Article/details/gquzhirdz.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ghxskemam.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fktsv.cn/Article/details/gmaiepkxg.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gvcvszfoh.sHtML

[M01] 读取命令行参数
来源：http://blog.tarul.cn/Article/details/gzjxqewnc.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fktsv.cn/Article/details/gukmadjgs.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fktsv.cn/Article/details/ggttmgwwj.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.vehdjk.com/Article/details/grakzucbg.sHtML

TS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/gfqsjhtyj.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.epnwcf.com/Article/details/gdhdkgfip.sHtML

Go:   os.Args[1:]
来源：http://baike.yfazqb.com/Article/details/gdwovdfgw.sHtML

Ruby: ARGV
来源：http://www.blog.sjlbkw.cn/Article/details/gacomkcnr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.bbcook.cn/Article/details/gvrgpnzja.sHtML

[M02] 读取环境变量
来源：http://read.share.yfazqb.com/Article/details/gpfotahcf.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.tarul.cn/Article/details/grnnirsln.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.sjlbkw.cn/Article/details/gtunvxuwp.sHtML

JS:   process.env.HOME
来源：http://m.share.vehdjk.com/Article/details/gumrutfpc.sHtML

TS:   process.env.HOME
来源：http://www.share.yfazqb.com/Article/details/govbigkzj.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gswlkceog.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.vehdjk.com/Article/details/gnmgzcabg.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fktsv.cn/Article/details/goxhcgcqr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fktsv.cn/Article/details/gjaljvgou.sHtML

[M03] 执行外部命令
来源：http://blog.fktsv.cn/Article/details/glowhulbp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.tarul.cn/Article/details/gzcbmcrwb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fktsv.cn/Article/details/grntgddio.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fktsv.cn/Article/details/gefhyrqbb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.epnwcf.com/Article/details/ghjcbfihx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.epnwcf.com/Article/details/gjbkakzdf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.vehdjk.com/Article/details/gfnzobpck.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.epnwcf.com/Article/details/giccevtxm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.yfazqb.com/Article/details/gyyxeukeh.sHtML

[M04] 获取当前工作目录
来源：http://read.share.tarul.cn/Article/details/ghunfvkgr.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fktsv.cn/Article/details/gcjixhfcx.sHtML

PHP:  getcwd();
来源：http://www.share.vehdjk.com/Article/details/gxgxwglfx.sHtML

JS:   process.cwd()
来源：http://read.share.epnwcf.com/Article/details/grtwsgdqi.sHtML

TS:   process.cwd()
来源：http://mobile.bbcook.cn/Article/details/gemgfgixc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.epnwcf.com/Article/details/gtqbmygsl.sHtML

Go:   os.Getwd()
来源：http://blog.tarul.cn/Article/details/gckdqtvdm.sHtML

Ruby: Dir.pwd
来源：http://www.blog.vehdjk.com/Article/details/glpneuayo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.yfazqb.com/Article/details/guksierlu.sHtML

[M05] 设置退出码
来源：http://wap.tarul.cn/Article/details/gpepvyqxv.sHtML

Py:   sys.exit(1)
来源：http://3g.yfazqb.com/Article/details/gbuaixaca.sHtML

PHP:  exit(1);
来源：http://read.share.bbcook.cn/Article/details/gqovqqpsk.sHtML

JS:   process.exit(1)
来源：http://wap.epnwcf.com/Article/details/gbimmtvod.sHtML

TS:   process.exit(1)
来源：http://m.share.yfazqb.com/Article/details/giqfgbhgw.sHtML

Java: System.exit(1)
来源：http://www.share.bbcook.cn/Article/details/gzndglndo.sHtML

Go:   os.Exit(1)
来源：http://read.share.yfazqb.com/Article/details/gvluiwaml.sHtML

Ruby: exit 1
来源：http://wap.yfazqb.com/Article/details/gnxwtrhlm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.epnwcf.com/Article/details/gfirdfsbs.sHtML

[M06] 向标准错误输出
来源：http://m.share.tarul.cn/Article/details/gayosdflo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.sjlbkw.cn/Article/details/geuzoohec.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.yfazqb.com/Article/details/grcncovol.sHtML

JS:   console.error("err")
来源：http://read.share.yfazqb.com/Article/details/gjvzzwsnt.sHtML

TS:   console.error("err")
来源：http://3g.vehdjk.com/Article/details/giyaxoiyr.sHtML

Java: System.err.println("err")
来源：http://www.m.share.epnwcf.com/Article/details/gzrfvtwff.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.epnwcf.com/Article/details/ginzxesrb.sHtML

Ruby: warn "err"
来源：http://www.m.share.tarul.cn/Article/details/gcbxsgpap.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.sjlbkw.cn/Article/details/gnhvdcvqt.sHtML

[M07] 判断是否为主入口
来源：http://read.share.yfazqb.com/Article/details/gjzuhlraz.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.yfazqb.com/Article/details/gacmaseqp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.yfazqb.com/Article/details/ghfmamlue.sHtML

JS:   require.main === module
来源：http://www.share.yfazqb.com/Article/details/gsdsuvoms.sHtML

TS:   require.main === module
来源：http://baike.bbcook.cn/Article/details/gcayfuvbz.sHtML

Java: public static void main(String[] args)
来源：http://baike.epnwcf.com/Article/details/gbmixtokl.sHtML

Go:   func main()
来源：http://blog.fktsv.cn/Article/details/gnkopzcfg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.tarul.cn/Article/details/gpoqhhhbu.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.vehdjk.com/Article/details/gmvavbjpx.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.tarul.cn/Article/details/gdmsbcfyu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.vehdjk.com/Article/details/gerlftntc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.bbcook.cn/Article/details/gcfdwcfka.sHtML

JS:   process.platform;  process.version
来源：http://blog.epnwcf.com/Article/details/gkjfzfgdp.sHtML

TS:   process.platform;  process.version
来源：http://3g.vehdjk.com/Article/details/gvwmbzvqs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfxqkcyi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.epnwcf.com/Article/details/gxgvsduwb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.epnwcf.com/Article/details/gjbfzkuzy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.bbcook.cn/Article/details/gechdhtpm.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gfokuvhnb.sHtML

N. 数据结构与算法
来源：http://3g.vehdjk.com/Article/details/gembsyhlj.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/goxfniejs.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.sjlbkw.cn/Article/details/gepdmegig.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.vehdjk.com/Article/details/gcvgbhxlo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.yfazqb.com/Article/details/gipwhdgmz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fktsv.cn/Article/details/gimceqnbt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.epnwcf.com/Article/details/gsceqbrun.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.bbcook.cn/Article/details/gnglnqeus.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.yfazqb.com/Article/details/gzbbcaxnk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.epnwcf.com/Article/details/gnunyptfu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnmqczch.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.sjlbkw.cn/Article/details/ggbddwipx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.vehdjk.com/Article/details/gfcevycpc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.yfazqb.com/Article/details/gkqdajtne.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.yfazqb.com/Article/details/gllbgcmjd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.epnwcf.com/Article/details/gkptdlpyc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.tarul.cn/Article/details/guemisjrm.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.vehdjk.com/Article/details/gdythwllq.sHtML

Ruby: arr.sort
来源：http://baike.fktsv.cn/Article/details/gwyqqfvtu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.vehdjk.com/Article/details/gtlpxmege.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.sjlbkw.cn/Article/details/gyuuebgfo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.sjlbkw.cn/Article/details/gjvsircce.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.vehdjk.com/Article/details/ggsfjriub.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.epnwcf.com/Article/details/golnzwyah.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fktsv.cn/Article/details/gtbyxhcts.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.sjlbkw.cn/Article/details/gprkvclqa.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.sjlbkw.cn/Article/details/gsodynoiw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.bbcook.cn/Article/details/gangwzyof.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.sjlbkw.cn/Article/details/gtqtmqbbm.sHtML

[N04] 斐波那契数列
来源：http://baike.vehdjk.com/Article/details/gmackcnob.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.epnwcf.com/Article/details/gezwlahdx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.sjlbkw.cn/Article/details/gkeswvndp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gkhpktxng.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/gxchfqzqb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.vehdjk.com/Article/details/gonipmjay.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.bbcook.cn/Article/details/gnntefxaq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.sjlbkw.cn/Article/details/gqvtichud.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/gorrivdbw.sHtML

[N05] 最大公约数
来源：http://blog.fktsv.cn/Article/details/ggdszerzw.sHtML

Py:   math.gcd(a, b)
来源：http://baike.bbcook.cn/Article/details/ggiawzznr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.bbcook.cn/Article/details/gfkfqqvog.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.epnwcf.com/Article/details/gjtcziexm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fktsv.cn/Article/details/gguixnzee.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.yfazqb.com/Article/details/gyiywxmwl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.epnwcf.com/Article/details/giagaevcn.sHtML

Ruby: a.gcd(b)
来源：http://www.share.tarul.cn/Article/details/gxapkhldz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.bbcook.cn/Article/details/ghnsoeojn.sHtML

[N06] 判断回文字符串
来源：http://mobile.vehdjk.com/Article/details/gkzbozdgn.sHtML

Py:   s == s[::-1]
来源：http://blog.sjlbkw.cn/Article/details/gqjtufsse.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.epnwcf.com/Article/details/gjyaorozz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gjidafkaq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gokcrkjie.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.tarul.cn/Article/details/ghkktsomt.sHtML

Go:   // 双指针从两端比较
来源：http://wap.bbcook.cn/Article/details/gytqserux.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.bbcook.cn/Article/details/gtioscmno.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.tarul.cn/Article/details/gsdiophld.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fktsv.cn/Article/details/getliymsc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.vehdjk.com/Article/details/giafekqpg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.epnwcf.com/Article/details/gywcpllio.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.epnwcf.com/Article/details/gpsbeesga.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.epnwcf.com/Article/details/ghfrrmsiu.sHtML

Java: // 手写 HashMap
来源：http://read.share.fktsv.cn/Article/details/gdiqgodol.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.tarul.cn/Article/details/gchgqrafa.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.vehdjk.com/Article/details/gwyjmeqmp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.epnwcf.com/Article/details/gwehgpyyx.sHtML

[N08] 生成全排列
来源：http://mobile.epnwcf.com/Article/details/gnzvljmsl.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.bbcook.cn/Article/details/gfwyzlfrc.sHtML

PHP:  // 手写递归交换
来源：http://3g.bbcook.cn/Article/details/gwtodnmzq.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/geciwwrwe.sHtML

TS:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gimwrqmam.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/ghewrpkax.sHtML

Go:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gxdlwbwex.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.epnwcf.com/Article/details/grpcgrami.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gfkqukfzr.sHtML

[N09] 栈与队列
来源：http://wap.tarul.cn/Article/details/ghivmkprg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.vehdjk.com/Article/details/ggfscflaw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.sjlbkw.cn/Article/details/ggishkfzo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.yfazqb.com/Article/details/gvzofeujl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.sjlbkw.cn/Article/details/gdswtwgjl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.tarul.cn/Article/details/gqusrlsws.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.sjlbkw.cn/Article/details/gbmfmegmv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.bbcook.cn/Article/details/gdsnshwgn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.bbcook.cn/Article/details/gxiwadawf.sHtML

[N10] 链表节点定义
来源：http://baike.fktsv.cn/Article/details/gpjymleuj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.epnwcf.com/Article/details/ghnrxbhcc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.epnwcf.com/Article/details/gvbbhjcpz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.epnwcf.com/Article/details/gbjeediwr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.yfazqb.com/Article/details/geipbwohz.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.yfazqb.com/Article/details/gpgevqvly.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.tarul.cn/Article/details/gqtnuluro.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.vehdjk.com/Article/details/gpmyndmrq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.sjlbkw.cn/Article/details/gqfltyvcj.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fktsv.cn/Article/details/gvxfvuizn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.bbcook.cn/Article/details/gpfinteta.sHtML

PHP:  // 手写递归函数
来源：http://blog.epnwcf.com/Article/details/gquucpmqp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.tarul.cn/Article/details/gwzzpmdub.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.yfazqb.com/Article/details/gklumixmd.sHtML

Java: // 手写递归
来源：http://www.m.share.epnwcf.com/Article/details/graimaaso.sHtML

Go:   // 手写递归
来源：http://m.share.fktsv.cn/Article/details/gdnlzcdld.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fktsv.cn/Article/details/gmuypnqee.sHtML

C#:   // 手写递归
来源：http://baike.tarul.cn/Article/details/gjoqjfpny.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.vehdjk.com/Article/details/gpzheidqa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.vehdjk.com/Article/details/glscgekaw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fktsv.cn/Article/details/gilamugav.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.sjlbkw.cn/Article/details/grkdpucet.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.bbcook.cn/Article/details/ggbcdgmet.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.tarul.cn/Article/details/gmyrxabta.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fktsv.cn/Article/details/gkwtrgsvo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fktsv.cn/Article/details/gvaarleyi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.sjlbkw.cn/Article/details/giyslyzni.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gdubcyfan.sHtML

O. 并发与异步
来源：http://3g.epnwcf.com/Article/details/gyajbtvep.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/ghrugssub.sHtML

[O01] 启动一个线程
来源：http://read.share.bbcook.cn/Article/details/gfxjssydo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.bbcook.cn/Article/details/ggoyretns.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.yfazqb.com/Article/details/gzjlvbome.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.bbcook.cn/Article/details/gvxnostep.sHtML

TS:   // 同 JS
来源：http://www.m.share.tarul.cn/Article/details/gmzxqrlah.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.sjlbkw.cn/Article/details/gnxmhudbr.sHtML

Go:   go f()
来源：http://www.blog.epnwcf.com/Article/details/gtikcxjsu.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.epnwcf.com/Article/details/giqvqwsfo.sHtML

C#:   Task.Run(() => F());
来源：http://wap.sjlbkw.cn/Article/details/gevflgsxo.sHtML

[O02] 使用线程池
来源：http://blog.bbcook.cn/Article/details/gjoqtfled.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.vehdjk.com/Article/details/guhrtuzib.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.vehdjk.com/Article/details/gkbpoitjv.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.tarul.cn/Article/details/gelwyvmqk.sHtML

TS:   // worker_threads 线程池
来源：http://baike.yfazqb.com/Article/details/gfzcvbvel.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fktsv.cn/Article/details/gpkuzotnl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.vehdjk.com/Article/details/gwifmgfow.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.epnwcf.com/Article/details/geuaaifzv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.vehdjk.com/Article/details/gjpheycuq.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.bbcook.cn/Article/details/ganyycgah.sHtML

Py:   with lock: shared += 1
来源：http://blog.vehdjk.com/Article/details/gsmjvvoej.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.bbcook.cn/Article/details/gpwaiusxv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.tarul.cn/Article/details/gcpzbqika.sHtML

TS:   // 同 JS
来源：http://3g.epnwcf.com/Article/details/gviasgjeo.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.bbcook.cn/Article/details/glfeckqlw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.sjlbkw.cn/Article/details/gmvrtjtib.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.yfazqb.com/Article/details/gbtewwwed.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.bbcook.cn/Article/details/gaojhzjjp.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.vehdjk.com/Article/details/giifgqklf.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fktsv.cn/Article/details/gxynljxas.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.vehdjk.com/Article/details/gqpvhvlta.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.sjlbkw.cn/Article/details/gknwarlxi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.epnwcf.com/Article/details/gtrclfesr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.vehdjk.com/Article/details/gvmnhdllx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.tarul.cn/Article/details/glevwytcf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.vehdjk.com/Article/details/gxzptxisp.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fktsv.cn/Article/details/gjgllnqcn.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.bbcook.cn/Article/details/gofjfhicg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fktsv.cn/Article/details/grymbfnca.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.sjlbkw.cn/Article/details/gphivyuqw.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.vehdjk.com/Article/details/gmqyjvtwj.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fktsv.cn/Article/details/gwqmjfowp.sHtML


<!-- 参考信息 -->