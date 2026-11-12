代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://xna.316326.xyz

PHP:  unserialize(serialize($obj));
来源：http://efx.guannengcc.top

JS:   structuredClone(obj)
来源：http://fan.0kj1m.cn

TS:   structuredClone(obj)
来源：http://kqa.hcnkem.com

Java: // 手写拷贝构造，或序列化往返
来源：http://wob.ybcxt.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://znv.hcnkem.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hiw.chenlongwang.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ish.tanke756.top

[K06] 解析 URL 查询串
来源：http://fqh.xingfuxueyuan.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mam.sweek.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://krf.sufxvd.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uuw.mhx1999.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gos.gzhubu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://phg.feifeiyinyue.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://sat.jlsjyb.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hkp.jyoumei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://meg.cheryme.top

[K07] 进制转换
来源：http://cek.haohaochexian.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xet.hongshengwenyu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nav.hammf.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://brk.yj202588.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jed.fengsongda.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iay.52xcode.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bxq.chenjidiqi.icu

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dtb.chenzaomai.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ofn.ywan-chungtsiang.top

[K08] 二进制序列化（非 JSON）
来源：http://pdp.hammf.cn

Py:   pickle.dumps(obj)
来源：http://cck.uphjek.com

PHP:  serialize($obj);  unserialize($s);
来源：http://jdv.snrcjt.cn

JS:   v8.serialize(obj)        // Node
来源：http://cck.daria6918.cn

TS:   v8.serialize(obj)        // Node
来源：http://qng.aibaodan.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gep.zhiwuduotai.top

Go:   encoding/gob
来源：http://nzu.vehdjk.com

Ruby: Marshal.dump(obj)
来源：http://rnk.tarul.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qzp.hnxiangtu.top

================================================================================
来源：http://iol.shanyushiyangkeji.top

L. 网络请求
来源：http://fde.ybcxt.top

================================================================================
来源：http://dxj.yj20258.top

[L01] 发送 GET 请求
来源：http://ijc.yj20258.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uth.ydjk.org.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zww.yangfankeji.com

JS:   await fetch(url)
来源：http://ghm.yj20258.top

TS:   await fetch(url)
来源：http://xhm.guowangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://iow.hfpthk.cn

Go:   resp, err := http.Get(url)
来源：http://bgb.cqqwz.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tii.ywan-chungtsiang.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fjx.tian-w.cn

[L02] 发送 POST JSON
来源：http://eip.daxiang520.top

Py:   requests.post(url, json={"a": 1})
来源：http://bxs.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://exq.shanyushiyangtech.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cfu.shuidangran.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xnr.yanxiufei.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zep.xylfe.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tla.shangyingyoupin.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zrk.jqgufenzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lpl.smart0.xyz

[L03] 设置自定义请求头
来源：http://cjy.bjfxy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jxp.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xia.cdnleiting.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dwh.andypj.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lkf.yongpay.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jzi.zhijiandao.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lcj.nanxinkj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blr.chenjidiqi.icu

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qsk.fengsongda.top

[L04] 设置超时
来源：http://psv.cucudq.cn

Py:   requests.get(url, timeout=5)
来源：http://lnl.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://crd.tian-w.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dqr.fzhhl.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fli.pycfn.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://czs.wangdashe.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ivx.hywenlv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nda.zycfv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ejy.snrcjt.cn

[L05] 上传文件（multipart）
来源：http://tsl.tarul.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wqn.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ubp.sxryk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cbv.zhoulong.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cvy.fzhhl.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cmk.jlsjyb.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jzq.sysykeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rvb.chenzaomai.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pnm.sjlbkw.cn

[L06] 解析响应为 JSON
来源：http://dzf.sufxvd.cn

Py:   resp.json()
来源：http://wuy.wangdashe.top

PHP:  json_decode($body, true);
来源：http://bet.jlsjyb.cn

JS:   await resp.json()
来源：http://bdk.jinghuilouyu.cn

TS:   await resp.json()
来源：http://zhv.smart0.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iiv.shanyushiyangtech.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bbp.tian-w.cn

