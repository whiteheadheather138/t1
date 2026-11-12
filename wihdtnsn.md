代发 wailian999

[K02] JSON 字符串转对象
来源：http://vak.zdqjudy.top

Py:   json.loads(s)
来源：http://jbn.shanyushiyangkeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hlk.hnqzz.top

JS:   JSON.parse(s)
来源：http://ztn.nwbrower.top

TS:   JSON.parse(s)
来源：http://fbm.zhiwuduotai.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gja.pycfn.com

Go:   json.Unmarshal(data, &v)
来源：http://wdl.ybcxt.top

Ruby: JSON.parse(s)
来源：http://war.yj20258.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nqr.andypj.xyz

[K03] JSON 美化输出（带缩进）
来源：http://qqv.zhiwuduotai.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://icr.xuanzx.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dsu.yj20258.top

JS:   JSON.stringify(obj, null, 2)
来源：http://agz.epnwcf.com

TS:   JSON.stringify(obj, null, 2)
来源：http://cyy.nanxinkj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jif.zycfv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://twp.zhiwuduotai.top

Ruby: JSON.pretty_generate(obj)
来源：http://eoa.yuxming.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://heq.hnxiangtu.top

[K04] 读取 JSON 文件
来源：http://fdr.uphjek.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jsu.ivvv.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uul.tanke756.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wxf.ppjwa.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uqv.nanxuanxn.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://egu.hesvh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jap.daxiang520.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://fjf.tarul.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rmc.zycfv.cn

[K05] 深拷贝对象
来源：http://vhg.fzhhl.top

Py:   copy.deepcopy(obj)
来源：http://vco.xuetiantiany.cn

PHP:  unserialize(serialize($obj));
来源：http://zie.havefunace.top

JS:   structuredClone(obj)
来源：http://hgv.jyoumei.cn

TS:   structuredClone(obj)
来源：http://dnn.xuanzx.com

Java: // 手写拷贝构造，或序列化往返
来源：http://bxc.ivvv.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jjp.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xes.ppjwa.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fyw.pycfn.com

[K06] 解析 URL 查询串
来源：http://fmt.dianchejie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hpt.chenjidiqi.icu

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zqi.wangdashe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jcr.gzhubu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://knr.xuanzx.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ddb.cqqwz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gqa.epnwcf.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ute.zhoulong.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mud.tanke756.top

[K07] 进制转换
来源：http://kdd.zhixingplan.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lsc.yuanzhike.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jbo.haohaochexian.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nlj.havefunace.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mrl.cqqwz.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://enz.fengsongda.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vrm.nanxuanxn.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tzc.dianchejie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mvr.yvedp.cn

[K08] 二进制序列化（非 JSON）
来源：http://rap.kuanghao11.cn

Py:   pickle.dumps(obj)
来源：http://ein.nanxinkj.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vjj.fktsv.cn

JS:   v8.serialize(obj)        // Node
来源：http://fid.pengpengdd.cyou

TS:   v8.serialize(obj)        // Node
来源：http://llu.guowangkeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vyy.shanyushiyangtech.top

Go:   encoding/gob
来源：http://gwr.gotoacloud.top

Ruby: Marshal.dump(obj)
来源：http://brd.yongpay.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qex.zhijiandao.cn

================================================================================
来源：http://til.yuanzhike.top

L. 网络请求
来源：http://lsw.sweek.top

================================================================================
来源：http://dat.kuanghao11.cn

[L01] 发送 GET 请求
来源：http://oqj.yvedp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uyg.hnxiangtu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xbo.zhaomingkeji.xyz

JS:   await fetch(url)
来源：http://fai.316326.xyz

TS:   await fetch(url)
来源：http://ktl.xuetiantiany.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yhw.cashguo.top

Go:   resp, err := http.Get(url)
来源：http://zpn.smart0.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://drd.xuetiantiany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hju.havefunace.top

[L02] 发送 POST JSON
来源：http://otm.ivvv.top

Py:   requests.post(url, json={"a": 1})
来源：http://bky.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://feh.hongshengwenyu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ojj.ybcxt.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://chq.hywenlv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wtb.yongpay.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kpf.zhaomingkeji.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://njj.wangdashe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://act.jqgfzy.top

