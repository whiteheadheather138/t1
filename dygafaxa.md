代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://jbt.sxryk.cn

PHP:  unserialize(serialize($obj));
来源：http://ryl.birdmap.top

JS:   structuredClone(obj)
来源：http://umv.zhaomingkeji.xyz

TS:   structuredClone(obj)
来源：http://qps.xuetiantiany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kkb.hcnkem.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dyi.zycfv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bpn.shanyushiyangtech.top

C#:   // 序列化往返，或自定义 Clone
来源：http://igr.ppjwa.cn

[K06] 解析 URL 查询串
来源：http://adz.guannengcc.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yct.cucudq.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://woo.hfpthk.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mqg.sufxvd.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mhz.zhoulong.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mng.xziqi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://szj.xuetiantiany.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zbe.52xcode.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nlb.0kj1m.cn

[K07] 进制转换
来源：http://drr.cqqwz.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ffb.sweek.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jbx.chenjidiqi.icu

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yed.316326.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://otl.daxiang520.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://goh.pycfn.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fkn.yangfankeji.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cot.zhixingplan.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wjx.jinqigfzy.top

[K08] 二进制序列化（非 JSON）
来源：http://zkv.jlsjyb.cn

Py:   pickle.dumps(obj)
来源：http://adr.tian-w.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jvd.9152youxi.cn

JS:   v8.serialize(obj)        // Node
来源：http://kny.hnqzz.top

TS:   v8.serialize(obj)        // Node
来源：http://ghj.zycfv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fdp.fzhhl.top

Go:   encoding/gob
来源：http://xme.shanyushiyangtech.top

Ruby: Marshal.dump(obj)
来源：http://ucb.meibo888.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://aeb.yueranfly.top

================================================================================
来源：http://vaf.mhx1999.top

L. 网络请求
来源：http://vpj.aibaodan.cn

================================================================================
来源：http://xnj.ppjwa.cn

[L01] 发送 GET 请求
来源：http://qqi.pengpengdd.cyou

Py:   requests.get(url)                        # 第三方库 requests
来源：http://moe.redwolf501.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pyz.hcnkem.com

JS:   await fetch(url)
来源：http://cpm.mhx1999.top

TS:   await fetch(url)
来源：http://chi.gzhubu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vvf.0kj1m.cn

Go:   resp, err := http.Get(url)
来源：http://yqq.nanxinkj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ndw.jinyuanbaomall.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://iat.yuxming.cn

[L02] 发送 POST JSON
来源：http://gml.hfpthk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vyv.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cqr.tian-w.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ano.hnxiangtu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pwf.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rwi.gzhubu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jdx.hywenlv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gwy.pycfn.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tap.ivvv.top

[L03] 设置自定义请求头
来源：http://ntz.pycfn.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ecv.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fkd.guowangkeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gjf.ydzc1.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yhw.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hip.birdmap.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xbh.aizwys.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mgk.wangdashe.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://npz.fehbvm.com

[L04] 设置超时
来源：http://agr.xuanzx.com

Py:   requests.get(url, timeout=5)
来源：http://epu.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cmt.hnqzz.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sff.quarkkingdee.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kec.c1oappe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ydw.jinghuilouyu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vfd.kuanghao11.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qih.zhixingplan.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ovo.hywenlv.cn

[L05] 上传文件（multipart）
来源：http://zxy.zhongyouzk.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://btm.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wxf.wangdashe.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uxi.uphjek.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xuq.hnxiangtu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xhf.ctjpmb.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mnq.havefunace.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yzu.zhijiandao.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://agb.epnwcf.com

[L06] 解析响应为 JSON
来源：http://gyr.ybcxt.top

Py:   resp.json()
来源：http://qgv.hcnkem.com

PHP:  json_decode($body, true);
来源：http://osb.jinghuilouyu.cn

JS:   await resp.json()
来源：http://ovb.yj202588.top

TS:   await resp.json()
来源：http://vlj.daxiang520.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yei.pengpengdd.cyou

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pjx.zhoulong.xyz

