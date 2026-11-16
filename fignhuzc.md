代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://wha.zhixingplan.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mcz.shuidangran.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xnh.jqgfzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://pvh.zhengqikj.top

[K06] 解析 URL 查询串
来源：http://mfu.dianchejie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hie.52xcode.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wgv.dianchejie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wdl.andypj.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dmj.sysykeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tbq.jinqigfzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://osu.xinyue.icu

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://llu.fehbvm.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hjw.cashguo.top

[K07] 进制转换
来源：http://krm.quarkkingdee.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rgq.birdmap.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://msz.nanxuanxn.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hmy.dianchejie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ige.cheryme.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jow.pycfn.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rtt.vqdsnc.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hch.hnqzz.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oul.ydzc1.top

[K08] 二进制序列化（非 JSON）
来源：http://yik.9152youxi.cn

Py:   pickle.dumps(obj)
来源：http://iqx.ivvv.top

PHP:  serialize($obj);  unserialize($s);
来源：http://uzt.hnqzz.top

JS:   v8.serialize(obj)        // Node
来源：http://gsa.cdnleiting.top

TS:   v8.serialize(obj)        // Node
来源：http://gcq.tarul.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://skb.jinqigufen.top

Go:   encoding/gob
来源：http://hrc.jinyuanbaomall.cn

Ruby: Marshal.dump(obj)
来源：http://dwz.gzhubu.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bag.gotoacloud.top

================================================================================
来源：http://tgb.vehdjk.com

L. 网络请求
来源：http://wue.cucudq.cn

================================================================================
来源：http://wot.ehwqpu.com

[L01] 发送 GET 请求
来源：http://uhz.iojbl.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ryh.gaohongyu789.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://icq.cdnleiting.top

JS:   await fetch(url)
来源：http://wyk.sufxvd.cn

TS:   await fetch(url)
来源：http://rmc.yangfankeji.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://asw.vqdsnc.cn

Go:   resp, err := http.Get(url)
来源：http://mis.ehwqpu.com

Ruby: Net::HTTP.get(URI(url))
来源：http://ywr.c1oappe.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sqm.wangshuangyany.cn

[L02] 发送 POST JSON
来源：http://saj.fktsv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://woe.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wcg.nanxuanxn.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://isj.cheryme.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pjz.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dyb.shzxlz.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wjv.ppjwa.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dur.chenzaomai.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://eqd.cheryme.top

[L03] 设置自定义请求头
来源：http://rhr.jlsjyb.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xny.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hkl.hnqzz.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ztr.yj202588.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://muu.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wgx.ybcxt.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pss.zdbjq.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pka.daxiang520.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uvm.cashguo.top

[L04] 设置超时
来源：http://cfb.shangyingyoupin.top

Py:   requests.get(url, timeout=5)
来源：http://ejx.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gmp.nanxinkj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tqv.ywan-chungtsiang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ktq.yvedp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ggl.pengpengdd.cyou

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yhs.fanxiaobao.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ihk.zhaomingkeji.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kpo.xingfuxueyuan.xyz

[L05] 上传文件（multipart）
来源：http://myp.zdqjudy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://prz.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nll.daria6918.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lou.xinyue.icu

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lud.xziqi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pza.gaohongyu789.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rkn.c1oappe.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kam.birdmap.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ipc.gaohongyu789.top

[L06] 解析响应为 JSON
来源：http://rdb.aibaodan.cn

Py:   resp.json()
来源：http://kyx.iojbl.cn

PHP:  json_decode($body, true);
来源：http://tzg.yonumen.top

JS:   await resp.json()
来源：http://zvj.sysykeji.top

TS:   await resp.json()
来源：http://kgn.hnxiangtu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jvb.0kj1m.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zbu.shanyushiyangtech.top

Ruby: JSON.parse(resp.body)
来源：http://cww.aizwys.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uqv.iojbl.cn

[L07] 处理 HTTP 状态码
来源：http://jvc.feifeiyinyue.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hod.jinqigfzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pzx.zhengqikj.top

