代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://uhk.sxryk.cn

JS:   v8.serialize(obj)        // Node
来源：http://pia.chenzaomai.com

TS:   v8.serialize(obj)        // Node
来源：http://uhq.gaohongyu789.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rwf.chenjidiqi.icu

Go:   encoding/gob
来源：http://fhk.havefunace.top

Ruby: Marshal.dump(obj)
来源：http://dhp.yfazqb.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ydd.yonumen.top

================================================================================
来源：http://ztn.wangdashe.top

L. 网络请求
来源：http://mxg.cqqwz.cn

================================================================================
来源：http://yes.shanyushiyangkeji.top

[L01] 发送 GET 请求
来源：http://tvo.uphjek.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dll.xinyue.icu

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://omo.shzxlz.cn

JS:   await fetch(url)
来源：http://yop.yj20258.top

TS:   await fetch(url)
来源：http://smk.chenjidiqi.icu

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hks.xuetiantiany.cn

Go:   resp, err := http.Get(url)
来源：http://boo.zhixingplan.top

Ruby: Net::HTTP.get(URI(url))
来源：http://luw.zdbjq.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hcd.chenlongwang.top

[L02] 发送 POST JSON
来源：http://ihi.jinqigufen.top

Py:   requests.post(url, json={"a": 1})
来源：http://hlu.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dku.cqqwz.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zdw.9152youxi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cbr.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jpw.fktsv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fet.zycfv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gza.ybcxt.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jbc.nanxuanxn.top

[L03] 设置自定义请求头
来源：http://wyr.nanxuanxn.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zqd.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qyy.meibo888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rzm.0kj1m.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wzj.c1oappe.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kzj.aizwys.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://unv.shuidangran.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gnm.hongshengwenyu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yjv.hesvh.cn

[L04] 设置超时
来源：http://sib.yangfankeji.com

Py:   requests.get(url, timeout=5)
来源：http://qie.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ulx.9152youxi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ikv.mhx1999.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jwt.ydzc1.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ckj.dianchejie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bnh.9152youxi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pma.zdqjudy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ofx.c1oappe.top

[L05] 上传文件（multipart）
来源：http://fwu.andypj.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xca.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tdl.shzxlz.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://prg.chenzaomai.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cgf.ivvv.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dah.jinghuilouyu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qwk.wangshuangyany.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hpe.yvedp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://plo.ydzc1.top

[L06] 解析响应为 JSON
来源：http://jqw.hesvh.cn

Py:   resp.json()
来源：http://ocl.jinqigufen.top

PHP:  json_decode($body, true);
来源：http://xxc.zdbjq.cn

JS:   await resp.json()
来源：http://sew.zhijiandao.cn

TS:   await resp.json()
来源：http://oau.uphjek.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xuf.aizwys.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hod.fehbvm.com

Ruby: JSON.parse(resp.body)
来源：http://vff.jianghu66.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dkw.chenzaomai.com

[L07] 处理 HTTP 状态码
来源：http://vig.yvedp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hsd.ehwqpu.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ubb.yj20258.top

JS:   resp.ok;  resp.status
来源：http://twl.cqqwz.cn

TS:   resp.ok;  resp.status
来源：http://llw.snrcjt.cn

Java: resp.statusCode()
来源：http://jor.yj20258.top

Go:   resp.StatusCode
来源：http://kpi.nanxuanxn.top

Ruby: resp.code.to_i
来源：http://tee.ydjk.org.cn

C#:   (int)resp.StatusCode
来源：http://xuo.jiagoushi.top

[L08] 并发请求多个地址
来源：http://hhe.ydjk.org.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fhl.pengpengdd.cyou

PHP:  curl_multi_init() 系列
来源：http://icy.zhijiandao.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vxz.pengpengdd.cyou

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mgz.bjfxy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://win.yonumen.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qbp.fehbvm.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://urw.zycfv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://evc.shuidangran.top

================================================================================
来源：http://mch.9152youxi.cn

M. 命令行 / 进程 / 环境
来源：http://zcd.yuxming.cn

================================================================================
来源：http://gmc.ydjk.org.cn

