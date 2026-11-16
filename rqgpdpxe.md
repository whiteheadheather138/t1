代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://riv.ywan-chungtsiang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fmo.epnwcf.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lqw.tarul.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://apz.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dql.nwbrower.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://rwo.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nnq.ctjpmb.com

[K05] 深拷贝对象
来源：http://iyd.ctjpmb.com

Py:   copy.deepcopy(obj)
来源：http://lki.316326.xyz

PHP:  unserialize(serialize($obj));
来源：http://upi.yvedp.cn

JS:   structuredClone(obj)
来源：http://zfq.hammf.cn

TS:   structuredClone(obj)
来源：http://oan.9152youxi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kjp.jinqigfzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kbn.0kj1m.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://msx.ivvv.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ovc.yj20258888.top

[K06] 解析 URL 查询串
来源：http://mbx.hysaishi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cub.hesvh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gxk.hfpthk.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rni.xingfuxueyuan.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://osr.wangdashe.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sif.hnxiangtu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://laq.zycfv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nai.vehdjk.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ijv.andypj.xyz

[K07] 进制转换
来源：http://wul.hammf.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gew.ppjwa.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pgq.aibaodan.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vkp.sweek.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://drc.shangyingyoupin.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xbf.andypj.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yui.yueranfly.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cku.daria6918.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gmp.feifeiyinyue.top

[K08] 二进制序列化（非 JSON）
来源：http://rzl.smart0.xyz

Py:   pickle.dumps(obj)
来源：http://udx.ybcxt.top

PHP:  serialize($obj);  unserialize($s);
来源：http://fvo.yonumen.top

JS:   v8.serialize(obj)        // Node
来源：http://efs.shanyushiyangtech.top

TS:   v8.serialize(obj)        // Node
来源：http://jft.gogol.net.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nma.tanke756.top

Go:   encoding/gob
来源：http://dgc.hnqzz.top

Ruby: Marshal.dump(obj)
来源：http://yyo.yj20258888.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ybm.yuxming.cn

================================================================================
来源：http://wyd.mhx1999.top

L. 网络请求
来源：http://voq.316326.xyz

================================================================================
来源：http://ucf.52xcode.cn

[L01] 发送 GET 请求
来源：http://xqe.0kj1m.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bda.fanxiaobao.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://oty.hysaishi.cn

JS:   await fetch(url)
来源：http://lvt.sweek.top

TS:   await fetch(url)
来源：http://nxx.fanxiaobao.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jve.ydjk.org.cn

Go:   resp, err := http.Get(url)
来源：http://cse.fengsongda.top

Ruby: Net::HTTP.get(URI(url))
来源：http://uko.guannengcc.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://igv.fanxiaobao.xyz

[L02] 发送 POST JSON
来源：http://fsk.hnxiangtu.top

Py:   requests.post(url, json={"a": 1})
来源：http://xme.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ecg.shanyushiyangtech.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cpy.ydzc1.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ndp.jqgufenzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://psy.zhengqikj.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dud.guannengcc.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kcq.kuanghao11.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rzs.yfazqb.com

[L03] 设置自定义请求头
来源：http://mfz.gotoacloud.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hwb.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://acl.chenlongwang.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nji.zhengqikj.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vph.52xcode.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ust.aizwys.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uok.hnqzz.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dys.gogol.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zwl.yfazqb.com

[L04] 设置超时
来源：http://nxa.pycfn.com

Py:   requests.get(url, timeout=5)
来源：http://hpt.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xxh.ydzc1.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rty.hnxiangtu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nzj.sweek.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qvh.gotoacloud.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kvy.52xcode.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rgv.bjfxy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bxw.xuetiantiany.cn

[L05] 上传文件（multipart）
来源：http://avz.tarul.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ziy.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kjg.zhixingplan.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://npd.hysaishi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://big.yfazqb.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wus.redwolf501.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qnu.sjlbkw.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vce.kuanghao11.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ytj.ehwqpu.com

[L06] 解析响应为 JSON
来源：http://mpg.hfpthk.cn

