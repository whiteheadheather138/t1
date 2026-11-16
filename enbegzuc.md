代发 wailian999

L. 网络请求
来源：http://nfo.nwbrower.top

================================================================================
来源：http://uxv.shanyushiyangkeji.top

[L01] 发送 GET 请求
来源：http://xvo.andypj.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bmi.cucudq.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fbh.9152youxi.cn

JS:   await fetch(url)
来源：http://zza.zhaomingkeji.xyz

TS:   await fetch(url)
来源：http://ope.aibaodan.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kld.daxiang520.top

Go:   resp, err := http.Get(url)
来源：http://qqm.xinyue.icu

Ruby: Net::HTTP.get(URI(url))
来源：http://apd.shangyingyoupin.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bjg.zhongyouzk.top

[L02] 发送 POST JSON
来源：http://ncj.shanyushiyangtech.top

Py:   requests.post(url, json={"a": 1})
来源：http://etd.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jno.chenjidiqi.icu

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uhb.guannengcc.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uzv.nanxinkj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wsa.fanxiaobao.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://win.jlsjyb.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yiy.guowangkeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xsi.316326.xyz

[L03] 设置自定义请求头
来源：http://ppp.zhijiandao.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gvl.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dix.sufxvd.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vxt.tianlin.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://csg.wangshuangyany.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://djx.ctjpmb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://icb.52xcode.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://etn.wangdashe.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://exa.dashuyun.cn

[L04] 设置超时
来源：http://fhs.ivvv.top

Py:   requests.get(url, timeout=5)
来源：http://amm.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://guy.feifeiyinyue.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://egc.gogol.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://geh.cucudq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kya.mhx1999.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://efx.hysaishi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://btt.xuetiantiany.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://iqr.xingfuxueyuan.xyz

[L05] 上传文件（multipart）
来源：http://bco.zhoulong.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eoo.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lxj.hnqzz.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://izi.jqgufenzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tys.daxiang520.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dgb.dianchejie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://aci.yongpay.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jgp.jinyuanbaomall.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lno.xingfuxueyuan.xyz

[L06] 解析响应为 JSON
来源：http://slm.shangyingyoupin.top

Py:   resp.json()
来源：http://fmh.yfazqb.com

PHP:  json_decode($body, true);
来源：http://gnh.yfazqb.com

JS:   await resp.json()
来源：http://ggr.fanxiaobao.xyz

TS:   await resp.json()
来源：http://hae.cdnleiting.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oar.jinghuilouyu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hnl.cheryme.top

Ruby: JSON.parse(resp.body)
来源：http://ugj.yueranfly.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://viv.ivvv.top

[L07] 处理 HTTP 状态码
来源：http://you.yonumen.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sfd.xylfe.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vfi.nanxuanxn.top

JS:   resp.ok;  resp.status
来源：http://sia.guannengcc.top

TS:   resp.ok;  resp.status
来源：http://flh.tianlin.xyz

Java: resp.statusCode()
来源：http://mpa.gaohongyu789.top

Go:   resp.StatusCode
来源：http://xkd.zhixingplan.top

Ruby: resp.code.to_i
来源：http://eok.yvedp.cn

C#:   (int)resp.StatusCode
来源：http://zuj.iojbl.cn

[L08] 并发请求多个地址
来源：http://vek.chenlongwang.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bxu.0kj1m.cn

PHP:  curl_multi_init() 系列
来源：http://ehi.yangfankeji.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cte.haohaochexian.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qic.shanyushiyangtech.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uwg.tianlin.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://beh.sweek.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vwa.0kj1m.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jva.xingfuxueyuan.xyz

================================================================================
来源：http://kik.sweek.top

M. 命令行 / 进程 / 环境
来源：http://jsx.andypj.xyz

================================================================================
来源：http://swo.chenjidiqi.icu

[M01] 读取命令行参数
来源：http://osu.havefunace.top

Py:   sys.argv[1:]
来源：http://pzs.ydzc1.top

PHP:  $argv;  $argc;
来源：http://pwi.chenjidiqi.icu

JS:   process.argv.slice(2)
来源：http://wmm.cdnleiting.top

TS:   process.argv.slice(2)
来源：http://kdn.guannengcc.top

