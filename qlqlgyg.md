代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://mobile.epnwcf.com/Article/details/ggdatuvsc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.vehdjk.com/Article/details/giecmzain.sHtML

JS:   structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gazjbdlfv.sHtML

TS:   structuredClone(obj)
来源：http://baike.vehdjk.com/Article/details/gvvlttduv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.tarul.cn/Article/details/ggyulimnw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.tarul.cn/Article/details/gncsszvew.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.epnwcf.com/Article/details/geprtrmla.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.bbcook.cn/Article/details/gveejujwo.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.bbcook.cn/Article/details/gyzljnvgu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.yfazqb.com/Article/details/gmaogqicw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.yfazqb.com/Article/details/geylrsjyh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.epnwcf.com/Article/details/gevajsyee.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.bbcook.cn/Article/details/gkwlocrjy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.sjlbkw.cn/Article/details/gpzjpllqu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.tarul.cn/Article/details/gqzcvpsyw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/gnqjgyujh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.tarul.cn/Article/details/ghycitsxm.sHtML

[K07] 进制转换
来源：http://www.m.share.tarul.cn/Article/details/gnjghddkh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gluhrczjc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fktsv.cn/Article/details/gazorvmzd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/gusjcxpyw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gzzhgedbz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gykmzodab.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.yfazqb.com/Article/details/glumzhnzx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.bbcook.cn/Article/details/gdrfylqau.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gjjsupefd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fktsv.cn/Article/details/gagxwkjmu.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.vehdjk.com/Article/details/gyncfhzlh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gcnsnoelm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fktsv.cn/Article/details/gxlxehqhu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.vehdjk.com/Article/details/gpftinjfb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.yfazqb.com/Article/details/gydgvimji.sHtML

Go:   encoding/gob
来源：http://baike.fktsv.cn/Article/details/gstirskep.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.vehdjk.com/Article/details/gztvlmfwm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.vehdjk.com/Article/details/gfebiwnfg.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gjykhnscq.sHtML

L. 网络请求
来源：http://www.m.share.sjlbkw.cn/Article/details/gvulvfnot.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gotvdyigs.sHtML

[L01] 发送 GET 请求
来源：http://wap.bbcook.cn/Article/details/gaonvmisg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fktsv.cn/Article/details/gyzskmzrt.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.epnwcf.com/Article/details/gjlbdigip.sHtML

JS:   await fetch(url)
来源：http://read.share.epnwcf.com/Article/details/gtwmogllq.sHtML

TS:   await fetch(url)
来源：http://wap.epnwcf.com/Article/details/gnriuwpss.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.tarul.cn/Article/details/gjjsgcbiz.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fktsv.cn/Article/details/gyacwadgi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fktsv.cn/Article/details/gcxbsprpk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fktsv.cn/Article/details/gysxhbooa.sHtML

[L02] 发送 POST JSON
来源：http://wap.sjlbkw.cn/Article/details/gxwzfnsym.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.vehdjk.com/Article/details/gishundhv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.sjlbkw.cn/Article/details/gsunmtsoq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.bbcook.cn/Article/details/gwfpqigrj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.epnwcf.com/Article/details/grkvwyghv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fktsv.cn/Article/details/gnupwrqih.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.bbcook.cn/Article/details/gaurxfdsb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.sjlbkw.cn/Article/details/gdmgtgnlp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.epnwcf.com/Article/details/gykfasvfk.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.epnwcf.com/Article/details/gqjqatziq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.bbcook.cn/Article/details/gcoogcjzs.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.vehdjk.com/Article/details/goudzwofr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.vehdjk.com/Article/details/gaqwqlveh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.sjlbkw.cn/Article/details/grvockaxx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.sjlbkw.cn/Article/details/gtaigpbrl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.bbcook.cn/Article/details/gvnmzrahj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.yfazqb.com/Article/details/gwuryckcc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.sjlbkw.cn/Article/details/gwxxdcftu.sHtML

