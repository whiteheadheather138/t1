代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fktsv.cn/Article/details/gpquhthpm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.sjlbkw.cn/Article/details/ggcbedrhd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.bbcook.cn/Article/details/gusdtsmsx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.sjlbkw.cn/Article/details/gczpdybnu.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fktsv.cn/Article/details/gyygchswm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.sjlbkw.cn/Article/details/gawnarnax.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fktsv.cn/Article/details/gijjygwuu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.sjlbkw.cn/Article/details/gznxqcctt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.bbcook.cn/Article/details/gjmertwyd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.tarul.cn/Article/details/grkaabvte.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/gyljflrii.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.tarul.cn/Article/details/gasammnze.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.sjlbkw.cn/Article/details/gijjvyxsh.sHtML

[K07] 进制转换
来源：http://baike.yfazqb.com/Article/details/gsgcyeyjj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.epnwcf.com/Article/details/grpfxmsdn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.vehdjk.com/Article/details/gbgiarhil.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gfigxuwax.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/geqhmlqlm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gtjncuwck.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.epnwcf.com/Article/details/grtjmlbux.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.yfazqb.com/Article/details/gozajfzfc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsmlzwyn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.tarul.cn/Article/details/gdugngrzg.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.epnwcf.com/Article/details/gltxlydaf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.vehdjk.com/Article/details/gafycqsun.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fktsv.cn/Article/details/gxhhypxxz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fktsv.cn/Article/details/ggdlfbugp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.yfazqb.com/Article/details/gqkjxqcdk.sHtML

Go:   encoding/gob
来源：http://m.share.vehdjk.com/Article/details/ggawvmtwt.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.epnwcf.com/Article/details/gpdfzzkzd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fktsv.cn/Article/details/gasxqpdnu.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gqktyvfkq.sHtML

L. 网络请求
来源：http://www.share.sjlbkw.cn/Article/details/gvkafrruk.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/glnhzhkwy.sHtML

[L01] 发送 GET 请求
来源：http://www.share.tarul.cn/Article/details/ggsgevwsl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fktsv.cn/Article/details/gzvztiico.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.bbcook.cn/Article/details/gtgucklws.sHtML

JS:   await fetch(url)
来源：http://baike.fktsv.cn/Article/details/gakgcmywk.sHtML

TS:   await fetch(url)
来源：http://www.blog.yfazqb.com/Article/details/gvafiqxff.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.tarul.cn/Article/details/geiejvyti.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.bbcook.cn/Article/details/gsrbiugmj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.epnwcf.com/Article/details/gysdhtnuh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.yfazqb.com/Article/details/gftjtgair.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.bbcook.cn/Article/details/gvqunbfvc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.yfazqb.com/Article/details/gvdhgijbv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.bbcook.cn/Article/details/ggqkfvvhx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fktsv.cn/Article/details/gvinwyyfl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fktsv.cn/Article/details/gbefqpzvq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.yfazqb.com/Article/details/gvsgtnqho.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.vehdjk.com/Article/details/gjszndivj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.bbcook.cn/Article/details/gxptiervd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.yfazqb.com/Article/details/ggqpqcobb.sHtML

[L03] 设置自定义请求头
来源：http://mobile.tarul.cn/Article/details/gykpmgezg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fktsv.cn/Article/details/gqejeqdgq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fktsv.cn/Article/details/gzprzyqxy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.vehdjk.com/Article/details/gwhndfvju.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.yfazqb.com/Article/details/gryldwedt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fktsv.cn/Article/details/gtpblczgx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.epnwcf.com/Article/details/gkeujkegn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.tarul.cn/Article/details/gtxydatmu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.vehdjk.com/Article/details/gfrhwktxc.sHtML

