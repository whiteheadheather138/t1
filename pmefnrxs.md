代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://qwr.hysaishi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ofu.chenzaomai.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xhf.zycfv.cn

JS:   resp.ok;  resp.status
来源：http://plb.zhixingplan.top

TS:   resp.ok;  resp.status
来源：http://mvi.dashuyun.cn

Java: resp.statusCode()
来源：http://tnc.ctjpmb.com

Go:   resp.StatusCode
来源：http://tbg.zycfv.cn

Ruby: resp.code.to_i
来源：http://jme.ehwqpu.com

C#:   (int)resp.StatusCode
来源：http://rxo.ppjwa.cn

[L08] 并发请求多个地址
来源：http://fvf.vqdsnc.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://swn.jlsjyb.cn

PHP:  curl_multi_init() 系列
来源：http://dtl.ybcxt.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rmk.ybcxt.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fnf.hysaishi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fkd.yueranfly.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zsk.ydjk.org.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tnh.c1oappe.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hph.jqgfzy.top

================================================================================
来源：http://nyz.shanyushiyangtech.top

M. 命令行 / 进程 / 环境
来源：http://rcp.wangshuangyany.cn

================================================================================
来源：http://bly.kuanghao11.cn

[M01] 读取命令行参数
来源：http://mri.chenlongwang.top

Py:   sys.argv[1:]
来源：http://act.sufxvd.cn

PHP:  $argv;  $argc;
来源：http://zpd.mhx1999.top

JS:   process.argv.slice(2)
来源：http://qxs.shanyushiyangkeji.top

TS:   process.argv.slice(2)
来源：http://kok.aibaodan.cn

Java: args 数组（main 方法参数）
来源：http://gmp.shuidangran.top

Go:   os.Args[1:]
来源：http://amk.yuanzhike.top

Ruby: ARGV
来源：http://tsf.nanxinkj.top

C#:   args 数组（Main 方法参数）
来源：http://fdq.jinyuanbaomall.cn

[M02] 读取环境变量
来源：http://xsn.yj20258888.top

Py:   os.environ.get("HOME")
来源：http://ben.jinyuanbaomall.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://htc.ydjk.org.cn

JS:   process.env.HOME
来源：http://fni.ybcxt.top

TS:   process.env.HOME
来源：http://zos.cheryme.top

Java: System.getenv("HOME")
来源：http://xzp.yuanzhike.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://urd.pycfn.com

Ruby: ENV["HOME"]
来源：http://uzq.hnqzz.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zpz.bjfxy.top

[M03] 执行外部命令
来源：http://zbq.zdqjudy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nkv.xuanzx.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ohz.redwolf501.top

JS:   child_process.execSync("ls -l").toString()
来源：http://iah.jinqigufen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ioc.gaohongyu789.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cih.yongpay.top

Go:   exec.Command("ls", "-l").Output()
来源：http://sdi.shanyushiyangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://czl.ydjk.org.cn

C#:   Process.Start("ls", "-l");
来源：http://lpa.ydjk.org.cn

[M04] 获取当前工作目录
来源：http://odc.dianchejie.cn

Py:   os.getcwd()
来源：http://dij.yuanzhike.top

PHP:  getcwd();
来源：http://vpc.meibo888.top

JS:   process.cwd()
来源：http://fyh.quarkkingdee.top

TS:   process.cwd()
来源：http://isp.yj202588.top

Java: Path.of("").toAbsolutePath()
来源：http://jpp.shanyushiyangtech.top

Go:   os.Getwd()
来源：http://hkg.ybcxt.top

Ruby: Dir.pwd
来源：http://tif.hnxiangtu.top

C#:   Directory.GetCurrentDirectory()
来源：http://aut.nwbrower.top

[M05] 设置退出码
来源：http://psf.chenlongwang.top

Py:   sys.exit(1)
来源：http://bbs.xziqi.cn

PHP:  exit(1);
来源：http://rxx.guowangkeji.top

JS:   process.exit(1)
来源：http://zla.zdbjq.cn

TS:   process.exit(1)
来源：http://mvc.jqgufenzy.top

Java: System.exit(1)
来源：http://sfc.hongshengwenyu.top

Go:   os.Exit(1)
来源：http://vor.bbcook.cn

Ruby: exit 1
来源：http://yow.ehwqpu.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dqt.tarul.cn

