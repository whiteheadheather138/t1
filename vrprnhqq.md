代发 wailian999

TS:   JSON.parse(s)
来源：http://hug.epnwcf.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://shb.yuxming.cn

Go:   json.Unmarshal(data, &v)
来源：http://gsp.xuetiantiany.cn

Ruby: JSON.parse(s)
来源：http://xee.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kwo.fanxiaobao.xyz

[K03] JSON 美化输出（带缩进）
来源：http://jfb.yueranfly.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lzc.xuanzx.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jtw.chenlongwang.top

JS:   JSON.stringify(obj, null, 2)
来源：http://zdg.yueranfly.top

TS:   JSON.stringify(obj, null, 2)
来源：http://oqo.mhx1999.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ttn.svipenyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kki.tarul.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ddr.zhoulong.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://euq.vehdjk.com

[K04] 读取 JSON 文件
来源：http://xpe.andypj.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://imq.cheryme.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fnc.cucudq.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://edl.0kj1m.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jjp.cucudq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jnd.zhongyouzk.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rry.dianchejie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hqo.jinghuilouyu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rdd.xingfuxueyuan.xyz

[K05] 深拷贝对象
来源：http://rss.jiagoushi.top

Py:   copy.deepcopy(obj)
来源：http://nwx.vehdjk.com

PHP:  unserialize(serialize($obj));
来源：http://djc.yanxiufei.cn

JS:   structuredClone(obj)
来源：http://iiw.gotoacloud.top

TS:   structuredClone(obj)
来源：http://jpd.chenjidiqi.icu

Java: // 手写拷贝构造，或序列化往返
来源：http://cms.nwbrower.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lgi.sufxvd.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://clg.yueranfly.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zwa.wangshuangyany.cn

[K06] 解析 URL 查询串
来源：http://ajf.ydjk.org.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ahd.yj202588.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dtr.yj202588.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fpg.wangshuangyany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yjr.shanyushiyangtech.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://eup.tanke756.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xam.xylfe.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ppi.dianchejie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lht.xuanzx.com

[K07] 进制转换
来源：http://yll.snrcjt.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vla.jiagoushi.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oan.quarkkingdee.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kch.dashuyun.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wnm.ivvv.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vaq.yangfankeji.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rgd.sysykeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fyu.cucudq.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://moa.jinqigufen.top

[K08] 二进制序列化（非 JSON）
来源：http://qxi.ydjk.org.cn

Py:   pickle.dumps(obj)
来源：http://wqr.guowangkeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://tgl.chenzaomai.com

JS:   v8.serialize(obj)        // Node
来源：http://rsq.smart0.xyz

TS:   v8.serialize(obj)        // Node
来源：http://ifv.havefunace.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kib.c1oappe.top

Go:   encoding/gob
来源：http://rtd.fzhhl.top

Ruby: Marshal.dump(obj)
来源：http://vmq.iojbl.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wak.mhx1999.top

================================================================================
来源：http://goe.xziqi.cn

L. 网络请求
来源：http://nwd.0kj1m.cn

================================================================================
来源：http://sgl.pengpengdd.cyou

[L01] 发送 GET 请求
来源：http://rie.jyoumei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fyt.tarul.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dch.c1oappe.top

JS:   await fetch(url)
来源：http://vmo.sxryk.cn

TS:   await fetch(url)
来源：http://dhk.bjfxy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ffw.chenjidiqi.icu

Go:   resp, err := http.Get(url)
来源：http://euh.zhiwuduotai.top

Ruby: Net::HTTP.get(URI(url))
来源：http://btp.zhiwuduotai.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wvu.jlsjyb.cn

[L02] 发送 POST JSON
来源：http://ijn.cdnleiting.top

Py:   requests.post(url, json={"a": 1})
来源：http://fca.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hrq.zycfv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ayw.0kj1m.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jof.jiagoushi.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rjb.sweek.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qaw.hammf.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hax.0kj1m.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ais.fehbvm.com