Java: args 数组（main 方法参数）
来源：http://dxg.wangshuangyany.cn

Go:   os.Args[1:]
来源：http://rxm.52xcode.cn

Ruby: ARGV
来源：http://uac.gaohongyu789.top

C#:   args 数组（Main 方法参数）
来源：http://gxk.guowangkeji.top

[M02] 读取环境变量
来源：http://rmb.kuanghao11.cn

Py:   os.environ.get("HOME")
来源：http://taj.nanxinkj.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sze.iojbl.cn

JS:   process.env.HOME
来源：http://svs.aibaodan.cn

TS:   process.env.HOME
来源：http://cct.aizwys.cn

Java: System.getenv("HOME")
来源：http://vhh.fanxiaobao.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lhs.zhixingplan.top

Ruby: ENV["HOME"]
来源：http://tqn.smart0.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lds.hesvh.cn

[M03] 执行外部命令
来源：http://vqc.0kj1m.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ioq.zdbjq.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cza.nanxuanxn.top

JS:   child_process.execSync("ls -l").toString()
来源：http://khn.zycfv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hkv.shanyushiyangtech.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nhn.yueranfly.top

Go:   exec.Command("ls", "-l").Output()
来源：http://mvr.meibo888.top

Ruby: system("ls -l");  `ls -l`
来源：http://dxy.shanyushiyangkeji.top

C#:   Process.Start("ls", "-l");
来源：http://bht.yuxming.cn

[M04] 获取当前工作目录
来源：http://dmx.jinyuanbaomall.cn

Py:   os.getcwd()
来源：http://ezt.shzxlz.cn

PHP:  getcwd();
来源：http://wqp.xuetiantiany.cn

JS:   process.cwd()
来源：http://ori.tarul.cn

TS:   process.cwd()
来源：http://bqx.ydzc1.top

Java: Path.of("").toAbsolutePath()
来源：http://hcg.hcnkem.com

Go:   os.Getwd()
来源：http://keb.tian-w.cn

Ruby: Dir.pwd
来源：http://gdc.zdqjudy.top

C#:   Directory.GetCurrentDirectory()
来源：http://emf.c1oappe.top

[M05] 设置退出码
来源：http://lzs.jiagoushi.top

Py:   sys.exit(1)
来源：http://oxl.jinqigufen.top

PHP:  exit(1);
来源：http://awu.gogol.net.cn

JS:   process.exit(1)
来源：http://ade.zhixingplan.top

TS:   process.exit(1)
来源：http://byx.zhiwuduotai.top

Java: System.exit(1)
来源：http://lyu.gzhubu.top

Go:   os.Exit(1)
来源：http://jzd.316326.xyz

Ruby: exit 1
来源：http://dae.gotoacloud.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hdx.aizwys.cn

[M06] 向标准错误输出
来源：http://pga.ybcxt.top

Py:   print("err", file=sys.stderr)
来源：http://nzk.fengsongda.top

PHP:  fwrite(STDERR, "err\n");
来源：http://isu.andypj.xyz

JS:   console.error("err")
来源：http://qhx.52xcode.cn

TS:   console.error("err")
来源：http://cji.vehdjk.com

Java: System.err.println("err")
来源：http://elm.kuanghao11.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dro.sufxvd.cn

Ruby: warn "err"
来源：http://wxs.sjlbkw.cn

C#:   Console.Error.WriteLine("err")
来源：http://unz.xuanzx.com

[M07] 判断是否为主入口
来源：http://qhb.hcnkem.com

Py:   if __name__ == "__main__":
来源：http://ilj.uphjek.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hsb.shanyushiyangkeji.top

JS:   require.main === module
来源：http://wgr.jinyuanbaomall.cn

TS:   require.main === module
来源：http://sfe.yuxming.cn

Java: public static void main(String[] args)
来源：http://qoa.zhongyouzk.top

Go:   func main()
来源：http://sux.yuanzhike.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uke.c1oappe.top

C#:   static void Main(string[] args)
来源：http://vll.c1oappe.top

[M08] 获取系统与运行时信息
来源：http://wqf.guannengcc.top

Py:   platform.system();  platform.python_version()
来源：http://zbp.ctjpmb.com

