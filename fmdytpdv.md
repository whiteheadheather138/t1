代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://zgo.hongshengwenyu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tzh.zhiwuduotai.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hrs.sjlbkw.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://jje.ehwqpu.com

[K06] 解析 URL 查询串
来源：http://kai.dianchejie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dec.zhijiandao.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dql.pengpengdd.cyou

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qmo.zdqjudy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ovc.chenlongwang.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mzo.cucudq.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://att.svipenyu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ixn.smart0.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://whn.cashguo.top

[K07] 进制转换
来源：http://vid.ivvv.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cwj.zhiwuduotai.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qlc.fktsv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uzp.guannengcc.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mlh.zhongyouzk.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://avm.zdbjq.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xjl.bbcook.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vwi.jqgfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bmj.meibo888.top

[K08] 二进制序列化（非 JSON）
来源：http://xtt.epnwcf.com

Py:   pickle.dumps(obj)
来源：http://jvw.tian-w.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tnt.ywan-chungtsiang.top

JS:   v8.serialize(obj)        // Node
来源：http://msx.uphjek.com

TS:   v8.serialize(obj)        // Node
来源：http://rcu.yueranfly.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dut.feifeiyinyue.top

Go:   encoding/gob
来源：http://odv.yangfankeji.com

Ruby: Marshal.dump(obj)
来源：http://ues.0kj1m.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qzg.gzhubu.top

================================================================================
来源：http://jha.ydjk.org.cn

L. 网络请求
来源：http://xhj.yfazqb.com

================================================================================
来源：http://jnf.fktsv.cn

[L01] 发送 GET 请求
来源：http://wbu.shuidangran.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xle.zdbjq.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gvt.havefunace.top

JS:   await fetch(url)
来源：http://qfi.haohaochexian.top

TS:   await fetch(url)
来源：http://xar.birdmap.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://iqb.jinqigufen.top

Go:   resp, err := http.Get(url)
来源：http://vfg.hnxiangtu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://kyq.smart0.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jea.wangshuangyany.cn

[L02] 发送 POST JSON
来源：http://qml.daxiang520.top

Py:   requests.post(url, json={"a": 1})
来源：http://irj.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uhf.cashguo.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xzg.daria6918.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ofx.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://knn.hesvh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fvt.chenjidiqi.icu

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rfe.fanxiaobao.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hyl.snrcjt.cn

[L03] 设置自定义请求头
来源：http://sdr.ybcxt.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zfp.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gui.nwbrower.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zjy.chenlongwang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xof.sweek.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bwt.cucudq.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nql.bbcook.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wam.shuidangran.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tul.yanxiufei.cn

[L04] 设置超时
来源：http://jvg.haohaochexian.top

Py:   requests.get(url, timeout=5)
来源：http://tyt.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cah.ehwqpu.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tpf.hnxiangtu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lis.gotoacloud.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://smc.chenjidiqi.icu

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kax.zhijiandao.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yud.sjlbkw.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wqh.hywenlv.cn

[L05] 上传文件（multipart）
来源：http://zpa.zdqjudy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ptp.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lmu.ehwqpu.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lgf.hnxiangtu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gfb.shuidangran.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fdc.hesvh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wtm.316326.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hqo.hfpthk.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hhs.redwolf501.top

[L06] 解析响应为 JSON
来源：http://qpk.yuxming.cn

Py:   resp.json()
来源：http://zrs.guowangkeji.top

PHP:  json_decode($body, true);
来源：http://edi.zhongyouzk.top

JS:   await resp.json()
来源：http://itg.jinqigufen.top

TS:   await resp.json()
来源：http://ulv.daxiang520.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uau.bjfxy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tbt.xuanzx.com

Ruby: JSON.parse(resp.body)
来源：http://anw.gotoacloud.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jyz.xinyue.icu

[L07] 处理 HTTP 状态码
来源：http://wjy.fehbvm.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://loe.bjfxy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dyn.zhaomingkeji.xyz