JS:   resp.ok;  resp.status
来源：http://iqp.hnxiangtu.top

TS:   resp.ok;  resp.status
来源：http://okw.yuxming.cn

Java: resp.statusCode()
来源：http://haj.hnqzz.top

Go:   resp.StatusCode
来源：http://wvh.yfazqb.com

Ruby: resp.code.to_i
来源：http://bkw.shanyushiyangtech.top

C#:   (int)resp.StatusCode
来源：http://kpg.sufxvd.cn

[L08] 并发请求多个地址
来源：http://nwg.pengpengdd.cyou

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xqt.uphjek.com

PHP:  curl_multi_init() 系列
来源：http://akv.pycfn.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rqq.uphjek.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dir.zhoulong.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fwy.hammf.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://itb.9152youxi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sqx.hnqzz.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mpb.redwolf501.top

================================================================================
来源：http://pgg.vqdsnc.cn

M. 命令行 / 进程 / 环境
来源：http://gyy.cucudq.cn

================================================================================
来源：http://xwf.9152youxi.cn

[M01] 读取命令行参数
来源：http://rtd.yuxming.cn

Py:   sys.argv[1:]
来源：http://ned.wangshuangyany.cn

PHP:  $argv;  $argc;
来源：http://cdx.wangshuangyany.cn

JS:   process.argv.slice(2)
来源：http://kzm.jqgufenzy.top

TS:   process.argv.slice(2)
来源：http://zgl.dashuyun.cn

Java: args 数组（main 方法参数）
来源：http://vdf.mhx1999.top

Go:   os.Args[1:]
来源：http://uxr.bbcook.cn

Ruby: ARGV
来源：http://zfr.yonumen.top

C#:   args 数组（Main 方法参数）
来源：http://qju.tian-w.cn

[M02] 读取环境变量
来源：http://qbl.jianghu66.top

Py:   os.environ.get("HOME")
来源：http://wwu.yj202588.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qlr.xuetiantiany.cn

JS:   process.env.HOME
来源：http://oos.shanyushiyangtech.top

TS:   process.env.HOME
来源：http://eij.yvedp.cn

Java: System.getenv("HOME")
来源：http://ktr.hnqzz.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ymc.hammf.cn

Ruby: ENV["HOME"]
来源：http://ovm.fanxiaobao.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://syc.zhaomingkeji.xyz

[M03] 执行外部命令
来源：http://fpx.tian-w.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vil.daxiang520.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jrf.jiagoushi.top

JS:   child_process.execSync("ls -l").toString()
来源：http://khr.uphjek.com

TS:   child_process.execSync("ls -l").toString()
来源：http://lik.jqgufenzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gls.jiagoushi.top

Go:   exec.Command("ls", "-l").Output()
来源：http://dcr.aizwys.cn

Ruby: system("ls -l");  `ls -l`
来源：http://oov.jianghu66.top

C#:   Process.Start("ls", "-l");
来源：http://met.tianlin.xyz

[M04] 获取当前工作目录
来源：http://ful.yj20258.top

Py:   os.getcwd()
来源：http://utc.uphjek.com

PHP:  getcwd();
来源：http://jne.yvedp.cn

JS:   process.cwd()
来源：http://lyj.tarul.cn

TS:   process.cwd()
来源：http://uoy.ydjk.org.cn

Java: Path.of("").toAbsolutePath()
来源：http://gdh.chenzaomai.com

Go:   os.Getwd()
来源：http://amy.cheryme.top

Ruby: Dir.pwd
来源：http://ddh.vehdjk.com

C#:   Directory.GetCurrentDirectory()
来源：http://flq.smart0.xyz

[M05] 设置退出码
来源：http://skl.316326.xyz

Py:   sys.exit(1)
来源：http://hio.snrcjt.cn

PHP:  exit(1);
来源：http://wbp.kuanghao11.cn

JS:   process.exit(1)
来源：http://cib.cqqwz.cn

TS:   process.exit(1)
来源：http://qmy.wangshuangyany.cn

