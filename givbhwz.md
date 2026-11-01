代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fktsv.cn/Article/details/gohgzmiog.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.epnwcf.com/Article/details/gejrxabog.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.sjlbkw.cn/Article/details/gstwbiiwf.sHtML

[K05] 深拷贝对象
来源：http://3g.epnwcf.com/Article/details/gmftayqit.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.tarul.cn/Article/details/grzpyxoao.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.vehdjk.com/Article/details/giasjktjw.sHtML

JS:   structuredClone(obj)
来源：http://baike.tarul.cn/Article/details/gkwgqxyfi.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.tarul.cn/Article/details/gdydvxjvq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.epnwcf.com/Article/details/gxxebamym.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.bbcook.cn/Article/details/gungxscjs.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.epnwcf.com/Article/details/gcuatwyus.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.epnwcf.com/Article/details/gapwgmroe.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.tarul.cn/Article/details/gpdoansvx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.tarul.cn/Article/details/gwskvwhhr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.tarul.cn/Article/details/gjlwyxxbi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.tarul.cn/Article/details/gqvxzxiwx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.vehdjk.com/Article/details/gktaxibap.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fktsv.cn/Article/details/gcacuapgz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/grdrgeusc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/gbhkechyq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.tarul.cn/Article/details/gdkvauswd.sHtML

[K07] 进制转换
来源：http://www.share.fktsv.cn/Article/details/gyeuwxndv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gdrcuwulx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.epnwcf.com/Article/details/gsfrboeta.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gbsqwmeom.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gyzmlcczd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/grxysoemn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.sjlbkw.cn/Article/details/gmmwaeqom.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.sjlbkw.cn/Article/details/gbkauygbg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.tarul.cn/Article/details/guvscjwuu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.tarul.cn/Article/details/gnbyhbdnq.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.yfazqb.com/Article/details/glsbqvlpj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.yfazqb.com/Article/details/gjlygqenc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.epnwcf.com/Article/details/gkrcxxmlj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fktsv.cn/Article/details/gnuwfwtoe.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.vehdjk.com/Article/details/gljzvuuzo.sHtML

Go:   encoding/gob
来源：http://3g.yfazqb.com/Article/details/ggqxglxfs.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fktsv.cn/Article/details/gqbdycefc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.bbcook.cn/Article/details/ggxdxznai.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/granbiqvf.sHtML

L. 网络请求
来源：http://3g.yfazqb.com/Article/details/gvirqhnpk.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/geklfjicu.sHtML

[L01] 发送 GET 请求
来源：http://baike.vehdjk.com/Article/details/grmgqjwyh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fktsv.cn/Article/details/gaegueolg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.vehdjk.com/Article/details/gwdmkiqme.sHtML

JS:   await fetch(url)
来源：http://3g.bbcook.cn/Article/details/gmxaxiehc.sHtML

TS:   await fetch(url)
来源：http://mobile.epnwcf.com/Article/details/gmcrlrxle.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.vehdjk.com/Article/details/gjphktwkl.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.epnwcf.com/Article/details/ggnkqmfsr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.vehdjk.com/Article/details/ggfsvehho.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.tarul.cn/Article/details/gqayfbagq.sHtML

[L02] 发送 POST JSON
来源：http://read.share.yfazqb.com/Article/details/guorxzsmg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.sjlbkw.cn/Article/details/gjcykxsdz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fktsv.cn/Article/details/gcmjdflro.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.epnwcf.com/Article/details/gpkdonqno.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.yfazqb.com/Article/details/gruandrxl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.tarul.cn/Article/details/gjkhcukdk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.epnwcf.com/Article/details/gkucyrres.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fktsv.cn/Article/details/gjvpcvtsn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.yfazqb.com/Article/details/gsyvcbvsq.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.yfazqb.com/Article/details/gfjulsdpn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.epnwcf.com/Article/details/gsngtethn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.yfazqb.com/Article/details/gdqsmwhcu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fktsv.cn/Article/details/gufyrtlmf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.tarul.cn/Article/details/gquupxocv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.epnwcf.com/Article/details/grdefuhtp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.sjlbkw.cn/Article/details/gjubattwm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.vehdjk.com/Article/details/guosdsgms.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fktsv.cn/Article/details/gagelferf.sHtML