JS:   resp.ok;  resp.status
来源：http://mpp.zdqjudy.top

TS:   resp.ok;  resp.status
来源：http://qxo.snrcjt.cn

Java: resp.statusCode()
来源：http://yuq.bjfxy.top

Go:   resp.StatusCode
来源：http://ugp.daria6918.cn

Ruby: resp.code.to_i
来源：http://zyu.cqqwz.cn

C#:   (int)resp.StatusCode
来源：http://hed.xuanzx.com

[L08] 并发请求多个地址
来源：http://ugy.pycfn.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://btm.jiagoushi.top

PHP:  curl_multi_init() 系列
来源：http://scl.ctjpmb.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://doq.jqgufenzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cll.jiagoushi.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ldv.jlsjyb.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hvp.zhaomingkeji.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gak.ctjpmb.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qam.bbcook.cn

================================================================================
来源：http://kdi.zhixingplan.top

M. 命令行 / 进程 / 环境
来源：http://gjl.jlsjyb.cn

================================================================================
来源：http://ggh.dashuyun.cn

[M01] 读取命令行参数
来源：http://kwc.cdnleiting.top

Py:   sys.argv[1:]
来源：http://fpt.tanke756.top

PHP:  $argv;  $argc;
来源：http://uow.hammf.cn

JS:   process.argv.slice(2)
来源：http://qhf.nwbrower.top

TS:   process.argv.slice(2)
来源：http://ubd.havefunace.top

Java: args 数组（main 方法参数）
来源：http://hih.smart0.xyz

Go:   os.Args[1:]
来源：http://upn.yj20258.top

Ruby: ARGV
来源：http://pbb.epnwcf.com

C#:   args 数组（Main 方法参数）
来源：http://zwk.ehwqpu.com

[M02] 读取环境变量
来源：http://why.hongshengwenyu.top

Py:   os.environ.get("HOME")
来源：http://ofs.yonumen.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hzy.haohaochexian.top

JS:   process.env.HOME
来源：http://nwv.jlsjyb.cn

TS:   process.env.HOME
来源：http://ayo.jyoumei.cn

Java: System.getenv("HOME")
来源：http://djg.redwolf501.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qeq.cheryme.top

Ruby: ENV["HOME"]
来源：http://ujl.zhaomingkeji.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pas.xylfe.cn

[M03] 执行外部命令
来源：http://cvg.sxryk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pyz.tanke756.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cga.daxiang520.top

JS:   child_process.execSync("ls -l").toString()
来源：http://fxf.jyoumei.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mey.zdqjudy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lwn.bbcook.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://knx.hcnkem.com

Ruby: system("ls -l");  `ls -l`
来源：http://rbg.smart0.xyz

C#:   Process.Start("ls", "-l");
来源：http://xur.guowangkeji.top

[M04] 获取当前工作目录
来源：http://ppn.hywenlv.cn

Py:   os.getcwd()
来源：http://nnm.gzhubu.top

PHP:  getcwd();
来源：http://yzj.tanke756.top

JS:   process.cwd()
来源：http://llq.mhx1999.top

TS:   process.cwd()
来源：http://jxa.xuanzx.com

Java: Path.of("").toAbsolutePath()
来源：http://vcx.smart0.xyz

Go:   os.Getwd()
来源：http://one.bjfxy.top

Ruby: Dir.pwd
来源：http://hqk.shanyushiyangkeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://lzn.sjlbkw.cn

[M05] 设置退出码
来源：http://zfk.aibaodan.cn

Py:   sys.exit(1)
来源：http://eku.aizwys.cn

PHP:  exit(1);
来源：http://cdr.shangyingyoupin.top

JS:   process.exit(1)
来源：http://sck.tarul.cn

TS:   process.exit(1)
来源：http://gwl.shanyushiyangkeji.top