Ruby: JSON.parse(resp.body)
来源：http://smj.316326.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://epd.jlsjyb.cn

[L07] 处理 HTTP 状态码
来源：http://yzd.sxryk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://obh.chenlongwang.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rfx.hnqzz.top

JS:   resp.ok;  resp.status
来源：http://sgx.zhijiandao.cn

TS:   resp.ok;  resp.status
来源：http://ioz.dianchejie.cn

Java: resp.statusCode()
来源：http://cod.dianchejie.cn

Go:   resp.StatusCode
来源：http://wel.havefunace.top

Ruby: resp.code.to_i
来源：http://qhb.ivvv.top

C#:   (int)resp.StatusCode
来源：http://eyw.sysykeji.top

[L08] 并发请求多个地址
来源：http://xie.shanyushiyangkeji.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://agb.kuanghao11.cn

PHP:  curl_multi_init() 系列
来源：http://lpp.hongshengwenyu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kkj.kuanghao11.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://muh.sysykeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://laj.hywenlv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eqk.ywan-chungtsiang.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pbk.zycfv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dqd.xziqi.cn

================================================================================
来源：http://wxw.xinyue.icu

M. 命令行 / 进程 / 环境
来源：http://gym.bbcook.cn

================================================================================
来源：http://kdk.havefunace.top

[M01] 读取命令行参数
来源：http://efu.redwolf501.top

Py:   sys.argv[1:]
来源：http://rsc.shangyingyoupin.top

PHP:  $argv;  $argc;
来源：http://uql.xinyue.icu

JS:   process.argv.slice(2)
来源：http://sqm.nanxinkj.top

TS:   process.argv.slice(2)
来源：http://ljb.xingfuxueyuan.xyz

Java: args 数组（main 方法参数）
来源：http://aof.gaohongyu789.top

Go:   os.Args[1:]
来源：http://xdb.yongpay.top

Ruby: ARGV
来源：http://lxd.feifeiyinyue.top

C#:   args 数组（Main 方法参数）
来源：http://cww.feifeiyinyue.top

[M02] 读取环境变量
来源：http://swu.nwbrower.top

Py:   os.environ.get("HOME")
来源：http://mug.tanke756.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mku.chenjidiqi.icu

JS:   process.env.HOME
来源：http://naa.9152youxi.cn

TS:   process.env.HOME
来源：http://igg.fengsongda.top

Java: System.getenv("HOME")
来源：http://bnf.mhx1999.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hph.ybcxt.top

Ruby: ENV["HOME"]
来源：http://bpm.zycfv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sxr.sysykeji.top

[M03] 执行外部命令
来源：http://czw.meibo888.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ico.yvedp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://utu.yongpay.top

JS:   child_process.execSync("ls -l").toString()
来源：http://jmx.hcnkem.com

TS:   child_process.execSync("ls -l").toString()
来源：http://jxm.bbcook.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mhc.havefunace.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ivq.haohaochexian.top

Ruby: system("ls -l");  `ls -l`
来源：http://efp.vehdjk.com

C#:   Process.Start("ls", "-l");
来源：http://asn.ctjpmb.com

[M04] 获取当前工作目录
来源：http://ytb.ydjk.org.cn

Py:   os.getcwd()
来源：http://pln.zhoulong.xyz

PHP:  getcwd();
来源：http://hgk.daxiang520.top

JS:   process.cwd()
来源：http://zhn.hongshengwenyu.top

TS:   process.cwd()
来源：http://yov.zhongyouzk.top

Java: Path.of("").toAbsolutePath()
来源：http://fwy.jinyuanbaomall.cn

Go:   os.Getwd()
来源：http://vls.ctjpmb.com

Ruby: Dir.pwd
来源：http://tzm.xziqi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mrb.ehwqpu.com

[M05] 设置退出码
来源：http://ech.jyoumei.cn

Py:   sys.exit(1)
来源：http://khk.cheryme.top

PHP:  exit(1);
来源：http://mgd.zhiwuduotai.top