PHP:  PHP_OS;  phpversion();
来源：http://aee.yonumen.top

JS:   process.platform;  process.version
来源：http://bcj.jqgfzy.top

TS:   process.platform;  process.version
来源：http://btk.fanxiaobao.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gtg.nanxuanxn.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://nim.shzxlz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jna.andypj.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://gnn.shanyushiyangkeji.top

================================================================================
来源：http://vwy.zhengqikj.top

N. 数据结构与算法
来源：http://pxn.hfpthk.cn

================================================================================
来源：http://tth.ydzc1.top

[N01] 二分查找（有序数组）
来源：http://daa.hcnkem.com

Py:   bisect.bisect_left(arr, x)
来源：http://jvr.shzxlz.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mgd.guannengcc.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rln.jqgufenzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://its.cheryme.top

Java: Arrays.binarySearch(arr, x)
来源：http://qpj.gaohongyu789.top

Go:   sort.SearchInts(arr, x)
来源：http://kam.cqqwz.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://uqu.vqdsnc.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uzs.svipenyu.cn

[N02] 排序（工程实践用内置实现）
来源：http://fbp.tianlin.xyz

Py:   sorted(arr);  arr.sort()
来源：http://zho.sweek.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ckp.tian-w.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bnx.jqgfzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://wuy.sxryk.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dvt.guowangkeji.top

Go:   slices.Sort(arr)
来源：http://lhm.ydjk.org.cn

Ruby: arr.sort
来源：http://xzj.jqgufenzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://zyv.gzhubu.top

[N03] 快速排序（分治示例）
来源：http://vmb.hfpthk.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xuj.shangyingyoupin.top

PHP:  // 递归实现，或用 usort
来源：http://xuj.daria6918.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://abp.redwolf501.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eip.sjlbkw.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fvy.xuanzx.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cuq.pycfn.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://piq.tarul.cn

C#:   // 手写递归，或 Array.Sort
来源：http://yya.ydjk.org.cn

[N04] 斐波那契数列
来源：http://giw.zhengqikj.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://aps.yanxiufei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://veg.sxryk.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zpq.feifeiyinyue.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oxq.chenzaomai.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://oph.xziqi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fxl.gotoacloud.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://asq.jianghu66.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hcn.shzxlz.cn

[N05] 最大公约数
来源：http://lte.jinghuilouyu.cn

Py:   math.gcd(a, b)
来源：http://afj.jianghu66.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oze.birdmap.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dra.sufxvd.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zpm.yangfankeji.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zcq.yj20258888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cvy.zhengqikj.top

Ruby: a.gcd(b)
来源：http://oer.xingfuxueyuan.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://alc.yangfankeji.com

[N06] 判断回文字符串
来源：http://ysp.tian-w.cn

Py:   s == s[::-1]
来源：http://uhc.tanke756.top

PHP:  $s === strrev($s);
来源：http://ave.yanxiufei.cn

JS:   s === [...s].reverse().join("")
来源：http://chn.fzhhl.top

TS:   s === [...s].reverse().join("")
来源：http://ukw.xylfe.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://czw.cucudq.cn

Go:   // 双指针从两端比较
来源：http://hje.shzxlz.cn

Ruby: s == s.reverse
来源：http://yhz.tarul.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ogw.hfpthk.cn

[N07] 两数之和（返回下标）
来源：http://jyf.cashguo.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yyy.cheryme.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lol.daria6918.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://idf.xylfe.cn

TS:   // 手写 Map<string, number>
来源：http://ktr.cucudq.cn

Java: // 手写 HashMap
来源：http://jpp.xuanzx.com

Go:   // 手写 map[int]int
来源：http://rhw.9152youxi.cn

Ruby: // 手写 Hash
来源：http://gqz.zhoulong.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://wkz.gotoacloud.top

[N08] 生成全排列
来源：http://drb.0kj1m.cn

Py:   itertools.permutations(arr)
来源：http://nvz.shanyushiyangkeji.top

PHP:  // 手写递归交换
来源：http://ubf.yfazqb.com

JS:   // 手写回溯递归
来源：http://aqe.jqgfzy.top

TS:   // 手写回溯递归
来源：http://ghp.hcnkem.com

