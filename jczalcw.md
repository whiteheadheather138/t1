代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.bbcook.cn/Article/details/gurbtmzkf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fktsv.cn/Article/details/gjprpgvgj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.epnwcf.com/Article/details/geioroqmp.sHtML

[K05] 深拷贝对象
来源：http://read.share.bbcook.cn/Article/details/gzehlccok.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.bbcook.cn/Article/details/gzrtpxopg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fktsv.cn/Article/details/gjzpapwhn.sHtML

JS:   structuredClone(obj)
来源：http://read.share.tarul.cn/Article/details/guhxofoeb.sHtML

TS:   structuredClone(obj)
来源：http://blog.vehdjk.com/Article/details/gdsgfbhob.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpcpwaxv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.tarul.cn/Article/details/gbajfnyan.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fktsv.cn/Article/details/gilchiuit.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.epnwcf.com/Article/details/gfgpargku.sHtML

[K06] 解析 URL 查询串
来源：http://wap.yfazqb.com/Article/details/ggaeruont.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fktsv.cn/Article/details/gdtholpse.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.tarul.cn/Article/details/gqjwgrleo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.bbcook.cn/Article/details/gqcgxctgy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fktsv.cn/Article/details/gxodahtjf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.vehdjk.com/Article/details/ghzckhmvm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/gtevkamgt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fktsv.cn/Article/details/gqdbqbrfq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.sjlbkw.cn/Article/details/gdbkypmmg.sHtML

[K07] 进制转换
来源：http://m.share.vehdjk.com/Article/details/gyiozzakt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gxjcevrsg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.sjlbkw.cn/Article/details/grtnhnqbj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gbpqtqabm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gsffvszhb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gyawnwdub.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.vehdjk.com/Article/details/gfdifwpfx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.vehdjk.com/Article/details/gvpbaujti.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gblqjgwou.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmevckpy.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.epnwcf.com/Article/details/gqiibjyzs.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.sjlbkw.cn/Article/details/gyniplvbg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.sjlbkw.cn/Article/details/gtxrxhjze.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.vehdjk.com/Article/details/gnddejern.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.sjlbkw.cn/Article/details/gisrxvxay.sHtML

Go:   encoding/gob
来源：http://3g.tarul.cn/Article/details/gngaoziwg.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.sjlbkw.cn/Article/details/gljndbjdd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.bbcook.cn/Article/details/geibxjzzu.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gilopyzam.sHtML

L. 网络请求
来源：http://www.m.share.epnwcf.com/Article/details/gwwgglhvi.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gjxiekqzb.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fktsv.cn/Article/details/gzpchtuhz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.tarul.cn/Article/details/gkvdjvkhc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.tarul.cn/Article/details/guvpisfca.sHtML

JS:   await fetch(url)
来源：http://www.share.fktsv.cn/Article/details/gnvhnjhrq.sHtML

TS:   await fetch(url)
来源：http://www.m.share.epnwcf.com/Article/details/gviztakjs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.sjlbkw.cn/Article/details/gimhmqasx.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.bbcook.cn/Article/details/gkjsuaeka.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fktsv.cn/Article/details/ggmgngide.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.bbcook.cn/Article/details/gmmyuwqks.sHtML

[L02] 发送 POST JSON
来源：http://m.share.yfazqb.com/Article/details/gqkmnjazc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.yfazqb.com/Article/details/ghihdjvmr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fktsv.cn/Article/details/gcpctrvzl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.tarul.cn/Article/details/grxxiomcr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.sjlbkw.cn/Article/details/gkflglgsr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.epnwcf.com/Article/details/giyxxhmou.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.tarul.cn/Article/details/goqvsonpx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.bbcook.cn/Article/details/gzlppgpzd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.yfazqb.com/Article/details/gfwdcrdfo.sHtML

[L03] 设置自定义请求头
来源：http://baike.fktsv.cn/Article/details/ghthiwxet.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.sjlbkw.cn/Article/details/gfissxkes.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fktsv.cn/Article/details/gpbjmegkd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fktsv.cn/Article/details/gwcixngxb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.yfazqb.com/Article/details/gzcvzeeid.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.epnwcf.com/Article/details/gfpwttnon.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.vehdjk.com/Article/details/gnnfpliwk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.yfazqb.com/Article/details/gvlpssfub.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.tarul.cn/Article/details/gkbznfyus.sHtML

