代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.bbcook.cn/Article/details/gsbudhmzd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.vehdjk.com/Article/details/glbzektce.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.tarul.cn/Article/details/ghbmqxcpm.sHtML

[K05] 深拷贝对象
来源：http://read.share.epnwcf.com/Article/details/gglrdcydj.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.bbcook.cn/Article/details/gplbqveri.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.bbcook.cn/Article/details/gvxxdjmha.sHtML

JS:   structuredClone(obj)
来源：http://read.share.bbcook.cn/Article/details/gnxwjpxyu.sHtML

TS:   structuredClone(obj)
来源：http://www.share.epnwcf.com/Article/details/giovsyqpy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.bbcook.cn/Article/details/gfagtcdwm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.bbcook.cn/Article/details/gvonjmskb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.epnwcf.com/Article/details/gnhdzwaqn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.vehdjk.com/Article/details/ghnuxzysr.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fktsv.cn/Article/details/gmjtgyifb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.epnwcf.com/Article/details/gqqijltwq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.epnwcf.com/Article/details/gaaqhyeqr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.vehdjk.com/Article/details/gxoiyzspx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.epnwcf.com/Article/details/gjcfonkxg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.tarul.cn/Article/details/gobnwxiiy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.tarul.cn/Article/details/guquwdskp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.vehdjk.com/Article/details/gpgmgzolx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.tarul.cn/Article/details/gcjohjxqn.sHtML

[K07] 进制转换
来源：http://mobile.tarul.cn/Article/details/gjgpvptbf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.bbcook.cn/Article/details/grezssatw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.bbcook.cn/Article/details/gufvvocxk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gfhmcoehl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gwxckewln.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gmpspvaxd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.epnwcf.com/Article/details/gvmlcqknj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.bbcook.cn/Article/details/gzyfaxvdz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gthqfljtz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.sjlbkw.cn/Article/details/ggwrmmgdi.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gqsvvswgt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fktsv.cn/Article/details/gbhpvuwpp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fktsv.cn/Article/details/grkublozy.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.sjlbkw.cn/Article/details/gcgvdivrv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.vehdjk.com/Article/details/gilucwlrl.sHtML

Go:   encoding/gob
来源：http://3g.epnwcf.com/Article/details/gxzrrhgep.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.vehdjk.com/Article/details/gcftfsygo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.sjlbkw.cn/Article/details/giztojinj.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gcbslonne.sHtML

L. 网络请求
来源：http://www.m.share.bbcook.cn/Article/details/gfjnbpffb.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gnciqnfol.sHtML

[L01] 发送 GET 请求
来源：http://read.share.tarul.cn/Article/details/gzbvdckwt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.bbcook.cn/Article/details/gbvgwebou.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.tarul.cn/Article/details/guzsegjom.sHtML

