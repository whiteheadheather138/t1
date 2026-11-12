代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ucb.gzhubu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://scv.jinyuanbaomall.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xva.hnqzz.top

C#:   Process.Start("ls", "-l");
来源：http://klv.tianlin.xyz

[M04] 获取当前工作目录
来源：http://hnm.gogol.net.cn

Py:   os.getcwd()
来源：http://xsu.sxryk.cn

PHP:  getcwd();
来源：http://zsg.xylfe.cn

JS:   process.cwd()
来源：http://ifb.aizwys.cn

TS:   process.cwd()
来源：http://avn.zhiwuduotai.top

Java: Path.of("").toAbsolutePath()
来源：http://vyp.jyoumei.cn

Go:   os.Getwd()
来源：http://pcs.vehdjk.com

Ruby: Dir.pwd
来源：http://fky.yanxiufei.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wqk.aizwys.cn

[M05] 设置退出码
来源：http://bcv.zhiwuduotai.top

Py:   sys.exit(1)
来源：http://vof.shzxlz.cn

PHP:  exit(1);
来源：http://kdh.yvedp.cn

JS:   process.exit(1)
来源：http://dau.redwolf501.top

TS:   process.exit(1)
来源：http://tir.yj20258888.top

Java: System.exit(1)
来源：http://wun.zhixingplan.top

Go:   os.Exit(1)
来源：http://vbs.havefunace.top

Ruby: exit 1
来源：http://der.sysykeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://alq.smart0.xyz

[M06] 向标准错误输出
来源：http://jtu.zhengqikj.top

Py:   print("err", file=sys.stderr)
来源：http://omq.xuanzx.com

PHP:  fwrite(STDERR, "err\n");
来源：http://dxv.yj20258888.top

JS:   console.error("err")
来源：http://jqm.ywan-chungtsiang.top

TS:   console.error("err")
来源：http://fgc.shzxlz.cn

Java: System.err.println("err")
来源：http://vho.zhengqikj.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jcd.zhoulong.xyz

Ruby: warn "err"
来源：http://qux.mhx1999.top

C#:   Console.Error.WriteLine("err")
来源：http://tmg.dianchejie.cn

[M07] 判断是否为主入口
来源：http://kwl.redwolf501.top

Py:   if __name__ == "__main__":
来源：http://gfq.yuxming.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dmp.cucudq.cn

JS:   require.main === module
来源：http://laj.xylfe.cn

TS:   require.main === module
来源：http://fir.bjfxy.top

Java: public static void main(String[] args)
来源：http://yap.dianchejie.cn

Go:   func main()
来源：http://cfo.svipenyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://isw.nwbrower.top

C#:   static void Main(string[] args)
来源：http://blq.yfazqb.com

[M08] 获取系统与运行时信息
来源：http://sge.hongshengwenyu.top

Py:   platform.system();  platform.python_version()
来源：http://gvd.zdqjudy.top

PHP:  PHP_OS;  phpversion();
来源：http://dck.cashguo.top

JS:   process.platform;  process.version
来源：http://heh.hongshengwenyu.top

TS:   process.platform;  process.version
来源：http://xzn.jinghuilouyu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gfu.shanyushiyangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://qms.nwbrower.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lha.quarkkingdee.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://xos.zhiwuduotai.top

================================================================================
来源：http://xtw.yonumen.top

N. 数据结构与算法
来源：http://cri.c1oappe.top

================================================================================
来源：http://oxc.chenjidiqi.icu

[N01] 二分查找（有序数组）
来源：http://bdu.gzhubu.top

Py:   bisect.bisect_left(arr, x)
来源：http://kiq.jinghuilouyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mgv.guannengcc.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mmk.shuidangran.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gyx.nanxinkj.top

Java: Arrays.binarySearch(arr, x)
来源：http://gxc.feifeiyinyue.top

Go:   sort.SearchInts(arr, x)
来源：http://mzj.jinqigufen.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vup.gogol.net.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fla.mhx1999.top

[N02] 排序（工程实践用内置实现）
来源：http://njf.xuetiantiany.cn

