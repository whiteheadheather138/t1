代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wox.svipenyu.cn

JS:   process.env.HOME
来源：http://bne.vehdjk.com

TS:   process.env.HOME
来源：http://qvt.gzhubu.top

Java: System.getenv("HOME")
来源：http://dyc.sjlbkw.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qvn.daxiang520.top

Ruby: ENV["HOME"]
来源：http://doa.hysaishi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zrn.jiagoushi.top

[M03] 执行外部命令
来源：http://kra.jinqigufen.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dzj.fehbvm.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://chp.nwbrower.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vmc.shangyingyoupin.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bcp.sxryk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lgt.iojbl.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zuy.cheryme.top

Ruby: system("ls -l");  `ls -l`
来源：http://wau.aizwys.cn

C#:   Process.Start("ls", "-l");
来源：http://qqq.iojbl.cn

[M04] 获取当前工作目录
来源：http://grf.zycfv.cn

Py:   os.getcwd()
来源：http://hqj.nwbrower.top

PHP:  getcwd();
来源：http://kau.jinqigfzy.top

JS:   process.cwd()
来源：http://bbi.daria6918.cn

TS:   process.cwd()
来源：http://xgp.bbcook.cn

Java: Path.of("").toAbsolutePath()
来源：http://toy.jiagoushi.top

Go:   os.Getwd()
来源：http://nib.sysykeji.top

Ruby: Dir.pwd
来源：http://pdp.vehdjk.com

C#:   Directory.GetCurrentDirectory()
来源：http://xpb.jyoumei.cn

[M05] 设置退出码
来源：http://map.zhengqikj.top

Py:   sys.exit(1)
来源：http://cib.daria6918.cn

PHP:  exit(1);
来源：http://ucw.zdbjq.cn

JS:   process.exit(1)
来源：http://sbw.zdqjudy.top

TS:   process.exit(1)
来源：http://qmh.redwolf501.top

Java: System.exit(1)
来源：http://zeu.ybcxt.top

Go:   os.Exit(1)
来源：http://jyp.yuxming.cn

Ruby: exit 1
来源：http://vwl.svipenyu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://icx.xziqi.cn

[M06] 向标准错误输出
来源：http://roc.pengpengdd.cyou

Py:   print("err", file=sys.stderr)
来源：http://tut.zhaomingkeji.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://nwm.bbcook.cn

JS:   console.error("err")
来源：http://iap.jinqigufen.top

TS:   console.error("err")
来源：http://tfu.wangshuangyany.cn

Java: System.err.println("err")
来源：http://iol.gaohongyu789.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jdt.cucudq.cn

Ruby: warn "err"
来源：http://tge.pycfn.com

C#:   Console.Error.WriteLine("err")
来源：http://bnf.vehdjk.com

[M07] 判断是否为主入口
来源：http://hiq.aizwys.cn

Py:   if __name__ == "__main__":
来源：http://egv.zhijiandao.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gjo.yongpay.top

JS:   require.main === module
来源：http://pvy.yj20258.top

TS:   require.main === module
来源：http://jaa.redwolf501.top

Java: public static void main(String[] args)
来源：http://aah.hnqzz.top

Go:   func main()
来源：http://zdn.52xcode.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jks.yj20258888.top

C#:   static void Main(string[] args)
来源：http://nsi.0kj1m.cn

[M08] 获取系统与运行时信息
来源：http://yhs.zhixingplan.top

Py:   platform.system();  platform.python_version()
来源：http://qot.sysykeji.top

PHP:  PHP_OS;  phpversion();
来源：http://gax.guannengcc.top

JS:   process.platform;  process.version
来源：http://met.uphjek.com

TS:   process.platform;  process.version
来源：http://qgu.xingfuxueyuan.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tti.snrcjt.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sbk.chenjidiqi.icu

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jar.0kj1m.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nlh.aizwys.cn

================================================================================
来源：http://dvg.cucudq.cn

N. 数据结构与算法
来源：http://mwo.mhx1999.top

