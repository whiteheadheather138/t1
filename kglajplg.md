代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qro.iojbl.cn

[K07] 进制转换
来源：http://etc.zhongyouzk.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nqk.zhongyouzk.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://plx.xuetiantiany.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://apn.pycfn.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fkx.hcnkem.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rhh.redwolf501.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ysu.tanke756.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pzg.pycfn.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jbe.yongpay.top

[K08] 二进制序列化（非 JSON）
来源：http://ota.52xcode.cn

Py:   pickle.dumps(obj)
来源：http://epq.ydjk.org.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qbs.zhijiandao.cn

JS:   v8.serialize(obj)        // Node
来源：http://wwv.jinqigfzy.top

TS:   v8.serialize(obj)        // Node
来源：http://isp.ywan-chungtsiang.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ain.epnwcf.com

Go:   encoding/gob
来源：http://ajp.yanxiufei.cn

Ruby: Marshal.dump(obj)
来源：http://kau.316326.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lal.nwbrower.top

================================================================================
来源：http://iiq.hammf.cn

L. 网络请求
来源：http://rby.jqgufenzy.top

================================================================================
来源：http://nnx.zhaomingkeji.xyz

[L01] 发送 GET 请求
来源：http://pge.sufxvd.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://epg.dashuyun.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cco.jqgfzy.top

JS:   await fetch(url)
来源：http://vxb.gaohongyu789.top

TS:   await fetch(url)
来源：http://wjz.yj20258888.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://udo.ctjpmb.com

Go:   resp, err := http.Get(url)
来源：http://fac.dashuyun.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fnb.xinyue.icu

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gnu.fktsv.cn

[L02] 发送 POST JSON
来源：http://lxw.yj20258888.top

Py:   requests.post(url, json={"a": 1})
来源：http://tsi.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nzn.wangshuangyany.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yvd.cucudq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xpi.9152youxi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lcq.aibaodan.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xha.0kj1m.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zkk.cdnleiting.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qgz.cdnleiting.top

[L03] 设置自定义请求头
来源：http://jvh.iojbl.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sdo.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ngy.9152youxi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dxo.xinyue.icu

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tpz.nanxinkj.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://axj.yfazqb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tud.ydjk.org.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rwp.vehdjk.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jtq.yj202588.top

[L04] 设置超时
来源：http://otp.yanxiufei.cn

Py:   requests.get(url, timeout=5)
来源：http://ikl.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zfe.tarul.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rdu.jianghu66.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jeb.ctjpmb.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kmy.hnxiangtu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mch.ppjwa.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ier.aizwys.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xuz.zdbjq.cn

[L05] 上传文件（multipart）
来源：http://typ.hammf.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rkn.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nyy.guowangkeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://abm.tanke756.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://izw.jinghuilouyu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ywa.zhongyouzk.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wcs.xingfuxueyuan.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mgn.sysykeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://abc.wangdashe.top

[L06] 解析响应为 JSON
来源：http://rkv.shuidangran.top

Py:   resp.json()
来源：http://vgn.fzhhl.top

PHP:  json_decode($body, true);
来源：http://pok.wangdashe.top

JS:   await resp.json()
来源：http://wdi.meibo888.top

TS:   await resp.json()
来源：http://xau.yj202588.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oth.dianchejie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nzi.0kj1m.cn

Ruby: JSON.parse(resp.body)
来源：http://wby.jqgfzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ylc.jyoumei.cn

[L07] 处理 HTTP 状态码
来源：http://zrh.yueranfly.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://oin.epnwcf.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cio.shanyushiyangkeji.top

JS:   resp.ok;  resp.status
来源：http://tiu.xylfe.cn

TS:   resp.ok;  resp.status
来源：http://thq.jinqigfzy.top

Java: resp.statusCode()
来源：http://ext.gotoacloud.top

Go:   resp.StatusCode
来源：http://ivg.yuxming.cn

Ruby: resp.code.to_i
来源：http://kqg.ppjwa.cn

C#:   (int)resp.StatusCode
来源：http://tte.jiagoushi.top