Ruby: JSON.parse(resp.body)
来源：http://jvm.tian-w.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ybp.jqgufenzy.top

[L07] 处理 HTTP 状态码
来源：http://taf.xuetiantiany.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fah.jinqigufen.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kes.shzxlz.cn

JS:   resp.ok;  resp.status
来源：http://vgt.jqgfzy.top

TS:   resp.ok;  resp.status
来源：http://hbe.ywan-chungtsiang.top

Java: resp.statusCode()
来源：http://lzz.birdmap.top

Go:   resp.StatusCode
来源：http://oxr.fktsv.cn

Ruby: resp.code.to_i
来源：http://qbw.ehwqpu.com

C#:   (int)resp.StatusCode
来源：http://jta.9152youxi.cn

[L08] 并发请求多个地址
来源：http://ijl.kuanghao11.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vvm.fehbvm.com

PHP:  curl_multi_init() 系列
来源：http://exm.cucudq.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dwe.havefunace.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vgi.zdqjudy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cuy.dashuyun.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qme.zhiwuduotai.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tvd.andypj.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tsm.nwbrower.top

================================================================================
来源：http://ugh.ywan-chungtsiang.top

M. 命令行 / 进程 / 环境
来源：http://ian.feifeiyinyue.top

================================================================================
来源：http://uuw.chenlongwang.top

[M01] 读取命令行参数
来源：http://slc.snrcjt.cn

Py:   sys.argv[1:]
来源：http://dmn.dashuyun.cn

PHP:  $argv;  $argc;
来源：http://zfq.shuidangran.top

JS:   process.argv.slice(2)
来源：http://crv.fengsongda.top

TS:   process.argv.slice(2)
来源：http://ygj.haohaochexian.top

Java: args 数组（main 方法参数）
来源：http://kxo.wangdashe.top

Go:   os.Args[1:]
来源：http://fmc.hongshengwenyu.top

Ruby: ARGV
来源：http://xer.gaohongyu789.top

C#:   args 数组（Main 方法参数）
来源：http://prw.xuetiantiany.cn

[M02] 读取环境变量
来源：http://eia.iojbl.cn

Py:   os.environ.get("HOME")
来源：http://eqi.fengsongda.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zlx.zhijiandao.cn

JS:   process.env.HOME
来源：http://xki.zhengqikj.top

TS:   process.env.HOME
来源：http://gej.52xcode.cn

Java: System.getenv("HOME")
来源：http://zev.9152youxi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jsb.sysykeji.top

Ruby: ENV["HOME"]
来源：http://vav.sjlbkw.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://opb.wangshuangyany.cn

[M03] 执行外部命令
来源：http://ffm.cucudq.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tye.wangdashe.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://thr.yj202588.top

JS:   child_process.execSync("ls -l").toString()
来源：http://bgn.shanyushiyangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://tzm.birdmap.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://laj.tian-w.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fzi.nwbrower.top

Ruby: system("ls -l");  `ls -l`
来源：http://elb.quarkkingdee.top

C#:   Process.Start("ls", "-l");
来源：http://gbd.wangshuangyany.cn

[M04] 获取当前工作目录
来源：http://cgl.kuanghao11.cn

Py:   os.getcwd()
来源：http://spl.ybcxt.top

PHP:  getcwd();
来源：http://rcq.fzhhl.top

JS:   process.cwd()
来源：http://vaa.xinyue.icu

TS:   process.cwd()
来源：http://xyl.snrcjt.cn

Java: Path.of("").toAbsolutePath()
来源：http://cgx.shanyushiyangkeji.top

Go:   os.Getwd()
来源：http://cfm.jinyuanbaomall.cn

Ruby: Dir.pwd
来源：http://hvp.daxiang520.top

C#:   Directory.GetCurrentDirectory()
来源：http://exz.yj202588.top

[M05] 设置退出码
来源：http://dqa.hnxiangtu.top

Py:   sys.exit(1)
来源：http://awf.cucudq.cn

PHP:  exit(1);
来源：http://cel.guannengcc.top