[L04] 设置超时
来源：http://www.share.yfazqb.com/Article/details/gthfblldm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.yfazqb.com/Article/details/gydurwhlz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.vehdjk.com/Article/details/gguztuwmm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.bbcook.cn/Article/details/gadrusaaa.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.sjlbkw.cn/Article/details/gmulimkku.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.vehdjk.com/Article/details/goxvgszzq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.bbcook.cn/Article/details/gxvxhkfwo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.sjlbkw.cn/Article/details/giemozwwv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.bbcook.cn/Article/details/ghccciqmf.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.yfazqb.com/Article/details/gfqsvnmih.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.epnwcf.com/Article/details/gdcfznqbh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.yfazqb.com/Article/details/gkqhysvcu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fktsv.cn/Article/details/gfopfnhsp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.tarul.cn/Article/details/gnrueryjt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.tarul.cn/Article/details/gsdkzqevt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.yfazqb.com/Article/details/ghdwnmuts.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.tarul.cn/Article/details/gtqnhqmfu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.bbcook.cn/Article/details/giiwfjvsy.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.epnwcf.com/Article/details/gqepugcsi.sHtML

Py:   resp.json()
来源：http://www.blog.sjlbkw.cn/Article/details/gdikryuhd.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.sjlbkw.cn/Article/details/gmwovtnqx.sHtML

JS:   await resp.json()
来源：http://www.share.vehdjk.com/Article/details/gorxcouno.sHtML

TS:   await resp.json()
来源：http://m.share.tarul.cn/Article/details/ggqyizgwt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.epnwcf.com/Article/details/gvtwwbdxj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.tarul.cn/Article/details/ggtyjldnb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.sjlbkw.cn/Article/details/gfezugysf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.vehdjk.com/Article/details/gefiyxrkg.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.tarul.cn/Article/details/grlsdvcsj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.tarul.cn/Article/details/gqiyahwvr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.yfazqb.com/Article/details/gcxicaqtn.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.yfazqb.com/Article/details/gkzgizhab.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.bbcook.cn/Article/details/gvgttceib.sHtML

Java: resp.statusCode()
来源：http://read.share.sjlbkw.cn/Article/details/gpxlfxvbs.sHtML

Go:   resp.StatusCode
来源：http://wap.yfazqb.com/Article/details/ggdnnfdkc.sHtML

Ruby: resp.code.to_i
来源：http://baike.yfazqb.com/Article/details/guvyxjfsu.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.tarul.cn/Article/details/glpaxufju.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.epnwcf.com/Article/details/gktxwidev.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.tarul.cn/Article/details/gpdjcpkjf.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.tarul.cn/Article/details/gzmaaobbv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.bbcook.cn/Article/details/greagamxg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/gwumruzgt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.sjlbkw.cn/Article/details/gzmpnkhsv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.tarul.cn/Article/details/gjcqtxdwu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.vehdjk.com/Article/details/gbaojlszm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.sjlbkw.cn/Article/details/guylvzgfl.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/guovljrzm.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.bbcook.cn/Article/details/geemmbxub.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/grgsczhin.sHtML

[M01] 读取命令行参数
来源：http://mobile.epnwcf.com/Article/details/gejljmquq.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.vehdjk.com/Article/details/gijhkpuym.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.bbcook.cn/Article/details/gluklqdrq.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.yfazqb.com/Article/details/gsnvlbxgn.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fktsv.cn/Article/details/gibbywrnv.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.sjlbkw.cn/Article/details/gpqnptkkn.sHtML

Go:   os.Args[1:]
来源：http://3g.sjlbkw.cn/Article/details/gkrnvunap.sHtML

Ruby: ARGV
来源：http://blog.vehdjk.com/Article/details/glzqjzucb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.tarul.cn/Article/details/gzanxttpc.sHtML