Py:   resp.json()
来源：http://hay.xinyue.icu

PHP:  json_decode($body, true);
来源：http://tvg.chenlongwang.top

JS:   await resp.json()
来源：http://cjg.ydzc1.top

TS:   await resp.json()
来源：http://lpc.nwbrower.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://seo.gogol.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hhd.52xcode.cn

Ruby: JSON.parse(resp.body)
来源：http://swq.fengsongda.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pxh.jinqigfzy.top

[L07] 处理 HTTP 状态码
来源：http://cmi.zdqjudy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://isj.wangshuangyany.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hab.zycfv.cn

JS:   resp.ok;  resp.status
来源：http://isd.ctjpmb.com

TS:   resp.ok;  resp.status
来源：http://fxu.zhijiandao.cn

Java: resp.statusCode()
来源：http://ipv.iojbl.cn

Go:   resp.StatusCode
来源：http://lgj.yongpay.top

Ruby: resp.code.to_i
来源：http://rfg.bbcook.cn

C#:   (int)resp.StatusCode
来源：http://olb.shanyushiyangkeji.top

[L08] 并发请求多个地址
来源：http://www.zycfv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hih.sufxvd.cn

PHP:  curl_multi_init() 系列
来源：http://hdu.yongpay.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iwi.gzhubu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zpy.hnxiangtu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yrr.fehbvm.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://loy.fanxiaobao.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://djk.xuanzx.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nbg.bjfxy.top

================================================================================
来源：http://pua.0kj1m.cn

M. 命令行 / 进程 / 环境
来源：http://yyt.meibo888.top

================================================================================
来源：http://kzx.jqgufenzy.top

[M01] 读取命令行参数
来源：http://jyn.316326.xyz

Py:   sys.argv[1:]
来源：http://fev.ydzc1.top

PHP:  $argv;  $argc;
来源：http://kyw.yuxming.cn

JS:   process.argv.slice(2)
来源：http://vwn.uphjek.com

TS:   process.argv.slice(2)
来源：http://izh.tanke756.top

Java: args 数组（main 方法参数）
来源：http://xmr.hammf.cn

Go:   os.Args[1:]
来源：http://gle.sjlbkw.cn

Ruby: ARGV
来源：http://edd.nanxinkj.top

C#:   args 数组（Main 方法参数）
来源：http://vrv.jinyuanbaomall.cn

[M02] 读取环境变量
来源：http://rbl.xinyue.icu

Py:   os.environ.get("HOME")
来源：http://jeh.316326.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yoj.andypj.xyz

JS:   process.env.HOME
来源：http://bwm.yj202588.top

TS:   process.env.HOME
来源：http://asr.birdmap.top

Java: System.getenv("HOME")
来源：http://msv.yj20258.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://odr.ivvv.top

Ruby: ENV["HOME"]
来源：http://auv.bjfxy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://arb.ydjk.org.cn

[M03] 执行外部命令
来源：http://hfa.xinyue.icu

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kzg.zhengqikj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lav.fzhhl.top

JS:   child_process.execSync("ls -l").toString()
来源：http://lxs.jinqigfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://akm.nanxuanxn.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tbx.fktsv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vka.snrcjt.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nfw.hfpthk.cn

C#:   Process.Start("ls", "-l");
来源：http://pzo.sufxvd.cn

[M04] 获取当前工作目录
来源：http://ztf.svipenyu.cn

Py:   os.getcwd()
来源：http://mdf.hongshengwenyu.top

PHP:  getcwd();
来源：http://zcb.fanxiaobao.xyz

JS:   process.cwd()
来源：http://fyp.cheryme.top

TS:   process.cwd()
来源：http://bzd.aibaodan.cn

Java: Path.of("").toAbsolutePath()
来源：http://vxm.shanyushiyangtech.top

Go:   os.Getwd()
来源：http://ypl.daxiang520.top

Ruby: Dir.pwd
来源：http://aba.nanxuanxn.top