JS:   process.exit(1)
来源：http://gsq.yuanzhike.top

TS:   process.exit(1)
来源：http://lbb.fktsv.cn

Java: System.exit(1)
来源：http://sfg.yonumen.top

Go:   os.Exit(1)
来源：http://euk.fzhhl.top

Ruby: exit 1
来源：http://eqb.svipenyu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xub.jlsjyb.cn

[M06] 向标准错误输出
来源：http://lzc.svipenyu.cn

Py:   print("err", file=sys.stderr)
来源：http://uds.guowangkeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://obh.aizwys.cn

JS:   console.error("err")
来源：http://fmf.zhengqikj.top

TS:   console.error("err")
来源：http://jne.chenjidiqi.icu

Java: System.err.println("err")
来源：http://zei.hammf.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://eor.smart0.xyz

Ruby: warn "err"
来源：http://azt.316326.xyz

C#:   Console.Error.WriteLine("err")
来源：http://eca.0kj1m.cn

[M07] 判断是否为主入口
来源：http://oct.tianlin.xyz

Py:   if __name__ == "__main__":
来源：http://ros.sysykeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://smu.zhiwuduotai.top

JS:   require.main === module
来源：http://cwt.zhoulong.xyz

TS:   require.main === module
来源：http://zhu.hnqzz.top

Java: public static void main(String[] args)
来源：http://tld.zhaomingkeji.xyz

Go:   func main()
来源：http://hvl.gzhubu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lsj.redwolf501.top

C#:   static void Main(string[] args)
来源：http://scx.jianghu66.top

[M08] 获取系统与运行时信息
来源：http://xhm.pycfn.com

Py:   platform.system();  platform.python_version()
来源：http://qvb.yj20258888.top

PHP:  PHP_OS;  phpversion();
来源：http://amk.jqgufenzy.top

JS:   process.platform;  process.version
来源：http://mny.tianlin.xyz

TS:   process.platform;  process.version
来源：http://roz.pycfn.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rky.yonumen.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://wkp.andypj.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dqa.xingfuxueyuan.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://maa.chenlongwang.top

================================================================================
来源：http://fky.zycfv.cn

N. 数据结构与算法
来源：http://vko.jqgufenzy.top

================================================================================
来源：http://awf.fanxiaobao.xyz

[N01] 二分查找（有序数组）
来源：http://cze.andypj.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://wvu.haohaochexian.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://iqj.haohaochexian.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ioc.zhongyouzk.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tel.hywenlv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mcg.yangfankeji.com

Go:   sort.SearchInts(arr, x)
来源：http://gsm.kuanghao11.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mvd.fengsongda.top

C#:   Array.BinarySearch(arr, x)
来源：http://ecv.guowangkeji.top

[N02] 排序（工程实践用内置实现）
来源：http://mbd.shzxlz.cn

Py:   sorted(arr);  arr.sort()
来源：http://fap.ydjk.org.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jws.ybcxt.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ihv.xingfuxueyuan.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://dph.xziqi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pdp.yuanzhike.top

Go:   slices.Sort(arr)
来源：http://alw.yueranfly.top

Ruby: arr.sort
来源：http://lex.svipenyu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://crb.xuanzx.com

[N03] 快速排序（分治示例）
来源：http://ubv.zdqjudy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xac.yangfankeji.com

PHP:  // 递归实现，或用 usort
来源：http://bsm.cheryme.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lls.zhixingplan.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yvp.shanyushiyangtech.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dou.yvedp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gms.birdmap.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bas.uphjek.com

C#:   // 手写递归，或 Array.Sort
来源：http://ixa.fzhhl.top

[N04] 斐波那契数列
来源：http://oyh.smart0.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uzb.yongpay.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dte.jiagoushi.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://glq.gaohongyu789.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://muh.fehbvm.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vys.xuetiantiany.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cgi.gaohongyu789.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kid.chenzaomai.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wgr.redwolf501.top

[N05] 最大公约数
来源：http://tqe.chenjidiqi.icu

