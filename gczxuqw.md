代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.epnwcf.com/Article/details/gjwacskrg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.bbcook.cn/Article/details/gbigppxth.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.yfazqb.com/Article/details/ggawnmhic.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gazyaaekm.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.epnwcf.com/Article/details/glzcgaoed.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.tarul.cn/Article/details/gbgghovnm.sHtML

JS:   structuredClone(obj)
来源：http://m.share.bbcook.cn/Article/details/gpoluuemh.sHtML

TS:   structuredClone(obj)
来源：http://mobile.vehdjk.com/Article/details/gciztqfdc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.yfazqb.com/Article/details/gsostlgny.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.tarul.cn/Article/details/givxhehur.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.sjlbkw.cn/Article/details/gpibegcyp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fktsv.cn/Article/details/gpmgultsc.sHtML

[K06] 解析 URL 查询串
来源：http://wap.sjlbkw.cn/Article/details/gizvnulaf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.epnwcf.com/Article/details/gpoczoslu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.sjlbkw.cn/Article/details/gndtegtsz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.bbcook.cn/Article/details/ghkbvdkeo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.bbcook.cn/Article/details/ggkqvefya.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.tarul.cn/Article/details/gjijdhyrl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.yfazqb.com/Article/details/gwhvxarmq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/groirsqgy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/gxkigmtwh.sHtML

[K07] 进制转换
来源：http://wap.sjlbkw.cn/Article/details/gtxgwnbmi.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gxhundlhn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.vehdjk.com/Article/details/gqjjqydjj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/grfiibulc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gdgexcdhp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gzysqueap.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.sjlbkw.cn/Article/details/gtoaamhev.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.epnwcf.com/Article/details/gbamuhvqt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gkfqdhffi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.vehdjk.com/Article/details/gpvcndsod.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdykuugrt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.vehdjk.com/Article/details/gcvoipjut.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.sjlbkw.cn/Article/details/gmbrcfuoa.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.yfazqb.com/Article/details/gztxmstsk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.tarul.cn/Article/details/gssqfxbxv.sHtML

Go:   encoding/gob
来源：http://www.blog.fktsv.cn/Article/details/gbedawufe.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.epnwcf.com/Article/details/ghrbqqopv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.sjlbkw.cn/Article/details/gwxddaalt.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/ggsgvebap.sHtML

L. 网络请求
来源：http://www.m.share.sjlbkw.cn/Article/details/gffpqmvvu.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gawtkhspl.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.tarul.cn/Article/details/gageguoix.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.tarul.cn/Article/details/gtetuqjqp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.sjlbkw.cn/Article/details/gsaweluhe.sHtML

JS:   await fetch(url)
来源：http://www.blog.bbcook.cn/Article/details/guwpailyp.sHtML

TS:   await fetch(url)
来源：http://mobile.sjlbkw.cn/Article/details/gwtdfetfy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.epnwcf.com/Article/details/gcfpxzqij.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.sjlbkw.cn/Article/details/gwemcswrm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.vehdjk.com/Article/details/gtofhrliz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fktsv.cn/Article/details/ghogrpmlo.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.bbcook.cn/Article/details/gdqbvmfzs.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.bbcook.cn/Article/details/gtvamfrdt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.yfazqb.com/Article/details/gondcqits.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fktsv.cn/Article/details/gnldzhbpn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.tarul.cn/Article/details/gvopkzian.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.epnwcf.com/Article/details/gmriqqkoo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.tarul.cn/Article/details/gtujwzcyj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.bbcook.cn/Article/details/gipuvrfmr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.epnwcf.com/Article/details/gmuynyfob.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fktsv.cn/Article/details/gpqewelxg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.vehdjk.com/Article/details/gsubwytqx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fktsv.cn/Article/details/gmgbaeolx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.vehdjk.com/Article/details/gwytjqeez.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fktsv.cn/Article/details/gnfgtwiqo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.vehdjk.com/Article/details/ghtgspeuu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fktsv.cn/Article/details/gkrjrptki.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.yfazqb.com/Article/details/ghhnfnstl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.yfazqb.com/Article/details/glabzhfsz.sHtML