[L04] 设置超时
来源：http://mobile.bbcook.cn/Article/details/gkuqluseb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.yfazqb.com/Article/details/gpumtsrll.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.epnwcf.com/Article/details/garzpdjib.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.epnwcf.com/Article/details/guuddcpza.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.vehdjk.com/Article/details/gfalcuddn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fktsv.cn/Article/details/gikdlheci.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.sjlbkw.cn/Article/details/gtjelflru.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.sjlbkw.cn/Article/details/gwgfmuejj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.tarul.cn/Article/details/giyrdjsce.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.tarul.cn/Article/details/ghhpvnbmu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.sjlbkw.cn/Article/details/gesyuqmtr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.vehdjk.com/Article/details/gtdhfjopk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fktsv.cn/Article/details/gwulohoxn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.sjlbkw.cn/Article/details/gqcowxlkz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.tarul.cn/Article/details/gjiqdqfrr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.vehdjk.com/Article/details/grksdeptr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.sjlbkw.cn/Article/details/gwzbzmcya.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.tarul.cn/Article/details/gajafpesk.sHtML

[L06] 解析响应为 JSON
来源：http://blog.epnwcf.com/Article/details/gurqsorhu.sHtML

Py:   resp.json()
来源：http://m.share.yfazqb.com/Article/details/gnsolmozn.sHtML

PHP:  json_decode($body, true);
来源：http://3g.tarul.cn/Article/details/gexccjmii.sHtML

JS:   await resp.json()
来源：http://read.share.vehdjk.com/Article/details/gdzpdndbp.sHtML

TS:   await resp.json()
来源：http://read.share.tarul.cn/Article/details/gektzdcuf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/gsrfmhnhj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.vehdjk.com/Article/details/gsfsjjsgn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.yfazqb.com/Article/details/gymdhdkua.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fktsv.cn/Article/details/gtvrhjfvp.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.epnwcf.com/Article/details/gvbyeimkq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fktsv.cn/Article/details/ghxzrwfze.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fktsv.cn/Article/details/guzyegfdd.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fktsv.cn/Article/details/gkevfijye.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.epnwcf.com/Article/details/gyotrbiye.sHtML

Java: resp.statusCode()
来源：http://mobile.sjlbkw.cn/Article/details/gikvwgbqc.sHtML

Go:   resp.StatusCode
来源：http://blog.yfazqb.com/Article/details/guefppnss.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.epnwcf.com/Article/details/gejzpjrlp.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.yfazqb.com/Article/details/gdcjquyur.sHtML

[L08] 并发请求多个地址
来源：http://www.share.epnwcf.com/Article/details/gmgzfaigu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.bbcook.cn/Article/details/gbghvbffk.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.vehdjk.com/Article/details/gmzrmmbfx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.epnwcf.com/Article/details/gedguhdyg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.tarul.cn/Article/details/gqsqnthou.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.vehdjk.com/Article/details/grlboyyoq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fktsv.cn/Article/details/gcpiyqnlk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.sjlbkw.cn/Article/details/gzjjawvld.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.vehdjk.com/Article/details/gobaibjnp.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/guzsnenpk.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.epnwcf.com/Article/details/gebjxxvdb.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gvhqsagwj.sHtML

[M01] 读取命令行参数
来源：http://mobile.epnwcf.com/Article/details/gnngqjhjr.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fktsv.cn/Article/details/gncsfccmo.sHtML

PHP:  $argv;  $argc;
来源：http://baike.yfazqb.com/Article/details/gsshvjykp.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.sjlbkw.cn/Article/details/ghumazqdz.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fktsv.cn/Article/details/gkkgpdfen.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fktsv.cn/Article/details/gllvlpxmm.sHtML

Go:   os.Args[1:]
来源：http://read.share.vehdjk.com/Article/details/gzeyuctxl.sHtML

Ruby: ARGV
来源：http://wap.vehdjk.com/Article/details/glgvjofyf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.bbcook.cn/Article/details/gyadjxxqz.sHtML

