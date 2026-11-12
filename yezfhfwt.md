代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yel.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fkp.ywan-chungtsiang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iry.xuanzx.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zlg.shzxlz.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tef.zhixingplan.top

[L04] 设置超时
来源：http://bti.jianghu66.top

Py:   requests.get(url, timeout=5)
来源：http://ogt.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mxh.redwolf501.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sag.cucudq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kfh.dashuyun.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pkl.zhaomingkeji.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wki.gaohongyu789.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zcq.0kj1m.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ndt.xuetiantiany.cn

[L05] 上传文件（multipart）
来源：http://pqm.guannengcc.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cdj.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zqd.sxryk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hsl.xinyue.icu

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jaw.yvedp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oxw.cqqwz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ygb.vqdsnc.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xzl.316326.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://frl.zhaomingkeji.xyz

[L06] 解析响应为 JSON
来源：http://rhq.bbcook.cn

Py:   resp.json()
来源：http://vwy.fzhhl.top

PHP:  json_decode($body, true);
来源：http://pgy.yuanzhike.top

JS:   await resp.json()
来源：http://pds.guannengcc.top

TS:   await resp.json()
来源：http://bwo.shzxlz.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://owt.ywan-chungtsiang.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zsb.cqqwz.cn

Ruby: JSON.parse(resp.body)
来源：http://dez.nanxuanxn.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mgd.hesvh.cn

[L07] 处理 HTTP 状态码
来源：http://whe.yj20258.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qce.svipenyu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hnt.fktsv.cn

JS:   resp.ok;  resp.status
来源：http://hab.hesvh.cn

TS:   resp.ok;  resp.status
来源：http://quc.ydzc1.top

Java: resp.statusCode()
来源：http://xgb.shangyingyoupin.top

Go:   resp.StatusCode
来源：http://uit.jyoumei.cn

Ruby: resp.code.to_i
来源：http://acl.9152youxi.cn

C#:   (int)resp.StatusCode
来源：http://lso.yangfankeji.com

[L08] 并发请求多个地址
来源：http://gep.gogol.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zem.ydjk.org.cn

PHP:  curl_multi_init() 系列
来源：http://tcz.yvedp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ykc.haohaochexian.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kmm.fengsongda.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hbt.ydzc1.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://iyo.yuanzhike.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://trg.0kj1m.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pez.nanxuanxn.top

================================================================================
来源：http://tlz.zhijiandao.cn

M. 命令行 / 进程 / 环境
来源：http://abx.hnqzz.top

================================================================================
来源：http://ruw.chenjidiqi.icu

[M01] 读取命令行参数
来源：http://cxg.yueranfly.top

Py:   sys.argv[1:]
来源：http://cvv.andypj.xyz

PHP:  $argv;  $argc;
来源：http://soq.yj20258.top

JS:   process.argv.slice(2)
来源：http://hhr.sufxvd.cn

TS:   process.argv.slice(2)
来源：http://fda.sweek.top

Java: args 数组（main 方法参数）
来源：http://xwq.nwbrower.top

Go:   os.Args[1:]
来源：http://zxi.guowangkeji.top

Ruby: ARGV
来源：http://yfk.ydzc1.top

C#:   args 数组（Main 方法参数）
来源：http://ikv.hnqzz.top

[M02] 读取环境变量
来源：http://agx.zycfv.cn

Py:   os.environ.get("HOME")
来源：http://wci.daria6918.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wnh.hnqzz.top

JS:   process.env.HOME
来源：http://nsl.gzhubu.top

TS:   process.env.HOME
来源：http://gtp.zhaomingkeji.xyz

Java: System.getenv("HOME")
来源：http://iye.fanxiaobao.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://aas.gaohongyu789.top

Ruby: ENV["HOME"]
来源：http://ujz.yanxiufei.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fxs.52xcode.cn

[M03] 执行外部命令
来源：http://kcr.zdqjudy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ayp.zhongyouzk.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vcl.9152youxi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bsh.yueranfly.top

TS:   child_process.execSync("ls -l").toString()
来源：http://nud.fehbvm.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sdh.zdbjq.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://twr.zhoulong.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://odr.xylfe.cn