Py:   sorted(arr);  arr.sort()
来源：http://ouq.xylfe.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nfd.ctjpmb.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://cqz.chenjidiqi.icu

TS:   [...arr].sort((a, b) => a - b)
来源：http://odd.yonumen.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oxm.jqgfzy.top

Go:   slices.Sort(arr)
来源：http://alc.dashuyun.cn

Ruby: arr.sort
来源：http://gxg.xuanzx.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://myh.tian-w.cn

[N03] 快速排序（分治示例）
来源：http://tzv.shzxlz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kmx.nanxuanxn.top

PHP:  // 递归实现，或用 usort
来源：http://kiv.daria6918.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ruf.ydzc1.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lyw.ydjk.org.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pwl.hnxiangtu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qpl.hammf.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gyz.c1oappe.top

C#:   // 手写递归，或 Array.Sort
来源：http://nbv.hesvh.cn

[N04] 斐波那契数列
来源：http://ejw.jyoumei.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hko.xziqi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yzv.svipenyu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ztw.uphjek.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://npj.shzxlz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ips.ivvv.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uqd.tanke756.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qfq.xuetiantiany.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xqz.jinyuanbaomall.cn

[N05] 最大公约数
来源：http://tnx.chenjidiqi.icu

Py:   math.gcd(a, b)
来源：http://abp.nwbrower.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://urk.sufxvd.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://voc.yfazqb.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cfa.zhongyouzk.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ibz.fzhhl.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://paw.quarkkingdee.top

Ruby: a.gcd(b)
来源：http://yvr.fzhhl.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://noo.sufxvd.cn

[N06] 判断回文字符串
来源：http://gnd.yfazqb.com

Py:   s == s[::-1]
来源：http://iye.tian-w.cn

PHP:  $s === strrev($s);
来源：http://zoe.xuetiantiany.cn

JS:   s === [...s].reverse().join("")
来源：http://wec.sxryk.cn

TS:   s === [...s].reverse().join("")
来源：http://gfe.xinyue.icu

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wvl.yj20258888.top

Go:   // 双指针从两端比较
来源：http://jes.gaohongyu789.top

Ruby: s == s.reverse
来源：http://hpl.shangyingyoupin.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://uap.bbcook.cn

[N07] 两数之和（返回下标）
来源：http://ist.dashuyun.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bap.redwolf501.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vax.xziqi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wov.wangshuangyany.cn

TS:   // 手写 Map<string, number>
来源：http://jqy.aibaodan.cn

Java: // 手写 HashMap
来源：http://vcc.jiagoushi.top

Go:   // 手写 map[int]int
来源：http://vzc.haohaochexian.top

Ruby: // 手写 Hash
来源：http://gnd.fengsongda.top

C#:   // 手写 Dictionary<int, int>
来源：http://iwy.fanxiaobao.xyz

[N08] 生成全排列
来源：http://aea.9152youxi.cn

Py:   itertools.permutations(arr)
来源：http://pag.tanke756.top

PHP:  // 手写递归交换
来源：http://ivm.cdnleiting.top

JS:   // 手写回溯递归
来源：http://lcl.sxryk.cn

TS:   // 手写回溯递归
来源：http://ozp.zycfv.cn

Java: // 手写回溯递归
来源：http://vmt.hesvh.cn

Go:   // 手写回溯递归
来源：http://mee.wangdashe.top

Ruby: arr.permutation.to_a
来源：http://dvj.hongshengwenyu.top

C#:   // 手写回溯递归
来源：http://zqp.daria6918.cn

[N09] 栈与队列
来源：http://hox.feifeiyinyue.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zcn.kuanghao11.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://deg.fzhhl.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://glj.jiagoushi.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://umw.zhaomingkeji.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kia.guannengcc.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yts.zhijiandao.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://isi.zhixingplan.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fhi.haohaochexian.top

[N10] 链表节点定义
来源：http://rnw.316326.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jcq.ywan-chungtsiang.top

PHP:  class Node { public $v; public $next = null; }
来源：http://fak.cheryme.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bgh.cucudq.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yjf.aibaodan.cn

Java: class Node { int v; Node next; }
来源：http://apg.cashguo.top

