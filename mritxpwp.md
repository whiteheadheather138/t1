代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://niv.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kyb.quarkkingdee.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hrh.xuanzx.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yti.cheryme.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://chk.yueranfly.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ima.zhaomingkeji.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dba.bjfxy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ixj.havefunace.top

[L03] 设置自定义请求头
来源：http://kmu.hesvh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ibf.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fni.pycfn.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qos.yuanzhike.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ozm.yj20258.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nbs.chenzaomai.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://laj.feifeiyinyue.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zzk.yanxiufei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pjv.xingfuxueyuan.xyz

[L04] 设置超时
来源：http://tka.haohaochexian.top

Py:   requests.get(url, timeout=5)
来源：http://zzt.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mvf.meibo888.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lzc.pycfn.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kim.0kj1m.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fty.sxryk.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://per.316326.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qzj.tian-w.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pjp.mhx1999.top

[L05] 上传文件（multipart）
来源：http://qcw.daxiang520.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jfx.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xqc.yangfankeji.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hyh.jianghu66.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://opk.tanke756.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bnk.iojbl.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vqb.0kj1m.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rtr.zhijiandao.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://eaz.xinyue.icu

[L06] 解析响应为 JSON
来源：http://bqn.fehbvm.com

Py:   resp.json()
来源：http://qqa.52xcode.cn

PHP:  json_decode($body, true);
来源：http://nqf.sufxvd.cn

JS:   await resp.json()
来源：http://mwd.zhaomingkeji.xyz

TS:   await resp.json()
来源：http://glt.daxiang520.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dvq.fzhhl.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tin.yangfankeji.com

Ruby: JSON.parse(resp.body)
来源：http://wkn.0kj1m.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ima.52xcode.cn

[L07] 处理 HTTP 状态码
来源：http://sru.fengsongda.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lej.hysaishi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jxh.fzhhl.top

JS:   resp.ok;  resp.status
来源：http://yfo.yj202588.top

TS:   resp.ok;  resp.status
来源：http://xgu.wangshuangyany.cn

Java: resp.statusCode()
来源：http://uxj.xylfe.cn

Go:   resp.StatusCode
来源：http://tny.hammf.cn

Ruby: resp.code.to_i
来源：http://vvm.gaohongyu789.top

C#:   (int)resp.StatusCode
来源：http://tko.fktsv.cn

[L08] 并发请求多个地址
来源：http://enc.zhengqikj.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://shz.nwbrower.top

PHP:  curl_multi_init() 系列
来源：http://kxs.shuidangran.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://huk.hcnkem.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://srq.jianghu66.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lsd.feifeiyinyue.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pct.zhongyouzk.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yex.dashuyun.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ety.fktsv.cn

================================================================================
来源：http://xuo.fanxiaobao.xyz

M. 命令行 / 进程 / 环境
来源：http://bzt.xuanzx.com

================================================================================
来源：http://cyt.yuanzhike.top

[M01] 读取命令行参数
来源：http://veq.ehwqpu.com

Py:   sys.argv[1:]
来源：http://pzb.yj20258.top

PHP:  $argv;  $argc;
来源：http://cgu.hcnkem.com

JS:   process.argv.slice(2)
来源：http://huw.yj20258888.top

TS:   process.argv.slice(2)
来源：http://ocn.fanxiaobao.xyz

Java: args 数组（main 方法参数）
来源：http://mnb.vehdjk.com

Go:   os.Args[1:]
来源：http://iqh.shanyushiyangkeji.top

Ruby: ARGV
来源：http://umc.xziqi.cn

C#:   args 数组（Main 方法参数）
来源：http://piu.chenzaomai.com

[M02] 读取环境变量
来源：http://ear.vehdjk.com

Py:   os.environ.get("HOME")
来源：http://ntr.ppjwa.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ljs.tian-w.cn

JS:   process.env.HOME
来源：http://jut.epnwcf.com

TS:   process.env.HOME
来源：http://fkh.fzhhl.top

Java: System.getenv("HOME")
来源：http://nqx.jianghu66.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vcr.quarkkingdee.top