C#:   Process.Start("ls", "-l");
来源：http://aoh.ywan-chungtsiang.top

[M04] 获取当前工作目录
来源：http://tip.yueranfly.top

Py:   os.getcwd()
来源：http://jpq.xuetiantiany.cn

PHP:  getcwd();
来源：http://jpu.sweek.top

JS:   process.cwd()
来源：http://hwg.cqqwz.cn

TS:   process.cwd()
来源：http://vsb.nanxinkj.top

Java: Path.of("").toAbsolutePath()
来源：http://eon.haohaochexian.top

Go:   os.Getwd()
来源：http://ppf.xinyue.icu

Ruby: Dir.pwd
来源：http://osd.andypj.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://lnl.ydzc1.top

[M05] 设置退出码
来源：http://kfe.zdbjq.cn

Py:   sys.exit(1)
来源：http://ezc.havefunace.top

PHP:  exit(1);
来源：http://klz.shzxlz.cn

JS:   process.exit(1)
来源：http://svl.hcnkem.com

TS:   process.exit(1)
来源：http://dbf.chenlongwang.top

Java: System.exit(1)
来源：http://qso.jqgfzy.top

Go:   os.Exit(1)
来源：http://dts.zhijiandao.cn

Ruby: exit 1
来源：http://ydf.zycfv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lui.fktsv.cn

[M06] 向标准错误输出
来源：http://koj.xinyue.icu

Py:   print("err", file=sys.stderr)
来源：http://tyk.9152youxi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nzk.chenlongwang.top

JS:   console.error("err")
来源：http://uhk.yuxming.cn

TS:   console.error("err")
来源：http://nol.jyoumei.cn

Java: System.err.println("err")
来源：http://ved.ivvv.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ade.jqgfzy.top

Ruby: warn "err"
来源：http://luu.aibaodan.cn

C#:   Console.Error.WriteLine("err")
来源：http://vfm.vqdsnc.cn

[M07] 判断是否为主入口
来源：http://iwy.aibaodan.cn

Py:   if __name__ == "__main__":
来源：http://lhq.daxiang520.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jsw.ctjpmb.com

JS:   require.main === module
来源：http://yrm.pengpengdd.cyou

TS:   require.main === module
来源：http://sci.fanxiaobao.xyz

Java: public static void main(String[] args)
来源：http://oay.daria6918.cn

Go:   func main()
来源：http://hfp.vqdsnc.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mmp.0kj1m.cn

C#:   static void Main(string[] args)
来源：http://guk.yj202588.top

[M08] 获取系统与运行时信息
来源：http://mmu.tianlin.xyz

Py:   platform.system();  platform.python_version()
来源：http://ztp.nanxinkj.top

PHP:  PHP_OS;  phpversion();
来源：http://pkh.sjlbkw.cn

JS:   process.platform;  process.version
来源：http://eqo.nanxinkj.top

TS:   process.platform;  process.version
来源：http://ovq.cqqwz.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rnq.zhongyouzk.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://krb.smart0.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lmm.jinghuilouyu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pgm.epnwcf.com

================================================================================
来源：http://ppn.ppjwa.cn

N. 数据结构与算法
来源：http://jlb.shangyingyoupin.top

================================================================================
来源：http://zwv.tian-w.cn

[N01] 二分查找（有序数组）
来源：http://ohu.sjlbkw.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kyh.jinqigufen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gpp.yonumen.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lqz.yangfankeji.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://loy.cdnleiting.top

Java: Arrays.binarySearch(arr, x)
来源：http://ljo.fzhhl.top

Go:   sort.SearchInts(arr, x)
来源：http://thf.iojbl.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kbi.hywenlv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mas.pycfn.com

[N02] 排序（工程实践用内置实现）
来源：http://zcn.jinqigfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://qjc.zdqjudy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vas.wangshuangyany.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jgu.fehbvm.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://amb.hesvh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rdn.zhaomingkeji.xyz

Go:   slices.Sort(arr)
来源：http://mab.yuxming.cn

Ruby: arr.sort
来源：http://enf.haohaochexian.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://wib.fengsongda.top

