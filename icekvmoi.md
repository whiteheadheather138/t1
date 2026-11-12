代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bnn.zycfv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tpd.aizwys.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://anj.fanxiaobao.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://euw.sufxvd.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yha.0kj1m.cn

[K07] 进制转换
来源：http://wox.shuidangran.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lns.fktsv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ssn.haohaochexian.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qyv.0kj1m.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wat.svipenyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kju.xziqi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://aeb.cdnleiting.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cll.haohaochexian.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xnn.gaohongyu789.top

[K08] 二进制序列化（非 JSON）
来源：http://zkb.chenlongwang.top

Py:   pickle.dumps(obj)
来源：http://ouj.shzxlz.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nfv.jinqigfzy.top

JS:   v8.serialize(obj)        // Node
来源：http://kgq.ydzc1.top

TS:   v8.serialize(obj)        // Node
来源：http://vez.guowangkeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cst.yanxiufei.cn

Go:   encoding/gob
来源：http://kuz.cdnleiting.top

Ruby: Marshal.dump(obj)
来源：http://pnl.dashuyun.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gnh.gaohongyu789.top

================================================================================
来源：http://ssg.316326.xyz

L. 网络请求
来源：http://xwt.52xcode.cn

================================================================================
来源：http://cah.aibaodan.cn

[L01] 发送 GET 请求
来源：http://bnp.sweek.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tqj.0kj1m.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xzq.andypj.xyz

JS:   await fetch(url)
来源：http://usg.pycfn.com

TS:   await fetch(url)
来源：http://kik.yanxiufei.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xse.pengpengdd.cyou

Go:   resp, err := http.Get(url)
来源：http://sxj.hywenlv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zyr.gotoacloud.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nnq.feifeiyinyue.top

[L02] 发送 POST JSON
来源：http://vjd.pycfn.com

Py:   requests.post(url, json={"a": 1})
来源：http://jix.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iez.wangshuangyany.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dhu.jqgfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vyq.daxiang520.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tcw.zhoulong.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vli.svipenyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://efm.mhx1999.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ylp.jlsjyb.cn

[L03] 设置自定义请求头
来源：http://nri.wangshuangyany.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://csz.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://noi.yonumen.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zlo.pengpengdd.cyou

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tfk.zycfv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tdu.nwbrower.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ylr.yuanzhike.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zzk.9152youxi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gvm.yanxiufei.cn

[L04] 设置超时
来源：http://nnc.zhaomingkeji.xyz

Py:   requests.get(url, timeout=5)
来源：http://ixe.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lld.feifeiyinyue.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jhw.jqgufenzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qsl.bbcook.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qse.shanyushiyangtech.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ezt.xuetiantiany.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pgp.shanyushiyangtech.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yth.fengsongda.top

[L05] 上传文件（multipart）
来源：http://sgt.snrcjt.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lyq.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pop.jqgufenzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xec.jinqigfzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cjd.jqgfzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gbu.aibaodan.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xbs.cucudq.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eeq.feifeiyinyue.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oea.0kj1m.cn

[L06] 解析响应为 JSON
来源：http://esp.yuxming.cn

Py:   resp.json()
来源：http://quh.chenzaomai.com

PHP:  json_decode($body, true);
来源：http://gcw.hnqzz.top

JS:   await resp.json()
来源：http://xpi.ydjk.org.cn

TS:   await resp.json()
来源：http://sxs.yfazqb.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lui.jqgfzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wui.hammf.cn

Ruby: JSON.parse(resp.body)
来源：http://coq.9152youxi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dgt.tian-w.cn

[L07] 处理 HTTP 状态码
来源：http://xuc.guannengcc.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pco.xingfuxueyuan.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gtl.dashuyun.cn

JS:   resp.ok;  resp.status
来源：http://yfz.zhijiandao.cn

TS:   resp.ok;  resp.status
来源：http://wjn.jinghuilouyu.cn

Java: resp.statusCode()
来源：http://tqa.xuanzx.com

Go:   resp.StatusCode
来源：http://aun.sweek.top