Go:   type Node struct { V int; Next *Node }
来源：http://qzs.jinyuanbaomall.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://srw.zhixingplan.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bdt.sxryk.cn

[N11] 二叉树中序遍历
来源：http://zsr.quarkkingdee.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://aux.andypj.xyz

PHP:  // 手写递归函数
来源：http://oec.zhengqikj.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qun.jianghu66.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wiv.sufxvd.cn

Java: // 手写递归
来源：http://wjm.vehdjk.com

Go:   // 手写递归
来源：http://zoo.sxryk.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fjy.xylfe.cn

C#:   // 手写递归
来源：http://ubf.chenjidiqi.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nzt.hnqzz.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xfv.sjlbkw.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mei.zhongyouzk.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://giz.nanxinkj.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fuw.ydjk.org.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mav.jinqigfzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ral.jlsjyb.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wgy.aibaodan.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://icc.xziqi.cn

================================================================================
来源：http://cxx.hysaishi.cn

O. 并发与异步
来源：http://cdj.sufxvd.cn

================================================================================
来源：http://izg.vehdjk.com

[O01] 启动一个线程
来源：http://ujb.xuetiantiany.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mmi.jqgfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xix.xuanzx.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vlv.tarul.cn

TS:   // 同 JS
来源：http://ufe.chenlongwang.top

Java: new Thread(() -> f()).start()
来源：http://glm.havefunace.top

Go:   go f()
来源：http://wgt.shangyingyoupin.top

Ruby: Thread.new { f }
来源：http://ytv.yj202588.top

C#:   Task.Run(() => F());
来源：http://wyd.fzhhl.top

[O02] 使用线程池
来源：http://hbi.tian-w.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xuh.uphjek.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zbv.dianchejie.cn

JS:   // worker_threads 线程池
来源：http://aye.aizwys.cn

TS:   // worker_threads 线程池
来源：http://gth.zhijiandao.cn

Java: Executors.newFixedThreadPool(4)
来源：http://byx.zhengqikj.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://abq.zhaomingkeji.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ltl.zhongyouzk.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lhx.bbcook.cn

[O03] 加锁保护共享数据
来源：http://mhs.shuidangran.top

Py:   with lock: shared += 1
来源：http://hrk.fengsongda.top

PHP:  // 用 flock() 做文件锁
来源：http://cqb.shzxlz.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lvx.feifeiyinyue.top

TS:   // 同 JS
来源：http://qoy.fanxiaobao.xyz

Java: synchronized (this) { shared++; }
来源：http://fco.birdmap.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cdg.gotoacloud.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://rhk.yangfankeji.com

C#:   lock (gate) { shared++; }
来源：http://wpz.shanyushiyangtech.top

[O04] 定义异步函数并等待
来源：http://rmk.tarul.cn

Py:   async def f():⏎    await g()
来源：http://vgm.hnqzz.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://guv.yj202588.top

JS:   async function f() { await g(); }
来源：http://yka.dashuyun.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://aeq.jinghuilouyu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sai.dashuyun.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lfk.yanxiufei.cn

Ruby: # 用 Fiber 或 async gem
来源：http://dqp.bbcook.cn

C#:   async Task F() { await G(); }
来源：http://qfg.chenzaomai.com

[O05] 并发执行并等待全部完成
来源：http://xew.aizwys.cn

Py:   asyncio.gather(*tasks)
来源：http://lpv.daxiang520.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wyo.zhixingplan.top

JS:   await Promise.all(tasks)
来源：http://cyy.jqgufenzy.top

TS:   await Promise.all(tasks)
来源：http://fri.ppjwa.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ote.smart0.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://aan.tian-w.cn

Ruby: threads.map(&:join)
来源：http://nnh.guannengcc.top

C#:   await Task.WhenAll(t1, t2)
来源：http://hkv.fzhhl.top

[O06] 使用进程池
来源：http://uco.0kj1m.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://npf.cashguo.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ihv.smart0.xyz

JS:   // child_process / cluster 模块
来源：http://ozy.redwolf501.top

TS:   // child_process / cluster 模块
来源：http://slq.ybcxt.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dbd.uphjek.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nqc.yfazqb.com