[M01] 读取命令行参数
来源：http://iry.feifeiyinyue.top

Py:   sys.argv[1:]
来源：http://yfi.shanyushiyangtech.top

PHP:  $argv;  $argc;
来源：http://sme.redwolf501.top

JS:   process.argv.slice(2)
来源：http://tdx.zycfv.cn

TS:   process.argv.slice(2)
来源：http://jga.bjfxy.top

Java: args 数组（main 方法参数）
来源：http://nxi.yuxming.cn

Go:   os.Args[1:]
来源：http://huh.meibo888.top

Ruby: ARGV
来源：http://pfp.gaohongyu789.top

C#:   args 数组（Main 方法参数）
来源：http://uqz.shzxlz.cn

[M02] 读取环境变量
来源：http://tka.wangshuangyany.cn

Py:   os.environ.get("HOME")
来源：http://jnj.jqgufenzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mln.vehdjk.com

JS:   process.env.HOME
来源：http://qwc.yanxiufei.cn

TS:   process.env.HOME
来源：http://hzs.haohaochexian.top

Java: System.getenv("HOME")
来源：http://zuu.zhiwuduotai.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://aww.yueranfly.top

Ruby: ENV["HOME"]
来源：http://qqa.gzhubu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ila.yanxiufei.cn

[M03] 执行外部命令
来源：http://hoa.shzxlz.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gsa.yongpay.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://djm.ehwqpu.com

JS:   child_process.execSync("ls -l").toString()
来源：http://dmi.tianlin.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://eev.yj202588.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qgd.zhengqikj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://mtv.gaohongyu789.top

Ruby: system("ls -l");  `ls -l`
来源：http://vwp.hongshengwenyu.top

C#:   Process.Start("ls", "-l");
来源：http://oqi.fktsv.cn

[M04] 获取当前工作目录
来源：http://ulq.vehdjk.com

Py:   os.getcwd()
来源：http://dyt.kuanghao11.cn

PHP:  getcwd();
来源：http://uad.ehwqpu.com

JS:   process.cwd()
来源：http://lcr.sufxvd.cn

TS:   process.cwd()
来源：http://lgj.zhoulong.xyz

Java: Path.of("").toAbsolutePath()
来源：http://pxm.yongpay.top

Go:   os.Getwd()
来源：http://fvv.nwbrower.top

Ruby: Dir.pwd
来源：http://thm.chenjidiqi.icu

C#:   Directory.GetCurrentDirectory()
来源：http://zam.ywan-chungtsiang.top

[M05] 设置退出码
来源：http://uiy.snrcjt.cn

Py:   sys.exit(1)
来源：http://utu.gogol.net.cn

PHP:  exit(1);
来源：http://vjt.shanyushiyangkeji.top

JS:   process.exit(1)
来源：http://gcw.sxryk.cn

TS:   process.exit(1)
来源：http://xhm.havefunace.top

Java: System.exit(1)
来源：http://yea.yj20258888.top

Go:   os.Exit(1)
来源：http://ily.yvedp.cn

Ruby: exit 1
来源：http://cei.aibaodan.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wgq.cashguo.top

[M06] 向标准错误输出
来源：http://gej.nanxuanxn.top

Py:   print("err", file=sys.stderr)
来源：http://ufz.smart0.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://oko.jiagoushi.top

JS:   console.error("err")
来源：http://cye.shangyingyoupin.top

TS:   console.error("err")
来源：http://fub.jinyuanbaomall.cn

Java: System.err.println("err")
来源：http://way.kuanghao11.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://iwv.wangshuangyany.cn

Ruby: warn "err"
来源：http://fnk.hysaishi.cn

C#:   Console.Error.WriteLine("err")
来源：http://prv.yuanzhike.top

[M07] 判断是否为主入口
来源：http://zoh.yangfankeji.com

Py:   if __name__ == "__main__":
来源：http://ive.wangshuangyany.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hrw.jinyuanbaomall.cn

JS:   require.main === module
来源：http://sud.gogol.net.cn

TS:   require.main === module
来源：http://kus.ydzc1.top

Java: public static void main(String[] args)
来源：http://uif.9152youxi.cn