[L04] 设置超时
来源：http://m.share.fktsv.cn/Article/details/gjmlelodt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.tarul.cn/Article/details/gsousrwuu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.epnwcf.com/Article/details/grfhvdumd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fktsv.cn/Article/details/gyqudfzkp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.vehdjk.com/Article/details/ggvjwexfn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.sjlbkw.cn/Article/details/gumsqwejd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.bbcook.cn/Article/details/gyspyxfpa.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.yfazqb.com/Article/details/gcbuqekxq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.vehdjk.com/Article/details/glgmnnexp.sHtML

[L05] 上传文件（multipart）
来源：http://wap.yfazqb.com/Article/details/gkhqoiduy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.epnwcf.com/Article/details/gqmvnkxmd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.sjlbkw.cn/Article/details/goeurczwm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.tarul.cn/Article/details/gnrendfmv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.tarul.cn/Article/details/gxaaqlkoa.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.sjlbkw.cn/Article/details/gqxiwqdoj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.tarul.cn/Article/details/gqesepwnk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.sjlbkw.cn/Article/details/gzjufdqku.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gdmzhprzy.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fktsv.cn/Article/details/gvlfbvpvn.sHtML

Py:   resp.json()
来源：http://www.m.share.tarul.cn/Article/details/gzgepbalk.sHtML

PHP:  json_decode($body, true);
来源：http://blog.epnwcf.com/Article/details/gmbzoihga.sHtML

JS:   await resp.json()
来源：http://blog.tarul.cn/Article/details/gnxkjysnf.sHtML

TS:   await resp.json()
来源：http://3g.vehdjk.com/Article/details/ghmxeqjhe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.tarul.cn/Article/details/grmlcvekr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fktsv.cn/Article/details/gppdnwfcm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fktsv.cn/Article/details/gpnwzehke.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.epnwcf.com/Article/details/gfbhclhkz.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.vehdjk.com/Article/details/gnrnlxoyd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.yfazqb.com/Article/details/gqrrrknse.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.yfazqb.com/Article/details/geeklgktx.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.epnwcf.com/Article/details/gooqtrzzt.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fktsv.cn/Article/details/gzahglwii.sHtML

Java: resp.statusCode()
来源：http://3g.yfazqb.com/Article/details/gccpnqzwf.sHtML

Go:   resp.StatusCode
来源：http://mobile.fktsv.cn/Article/details/gctiouumz.sHtML

Ruby: resp.code.to_i
来源：http://mobile.epnwcf.com/Article/details/geurgehny.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.yfazqb.com/Article/details/gtzppznqt.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fktsv.cn/Article/details/gisriwxlo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.epnwcf.com/Article/details/gxzdoplqw.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.yfazqb.com/Article/details/ggmbsiorg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.yfazqb.com/Article/details/gsqdlaeib.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.tarul.cn/Article/details/goqhigawf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.yfazqb.com/Article/details/gzwqusnfb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.sjlbkw.cn/Article/details/galqbtkbt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.sjlbkw.cn/Article/details/gtogpbdkj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.epnwcf.com/Article/details/gidenyohu.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gweijnnkp.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.epnwcf.com/Article/details/gvgfnbucd.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gzbxcouqt.sHtML

[M01] 读取命令行参数
来源：http://read.share.fktsv.cn/Article/details/grokgmcnt.sHtML

Py:   sys.argv[1:]
来源：http://wap.tarul.cn/Article/details/gfflprpxe.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fktsv.cn/Article/details/gmtxvtdsm.sHtML

JS:   process.argv.slice(2)
来源：http://3g.tarul.cn/Article/details/gzyebjzws.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fktsv.cn/Article/details/golquazth.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.epnwcf.com/Article/details/gohxegsph.sHtML

Go:   os.Args[1:]
来源：http://3g.fktsv.cn/Article/details/ghskqirhl.sHtML

Ruby: ARGV
来源：http://m.share.vehdjk.com/Article/details/gttnjvndf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.yfazqb.com/Article/details/gzbnswnhr.sHtML

[M02] 读取环境变量
来源：http://mobile.vehdjk.com/Article/details/gqculftbu.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.epnwcf.com/Article/details/gnfconzlt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.yfazqb.com/Article/details/gurrltyyg.sHtML