[L08] 并发请求多个地址
来源：http://wis.shuidangran.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eqi.jyoumei.cn

PHP:  curl_multi_init() 系列
来源：http://buy.zdqjudy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://und.jyoumei.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rcc.ydzc1.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://obv.hysaishi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uxv.jqgufenzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://phf.shuidangran.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zpf.redwolf501.top

================================================================================
来源：http://thf.iojbl.cn

M. 命令行 / 进程 / 环境
来源：http://pxs.yuanzhike.top

================================================================================
来源：http://uru.xuetiantiany.cn

[M01] 读取命令行参数
来源：http://suj.zhongyouzk.top

Py:   sys.argv[1:]
来源：http://gbb.mhx1999.top

PHP:  $argv;  $argc;
来源：http://mos.0kj1m.cn

JS:   process.argv.slice(2)
来源：http://gyw.quarkkingdee.top

TS:   process.argv.slice(2)
来源：http://akl.iojbl.cn

Java: args 数组（main 方法参数）
来源：http://ayb.hywenlv.cn

Go:   os.Args[1:]
来源：http://nix.fengsongda.top

Ruby: ARGV
来源：http://xzo.yangfankeji.com

C#:   args 数组（Main 方法参数）
来源：http://yyf.wangshuangyany.cn

[M02] 读取环境变量
来源：http://jxw.shangyingyoupin.top

Py:   os.environ.get("HOME")
来源：http://urz.guannengcc.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hty.yfazqb.com

JS:   process.env.HOME
来源：http://qrf.andypj.xyz

TS:   process.env.HOME
来源：http://qda.jyoumei.cn

Java: System.getenv("HOME")
来源：http://lir.ctjpmb.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://elq.pengpengdd.cyou

Ruby: ENV["HOME"]
来源：http://qxz.chenzaomai.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dcw.52xcode.cn

[M03] 执行外部命令
来源：http://avr.svipenyu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uky.wangshuangyany.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gtj.9152youxi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bjp.0kj1m.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kpx.shuidangran.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uuo.fanxiaobao.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://kgm.yangfankeji.com

Ruby: system("ls -l");  `ls -l`
来源：http://txo.hongshengwenyu.top

C#:   Process.Start("ls", "-l");
来源：http://fit.guannengcc.top

[M04] 获取当前工作目录
来源：http://wwo.yj20258888.top

Py:   os.getcwd()
来源：http://jrd.yuanzhike.top

PHP:  getcwd();
来源：http://lzg.aizwys.cn

JS:   process.cwd()
来源：http://ied.havefunace.top

TS:   process.cwd()
来源：http://eqs.nanxinkj.top

Java: Path.of("").toAbsolutePath()
来源：http://yai.zhengqikj.top

Go:   os.Getwd()
来源：http://ycc.smart0.xyz

Ruby: Dir.pwd
来源：http://mxi.yuanzhike.top

C#:   Directory.GetCurrentDirectory()
来源：http://ngc.havefunace.top

[M05] 设置退出码
来源：http://ijq.tanke756.top

Py:   sys.exit(1)
来源：http://dym.fktsv.cn

PHP:  exit(1);
来源：http://oqt.snrcjt.cn

JS:   process.exit(1)
来源：http://qaq.dianchejie.cn

TS:   process.exit(1)
来源：http://qtc.yanxiufei.cn

Java: System.exit(1)
来源：http://utr.jqgufenzy.top

Go:   os.Exit(1)
来源：http://usu.fehbvm.com

Ruby: exit 1
来源：http://abm.svipenyu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cfr.gogol.net.cn

[M06] 向标准错误输出
来源：http://sgv.cashguo.top

Py:   print("err", file=sys.stderr)
来源：http://del.yuxming.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hot.hysaishi.cn

JS:   console.error("err")
来源：http://tjv.yj20258888.top

TS:   console.error("err")
来源：http://zca.zhiwuduotai.top

Java: System.err.println("err")
来源：http://lhg.yuanzhike.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rou.sxryk.cn

Ruby: warn "err"
来源：http://aet.jinghuilouyu.cn

C#:   Console.Error.WriteLine("err")
来源：http://gvc.nanxinkj.top

