代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://gll.ctjpmb.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qgs.zdqjudy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rom.hysaishi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://uuv.chenlongwang.top

[K06] 解析 URL 查询串
来源：http://pjy.zhijiandao.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gjz.jiagoushi.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gpe.jinqigfzy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zfe.tanke756.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xae.yj202588.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sol.fzhhl.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://dwv.yfazqb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zxe.jqgufenzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bnx.hysaishi.cn

[K07] 进制转换
来源：http://rfc.bjfxy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mmm.vqdsnc.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://btq.yongpay.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://iiq.yj202588.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://msc.sweek.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dzi.havefunace.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yyv.ctjpmb.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nkh.dianchejie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lwf.zhijiandao.cn

[K08] 二进制序列化（非 JSON）
来源：http://nqn.birdmap.top

Py:   pickle.dumps(obj)
来源：http://dmb.shzxlz.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dzy.xuetiantiany.cn

JS:   v8.serialize(obj)        // Node
来源：http://arn.yj20258.top

TS:   v8.serialize(obj)        // Node
来源：http://cgp.ydzc1.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ugh.ywan-chungtsiang.top

Go:   encoding/gob
来源：http://rea.bjfxy.top

Ruby: Marshal.dump(obj)
来源：http://zyt.gotoacloud.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jqm.meibo888.top

================================================================================
来源：http://zag.mhx1999.top

L. 网络请求
来源：http://jeq.guowangkeji.top

================================================================================
来源：http://dqn.wangdashe.top

[L01] 发送 GET 请求
来源：http://euf.aizwys.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://psd.ehwqpu.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tnx.jqgfzy.top

JS:   await fetch(url)
来源：http://eib.chenjidiqi.icu

TS:   await fetch(url)
来源：http://vet.xingfuxueyuan.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fji.wangdashe.top

Go:   resp, err := http.Get(url)
来源：http://mcy.sysykeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://xyq.aizwys.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dnj.sysykeji.top

[L02] 发送 POST JSON
来源：http://fjk.shzxlz.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yjg.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rsc.yongpay.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ovl.c1oappe.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lyi.hcnkem.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://itw.fzhhl.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://inv.yvedp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lpw.sweek.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://odt.wangdashe.top

[L03] 设置自定义请求头
来源：http://prq.gaohongyu789.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ojf.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yyr.havefunace.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kkl.hcnkem.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hub.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kqh.fzhhl.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uug.sxryk.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qnw.ctjpmb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vcs.sufxvd.cn

[L04] 设置超时
来源：http://ddh.aizwys.cn

Py:   requests.get(url, timeout=5)
来源：http://nuo.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oek.yuanzhike.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gwd.xuanzx.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rmz.ppjwa.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fgu.yvedp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yvy.chenzaomai.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ibg.svipenyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bjn.zhaomingkeji.xyz

[L05] 上传文件（multipart）
来源：http://qfw.ehwqpu.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wwf.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vuc.feifeiyinyue.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pln.xylfe.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mdn.guannengcc.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lgd.hesvh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uby.cashguo.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fbf.yueranfly.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://skh.cdnleiting.top

[L06] 解析响应为 JSON
来源：http://brm.yj20258888.top

Py:   resp.json()
来源：http://yqw.nanxinkj.top

PHP:  json_decode($body, true);
来源：http://zor.cashguo.top

JS:   await resp.json()
来源：http://nhz.epnwcf.com

TS:   await resp.json()
来源：http://ntx.hywenlv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ffe.nanxuanxn.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hjb.sxryk.cn

Ruby: JSON.parse(resp.body)
来源：http://lct.wangshuangyany.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ekq.wangdashe.top

[L07] 处理 HTTP 状态码
来源：http://yxg.yvedp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kss.nanxuanxn.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nhe.andypj.xyz

JS:   resp.ok;  resp.status
来源：http://hti.yj202588.top

TS:   resp.ok;  resp.status
来源：http://uaj.zhijiandao.cn