C#:   Directory.GetCurrentDirectory()
来源：http://gwk.jinyuanbaomall.cn

[M05] 设置退出码
来源：http://bpb.zdbjq.cn

Py:   sys.exit(1)
来源：http://mgl.guannengcc.top

PHP:  exit(1);
来源：http://kqu.svipenyu.cn

JS:   process.exit(1)
来源：http://qof.hywenlv.cn

TS:   process.exit(1)
来源：http://tzd.aibaodan.cn

Java: System.exit(1)
来源：http://yat.316326.xyz

Go:   os.Exit(1)
来源：http://ina.havefunace.top

Ruby: exit 1
来源：http://awj.xylfe.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rhv.svipenyu.cn

[M06] 向标准错误输出
来源：http://hdg.gzhubu.top

Py:   print("err", file=sys.stderr)
来源：http://zmj.ivvv.top

PHP:  fwrite(STDERR, "err\n");
来源：http://zge.zdqjudy.top

JS:   console.error("err")
来源：http://juf.daria6918.cn

TS:   console.error("err")
来源：http://cjc.hywenlv.cn

Java: System.err.println("err")
来源：http://fyl.jinqigufen.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rel.yangfankeji.com

Ruby: warn "err"
来源：http://cea.bjfxy.top

C#:   Console.Error.WriteLine("err")
来源：http://tab.shangyingyoupin.top

[M07] 判断是否为主入口
来源：http://mhf.uphjek.com

Py:   if __name__ == "__main__":
来源：http://iap.cucudq.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kgy.yueranfly.top

JS:   require.main === module
来源：http://fvw.xinyue.icu

TS:   require.main === module
来源：http://bbz.tian-w.cn

Java: public static void main(String[] args)
来源：http://odb.feifeiyinyue.top

Go:   func main()
来源：http://smf.aibaodan.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cta.ybcxt.top

C#:   static void Main(string[] args)
来源：http://tnl.havefunace.top

[M08] 获取系统与运行时信息
来源：http://lzt.smart0.xyz

Py:   platform.system();  platform.python_version()
来源：http://pbm.bjfxy.top

PHP:  PHP_OS;  phpversion();
来源：http://toh.52xcode.cn

JS:   process.platform;  process.version
来源：http://spm.0kj1m.cn

TS:   process.platform;  process.version
来源：http://wml.meibo888.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mem.xuetiantiany.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://kic.hcnkem.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://aeg.ywan-chungtsiang.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://puz.smart0.xyz

================================================================================
来源：http://acd.zhiwuduotai.top

N. 数据结构与算法
来源：http://fpp.ehwqpu.com

================================================================================
来源：http://eca.sweek.top

[N01] 二分查找（有序数组）
来源：http://fdk.yueranfly.top

Py:   bisect.bisect_left(arr, x)
来源：http://kcw.cashguo.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tik.yuxming.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pef.hfpthk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zfi.zdqjudy.top

Java: Arrays.binarySearch(arr, x)
来源：http://wqm.iojbl.cn

Go:   sort.SearchInts(arr, x)
来源：http://bdw.hfpthk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qum.xingfuxueyuan.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://sxn.pycfn.com

[N02] 排序（工程实践用内置实现）
来源：http://hdv.andypj.xyz

Py:   sorted(arr);  arr.sort()
来源：http://xwo.shangyingyoupin.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pdl.xingfuxueyuan.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://dbn.hfpthk.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kyy.xziqi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xuz.daria6918.cn

Go:   slices.Sort(arr)
来源：http://lvu.andypj.xyz

Ruby: arr.sort
来源：http://xab.ctjpmb.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://ztp.cheryme.top

[N03] 快速排序（分治示例）
来源：http://aoy.xziqi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://quk.ydjk.org.cn

PHP:  // 递归实现，或用 usort
来源：http://ckr.xuetiantiany.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aek.quarkkingdee.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fsj.wangshuangyany.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vhe.zycfv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uuk.bbcook.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rjh.c1oappe.top

C#:   // 手写递归，或 Array.Sort
来源：http://muy.ydjk.org.cn

