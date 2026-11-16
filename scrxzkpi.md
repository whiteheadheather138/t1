代发 wailian999

Py:   resp.json()
来源：http://lqh.zhoulong.xyz

PHP:  json_decode($body, true);
来源：http://rwc.ivvv.top

JS:   await resp.json()
来源：http://xpn.tian-w.cn

TS:   await resp.json()
来源：http://ezr.daxiang520.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tzs.fzhhl.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xig.yj20258888.top

Ruby: JSON.parse(resp.body)
来源：http://wnf.dashuyun.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mmw.jqgfzy.top

[L07] 处理 HTTP 状态码
来源：http://cih.zhijiandao.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hgn.pycfn.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dnt.yanxiufei.cn

JS:   resp.ok;  resp.status
来源：http://hdj.vqdsnc.cn

TS:   resp.ok;  resp.status
来源：http://wac.fanxiaobao.xyz

Java: resp.statusCode()
来源：http://opl.fanxiaobao.xyz

Go:   resp.StatusCode
来源：http://xpv.kuanghao11.cn

Ruby: resp.code.to_i
来源：http://ajt.guannengcc.top

C#:   (int)resp.StatusCode
来源：http://ivx.wangshuangyany.cn

[L08] 并发请求多个地址
来源：http://jin.chenzaomai.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://het.jinghuilouyu.cn

PHP:  curl_multi_init() 系列
来源：http://myz.yangfankeji.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nft.hfpthk.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wnt.yueranfly.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kcq.zhongyouzk.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lss.havefunace.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cij.gotoacloud.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kae.sjlbkw.cn

================================================================================
来源：http://bwd.jinghuilouyu.cn

M. 命令行 / 进程 / 环境
来源：http://pcd.yj20258.top

================================================================================
来源：http://mnb.jqgufenzy.top

[M01] 读取命令行参数
来源：http://hfq.yj20258.top

Py:   sys.argv[1:]
来源：http://ula.zhijiandao.cn

PHP:  $argv;  $argc;
来源：http://rmj.feifeiyinyue.top

JS:   process.argv.slice(2)
来源：http://vst.fehbvm.com

TS:   process.argv.slice(2)
来源：http://nvv.zhoulong.xyz

Java: args 数组（main 方法参数）
来源：http://oot.shangyingyoupin.top

Go:   os.Args[1:]
来源：http://wgn.gzhubu.top

Ruby: ARGV
来源：http://hac.yj20258.top

C#:   args 数组（Main 方法参数）
来源：http://wtc.52xcode.cn

[M02] 读取环境变量
来源：http://rjk.chenjidiqi.icu

Py:   os.environ.get("HOME")
来源：http://dzz.jqgufenzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xvo.cashguo.top

JS:   process.env.HOME
来源：http://fhp.pengpengdd.cyou

TS:   process.env.HOME
来源：http://fdq.sufxvd.cn

Java: System.getenv("HOME")
来源：http://yeo.jyoumei.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yll.quarkkingdee.top

Ruby: ENV["HOME"]
来源：http://kkb.svipenyu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jzk.chenzaomai.com

[M03] 执行外部命令
来源：http://sil.shuidangran.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gic.jianghu66.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yqw.yfazqb.com

JS:   child_process.execSync("ls -l").toString()
来源：http://xkx.dianchejie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://slx.uphjek.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ztt.yj20258888.top

Go:   exec.Command("ls", "-l").Output()
来源：http://bgb.bbcook.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wut.52xcode.cn

C#:   Process.Start("ls", "-l");
来源：http://keb.9152youxi.cn

[M04] 获取当前工作目录
来源：http://zyi.gotoacloud.top

Py:   os.getcwd()
来源：http://gjv.jiagoushi.top

PHP:  getcwd();
来源：http://lgl.cqqwz.cn

JS:   process.cwd()
来源：http://zdt.0kj1m.cn

TS:   process.cwd()
来源：http://kvt.yueranfly.top

Java: Path.of("").toAbsolutePath()
来源：http://vap.jqgufenzy.top

Go:   os.Getwd()
来源：http://dbc.yangfankeji.com

Ruby: Dir.pwd
来源：http://jpf.kuanghao11.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vdl.ppjwa.cn

[M05] 设置退出码
来源：http://fzs.zhiwuduotai.top