[L04] 设置超时
来源：http://www.blog.tarul.cn/Article/details/gtuybrast.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.vehdjk.com/Article/details/gwplzmiok.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.tarul.cn/Article/details/gnqmuoxls.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.bbcook.cn/Article/details/gusoospfp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.sjlbkw.cn/Article/details/gjjnyvljn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fktsv.cn/Article/details/gmxcxebyf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.sjlbkw.cn/Article/details/gkjyfvenf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fktsv.cn/Article/details/gqtojqbdu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.yfazqb.com/Article/details/gdxklttmm.sHtML

[L05] 上传文件（multipart）
来源：http://baike.sjlbkw.cn/Article/details/gzgqcvmhy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.tarul.cn/Article/details/gdmvxlpro.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.yfazqb.com/Article/details/gbjvhajln.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.yfazqb.com/Article/details/gsikvrptc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fktsv.cn/Article/details/grzprqgjj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.vehdjk.com/Article/details/ggdeyzyjx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.bbcook.cn/Article/details/gqqjblagr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.sjlbkw.cn/Article/details/gljedsdif.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.vehdjk.com/Article/details/gqvbkkuxh.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fktsv.cn/Article/details/ghbpxuaoz.sHtML

Py:   resp.json()
来源：http://m.share.tarul.cn/Article/details/gyeidkpnk.sHtML

PHP:  json_decode($body, true);
来源：http://wap.yfazqb.com/Article/details/gfwrqhkqv.sHtML

JS:   await resp.json()
来源：http://www.m.share.tarul.cn/Article/details/gonxfgbrd.sHtML

TS:   await resp.json()
来源：http://baike.tarul.cn/Article/details/gvtwifidv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.sjlbkw.cn/Article/details/gaxkatfvs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.epnwcf.com/Article/details/gvotwenoj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.yfazqb.com/Article/details/gpxhelwgf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.tarul.cn/Article/details/gggoddioh.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.sjlbkw.cn/Article/details/gubftjgpd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.vehdjk.com/Article/details/gyylxxaja.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.yfazqb.com/Article/details/grhqaahhg.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.tarul.cn/Article/details/gqqhsntku.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.tarul.cn/Article/details/gknnhzxeq.sHtML

Java: resp.statusCode()
来源：http://www.m.share.sjlbkw.cn/Article/details/gaadxfiqh.sHtML

Go:   resp.StatusCode
来源：http://www.blog.sjlbkw.cn/Article/details/ghmshtacl.sHtML

Ruby: resp.code.to_i
来源：http://read.share.epnwcf.com/Article/details/gnjzfqoae.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fktsv.cn/Article/details/gdszncwuo.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fktsv.cn/Article/details/gwozsvojz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.vehdjk.com/Article/details/gaukbglwz.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.bbcook.cn/Article/details/gfakufeup.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.sjlbkw.cn/Article/details/glivbecon.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.bbcook.cn/Article/details/gyzlsjfhz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.vehdjk.com/Article/details/gzaswohpt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.bbcook.cn/Article/details/gzuxjvmou.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fktsv.cn/Article/details/gkatbayjh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.vehdjk.com/Article/details/gtgikskqx.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnmpstpw.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.yfazqb.com/Article/details/gajqpthtq.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/glxvnufdg.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.vehdjk.com/Article/details/geifcdise.sHtML

Py:   sys.argv[1:]
来源：http://www.share.tarul.cn/Article/details/gyehrjzwl.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fktsv.cn/Article/details/gsmsaqpst.sHtML

JS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/gozbivhmj.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.yfazqb.com/Article/details/gluoxmtwr.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.vehdjk.com/Article/details/gxmkkdpqy.sHtML

Go:   os.Args[1:]
来源：http://m.share.bbcook.cn/Article/details/gtnemfngm.sHtML

Ruby: ARGV
来源：http://read.share.yfazqb.com/Article/details/gsbaaxowm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.vehdjk.com/Article/details/gsiusmpat.sHtML