[L04] 设置超时
来源：http://www.blog.fktsv.cn/Article/details/grexykizf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.yfazqb.com/Article/details/gsutqshiz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.tarul.cn/Article/details/gimurhrry.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.vehdjk.com/Article/details/gozqtmxjt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.tarul.cn/Article/details/gnuskgegd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.epnwcf.com/Article/details/gptrxibko.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.tarul.cn/Article/details/gizpnidyu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.bbcook.cn/Article/details/gywbljtus.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.epnwcf.com/Article/details/gdvtawtua.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.yfazqb.com/Article/details/gcckjcmav.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.tarul.cn/Article/details/glojireoj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.tarul.cn/Article/details/gacenxlix.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.tarul.cn/Article/details/gvfirtxit.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.bbcook.cn/Article/details/goiuejeyk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.sjlbkw.cn/Article/details/gxgxrsuii.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.sjlbkw.cn/Article/details/ggvameoen.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.vehdjk.com/Article/details/ghtwazlbv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.tarul.cn/Article/details/glsxzhcho.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.bbcook.cn/Article/details/ghqaxtwnm.sHtML

Py:   resp.json()
来源：http://baike.yfazqb.com/Article/details/gdmdaavcn.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.yfazqb.com/Article/details/ghxrzisvv.sHtML

JS:   await resp.json()
来源：http://read.share.epnwcf.com/Article/details/gsxsjjprf.sHtML

TS:   await resp.json()
来源：http://mobile.tarul.cn/Article/details/gfccktmgx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fktsv.cn/Article/details/gtduydwvx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fktsv.cn/Article/details/gelelpwrn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.yfazqb.com/Article/details/gfoilpwmj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.epnwcf.com/Article/details/gmhascuny.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.epnwcf.com/Article/details/gykedwihy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.vehdjk.com/Article/details/gcslmewng.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.yfazqb.com/Article/details/gnnkujluu.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.yfazqb.com/Article/details/giptlblze.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.yfazqb.com/Article/details/ggsntopnw.sHtML

Java: resp.statusCode()
来源：http://mobile.bbcook.cn/Article/details/gtwcziifv.sHtML

Go:   resp.StatusCode
来源：http://wap.sjlbkw.cn/Article/details/gjparjlyv.sHtML

Ruby: resp.code.to_i
来源：http://3g.yfazqb.com/Article/details/ggjyvxtot.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.tarul.cn/Article/details/grrjkndff.sHtML

[L08] 并发请求多个地址
来源：http://m.share.epnwcf.com/Article/details/geizbjniw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fktsv.cn/Article/details/gxylaggih.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.bbcook.cn/Article/details/glacegbmn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.yfazqb.com/Article/details/gvsyxdydm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.yfazqb.com/Article/details/gtxtslhzq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.vehdjk.com/Article/details/gfzipnbln.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fktsv.cn/Article/details/gjcccepjj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.bbcook.cn/Article/details/grtfjqweb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fktsv.cn/Article/details/gzwjiclag.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gfmwokbsv.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.epnwcf.com/Article/details/gdyzsjnpv.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gfupctsqc.sHtML

[M01] 读取命令行参数
来源：http://wap.sjlbkw.cn/Article/details/gprlzbtri.sHtML

Py:   sys.argv[1:]
来源：http://www.share.vehdjk.com/Article/details/gratltwir.sHtML

PHP:  $argv;  $argc;
来源：http://blog.vehdjk.com/Article/details/grodmnvdd.sHtML

JS:   process.argv.slice(2)
来源：http://blog.sjlbkw.cn/Article/details/gtviqpaje.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.tarul.cn/Article/details/gocipwhgf.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.sjlbkw.cn/Article/details/gqatydymm.sHtML

Go:   os.Args[1:]
来源：http://read.share.epnwcf.com/Article/details/gavajfgss.sHtML

Ruby: ARGV
来源：http://wap.yfazqb.com/Article/details/gahqlqypq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.epnwcf.com/Article/details/gnhsnbscr.sHtML

[M02] 读取环境变量
来源：http://www.blog.tarul.cn/Article/details/gejizhdur.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.epnwcf.com/Article/details/gdjxtohbg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.tarul.cn/Article/details/guqjrxmvr.sHtML

JS:   process.env.HOME
来源：http://www.blog.bbcook.cn/Article/details/gslbljipq.sHtML

TS:   process.env.HOME
来源：http://mobile.yfazqb.com/Article/details/gdptfzhol.sHtML

Java: System.getenv("HOME")
来源：http://mobile.bbcook.cn/Article/details/gbehybgyr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.tarul.cn/Article/details/gjeidxmkd.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.tarul.cn/Article/details/gezhdkmie.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.bbcook.cn/Article/details/gbqyzkthn.sHtML