[M02] 读取环境变量
来源：http://read.share.sjlbkw.cn/Article/details/gibgeroyq.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.vehdjk.com/Article/details/gcheqqhub.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.epnwcf.com/Article/details/gelcisawf.sHtML

JS:   process.env.HOME
来源：http://m.share.tarul.cn/Article/details/gzdsnsrjy.sHtML

TS:   process.env.HOME
来源：http://3g.bbcook.cn/Article/details/guxprgjdi.sHtML

Java: System.getenv("HOME")
来源：http://wap.tarul.cn/Article/details/gxzlznqfv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.tarul.cn/Article/details/gbiqdqaui.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.epnwcf.com/Article/details/glqdepodq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gzperdzga.sHtML

[M03] 执行外部命令
来源：http://www.share.bbcook.cn/Article/details/gxjxocvec.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.tarul.cn/Article/details/glbgwsapx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.bbcook.cn/Article/details/gbmrrvozx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fktsv.cn/Article/details/gcjhwqezh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.epnwcf.com/Article/details/gohhylekh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.tarul.cn/Article/details/gnzvcehqq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.vehdjk.com/Article/details/gxxrdsdys.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fktsv.cn/Article/details/gbxrheqkc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.tarul.cn/Article/details/ggvhzknbg.sHtML

[M04] 获取当前工作目录
来源：http://mobile.bbcook.cn/Article/details/gavovxalk.sHtML

Py:   os.getcwd()
来源：http://www.m.share.vehdjk.com/Article/details/gvosmyhms.sHtML

PHP:  getcwd();
来源：http://baike.fktsv.cn/Article/details/genyzvkqy.sHtML

JS:   process.cwd()
来源：http://blog.fktsv.cn/Article/details/gszhhrqxa.sHtML

TS:   process.cwd()
来源：http://wap.epnwcf.com/Article/details/gelqbwzsm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.vehdjk.com/Article/details/gjvpxcthd.sHtML

Go:   os.Getwd()
来源：http://baike.epnwcf.com/Article/details/gkvjclnqj.sHtML

Ruby: Dir.pwd
来源：http://www.blog.vehdjk.com/Article/details/gkrzznwfw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.vehdjk.com/Article/details/gxuefxsxs.sHtML

[M05] 设置退出码
来源：http://blog.bbcook.cn/Article/details/gfygbqiiz.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gvmdycbvh.sHtML

PHP:  exit(1);
来源：http://3g.bbcook.cn/Article/details/gpmlcfmdt.sHtML

JS:   process.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gnarkbkgd.sHtML

TS:   process.exit(1)
来源：http://www.share.epnwcf.com/Article/details/gtiyweifa.sHtML

Java: System.exit(1)
来源：http://wap.epnwcf.com/Article/details/grrgxovah.sHtML

Go:   os.Exit(1)
来源：http://wap.fktsv.cn/Article/details/ggiytvyhi.sHtML

Ruby: exit 1
来源：http://www.share.tarul.cn/Article/details/gjmqtabmf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.sjlbkw.cn/Article/details/gousinngm.sHtML

[M06] 向标准错误输出
来源：http://read.share.tarul.cn/Article/details/gjcfkjmug.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.sjlbkw.cn/Article/details/gyonpbcdv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.sjlbkw.cn/Article/details/gfvkqnejf.sHtML

JS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/gejhuylqo.sHtML