[M06] 向标准错误输出
来源：http://ixb.guowangkeji.top

Py:   print("err", file=sys.stderr)
来源：http://nud.yuanzhike.top

PHP:  fwrite(STDERR, "err\n");
来源：http://nyg.daxiang520.top

JS:   console.error("err")
来源：http://nds.jyoumei.cn

TS:   console.error("err")
来源：http://alq.yanxiufei.cn

Java: System.err.println("err")
来源：http://gdk.uphjek.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://spd.chenlongwang.top

Ruby: warn "err"
来源：http://baz.yanxiufei.cn

C#:   Console.Error.WriteLine("err")
来源：http://yog.chenlongwang.top

[M07] 判断是否为主入口
来源：http://mgl.aibaodan.cn

Py:   if __name__ == "__main__":
来源：http://ksg.fanxiaobao.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mru.nanxinkj.top

JS:   require.main === module
来源：http://rgj.zdqjudy.top

TS:   require.main === module
来源：http://iqn.zhongyouzk.top

Java: public static void main(String[] args)
来源：http://oog.wangshuangyany.cn

Go:   func main()
来源：http://vba.fzhhl.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ehn.tanke756.top

C#:   static void Main(string[] args)
来源：http://vmc.hywenlv.cn

[M08] 获取系统与运行时信息
来源：http://ick.jinqigufen.top

Py:   platform.system();  platform.python_version()
来源：http://wbt.wangdashe.top

PHP:  PHP_OS;  phpversion();
来源：http://hzc.zhongyouzk.top

JS:   process.platform;  process.version
来源：http://bnx.zdbjq.cn

TS:   process.platform;  process.version
来源：http://tkh.c1oappe.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ywg.guowangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://rng.yvedp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mzw.jinqigfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://gik.nwbrower.top

================================================================================
来源：http://yuk.guannengcc.top

N. 数据结构与算法
来源：http://otg.fanxiaobao.xyz

================================================================================
来源：http://fnp.zdbjq.cn

[N01] 二分查找（有序数组）
来源：http://gad.jinqigufen.top

Py:   bisect.bisect_left(arr, x)
来源：http://vma.epnwcf.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kky.nanxinkj.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vfq.bjfxy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xex.yuanzhike.top

Java: Arrays.binarySearch(arr, x)
来源：http://ega.yfazqb.com

Go:   sort.SearchInts(arr, x)
来源：http://nvw.vehdjk.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://fbd.gotoacloud.top

C#:   Array.BinarySearch(arr, x)
来源：http://jqm.daxiang520.top

[N02] 排序（工程实践用内置实现）
来源：http://kim.bjfxy.top

Py:   sorted(arr);  arr.sort()
来源：http://nor.meibo888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hsy.guannengcc.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://vlw.cqqwz.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://str.redwolf501.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uin.fengsongda.top

Go:   slices.Sort(arr)
来源：http://exi.jinghuilouyu.cn

Ruby: arr.sort
来源：http://pqf.gzhubu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ccs.c1oappe.top

[N03] 快速排序（分治示例）
来源：http://kkq.iojbl.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qrp.jyoumei.cn

PHP:  // 递归实现，或用 usort
来源：http://hqf.meibo888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sba.bbcook.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dgy.hesvh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mxx.nwbrower.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uso.pengpengdd.cyou

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fwc.shanyushiyangkeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://neo.fktsv.cn

[N04] 斐波那契数列
来源：http://ynr.yonumen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ptt.jinqigufen.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zgu.yangfankeji.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ffe.yangfankeji.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lpi.ydzc1.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gfh.yj202588.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nbc.mhx1999.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pur.vehdjk.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://elm.birdmap.top

[N05] 最大公约数
来源：http://fyx.smart0.xyz

Py:   math.gcd(a, b)
来源：http://gdj.0kj1m.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ocb.cqqwz.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wlq.xingfuxueyuan.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rng.zdqjudy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hre.cdnleiting.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wjf.xuetiantiany.cn

Ruby: a.gcd(b)
来源：http://soy.ctjpmb.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lvr.chenlongwang.top

[N06] 判断回文字符串
来源：http://bhc.tarul.cn

Py:   s == s[::-1]
来源：http://aip.gaohongyu789.top

PHP:  $s === strrev($s);
来源：http://bmt.cqqwz.cn

JS:   s === [...s].reverse().join("")
来源：http://imm.nwbrower.top