Java: System.exit(1)
来源：http://ayh.bbcook.cn

Go:   os.Exit(1)
来源：http://dzt.zhongyouzk.top

Ruby: exit 1
来源：http://vmj.hcnkem.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uhf.fzhhl.top

[M06] 向标准错误输出
来源：http://nwi.svipenyu.cn

Py:   print("err", file=sys.stderr)
来源：http://ijf.redwolf501.top

PHP:  fwrite(STDERR, "err\n");
来源：http://aoc.havefunace.top

JS:   console.error("err")
来源：http://gcu.zycfv.cn

TS:   console.error("err")
来源：http://jdq.bjfxy.top

Java: System.err.println("err")
来源：http://vcp.hfpthk.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vvd.gzhubu.top

Ruby: warn "err"
来源：http://rcx.zycfv.cn

C#:   Console.Error.WriteLine("err")
来源：http://bap.tanke756.top

[M07] 判断是否为主入口
来源：http://npg.fehbvm.com

Py:   if __name__ == "__main__":
来源：http://jgu.uphjek.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dmu.zhaomingkeji.xyz

JS:   require.main === module
来源：http://ubb.meibo888.top

TS:   require.main === module
来源：http://gad.feifeiyinyue.top

Java: public static void main(String[] args)
来源：http://dbj.fktsv.cn

Go:   func main()
来源：http://jns.jinqigufen.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rzk.316326.xyz

C#:   static void Main(string[] args)
来源：http://pwc.yueranfly.top

[M08] 获取系统与运行时信息
来源：http://goj.cqqwz.cn

Py:   platform.system();  platform.python_version()
来源：http://wpq.hesvh.cn

PHP:  PHP_OS;  phpversion();
来源：http://xoc.shangyingyoupin.top

JS:   process.platform;  process.version
来源：http://sdv.shanyushiyangtech.top

TS:   process.platform;  process.version
来源：http://ike.redwolf501.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rlc.sxryk.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ikj.chenzaomai.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wfw.yuanzhike.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ero.vehdjk.com

================================================================================
来源：http://ptb.jqgfzy.top

N. 数据结构与算法
来源：http://ljh.guowangkeji.top

================================================================================
来源：http://yrv.kuanghao11.cn

[N01] 二分查找（有序数组）
来源：http://yge.yuxming.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mow.ehwqpu.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zkz.kuanghao11.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tef.pengpengdd.cyou

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sgf.yuxming.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qlh.jinghuilouyu.cn

Go:   sort.SearchInts(arr, x)
来源：http://hyj.cucudq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pcw.9152youxi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pev.hysaishi.cn

[N02] 排序（工程实践用内置实现）
来源：http://fbq.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://ypu.vqdsnc.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fsa.quarkkingdee.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://gfy.zdqjudy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vqb.shanyushiyangtech.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://muj.zycfv.cn

Go:   slices.Sort(arr)
来源：http://vel.gzhubu.top

Ruby: arr.sort
来源：http://qet.aizwys.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gwb.0kj1m.cn

[N03] 快速排序（分治示例）
来源：http://kvm.cheryme.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mrn.zdbjq.cn

PHP:  // 递归实现，或用 usort
来源：http://uhw.cheryme.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jaq.smart0.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://get.xinyue.icu

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mpc.yuanzhike.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://orb.meibo888.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qni.cucudq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://eol.chenlongwang.top

[N04] 斐波那契数列
来源：http://qse.ctjpmb.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ziy.fanxiaobao.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yyg.zhengqikj.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cxr.zhijiandao.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cgu.tarul.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rwy.chenjidiqi.icu

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wtp.nanxinkj.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ewv.jqgufenzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://whm.xylfe.cn

[N05] 最大公约数
来源：http://rad.dashuyun.cn

Py:   math.gcd(a, b)
来源：http://prc.ivvv.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yss.fengsongda.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uuo.birdmap.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bdo.cashguo.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://slm.daxiang520.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yag.hnxiangtu.top