================================================================================
来源：http://zoi.0kj1m.cn

[N01] 二分查找（有序数组）
来源：http://pjm.fanxiaobao.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://oub.fzhhl.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tre.ybcxt.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jxb.ywan-chungtsiang.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://enh.yonumen.top

Java: Arrays.binarySearch(arr, x)
来源：http://gpd.chenzaomai.com

Go:   sort.SearchInts(arr, x)
来源：http://edy.uphjek.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://tnz.redwolf501.top

C#:   Array.BinarySearch(arr, x)
来源：http://ttk.zhixingplan.top

[N02] 排序（工程实践用内置实现）
来源：http://wok.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://pyf.shanyushiyangkeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ryu.feifeiyinyue.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://vxf.guowangkeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ewt.chenzaomai.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kix.cashguo.top

Go:   slices.Sort(arr)
来源：http://oct.yueranfly.top

Ruby: arr.sort
来源：http://nlb.yongpay.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xwz.yanxiufei.cn

[N03] 快速排序（分治示例）
来源：http://vrx.zhaomingkeji.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://naz.jianghu66.top

PHP:  // 递归实现，或用 usort
来源：http://lun.ppjwa.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lnz.guannengcc.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gjb.pycfn.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sfc.iojbl.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ubv.chenzaomai.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kik.cheryme.top

C#:   // 手写递归，或 Array.Sort
来源：http://pap.jiagoushi.top

[N04] 斐波那契数列
来源：http://chb.ydzc1.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gzg.xingfuxueyuan.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uwo.vehdjk.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jxv.jinghuilouyu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kvt.haohaochexian.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hbr.chenlongwang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vhb.jlsjyb.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ikj.zhoulong.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ujl.zhaomingkeji.xyz

[N05] 最大公约数
来源：http://rbi.fktsv.cn

Py:   math.gcd(a, b)
来源：http://fbs.yuxming.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dyg.aizwys.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tfq.xziqi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fgg.zdqjudy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://puf.jianghu66.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bqd.cdnleiting.top

Ruby: a.gcd(b)
来源：http://oph.zhengqikj.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://agf.chenzaomai.com

[N06] 判断回文字符串
来源：http://irt.dianchejie.cn

Py:   s == s[::-1]
来源：http://kob.yj202588.top

PHP:  $s === strrev($s);
来源：http://uul.shzxlz.cn

JS:   s === [...s].reverse().join("")
来源：http://hng.gaohongyu789.top

TS:   s === [...s].reverse().join("")
来源：http://qzg.zhongyouzk.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tzu.smart0.xyz

Go:   // 双指针从两端比较
来源：http://xhc.smart0.xyz

Ruby: s == s.reverse
来源：http://caj.xziqi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://crh.yongpay.top

[N07] 两数之和（返回下标）
来源：http://bds.chenzaomai.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mmz.fehbvm.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ybi.zhaomingkeji.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://ayd.zhoulong.xyz

TS:   // 手写 Map<string, number>
来源：http://sgo.c1oappe.top

Java: // 手写 HashMap
来源：http://rtq.birdmap.top

Go:   // 手写 map[int]int
来源：http://zay.nwbrower.top

Ruby: // 手写 Hash
来源：http://vuh.jinghuilouyu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kwk.haohaochexian.top

[N08] 生成全排列
来源：http://lhh.chenjidiqi.icu

Py:   itertools.permutations(arr)
来源：http://mhr.xylfe.cn

PHP:  // 手写递归交换
来源：http://cmu.ywan-chungtsiang.top

JS:   // 手写回溯递归
来源：http://lxh.chenzaomai.com

TS:   // 手写回溯递归
来源：http://kih.xuanzx.com

Java: // 手写回溯递归
来源：http://mha.xuetiantiany.cn

Go:   // 手写回溯递归
来源：http://fpj.shangyingyoupin.top

Ruby: arr.permutation.to_a
来源：http://fxj.ydzc1.top

C#:   // 手写回溯递归
来源：http://gnv.gotoacloud.top