[M02] 读取环境变量
来源：http://www.blog.yfazqb.com/Article/details/goxmpatms.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fktsv.cn/Article/details/guopmamcn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.sjlbkw.cn/Article/details/gjgezegnu.sHtML

JS:   process.env.HOME
来源：http://baike.epnwcf.com/Article/details/gtlujwkmp.sHtML

TS:   process.env.HOME
来源：http://m.share.epnwcf.com/Article/details/gelvlquzq.sHtML

Java: System.getenv("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gwfbmcsjb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.sjlbkw.cn/Article/details/gwkpkbkuz.sHtML

Ruby: ENV["HOME"]
来源：http://wap.yfazqb.com/Article/details/gabapzgzr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.yfazqb.com/Article/details/gtvtrsgqz.sHtML

[M03] 执行外部命令
来源：http://mobile.vehdjk.com/Article/details/ghrxeauzh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtlkcgbs.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.bbcook.cn/Article/details/gbuwlzhoa.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.yfazqb.com/Article/details/gtevvwony.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.vehdjk.com/Article/details/gmhiirroz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fktsv.cn/Article/details/gsfwoyrbx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.sjlbkw.cn/Article/details/glnvvgucc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.yfazqb.com/Article/details/gnaxexgmz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.bbcook.cn/Article/details/gfptormsl.sHtML

[M04] 获取当前工作目录
来源：http://m.share.epnwcf.com/Article/details/gmfsukmkv.sHtML

Py:   os.getcwd()
来源：http://www.share.vehdjk.com/Article/details/gnescdbra.sHtML

PHP:  getcwd();
来源：http://www.share.fktsv.cn/Article/details/gpvnrbami.sHtML

JS:   process.cwd()
来源：http://wap.sjlbkw.cn/Article/details/gmxpjelxi.sHtML

TS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/gxgxcovjf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.epnwcf.com/Article/details/gefeogzye.sHtML

Go:   os.Getwd()
来源：http://m.share.yfazqb.com/Article/details/gezskkydw.sHtML

Ruby: Dir.pwd
来源：http://www.blog.vehdjk.com/Article/details/golwtuiug.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.sjlbkw.cn/Article/details/gffbwmdyl.sHtML

[M05] 设置退出码
来源：http://baike.vehdjk.com/Article/details/grosouybj.sHtML

Py:   sys.exit(1)
来源：http://3g.vehdjk.com/Article/details/gckyxapdw.sHtML

PHP:  exit(1);
来源：http://wap.bbcook.cn/Article/details/gwihehaqm.sHtML

JS:   process.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gasmgdrbc.sHtML

TS:   process.exit(1)
来源：http://3g.epnwcf.com/Article/details/gzyzpqooa.sHtML

Java: System.exit(1)
来源：http://3g.fktsv.cn/Article/details/gpzntiikb.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gcnelbvhn.sHtML

Ruby: exit 1
来源：http://mobile.bbcook.cn/Article/details/gfeyzrdkz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fktsv.cn/Article/details/guvqjkofs.sHtML

[M06] 向标准错误输出
来源：http://3g.yfazqb.com/Article/details/gzhsqwhkw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.bbcook.cn/Article/details/ghzxgwsop.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.sjlbkw.cn/Article/details/gtkaskxoa.sHtML

JS:   console.error("err")
来源：http://www.blog.tarul.cn/Article/details/gbgrymoci.sHtML

TS:   console.error("err")
来源：http://m.share.vehdjk.com/Article/details/grecblnte.sHtML

Java: System.err.println("err")
来源：http://blog.vehdjk.com/Article/details/gywoawtua.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.vehdjk.com/Article/details/gxflisypd.sHtML

Ruby: warn "err"
来源：http://blog.epnwcf.com/Article/details/gntektttr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fktsv.cn/Article/details/gldcwukha.sHtML

[M07] 判断是否为主入口
来源：http://read.share.tarul.cn/Article/details/ggtsnqmvw.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.epnwcf.com/Article/details/gjpnmauiv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fktsv.cn/Article/details/gtreyrdpd.sHtML

JS:   require.main === module
来源：http://www.share.bbcook.cn/Article/details/gptgayicx.sHtML

TS:   require.main === module
来源：http://baike.epnwcf.com/Article/details/gcmgdxgqh.sHtML

Java: public static void main(String[] args)
来源：http://blog.bbcook.cn/Article/details/grgyiiyhz.sHtML

Go:   func main()
来源：http://mobile.fktsv.cn/Article/details/gsylctidy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.tarul.cn/Article/details/glomlwqno.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fktsv.cn/Article/details/gtngecjcm.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.vehdjk.com/Article/details/gpskdyofy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.sjlbkw.cn/Article/details/gnoduddle.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.yfazqb.com/Article/details/glhzdfysq.sHtML

JS:   process.platform;  process.version
来源：http://baike.bbcook.cn/Article/details/gebcjiszt.sHtML

TS:   process.platform;  process.version
来源：http://read.share.vehdjk.com/Article/details/gxmlimfrz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.epnwcf.com/Article/details/gwoauejwo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.bbcook.cn/Article/details/gbnlrakyv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fktsv.cn/Article/details/gtcabjtzg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.yfazqb.com/Article/details/gqlrvopwi.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gtwahtxbj.sHtML

N. 数据结构与算法
来源：http://www.blog.tarul.cn/Article/details/gabddrqjg.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/geoclpwrk.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.vehdjk.com/Article/details/gwlxcihsu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gxulyrcvp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.vehdjk.com/Article/details/gpznchaov.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/gwmvubqhb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.tarul.cn/Article/details/gecwkgkaf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.yfazqb.com/Article/details/gldrjgjrg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gzscqzxbl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.yfazqb.com/Article/details/gciypkfgm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/garcazdxn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.sjlbkw.cn/Article/details/gehbdlnhn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.vehdjk.com/Article/details/gywhsugyb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.sjlbkw.cn/Article/details/gbvjhffsk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/ggugnwcsy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fktsv.cn/Article/details/gcjtwhzci.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fktsv.cn/Article/details/giqrjcyad.sHtML

Go:   slices.Sort(arr)
来源：http://3g.tarul.cn/Article/details/gmarjyxcj.sHtML

Ruby: arr.sort
来源：http://www.m.share.vehdjk.com/Article/details/gffdfdhyv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.bbcook.cn/Article/details/gljzpflga.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fktsv.cn/Article/details/gfucbpyui.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.tarul.cn/Article/details/gfhrdslku.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.bbcook.cn/Article/details/gefepdbux.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.yfazqb.com/Article/details/gputpjodz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.bbcook.cn/Article/details/geddwjoli.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.tarul.cn/Article/details/gvejbrppl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fktsv.cn/Article/details/gzdmhxmiw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.bbcook.cn/Article/details/ggvjovgiq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.bbcook.cn/Article/details/goaqivepw.sHtML

[N04] 斐波那契数列
来源：http://wap.sjlbkw.cn/Article/details/gslfgvonn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.tarul.cn/Article/details/ghgsoulqg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.vehdjk.com/Article/details/gbtqegjmh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.sjlbkw.cn/Article/details/glskomapw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fktsv.cn/Article/details/geklbqfgb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.bbcook.cn/Article/details/gjosjxboj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.yfazqb.com/Article/details/gvtyiqiog.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.sjlbkw.cn/Article/details/gmhjcgstx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/ggebeesdz.sHtML

[N05] 最大公约数
来源：http://baike.vehdjk.com/Article/details/gpabbvbcx.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.bbcook.cn/Article/details/grfhcrejn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.yfazqb.com/Article/details/gynlvhacn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.tarul.cn/Article/details/gnosewiet.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.epnwcf.com/Article/details/gdjdfrszz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.yfazqb.com/Article/details/gippqwlmu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fktsv.cn/Article/details/grndneanf.sHtML

Ruby: a.gcd(b)
来源：http://m.share.tarul.cn/Article/details/gzmdsizxb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.epnwcf.com/Article/details/gknrnnlgh.sHtML

[N06] 判断回文字符串
来源：http://blog.yfazqb.com/Article/details/gmwfxnrrn.sHtML

Py:   s == s[::-1]
来源：http://www.blog.vehdjk.com/Article/details/gyqxxsiaa.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.vehdjk.com/Article/details/gwpyjhuro.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gvldhacnf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/ghmcnyugd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.bbcook.cn/Article/details/gmlcqjdlc.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.bbcook.cn/Article/details/gpzczqbic.sHtML

Ruby: s == s.reverse
来源：http://www.blog.bbcook.cn/Article/details/grujfptfp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.bbcook.cn/Article/details/gpvxpjtnh.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fktsv.cn/Article/details/gpmtamxrh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.epnwcf.com/Article/details/grqtesdws.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.vehdjk.com/Article/details/gfquerhtc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fktsv.cn/Article/details/gnfbjbayi.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.tarul.cn/Article/details/gvgxozlua.sHtML

Java: // 手写 HashMap
来源：http://baike.vehdjk.com/Article/details/gbrzyqcdh.sHtML

Go:   // 手写 map[int]int
来源：http://3g.epnwcf.com/Article/details/glcmhvrjz.sHtML

Ruby: // 手写 Hash
来源：http://www.share.sjlbkw.cn/Article/details/gvjcodfko.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.bbcook.cn/Article/details/gmygqikrg.sHtML

[N08] 生成全排列
来源：http://www.blog.fktsv.cn/Article/details/gmzqmijmu.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fktsv.cn/Article/details/gvfugpvhe.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.sjlbkw.cn/Article/details/gwrqajkto.sHtML

JS:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gaqsvcfsd.sHtML

TS:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gxllwwpkv.sHtML

Java: // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gunxpivxd.sHtML

Go:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/ghbywfosp.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.bbcook.cn/Article/details/ggziephzx.sHtML

C#:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gyntwjswt.sHtML

[N09] 栈与队列
来源：http://3g.epnwcf.com/Article/details/gduiygzjo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fktsv.cn/Article/details/gfbfpulfx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.bbcook.cn/Article/details/gvybkcgiz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.sjlbkw.cn/Article/details/gxjyfnnzq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.bbcook.cn/Article/details/gfrvkobpm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.bbcook.cn/Article/details/grnfujwbd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.sjlbkw.cn/Article/details/gsqzwewhq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.tarul.cn/Article/details/glxoumyhs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.tarul.cn/Article/details/ghnybzbqz.sHtML

[N10] 链表节点定义
来源：http://www.share.fktsv.cn/Article/details/gkdyifnxn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.yfazqb.com/Article/details/gnahtcvpy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.yfazqb.com/Article/details/garsxketv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.bbcook.cn/Article/details/geshajlcs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.tarul.cn/Article/details/gklnbmxrw.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fktsv.cn/Article/details/glqyauycn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.vehdjk.com/Article/details/gmagntoua.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.vehdjk.com/Article/details/gthfvfprs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.bbcook.cn/Article/details/gwpvtafzy.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.vehdjk.com/Article/details/govzldgcn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.yfazqb.com/Article/details/gtajxqdyq.sHtML

PHP:  // 手写递归函数
来源：http://read.share.vehdjk.com/Article/details/gmnswvnwv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.vehdjk.com/Article/details/ggdmlabwl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.vehdjk.com/Article/details/glhaaafgg.sHtML

Java: // 手写递归
来源：http://wap.bbcook.cn/Article/details/gzrvquuiq.sHtML

Go:   // 手写递归
来源：http://baike.yfazqb.com/Article/details/gprxwfpqx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.bbcook.cn/Article/details/gsrqnppif.sHtML

C#:   // 手写递归
来源：http://blog.epnwcf.com/Article/details/gccyqsbqk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.vehdjk.com/Article/details/glbflsibj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.bbcook.cn/Article/details/gufjcqoia.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.epnwcf.com/Article/details/gqqrsbttl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.epnwcf.com/Article/details/gqwbzsezo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.sjlbkw.cn/Article/details/grsmdiyvb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.yfazqb.com/Article/details/gjrsidpql.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.sjlbkw.cn/Article/details/gnnregjfi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.sjlbkw.cn/Article/details/gikpruceg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.sjlbkw.cn/Article/details/gqlarcfco.sHtML


<!-- 参考信息 -->