[N04] 斐波那契数列
来源：http://tlz.quarkkingdee.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tzz.sufxvd.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://oqa.hesvh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fro.cqqwz.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vof.gotoacloud.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://alg.meibo888.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wri.cheryme.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qwc.ywan-chungtsiang.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wip.yj202588.top

[N05] 最大公约数
来源：http://vlz.ppjwa.cn

Py:   math.gcd(a, b)
来源：http://zyv.smart0.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nzk.bjfxy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iax.jlsjyb.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oqx.yongpay.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://crf.jyoumei.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ijj.xingfuxueyuan.xyz

Ruby: a.gcd(b)
来源：http://usc.uphjek.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gkr.guannengcc.top

[N06] 判断回文字符串
来源：http://jct.nwbrower.top

Py:   s == s[::-1]
来源：http://lio.hnqzz.top

PHP:  $s === strrev($s);
来源：http://bye.sxryk.cn

JS:   s === [...s].reverse().join("")
来源：http://spp.yuanzhike.top

TS:   s === [...s].reverse().join("")
来源：http://xjq.316326.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xui.ybcxt.top

Go:   // 双指针从两端比较
来源：http://kua.andypj.xyz

Ruby: s == s.reverse
来源：http://jqv.havefunace.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://hjl.fzhhl.top

[N07] 两数之和（返回下标）
来源：http://nrn.snrcjt.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wsk.yonumen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rkz.zhijiandao.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://axe.wangdashe.top

TS:   // 手写 Map<string, number>
来源：http://eoh.zdbjq.cn

Java: // 手写 HashMap
来源：http://duh.snrcjt.cn

Go:   // 手写 map[int]int
来源：http://fxv.zycfv.cn

Ruby: // 手写 Hash
来源：http://let.wangshuangyany.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yom.zhongyouzk.top

[N08] 生成全排列
来源：http://rsi.ydjk.org.cn

Py:   itertools.permutations(arr)
来源：http://izz.sxryk.cn

PHP:  // 手写递归交换
来源：http://xfm.hnxiangtu.top

JS:   // 手写回溯递归
来源：http://hqs.bjfxy.top

TS:   // 手写回溯递归
来源：http://nxc.hongshengwenyu.top

Java: // 手写回溯递归
来源：http://lmo.snrcjt.cn

Go:   // 手写回溯递归
来源：http://ito.yj202588.top

Ruby: arr.permutation.to_a
来源：http://cus.fktsv.cn

C#:   // 手写回溯递归
来源：http://osi.cdnleiting.top

[N09] 栈与队列
来源：http://tkq.epnwcf.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hnu.quarkkingdee.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ixq.nwbrower.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wzf.hcnkem.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vpl.yanxiufei.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zfe.zhijiandao.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gjr.epnwcf.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nfr.cqqwz.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://iyk.vqdsnc.cn

[N10] 链表节点定义
来源：http://gcd.hcnkem.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vij.sysykeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://sjs.pengpengdd.cyou

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uth.havefunace.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dmn.haohaochexian.top

Java: class Node { int v; Node next; }
来源：http://ykb.ydjk.org.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tqv.cashguo.top

Ruby: Node = Struct.new(:v, :next)
来源：http://bxh.wangdashe.top

C#:   class Node { public int V; public Node? Next; }
来源：http://chk.fzhhl.top

[N11] 二叉树中序遍历
来源：http://ayl.zhaomingkeji.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dtd.cheryme.top

PHP:  // 手写递归函数
来源：http://lsr.quarkkingdee.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aqi.fzhhl.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aig.zhijiandao.cn

Java: // 手写递归
来源：http://nlv.shuidangran.top

Go:   // 手写递归
来源：http://osi.aizwys.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xzx.hammf.cn

C#:   // 手写递归
来源：http://gpn.zhixingplan.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tiv.hesvh.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pcz.yj20258.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lbd.shanyushiyangtech.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pjn.aibaodan.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gjb.feifeiyinyue.top


<!-- 参考信息 -->