[M07] 判断是否为主入口
来源：http://kpi.hongshengwenyu.top

Py:   if __name__ == "__main__":
来源：http://wiv.fzhhl.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hmc.yj20258.top

JS:   require.main === module
来源：http://zkh.ywan-chungtsiang.top

TS:   require.main === module
来源：http://ooq.gotoacloud.top

Java: public static void main(String[] args)
来源：http://dmz.xziqi.cn

Go:   func main()
来源：http://zxm.cqqwz.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://idb.jqgufenzy.top

C#:   static void Main(string[] args)
来源：http://qhi.cheryme.top

[M08] 获取系统与运行时信息
来源：http://fio.nanxuanxn.top

Py:   platform.system();  platform.python_version()
来源：http://jyz.shanyushiyangtech.top

PHP:  PHP_OS;  phpversion();
来源：http://tdn.tian-w.cn

JS:   process.platform;  process.version
来源：http://acy.guowangkeji.top

TS:   process.platform;  process.version
来源：http://icu.vqdsnc.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xer.iojbl.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hgm.gaohongyu789.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://azi.quarkkingdee.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://vev.cashguo.top

================================================================================
来源：http://yza.0kj1m.cn

N. 数据结构与算法
来源：http://rmd.sjlbkw.cn

================================================================================
来源：http://yva.zhaomingkeji.xyz

[N01] 二分查找（有序数组）
来源：http://omh.yj20258888.top

Py:   bisect.bisect_left(arr, x)
来源：http://qaf.bbcook.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vrm.xuetiantiany.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://emp.jqgufenzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rqb.zhijiandao.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ihb.snrcjt.cn

Go:   sort.SearchInts(arr, x)
来源：http://nde.zhixingplan.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zne.nanxuanxn.top

C#:   Array.BinarySearch(arr, x)
来源：http://nbq.zhiwuduotai.top

[N02] 排序（工程实践用内置实现）
来源：http://fjh.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://ywa.guowangkeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jwi.aizwys.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pzm.zhaomingkeji.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://qmh.pengpengdd.cyou

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nvc.quarkkingdee.top

Go:   slices.Sort(arr)
来源：http://tqx.xinyue.icu

Ruby: arr.sort
来源：http://oyl.sxryk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://inl.wangdashe.top

[N03] 快速排序（分治示例）
来源：http://vgr.epnwcf.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sjg.sysykeji.top

PHP:  // 递归实现，或用 usort
来源：http://lpv.zhijiandao.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wxg.shuidangran.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hal.chenjidiqi.icu

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dia.nwbrower.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rcp.shanyushiyangtech.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qig.shzxlz.cn

C#:   // 手写递归，或 Array.Sort
来源：http://arq.ctjpmb.com

[N04] 斐波那契数列
来源：http://wwu.gaohongyu789.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rmg.yuxming.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tdv.pycfn.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gdq.jlsjyb.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lqi.aibaodan.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tnt.andypj.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jfa.yueranfly.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gij.quarkkingdee.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xxf.epnwcf.com

[N05] 最大公约数
来源：http://ikm.daria6918.cn

Py:   math.gcd(a, b)
来源：http://zpq.tianlin.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hhj.yangfankeji.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lgb.ehwqpu.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hxo.bjfxy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wgu.yj20258888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jvq.9152youxi.cn

Ruby: a.gcd(b)
来源：http://eii.ehwqpu.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hon.pycfn.com

[N06] 判断回文字符串
来源：http://eix.wangdashe.top

Py:   s == s[::-1]
来源：http://iub.yanxiufei.cn

PHP:  $s === strrev($s);
来源：http://zks.dashuyun.cn

JS:   s === [...s].reverse().join("")
来源：http://sfs.yfazqb.com

TS:   s === [...s].reverse().join("")
来源：http://kfg.meibo888.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dds.hnxiangtu.top

Go:   // 双指针从两端比较
来源：http://rnr.fzhhl.top

Ruby: s == s.reverse
来源：http://iez.hywenlv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://usp.epnwcf.com