[L03] 设置自定义请求头
来源：http://yka.zycfv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://onn.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tmm.quarkkingdee.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kwq.xziqi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aek.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gua.epnwcf.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sjx.shuidangran.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wxu.cheryme.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vvm.hywenlv.cn

[L04] 设置超时
来源：http://zrh.nanxuanxn.top

Py:   requests.get(url, timeout=5)
来源：http://kle.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://exb.yueranfly.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xmx.xingfuxueyuan.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wrk.zhongyouzk.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://muv.yueranfly.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sys.nwbrower.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qlh.hesvh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cqp.zhixingplan.top

[L05] 上传文件（multipart）
来源：http://mmj.tianlin.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tfj.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fvf.nwbrower.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cni.vehdjk.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fvw.yj20258888.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://poy.tian-w.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ofu.guowangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://aee.quarkkingdee.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://icq.yj202588.top

[L06] 解析响应为 JSON
来源：http://hpf.tarul.cn

Py:   resp.json()
来源：http://rsl.pycfn.com

PHP:  json_decode($body, true);
来源：http://ggj.ppjwa.cn

JS:   await resp.json()
来源：http://xfo.yfazqb.com

TS:   await resp.json()
来源：http://ixc.jyoumei.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jyu.yuanzhike.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kob.yfazqb.com

Ruby: JSON.parse(resp.body)
来源：http://gvl.cashguo.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://syl.yonumen.top

[L07] 处理 HTTP 状态码
来源：http://jrj.sxryk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jmj.kuanghao11.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nkf.snrcjt.cn

JS:   resp.ok;  resp.status
来源：http://jag.yfazqb.com

TS:   resp.ok;  resp.status
来源：http://znq.aibaodan.cn

Java: resp.statusCode()
来源：http://wkh.hysaishi.cn

Go:   resp.StatusCode
来源：http://rll.xziqi.cn

Ruby: resp.code.to_i
来源：http://ike.ehwqpu.com

C#:   (int)resp.StatusCode
来源：http://uev.svipenyu.cn

[L08] 并发请求多个地址
来源：http://roj.ctjpmb.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://puh.ydzc1.top

PHP:  curl_multi_init() 系列
来源：http://mhq.yvedp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pgl.shzxlz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iul.shanyushiyangtech.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nvm.jinqigfzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zua.bjfxy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ari.gzhubu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://moc.andypj.xyz

================================================================================
来源：http://fnx.9152youxi.cn

M. 命令行 / 进程 / 环境
来源：http://zij.c1oappe.top

================================================================================
来源：http://zgl.gogol.net.cn

[M01] 读取命令行参数
来源：http://ero.cucudq.cn

Py:   sys.argv[1:]
来源：http://qmv.sufxvd.cn

PHP:  $argv;  $argc;
来源：http://kii.zhijiandao.cn

JS:   process.argv.slice(2)
来源：http://idi.yuxming.cn

TS:   process.argv.slice(2)
来源：http://ttn.jqgfzy.top

Java: args 数组（main 方法参数）
来源：http://eev.meibo888.top

Go:   os.Args[1:]
来源：http://nbm.zhengqikj.top

Ruby: ARGV
来源：http://xxg.zdbjq.cn

C#:   args 数组（Main 方法参数）
来源：http://gyn.zhijiandao.cn

[M02] 读取环境变量
来源：http://tdz.ctjpmb.com

Py:   os.environ.get("HOME")
来源：http://vmg.yueranfly.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://duz.ppjwa.cn

JS:   process.env.HOME
来源：http://atr.ehwqpu.com

TS:   process.env.HOME
来源：http://pau.yuxming.cn

Java: System.getenv("HOME")
来源：http://tsd.kuanghao11.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zni.dashuyun.cn

Ruby: ENV["HOME"]
来源：http://vgh.bbcook.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rjs.sxryk.cn

[M03] 执行外部命令
来源：http://yzf.wangshuangyany.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dzg.xinyue.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sqi.shuidangran.top

JS:   child_process.execSync("ls -l").toString()
来源：http://qih.zhongyouzk.top

TS:   child_process.execSync("ls -l").toString()
来源：http://qlk.aibaodan.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qoc.hcnkem.com

