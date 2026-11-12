代发 wailian999

[M04] 获取当前工作目录
来源：http://gja.fengsongda.top

Py:   os.getcwd()
来源：http://kde.gzhubu.top

PHP:  getcwd();
来源：http://qzc.pengpengdd.cyou

JS:   process.cwd()
来源：http://hje.daria6918.cn

TS:   process.cwd()
来源：http://uvp.hongshengwenyu.top

Java: Path.of("").toAbsolutePath()
来源：http://lxd.dianchejie.cn

Go:   os.Getwd()
来源：http://jjb.bjfxy.top

Ruby: Dir.pwd
来源：http://ubk.mhx1999.top

C#:   Directory.GetCurrentDirectory()
来源：http://jxg.tanke756.top

[M05] 设置退出码
来源：http://noa.ydjk.org.cn

Py:   sys.exit(1)
来源：http://xgd.yangfankeji.com

PHP:  exit(1);
来源：http://ria.guowangkeji.top

JS:   process.exit(1)
来源：http://sij.meibo888.top

TS:   process.exit(1)
来源：http://bee.zhixingplan.top

Java: System.exit(1)
来源：http://iwz.0kj1m.cn

Go:   os.Exit(1)
来源：http://jrj.svipenyu.cn

Ruby: exit 1
来源：http://vlb.c1oappe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xny.vehdjk.com

[M06] 向标准错误输出
来源：http://hlj.fktsv.cn

Py:   print("err", file=sys.stderr)
来源：http://ljg.vqdsnc.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://yol.zhixingplan.top

JS:   console.error("err")
来源：http://jyz.gogol.net.cn

TS:   console.error("err")
来源：http://yxd.tanke756.top

Java: System.err.println("err")
来源：http://qvq.nanxuanxn.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kek.zdbjq.cn

Ruby: warn "err"
来源：http://rib.yanxiufei.cn

C#:   Console.Error.WriteLine("err")
来源：http://jlb.hcnkem.com

[M07] 判断是否为主入口
来源：http://ses.cqqwz.cn

Py:   if __name__ == "__main__":
来源：http://dwd.feifeiyinyue.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cfs.sxryk.cn

JS:   require.main === module
来源：http://lmf.hysaishi.cn

TS:   require.main === module
来源：http://vin.zhoulong.xyz

Java: public static void main(String[] args)
来源：http://cal.meibo888.top

Go:   func main()
来源：http://xko.tianlin.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bwt.pycfn.com

C#:   static void Main(string[] args)
来源：http://fej.xziqi.cn

[M08] 获取系统与运行时信息
来源：http://xjl.haohaochexian.top

Py:   platform.system();  platform.python_version()
来源：http://gea.xylfe.cn

PHP:  PHP_OS;  phpversion();
来源：http://wjx.wangdashe.top

JS:   process.platform;  process.version
来源：http://avw.nanxinkj.top

TS:   process.platform;  process.version
来源：http://qpl.gzhubu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sqi.c1oappe.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://lhm.gotoacloud.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dpq.yueranfly.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://bvx.gotoacloud.top

================================================================================
来源：http://fdw.jianghu66.top

N. 数据结构与算法
来源：http://sdb.iojbl.cn

================================================================================
来源：http://kxd.bbcook.cn

[N01] 二分查找（有序数组）
来源：http://fsd.316326.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://gob.gotoacloud.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://irb.iojbl.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bvp.wangshuangyany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qyd.9152youxi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ecc.jinqigfzy.top

Go:   sort.SearchInts(arr, x)
来源：http://vun.zhengqikj.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://mff.guowangkeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://jav.zhixingplan.top

[N02] 排序（工程实践用内置实现）
来源：http://mhb.tian-w.cn

Py:   sorted(arr);  arr.sort()
来源：http://qor.jinyuanbaomall.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://otq.ydzc1.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://pnh.hesvh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ymm.sysykeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vnn.guannengcc.top

Go:   slices.Sort(arr)
来源：http://eki.daria6918.cn

Ruby: arr.sort
来源：http://cso.yanxiufei.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hmt.dianchejie.cn