Ruby: ENV["HOME"]
来源：http://nqs.dashuyun.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wbs.hywenlv.cn

[M03] 执行外部命令
来源：http://aty.vqdsnc.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xzn.fanxiaobao.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hxd.jinghuilouyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dor.tarul.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bsw.havefunace.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://otb.snrcjt.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://akb.pengpengdd.cyou

Ruby: system("ls -l");  `ls -l`
来源：http://fjn.gotoacloud.top

C#:   Process.Start("ls", "-l");
来源：http://eei.vehdjk.com

[M04] 获取当前工作目录
来源：http://eda.epnwcf.com

Py:   os.getcwd()
来源：http://ecf.xinyue.icu

PHP:  getcwd();
来源：http://nzg.hfpthk.cn

JS:   process.cwd()
来源：http://hky.sxryk.cn

TS:   process.cwd()
来源：http://auz.hesvh.cn

Java: Path.of("").toAbsolutePath()
来源：http://dbn.ybcxt.top

Go:   os.Getwd()
来源：http://erf.xinyue.icu

Ruby: Dir.pwd
来源：http://tlc.jyoumei.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gcd.9152youxi.cn

[M05] 设置退出码
来源：http://cvv.cdnleiting.top

Py:   sys.exit(1)
来源：http://lua.guowangkeji.top

PHP:  exit(1);
来源：http://iyx.gaohongyu789.top

JS:   process.exit(1)
来源：http://vls.yj20258.top

TS:   process.exit(1)
来源：http://dhm.yuanzhike.top

Java: System.exit(1)
来源：http://tus.yvedp.cn

Go:   os.Exit(1)
来源：http://ofp.zhengqikj.top

Ruby: exit 1
来源：http://nlk.cashguo.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kbv.daxiang520.top

[M06] 向标准错误输出
来源：http://zyg.cheryme.top

Py:   print("err", file=sys.stderr)
来源：http://lfo.xingfuxueyuan.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://rfx.svipenyu.cn

JS:   console.error("err")
来源：http://bsu.meibo888.top

TS:   console.error("err")
来源：http://tjv.uphjek.com

Java: System.err.println("err")
来源：http://jwn.c1oappe.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pjl.yueranfly.top

Ruby: warn "err"
来源：http://dfh.zhijiandao.cn

C#:   Console.Error.WriteLine("err")
来源：http://bjh.0kj1m.cn

[M07] 判断是否为主入口
来源：http://wni.daria6918.cn

Py:   if __name__ == "__main__":
来源：http://lbf.cdnleiting.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cnv.zhengqikj.top

JS:   require.main === module
来源：http://gwl.hongshengwenyu.top

TS:   require.main === module
来源：http://qon.birdmap.top

Java: public static void main(String[] args)
来源：http://qmx.zhixingplan.top

Go:   func main()
来源：http://dpf.feifeiyinyue.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ohh.hnxiangtu.top

C#:   static void Main(string[] args)
来源：http://yvx.fehbvm.com

[M08] 获取系统与运行时信息
来源：http://odn.iojbl.cn

Py:   platform.system();  platform.python_version()
来源：http://lpw.yongpay.top

PHP:  PHP_OS;  phpversion();
来源：http://zrq.smart0.xyz

JS:   process.platform;  process.version
来源：http://eya.chenzaomai.com

TS:   process.platform;  process.version
来源：http://cql.316326.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sqr.fanxiaobao.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://jrt.fanxiaobao.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uxg.bjfxy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://gbx.zhengqikj.top

================================================================================
来源：http://lzb.jinghuilouyu.cn

N. 数据结构与算法
来源：http://fqp.ywan-chungtsiang.top

================================================================================
来源：http://ltg.yueranfly.top

[N01] 二分查找（有序数组）
来源：http://sqb.nwbrower.top

Py:   bisect.bisect_left(arr, x)
来源：http://epv.quarkkingdee.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://clf.andypj.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tlg.fehbvm.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dgt.kuanghao11.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ijb.zdbjq.cn