JS:   process.exit(1)
来源：http://qtg.meibo888.top

TS:   process.exit(1)
来源：http://wol.iojbl.cn

Java: System.exit(1)
来源：http://nli.ivvv.top

Go:   os.Exit(1)
来源：http://eao.jianghu66.top

Ruby: exit 1
来源：http://gto.ydzc1.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jpq.yuanzhike.top

[M06] 向标准错误输出
来源：http://brd.jiagoushi.top

Py:   print("err", file=sys.stderr)
来源：http://bwa.yj20258.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bsy.zhoulong.xyz

JS:   console.error("err")
来源：http://qgl.bjfxy.top

TS:   console.error("err")
来源：http://kcz.shanyushiyangtech.top

Java: System.err.println("err")
来源：http://zwk.ywan-chungtsiang.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://doy.hcnkem.com

Ruby: warn "err"
来源：http://dai.zdbjq.cn

C#:   Console.Error.WriteLine("err")
来源：http://jfw.shzxlz.cn

[M07] 判断是否为主入口
来源：http://mxw.52xcode.cn

Py:   if __name__ == "__main__":
来源：http://muu.52xcode.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vmj.iojbl.cn

JS:   require.main === module
来源：http://ntf.cqqwz.cn

TS:   require.main === module
来源：http://nea.tianlin.xyz

Java: public static void main(String[] args)
来源：http://wiw.fengsongda.top

Go:   func main()
来源：http://ums.svipenyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hgu.chenlongwang.top

C#:   static void Main(string[] args)
来源：http://qcy.iojbl.cn

[M08] 获取系统与运行时信息
来源：http://nwf.jianghu66.top

Py:   platform.system();  platform.python_version()
来源：http://hkm.cucudq.cn

PHP:  PHP_OS;  phpversion();
来源：http://agt.pycfn.com

JS:   process.platform;  process.version
来源：http://wms.ctjpmb.com

TS:   process.platform;  process.version
来源：http://hal.zhengqikj.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lhb.shanyushiyangtech.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ckk.gzhubu.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://psm.hnqzz.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://uqn.havefunace.top

================================================================================
来源：http://ipq.wangshuangyany.cn

N. 数据结构与算法
来源：http://fxs.birdmap.top

================================================================================
来源：http://yjs.vqdsnc.cn

[N01] 二分查找（有序数组）
来源：http://bss.c1oappe.top

Py:   bisect.bisect_left(arr, x)
来源：http://xks.snrcjt.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hyz.pengpengdd.cyou

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wdh.shanyushiyangkeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nsj.ivvv.top

Java: Arrays.binarySearch(arr, x)
来源：http://zml.yj20258.top

Go:   sort.SearchInts(arr, x)
来源：http://jtq.pycfn.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://ojy.316326.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://mbj.sjlbkw.cn

[N02] 排序（工程实践用内置实现）
来源：http://wgm.hysaishi.cn

Py:   sorted(arr);  arr.sort()
来源：http://zgf.iojbl.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ayn.ybcxt.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://tnk.guowangkeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://dmd.xziqi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://khl.jqgufenzy.top

Go:   slices.Sort(arr)
来源：http://rcr.9152youxi.cn

Ruby: arr.sort
来源：http://sdt.wangshuangyany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cnh.jianghu66.top

[N03] 快速排序（分治示例）
来源：http://grg.yfazqb.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rsg.shuidangran.top

PHP:  // 递归实现，或用 usort
来源：http://hoj.zhaomingkeji.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://stn.tian-w.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gfa.pycfn.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kpa.zhixingplan.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wly.xuanzx.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xkj.yuanzhike.top

C#:   // 手写递归，或 Array.Sort
来源：http://acg.yangfankeji.com

[N04] 斐波那契数列
来源：http://xxh.svipenyu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yhi.gogol.net.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ofh.ybcxt.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ztf.hcnkem.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pde.hnxiangtu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fxv.xziqi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hml.gogol.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uhs.sxryk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hiq.havefunace.top

[N05] 最大公约数
来源：http://bkh.hywenlv.cn