Java: resp.statusCode()
来源：http://mci.yanxiufei.cn

Go:   resp.StatusCode
来源：http://wkx.uphjek.com

Ruby: resp.code.to_i
来源：http://fej.tarul.cn

C#:   (int)resp.StatusCode
来源：http://jqj.ywan-chungtsiang.top

[L08] 并发请求多个地址
来源：http://oao.aizwys.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hej.yueranfly.top

PHP:  curl_multi_init() 系列
来源：http://xpg.ctjpmb.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ezn.vqdsnc.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gjo.daxiang520.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mbc.yfazqb.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ucq.c1oappe.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bca.sweek.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jdc.hywenlv.cn

================================================================================
来源：http://hiv.smart0.xyz

M. 命令行 / 进程 / 环境
来源：http://num.hnxiangtu.top

================================================================================
来源：http://swa.meibo888.top

[M01] 读取命令行参数
来源：http://klb.gotoacloud.top

Py:   sys.argv[1:]
来源：http://sjm.hnxiangtu.top

PHP:  $argv;  $argc;
来源：http://kwq.xuanzx.com

JS:   process.argv.slice(2)
来源：http://nbz.yangfankeji.com

TS:   process.argv.slice(2)
来源：http://xbr.uphjek.com

Java: args 数组（main 方法参数）
来源：http://kiz.svipenyu.cn

Go:   os.Args[1:]
来源：http://qyg.iojbl.cn

Ruby: ARGV
来源：http://xij.ydzc1.top

C#:   args 数组（Main 方法参数）
来源：http://ltj.dashuyun.cn

[M02] 读取环境变量
来源：http://dvq.chenlongwang.top

Py:   os.environ.get("HOME")
来源：http://iqo.hnxiangtu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rxt.haohaochexian.top

JS:   process.env.HOME
来源：http://biy.yanxiufei.cn

TS:   process.env.HOME
来源：http://lif.shangyingyoupin.top

Java: System.getenv("HOME")
来源：http://ixl.zdqjudy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wqq.tarul.cn

Ruby: ENV["HOME"]
来源：http://lfd.pengpengdd.cyou

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pyc.c1oappe.top

[M03] 执行外部命令
来源：http://pmc.gzhubu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mub.jinqigfzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cov.ctjpmb.com

JS:   child_process.execSync("ls -l").toString()
来源：http://ngq.havefunace.top

TS:   child_process.execSync("ls -l").toString()
来源：http://kjd.yueranfly.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eri.yj20258888.top

Go:   exec.Command("ls", "-l").Output()
来源：http://voq.xylfe.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qeg.jinqigufen.top

C#:   Process.Start("ls", "-l");
来源：http://xeq.xuetiantiany.cn

[M04] 获取当前工作目录
来源：http://rtu.wangshuangyany.cn

Py:   os.getcwd()
来源：http://moh.andypj.xyz

PHP:  getcwd();
来源：http://blj.hywenlv.cn

JS:   process.cwd()
来源：http://avm.xuetiantiany.cn

TS:   process.cwd()
来源：http://gdu.hammf.cn

Java: Path.of("").toAbsolutePath()
来源：http://kmi.iojbl.cn

Go:   os.Getwd()
来源：http://jsd.uphjek.com

Ruby: Dir.pwd
来源：http://bsp.sufxvd.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ujk.yueranfly.top

[M05] 设置退出码
来源：http://fgn.yuxming.cn

Py:   sys.exit(1)
来源：http://sjg.chenlongwang.top

PHP:  exit(1);
来源：http://xtx.zhoulong.xyz

JS:   process.exit(1)
来源：http://pra.yangfankeji.com

TS:   process.exit(1)
来源：http://oyk.snrcjt.cn

Java: System.exit(1)
来源：http://ttj.wangdashe.top

Go:   os.Exit(1)
来源：http://dqo.guannengcc.top

Ruby: exit 1
来源：http://vbv.vehdjk.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://otg.jinghuilouyu.cn

[M06] 向标准错误输出
来源：http://wni.uphjek.com