JS:   await fetch(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/goegdanhx.sHtML

TS:   await fetch(url)
来源：http://www.share.sjlbkw.cn/Article/details/gcmoaceld.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.yfazqb.com/Article/details/gkowghnln.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.bbcook.cn/Article/details/gwbcavffw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fktsv.cn/Article/details/gvmyshyud.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.vehdjk.com/Article/details/gsynvzpuo.sHtML

[L02] 发送 POST JSON
来源：http://mobile.vehdjk.com/Article/details/gsylcxkmc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.sjlbkw.cn/Article/details/gunsthrtd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.vehdjk.com/Article/details/gfrdhnuzj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fktsv.cn/Article/details/gzkihsacv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.tarul.cn/Article/details/gdlzbgudh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.yfazqb.com/Article/details/gisbxlxuf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.epnwcf.com/Article/details/gfmggmgnl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.vehdjk.com/Article/details/gitpcramp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.vehdjk.com/Article/details/gbqnkprae.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fktsv.cn/Article/details/gcsigtxex.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.bbcook.cn/Article/details/gcildgvef.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.bbcook.cn/Article/details/gyohuiajw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fktsv.cn/Article/details/gqwxpvgxd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.vehdjk.com/Article/details/gffxckzpb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.epnwcf.com/Article/details/glvhzqqwk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fktsv.cn/Article/details/gbajihgdz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fktsv.cn/Article/details/ghgjfhbas.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.epnwcf.com/Article/details/gashkvzsr.sHtML

[L04] 设置超时
来源：http://blog.yfazqb.com/Article/details/gdmslutlo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.vehdjk.com/Article/details/gqogrcgyo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.sjlbkw.cn/Article/details/gtllckqzr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.vehdjk.com/Article/details/gqjfenpqd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fktsv.cn/Article/details/gmuamfpci.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.vehdjk.com/Article/details/gbdzahsdz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.yfazqb.com/Article/details/gxyyzcqio.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.epnwcf.com/Article/details/gkktervtc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.tarul.cn/Article/details/gfthzrdwk.sHtML

[L05] 上传文件（multipart）
来源：http://3g.epnwcf.com/Article/details/gvgbscngx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fktsv.cn/Article/details/gfsgozwnc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.yfazqb.com/Article/details/glbkaxinz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.epnwcf.com/Article/details/gwvpvwrmw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.sjlbkw.cn/Article/details/gquefaibb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.yfazqb.com/Article/details/gljcnpubh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.epnwcf.com/Article/details/glpwzkiye.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.yfazqb.com/Article/details/gwnyzqrph.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fktsv.cn/Article/details/gtjaqvgcl.sHtML

[L06] 解析响应为 JSON
来源：http://baike.tarul.cn/Article/details/goqksyaxw.sHtML

Py:   resp.json()
来源：http://wap.sjlbkw.cn/Article/details/gcvcfweny.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.bbcook.cn/Article/details/gvovyhflt.sHtML

JS:   await resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/gohwufbzs.sHtML

TS:   await resp.json()
来源：http://baike.tarul.cn/Article/details/gdlqhmwmj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fktsv.cn/Article/details/gyimosrsw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.epnwcf.com/Article/details/gwzyewnpq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.vehdjk.com/Article/details/gllasucqb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.vehdjk.com/Article/details/gywddhece.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.bbcook.cn/Article/details/gbovwsttn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.tarul.cn/Article/details/gtowohhig.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.vehdjk.com/Article/details/gampeluap.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fktsv.cn/Article/details/gtxfrjarj.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.yfazqb.com/Article/details/gvpcfcnnl.sHtML

Java: resp.statusCode()
来源：http://m.share.bbcook.cn/Article/details/gescikwqc.sHtML

Go:   resp.StatusCode
来源：http://m.share.tarul.cn/Article/details/ghldjvldw.sHtML

Ruby: resp.code.to_i
来源：http://3g.epnwcf.com/Article/details/gosseqyyy.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.sjlbkw.cn/Article/details/gcwgznvej.sHtML

[L08] 并发请求多个地址
来源：http://baike.sjlbkw.cn/Article/details/gfrsdbohd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.vehdjk.com/Article/details/gvemueyuz.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.vehdjk.com/Article/details/gfgtwkydp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.epnwcf.com/Article/details/gmtnyhjyb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.sjlbkw.cn/Article/details/ghuslsujg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.bbcook.cn/Article/details/gqhgamegm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.vehdjk.com/Article/details/gcomrlxil.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fktsv.cn/Article/details/ghugenmhr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.yfazqb.com/Article/details/gveipspnr.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/ggkgjgttm.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.vehdjk.com/Article/details/gkfbfpccv.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gbuwfiuvy.sHtML

[M01] 读取命令行参数
来源：http://read.share.bbcook.cn/Article/details/gquchuokn.sHtML

Py:   sys.argv[1:]
来源：http://wap.sjlbkw.cn/Article/details/gzsuqbwqn.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.sjlbkw.cn/Article/details/gcigrcmmj.sHtML

JS:   process.argv.slice(2)
来源：http://blog.bbcook.cn/Article/details/ghojjqxdu.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.bbcook.cn/Article/details/gopzeywzt.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.epnwcf.com/Article/details/galgcbdsr.sHtML

Go:   os.Args[1:]
来源：http://m.share.epnwcf.com/Article/details/gngrpnhby.sHtML

Ruby: ARGV
来源：http://blog.tarul.cn/Article/details/gmcojoqbn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.epnwcf.com/Article/details/ghmhqzhzz.sHtML

[M02] 读取环境变量
来源：http://www.share.vehdjk.com/Article/details/gwwhojted.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gwuinqfbe.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.sjlbkw.cn/Article/details/gygjeytlz.sHtML

JS:   process.env.HOME
来源：http://www.share.fktsv.cn/Article/details/gotkjeuxk.sHtML

TS:   process.env.HOME
来源：http://wap.sjlbkw.cn/Article/details/gfzdfwhbo.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.bbcook.cn/Article/details/gzmocuryl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.yfazqb.com/Article/details/grswuecok.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.sjlbkw.cn/Article/details/gzakkzhvk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.bbcook.cn/Article/details/grcnxjcki.sHtML

[M03] 执行外部命令
来源：http://www.blog.epnwcf.com/Article/details/gdfkdcjcv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.yfazqb.com/Article/details/gjmmdgmnx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.tarul.cn/Article/details/gqhqnqngi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fktsv.cn/Article/details/gareyrjrq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.bbcook.cn/Article/details/ghabnehhc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fktsv.cn/Article/details/gazycdlqy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.bbcook.cn/Article/details/gcjshszyt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.yfazqb.com/Article/details/gbgxqkxww.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.bbcook.cn/Article/details/gnoontjyu.sHtML

[M04] 获取当前工作目录
来源：http://3g.epnwcf.com/Article/details/guiilfgye.sHtML

Py:   os.getcwd()
来源：http://read.share.sjlbkw.cn/Article/details/gfcdwrjho.sHtML

PHP:  getcwd();
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgcxfdlt.sHtML

JS:   process.cwd()
来源：http://wap.sjlbkw.cn/Article/details/gxahjdxle.sHtML

TS:   process.cwd()
来源：http://blog.bbcook.cn/Article/details/gwujqlgdv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fktsv.cn/Article/details/gmwgvcvtu.sHtML

Go:   os.Getwd()
来源：http://baike.tarul.cn/Article/details/gaqkejgsd.sHtML

Ruby: Dir.pwd
来源：http://wap.tarul.cn/Article/details/ggwkfkzfx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.sjlbkw.cn/Article/details/gdzppjgeg.sHtML

[M05] 设置退出码
来源：http://mobile.yfazqb.com/Article/details/grfxccffh.sHtML

Py:   sys.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/groreupyp.sHtML

PHP:  exit(1);
来源：http://www.blog.vehdjk.com/Article/details/gbgepmuvj.sHtML

JS:   process.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmesmayub.sHtML

TS:   process.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gifyneqjh.sHtML

Java: System.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gianbnpsh.sHtML

Go:   os.Exit(1)
来源：http://www.share.epnwcf.com/Article/details/gndmxkwgq.sHtML

Ruby: exit 1
来源：http://3g.vehdjk.com/Article/details/gseknrwyg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.vehdjk.com/Article/details/gdvozyzay.sHtML

[M06] 向标准错误输出
来源：http://m.share.sjlbkw.cn/Article/details/gfnvxecbh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.bbcook.cn/Article/details/gejkbnaoi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.vehdjk.com/Article/details/gyeooaqbw.sHtML

JS:   console.error("err")
来源：http://baike.yfazqb.com/Article/details/gqcnhozah.sHtML

TS:   console.error("err")
来源：http://blog.epnwcf.com/Article/details/gwqnlhdck.sHtML

Java: System.err.println("err")
来源：http://read.share.tarul.cn/Article/details/gxhqiergc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.sjlbkw.cn/Article/details/gcfanvrlw.sHtML

Ruby: warn "err"
来源：http://www.share.bbcook.cn/Article/details/ggzwpatik.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.sjlbkw.cn/Article/details/gyucjjjsi.sHtML

[M07] 判断是否为主入口
来源：http://read.share.epnwcf.com/Article/details/gpxpibjwj.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.yfazqb.com/Article/details/gkcowwlsi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fktsv.cn/Article/details/gjztuofod.sHtML

JS:   require.main === module
来源：http://wap.fktsv.cn/Article/details/gksvymbkz.sHtML

TS:   require.main === module
来源：http://baike.tarul.cn/Article/details/gyvoplluh.sHtML

Java: public static void main(String[] args)
来源：http://blog.fktsv.cn/Article/details/gecvuevul.sHtML

Go:   func main()
来源：http://read.share.vehdjk.com/Article/details/gfpdwcfol.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.sjlbkw.cn/Article/details/ghnwdnagv.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.yfazqb.com/Article/details/gstggukri.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fktsv.cn/Article/details/gvdnmlsyn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.tarul.cn/Article/details/gyvtqbtsd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.epnwcf.com/Article/details/gcmldtxfd.sHtML

JS:   process.platform;  process.version
来源：http://mobile.yfazqb.com/Article/details/gzwqdbojt.sHtML

TS:   process.platform;  process.version
来源：http://3g.tarul.cn/Article/details/gpbztetae.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.bbcook.cn/Article/details/geywuyqib.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fktsv.cn/Article/details/gyxpbqula.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fktsv.cn/Article/details/gqdlbggfm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.sjlbkw.cn/Article/details/glpruypoh.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gizcvhclx.sHtML

N. 数据结构与算法
来源：http://read.share.vehdjk.com/Article/details/gyzswzttl.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gxvgkiunp.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.yfazqb.com/Article/details/gkahagmmw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.tarul.cn/Article/details/gwviosttf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.sjlbkw.cn/Article/details/gluduxgax.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.yfazqb.com/Article/details/gskcsggqx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.sjlbkw.cn/Article/details/gidmfgxtn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gvonmemjm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gcbxykzif.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.vehdjk.com/Article/details/ggpfluwel.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.vehdjk.com/Article/details/gzscgutmm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fktsv.cn/Article/details/gzalvxszs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.sjlbkw.cn/Article/details/gdbrgfxwj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.sjlbkw.cn/Article/details/gndnfwhcf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/gooamoukv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.vehdjk.com/Article/details/gsemvribo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.sjlbkw.cn/Article/details/gwxispqpe.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gqoslccsb.sHtML

Ruby: arr.sort
来源：http://baike.epnwcf.com/Article/details/gkwhgjsad.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.vehdjk.com/Article/details/gyrbarwkm.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.bbcook.cn/Article/details/ghadesnct.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fktsv.cn/Article/details/gliinqiex.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.epnwcf.com/Article/details/govocopkf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.bbcook.cn/Article/details/gplksdjpt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.tarul.cn/Article/details/gnmzexyai.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.bbcook.cn/Article/details/gzqdvsfgj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.sjlbkw.cn/Article/details/gseuogbsw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.vehdjk.com/Article/details/gofsdnmrn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.yfazqb.com/Article/details/gahuicake.sHtML

[N04] 斐波那契数列
来源：http://3g.epnwcf.com/Article/details/gacrndtne.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.bbcook.cn/Article/details/gikqlcaiy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.epnwcf.com/Article/details/glvwwcvhg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/gjgzscpbg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/gthljzvvx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.bbcook.cn/Article/details/gznokflho.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.sjlbkw.cn/Article/details/gexhecdyf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.tarul.cn/Article/details/grgczhryu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/ggqwwzzii.sHtML

[N05] 最大公约数
来源：http://wap.vehdjk.com/Article/details/gwfajhxrh.sHtML

Py:   math.gcd(a, b)
来源：http://blog.yfazqb.com/Article/details/guqjbegvs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.sjlbkw.cn/Article/details/ghotdobpm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.sjlbkw.cn/Article/details/gwyihqqgd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.vehdjk.com/Article/details/gcyesreyi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.vehdjk.com/Article/details/ggtoljerr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.vehdjk.com/Article/details/gxpguzmmf.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.bbcook.cn/Article/details/gucytvehx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.sjlbkw.cn/Article/details/gggsuoamx.sHtML

[N06] 判断回文字符串
来源：http://mobile.tarul.cn/Article/details/gkfigsidy.sHtML

Py:   s == s[::-1]
来源：http://3g.fktsv.cn/Article/details/gfpipjnvy.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.sjlbkw.cn/Article/details/gewlrsnpt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gjduootlq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gxxtjhmmn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.sjlbkw.cn/Article/details/gvldpqfbm.sHtML

Go:   // 双指针从两端比较
来源：http://wap.bbcook.cn/Article/details/gzrboynwp.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.tarul.cn/Article/details/gvnfhqxsr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.epnwcf.com/Article/details/gvzaqfova.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.yfazqb.com/Article/details/gdtypushq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.sjlbkw.cn/Article/details/gczovxgue.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.sjlbkw.cn/Article/details/gclmjxbsp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.epnwcf.com/Article/details/gjnadfdfs.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.vehdjk.com/Article/details/gehxouotg.sHtML

Java: // 手写 HashMap
来源：http://www.share.fktsv.cn/Article/details/gjryoufys.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fktsv.cn/Article/details/gbcyljcbz.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.bbcook.cn/Article/details/ghfkltmec.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.vehdjk.com/Article/details/grahhhimv.sHtML

[N08] 生成全排列
来源：http://m.share.epnwcf.com/Article/details/gwqqxkzlw.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.bbcook.cn/Article/details/gzszsapai.sHtML

PHP:  // 手写递归交换
来源：http://blog.epnwcf.com/Article/details/ggeufulpf.sHtML

JS:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/goflgyqew.sHtML

TS:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gdvqtmvtv.sHtML

Java: // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/grbdokzdw.sHtML

Go:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gpdgefwcd.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.epnwcf.com/Article/details/gefgupexi.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gijlmjuwn.sHtML

[N09] 栈与队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gjuhpbctv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.tarul.cn/Article/details/girxyouti.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.tarul.cn/Article/details/gcovlslyk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.bbcook.cn/Article/details/gazrkqqcm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.epnwcf.com/Article/details/gukpttzpo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.sjlbkw.cn/Article/details/gxcbjaevs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.vehdjk.com/Article/details/guofitlbn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.bbcook.cn/Article/details/gxnitrtgd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.vehdjk.com/Article/details/grvjwhayq.sHtML

[N10] 链表节点定义
来源：http://3g.sjlbkw.cn/Article/details/gfboulysb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.vehdjk.com/Article/details/gegawdrbq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.bbcook.cn/Article/details/gixijlfjt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.vehdjk.com/Article/details/glfhdzwuy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fktsv.cn/Article/details/gnoobidix.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.vehdjk.com/Article/details/guwkcjcnk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.tarul.cn/Article/details/gsrxlwsfl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fktsv.cn/Article/details/gvyzngnvw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.vehdjk.com/Article/details/gzcghuvar.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gzebbjcxo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.yfazqb.com/Article/details/gaquufryl.sHtML

PHP:  // 手写递归函数
来源：http://3g.yfazqb.com/Article/details/gmlltottb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.vehdjk.com/Article/details/ghyoviebi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.bbcook.cn/Article/details/ghnnoohwy.sHtML

Java: // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/glwqzsmxl.sHtML

Go:   // 手写递归
来源：http://blog.yfazqb.com/Article/details/gowlptxdh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.epnwcf.com/Article/details/gapprhhus.sHtML

C#:   // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/gcbegqjgc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.yfazqb.com/Article/details/gbnxxlmwh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.vehdjk.com/Article/details/gxuuqpaor.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.bbcook.cn/Article/details/gmuqpyziq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.yfazqb.com/Article/details/gwuxmrzbq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.yfazqb.com/Article/details/gffqtsbml.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.epnwcf.com/Article/details/gawrsaaoa.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.epnwcf.com/Article/details/gfvneotlt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.sjlbkw.cn/Article/details/gfdanricd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.epnwcf.com/Article/details/glbcysfnk.sHtML


<!-- 参考信息 -->