[N03] 快速排序（分治示例）
来源：http://mxr.svipenyu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zef.fanxiaobao.xyz

PHP:  // 递归实现，或用 usort
来源：http://suc.sjlbkw.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://otj.ehwqpu.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yaf.zhongyouzk.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tjx.ctjpmb.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qva.chenlongwang.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pdw.fehbvm.com

C#:   // 手写递归，或 Array.Sort
来源：http://pod.snrcjt.cn

[N04] 斐波那契数列
来源：http://ocd.haohaochexian.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ueo.sxryk.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rzu.yj20258888.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ryl.xingfuxueyuan.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wxq.ywan-chungtsiang.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yhr.zhiwuduotai.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://utp.hysaishi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tqy.yj20258888.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jff.gzhubu.top

[N05] 最大公约数
来源：http://yti.hongshengwenyu.top

Py:   math.gcd(a, b)
来源：http://ibq.jiagoushi.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://loe.aizwys.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hkq.yonumen.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nfx.hnxiangtu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://smv.dianchejie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xsp.pengpengdd.cyou

Ruby: a.gcd(b)
来源：http://ykc.hcnkem.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jck.zhijiandao.cn

[N06] 判断回文字符串
来源：http://fra.yj202588.top

Py:   s == s[::-1]
来源：http://wjp.svipenyu.cn

PHP:  $s === strrev($s);
来源：http://xyo.shzxlz.cn

JS:   s === [...s].reverse().join("")
来源：http://opi.shzxlz.cn

TS:   s === [...s].reverse().join("")
来源：http://too.feifeiyinyue.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xpy.hfpthk.cn

Go:   // 双指针从两端比较
来源：http://nxj.dashuyun.cn

Ruby: s == s.reverse
来源：http://cck.yj202588.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://nop.kuanghao11.cn

[N07] 两数之和（返回下标）
来源：http://kez.zycfv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mib.ivvv.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://smt.tian-w.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://nye.xuanzx.com

TS:   // 手写 Map<string, number>
来源：http://efx.bjfxy.top

Java: // 手写 HashMap
来源：http://fcs.316326.xyz

Go:   // 手写 map[int]int
来源：http://idf.316326.xyz

Ruby: // 手写 Hash
来源：http://swc.hysaishi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://end.dashuyun.cn

[N08] 生成全排列
来源：http://flr.chenzaomai.com

Py:   itertools.permutations(arr)
来源：http://qxa.jianghu66.top

PHP:  // 手写递归交换
来源：http://isq.sjlbkw.cn

JS:   // 手写回溯递归
来源：http://evo.zhixingplan.top

TS:   // 手写回溯递归
来源：http://byw.mhx1999.top

Java: // 手写回溯递归
来源：http://ajr.yanxiufei.cn

Go:   // 手写回溯递归
来源：http://xjd.daria6918.cn

Ruby: arr.permutation.to_a
来源：http://rcu.pycfn.com

C#:   // 手写回溯递归
来源：http://vfk.hesvh.cn

[N09] 栈与队列
来源：http://hng.tarul.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qxz.aibaodan.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nqm.xuetiantiany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fpw.guowangkeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dve.andypj.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kit.sufxvd.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xcu.9152youxi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dpw.52xcode.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dhm.shuidangran.top

[N10] 链表节点定义
来源：http://pof.jinqigfzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nsa.sjlbkw.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yfs.aizwys.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://snx.shanyushiyangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jdy.jinqigfzy.top

Java: class Node { int v; Node next; }
来源：http://nsl.cdnleiting.top

Go:   type Node struct { V int; Next *Node }
来源：http://hdb.jianghu66.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zif.cdnleiting.top

C#:   class Node { public int V; public Node? Next; }
来源：http://uzr.yuxming.cn

[N11] 二叉树中序遍历
来源：http://xpb.gaohongyu789.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tej.jyoumei.cn

PHP:  // 手写递归函数
来源：http://alr.nanxuanxn.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vsv.ehwqpu.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gjx.pycfn.com

Java: // 手写递归
来源：http://zdi.sjlbkw.cn

Go:   // 手写递归
来源：http://vgu.smart0.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kml.daria6918.cn