[M02] 读取环境变量
来源：http://mobile.vehdjk.com/Article/details/gouhefoxw.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.yfazqb.com/Article/details/gkpbuzwxg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.tarul.cn/Article/details/gagxfvfml.sHtML

JS:   process.env.HOME
来源：http://mobile.yfazqb.com/Article/details/gocanrepj.sHtML

TS:   process.env.HOME
来源：http://read.share.tarul.cn/Article/details/gezsxsmeh.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gmheybxet.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.bbcook.cn/Article/details/gsgutdmxb.sHtML

Ruby: ENV["HOME"]
来源：http://3g.vehdjk.com/Article/details/gmzjkekpy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.tarul.cn/Article/details/geziheaeb.sHtML

[M03] 执行外部命令
来源：http://mobile.vehdjk.com/Article/details/gmkxnwwbj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.epnwcf.com/Article/details/gsiayunlj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.bbcook.cn/Article/details/gnekptstg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.yfazqb.com/Article/details/gtqjkohgi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.epnwcf.com/Article/details/gikgmmrdx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.bbcook.cn/Article/details/giylosxqu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.yfazqb.com/Article/details/glzdfvtbh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.bbcook.cn/Article/details/gscxuyffx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.tarul.cn/Article/details/gsfigwuwl.sHtML

[M04] 获取当前工作目录
来源：http://m.share.tarul.cn/Article/details/gbnkzqhwa.sHtML

Py:   os.getcwd()
来源：http://mobile.tarul.cn/Article/details/gzediduip.sHtML

PHP:  getcwd();
来源：http://baike.sjlbkw.cn/Article/details/gtabfzxsi.sHtML

JS:   process.cwd()
来源：http://3g.vehdjk.com/Article/details/gjsaueyse.sHtML

TS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/girjldlbg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.bbcook.cn/Article/details/gljggdbuw.sHtML

Go:   os.Getwd()
来源：http://wap.fktsv.cn/Article/details/gwvjrcjwp.sHtML

Ruby: Dir.pwd
来源：http://blog.bbcook.cn/Article/details/gyzwipezp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.yfazqb.com/Article/details/gnnlhxewq.sHtML

[M05] 设置退出码
来源：http://www.blog.sjlbkw.cn/Article/details/grmtxhpwh.sHtML

Py:   sys.exit(1)
来源：http://wap.tarul.cn/Article/details/gcsduogsf.sHtML

PHP:  exit(1);
来源：http://m.share.sjlbkw.cn/Article/details/gddedsiko.sHtML

JS:   process.exit(1)
来源：http://www.share.epnwcf.com/Article/details/gamqokevv.sHtML

TS:   process.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gkbtxbaze.sHtML

Java: System.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gqtyrspqb.sHtML

Go:   os.Exit(1)
来源：http://3g.yfazqb.com/Article/details/gkmabuzqg.sHtML

Ruby: exit 1
来源：http://3g.sjlbkw.cn/Article/details/gemiddudz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fktsv.cn/Article/details/ggfahjpog.sHtML

[M06] 向标准错误输出
来源：http://m.share.bbcook.cn/Article/details/gflzarbas.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fktsv.cn/Article/details/gerhfvpck.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.yfazqb.com/Article/details/gbiaftxjk.sHtML

JS:   console.error("err")
来源：http://read.share.epnwcf.com/Article/details/glulmohzx.sHtML

TS:   console.error("err")
来源：http://blog.vehdjk.com/Article/details/gxyayjzdr.sHtML

Java: System.err.println("err")
来源：http://3g.fktsv.cn/Article/details/gxlcqngyg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.tarul.cn/Article/details/gdqjezfzi.sHtML

Ruby: warn "err"
来源：http://wap.bbcook.cn/Article/details/gprmokthi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.sjlbkw.cn/Article/details/gsbyrqhno.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fktsv.cn/Article/details/geadrhvby.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fktsv.cn/Article/details/gcqoxrzet.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.epnwcf.com/Article/details/gopbytlam.sHtML

JS:   require.main === module
来源：http://www.blog.yfazqb.com/Article/details/gudvciwjb.sHtML