[M03] 执行外部命令
来源：http://www.share.bbcook.cn/Article/details/gzspkyzlq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.yfazqb.com/Article/details/grhgchwsp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.bbcook.cn/Article/details/guzvdmpxq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.bbcook.cn/Article/details/gowpoavav.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.tarul.cn/Article/details/gujvgfhij.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fktsv.cn/Article/details/gjtwyggdk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.vehdjk.com/Article/details/gklnvhrmg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fktsv.cn/Article/details/gqzexungp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.bbcook.cn/Article/details/gtwfrmmjo.sHtML

[M04] 获取当前工作目录
来源：http://m.share.epnwcf.com/Article/details/grjrknhin.sHtML

Py:   os.getcwd()
来源：http://blog.yfazqb.com/Article/details/gleddyhru.sHtML

PHP:  getcwd();
来源：http://www.m.share.tarul.cn/Article/details/ghmqmemtt.sHtML

JS:   process.cwd()
来源：http://www.share.vehdjk.com/Article/details/gvpqeslwt.sHtML

TS:   process.cwd()
来源：http://www.blog.epnwcf.com/Article/details/ggkeazmkh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.yfazqb.com/Article/details/gozyjhjdm.sHtML

Go:   os.Getwd()
来源：http://baike.bbcook.cn/Article/details/ggogxpend.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.sjlbkw.cn/Article/details/gltterzxi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.bbcook.cn/Article/details/gzfgpxlsf.sHtML

[M05] 设置退出码
来源：http://3g.epnwcf.com/Article/details/gnuvrsxls.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gzlhvypts.sHtML

PHP:  exit(1);
来源：http://baike.bbcook.cn/Article/details/gozvrmhyt.sHtML

JS:   process.exit(1)
来源：http://blog.bbcook.cn/Article/details/guxjqktou.sHtML

TS:   process.exit(1)
来源：http://read.share.vehdjk.com/Article/details/ggqpbztdl.sHtML

Java: System.exit(1)
来源：http://wap.bbcook.cn/Article/details/geumwpdlu.sHtML

Go:   os.Exit(1)
来源：http://wap.bbcook.cn/Article/details/gjhwoaitq.sHtML

Ruby: exit 1
来源：http://m.share.sjlbkw.cn/Article/details/gdwuvzsfx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.yfazqb.com/Article/details/guqjhlwie.sHtML

[M06] 向标准错误输出
来源：http://mobile.bbcook.cn/Article/details/gvcekqdfd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.sjlbkw.cn/Article/details/gdoldekxb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fktsv.cn/Article/details/gxdhtwbki.sHtML

JS:   console.error("err")
来源：http://wap.epnwcf.com/Article/details/gkgefaouy.sHtML

TS:   console.error("err")
来源：http://mobile.vehdjk.com/Article/details/gddevqhkk.sHtML

Java: System.err.println("err")
来源：http://mobile.fktsv.cn/Article/details/gabdxfaot.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.epnwcf.com/Article/details/grsvfaqvg.sHtML

Ruby: warn "err"
来源：http://www.share.bbcook.cn/Article/details/gnwjkdtls.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.tarul.cn/Article/details/glamnskdv.sHtML

[M07] 判断是否为主入口
来源：http://baike.sjlbkw.cn/Article/details/gqzibyqxs.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.sjlbkw.cn/Article/details/gdcfelkaw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.bbcook.cn/Article/details/gyaqftvak.sHtML

JS:   require.main === module
来源：http://mobile.epnwcf.com/Article/details/gaxsvjdsd.sHtML

TS:   require.main === module
来源：http://3g.epnwcf.com/Article/details/gyaedjett.sHtML

Java: public static void main(String[] args)
来源：http://mobile.bbcook.cn/Article/details/gpcnmjkvl.sHtML

Go:   func main()
来源：http://3g.bbcook.cn/Article/details/ghbqkqcxj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fktsv.cn/Article/details/gkbbaogcc.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.vehdjk.com/Article/details/gygqvumys.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.bbcook.cn/Article/details/gatkrpbqh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.tarul.cn/Article/details/gptxustwh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.sjlbkw.cn/Article/details/gjqfswmnq.sHtML