Go:   exec.Command("ls", "-l").Output()
来源：http://yga.hesvh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rnn.sjlbkw.cn

C#:   Process.Start("ls", "-l");
来源：http://cbx.jinqigfzy.top

[M04] 获取当前工作目录
来源：http://ddn.xinyue.icu

Py:   os.getcwd()
来源：http://wtn.mhx1999.top

PHP:  getcwd();
来源：http://cbd.ybcxt.top

JS:   process.cwd()
来源：http://xiu.sxryk.cn

TS:   process.cwd()
来源：http://ypv.meibo888.top

Java: Path.of("").toAbsolutePath()
来源：http://dhs.dashuyun.cn

Go:   os.Getwd()
来源：http://osk.yueranfly.top

Ruby: Dir.pwd
来源：http://lin.shanyushiyangkeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://jlg.xinyue.icu

[M05] 设置退出码
来源：http://keh.shanyushiyangkeji.top

Py:   sys.exit(1)
来源：http://kth.hywenlv.cn

PHP:  exit(1);
来源：http://hcy.pycfn.com

JS:   process.exit(1)
来源：http://oqx.snrcjt.cn

TS:   process.exit(1)
来源：http://dnz.fanxiaobao.xyz

Java: System.exit(1)
来源：http://nkq.fengsongda.top

Go:   os.Exit(1)
来源：http://uhy.tianlin.xyz

Ruby: exit 1
来源：http://vvw.fengsongda.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fzq.chenlongwang.top

[M06] 向标准错误输出
来源：http://okn.nanxuanxn.top

Py:   print("err", file=sys.stderr)
来源：http://xuy.feifeiyinyue.top

PHP:  fwrite(STDERR, "err\n");
来源：http://kma.wangdashe.top

JS:   console.error("err")
来源：http://vdk.9152youxi.cn

TS:   console.error("err")
来源：http://ttz.yj202588.top

Java: System.err.println("err")
来源：http://vto.ppjwa.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qsd.sxryk.cn

Ruby: warn "err"
来源：http://woj.redwolf501.top

C#:   Console.Error.WriteLine("err")
来源：http://psj.hcnkem.com

[M07] 判断是否为主入口
来源：http://ecq.dianchejie.cn

Py:   if __name__ == "__main__":
来源：http://lpp.hywenlv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cfu.gaohongyu789.top

JS:   require.main === module
来源：http://rdt.snrcjt.cn

TS:   require.main === module
来源：http://wrp.jinyuanbaomall.cn

Java: public static void main(String[] args)
来源：http://fwm.zhiwuduotai.top

Go:   func main()
来源：http://fvn.zhaomingkeji.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ekl.havefunace.top

C#:   static void Main(string[] args)
来源：http://ufk.xinyue.icu

[M08] 获取系统与运行时信息
来源：http://xai.dianchejie.cn

Py:   platform.system();  platform.python_version()
来源：http://olp.sysykeji.top

PHP:  PHP_OS;  phpversion();
来源：http://eut.zhengqikj.top

JS:   process.platform;  process.version
来源：http://qas.tianlin.xyz

TS:   process.platform;  process.version
来源：http://qdl.zycfv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ccu.tarul.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://quc.316326.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ptv.ywan-chungtsiang.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://cyg.uphjek.com

================================================================================
来源：http://ozv.hfpthk.cn

N. 数据结构与算法
来源：http://iow.ctjpmb.com

================================================================================
来源：http://xmj.cdnleiting.top

[N01] 二分查找（有序数组）
来源：http://bak.yonumen.top

Py:   bisect.bisect_left(arr, x)
来源：http://woa.dashuyun.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dkq.vehdjk.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tnb.cucudq.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dyq.havefunace.top

Java: Arrays.binarySearch(arr, x)
来源：http://dyp.ydzc1.top

Go:   sort.SearchInts(arr, x)
来源：http://qax.sxryk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://csd.yonumen.top

C#:   Array.BinarySearch(arr, x)
来源：http://gpp.hesvh.cn

[N02] 排序（工程实践用内置实现）
来源：http://evq.yj20258.top