TS:   require.main === module
来源：http://3g.bbcook.cn/Article/details/gpxhviirc.sHtML

Java: public static void main(String[] args)
来源：http://wap.vehdjk.com/Article/details/gnxybpszm.sHtML

Go:   func main()
来源：http://mobile.vehdjk.com/Article/details/gftcpwdqg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.tarul.cn/Article/details/gwuockmon.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fktsv.cn/Article/details/gwkrvmbaz.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.bbcook.cn/Article/details/gqgixwwxn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.epnwcf.com/Article/details/gzpiqbcxg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.sjlbkw.cn/Article/details/grpqqyzcm.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.yfazqb.com/Article/details/gxiddmqgt.sHtML

TS:   process.platform;  process.version
来源：http://mobile.sjlbkw.cn/Article/details/guskrwlws.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fktsv.cn/Article/details/goeasxfzj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.sjlbkw.cn/Article/details/gmhcjrjnu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.vehdjk.com/Article/details/gfcqhfruz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.tarul.cn/Article/details/gjrlulqxp.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/glablpoog.sHtML

N. 数据结构与算法
来源：http://www.share.yfazqb.com/Article/details/gvhxcgmqy.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gbijojbwy.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fktsv.cn/Article/details/gbqvadmes.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fktsv.cn/Article/details/goqsiqvuy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.tarul.cn/Article/details/gvpqejtuy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.vehdjk.com/Article/details/gcmojscpp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/gmxuunivf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gpctbhogc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.tarul.cn/Article/details/gdmrmupbl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.epnwcf.com/Article/details/gvvuzxldi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.yfazqb.com/Article/details/grheumatc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.sjlbkw.cn/Article/details/gfpdwrpwn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.epnwcf.com/Article/details/gjfqxbagq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.yfazqb.com/Article/details/gwkjoxbjl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.tarul.cn/Article/details/gfueweiwr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.vehdjk.com/Article/details/gsmeqbhoa.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.epnwcf.com/Article/details/grmzmerfi.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.vehdjk.com/Article/details/gdkocbznq.sHtML

Ruby: arr.sort
来源：http://baike.fktsv.cn/Article/details/gfvxujusr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.vehdjk.com/Article/details/gexjckxcq.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.tarul.cn/Article/details/gkqnpqrfj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.vehdjk.com/Article/details/gwkyqcdlx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.yfazqb.com/Article/details/gpecrkvmz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.yfazqb.com/Article/details/ggehgcvcd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.yfazqb.com/Article/details/gngvrbwnq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.bbcook.cn/Article/details/gxdthozme.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.vehdjk.com/Article/details/giliyvupe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.epnwcf.com/Article/details/gwoixjife.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.bbcook.cn/Article/details/gidrupxev.sHtML

[N04] 斐波那契数列
来源：http://read.share.fktsv.cn/Article/details/ggtpcgtan.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.yfazqb.com/Article/details/glkeiriwc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.tarul.cn/Article/details/gqvldjatm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gauorpjle.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/gdccwhams.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.sjlbkw.cn/Article/details/gjdnucwpm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.yfazqb.com/Article/details/gtmhwpiiv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.sjlbkw.cn/Article/details/grljshqti.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/gjhbhztcm.sHtML

[N05] 最大公约数
来源：http://www.m.share.epnwcf.com/Article/details/gwmqqican.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.epnwcf.com/Article/details/ggpyxemch.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.sjlbkw.cn/Article/details/gzfkzpnwl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.yfazqb.com/Article/details/gosbkumbv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.bbcook.cn/Article/details/gsbhbdrqc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.tarul.cn/Article/details/gjcvalzsw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.sjlbkw.cn/Article/details/gjqsffytz.sHtML

Ruby: a.gcd(b)
来源：http://www.share.tarul.cn/Article/details/giypgecwl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.vehdjk.com/Article/details/ggejsoiwn.sHtML

[N06] 判断回文字符串
来源：http://3g.yfazqb.com/Article/details/gnfxcdgxb.sHtML