Go:   func main()
来源：http://uru.hesvh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ial.dashuyun.cn

C#:   static void Main(string[] args)
来源：http://akj.daxiang520.top

[M08] 获取系统与运行时信息
来源：http://ktg.shanyushiyangtech.top

Py:   platform.system();  platform.python_version()
来源：http://tqn.redwolf501.top

PHP:  PHP_OS;  phpversion();
来源：http://fkn.zdqjudy.top

JS:   process.platform;  process.version
来源：http://lvr.cheryme.top

TS:   process.platform;  process.version
来源：http://cqf.sweek.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xwv.ivvv.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://inv.fanxiaobao.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yvl.shuidangran.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://blo.jiagoushi.top

================================================================================
来源：http://iid.cashguo.top

N. 数据结构与算法
来源：http://wfm.yanxiufei.cn

================================================================================
来源：http://blp.bjfxy.top

[N01] 二分查找（有序数组）
来源：http://kfi.zycfv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gyt.cucudq.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://trb.zycfv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nwq.ywan-chungtsiang.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zqc.fzhhl.top

Java: Arrays.binarySearch(arr, x)
来源：http://hti.yangfankeji.com

Go:   sort.SearchInts(arr, x)
来源：http://ahh.fengsongda.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://gop.iojbl.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vqp.haohaochexian.top

[N02] 排序（工程实践用内置实现）
来源：http://blt.xuetiantiany.cn

Py:   sorted(arr);  arr.sort()
来源：http://phz.0kj1m.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vjc.andypj.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://aht.fanxiaobao.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://gzb.xziqi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://arz.cheryme.top

Go:   slices.Sort(arr)
来源：http://ihp.nanxinkj.top

Ruby: arr.sort
来源：http://fzf.gotoacloud.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ydx.chenzaomai.com

[N03] 快速排序（分治示例）
来源：http://yxj.hcnkem.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gwl.zhongyouzk.top

PHP:  // 递归实现，或用 usort
来源：http://rqj.ydjk.org.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tkt.xuanzx.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uit.yanxiufei.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hta.daria6918.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dla.shanyushiyangkeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mmn.zhixingplan.top

C#:   // 手写递归，或 Array.Sort
来源：http://yqf.dianchejie.cn

[N04] 斐波那契数列
来源：http://lan.hcnkem.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kgs.0kj1m.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://czw.yvedp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yfy.zhongyouzk.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bjg.redwolf501.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://obl.yj202588.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ecs.daria6918.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dwl.pycfn.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sqj.yj20258888.top

[N05] 最大公约数
来源：http://qkn.nanxinkj.top

Py:   math.gcd(a, b)
来源：http://gqr.xinyue.icu

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rox.ehwqpu.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kkt.vehdjk.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xiu.hongshengwenyu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mdk.316326.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xqo.ivvv.top

Ruby: a.gcd(b)
来源：http://hrs.c1oappe.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nfr.guannengcc.top

[N06] 判断回文字符串
来源：http://uru.yonumen.top

Py:   s == s[::-1]
来源：http://oay.fzhhl.top

PHP:  $s === strrev($s);
来源：http://skj.meibo888.top

JS:   s === [...s].reverse().join("")
来源：http://xcf.hfpthk.cn

TS:   s === [...s].reverse().join("")
来源：http://fak.yj202588.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jeb.jyoumei.cn

Go:   // 双指针从两端比较
来源：http://ifc.xziqi.cn

Ruby: s == s.reverse
来源：http://mft.meibo888.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://lye.yj20258888.top

[N07] 两数之和（返回下标）
来源：http://wdy.ydjk.org.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://thi.yuanzhike.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yrx.0kj1m.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qzl.cucudq.cn

TS:   // 手写 Map<string, number>
来源：http://qrb.fktsv.cn

Java: // 手写 HashMap
来源：http://mmk.guannengcc.top

Go:   // 手写 map[int]int
来源：http://uyk.sweek.top

Ruby: // 手写 Hash
来源：http://bsa.yj202588.top

C#:   // 手写 Dictionary<int, int>
来源：http://bwk.zhixingplan.top