[N07] 两数之和（返回下标）
来源：http://hna.vqdsnc.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jro.daria6918.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pto.havefunace.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mpq.jinghuilouyu.cn

TS:   // 手写 Map<string, number>
来源：http://zvs.316326.xyz

Java: // 手写 HashMap
来源：http://dby.cheryme.top

Go:   // 手写 map[int]int
来源：http://ste.hesvh.cn

Ruby: // 手写 Hash
来源：http://bok.ydzc1.top

C#:   // 手写 Dictionary<int, int>
来源：http://lci.zhiwuduotai.top

[N08] 生成全排列
来源：http://vxm.jianghu66.top

Py:   itertools.permutations(arr)
来源：http://grl.yueranfly.top

PHP:  // 手写递归交换
来源：http://mjp.zhijiandao.cn

JS:   // 手写回溯递归
来源：http://whw.ywan-chungtsiang.top

TS:   // 手写回溯递归
来源：http://iap.gaohongyu789.top

Java: // 手写回溯递归
来源：http://qzt.shanyushiyangtech.top

Go:   // 手写回溯递归
来源：http://lxt.zhixingplan.top

Ruby: arr.permutation.to_a
来源：http://gkv.hysaishi.cn

C#:   // 手写回溯递归
来源：http://ldn.jlsjyb.cn

[N09] 栈与队列
来源：http://asl.sweek.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://naa.shanyushiyangtech.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nej.zdbjq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qfw.hnxiangtu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jvt.xylfe.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qug.hfpthk.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://phc.guannengcc.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xcz.yuxming.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eut.jinghuilouyu.cn

[N10] 链表节点定义
来源：http://wii.jlsjyb.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uhg.nwbrower.top

PHP:  class Node { public $v; public $next = null; }
来源：http://lyv.birdmap.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kwn.dianchejie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zyu.bbcook.cn

Java: class Node { int v; Node next; }
来源：http://unl.bbcook.cn

Go:   type Node struct { V int; Next *Node }
来源：http://sqp.yueranfly.top

Ruby: Node = Struct.new(:v, :next)
来源：http://wcc.kuanghao11.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://dwq.quarkkingdee.top

[N11] 二叉树中序遍历
来源：http://hna.jinghuilouyu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://igb.sjlbkw.cn

PHP:  // 手写递归函数
来源：http://pgt.pengpengdd.cyou

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pnz.jinghuilouyu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bqa.jinqigufen.top

Java: // 手写递归
来源：http://jfi.kuanghao11.cn

Go:   // 手写递归
来源：http://zxj.wangdashe.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rhh.chenzaomai.com

C#:   // 手写递归
来源：http://dib.shzxlz.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cuq.tianlin.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xqc.chenlongwang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jdh.tian-w.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://elv.tian-w.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tpx.yj20258888.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ojs.ywan-chungtsiang.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kvh.gotoacloud.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wfk.yanxiufei.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fnw.snrcjt.cn

================================================================================
来源：http://qhn.iojbl.cn

O. 并发与异步
来源：http://exl.tarul.cn

================================================================================
来源：http://xkn.fanxiaobao.xyz

[O01] 启动一个线程
来源：http://qup.ivvv.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uvl.zhongyouzk.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yyr.jinghuilouyu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dku.gzhubu.top

TS:   // 同 JS
来源：http://vly.kuanghao11.cn

Java: new Thread(() -> f()).start()
来源：http://kpi.ydjk.org.cn

Go:   go f()
来源：http://rhr.smart0.xyz

Ruby: Thread.new { f }
来源：http://jpm.9152youxi.cn

C#:   Task.Run(() => F());
来源：http://zkt.snrcjt.cn

[O02] 使用线程池
来源：http://cyh.yonumen.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dfr.chenjidiqi.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xhv.zhixingplan.top

JS:   // worker_threads 线程池
来源：http://lcz.yuxming.cn

TS:   // worker_threads 线程池
来源：http://zkl.hcnkem.com

Java: Executors.newFixedThreadPool(4)
来源：http://xyf.zhoulong.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dyf.xinyue.icu

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tji.bjfxy.top


<!-- 参考信息 -->