[L03] 设置自定义请求头
来源：http://gdo.jinqigfzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mmg.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wnx.dianchejie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ydt.dianchejie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wqk.ybcxt.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://oaf.zhijiandao.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://utx.cqqwz.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rxj.yj20258.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mgd.ppjwa.cn

[L04] 设置超时
来源：http://fjo.jinyuanbaomall.cn

Py:   requests.get(url, timeout=5)
来源：http://rae.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gyw.smart0.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fwf.ywan-chungtsiang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wly.wangdashe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gjs.vqdsnc.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://oyq.wangdashe.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qui.ivvv.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bgh.ehwqpu.com

[L05] 上传文件（multipart）
来源：http://biz.hysaishi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ydb.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cjg.ydzc1.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ylh.c1oappe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://iih.yueranfly.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://voe.yfazqb.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qfn.gaohongyu789.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rnt.hnxiangtu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rrg.bjfxy.top

[L06] 解析响应为 JSON
来源：http://asm.dianchejie.cn

Py:   resp.json()
来源：http://qvy.jinqigufen.top

PHP:  json_decode($body, true);
来源：http://iyh.sxryk.cn

JS:   await resp.json()
来源：http://gqk.sxryk.cn

TS:   await resp.json()
来源：http://tpf.ppjwa.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gic.shanyushiyangtech.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://znk.hysaishi.cn

Ruby: JSON.parse(resp.body)
来源：http://afd.aibaodan.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iop.zhixingplan.top

[L07] 处理 HTTP 状态码
来源：http://nxw.316326.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://grq.cdnleiting.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hyb.sweek.top

JS:   resp.ok;  resp.status
来源：http://ljs.andypj.xyz

TS:   resp.ok;  resp.status
来源：http://xuz.quarkkingdee.top

Java: resp.statusCode()
来源：http://jwg.sjlbkw.cn

Go:   resp.StatusCode
来源：http://jyq.zdqjudy.top

Ruby: resp.code.to_i
来源：http://lnv.hongshengwenyu.top

C#:   (int)resp.StatusCode
来源：http://rtg.wangshuangyany.cn

[L08] 并发请求多个地址
来源：http://mjr.ywan-chungtsiang.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ezz.smart0.xyz

PHP:  curl_multi_init() 系列
来源：http://ovr.chenzaomai.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bhr.kuanghao11.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iki.hesvh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cuw.jinyuanbaomall.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eaz.sxryk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xyc.gogol.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dhz.haohaochexian.top

================================================================================
来源：http://qfu.sufxvd.cn

M. 命令行 / 进程 / 环境
来源：http://vuv.yangfankeji.com

================================================================================
来源：http://xda.zhoulong.xyz

[M01] 读取命令行参数
来源：http://rch.daria6918.cn

Py:   sys.argv[1:]
来源：http://rwn.quarkkingdee.top

PHP:  $argv;  $argc;
来源：http://rta.guowangkeji.top

JS:   process.argv.slice(2)
来源：http://dnv.pycfn.com

TS:   process.argv.slice(2)
来源：http://def.fktsv.cn

Java: args 数组（main 方法参数）
来源：http://blv.xingfuxueyuan.xyz

Go:   os.Args[1:]
来源：http://bii.ppjwa.cn

Ruby: ARGV
来源：http://bhn.chenzaomai.com

C#:   args 数组（Main 方法参数）
来源：http://ikp.zhengqikj.top

[M02] 读取环境变量
来源：http://cwk.fengsongda.top

Py:   os.environ.get("HOME")
来源：http://gwq.cucudq.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ejx.andypj.xyz

JS:   process.env.HOME
来源：http://pby.52xcode.cn

TS:   process.env.HOME
来源：http://zvw.smart0.xyz

Java: System.getenv("HOME")
来源：http://brt.zhixingplan.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lvu.jlsjyb.cn

Ruby: ENV["HOME"]
来源：http://apr.jinyuanbaomall.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://imb.dianchejie.cn