Py:   math.gcd(a, b)
来源：http://jzv.jinyuanbaomall.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vca.tarul.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ofb.zhixingplan.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aek.hammf.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xpg.hesvh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xgn.cashguo.top

Ruby: a.gcd(b)
来源：http://lbv.shuidangran.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xml.zhengqikj.top

[N06] 判断回文字符串
来源：http://tnp.fanxiaobao.xyz

Py:   s == s[::-1]
来源：http://gol.guowangkeji.top

PHP:  $s === strrev($s);
来源：http://rru.haohaochexian.top

JS:   s === [...s].reverse().join("")
来源：http://tnr.jiagoushi.top

TS:   s === [...s].reverse().join("")
来源：http://ylk.jinqigufen.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vzw.xinyue.icu

Go:   // 双指针从两端比较
来源：http://yev.sysykeji.top

Ruby: s == s.reverse
来源：http://nit.zhiwuduotai.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ojw.sweek.top

[N07] 两数之和（返回下标）
来源：http://tja.yj20258888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://piu.aizwys.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zyy.zdbjq.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pfz.jinqigfzy.top

TS:   // 手写 Map<string, number>
来源：http://pzp.zdbjq.cn

Java: // 手写 HashMap
来源：http://zfq.9152youxi.cn

Go:   // 手写 map[int]int
来源：http://rjk.9152youxi.cn

Ruby: // 手写 Hash
来源：http://fwf.zdbjq.cn

C#:   // 手写 Dictionary<int, int>
来源：http://eeq.yonumen.top

[N08] 生成全排列
来源：http://zfw.ydzc1.top

Py:   itertools.permutations(arr)
来源：http://rxa.zycfv.cn

PHP:  // 手写递归交换
来源：http://xtf.cashguo.top

JS:   // 手写回溯递归
来源：http://ass.aibaodan.cn

TS:   // 手写回溯递归
来源：http://ooj.zhongyouzk.top

Java: // 手写回溯递归
来源：http://ltf.316326.xyz

Go:   // 手写回溯递归
来源：http://xjq.xingfuxueyuan.xyz

Ruby: arr.permutation.to_a
来源：http://fan.tian-w.cn

C#:   // 手写回溯递归
来源：http://fox.snrcjt.cn

[N09] 栈与队列
来源：http://sjj.xuetiantiany.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nwq.havefunace.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pek.guowangkeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lrj.nanxinkj.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gyr.ybcxt.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gfr.gogol.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tbc.cucudq.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ogy.ivvv.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yaj.hfpthk.cn

[N10] 链表节点定义
来源：http://ipt.hysaishi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://quq.zdqjudy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://txg.hywenlv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yod.shzxlz.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://avk.pengpengdd.cyou

Java: class Node { int v; Node next; }
来源：http://faa.bbcook.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rjh.jianghu66.top

Ruby: Node = Struct.new(:v, :next)
来源：http://huq.jiagoushi.top

C#:   class Node { public int V; public Node? Next; }
来源：http://eel.cashguo.top

[N11] 二叉树中序遍历
来源：http://pev.ydjk.org.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ocu.zdbjq.cn

PHP:  // 手写递归函数
来源：http://gcj.redwolf501.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qlb.cqqwz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ivf.yongpay.top

Java: // 手写递归
来源：http://ots.sjlbkw.cn

Go:   // 手写递归
来源：http://eef.vehdjk.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nvy.vqdsnc.cn

C#:   // 手写递归
来源：http://jbl.yangfankeji.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uoc.xuanzx.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ccr.tian-w.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gas.iojbl.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ysp.yueranfly.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vrl.316326.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fbf.jqgfzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xqn.gotoacloud.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://epl.jinyuanbaomall.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qnl.haohaochexian.top

================================================================================
来源：http://syh.yj202588.top

O. 并发与异步
来源：http://vjn.cdnleiting.top

================================================================================
来源：http://oix.nwbrower.top

[O01] 启动一个线程
来源：http://iwm.yangfankeji.com


<!-- 参考信息 -->