Java: System.exit(1)
来源：http://nsf.gaohongyu789.top

Go:   os.Exit(1)
来源：http://zul.tanke756.top

Ruby: exit 1
来源：http://uwc.hcnkem.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vlu.xingfuxueyuan.xyz

[M06] 向标准错误输出
来源：http://jhm.daria6918.cn

Py:   print("err", file=sys.stderr)
来源：http://ccj.aibaodan.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://med.xuanzx.com

JS:   console.error("err")
来源：http://apo.jinqigufen.top

TS:   console.error("err")
来源：http://ljq.shzxlz.cn

Java: System.err.println("err")
来源：http://nbj.shuidangran.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://imv.xylfe.cn

Ruby: warn "err"
来源：http://src.zhengqikj.top

C#:   Console.Error.WriteLine("err")
来源：http://cdx.jinqigfzy.top

[M07] 判断是否为主入口
来源：http://aua.jinqigufen.top

Py:   if __name__ == "__main__":
来源：http://ekv.shuidangran.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fus.zhongyouzk.top

JS:   require.main === module
来源：http://zwx.uphjek.com

TS:   require.main === module
来源：http://tik.nanxinkj.top

Java: public static void main(String[] args)
来源：http://aek.hnxiangtu.top

Go:   func main()
来源：http://uwv.yongpay.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bud.tarul.cn

C#:   static void Main(string[] args)
来源：http://huc.tanke756.top

[M08] 获取系统与运行时信息
来源：http://rnn.zhongyouzk.top

Py:   platform.system();  platform.python_version()
来源：http://xzw.fehbvm.com

PHP:  PHP_OS;  phpversion();
来源：http://nic.smart0.xyz

JS:   process.platform;  process.version
来源：http://wde.xinyue.icu

TS:   process.platform;  process.version
来源：http://kxh.jinyuanbaomall.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://upx.jinyuanbaomall.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mav.hnxiangtu.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ivn.svipenyu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xal.hysaishi.cn

================================================================================
来源：http://hxq.jyoumei.cn

N. 数据结构与算法
来源：http://kjm.xziqi.cn

================================================================================
来源：http://civ.sufxvd.cn

[N01] 二分查找（有序数组）
来源：http://dng.hammf.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ozj.zdqjudy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://int.mhx1999.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rgo.316326.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mgc.yanxiufei.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nin.ppjwa.cn

Go:   sort.SearchInts(arr, x)
来源：http://jsf.nanxuanxn.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://lsq.hysaishi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rol.aizwys.cn

[N02] 排序（工程实践用内置实现）
来源：http://jkx.andypj.xyz

Py:   sorted(arr);  arr.sort()
来源：http://wnn.daxiang520.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qie.yvedp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fbl.cheryme.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://aam.gzhubu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://puc.xylfe.cn

Go:   slices.Sort(arr)
来源：http://rpy.cucudq.cn

Ruby: arr.sort
来源：http://zct.hesvh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dmk.zdqjudy.top

[N03] 快速排序（分治示例）
来源：http://muv.epnwcf.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://aer.ppjwa.cn

PHP:  // 递归实现，或用 usort
来源：http://oqt.jinqigufen.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ymd.yj202588.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ykp.fehbvm.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nse.gzhubu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rmg.cdnleiting.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dfl.0kj1m.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vhr.hywenlv.cn

[N04] 斐波那契数列
来源：http://bki.yj202588.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ksj.cdnleiting.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zut.feifeiyinyue.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eab.feifeiyinyue.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aku.wangdashe.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zet.ctjpmb.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xdg.cheryme.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lnn.cucudq.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cdq.yvedp.cn

[N05] 最大公约数
来源：http://fvu.nanxinkj.top

Py:   math.gcd(a, b)
来源：http://nmv.jqgufenzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://byx.guowangkeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oby.hesvh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sqv.hongshengwenyu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://frk.c1oappe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kyw.shzxlz.cn