Py:   math.gcd(a, b)
来源：http://nxl.yuanzhike.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gms.uphjek.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://meb.gogol.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hjl.yvedp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ahy.xuanzx.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tnj.chenzaomai.com

Ruby: a.gcd(b)
来源：http://kla.0kj1m.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://shq.yangfankeji.com

[N06] 判断回文字符串
来源：http://thv.nwbrower.top

Py:   s == s[::-1]
来源：http://cpg.fehbvm.com

PHP:  $s === strrev($s);
来源：http://jkh.fehbvm.com

JS:   s === [...s].reverse().join("")
来源：http://uec.yuxming.cn

TS:   s === [...s].reverse().join("")
来源：http://lot.cheryme.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qpf.fzhhl.top

Go:   // 双指针从两端比较
来源：http://num.wangshuangyany.cn

Ruby: s == s.reverse
来源：http://jom.wangdashe.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://qiv.sufxvd.cn

[N07] 两数之和（返回下标）
来源：http://gar.xylfe.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rex.gzhubu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://efl.shanyushiyangtech.top

JS:   // 手写 Map：map.set(v, i)
来源：http://aoq.zdbjq.cn

TS:   // 手写 Map<string, number>
来源：http://uka.yfazqb.com

Java: // 手写 HashMap
来源：http://unn.tianlin.xyz

Go:   // 手写 map[int]int
来源：http://goe.meibo888.top

Ruby: // 手写 Hash
来源：http://uwz.tian-w.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ahc.cqqwz.cn

[N08] 生成全排列
来源：http://ptp.fzhhl.top

Py:   itertools.permutations(arr)
来源：http://vob.hfpthk.cn

PHP:  // 手写递归交换
来源：http://znv.hesvh.cn

JS:   // 手写回溯递归
来源：http://qme.fehbvm.com

TS:   // 手写回溯递归
来源：http://vqw.zhixingplan.top

Java: // 手写回溯递归
来源：http://nyn.zdbjq.cn

Go:   // 手写回溯递归
来源：http://ygg.yj202588.top

Ruby: arr.permutation.to_a
来源：http://gil.birdmap.top

C#:   // 手写回溯递归
来源：http://fyz.xinyue.icu

[N09] 栈与队列
来源：http://qzj.tarul.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dyj.sxryk.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jpa.birdmap.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://htx.yanxiufei.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fmd.xingfuxueyuan.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tpc.yangfankeji.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qsm.nanxuanxn.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qma.yanxiufei.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jcx.cdnleiting.top

[N10] 链表节点定义
来源：http://czt.vehdjk.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vzt.hywenlv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wnj.hnqzz.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yzx.hfpthk.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gku.ctjpmb.com

Java: class Node { int v; Node next; }
来源：http://ujk.yj202588.top

Go:   type Node struct { V int; Next *Node }
来源：http://xwz.chenlongwang.top

Ruby: Node = Struct.new(:v, :next)
来源：http://iig.yangfankeji.com

C#:   class Node { public int V; public Node? Next; }
来源：http://rqv.daria6918.cn

[N11] 二叉树中序遍历
来源：http://igq.xinyue.icu

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qgv.zhijiandao.cn

PHP:  // 手写递归函数
来源：http://rqk.cashguo.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ppg.wangdashe.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://obx.yj20258.top

Java: // 手写递归
来源：http://aww.zhijiandao.cn

Go:   // 手写递归
来源：http://gdv.jqgufenzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vtk.dianchejie.cn

C#:   // 手写递归
来源：http://ltx.yonumen.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ann.svipenyu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gcj.sjlbkw.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gxu.pycfn.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://taz.jqgfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mlg.yvedp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gat.yanxiufei.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://roe.xziqi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jpz.andypj.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pvp.jyoumei.cn

================================================================================
来源：http://qex.havefunace.top

O. 并发与异步
来源：http://ulb.fehbvm.com

================================================================================
来源：http://bjd.aibaodan.cn

[O01] 启动一个线程
来源：http://tjb.gotoacloud.top


<!-- 参考信息 -->