TS:   s === [...s].reverse().join("")
来源：http://sij.snrcjt.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ibr.hesvh.cn

Go:   // 双指针从两端比较
来源：http://onc.guannengcc.top

Ruby: s == s.reverse
来源：http://qmb.xylfe.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gbo.ppjwa.cn

[N07] 两数之和（返回下标）
来源：http://bpw.jianghu66.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ode.cqqwz.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://odh.andypj.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://zxj.pycfn.com

TS:   // 手写 Map<string, number>
来源：http://elv.jiagoushi.top

Java: // 手写 HashMap
来源：http://qub.zhiwuduotai.top

Go:   // 手写 map[int]int
来源：http://lxr.havefunace.top

Ruby: // 手写 Hash
来源：http://oim.xuanzx.com

C#:   // 手写 Dictionary<int, int>
来源：http://bhv.zhongyouzk.top

[N08] 生成全排列
来源：http://eec.bjfxy.top

Py:   itertools.permutations(arr)
来源：http://uuj.jinqigufen.top

PHP:  // 手写递归交换
来源：http://vgr.jlsjyb.cn

JS:   // 手写回溯递归
来源：http://vud.cashguo.top

TS:   // 手写回溯递归
来源：http://hht.uphjek.com

Java: // 手写回溯递归
来源：http://rbn.tian-w.cn

Go:   // 手写回溯递归
来源：http://pcn.epnwcf.com

Ruby: arr.permutation.to_a
来源：http://ujn.jinqigfzy.top

C#:   // 手写回溯递归
来源：http://met.aizwys.cn

[N09] 栈与队列
来源：http://rec.fzhhl.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fpp.bjfxy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yaz.haohaochexian.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vds.pengpengdd.cyou

TS:   arr.push(x) / arr.pop() 作栈
来源：http://knl.dashuyun.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://byp.shanyushiyangkeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hmk.fehbvm.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yoa.nanxuanxn.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qsv.snrcjt.cn

[N10] 链表节点定义
来源：http://idr.daria6918.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lrn.cucudq.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bgy.cashguo.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qxv.nwbrower.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://brv.zhiwuduotai.top

Java: class Node { int v; Node next; }
来源：http://ugf.shanyushiyangtech.top

Go:   type Node struct { V int; Next *Node }
来源：http://vab.feifeiyinyue.top

Ruby: Node = Struct.new(:v, :next)
来源：http://iwn.yj20258888.top

C#:   class Node { public int V; public Node? Next; }
来源：http://krn.gotoacloud.top

[N11] 二叉树中序遍历
来源：http://xbw.pengpengdd.cyou

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ero.zhiwuduotai.top

PHP:  // 手写递归函数
来源：http://dyx.fzhhl.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://myz.sysykeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cxt.jinyuanbaomall.cn

Java: // 手写递归
来源：http://tip.cqqwz.cn

Go:   // 手写递归
来源：http://ibm.zdbjq.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mcv.yongpay.top

C#:   // 手写递归
来源：http://rbd.pycfn.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nfy.zhengqikj.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uyi.zhixingplan.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qyy.316326.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gdm.yj202588.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gzg.9152youxi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://puz.jqgfzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blz.gzhubu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mkz.ehwqpu.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://eee.cheryme.top

================================================================================
来源：http://ezk.xingfuxueyuan.xyz

O. 并发与异步
来源：http://qvo.shuidangran.top

================================================================================
来源：http://gjn.snrcjt.cn

[O01] 启动一个线程
来源：http://fad.pycfn.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lej.fanxiaobao.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fae.hysaishi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bqd.daxiang520.top

TS:   // 同 JS
来源：http://gup.pengpengdd.cyou

Java: new Thread(() -> f()).start()
来源：http://bow.jqgfzy.top

Go:   go f()
来源：http://ivc.fengsongda.top

Ruby: Thread.new { f }
来源：http://won.zhengqikj.top

C#:   Task.Run(() => F());
来源：http://obm.fzhhl.top

[O02] 使用线程池
来源：http://uqy.xuetiantiany.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cqq.gotoacloud.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oxz.tanke756.top

JS:   // worker_threads 线程池
来源：http://xod.hesvh.cn

TS:   // worker_threads 线程池
来源：http://hsw.uphjek.com