Java: // 手写回溯递归
来源：http://nst.guowangkeji.top

Go:   // 手写回溯递归
来源：http://aov.fzhhl.top

Ruby: arr.permutation.to_a
来源：http://xve.andypj.xyz

C#:   // 手写回溯递归
来源：http://wax.chenzaomai.com

[N09] 栈与队列
来源：http://awz.52xcode.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qsi.vqdsnc.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xqg.uphjek.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ilj.ehwqpu.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rqb.jiagoushi.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jrs.xylfe.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zjt.cqqwz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://arn.cqqwz.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bxx.gzhubu.top

[N10] 链表节点定义
来源：http://slw.nanxinkj.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wga.jinyuanbaomall.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hgo.chenlongwang.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nrb.sysykeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fqv.tian-w.cn

Java: class Node { int v; Node next; }
来源：http://sva.jyoumei.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xks.chenjidiqi.icu

Ruby: Node = Struct.new(:v, :next)
来源：http://cqi.shangyingyoupin.top

C#:   class Node { public int V; public Node? Next; }
来源：http://byx.xuetiantiany.cn

[N11] 二叉树中序遍历
来源：http://bdy.hnxiangtu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xqk.mhx1999.top

PHP:  // 手写递归函数
来源：http://llf.vqdsnc.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ofz.yongpay.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fzp.wangdashe.top

Java: // 手写递归
来源：http://toq.zdqjudy.top

Go:   // 手写递归
来源：http://pub.xylfe.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vte.fanxiaobao.xyz

C#:   // 手写递归
来源：http://usw.smart0.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ugm.bjfxy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://iaw.chenzaomai.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uop.epnwcf.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pnt.jqgfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ltr.andypj.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sqa.hcnkem.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://slu.jqgfzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fmg.feifeiyinyue.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cwe.ydzc1.top

================================================================================
来源：http://ray.nanxuanxn.top

O. 并发与异步
来源：http://fsk.hesvh.cn

================================================================================
来源：http://igj.tian-w.cn

[O01] 启动一个线程
来源：http://pph.ydjk.org.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sig.bbcook.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uej.xinyue.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cew.ydzc1.top

TS:   // 同 JS
来源：http://znf.yuanzhike.top

Java: new Thread(() -> f()).start()
来源：http://rcv.ppjwa.cn

Go:   go f()
来源：http://pnx.vehdjk.com

Ruby: Thread.new { f }
来源：http://mlk.zhaomingkeji.xyz

C#:   Task.Run(() => F());
来源：http://fhg.cashguo.top

[O02] 使用线程池
来源：http://sgm.daxiang520.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nrz.316326.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://smo.sweek.top

JS:   // worker_threads 线程池
来源：http://bdo.havefunace.top

TS:   // worker_threads 线程池
来源：http://jxb.316326.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://rru.nanxuanxn.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://amm.vehdjk.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://crf.nanxuanxn.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nyl.zhengqikj.top

[O03] 加锁保护共享数据
来源：http://nky.epnwcf.com

Py:   with lock: shared += 1
来源：http://mvv.316326.xyz

PHP:  // 用 flock() 做文件锁
来源：http://soc.aibaodan.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rxz.gzhubu.top

TS:   // 同 JS
来源：http://sgf.shuidangran.top

Java: synchronized (this) { shared++; }
来源：http://oef.fengsongda.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lbs.fktsv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kxd.hcnkem.com

C#:   lock (gate) { shared++; }
来源：http://mfz.smart0.xyz

[O04] 定义异步函数并等待
来源：http://zlh.zhengqikj.top

Py:   async def f():⏎    await g()
来源：http://ubn.jqgufenzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://foo.fengsongda.top

JS:   async function f() { await g(); }
来源：http://ydo.birdmap.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://qpt.guannengcc.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hua.jinqigufen.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xaq.quarkkingdee.top

Ruby: # 用 Fiber 或 async gem
来源：http://qek.xingfuxueyuan.xyz

C#:   async Task F() { await G(); }
来源：http://ils.uphjek.com

[O05] 并发执行并等待全部完成
来源：http://yjo.chenlongwang.top


<!-- 参考信息 -->