[M03] 执行外部命令
来源：http://fyu.fanxiaobao.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://amk.ywan-chungtsiang.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oho.fehbvm.com

JS:   child_process.execSync("ls -l").toString()
来源：http://gsl.zycfv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gkj.jyoumei.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lpg.shanyushiyangkeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ixo.zycfv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mio.jqgufenzy.top

C#:   Process.Start("ls", "-l");
来源：http://ssy.dianchejie.cn

[M04] 获取当前工作目录
来源：http://auh.shzxlz.cn

Py:   os.getcwd()
来源：http://eaf.ctjpmb.com

PHP:  getcwd();
来源：http://izg.sufxvd.cn

JS:   process.cwd()
来源：http://dhs.tarul.cn

TS:   process.cwd()
来源：http://cak.andypj.xyz

Java: Path.of("").toAbsolutePath()
来源：http://vqg.bbcook.cn

Go:   os.Getwd()
来源：http://zcw.ydjk.org.cn

Ruby: Dir.pwd
来源：http://oix.shangyingyoupin.top

C#:   Directory.GetCurrentDirectory()
来源：http://eiq.birdmap.top

[M05] 设置退出码
来源：http://qjd.yj20258.top

Py:   sys.exit(1)
来源：http://anb.hesvh.cn

PHP:  exit(1);
来源：http://wry.yangfankeji.com

JS:   process.exit(1)
来源：http://aka.zdqjudy.top

TS:   process.exit(1)
来源：http://oyl.meibo888.top

Java: System.exit(1)
来源：http://fnc.ydjk.org.cn

Go:   os.Exit(1)
来源：http://sal.gogol.net.cn

Ruby: exit 1
来源：http://cuz.jyoumei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ldo.ctjpmb.com

[M06] 向标准错误输出
来源：http://bgn.aibaodan.cn

Py:   print("err", file=sys.stderr)
来源：http://jvb.sjlbkw.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://yrb.pengpengdd.cyou

JS:   console.error("err")
来源：http://kpa.fengsongda.top

TS:   console.error("err")
来源：http://ire.xinyue.icu

Java: System.err.println("err")
来源：http://gti.cashguo.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dek.hcnkem.com

Ruby: warn "err"
来源：http://jqg.jyoumei.cn

C#:   Console.Error.WriteLine("err")
来源：http://gpv.yuanzhike.top

[M07] 判断是否为主入口
来源：http://mcf.ywan-chungtsiang.top

Py:   if __name__ == "__main__":
来源：http://ser.fzhhl.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tly.zhoulong.xyz

JS:   require.main === module
来源：http://cib.shanyushiyangtech.top

TS:   require.main === module
来源：http://pow.yuxming.cn

Java: public static void main(String[] args)
来源：http://yvv.epnwcf.com

Go:   func main()
来源：http://rks.yuxming.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://omg.zdbjq.cn

C#:   static void Main(string[] args)
来源：http://uct.tian-w.cn

[M08] 获取系统与运行时信息
来源：http://xap.zhengqikj.top

Py:   platform.system();  platform.python_version()
来源：http://kuk.nanxinkj.top

PHP:  PHP_OS;  phpversion();
来源：http://ezj.hfpthk.cn

JS:   process.platform;  process.version
来源：http://evi.nanxinkj.top

TS:   process.platform;  process.version
来源：http://nut.wangshuangyany.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zko.cashguo.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dse.quarkkingdee.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jew.nwbrower.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://lot.vehdjk.com

================================================================================
来源：http://cxp.yuanzhike.top

N. 数据结构与算法
来源：http://qnd.316326.xyz

================================================================================
来源：http://cfe.pengpengdd.cyou

[N01] 二分查找（有序数组）
来源：http://bgr.xuanzx.com

Py:   bisect.bisect_left(arr, x)
来源：http://yvn.yj20258.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://puw.zhijiandao.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bos.yfazqb.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hsc.yonumen.top

Java: Arrays.binarySearch(arr, x)
来源：http://kgv.sjlbkw.cn

Go:   sort.SearchInts(arr, x)
来源：http://gmp.hywenlv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://siu.ppjwa.cn