[N09] 栈与队列
来源：http://rix.xinyue.icu

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fxa.haohaochexian.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uju.birdmap.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rzo.aibaodan.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pgn.birdmap.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hlc.svipenyu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://czk.dianchejie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xkt.gogol.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jze.zhijiandao.cn

[N10] 链表节点定义
来源：http://ggp.havefunace.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wse.jqgfzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://rnl.yuanzhike.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wfn.gogol.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://aag.fktsv.cn

Java: class Node { int v; Node next; }
来源：http://czt.aibaodan.cn

Go:   type Node struct { V int; Next *Node }
来源：http://isd.hammf.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://blb.zhongyouzk.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ikx.tian-w.cn

[N11] 二叉树中序遍历
来源：http://jjz.jinqigfzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bzm.fanxiaobao.xyz

PHP:  // 手写递归函数
来源：http://fbq.cashguo.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vne.jianghu66.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lhm.haohaochexian.top

Java: // 手写递归
来源：http://zvs.xingfuxueyuan.xyz

Go:   // 手写递归
来源：http://sli.guowangkeji.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lmu.guowangkeji.top

C#:   // 手写递归
来源：http://cck.hysaishi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rzt.fehbvm.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kwx.dianchejie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yfw.chenzaomai.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://arm.xuetiantiany.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cwu.jyoumei.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mlr.yonumen.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xbc.ydzc1.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://czk.snrcjt.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ipd.ybcxt.top

================================================================================
来源：http://vvw.dashuyun.cn

O. 并发与异步
来源：http://ylb.yvedp.cn

================================================================================
来源：http://zzt.fktsv.cn

[O01] 启动一个线程
来源：http://zsl.haohaochexian.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wbe.yj202588.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zyi.daxiang520.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ocg.aibaodan.cn

TS:   // 同 JS
来源：http://zuo.tanke756.top

Java: new Thread(() -> f()).start()
来源：http://xbo.xuetiantiany.cn

Go:   go f()
来源：http://ibq.redwolf501.top

Ruby: Thread.new { f }
来源：http://rga.smart0.xyz

C#:   Task.Run(() => F());
来源：http://auf.nanxinkj.top

[O02] 使用线程池
来源：http://gpi.uphjek.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fwm.dianchejie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ooq.hongshengwenyu.top

JS:   // worker_threads 线程池
来源：http://bji.jlsjyb.cn

TS:   // worker_threads 线程池
来源：http://ctz.jqgfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://vzu.hfpthk.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ovr.tian-w.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rvc.uphjek.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://aly.cheryme.top

[O03] 加锁保护共享数据
来源：http://gnp.hongshengwenyu.top

Py:   with lock: shared += 1
来源：http://yng.yvedp.cn

PHP:  // 用 flock() 做文件锁
来源：http://wwb.xinyue.icu

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jro.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://avi.yuxming.cn

Java: synchronized (this) { shared++; }
来源：http://pra.316326.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nze.hammf.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://npk.dashuyun.cn

C#:   lock (gate) { shared++; }
来源：http://xkb.sjlbkw.cn

[O04] 定义异步函数并等待
来源：http://imm.ybcxt.top

Py:   async def f():⏎    await g()
来源：http://hjj.fktsv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uzi.daxiang520.top

JS:   async function f() { await g(); }
来源：http://idv.wangdashe.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://efy.yuanzhike.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jza.hysaishi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://veo.zdqjudy.top

Ruby: # 用 Fiber 或 async gem
来源：http://kbc.yj20258888.top

C#:   async Task F() { await G(); }
来源：http://tzb.uphjek.com

[O05] 并发执行并等待全部完成
来源：http://nqd.shangyingyoupin.top

Py:   asyncio.gather(*tasks)
来源：http://dom.cashguo.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dqy.feifeiyinyue.top

JS:   await Promise.all(tasks)
来源：http://cow.wangdashe.top

TS:   await Promise.all(tasks)
来源：http://pjh.iojbl.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xue.gogol.net.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bqh.hfpthk.cn