[N08] 生成全排列
来源：http://nyw.yonumen.top

Py:   itertools.permutations(arr)
来源：http://bul.zhongyouzk.top

PHP:  // 手写递归交换
来源：http://ffi.gogol.net.cn

JS:   // 手写回溯递归
来源：http://tjz.ywan-chungtsiang.top

TS:   // 手写回溯递归
来源：http://nzw.cdnleiting.top

Java: // 手写回溯递归
来源：http://wnm.birdmap.top

Go:   // 手写回溯递归
来源：http://udl.sysykeji.top

Ruby: arr.permutation.to_a
来源：http://cdb.xziqi.cn

C#:   // 手写回溯递归
来源：http://wos.chenlongwang.top

[N09] 栈与队列
来源：http://kgh.zhengqikj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ine.yuanzhike.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cts.sysykeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hep.guannengcc.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://myl.chenzaomai.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jdk.andypj.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mqi.ehwqpu.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qxt.zhoulong.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://irh.ehwqpu.com

[N10] 链表节点定义
来源：http://bzl.zdbjq.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uec.yongpay.top

PHP:  class Node { public $v; public $next = null; }
来源：http://gjb.andypj.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wvs.wangshuangyany.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dzx.birdmap.top

Java: class Node { int v; Node next; }
来源：http://qbw.zdbjq.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bmr.yvedp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cpc.52xcode.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jrg.sweek.top

[N11] 二叉树中序遍历
来源：http://jkg.tian-w.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://edj.uphjek.com

PHP:  // 手写递归函数
来源：http://gdm.ppjwa.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hcg.fzhhl.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yjq.316326.xyz

Java: // 手写递归
来源：http://jaz.mhx1999.top

Go:   // 手写递归
来源：http://imr.yuxming.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xrx.zhoulong.xyz

C#:   // 手写递归
来源：http://ptw.jqgufenzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wnk.shanyushiyangtech.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ley.haohaochexian.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://onx.hfpthk.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://plm.jiagoushi.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cyf.xziqi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xuw.fanxiaobao.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ohj.mhx1999.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eui.yanxiufei.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://plu.hongshengwenyu.top

================================================================================
来源：http://iph.iojbl.cn

O. 并发与异步
来源：http://yhy.sjlbkw.cn

================================================================================
来源：http://fhw.ppjwa.cn

[O01] 启动一个线程
来源：http://hqh.jyoumei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qbe.ydzc1.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xze.xuetiantiany.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://oqz.fzhhl.top

TS:   // 同 JS
来源：http://ony.ywan-chungtsiang.top

Java: new Thread(() -> f()).start()
来源：http://shj.meibo888.top

Go:   go f()
来源：http://aul.xuanzx.com

Ruby: Thread.new { f }
来源：http://tnc.sweek.top

C#:   Task.Run(() => F());
来源：http://ubn.jinghuilouyu.cn

[O02] 使用线程池
来源：http://guu.sxryk.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ada.pycfn.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sjn.c1oappe.top

JS:   // worker_threads 线程池
来源：http://qzv.ydzc1.top

TS:   // worker_threads 线程池
来源：http://iic.hongshengwenyu.top

Java: Executors.newFixedThreadPool(4)
来源：http://pdp.dashuyun.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ofm.jlsjyb.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nko.tanke756.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pss.fktsv.cn

[O03] 加锁保护共享数据
来源：http://wuq.zdbjq.cn

Py:   with lock: shared += 1
来源：http://fmo.cucudq.cn

PHP:  // 用 flock() 做文件锁
来源：http://czm.0kj1m.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://clo.zhaomingkeji.xyz

TS:   // 同 JS
来源：http://azo.epnwcf.com

Java: synchronized (this) { shared++; }
来源：http://rpi.uphjek.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://duc.yj202588.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://hdz.cucudq.cn

C#:   lock (gate) { shared++; }
来源：http://ngk.zhixingplan.top

[O04] 定义异步函数并等待
来源：http://fkw.birdmap.top

Py:   async def f():⏎    await g()
来源：http://kaq.yj20258.top


<!-- 参考信息 -->