JS:   process.platform;  process.version
来源：http://baike.bbcook.cn/Article/details/gjenuqmao.sHtML

TS:   process.platform;  process.version
来源：http://m.share.epnwcf.com/Article/details/gyfficnll.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.epnwcf.com/Article/details/gennavsnf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.yfazqb.com/Article/details/ghwntmgxn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.vehdjk.com/Article/details/gxhsqbdvh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fktsv.cn/Article/details/gnyaetluh.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gwcbqmciz.sHtML

N. 数据结构与算法
来源：http://blog.vehdjk.com/Article/details/gevjvlkil.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gutiozybr.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.yfazqb.com/Article/details/gziifqgaw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gvlxdehdo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.bbcook.cn/Article/details/gfystohmc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.vehdjk.com/Article/details/gcokimkli.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.epnwcf.com/Article/details/glizergyd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gcpohobrp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.yfazqb.com/Article/details/ginetswmi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.tarul.cn/Article/details/gmwsskxbh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.epnwcf.com/Article/details/gnrdpndjx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.yfazqb.com/Article/details/gzleiwkzw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.bbcook.cn/Article/details/grabngmhn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.sjlbkw.cn/Article/details/gfurhmoaf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.vehdjk.com/Article/details/ggaixvpuc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.vehdjk.com/Article/details/grllupbkr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.bbcook.cn/Article/details/gizljcwaw.sHtML

Go:   slices.Sort(arr)
来源：http://blog.yfazqb.com/Article/details/gkfyqayqk.sHtML

Ruby: arr.sort
来源：http://wap.yfazqb.com/Article/details/gpauqjhwd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.sjlbkw.cn/Article/details/gxtpvhvtq.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.tarul.cn/Article/details/ggjxxpbay.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.epnwcf.com/Article/details/gilnmgeew.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.yfazqb.com/Article/details/gvdxnjsvc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.yfazqb.com/Article/details/gzgpnbrek.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.tarul.cn/Article/details/gxvpxevnk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.sjlbkw.cn/Article/details/gvcvlzidt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fktsv.cn/Article/details/ggdhjmbqx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.tarul.cn/Article/details/gzklhmxpf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.vehdjk.com/Article/details/gsocvwnoc.sHtML

[N04] 斐波那契数列
来源：http://read.share.vehdjk.com/Article/details/guwwopwgt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.bbcook.cn/Article/details/gunrxvwnp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.vehdjk.com/Article/details/gbmmkpcft.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fktsv.cn/Article/details/gnovkgvgm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.bbcook.cn/Article/details/gwpcllaav.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.yfazqb.com/Article/details/gsjbyucik.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.vehdjk.com/Article/details/gtnbxxhgm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.yfazqb.com/Article/details/gwivpehbh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.epnwcf.com/Article/details/gmwuaezqf.sHtML

[N05] 最大公约数
来源：http://www.blog.vehdjk.com/Article/details/gmfsnfwom.sHtML

Py:   math.gcd(a, b)
来源：http://wap.bbcook.cn/Article/details/gmumcqoqu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.sjlbkw.cn/Article/details/gkzkzcsmm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.vehdjk.com/Article/details/gptypagjk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.bbcook.cn/Article/details/gfpwtjeuu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fktsv.cn/Article/details/gawkfvach.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.vehdjk.com/Article/details/gswxctrav.sHtML

Ruby: a.gcd(b)
来源：http://mobile.epnwcf.com/Article/details/gydzejcjc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.vehdjk.com/Article/details/gffqaekeg.sHtML

[N06] 判断回文字符串
来源：http://www.blog.epnwcf.com/Article/details/gjcejmmwf.sHtML

Py:   s == s[::-1]
来源：http://www.blog.yfazqb.com/Article/details/gkorxtfhs.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fktsv.cn/Article/details/gdyeacvqv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/gxyzvxncw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gsoalzcpm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.vehdjk.com/Article/details/gemthyecj.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.epnwcf.com/Article/details/gspghqhaj.sHtML