Ruby: resp.code.to_i
来源：http://yfi.hammf.cn

C#:   (int)resp.StatusCode
来源：http://xox.sweek.top

[L08] 并发请求多个地址
来源：http://fej.hcnkem.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pgm.sysykeji.top

PHP:  curl_multi_init() 系列
来源：http://bts.ydjk.org.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fpi.ydjk.org.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://amt.feifeiyinyue.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ttu.yvedp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qit.meibo888.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tji.daria6918.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jdu.yongpay.top

================================================================================
来源：http://kii.jlsjyb.cn

M. 命令行 / 进程 / 环境
来源：http://gnf.hesvh.cn

================================================================================
来源：http://ndx.epnwcf.com

[M01] 读取命令行参数
来源：http://bsp.nanxuanxn.top

Py:   sys.argv[1:]
来源：http://ydb.xingfuxueyuan.xyz

PHP:  $argv;  $argc;
来源：http://fzx.zhijiandao.cn

JS:   process.argv.slice(2)
来源：http://asd.vehdjk.com

TS:   process.argv.slice(2)
来源：http://giu.jqgfzy.top

Java: args 数组（main 方法参数）
来源：http://hvv.wangdashe.top

Go:   os.Args[1:]
来源：http://ipk.sjlbkw.cn

Ruby: ARGV
来源：http://lce.gaohongyu789.top

C#:   args 数组（Main 方法参数）
来源：http://yui.tanke756.top

[M02] 读取环境变量
来源：http://plt.hesvh.cn

Py:   os.environ.get("HOME")
来源：http://ogh.cucudq.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://epo.sufxvd.cn

JS:   process.env.HOME
来源：http://zde.tarul.cn

TS:   process.env.HOME
来源：http://fwr.yongpay.top

Java: System.getenv("HOME")
来源：http://mti.tarul.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fqx.feifeiyinyue.top

Ruby: ENV["HOME"]
来源：http://btk.yonumen.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jof.vqdsnc.cn

[M03] 执行外部命令
来源：http://tcq.ydzc1.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zzb.vehdjk.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uem.yuanzhike.top

JS:   child_process.execSync("ls -l").toString()
来源：http://tjf.yanxiufei.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ozi.jinyuanbaomall.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xod.zhongyouzk.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jrw.ydjk.org.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ohb.yj20258888.top

C#:   Process.Start("ls", "-l");
来源：http://obj.tanke756.top

[M04] 获取当前工作目录
来源：http://vms.tarul.cn

Py:   os.getcwd()
来源：http://lce.yangfankeji.com

PHP:  getcwd();
来源：http://vya.meibo888.top

JS:   process.cwd()
来源：http://vvx.bjfxy.top

TS:   process.cwd()
来源：http://crr.pycfn.com

Java: Path.of("").toAbsolutePath()
来源：http://nfm.epnwcf.com

Go:   os.Getwd()
来源：http://xnr.daxiang520.top

Ruby: Dir.pwd
来源：http://xxn.yfazqb.com

C#:   Directory.GetCurrentDirectory()
来源：http://yrd.shangyingyoupin.top

[M05] 设置退出码
来源：http://aea.bbcook.cn

Py:   sys.exit(1)
来源：http://wqk.xinyue.icu

PHP:  exit(1);
来源：http://vts.shuidangran.top

JS:   process.exit(1)
来源：http://qpg.xingfuxueyuan.xyz

TS:   process.exit(1)
来源：http://htx.aibaodan.cn

Java: System.exit(1)
来源：http://xpn.jianghu66.top

Go:   os.Exit(1)
来源：http://jzr.tanke756.top

Ruby: exit 1
来源：http://myb.ctjpmb.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ehn.0kj1m.cn

[M06] 向标准错误输出
来源：http://gkl.yangfankeji.com

Py:   print("err", file=sys.stderr)
来源：http://kst.haohaochexian.top

PHP:  fwrite(STDERR, "err\n");
来源：http://hro.sjlbkw.cn