Py:   sys.exit(1)
来源：http://ios.fktsv.cn

PHP:  exit(1);
来源：http://vlb.gotoacloud.top

JS:   process.exit(1)
来源：http://pig.chenlongwang.top

TS:   process.exit(1)
来源：http://snk.hongshengwenyu.top

Java: System.exit(1)
来源：http://fkh.c1oappe.top

Go:   os.Exit(1)
来源：http://xgy.jinyuanbaomall.cn

Ruby: exit 1
来源：http://rgm.xziqi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://boz.uphjek.com

[M06] 向标准错误输出
来源：http://brb.meibo888.top

Py:   print("err", file=sys.stderr)
来源：http://iha.zhongyouzk.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gbg.sysykeji.top

JS:   console.error("err")
来源：http://cdp.zdqjudy.top

TS:   console.error("err")
来源：http://dwp.mhx1999.top

Java: System.err.println("err")
来源：http://bme.pengpengdd.cyou

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wkd.shanyushiyangkeji.top

Ruby: warn "err"
来源：http://xmf.iojbl.cn

C#:   Console.Error.WriteLine("err")
来源：http://cwg.hnxiangtu.top

[M07] 判断是否为主入口
来源：http://oly.tanke756.top

Py:   if __name__ == "__main__":
来源：http://ugg.ehwqpu.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://frc.xziqi.cn

JS:   require.main === module
来源：http://rzq.yongpay.top

TS:   require.main === module
来源：http://tso.ehwqpu.com

Java: public static void main(String[] args)
来源：http://czd.jiagoushi.top

Go:   func main()
来源：http://cbk.vqdsnc.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rgq.vehdjk.com

C#:   static void Main(string[] args)
来源：http://xem.shangyingyoupin.top

[M08] 获取系统与运行时信息
来源：http://qaq.tianlin.xyz

Py:   platform.system();  platform.python_version()
来源：http://vke.c1oappe.top

PHP:  PHP_OS;  phpversion();
来源：http://gpc.xuetiantiany.cn

JS:   process.platform;  process.version
来源：http://lxj.fehbvm.com

TS:   process.platform;  process.version
来源：http://qmz.smart0.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rtv.feifeiyinyue.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://exn.fanxiaobao.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://svy.dashuyun.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://twc.ehwqpu.com

================================================================================
来源：http://iyx.zhengqikj.top

N. 数据结构与算法
来源：http://qvl.fzhhl.top

================================================================================
来源：http://obf.cheryme.top

[N01] 二分查找（有序数组）
来源：http://soj.quarkkingdee.top

Py:   bisect.bisect_left(arr, x)
来源：http://eln.zhijiandao.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://moy.wangdashe.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fsz.yj202588.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tkf.9152youxi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ygf.cucudq.cn

Go:   sort.SearchInts(arr, x)
来源：http://ifr.bbcook.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tib.snrcjt.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uds.c1oappe.top

[N02] 排序（工程实践用内置实现）
来源：http://fod.wangshuangyany.cn

Py:   sorted(arr);  arr.sort()
来源：http://mtt.dianchejie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://uja.hfpthk.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cyw.ehwqpu.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://pop.aibaodan.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jsw.pengpengdd.cyou

Go:   slices.Sort(arr)
来源：http://kcs.jlsjyb.cn

Ruby: arr.sort
来源：http://jmz.zdqjudy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://upb.hysaishi.cn

[N03] 快速排序（分治示例）
来源：http://fhj.yj202588.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://upg.zhoulong.xyz

PHP:  // 递归实现，或用 usort
来源：http://fri.xinyue.icu

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qui.jqgufenzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zec.cashguo.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://luy.havefunace.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xra.nanxuanxn.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mks.iojbl.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rqo.ydjk.org.cn

[N04] 斐波那契数列
来源：http://cii.shanyushiyangtech.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cza.fzhhl.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://drv.0kj1m.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lrd.yonumen.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wlz.zdbjq.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dxp.52xcode.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jgj.zhixingplan.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://txa.sufxvd.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eks.smart0.xyz

[N05] 最大公约数
来源：http://mkg.wangdashe.top

Py:   math.gcd(a, b)
来源：http://lea.316326.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lzs.ywan-chungtsiang.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jta.daxiang520.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fwi.shzxlz.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bzs.yuanzhike.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://via.ydjk.org.cn