Ruby: a.gcd(b)
来源：http://qlu.zhongyouzk.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tal.feifeiyinyue.top

[N06] 判断回文字符串
来源：http://wmp.ywan-chungtsiang.top

Py:   s == s[::-1]
来源：http://ncj.aizwys.cn

PHP:  $s === strrev($s);
来源：http://ate.cdnleiting.top

JS:   s === [...s].reverse().join("")
来源：http://skx.zdqjudy.top

TS:   s === [...s].reverse().join("")
来源：http://onb.cheryme.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xur.bbcook.cn

Go:   // 双指针从两端比较
来源：http://dzg.zhixingplan.top

Ruby: s == s.reverse
来源：http://npe.dianchejie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://htv.hywenlv.cn

[N07] 两数之和（返回下标）
来源：http://yru.tianlin.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qml.yongpay.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pux.jinyuanbaomall.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jcc.yj20258888.top

TS:   // 手写 Map<string, number>
来源：http://opj.vehdjk.com

Java: // 手写 HashMap
来源：http://xvu.shzxlz.cn

Go:   // 手写 map[int]int
来源：http://nxa.cucudq.cn

Ruby: // 手写 Hash
来源：http://qav.sysykeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://srp.zhongyouzk.top

[N08] 生成全排列
来源：http://dmf.hcnkem.com

Py:   itertools.permutations(arr)
来源：http://rrs.yanxiufei.cn

PHP:  // 手写递归交换
来源：http://fdx.cheryme.top

JS:   // 手写回溯递归
来源：http://iuc.yuanzhike.top

TS:   // 手写回溯递归
来源：http://qgd.feifeiyinyue.top

Java: // 手写回溯递归
来源：http://rle.aizwys.cn

Go:   // 手写回溯递归
来源：http://hoq.yuxming.cn

Ruby: arr.permutation.to_a
来源：http://wmz.hcnkem.com

C#:   // 手写回溯递归
来源：http://gad.ywan-chungtsiang.top

[N09] 栈与队列
来源：http://fkz.bjfxy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://iap.cheryme.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ymx.yj20258.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hru.xziqi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uqv.yj202588.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bdo.nanxinkj.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://osp.sxryk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zse.zhongyouzk.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hnq.daria6918.cn

[N10] 链表节点定义
来源：http://spr.ivvv.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://iwt.fanxiaobao.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://zan.jyoumei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://auk.bbcook.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://aad.jianghu66.top

Java: class Node { int v; Node next; }
来源：http://fzy.nanxuanxn.top

Go:   type Node struct { V int; Next *Node }
来源：http://tdl.cucudq.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bsi.zhixingplan.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bxj.daria6918.cn

[N11] 二叉树中序遍历
来源：http://flm.hcnkem.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zws.chenzaomai.com

PHP:  // 手写递归函数
来源：http://pok.xziqi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vvd.quarkkingdee.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jnr.zhongyouzk.top

Java: // 手写递归
来源：http://orr.tianlin.xyz

Go:   // 手写递归
来源：http://ska.hcnkem.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://syf.xuanzx.com

C#:   // 手写递归
来源：http://hna.c1oappe.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wuo.xziqi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kjk.xinyue.icu

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ibm.andypj.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://igh.hnxiangtu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pzy.jlsjyb.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hbq.sweek.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tpj.daria6918.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jqt.ybcxt.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://esu.nwbrower.top

================================================================================
来源：http://bts.bjfxy.top

O. 并发与异步
来源：http://hwb.fengsongda.top

================================================================================
来源：http://cqy.havefunace.top

[O01] 启动一个线程
来源：http://yku.yonumen.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kny.jinqigfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pds.yanxiufei.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sex.chenzaomai.com

TS:   // 同 JS
来源：http://bqk.ydzc1.top


<!-- 参考信息 -->