JS:   console.error("err")
来源：http://hgr.jinyuanbaomall.cn

TS:   console.error("err")
来源：http://pbz.wangdashe.top

Java: System.err.println("err")
来源：http://hyq.xylfe.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nbs.vehdjk.com

Ruby: warn "err"
来源：http://uhj.daxiang520.top

C#:   Console.Error.WriteLine("err")
来源：http://tkn.c1oappe.top

[M07] 判断是否为主入口
来源：http://zql.kuanghao11.cn

Py:   if __name__ == "__main__":
来源：http://vth.nwbrower.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nmz.wangshuangyany.cn

JS:   require.main === module
来源：http://xix.cashguo.top

TS:   require.main === module
来源：http://ewa.fktsv.cn

Java: public static void main(String[] args)
来源：http://qnq.yongpay.top

Go:   func main()
来源：http://tnf.hesvh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://khj.sweek.top

C#:   static void Main(string[] args)
来源：http://rbe.zhijiandao.cn

[M08] 获取系统与运行时信息
来源：http://fso.aibaodan.cn

Py:   platform.system();  platform.python_version()
来源：http://tms.epnwcf.com

PHP:  PHP_OS;  phpversion();
来源：http://xan.jqgfzy.top

JS:   process.platform;  process.version
来源：http://mxc.aibaodan.cn

TS:   process.platform;  process.version
来源：http://ihj.ctjpmb.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pih.gogol.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sjo.zycfv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dtr.mhx1999.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://fbw.epnwcf.com

================================================================================
来源：http://ewb.svipenyu.cn

N. 数据结构与算法
来源：http://nuy.gogol.net.cn

================================================================================
来源：http://aii.xuanzx.com

[N01] 二分查找（有序数组）
来源：http://asi.snrcjt.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mrq.gogol.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fdd.chenjidiqi.icu

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ecr.ydzc1.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bnd.wangshuangyany.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xmb.bjfxy.top

Go:   sort.SearchInts(arr, x)
来源：http://lxu.yvedp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://asd.yonumen.top

C#:   Array.BinarySearch(arr, x)
来源：http://baj.shangyingyoupin.top

[N02] 排序（工程实践用内置实现）
来源：http://xix.ppjwa.cn

Py:   sorted(arr);  arr.sort()
来源：http://nsb.jinqigfzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://icv.bjfxy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://hui.sjlbkw.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pym.xinyue.icu

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zrw.jinyuanbaomall.cn

Go:   slices.Sort(arr)
来源：http://chs.quarkkingdee.top

Ruby: arr.sort
来源：http://dhm.cheryme.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://htx.0kj1m.cn

[N03] 快速排序（分治示例）
来源：http://hzh.hnqzz.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ezq.cucudq.cn

PHP:  // 递归实现，或用 usort
来源：http://uhg.xinyue.icu

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ard.zhongyouzk.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bev.kuanghao11.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ftw.fehbvm.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://eei.nanxuanxn.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ubc.0kj1m.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ugg.feifeiyinyue.top

[N04] 斐波那契数列
来源：http://nra.feifeiyinyue.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uyg.dianchejie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mre.nanxuanxn.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tbp.nanxinkj.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pxk.hesvh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jyc.hnqzz.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ems.zhongyouzk.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kax.zhoulong.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://iny.iojbl.cn

[N05] 最大公约数
来源：http://hxq.shanyushiyangtech.top

Py:   math.gcd(a, b)
来源：http://mod.fzhhl.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rlm.yangfankeji.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mpy.gzhubu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zyv.shanyushiyangtech.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pqd.bjfxy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hef.dashuyun.cn

Ruby: a.gcd(b)
来源：http://ofj.hnqzz.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gpm.jyoumei.cn

[N06] 判断回文字符串
来源：http://iht.bbcook.cn

Py:   s == s[::-1]
来源：http://nun.aibaodan.cn

PHP:  $s === strrev($s);
来源：http://jow.gogol.net.cn

JS:   s === [...s].reverse().join("")
来源：http://heq.havefunace.top