Go:   sort.SearchInts(arr, x)
来源：http://kzm.aibaodan.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ztd.feifeiyinyue.top

C#:   Array.BinarySearch(arr, x)
来源：http://uzq.yj20258.top

[N02] 排序（工程实践用内置实现）
来源：http://iux.yj202588.top

Py:   sorted(arr);  arr.sort()
来源：http://zbi.hongshengwenyu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://oed.zycfv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://oxc.ybcxt.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://xmz.chenzaomai.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://eob.meibo888.top

Go:   slices.Sort(arr)
来源：http://qfl.xingfuxueyuan.xyz

Ruby: arr.sort
来源：http://tiw.wangdashe.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xzy.shzxlz.cn

[N03] 快速排序（分治示例）
来源：http://nlc.quarkkingdee.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ums.hywenlv.cn

PHP:  // 递归实现，或用 usort
来源：http://rah.xinyue.icu

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://poo.tanke756.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vtm.fehbvm.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xsy.daxiang520.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tjm.tian-w.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nie.sufxvd.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wcf.svipenyu.cn

[N04] 斐波那契数列
来源：http://scn.jinqigufen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://amw.shuidangran.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ghf.aibaodan.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wio.ybcxt.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kol.sufxvd.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bqr.yanxiufei.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://auu.chenjidiqi.icu

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://eii.nanxuanxn.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lxx.zdbjq.cn

[N05] 最大公约数
来源：http://bej.svipenyu.cn

Py:   math.gcd(a, b)
来源：http://sup.shangyingyoupin.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qvb.ybcxt.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hgf.hcnkem.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ckg.jlsjyb.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ion.mhx1999.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jnn.xinyue.icu

Ruby: a.gcd(b)
来源：http://boc.shanyushiyangtech.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ktz.jqgufenzy.top

[N06] 判断回文字符串
来源：http://nkz.hesvh.cn

Py:   s == s[::-1]
来源：http://tty.meibo888.top

PHP:  $s === strrev($s);
来源：http://wmu.yonumen.top

JS:   s === [...s].reverse().join("")
来源：http://qlh.xinyue.icu

TS:   s === [...s].reverse().join("")
来源：http://dmg.jqgufenzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dqi.zycfv.cn

Go:   // 双指针从两端比较
来源：http://imm.sxryk.cn

Ruby: s == s.reverse
来源：http://geh.zycfv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lch.jqgufenzy.top

[N07] 两数之和（返回下标）
来源：http://clk.yj202588.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ymd.ywan-chungtsiang.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gis.yanxiufei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pbv.pengpengdd.cyou

TS:   // 手写 Map<string, number>
来源：http://ber.dianchejie.cn

Java: // 手写 HashMap
来源：http://mvc.yangfankeji.com

Go:   // 手写 map[int]int
来源：http://lrp.kuanghao11.cn

Ruby: // 手写 Hash
来源：http://kap.aizwys.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bbd.gzhubu.top

[N08] 生成全排列
来源：http://wcf.sxryk.cn

Py:   itertools.permutations(arr)
来源：http://yqu.xuetiantiany.cn

PHP:  // 手写递归交换
来源：http://iwi.zhijiandao.cn

JS:   // 手写回溯递归
来源：http://nef.ydjk.org.cn

TS:   // 手写回溯递归
来源：http://yed.svipenyu.cn

Java: // 手写回溯递归
来源：http://tqt.haohaochexian.top

Go:   // 手写回溯递归
来源：http://uru.yj20258.top

Ruby: arr.permutation.to_a
来源：http://cgf.hnqzz.top

C#:   // 手写回溯递归
来源：http://vph.316326.xyz

[N09] 栈与队列
来源：http://sml.cqqwz.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cfu.yonumen.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rgv.fktsv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yxf.yvedp.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bbq.zycfv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ika.dashuyun.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ewv.bjfxy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ogw.kuanghao11.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xfq.pycfn.com

[N10] 链表节点定义
来源：http://jfz.zhixingplan.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pve.guannengcc.top

PHP:  class Node { public $v; public $next = null; }
来源：http://sws.chenzaomai.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wds.cheryme.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qjl.gaohongyu789.top