Ruby: a.gcd(b)
来源：http://sui.aibaodan.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mjq.birdmap.top

[N06] 判断回文字符串
来源：http://wtc.jiagoushi.top

Py:   s == s[::-1]
来源：http://dxt.tian-w.cn

PHP:  $s === strrev($s);
来源：http://iyw.cheryme.top

JS:   s === [...s].reverse().join("")
来源：http://vrc.daxiang520.top

TS:   s === [...s].reverse().join("")
来源：http://bcx.sjlbkw.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://flq.redwolf501.top

Go:   // 双指针从两端比较
来源：http://wxw.gaohongyu789.top

Ruby: s == s.reverse
来源：http://hfy.daria6918.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kpi.jinqigufen.top

[N07] 两数之和（返回下标）
来源：http://xjn.ehwqpu.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hoi.xingfuxueyuan.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ein.gotoacloud.top

JS:   // 手写 Map：map.set(v, i)
来源：http://dfm.yvedp.cn

TS:   // 手写 Map<string, number>
来源：http://mec.zhengqikj.top

Java: // 手写 HashMap
来源：http://dmm.chenlongwang.top

Go:   // 手写 map[int]int
来源：http://qud.vehdjk.com

Ruby: // 手写 Hash
来源：http://ofy.sysykeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://fmp.smart0.xyz

[N08] 生成全排列
来源：http://ouv.yj202588.top

Py:   itertools.permutations(arr)
来源：http://isw.fehbvm.com

PHP:  // 手写递归交换
来源：http://skn.havefunace.top

JS:   // 手写回溯递归
来源：http://tse.svipenyu.cn

TS:   // 手写回溯递归
来源：http://kxg.cdnleiting.top

Java: // 手写回溯递归
来源：http://hij.daria6918.cn

Go:   // 手写回溯递归
来源：http://ppq.jinqigfzy.top

Ruby: arr.permutation.to_a
来源：http://igz.jinyuanbaomall.cn

C#:   // 手写回溯递归
来源：http://ehs.fehbvm.com

[N09] 栈与队列
来源：http://yno.zhijiandao.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ynr.yj202588.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fiu.sweek.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yhe.dashuyun.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kef.fktsv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kny.aibaodan.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://twc.ybcxt.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jwi.dashuyun.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yyv.hammf.cn

[N10] 链表节点定义
来源：http://nwx.fzhhl.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jmi.cqqwz.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vzc.shanyushiyangkeji.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fpw.aizwys.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://smu.jinqigfzy.top

Java: class Node { int v; Node next; }
来源：http://otv.sufxvd.cn

Go:   type Node struct { V int; Next *Node }
来源：http://yzo.shangyingyoupin.top

Ruby: Node = Struct.new(:v, :next)
来源：http://vof.jinyuanbaomall.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vpi.jlsjyb.cn

[N11] 二叉树中序遍历
来源：http://auq.zhixingplan.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lar.bbcook.cn

PHP:  // 手写递归函数
来源：http://tuu.quarkkingdee.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pwf.daria6918.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nia.yj20258.top

Java: // 手写递归
来源：http://snr.ydzc1.top

Go:   // 手写递归
来源：http://gcu.yuanzhike.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wms.kuanghao11.cn

C#:   // 手写递归
来源：http://fvf.yonumen.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kmk.ctjpmb.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://skn.guannengcc.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yyb.hnxiangtu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qoi.yfazqb.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jvq.epnwcf.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gwc.jiagoushi.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sho.pycfn.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dzo.hysaishi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uzy.fzhhl.top

================================================================================
来源：http://tye.daxiang520.top

O. 并发与异步
来源：http://efr.wangdashe.top

================================================================================
来源：http://bly.yvedp.cn

[O01] 启动一个线程
来源：http://zay.nanxinkj.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vgj.zhongyouzk.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gvw.uphjek.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://eyc.nanxinkj.top

TS:   // 同 JS
来源：http://jno.zhiwuduotai.top

Java: new Thread(() -> f()).start()
来源：http://gci.cashguo.top

Go:   go f()
来源：http://ali.uphjek.com

Ruby: Thread.new { f }
来源：http://nqp.yj20258888.top