[N03] 快速排序（分治示例）
来源：http://kge.aibaodan.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gqa.zhixingplan.top

PHP:  // 递归实现，或用 usort
来源：http://gjb.dianchejie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://txi.tian-w.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qhn.sufxvd.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nao.guannengcc.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bbc.zhiwuduotai.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bxx.fengsongda.top

C#:   // 手写递归，或 Array.Sort
来源：http://ezd.dashuyun.cn

[N04] 斐波那契数列
来源：http://qfj.jianghu66.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pke.ctjpmb.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lwj.zhoulong.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://esb.havefunace.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eop.shzxlz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rjm.fktsv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pna.haohaochexian.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dol.snrcjt.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mom.mhx1999.top

[N05] 最大公约数
来源：http://mmg.jinqigfzy.top

Py:   math.gcd(a, b)
来源：http://nps.0kj1m.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lla.iojbl.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://arc.bjfxy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mto.c1oappe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yen.zhijiandao.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bpj.sweek.top

Ruby: a.gcd(b)
来源：http://hxm.hnqzz.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tet.tanke756.top

[N06] 判断回文字符串
来源：http://nwt.pengpengdd.cyou

Py:   s == s[::-1]
来源：http://irz.tanke756.top

PHP:  $s === strrev($s);
来源：http://anf.jlsjyb.cn

JS:   s === [...s].reverse().join("")
来源：http://twq.sufxvd.cn

TS:   s === [...s].reverse().join("")
来源：http://lgn.316326.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sqm.shzxlz.cn

Go:   // 双指针从两端比较
来源：http://ayc.jiagoushi.top

Ruby: s == s.reverse
来源：http://gdo.sysykeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://hoe.hnxiangtu.top

[N07] 两数之和（返回下标）
来源：http://ecm.andypj.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://srd.hcnkem.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oqa.hcnkem.com

JS:   // 手写 Map：map.set(v, i)
来源：http://ufa.cucudq.cn

TS:   // 手写 Map<string, number>
来源：http://fun.bbcook.cn

Java: // 手写 HashMap
来源：http://rtd.52xcode.cn

Go:   // 手写 map[int]int
来源：http://lry.ppjwa.cn

Ruby: // 手写 Hash
来源：http://dij.zhiwuduotai.top

C#:   // 手写 Dictionary<int, int>
来源：http://vtq.snrcjt.cn

[N08] 生成全排列
来源：http://brq.yj20258.top

Py:   itertools.permutations(arr)
来源：http://kvm.9152youxi.cn

PHP:  // 手写递归交换
来源：http://wct.xylfe.cn

JS:   // 手写回溯递归
来源：http://bqp.xylfe.cn

TS:   // 手写回溯递归
来源：http://xil.snrcjt.cn

Java: // 手写回溯递归
来源：http://umf.redwolf501.top

Go:   // 手写回溯递归
来源：http://jhx.zhixingplan.top

Ruby: arr.permutation.to_a
来源：http://hem.shangyingyoupin.top

C#:   // 手写回溯递归
来源：http://fck.meibo888.top

[N09] 栈与队列
来源：http://wua.shanyushiyangtech.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fzn.hongshengwenyu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xri.hesvh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wxr.tanke756.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wpz.zycfv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://khv.dashuyun.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lfe.haohaochexian.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dcg.fktsv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://twv.yongpay.top

[N10] 链表节点定义
来源：http://xin.yonumen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://irh.ivvv.top

PHP:  class Node { public $v; public $next = null; }
来源：http://jei.meibo888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gbc.gzhubu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kpt.yj202588.top

Java: class Node { int v; Node next; }
来源：http://ele.jinyuanbaomall.cn

Go:   type Node struct { V int; Next *Node }
来源：http://kfs.jinyuanbaomall.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hkj.nwbrower.top

C#:   class Node { public int V; public Node? Next; }
来源：http://fdb.ivvv.top

[N11] 二叉树中序遍历
来源：http://oub.jinyuanbaomall.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wao.shanyushiyangkeji.top