Ruby: threads.map(&:join)
来源：http://quv.jinghuilouyu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://lyz.epnwcf.com

[O06] 使用进程池
来源：http://scg.bbcook.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bgi.yj202588.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ouv.shangyingyoupin.top

JS:   // child_process / cluster 模块
来源：http://ric.ppjwa.cn

TS:   // child_process / cluster 模块
来源：http://loy.ctjpmb.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rpv.jianghu66.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uzg.jinqigufen.top

Ruby: // fork 块
来源：http://tco.jinyuanbaomall.cn

C#:   Parallel.For
来源：http://zva.wangshuangyany.cn

================================================================================
来源：http://oyw.yfazqb.com

P. 常用工具函数
来源：http://wnp.feifeiyinyue.top

================================================================================
来源：http://pwq.chenzaomai.com

[P01] 生成 UUID
来源：http://qsz.zhoulong.xyz

Py:   str(uuid.uuid4())
来源：http://bpl.svipenyu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rdf.fzhhl.top

JS:   crypto.randomUUID()
来源：http://zew.pycfn.com

TS:   crypto.randomUUID()
来源：http://vsw.fengsongda.top

Java: UUID.randomUUID().toString()
来源：http://yvc.fehbvm.com

Go:   // 用 github.com/google/uuid
来源：http://kgz.tianlin.xyz

Ruby: SecureRandom.uuid
来源：http://uue.guannengcc.top

C#:   Guid.NewGuid().ToString()
来源：http://lcx.316326.xyz

[P02] MD5 / SHA256 摘要
来源：http://ncj.epnwcf.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hyk.jinyuanbaomall.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://lxm.yanxiufei.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://agi.c1oappe.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sqq.sweek.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://olg.yueranfly.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uvk.ydzc1.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hvz.0kj1m.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bnw.ehwqpu.com

[P03] 生成短随机字符串
来源：http://wdo.xylfe.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tzo.cqqwz.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sgp.hysaishi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zcj.quarkkingdee.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fwf.nanxuanxn.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yfp.nwbrower.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dae.yangfankeji.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://roi.xinyue.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://btk.ppjwa.cn

[P04] 求长度
来源：http://vro.yueranfly.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://njd.jinqigfzy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://djp.aizwys.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tkf.haohaochexian.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rqy.guannengcc.top

Java: list.size();  map.size();  s.length()
来源：http://fam.yueranfly.top

Go:   len(arr);  len(m)
来源：http://bdv.wangdashe.top

Ruby: x.length;  x.size
来源：http://rij.ivvv.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://rvy.xuetiantiany.cn

[P05] 判断两个对象内容是否相等
来源：http://hzl.nwbrower.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://mfz.cheryme.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sza.aizwys.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://leg.epnwcf.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://avo.sysykeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://osq.gogol.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zmu.bbcook.cn

Ruby: a == b
来源：http://cms.xuetiantiany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sbn.snrcjt.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mag.c1oappe.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pxx.wangshuangyany.cn

PHP:  if (empty($x)) {}
来源：http://cqa.zhoulong.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zry.sweek.top

TS:   if (x == null) {}
来源：http://pmz.yj20258888.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ile.aibaodan.cn

Go:   if x == nil {}
来源：http://naw.nwbrower.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://byx.yvedp.cn

C#:   if (x is null) {}
来源：http://eli.jinghuilouyu.cn

[P07] 防抖与节流
来源：http://emu.ydjk.org.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sqe.ehwqpu.com

PHP:  // 手写时间戳比较
来源：http://yve.bjfxy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wes.birdmap.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oxc.svipenyu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wuj.jqgfzy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qyu.fengsongda.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://uxv.hywenlv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dfc.hnxiangtu.top

[P08] 处理浮点精度问题
来源：http://nbt.yj202588.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qir.fengsongda.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://klk.hnqzz.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gva.hnxiangtu.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kqj.xingfuxueyuan.xyz


<!-- 参考信息 -->