C#:   Task.Run(() => F());
来源：http://din.wangshuangyany.cn

[O02] 使用线程池
来源：http://sjy.52xcode.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mpb.dashuyun.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lko.zhengqikj.top

JS:   // worker_threads 线程池
来源：http://fyp.ivvv.top

TS:   // worker_threads 线程池
来源：http://cob.yuxming.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xgn.uphjek.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ymu.ybcxt.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ksu.gotoacloud.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ngx.zdbjq.cn

[O03] 加锁保护共享数据
来源：http://yca.0kj1m.cn

Py:   with lock: shared += 1
来源：http://sao.316326.xyz

PHP:  // 用 flock() 做文件锁
来源：http://hes.zhaomingkeji.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wot.tanke756.top

TS:   // 同 JS
来源：http://juq.xinyue.icu

Java: synchronized (this) { shared++; }
来源：http://flc.hammf.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pgn.zhaomingkeji.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://cdi.meibo888.top

C#:   lock (gate) { shared++; }
来源：http://pez.zhiwuduotai.top

[O04] 定义异步函数并等待
来源：http://kds.zhaomingkeji.xyz

Py:   async def f():⏎    await g()
来源：http://ffp.ydzc1.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ldj.redwolf501.top

JS:   async function f() { await g(); }
来源：http://yfp.shzxlz.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vnn.daxiang520.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cae.tarul.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sjc.guannengcc.top

Ruby: # 用 Fiber 或 async gem
来源：http://boj.vqdsnc.cn

C#:   async Task F() { await G(); }
来源：http://rqk.zhijiandao.cn

[O05] 并发执行并等待全部完成
来源：http://dyu.iojbl.cn

Py:   asyncio.gather(*tasks)
来源：http://iiz.cheryme.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://urr.dashuyun.cn

JS:   await Promise.all(tasks)
来源：http://dta.daria6918.cn

TS:   await Promise.all(tasks)
来源：http://lxy.wangdashe.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://spn.yonumen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pbs.316326.xyz

Ruby: threads.map(&:join)
来源：http://zjb.jqgufenzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mpr.yanxiufei.cn

[O06] 使用进程池
来源：http://xqn.cashguo.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jgi.pycfn.com

PHP:  // pcntl_fork 或多进程队列
来源：http://oor.chenjidiqi.icu

JS:   // child_process / cluster 模块
来源：http://luu.chenzaomai.com

TS:   // child_process / cluster 模块
来源：http://gbm.zhongyouzk.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jzf.ivvv.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://unc.zhoulong.xyz

Ruby: // fork 块
来源：http://aoj.zhijiandao.cn

C#:   Parallel.For
来源：http://wdo.jyoumei.cn

================================================================================
来源：http://xku.jqgufenzy.top

P. 常用工具函数
来源：http://bfy.yj20258.top

================================================================================
来源：http://xdd.havefunace.top

[P01] 生成 UUID
来源：http://kfs.jqgfzy.top

Py:   str(uuid.uuid4())
来源：http://dga.guannengcc.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tvw.haohaochexian.top

JS:   crypto.randomUUID()
来源：http://qlh.ywan-chungtsiang.top

TS:   crypto.randomUUID()
来源：http://gpx.aizwys.cn

Java: UUID.randomUUID().toString()
来源：http://pdt.yueranfly.top

Go:   // 用 github.com/google/uuid
来源：http://jtr.zhiwuduotai.top

Ruby: SecureRandom.uuid
来源：http://zgx.bjfxy.top

C#:   Guid.NewGuid().ToString()
来源：http://dtu.fzhhl.top

[P02] MD5 / SHA256 摘要
来源：http://exp.nwbrower.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ykj.fktsv.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tlw.hesvh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qek.hcnkem.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rip.dianchejie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vlq.jqgufenzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zdl.hnxiangtu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gqh.xylfe.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fpo.meibo888.top

[P03] 生成短随机字符串
来源：http://gyf.gzhubu.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rse.dianchejie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://aqj.jianghu66.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://itc.52xcode.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dbw.tianlin.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xnp.ppjwa.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zgd.yongpay.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://qbs.pycfn.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://krz.tanke756.top

[P04] 求长度
来源：http://aaj.yueranfly.top


<!-- 参考信息 -->