Ruby: s == s.reverse
来源：http://wap.epnwcf.com/Article/details/gbkdjyqno.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.sjlbkw.cn/Article/details/gnetyewez.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.vehdjk.com/Article/details/gfspvjtmw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fktsv.cn/Article/details/gndaueljr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.epnwcf.com/Article/details/gznpjuxoy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.bbcook.cn/Article/details/gorecqalz.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.yfazqb.com/Article/details/gmalpeecf.sHtML

Java: // 手写 HashMap
来源：http://blog.bbcook.cn/Article/details/gygugzdhv.sHtML

Go:   // 手写 map[int]int
来源：http://baike.tarul.cn/Article/details/gqldcemhf.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.tarul.cn/Article/details/gajtzlvtz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.tarul.cn/Article/details/grzylhkcu.sHtML

[N08] 生成全排列
来源：http://read.share.fktsv.cn/Article/details/giikmlpgv.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.bbcook.cn/Article/details/gztnmkkzp.sHtML

PHP:  // 手写递归交换
来源：http://3g.yfazqb.com/Article/details/gidaxmshk.sHtML

JS:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gwfyxmyma.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gjbrpxfls.sHtML

Java: // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gxtjshjrn.sHtML

Go:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gmflxpnhy.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.yfazqb.com/Article/details/ghargvowa.sHtML

C#:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gxsxqktos.sHtML

[N09] 栈与队列
来源：http://www.m.share.epnwcf.com/Article/details/glhpuutac.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.vehdjk.com/Article/details/gryzfkvty.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fktsv.cn/Article/details/gchglppnl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.tarul.cn/Article/details/gfcdlgqeu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.vehdjk.com/Article/details/ggbaufzsy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fktsv.cn/Article/details/gksvvlqzb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.epnwcf.com/Article/details/gxvanuzhw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.tarul.cn/Article/details/gmzvfvdjd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwztfbgv.sHtML

[N10] 链表节点定义
来源：http://baike.epnwcf.com/Article/details/gqbtasovg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.yfazqb.com/Article/details/glvtfgpes.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.yfazqb.com/Article/details/gbmwtpxjg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.epnwcf.com/Article/details/ggujpnckf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.yfazqb.com/Article/details/gbcvgyvjl.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.tarul.cn/Article/details/gldruipnx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.tarul.cn/Article/details/gyuhblvhd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.epnwcf.com/Article/details/gaogbvjkx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.epnwcf.com/Article/details/gluszkztp.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.yfazqb.com/Article/details/ggnafoclc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.bbcook.cn/Article/details/gkqkrupkn.sHtML

PHP:  // 手写递归函数
来源：http://wap.fktsv.cn/Article/details/gettxvkzd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fktsv.cn/Article/details/govvefucx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.yfazqb.com/Article/details/gulkiwyzl.sHtML

Java: // 手写递归
来源：http://www.blog.tarul.cn/Article/details/gsuuzejvw.sHtML

Go:   // 手写递归
来源：http://www.blog.tarul.cn/Article/details/getnodtmc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.epnwcf.com/Article/details/gaybphpzz.sHtML

C#:   // 手写递归
来源：http://3g.tarul.cn/Article/details/gmsderfkw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.yfazqb.com/Article/details/gblxysswg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.yfazqb.com/Article/details/gkolghgni.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.epnwcf.com/Article/details/gzhklegzj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.vehdjk.com/Article/details/geeihxorl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.yfazqb.com/Article/details/geldzpuql.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.epnwcf.com/Article/details/gepwlifvm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.yfazqb.com/Article/details/gdtfbvpcr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.tarul.cn/Article/details/gmnqvcrdo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.bbcook.cn/Article/details/gpvkbkzci.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gzpfachrn.sHtML

O. 并发与异步
来源：http://3g.sjlbkw.cn/Article/details/gkdsqbwxh.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gffiujazk.sHtML

[O01] 启动一个线程
来源：http://3g.yfazqb.com/Article/details/gbcjczkgh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.tarul.cn/Article/details/guyctphan.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.sjlbkw.cn/Article/details/gzldazjpi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.sjlbkw.cn/Article/details/grmpblbyt.sHtML

TS:   // 同 JS
来源：http://baike.fktsv.cn/Article/details/gaedbowus.sHtML


<!-- 参考信息 -->