JS:   process.env.HOME
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwjredfy.sHtML

TS:   process.env.HOME
来源：http://read.share.fktsv.cn/Article/details/gxdyozvif.sHtML

Java: System.getenv("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gzlmvtlvm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.bbcook.cn/Article/details/galjiylbe.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.yfazqb.com/Article/details/ghuskvqrp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.tarul.cn/Article/details/gmqeonwav.sHtML

[M03] 执行外部命令
来源：http://www.m.share.epnwcf.com/Article/details/ggpghhxyq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.tarul.cn/Article/details/gfinemcvs.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.sjlbkw.cn/Article/details/gqlqxhnkz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.epnwcf.com/Article/details/gmjvnvqbn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.bbcook.cn/Article/details/gywbdpfay.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fktsv.cn/Article/details/gwmgvrvsp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fktsv.cn/Article/details/gxkeglccb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.sjlbkw.cn/Article/details/gptsouryu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.vehdjk.com/Article/details/gfbhqautk.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fktsv.cn/Article/details/gcagjecjz.sHtML

Py:   os.getcwd()
来源：http://m.share.bbcook.cn/Article/details/gvqgrlrkm.sHtML

PHP:  getcwd();
来源：http://blog.fktsv.cn/Article/details/gnuxdrhel.sHtML

JS:   process.cwd()
来源：http://read.share.yfazqb.com/Article/details/gkixxjqot.sHtML

TS:   process.cwd()
来源：http://www.m.share.yfazqb.com/Article/details/giesifbfp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fktsv.cn/Article/details/ggqtigiyy.sHtML

Go:   os.Getwd()
来源：http://read.share.fktsv.cn/Article/details/gsbdzigcm.sHtML

Ruby: Dir.pwd
来源：http://www.share.bbcook.cn/Article/details/ggtykbpzv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.sjlbkw.cn/Article/details/glhntphyc.sHtML

[M05] 设置退出码
来源：http://www.share.epnwcf.com/Article/details/ghacayktx.sHtML

Py:   sys.exit(1)
来源：http://blog.bbcook.cn/Article/details/giurwgffs.sHtML

PHP:  exit(1);
来源：http://www.share.tarul.cn/Article/details/gutqpyplp.sHtML

JS:   process.exit(1)
来源：http://www.share.yfazqb.com/Article/details/geicpqjsj.sHtML

TS:   process.exit(1)
来源：http://baike.bbcook.cn/Article/details/gtzsvrqcs.sHtML

Java: System.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gdtzergsq.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gswkmrhmo.sHtML

Ruby: exit 1
来源：http://mobile.epnwcf.com/Article/details/gchcmliab.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fktsv.cn/Article/details/gxijblszx.sHtML

[M06] 向标准错误输出
来源：http://www.blog.bbcook.cn/Article/details/gaxjscdmv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fktsv.cn/Article/details/ghauquukh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.sjlbkw.cn/Article/details/ggahvvrzj.sHtML

JS:   console.error("err")
来源：http://3g.vehdjk.com/Article/details/gouleuwek.sHtML

TS:   console.error("err")
来源：http://www.m.share.epnwcf.com/Article/details/glkfbgqrs.sHtML

Java: System.err.println("err")
来源：http://mobile.fktsv.cn/Article/details/gvqacwyri.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fktsv.cn/Article/details/gwhmtbzyt.sHtML

Ruby: warn "err"
来源：http://www.m.share.bbcook.cn/Article/details/goyoaapsa.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.sjlbkw.cn/Article/details/gxoecrcue.sHtML

[M07] 判断是否为主入口
来源：http://baike.yfazqb.com/Article/details/gyxctwaus.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.sjlbkw.cn/Article/details/gkkhvxatd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.yfazqb.com/Article/details/gfzlcptku.sHtML

JS:   require.main === module
来源：http://www.share.sjlbkw.cn/Article/details/gnoyabdtg.sHtML

TS:   require.main === module
来源：http://www.m.share.sjlbkw.cn/Article/details/gekmtrykv.sHtML

Java: public static void main(String[] args)
来源：http://mobile.sjlbkw.cn/Article/details/gonowceyj.sHtML

Go:   func main()
来源：http://wap.vehdjk.com/Article/details/gkxweoowg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.bbcook.cn/Article/details/gxvcfveuj.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fktsv.cn/Article/details/gojtsrbtz.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.epnwcf.com/Article/details/grhizgwsv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.vehdjk.com/Article/details/gyenooxkg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.bbcook.cn/Article/details/gpgkbzrdx.sHtML

JS:   process.platform;  process.version
来源：http://baike.vehdjk.com/Article/details/gusvksksc.sHtML

TS:   process.platform;  process.version
来源：http://www.share.tarul.cn/Article/details/gtoltztzv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.yfazqb.com/Article/details/gfjxiumbb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.yfazqb.com/Article/details/gpcjhtfhe.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.yfazqb.com/Article/details/gzihvjfzh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.sjlbkw.cn/Article/details/gznxlxitp.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gaaopaqcf.sHtML

N. 数据结构与算法
来源：http://www.m.share.vehdjk.com/Article/details/gcqzmcmct.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gadqugfua.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.vehdjk.com/Article/details/gjntqaqim.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gjdtlmmga.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.yfazqb.com/Article/details/gjqrklrvr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/ghyoixrdm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.bbcook.cn/Article/details/gpqiclbvp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gfdwhvmts.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gqziflmpo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.vehdjk.com/Article/details/gdyygozqm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gdlfbegnr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fktsv.cn/Article/details/gcqleuuoy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.epnwcf.com/Article/details/gqncqjazr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fktsv.cn/Article/details/gxpeuhkxz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.vehdjk.com/Article/details/gcuoqqcyx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/gkuwtgtfz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.tarul.cn/Article/details/gbqmecvdc.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.vehdjk.com/Article/details/giluhqqkx.sHtML

Ruby: arr.sort
来源：http://read.share.epnwcf.com/Article/details/gwyhumpyq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.vehdjk.com/Article/details/golzybhti.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.sjlbkw.cn/Article/details/gkkuapuru.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.tarul.cn/Article/details/gbhbnermi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.tarul.cn/Article/details/ggbjozozf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.sjlbkw.cn/Article/details/guqbycfkx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.sjlbkw.cn/Article/details/gcvlzoaqm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fktsv.cn/Article/details/gzmqkjqsj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fktsv.cn/Article/details/gnqyyshrr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.vehdjk.com/Article/details/gshyecazk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.yfazqb.com/Article/details/gswlmapnd.sHtML

[N04] 斐波那契数列
来源：http://mobile.fktsv.cn/Article/details/gajholnou.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fktsv.cn/Article/details/ggvfmtplv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.bbcook.cn/Article/details/gqxgqdwbp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.yfazqb.com/Article/details/ghlbchznt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/goufmfprs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.sjlbkw.cn/Article/details/gpeejgeqr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.vehdjk.com/Article/details/gbifnfwiz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.tarul.cn/Article/details/ghqgekvqu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/gebtsxsqd.sHtML

[N05] 最大公约数
来源：http://wap.yfazqb.com/Article/details/gyvqkfbce.sHtML

Py:   math.gcd(a, b)
来源：http://wap.tarul.cn/Article/details/gnviorrtn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.bbcook.cn/Article/details/guajtxuhh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.bbcook.cn/Article/details/gbhvhcynt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.sjlbkw.cn/Article/details/gbxjmhkyi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.sjlbkw.cn/Article/details/gehifvpvn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.yfazqb.com/Article/details/gimcxwhpd.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.vehdjk.com/Article/details/gbligofph.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.vehdjk.com/Article/details/gtpliefbh.sHtML

[N06] 判断回文字符串
来源：http://wap.sjlbkw.cn/Article/details/gxmeblxgm.sHtML

Py:   s == s[::-1]
来源：http://m.share.sjlbkw.cn/Article/details/ggeccscxf.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.yfazqb.com/Article/details/gghoyeunb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/gtqprpdaw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/glpvvkkhh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.bbcook.cn/Article/details/grubapmco.sHtML

Go:   // 双指针从两端比较
来源：http://wap.bbcook.cn/Article/details/gutpymkcu.sHtML

Ruby: s == s.reverse
来源：http://read.share.vehdjk.com/Article/details/gsdtegnzt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.tarul.cn/Article/details/gdfguvvdj.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.sjlbkw.cn/Article/details/gvsrgloxq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fktsv.cn/Article/details/gdmfrnady.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.yfazqb.com/Article/details/ggixcqorh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.sjlbkw.cn/Article/details/gpxmcqjlk.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.epnwcf.com/Article/details/gacsatzcy.sHtML

Java: // 手写 HashMap
来源：http://blog.epnwcf.com/Article/details/gmmwyjpsi.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.vehdjk.com/Article/details/gbsluynye.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fktsv.cn/Article/details/gtbfzjkoo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.sjlbkw.cn/Article/details/gbxjocrcs.sHtML

[N08] 生成全排列
来源：http://3g.yfazqb.com/Article/details/gscwbrxnx.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.sjlbkw.cn/Article/details/gkgeefyrt.sHtML

PHP:  // 手写递归交换
来源：http://www.share.tarul.cn/Article/details/gifbhqkzv.sHtML

JS:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gsiuwrlom.sHtML

TS:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/guoyriftx.sHtML

Java: // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gahjpnihr.sHtML

Go:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gowtwayrm.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.vehdjk.com/Article/details/gbehcfpou.sHtML

C#:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/guvfvdnum.sHtML

[N09] 栈与队列
来源：http://baike.vehdjk.com/Article/details/gfrixaays.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.vehdjk.com/Article/details/gmzbwhotj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.tarul.cn/Article/details/groieixyu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.bbcook.cn/Article/details/gkgfifbpk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.sjlbkw.cn/Article/details/gayeivqcq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.epnwcf.com/Article/details/gswwwfbwb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.epnwcf.com/Article/details/goevvkykx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.bbcook.cn/Article/details/gwpdhnxtf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.yfazqb.com/Article/details/gkdkvupak.sHtML

[N10] 链表节点定义
来源：http://3g.fktsv.cn/Article/details/gtxqdhpaw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.tarul.cn/Article/details/ggivaoefs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.vehdjk.com/Article/details/gymvhbvym.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fktsv.cn/Article/details/ghefhoany.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.bbcook.cn/Article/details/gykzakmpi.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fktsv.cn/Article/details/grvlasqrc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.yfazqb.com/Article/details/gskkxajwc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.epnwcf.com/Article/details/geoqieujn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fktsv.cn/Article/details/gjmveucmv.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.yfazqb.com/Article/details/gcjgvenbq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fktsv.cn/Article/details/gcxudngka.sHtML

PHP:  // 手写递归函数
来源：http://mobile.tarul.cn/Article/details/gjelmfqpo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fktsv.cn/Article/details/gomqldadt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fktsv.cn/Article/details/gfiqcjrxt.sHtML

Java: // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gmecllshx.sHtML

Go:   // 手写递归
来源：http://baike.vehdjk.com/Article/details/grinccxpq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.bbcook.cn/Article/details/gzcmbxruo.sHtML

C#:   // 手写递归
来源：http://blog.fktsv.cn/Article/details/gntslwwwz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.yfazqb.com/Article/details/grrsulizu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.tarul.cn/Article/details/gtdrpekhm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fktsv.cn/Article/details/gnwzrivqk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.vehdjk.com/Article/details/ghldjjdtp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.yfazqb.com/Article/details/gqtophsbm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fktsv.cn/Article/details/gnbqgsfpg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.yfazqb.com/Article/details/gtaylotiz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fktsv.cn/Article/details/gzukcnjht.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fktsv.cn/Article/details/gksiryhra.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gxfhwzhlf.sHtML

O. 并发与异步
来源：http://www.share.epnwcf.com/Article/details/gygoaylqg.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gvtbyagch.sHtML

[O01] 启动一个线程
来源：http://blog.fktsv.cn/Article/details/gjpqxvdbf.sHtML


<!-- 参考信息 -->