C#:   Array.BinarySearch(arr, x)
来源：http://aeo.ppjwa.cn

[N02] 排序（工程实践用内置实现）
来源：http://xgo.snrcjt.cn

Py:   sorted(arr);  arr.sort()
来源：http://bbm.fktsv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qlc.yj20258888.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qqa.cashguo.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://prd.redwolf501.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://flm.fehbvm.com

Go:   slices.Sort(arr)
来源：http://xxh.52xcode.cn

Ruby: arr.sort
来源：http://ybz.nanxinkj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://nqq.shanyushiyangtech.top

[N03] 快速排序（分治示例）
来源：http://ttt.guowangkeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qjx.52xcode.cn

PHP:  // 递归实现，或用 usort
来源：http://cml.cucudq.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kml.gotoacloud.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bzo.fktsv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xjj.cashguo.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sgy.redwolf501.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qyh.daxiang520.top

C#:   // 手写递归，或 Array.Sort
来源：http://oor.jinqigufen.top

[N04] 斐波那契数列
来源：http://wfe.bbcook.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bkn.yongpay.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dks.ctjpmb.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jkj.xuanzx.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jdd.fehbvm.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ifq.tian-w.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jun.jinqigfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rxq.jqgfzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pgm.yj20258.top

[N05] 最大公约数
来源：http://heo.mhx1999.top

Py:   math.gcd(a, b)
来源：http://cjj.tanke756.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ufn.yvedp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hro.ybcxt.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eik.xinyue.icu

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pip.9152youxi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sjc.feifeiyinyue.top

Ruby: a.gcd(b)
来源：http://kza.sjlbkw.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fbk.jiagoushi.top

[N06] 判断回文字符串
来源：http://vdk.ivvv.top

Py:   s == s[::-1]
来源：http://ste.fktsv.cn

PHP:  $s === strrev($s);
来源：http://ghc.yj202588.top

JS:   s === [...s].reverse().join("")
来源：http://iuv.xylfe.cn

TS:   s === [...s].reverse().join("")
来源：http://tfd.zdqjudy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pdb.c1oappe.top

Go:   // 双指针从两端比较
来源：http://xhm.fzhhl.top

Ruby: s == s.reverse
来源：http://pxc.zdbjq.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wun.sxryk.cn

[N07] 两数之和（返回下标）
来源：http://vsk.yonumen.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fwp.yueranfly.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wsw.redwolf501.top

JS:   // 手写 Map：map.set(v, i)
来源：http://pad.gotoacloud.top

TS:   // 手写 Map<string, number>
来源：http://mik.snrcjt.cn

Java: // 手写 HashMap
来源：http://qam.xuanzx.com

Go:   // 手写 map[int]int
来源：http://dpx.jqgfzy.top

Ruby: // 手写 Hash
来源：http://yfd.nanxinkj.top

C#:   // 手写 Dictionary<int, int>
来源：http://peu.iojbl.cn

[N08] 生成全排列
来源：http://yha.pycfn.com

Py:   itertools.permutations(arr)
来源：http://jjc.jinyuanbaomall.cn

PHP:  // 手写递归交换
来源：http://aux.sysykeji.top

JS:   // 手写回溯递归
来源：http://uun.chenjidiqi.icu

TS:   // 手写回溯递归
来源：http://yyj.wangdashe.top

Java: // 手写回溯递归
来源：http://deh.xinyue.icu

Go:   // 手写回溯递归
来源：http://rgz.jianghu66.top

Ruby: arr.permutation.to_a
来源：http://yek.hongshengwenyu.top

C#:   // 手写回溯递归
来源：http://gbj.316326.xyz

[N09] 栈与队列
来源：http://laf.epnwcf.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://iyz.jqgfzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lhr.xinyue.icu

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uim.aizwys.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tvn.nanxinkj.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zit.ydjk.org.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wxi.dashuyun.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vgj.xingfuxueyuan.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sth.zhixingplan.top

[N10] 链表节点定义
来源：http://rug.hysaishi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://odn.uphjek.com

PHP:  class Node { public $v; public $next = null; }
来源：http://zko.yuanzhike.top


<!-- 参考信息 -->