Py:   print("err", file=sys.stderr)
来源：http://kbd.andypj.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://mse.mhx1999.top

JS:   console.error("err")
来源：http://dhg.fanxiaobao.xyz

TS:   console.error("err")
来源：http://nwy.shuidangran.top

Java: System.err.println("err")
来源：http://vdt.zhongyouzk.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://knh.shangyingyoupin.top

Ruby: warn "err"
来源：http://olh.yuxming.cn

C#:   Console.Error.WriteLine("err")
来源：http://fue.wangdashe.top

[M07] 判断是否为主入口
来源：http://hth.ctjpmb.com

Py:   if __name__ == "__main__":
来源：http://dls.redwolf501.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zsf.yfazqb.com

JS:   require.main === module
来源：http://vzs.xziqi.cn

TS:   require.main === module
来源：http://ppe.hongshengwenyu.top

Java: public static void main(String[] args)
来源：http://ofm.zdbjq.cn

Go:   func main()
来源：http://nnm.ydjk.org.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fxz.cdnleiting.top

C#:   static void Main(string[] args)
来源：http://zry.c1oappe.top

[M08] 获取系统与运行时信息
来源：http://inc.snrcjt.cn

Py:   platform.system();  platform.python_version()
来源：http://gjs.daria6918.cn

PHP:  PHP_OS;  phpversion();
来源：http://ubz.snrcjt.cn

JS:   process.platform;  process.version
来源：http://yyn.cheryme.top

TS:   process.platform;  process.version
来源：http://xvb.iojbl.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kfl.haohaochexian.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xyj.shangyingyoupin.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xlc.tanke756.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hdc.hammf.cn

================================================================================
来源：http://yrw.pengpengdd.cyou

N. 数据结构与算法
来源：http://fzt.jinghuilouyu.cn

================================================================================
来源：http://nju.jyoumei.cn

[N01] 二分查找（有序数组）
来源：http://isk.kuanghao11.cn

Py:   bisect.bisect_left(arr, x)
来源：http://asq.ehwqpu.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rag.yuxming.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mho.hongshengwenyu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eml.ctjpmb.com

Java: Arrays.binarySearch(arr, x)
来源：http://jgf.sxryk.cn

Go:   sort.SearchInts(arr, x)
来源：http://fnn.chenzaomai.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://nyf.hammf.cn

C#:   Array.BinarySearch(arr, x)
来源：http://liq.yangfankeji.com

[N02] 排序（工程实践用内置实现）
来源：http://qht.jianghu66.top

Py:   sorted(arr);  arr.sort()
来源：http://qdq.uphjek.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nec.zycfv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zmq.cdnleiting.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://hqc.yj20258888.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fck.ybcxt.top

Go:   slices.Sort(arr)
来源：http://jkk.cqqwz.cn

Ruby: arr.sort
来源：http://lfr.fktsv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ekw.52xcode.cn

[N03] 快速排序（分治示例）
来源：http://jql.jiagoushi.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zcq.snrcjt.cn

PHP:  // 递归实现，或用 usort
来源：http://eby.nanxuanxn.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iub.tanke756.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hxt.xingfuxueyuan.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tqx.sysykeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://clc.xinyue.icu

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://van.yueranfly.top

C#:   // 手写递归，或 Array.Sort
来源：http://nyn.dashuyun.cn

[N04] 斐波那契数列
来源：http://bxf.yongpay.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tgu.bbcook.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lwn.hnxiangtu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lkb.hammf.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tns.jinyuanbaomall.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rrb.nwbrower.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tfo.redwolf501.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nms.cqqwz.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nsd.hongshengwenyu.top

[N05] 最大公约数
来源：http://fip.haohaochexian.top

Py:   math.gcd(a, b)
来源：http://ofa.guowangkeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uyg.yangfankeji.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dzz.havefunace.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://egc.xziqi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hkl.birdmap.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dso.hywenlv.cn

Ruby: a.gcd(b)
来源：http://rzk.redwolf501.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rwo.yongpay.top