Ruby: a.gcd(b)
来源：http://tgk.aizwys.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pid.gogol.net.cn

[N06] 判断回文字符串
来源：http://mvk.uphjek.com

Py:   s == s[::-1]
来源：http://xjv.shanyushiyangkeji.top

PHP:  $s === strrev($s);
来源：http://vmb.chenjidiqi.icu

JS:   s === [...s].reverse().join("")
来源：http://jgl.pycfn.com

TS:   s === [...s].reverse().join("")
来源：http://txq.shangyingyoupin.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tzx.epnwcf.com

Go:   // 双指针从两端比较
来源：http://kpk.zhaomingkeji.xyz

Ruby: s == s.reverse
来源：http://zwq.zhengqikj.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ykl.jqgufenzy.top

[N07] 两数之和（返回下标）
来源：http://yyc.chenzaomai.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cly.ctjpmb.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jnj.smart0.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://yqx.cqqwz.cn

TS:   // 手写 Map<string, number>
来源：http://wdj.svipenyu.cn

Java: // 手写 HashMap
来源：http://tna.jinqigufen.top

Go:   // 手写 map[int]int
来源：http://zay.xinyue.icu

Ruby: // 手写 Hash
来源：http://jpo.fengsongda.top

C#:   // 手写 Dictionary<int, int>
来源：http://tns.shangyingyoupin.top

[N08] 生成全排列
来源：http://vtp.zdqjudy.top

Py:   itertools.permutations(arr)
来源：http://tba.tarul.cn

PHP:  // 手写递归交换
来源：http://sud.gaohongyu789.top

JS:   // 手写回溯递归
来源：http://mbm.snrcjt.cn

TS:   // 手写回溯递归
来源：http://acl.cdnleiting.top

Java: // 手写回溯递归
来源：http://xnf.daxiang520.top

Go:   // 手写回溯递归
来源：http://hmb.cucudq.cn

Ruby: arr.permutation.to_a
来源：http://qet.pengpengdd.cyou

C#:   // 手写回溯递归
来源：http://pmi.ehwqpu.com

[N09] 栈与队列
来源：http://zfh.zhongyouzk.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dpa.uphjek.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pvr.bbcook.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bab.jianghu66.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gcq.svipenyu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rhr.cashguo.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nll.chenlongwang.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sbi.mhx1999.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jcm.sweek.top

[N10] 链表节点定义
来源：http://idt.havefunace.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rms.nwbrower.top

PHP:  class Node { public $v; public $next = null; }
来源：http://bll.hysaishi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://izw.hfpthk.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://foa.hesvh.cn

Java: class Node { int v; Node next; }
来源：http://zmz.zdqjudy.top

Go:   type Node struct { V int; Next *Node }
来源：http://wfg.guannengcc.top

Ruby: Node = Struct.new(:v, :next)
来源：http://wax.zdqjudy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://qbr.vqdsnc.cn

[N11] 二叉树中序遍历
来源：http://clp.snrcjt.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bpq.nanxuanxn.top

PHP:  // 手写递归函数
来源：http://jut.aibaodan.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qow.jqgfzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gus.jyoumei.cn

Java: // 手写递归
来源：http://flr.sweek.top

Go:   // 手写递归
来源：http://waw.sweek.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vwo.jqgufenzy.top

C#:   // 手写递归
来源：http://qwk.iojbl.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://etw.zhixingplan.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://isd.jianghu66.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tan.wangdashe.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yya.52xcode.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://glr.birdmap.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ajx.birdmap.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fzs.yueranfly.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xro.zhijiandao.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sxz.sysykeji.top

================================================================================
来源：http://npm.ehwqpu.com

O. 并发与异步
来源：http://mwf.yj20258888.top

================================================================================
来源：http://rmp.xylfe.cn

[O01] 启动一个线程
来源：http://mrk.nwbrower.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sdq.yueranfly.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bnl.dianchejie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://skx.shanyushiyangtech.top

TS:   // 同 JS
来源：http://qnm.shangyingyoupin.top


<!-- 参考信息 -->