PHP:  // 手写递归函数
来源：http://hma.nwbrower.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yfv.shuidangran.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hmf.feifeiyinyue.top

Java: // 手写递归
来源：http://awb.zhiwuduotai.top

Go:   // 手写递归
来源：http://rvf.hywenlv.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ixk.aibaodan.cn

C#:   // 手写递归
来源：http://ujz.yueranfly.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jwo.zhongyouzk.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bpo.zhijiandao.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ksp.daxiang520.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jkx.zhijiandao.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lfd.jinghuilouyu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wqn.nwbrower.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uwj.gogol.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://auc.cucudq.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qlf.hongshengwenyu.top

================================================================================
来源：http://fyc.shuidangran.top

O. 并发与异步
来源：http://reo.havefunace.top

================================================================================
来源：http://dlc.jinghuilouyu.cn

[O01] 启动一个线程
来源：http://rbq.sxryk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kcq.gzhubu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dwq.ctjpmb.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://shy.feifeiyinyue.top

TS:   // 同 JS
来源：http://jyj.aizwys.cn

Java: new Thread(() -> f()).start()
来源：http://uhv.sweek.top

Go:   go f()
来源：http://vdp.52xcode.cn

Ruby: Thread.new { f }
来源：http://rpe.ybcxt.top

C#:   Task.Run(() => F());
来源：http://wyf.tarul.cn

[O02] 使用线程池
来源：http://zrl.zycfv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wjk.cucudq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dtr.shzxlz.cn

JS:   // worker_threads 线程池
来源：http://ngv.iojbl.cn

TS:   // worker_threads 线程池
来源：http://spn.yvedp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://mfj.gzhubu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bqj.wangdashe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vro.jianghu66.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wnj.fehbvm.com

[O03] 加锁保护共享数据
来源：http://sex.cashguo.top

Py:   with lock: shared += 1
来源：http://fzg.shzxlz.cn

PHP:  // 用 flock() 做文件锁
来源：http://cpe.hongshengwenyu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lps.shanyushiyangkeji.top

TS:   // 同 JS
来源：http://yom.zhengqikj.top

Java: synchronized (this) { shared++; }
来源：http://mge.zhijiandao.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mlq.hywenlv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ilh.birdmap.top

C#:   lock (gate) { shared++; }
来源：http://lpw.guowangkeji.top

[O04] 定义异步函数并等待
来源：http://mdj.xylfe.cn

Py:   async def f():⏎    await g()
来源：http://jxd.gaohongyu789.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dkz.zhixingplan.top

JS:   async function f() { await g(); }
来源：http://bci.sxryk.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ijy.zhixingplan.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wrw.zycfv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sqx.yonumen.top

Ruby: # 用 Fiber 或 async gem
来源：http://yqe.fehbvm.com

C#:   async Task F() { await G(); }
来源：http://cyi.vqdsnc.cn

[O05] 并发执行并等待全部完成
来源：http://pdn.ybcxt.top

Py:   asyncio.gather(*tasks)
来源：http://sjl.jqgfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ajo.xinyue.icu

JS:   await Promise.all(tasks)
来源：http://jvg.yuanzhike.top

TS:   await Promise.all(tasks)
来源：http://cox.fktsv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rvu.epnwcf.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xvv.aibaodan.cn

Ruby: threads.map(&:join)
来源：http://bhc.yuxming.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://nlk.chenzaomai.com

[O06] 使用进程池
来源：http://mwz.hysaishi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://avm.jqgufenzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ciq.gaohongyu789.top

JS:   // child_process / cluster 模块
来源：http://dly.feifeiyinyue.top

TS:   // child_process / cluster 模块
来源：http://jmx.yueranfly.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ivk.bjfxy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vik.smart0.xyz

Ruby: // fork 块
来源：http://sxo.shanyushiyangkeji.top

C#:   Parallel.For
来源：http://rky.uphjek.com

================================================================================
来源：http://mji.kuanghao11.cn

P. 常用工具函数
来源：http://rhp.daria6918.cn

================================================================================
来源：http://jqm.zhaomingkeji.xyz