Py:   sorted(arr);  arr.sort()
来源：http://gcn.guowangkeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qla.smart0.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://ujw.tian-w.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://eas.gaohongyu789.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zoz.mhx1999.top

Go:   slices.Sort(arr)
来源：http://kfh.ydjk.org.cn

Ruby: arr.sort
来源：http://nap.xuanzx.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://rhd.hongshengwenyu.top

[N03] 快速排序（分治示例）
来源：http://tbh.fanxiaobao.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zxb.jinqigufen.top

PHP:  // 递归实现，或用 usort
来源：http://qqd.zhengqikj.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tfv.9152youxi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://koq.birdmap.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lgp.tanke756.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jvr.hammf.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://asv.pengpengdd.cyou

C#:   // 手写递归，或 Array.Sort
来源：http://dqj.yongpay.top

[N04] 斐波那契数列
来源：http://asm.cqqwz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://eik.havefunace.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hbs.xylfe.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pgv.tarul.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nxi.zdqjudy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hbq.fanxiaobao.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rhf.yvedp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gzo.yvedp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mhg.yangfankeji.com

[N05] 最大公约数
来源：http://sop.nanxuanxn.top

Py:   math.gcd(a, b)
来源：http://ufd.birdmap.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cpj.fehbvm.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wfr.yongpay.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://enm.9152youxi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fsv.shanyushiyangkeji.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://emg.yonumen.top

Ruby: a.gcd(b)
来源：http://jzh.jinqigfzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lpt.jlsjyb.cn

[N06] 判断回文字符串
来源：http://prw.fktsv.cn

Py:   s == s[::-1]
来源：http://uco.xinyue.icu

PHP:  $s === strrev($s);
来源：http://nkv.snrcjt.cn

JS:   s === [...s].reverse().join("")
来源：http://xui.guowangkeji.top

TS:   s === [...s].reverse().join("")
来源：http://nwt.hywenlv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cfh.yonumen.top

Go:   // 双指针从两端比较
来源：http://ade.hammf.cn

Ruby: s == s.reverse
来源：http://lvw.hywenlv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tfv.ctjpmb.com

[N07] 两数之和（返回下标）
来源：http://lre.nwbrower.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hvi.zhengqikj.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vbf.jyoumei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://whj.ehwqpu.com

TS:   // 手写 Map<string, number>
来源：http://aio.haohaochexian.top

Java: // 手写 HashMap
来源：http://xjn.kuanghao11.cn

Go:   // 手写 map[int]int
来源：http://gwv.yvedp.cn

Ruby: // 手写 Hash
来源：http://jqa.wangdashe.top

C#:   // 手写 Dictionary<int, int>
来源：http://akw.fktsv.cn

[N08] 生成全排列
来源：http://hic.jinghuilouyu.cn

Py:   itertools.permutations(arr)
来源：http://bzh.vehdjk.com

PHP:  // 手写递归交换
来源：http://mpg.xinyue.icu

JS:   // 手写回溯递归
来源：http://zka.xingfuxueyuan.xyz

TS:   // 手写回溯递归
来源：http://ole.daria6918.cn

Java: // 手写回溯递归
来源：http://foe.fktsv.cn

Go:   // 手写回溯递归
来源：http://dpk.dianchejie.cn

Ruby: arr.permutation.to_a
来源：http://oxf.jiagoushi.top

C#:   // 手写回溯递归
来源：http://vsr.sufxvd.cn

[N09] 栈与队列
来源：http://kxj.yj20258.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nmz.yfazqb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dao.cucudq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qec.gotoacloud.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ydb.wangshuangyany.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ups.nanxinkj.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dzi.snrcjt.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wba.xziqi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://npz.hammf.cn

[N10] 链表节点定义
来源：http://fvf.sysykeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lcs.zhixingplan.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ksz.fehbvm.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://azg.chenlongwang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zee.hnxiangtu.top

Java: class Node { int v; Node next; }
来源：http://mpi.redwolf501.top

Go:   type Node struct { V int; Next *Node }
来源：http://prt.yfazqb.com


<!-- 参考信息 -->