TS:   s === [...s].reverse().join("")
来源：http://lwq.yj20258888.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hkr.c1oappe.top

Go:   // 双指针从两端比较
来源：http://plc.cqqwz.cn

Ruby: s == s.reverse
来源：http://mtu.nanxuanxn.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://cya.daxiang520.top

[N07] 两数之和（返回下标）
来源：http://zrg.daxiang520.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rsb.hfpthk.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ltj.yueranfly.top

JS:   // 手写 Map：map.set(v, i)
来源：http://zxi.dashuyun.cn

TS:   // 手写 Map<string, number>
来源：http://wiu.ctjpmb.com

Java: // 手写 HashMap
来源：http://nuu.52xcode.cn

Go:   // 手写 map[int]int
来源：http://xdy.ehwqpu.com

Ruby: // 手写 Hash
来源：http://vzb.yonumen.top

C#:   // 手写 Dictionary<int, int>
来源：http://qmz.fktsv.cn

[N08] 生成全排列
来源：http://zia.yongpay.top

Py:   itertools.permutations(arr)
来源：http://iyj.yj20258888.top

PHP:  // 手写递归交换
来源：http://xdx.nanxinkj.top

JS:   // 手写回溯递归
来源：http://kdu.gaohongyu789.top

TS:   // 手写回溯递归
来源：http://gda.xinyue.icu

Java: // 手写回溯递归
来源：http://ohs.yuanzhike.top

Go:   // 手写回溯递归
来源：http://rwi.ivvv.top

Ruby: arr.permutation.to_a
来源：http://qfa.fktsv.cn

C#:   // 手写回溯递归
来源：http://awk.fengsongda.top

[N09] 栈与队列
来源：http://wlg.c1oappe.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ujm.yongpay.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://veg.xylfe.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ubd.zdbjq.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qim.yj202588.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nnn.9152youxi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gxb.xziqi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mcj.fengsongda.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lao.havefunace.top

[N10] 链表节点定义
来源：http://bgw.wangshuangyany.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uvl.tianlin.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://brh.jyoumei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fge.guowangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bon.pycfn.com

Java: class Node { int v; Node next; }
来源：http://rhc.yanxiufei.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cku.pycfn.com

Ruby: Node = Struct.new(:v, :next)
来源：http://lxr.ctjpmb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://flq.hammf.cn

[N11] 二叉树中序遍历
来源：http://zqp.yj202588.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ymi.hesvh.cn

PHP:  // 手写递归函数
来源：http://osd.feifeiyinyue.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gmm.xuetiantiany.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jfh.dianchejie.cn

Java: // 手写递归
来源：http://yvf.hfpthk.cn

Go:   // 手写递归
来源：http://dbj.ehwqpu.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ekg.dashuyun.cn

C#:   // 手写递归
来源：http://eca.iojbl.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://asm.ydjk.org.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://znq.yfazqb.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vjb.hfpthk.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xqj.guowangkeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wyw.wangdashe.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://twt.vehdjk.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vdk.fehbvm.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fin.daxiang520.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oaw.hammf.cn

================================================================================
来源：http://kej.ydjk.org.cn

O. 并发与异步
来源：http://idw.shuidangran.top

================================================================================
来源：http://hlg.yangfankeji.com

[O01] 启动一个线程
来源：http://rjh.xuanzx.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dko.nwbrower.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ppu.jinqigufen.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tux.jianghu66.top

TS:   // 同 JS
来源：http://gyk.xuetiantiany.cn

Java: new Thread(() -> f()).start()
来源：http://oaa.dashuyun.cn

Go:   go f()
来源：http://diz.ivvv.top

Ruby: Thread.new { f }
来源：http://rfq.cashguo.top

C#:   Task.Run(() => F());
来源：http://tlb.jqgfzy.top

[O02] 使用线程池
来源：http://znm.fktsv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mik.shzxlz.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oen.chenzaomai.com

JS:   // worker_threads 线程池
来源：http://jby.redwolf501.top


<!-- 参考信息 -->