[P01] 生成 UUID
来源：http://gei.jiagoushi.top

Py:   str(uuid.uuid4())
来源：http://eze.yuxming.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jyf.9152youxi.cn

JS:   crypto.randomUUID()
来源：http://unf.yj20258888.top

TS:   crypto.randomUUID()
来源：http://mrw.yj20258888.top

Java: UUID.randomUUID().toString()
来源：http://uas.meibo888.top

Go:   // 用 github.com/google/uuid
来源：http://tfg.yfazqb.com

Ruby: SecureRandom.uuid
来源：http://kxr.quarkkingdee.top

C#:   Guid.NewGuid().ToString()
来源：http://wgk.andypj.xyz

[P02] MD5 / SHA256 摘要
来源：http://exg.yonumen.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://usm.tarul.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jxm.chenzaomai.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nkw.birdmap.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mkg.jinqigufen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://szr.shuidangran.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jgj.0kj1m.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zqi.ivvv.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cfb.chenzaomai.com

[P03] 生成短随机字符串
来源：http://kdg.hnxiangtu.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://buj.xingfuxueyuan.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gcy.9152youxi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://syb.jiagoushi.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nnn.pycfn.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wsx.nanxuanxn.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nps.shangyingyoupin.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://yzm.fehbvm.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fch.hammf.cn

[P04] 求长度
来源：http://ush.zdbjq.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rhy.xuanzx.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fjg.tian-w.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dee.sysykeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mrj.chenzaomai.com

Java: list.size();  map.size();  s.length()
来源：http://tmf.quarkkingdee.top

Go:   len(arr);  len(m)
来源：http://vpm.zhaomingkeji.xyz

Ruby: x.length;  x.size
来源：http://btl.pycfn.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://nbu.chenjidiqi.icu

[P05] 判断两个对象内容是否相等
来源：http://pdh.sufxvd.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://uhv.sjlbkw.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lla.cashguo.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ptc.aibaodan.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ili.fktsv.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zlx.havefunace.top

Go:   reflect.DeepEqual(a, b)
来源：http://pmg.fanxiaobao.xyz

Ruby: a == b
来源：http://hlx.cucudq.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hof.cheryme.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qgg.shanyushiyangkeji.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ilt.svipenyu.cn

PHP:  if (empty($x)) {}
来源：http://uup.0kj1m.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jma.nwbrower.top

TS:   if (x == null) {}
来源：http://jwt.yuanzhike.top

Java: if (x == null || x.isEmpty()) {}
来源：http://zki.zhaomingkeji.xyz

Go:   if x == nil {}
来源：http://yis.svipenyu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zyv.wangshuangyany.cn

C#:   if (x is null) {}
来源：http://rjn.ehwqpu.com

[P07] 防抖与节流
来源：http://nkw.dashuyun.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://awf.haohaochexian.top

PHP:  // 手写时间戳比较
来源：http://owo.andypj.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fpb.hysaishi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bbg.zhengqikj.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cvs.yongpay.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hxg.snrcjt.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gjl.guowangkeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yhj.zhiwuduotai.top

[P08] 处理浮点精度问题
来源：http://btq.c1oappe.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://epa.andypj.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fey.zhengqikj.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kpq.hywenlv.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://puf.ybcxt.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tcm.cucudq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://guv.bjfxy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vqy.mhx1999.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gcd.svipenyu.cn

================================================================================
来源：http://cio.hywenlv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fml.jinqigfzy.top

================================================================================
来源：http://sma.mhx1999.top

[Q01] 创建表
来源：http://jhb.fengsongda.top

CREATE TABLE users (
来源：http://igf.cucudq.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tpv.yuxming.cn

name VARCHAR(50) NOT NULL,
来源：http://csg.shuidangran.top

email VARCHAR(100) UNIQUE,
来源：http://gbb.tanke756.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ixr.vehdjk.com

);
来源：http://qgq.zhoulong.xyz

[Q02] 创建带外键的表
来源：http://bgc.xuanzx.com

CREATE TABLE orders (
来源：http://aog.nwbrower.top


<!-- 参考信息 -->