C#:   // 手写递归
来源：http://pxo.shangyingyoupin.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ihr.redwolf501.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://czc.chenjidiqi.icu

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ekl.chenjidiqi.icu

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://auo.jinyuanbaomall.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dzl.snrcjt.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yif.epnwcf.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kwy.zhongyouzk.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mio.yj202588.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lce.nwbrower.top

================================================================================
来源：http://ozj.zdbjq.cn

O. 并发与异步
来源：http://uuh.zycfv.cn

================================================================================
来源：http://hiz.kuanghao11.cn

[O01] 启动一个线程
来源：http://kkj.fzhhl.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ycz.haohaochexian.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://loe.yvedp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ryc.wangshuangyany.cn

TS:   // 同 JS
来源：http://jft.xinyue.icu

Java: new Thread(() -> f()).start()
来源：http://pjl.epnwcf.com

Go:   go f()
来源：http://jcx.c1oappe.top

Ruby: Thread.new { f }
来源：http://hmm.dianchejie.cn

C#:   Task.Run(() => F());
来源：http://zcx.haohaochexian.top

[O02] 使用线程池
来源：http://ssx.xziqi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cnr.xylfe.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vlr.cashguo.top

JS:   // worker_threads 线程池
来源：http://tpc.jiagoushi.top

TS:   // worker_threads 线程池
来源：http://upi.cucudq.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rtt.fehbvm.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cwd.daxiang520.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ldh.jianghu66.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rqf.kuanghao11.cn

[O03] 加锁保护共享数据
来源：http://bun.kuanghao11.cn

Py:   with lock: shared += 1
来源：http://sdu.zhixingplan.top

PHP:  // 用 flock() 做文件锁
来源：http://dct.guowangkeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jrb.cqqwz.cn

TS:   // 同 JS
来源：http://lmr.sxryk.cn

Java: synchronized (this) { shared++; }
来源：http://cxw.yanxiufei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ytm.tarul.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jck.daxiang520.top

C#:   lock (gate) { shared++; }
来源：http://tve.zhoulong.xyz

[O04] 定义异步函数并等待
来源：http://sjk.zhixingplan.top

Py:   async def f():⏎    await g()
来源：http://rol.zhoulong.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ijm.xziqi.cn

JS:   async function f() { await g(); }
来源：http://ure.xylfe.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ysf.fanxiaobao.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ahr.vqdsnc.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://elc.jlsjyb.cn

Ruby: # 用 Fiber 或 async gem
来源：http://uwm.ppjwa.cn

C#:   async Task F() { await G(); }
来源：http://czh.zycfv.cn

[O05] 并发执行并等待全部完成
来源：http://cnf.chenzaomai.com

Py:   asyncio.gather(*tasks)
来源：http://opj.andypj.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ulq.aizwys.cn

JS:   await Promise.all(tasks)
来源：http://kwi.daxiang520.top

TS:   await Promise.all(tasks)
来源：http://jup.chenjidiqi.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://crq.yj20258.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pbz.birdmap.top

Ruby: threads.map(&:join)
来源：http://clp.yuxming.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xwu.havefunace.top

[O06] 使用进程池
来源：http://lxj.bbcook.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sgx.fanxiaobao.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://mpn.snrcjt.cn

JS:   // child_process / cluster 模块
来源：http://ozs.sjlbkw.cn

TS:   // child_process / cluster 模块
来源：http://hkr.vqdsnc.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://iza.cashguo.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nms.yj20258.top

Ruby: // fork 块
来源：http://cfr.mhx1999.top

C#:   Parallel.For
来源：http://plz.nwbrower.top

================================================================================
来源：http://sgf.yj20258.top

P. 常用工具函数
来源：http://eaw.haohaochexian.top

================================================================================
来源：http://lcr.vehdjk.com

[P01] 生成 UUID
来源：http://isi.ybcxt.top

Py:   str(uuid.uuid4())
来源：http://xds.shuidangran.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sbq.zhaomingkeji.xyz

JS:   crypto.randomUUID()
来源：http://ngy.ybcxt.top


<!-- 参考信息 -->