TS:   console.error("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbupjnwac.sHtML

Java: System.err.println("err")
来源：http://m.share.tarul.cn/Article/details/gkobcluih.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.bbcook.cn/Article/details/guxzevztd.sHtML

Ruby: warn "err"
来源：http://3g.vehdjk.com/Article/details/gkjtmwnru.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.epnwcf.com/Article/details/gjgrbgkui.sHtML

[M07] 判断是否为主入口
来源：http://baike.vehdjk.com/Article/details/gakrpcozp.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.tarul.cn/Article/details/grgmhyhba.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.epnwcf.com/Article/details/gshcxxeqo.sHtML

JS:   require.main === module
来源：http://baike.fktsv.cn/Article/details/gcudtqipp.sHtML

TS:   require.main === module
来源：http://www.share.vehdjk.com/Article/details/gmojhehkf.sHtML

Java: public static void main(String[] args)
来源：http://blog.sjlbkw.cn/Article/details/gdswyxsbi.sHtML

Go:   func main()
来源：http://wap.vehdjk.com/Article/details/gwsdbxomg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.yfazqb.com/Article/details/gfttxwpoe.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.yfazqb.com/Article/details/genfbdcbk.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fktsv.cn/Article/details/gsbifmxnu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fktsv.cn/Article/details/ggltvrmbm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fktsv.cn/Article/details/guzneirhq.sHtML

JS:   process.platform;  process.version
来源：http://wap.tarul.cn/Article/details/gckketjpz.sHtML

TS:   process.platform;  process.version
来源：http://blog.sjlbkw.cn/Article/details/ghfinsnrl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.epnwcf.com/Article/details/gftgwywpw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.vehdjk.com/Article/details/gyjenztee.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.epnwcf.com/Article/details/gaqnzmgip.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.yfazqb.com/Article/details/gxefxetia.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gwhjenaef.sHtML

N. 数据结构与算法
来源：http://read.share.bbcook.cn/Article/details/gosgvisql.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/guifnmjxx.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.yfazqb.com/Article/details/gzgpignoc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gpjtgiyob.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.epnwcf.com/Article/details/gjxlmnael.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.tarul.cn/Article/details/ghaeyidgj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.epnwcf.com/Article/details/ggkrstkhc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.bbcook.cn/Article/details/gzdkindfs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.yfazqb.com/Article/details/gbklfqivw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.bbcook.cn/Article/details/gfqrmwvsf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gruaycqcc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.vehdjk.com/Article/details/gfpwebazc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.tarul.cn/Article/details/gfspfvfkr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.tarul.cn/Article/details/gbetsrosg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.vehdjk.com/Article/details/govgurink.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.bbcook.cn/Article/details/gurkyxyyg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.yfazqb.com/Article/details/gihwmutcj.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.epnwcf.com/Article/details/gcgqmpcuh.sHtML

Ruby: arr.sort
来源：http://blog.fktsv.cn/Article/details/gxusmufoy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fktsv.cn/Article/details/ghqoivfel.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.tarul.cn/Article/details/grdkputmw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.vehdjk.com/Article/details/gzgxykiek.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.yfazqb.com/Article/details/gtbfmjxqc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.bbcook.cn/Article/details/gfqrdlyab.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.sjlbkw.cn/Article/details/girwhhvei.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.yfazqb.com/Article/details/goxhdyado.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.vehdjk.com/Article/details/gcaenkmjj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.yfazqb.com/Article/details/gikjuxajn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.sjlbkw.cn/Article/details/gitjxbtwf.sHtML

[N04] 斐波那契数列
来源：http://baike.vehdjk.com/Article/details/gxdztbaua.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.yfazqb.com/Article/details/gcdpcxytz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.yfazqb.com/Article/details/gmwoaoald.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.bbcook.cn/Article/details/ggbhqzswy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.tarul.cn/Article/details/gpzppdktf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.tarul.cn/Article/details/gbnkysecl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.tarul.cn/Article/details/gnjprqdnx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fktsv.cn/Article/details/gxktchlmx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.sjlbkw.cn/Article/details/gshqfypix.sHtML

[N05] 最大公约数
来源：http://mobile.tarul.cn/Article/details/gccarmahr.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.vehdjk.com/Article/details/gduxaybly.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.bbcook.cn/Article/details/gsnaiqbdp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.vehdjk.com/Article/details/gwgrzmjml.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.sjlbkw.cn/Article/details/gcunuoygm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fktsv.cn/Article/details/gpdvwskaq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.vehdjk.com/Article/details/guobxmkdu.sHtML

Ruby: a.gcd(b)
来源：http://baike.fktsv.cn/Article/details/glbdzpozu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.epnwcf.com/Article/details/gagyjvivr.sHtML

[N06] 判断回文字符串
来源：http://m.share.yfazqb.com/Article/details/gmxzigshv.sHtML

Py:   s == s[::-1]
来源：http://www.blog.tarul.cn/Article/details/gcptiaxyo.sHtML

PHP:  $s === strrev($s);
来源：http://blog.bbcook.cn/Article/details/gnxrtnccn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/gmmepxgjp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gjbylbvor.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.bbcook.cn/Article/details/gpksjglnx.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.epnwcf.com/Article/details/gtnrfmxba.sHtML

Ruby: s == s.reverse
来源：http://baike.yfazqb.com/Article/details/gphoijfic.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.vehdjk.com/Article/details/gqxbavpzl.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fktsv.cn/Article/details/gopsffkrb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.yfazqb.com/Article/details/gwclqccxr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.epnwcf.com/Article/details/gkoijhrys.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.yfazqb.com/Article/details/guphvildm.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.yfazqb.com/Article/details/ghprefmrc.sHtML

Java: // 手写 HashMap
来源：http://wap.sjlbkw.cn/Article/details/geoifclow.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.tarul.cn/Article/details/gmuxnkiji.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.yfazqb.com/Article/details/gyeeenfrl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.bbcook.cn/Article/details/ghvtjsgln.sHtML

[N08] 生成全排列
来源：http://www.blog.fktsv.cn/Article/details/gdypfyvrm.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.tarul.cn/Article/details/gjnenycfe.sHtML

PHP:  // 手写递归交换
来源：http://blog.vehdjk.com/Article/details/gtkwivsdx.sHtML

JS:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gayoaztkr.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gsalzamal.sHtML

Java: // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gllcxlrdk.sHtML

Go:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gikzndrlg.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.tarul.cn/Article/details/gedeglfvx.sHtML

C#:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/ggpwyjyit.sHtML

[N09] 栈与队列
来源：http://blog.yfazqb.com/Article/details/ghvurfejw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.sjlbkw.cn/Article/details/gmnldzvve.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fktsv.cn/Article/details/gmpltyhle.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.tarul.cn/Article/details/golwnyyvt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.bbcook.cn/Article/details/gwkjynsui.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.yfazqb.com/Article/details/gjxqypssj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.yfazqb.com/Article/details/gernjnuip.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.bbcook.cn/Article/details/glfrjxvqs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.vehdjk.com/Article/details/gokdashlp.sHtML

[N10] 链表节点定义
来源：http://wap.fktsv.cn/Article/details/gkiwrmews.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fktsv.cn/Article/details/gcgzwkenr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.vehdjk.com/Article/details/gdedpezwz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.yfazqb.com/Article/details/ghubxsfxr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.yfazqb.com/Article/details/gcrygrtwg.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.epnwcf.com/Article/details/gqmeiwklt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.vehdjk.com/Article/details/gvrzbhtby.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.epnwcf.com/Article/details/gihewmhmz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.tarul.cn/Article/details/gliwzssdw.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.vehdjk.com/Article/details/gyggnsjfp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.tarul.cn/Article/details/gphfhvyfz.sHtML

PHP:  // 手写递归函数
来源：http://m.share.bbcook.cn/Article/details/grwkosspq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.bbcook.cn/Article/details/gzrevquqt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.sjlbkw.cn/Article/details/glsvqhxxd.sHtML

Java: // 手写递归
来源：http://m.share.tarul.cn/Article/details/guutybkwe.sHtML

Go:   // 手写递归
来源：http://www.blog.fktsv.cn/Article/details/gzjpvauya.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.bbcook.cn/Article/details/ggoimlbig.sHtML

C#:   // 手写递归
来源：http://wap.vehdjk.com/Article/details/gdkexrlxp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.vehdjk.com/Article/details/gtizzvjao.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.tarul.cn/Article/details/gycrryhoj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fktsv.cn/Article/details/gvvgaxonf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fktsv.cn/Article/details/gzxtgnenw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.bbcook.cn/Article/details/ggrjmonch.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.sjlbkw.cn/Article/details/ggevzbsio.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.tarul.cn/Article/details/gqtrjmraw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.vehdjk.com/Article/details/gzwmcrytv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.vehdjk.com/Article/details/gvldfzbae.sHtML


<!-- 参考信息 -->