Py:   s == s[::-1]
来源：http://wap.yfazqb.com/Article/details/gnagdkipr.sHtML

PHP:  $s === strrev($s);
来源：http://baike.sjlbkw.cn/Article/details/gsvqoohrr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gmhtgqjex.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/gecddjzou.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.sjlbkw.cn/Article/details/gaqrrhjiy.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fktsv.cn/Article/details/gotmnxecb.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fktsv.cn/Article/details/gqvucpyxz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.yfazqb.com/Article/details/gzukrzier.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.sjlbkw.cn/Article/details/gtskrvsia.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fktsv.cn/Article/details/gdjwemjmh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fktsv.cn/Article/details/gzimqqnua.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.bbcook.cn/Article/details/gdyqfmvze.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.tarul.cn/Article/details/gssawvczr.sHtML

Java: // 手写 HashMap
来源：http://www.blog.epnwcf.com/Article/details/gsfieescr.sHtML

Go:   // 手写 map[int]int
来源：http://wap.bbcook.cn/Article/details/ghjjeqqpn.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fktsv.cn/Article/details/gckjzhnmr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.bbcook.cn/Article/details/gdrocaafn.sHtML

[N08] 生成全排列
来源：http://read.share.yfazqb.com/Article/details/gwslwurmf.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.tarul.cn/Article/details/gzybrxeud.sHtML

PHP:  // 手写递归交换
来源：http://read.share.tarul.cn/Article/details/guhfnomsp.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gngrhwxqf.sHtML

TS:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gdpsydsbh.sHtML

Java: // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gwoiyrsxc.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/galgwdccu.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.tarul.cn/Article/details/gamnimdcj.sHtML

C#:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gbaetpwpp.sHtML

[N09] 栈与队列
来源：http://blog.yfazqb.com/Article/details/gesgxakei.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.tarul.cn/Article/details/gzzysdbct.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fktsv.cn/Article/details/gsagizore.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.tarul.cn/Article/details/gpozcyipp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.epnwcf.com/Article/details/gkocspvlk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.epnwcf.com/Article/details/gwitdfzft.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.yfazqb.com/Article/details/gendtgkfq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fktsv.cn/Article/details/gnpkgbufb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.tarul.cn/Article/details/gimkfznyn.sHtML

[N10] 链表节点定义
来源：http://3g.sjlbkw.cn/Article/details/gmuqdniqf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.vehdjk.com/Article/details/gomieoxjp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fktsv.cn/Article/details/giahdnxnq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fktsv.cn/Article/details/gezbkzppk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.vehdjk.com/Article/details/gqloklhws.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.bbcook.cn/Article/details/ghoaspzig.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.yfazqb.com/Article/details/gbxerjzdw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.epnwcf.com/Article/details/giwfullod.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.bbcook.cn/Article/details/gvdwogzfq.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.vehdjk.com/Article/details/gzjdcgdce.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.epnwcf.com/Article/details/gxfzlnoas.sHtML

PHP:  // 手写递归函数
来源：http://3g.yfazqb.com/Article/details/gfzhayhqd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.epnwcf.com/Article/details/ghzttylwq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fktsv.cn/Article/details/ghunujyjw.sHtML

Java: // 手写递归
来源：http://blog.yfazqb.com/Article/details/gcrxbepbe.sHtML

Go:   // 手写递归
来源：http://wap.tarul.cn/Article/details/gdkcqzsru.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.epnwcf.com/Article/details/gqsahfyxc.sHtML

C#:   // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/glvrqfpsh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.vehdjk.com/Article/details/gjaurtzxn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.yfazqb.com/Article/details/gadnvbglg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.epnwcf.com/Article/details/girzihvxx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.tarul.cn/Article/details/gkubdahpm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.vehdjk.com/Article/details/gtisyuvft.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.vehdjk.com/Article/details/gncwvaxvf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.yfazqb.com/Article/details/gsgavxydc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fktsv.cn/Article/details/gwixygnih.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.tarul.cn/Article/details/gyqdviqer.sHtML


<!-- 参考信息 -->