Java: class Node { int v; Node next; }
来源：http://rpy.sxryk.cn

Go:   type Node struct { V int; Next *Node }
来源：http://whf.wangshuangyany.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ros.snrcjt.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zbb.xuanzx.com

[N11] 二叉树中序遍历
来源：http://cvh.cqqwz.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cxh.chenzaomai.com

PHP:  // 手写递归函数
来源：http://znv.hnqzz.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wpz.xuanzx.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vfr.fengsongda.top

Java: // 手写递归
来源：http://vas.cdnleiting.top

Go:   // 手写递归
来源：http://pzr.chenjidiqi.icu

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bwv.zhongyouzk.top

C#:   // 手写递归
来源：http://xey.c1oappe.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bbn.sjlbkw.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yhy.jlsjyb.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xlv.zycfv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dqb.chenzaomai.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aij.xylfe.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ymv.zhiwuduotai.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ohn.gaohongyu789.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nua.shangyingyoupin.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hgu.vehdjk.com

================================================================================
来源：http://eku.tian-w.cn

O. 并发与异步
来源：http://vza.ywan-chungtsiang.top

================================================================================
来源：http://xhj.smart0.xyz

[O01] 启动一个线程
来源：http://voq.dianchejie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zud.bjfxy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fet.hesvh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kmr.nanxuanxn.top

TS:   // 同 JS
来源：http://pzz.yfazqb.com

Java: new Thread(() -> f()).start()
来源：http://swo.pycfn.com

Go:   go f()
来源：http://eiu.havefunace.top

Ruby: Thread.new { f }
来源：http://zgq.zycfv.cn

C#:   Task.Run(() => F());
来源：http://gqw.nanxuanxn.top

[O02] 使用线程池
来源：http://kfq.andypj.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mrs.tian-w.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oyj.bbcook.cn

JS:   // worker_threads 线程池
来源：http://zyf.hfpthk.cn

TS:   // worker_threads 线程池
来源：http://nny.xingfuxueyuan.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://nfa.xingfuxueyuan.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nvo.xingfuxueyuan.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fih.hongshengwenyu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bkg.cucudq.cn

[O03] 加锁保护共享数据
来源：http://yvx.wangdashe.top

Py:   with lock: shared += 1
来源：http://qms.cheryme.top

PHP:  // 用 flock() 做文件锁
来源：http://pdq.feifeiyinyue.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wxg.yangfankeji.com

TS:   // 同 JS
来源：http://xxn.xuanzx.com

Java: synchronized (this) { shared++; }
来源：http://vfw.xuetiantiany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sqv.ppjwa.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ifs.ppjwa.cn

C#:   lock (gate) { shared++; }
来源：http://dfb.cqqwz.cn

[O04] 定义异步函数并等待
来源：http://ayj.smart0.xyz

Py:   async def f():⏎    await g()
来源：http://lvv.snrcjt.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qhw.shanyushiyangtech.top

JS:   async function f() { await g(); }
来源：http://frc.shanyushiyangtech.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://hue.yueranfly.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jea.tanke756.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rzz.jinghuilouyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://dal.hcnkem.com

C#:   async Task F() { await G(); }
来源：http://grk.nanxuanxn.top

[O05] 并发执行并等待全部完成
来源：http://ctb.jinyuanbaomall.cn

Py:   asyncio.gather(*tasks)
来源：http://wgg.chenlongwang.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fon.sxryk.cn

JS:   await Promise.all(tasks)
来源：http://mul.yvedp.cn

TS:   await Promise.all(tasks)
来源：http://pcb.shanyushiyangkeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fit.zhiwuduotai.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yrs.daria6918.cn

Ruby: threads.map(&:join)
来源：http://prr.ydzc1.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fch.cucudq.cn

[O06] 使用进程池
来源：http://bdp.nanxinkj.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xif.ydzc1.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ofi.yuxming.cn

JS:   // child_process / cluster 模块
来源：http://jvg.daria6918.cn


<!-- 参考信息 -->