Java: Executors.newFixedThreadPool(4)
来源：http://gro.zhengqikj.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tlw.bjfxy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jks.zhaomingkeji.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rtk.shanyushiyangtech.top

[O03] 加锁保护共享数据
来源：http://phz.pycfn.com

Py:   with lock: shared += 1
来源：http://blf.aizwys.cn

PHP:  // 用 flock() 做文件锁
来源：http://jgc.shanyushiyangtech.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hks.wangdashe.top

TS:   // 同 JS
来源：http://nfl.chenlongwang.top

Java: synchronized (this) { shared++; }
来源：http://wvj.shangyingyoupin.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cya.xinyue.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://bnu.shzxlz.cn

C#:   lock (gate) { shared++; }
来源：http://uit.tarul.cn

[O04] 定义异步函数并等待
来源：http://wvz.hcnkem.com

Py:   async def f():⏎    await g()
来源：http://eoe.hammf.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qfq.ydjk.org.cn

JS:   async function f() { await g(); }
来源：http://ixf.zhengqikj.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://cos.yfazqb.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lfe.hammf.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oky.fktsv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://std.hysaishi.cn

C#:   async Task F() { await G(); }
来源：http://xzy.pengpengdd.cyou

[O05] 并发执行并等待全部完成
来源：http://voj.fengsongda.top

Py:   asyncio.gather(*tasks)
来源：http://jtc.jyoumei.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xui.sjlbkw.cn

JS:   await Promise.all(tasks)
来源：http://xrz.ydjk.org.cn

TS:   await Promise.all(tasks)
来源：http://cow.zhixingplan.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lvs.vqdsnc.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vmx.yongpay.top

Ruby: threads.map(&:join)
来源：http://pui.hcnkem.com

C#:   await Task.WhenAll(t1, t2)
来源：http://otp.redwolf501.top

[O06] 使用进程池
来源：http://hdi.epnwcf.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://shw.zhiwuduotai.top

PHP:  // pcntl_fork 或多进程队列
来源：http://sjc.yanxiufei.cn

JS:   // child_process / cluster 模块
来源：http://niy.jyoumei.cn

TS:   // child_process / cluster 模块
来源：http://wph.ywan-chungtsiang.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rvg.shangyingyoupin.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jjy.nanxuanxn.top

Ruby: // fork 块
来源：http://hjr.shangyingyoupin.top

C#:   Parallel.For
来源：http://rui.vqdsnc.cn

================================================================================
来源：http://nrq.sufxvd.cn

P. 常用工具函数
来源：http://asj.yfazqb.com

================================================================================
来源：http://dkk.gaohongyu789.top

[P01] 生成 UUID
来源：http://oyu.jinqigfzy.top

Py:   str(uuid.uuid4())
来源：http://qhi.nanxinkj.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://orp.shuidangran.top

JS:   crypto.randomUUID()
来源：http://myf.zdqjudy.top

TS:   crypto.randomUUID()
来源：http://lyj.shanyushiyangtech.top

Java: UUID.randomUUID().toString()
来源：http://eme.quarkkingdee.top

Go:   // 用 github.com/google/uuid
来源：http://vqb.ybcxt.top

Ruby: SecureRandom.uuid
来源：http://mmo.uphjek.com

C#:   Guid.NewGuid().ToString()
来源：http://rxg.sxryk.cn

[P02] MD5 / SHA256 摘要
来源：http://zet.zdqjudy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vji.uphjek.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://ukm.xuetiantiany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rze.chenjidiqi.icu

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dwm.tian-w.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vif.tian-w.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cmk.snrcjt.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ihg.yanxiufei.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bbm.jianghu66.top

[P03] 生成短随机字符串
来源：http://avv.xinyue.icu

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://emv.wangdashe.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yru.shuidangran.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jil.hongshengwenyu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cab.zhiwuduotai.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fez.cheryme.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dcx.uphjek.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://yoy.316326.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qci.52xcode.cn

[P04] 求长度
来源：http://ekr.yuxming.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qgu.ivvv.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://reo.haohaochexian.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hut.sxryk.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cgt.yfazqb.com

Java: list.size();  map.size();  s.length()
来源：http://joa.zdbjq.cn

Go:   len(arr);  len(m)
来源：http://thg.cheryme.top

Ruby: x.length;  x.size
来源：http://hjm.sysykeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://mrc.fanxiaobao.xyz


<!-- 参考信息 -->