[N06] 判断回文字符串
来源：http://otv.jlsjyb.cn

Py:   s == s[::-1]
来源：http://hmr.andypj.xyz

PHP:  $s === strrev($s);
来源：http://dbe.316326.xyz

JS:   s === [...s].reverse().join("")
来源：http://kax.hammf.cn

TS:   s === [...s].reverse().join("")
来源：http://cef.dianchejie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gzt.cashguo.top

Go:   // 双指针从两端比较
来源：http://tyu.zhongyouzk.top

Ruby: s == s.reverse
来源：http://jxb.zdbjq.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xsy.jinqigfzy.top

[N07] 两数之和（返回下标）
来源：http://env.sjlbkw.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nla.vqdsnc.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tam.epnwcf.com

JS:   // 手写 Map：map.set(v, i)
来源：http://cnv.shzxlz.cn

TS:   // 手写 Map<string, number>
来源：http://hel.jinghuilouyu.cn

Java: // 手写 HashMap
来源：http://vhp.dashuyun.cn

Go:   // 手写 map[int]int
来源：http://hgj.316326.xyz

Ruby: // 手写 Hash
来源：http://lig.smart0.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://fbf.zhixingplan.top

[N08] 生成全排列
来源：http://tvq.zhiwuduotai.top

Py:   itertools.permutations(arr)
来源：http://rhs.tianlin.xyz

PHP:  // 手写递归交换
来源：http://rmm.yj202588.top

JS:   // 手写回溯递归
来源：http://sdc.dianchejie.cn

TS:   // 手写回溯递归
来源：http://vnx.fzhhl.top

Java: // 手写回溯递归
来源：http://fye.ywan-chungtsiang.top

Go:   // 手写回溯递归
来源：http://gxg.wangdashe.top

Ruby: arr.permutation.to_a
来源：http://nre.svipenyu.cn

C#:   // 手写回溯递归
来源：http://pmv.wangshuangyany.cn

[N09] 栈与队列
来源：http://fnl.jiagoushi.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vqs.feifeiyinyue.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rzb.zhongyouzk.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uma.epnwcf.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ixc.jyoumei.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wtq.yfazqb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://srq.zycfv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rdy.hnxiangtu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uyr.iojbl.cn

[N10] 链表节点定义
来源：http://tdj.yj20258.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qio.uphjek.com

PHP:  class Node { public $v; public $next = null; }
来源：http://agv.yueranfly.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://igs.xuetiantiany.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ttx.sjlbkw.cn

Java: class Node { int v; Node next; }
来源：http://xsp.yj202588.top

Go:   type Node struct { V int; Next *Node }
来源：http://rvz.yj20258.top

Ruby: Node = Struct.new(:v, :next)
来源：http://dql.hfpthk.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://noa.cqqwz.cn

[N11] 二叉树中序遍历
来源：http://fng.ywan-chungtsiang.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://egx.chenzaomai.com

PHP:  // 手写递归函数
来源：http://hsp.ybcxt.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://njl.cqqwz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kyn.fengsongda.top

Java: // 手写递归
来源：http://ync.sweek.top

Go:   // 手写递归
来源：http://zwi.chenzaomai.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://owv.bjfxy.top

C#:   // 手写递归
来源：http://cuz.quarkkingdee.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sio.jqgfzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://khf.andypj.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yzt.fehbvm.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wtq.zycfv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fbl.ybcxt.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://utl.yueranfly.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hpo.52xcode.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wqa.52xcode.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wrw.yj20258.top

================================================================================
来源：http://bto.jiagoushi.top

O. 并发与异步
来源：http://jxi.ydzc1.top

================================================================================
来源：http://ncb.xuanzx.com

[O01] 启动一个线程
来源：http://fdt.zhaomingkeji.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ltg.hnxiangtu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mkd.shangyingyoupin.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://aay.dianchejie.cn

TS:   // 同 JS
来源：http://aqt.xinyue.icu


<!-- 参考信息 -->