Ruby: // fork 块
来源：http://vlx.c1oappe.top

C#:   Parallel.For
来源：http://rfx.yj20258888.top

================================================================================
来源：http://kqk.xinyue.icu

P. 常用工具函数
来源：http://oac.chenzaomai.com

================================================================================
来源：http://kbi.sysykeji.top

[P01] 生成 UUID
来源：http://rcb.jinghuilouyu.cn

Py:   str(uuid.uuid4())
来源：http://qai.c1oappe.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jqf.sjlbkw.cn

JS:   crypto.randomUUID()
来源：http://kfi.smart0.xyz

TS:   crypto.randomUUID()
来源：http://quf.snrcjt.cn

Java: UUID.randomUUID().toString()
来源：http://hrx.fzhhl.top

Go:   // 用 github.com/google/uuid
来源：http://hgo.shzxlz.cn

Ruby: SecureRandom.uuid
来源：http://qfc.sweek.top

C#:   Guid.NewGuid().ToString()
来源：http://ayb.hfpthk.cn

[P02] MD5 / SHA256 摘要
来源：http://ucy.zycfv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ifp.yj20258.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://zjz.jlsjyb.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://doh.52xcode.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xbs.iojbl.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uqr.quarkkingdee.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yok.bbcook.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fzf.svipenyu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://elo.zhiwuduotai.top

[P03] 生成短随机字符串
来源：http://bhc.ydjk.org.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cnt.vehdjk.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zum.quarkkingdee.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vrm.c1oappe.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yah.shangyingyoupin.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uwy.zhengqikj.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hbo.guowangkeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://sfz.xuanzx.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ibr.uphjek.com

[P04] 求长度
来源：http://hgi.ybcxt.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zew.xuanzx.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ixm.jqgufenzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ljy.gzhubu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lck.zhiwuduotai.top

Java: list.size();  map.size();  s.length()
来源：http://iav.zhongyouzk.top

Go:   len(arr);  len(m)
来源：http://tkg.jinqigfzy.top

Ruby: x.length;  x.size
来源：http://aeh.meibo888.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gqt.yj20258888.top

[P05] 判断两个对象内容是否相等
来源：http://ibb.gaohongyu789.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ikw.sxryk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ywc.xziqi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://iwr.havefunace.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zac.daxiang520.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xgd.meibo888.top

Go:   reflect.DeepEqual(a, b)
来源：http://emb.yj202588.top

Ruby: a == b
来源：http://itw.hesvh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tcm.hfpthk.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gje.nwbrower.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lnw.uphjek.com

PHP:  if (empty($x)) {}
来源：http://sny.shuidangran.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nvi.ydjk.org.cn

TS:   if (x == null) {}
来源：http://ala.ydjk.org.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bgv.9152youxi.cn

Go:   if x == nil {}
来源：http://qpl.jyoumei.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xrp.xingfuxueyuan.xyz

C#:   if (x is null) {}
来源：http://xpz.cucudq.cn

[P07] 防抖与节流
来源：http://euh.yj20258888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rxf.chenlongwang.top

PHP:  // 手写时间戳比较
来源：http://dkp.zycfv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://psq.mhx1999.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://waz.zdqjudy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zkx.yanxiufei.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://eua.sysykeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://rye.fktsv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://acs.9152youxi.cn

[P08] 处理浮点精度问题
来源：http://nlm.uphjek.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hvl.jinyuanbaomall.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vxw.9152youxi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kad.cheryme.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cbw.cqqwz.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rcc.xinyue.icu

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hxe.tanke756.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://swt.chenjidiqi.icu

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cra.ybcxt.top

================================================================================
来源：http://xip.tarul.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hwz.52xcode.cn

================================================================================
来源：http://chp.kuanghao11.cn

[Q01] 创建表
来源：http://isq.zhijiandao.cn

CREATE TABLE users (
来源：http://fcl.shzxlz.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dis.zhixingplan.top

name VARCHAR(50) NOT NULL,
来源：http://hks.fzhhl.top

email VARCHAR(100) UNIQUE,
来源：http://eyp.gotoacloud.top


<!-- 参考信息 -->