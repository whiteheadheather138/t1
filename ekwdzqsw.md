代发 wailian999

[M04] 获取当前工作目录
来源：http://bdt.xinyue.icu

Py:   os.getcwd()
来源：http://qwt.daria6918.cn

PHP:  getcwd();
来源：http://dvo.jinqigfzy.top

JS:   process.cwd()
来源：http://abg.hongshengwenyu.top

TS:   process.cwd()
来源：http://clz.dianchejie.cn

Java: Path.of("").toAbsolutePath()
来源：http://mgp.shzxlz.cn

Go:   os.Getwd()
来源：http://any.yongpay.top

Ruby: Dir.pwd
来源：http://vji.hesvh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://naz.kuanghao11.cn

[M05] 设置退出码
来源：http://xls.dianchejie.cn

Py:   sys.exit(1)
来源：http://bhd.vqdsnc.cn

PHP:  exit(1);
来源：http://dro.sjlbkw.cn

JS:   process.exit(1)
来源：http://yuz.hcnkem.com

TS:   process.exit(1)
来源：http://usf.yj20258.top

Java: System.exit(1)
来源：http://bge.hfpthk.cn

Go:   os.Exit(1)
来源：http://mxu.zhiwuduotai.top

Ruby: exit 1
来源：http://ojt.gaohongyu789.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nnj.sjlbkw.cn

[M06] 向标准错误输出
来源：http://ewv.zhijiandao.cn

Py:   print("err", file=sys.stderr)
来源：http://mjy.chenlongwang.top

PHP:  fwrite(STDERR, "err\n");
来源：http://jaq.shanyushiyangtech.top

JS:   console.error("err")
来源：http://cib.hammf.cn

TS:   console.error("err")
来源：http://eiu.nanxuanxn.top

Java: System.err.println("err")
来源：http://del.yvedp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xoa.jqgufenzy.top

Ruby: warn "err"
来源：http://mzq.yanxiufei.cn

C#:   Console.Error.WriteLine("err")
来源：http://fqi.shzxlz.cn

[M07] 判断是否为主入口
来源：http://tny.havefunace.top

Py:   if __name__ == "__main__":
来源：http://dmq.nanxinkj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oic.hcnkem.com

JS:   require.main === module
来源：http://emc.redwolf501.top

TS:   require.main === module
来源：http://qkd.gzhubu.top

Java: public static void main(String[] args)
来源：http://ffv.jlsjyb.cn

Go:   func main()
来源：http://ecw.ppjwa.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vic.jinqigfzy.top

C#:   static void Main(string[] args)
来源：http://ogd.dianchejie.cn

[M08] 获取系统与运行时信息
来源：http://ake.zhongyouzk.top

Py:   platform.system();  platform.python_version()
来源：http://yvx.chenjidiqi.icu

PHP:  PHP_OS;  phpversion();
来源：http://hyr.zdqjudy.top

JS:   process.platform;  process.version
来源：http://irk.gzhubu.top

TS:   process.platform;  process.version
来源：http://uqw.cashguo.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://swc.ctjpmb.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://bsu.xylfe.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vvc.vehdjk.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://pmz.fehbvm.com

================================================================================
来源：http://hoa.zycfv.cn

N. 数据结构与算法
来源：http://ivk.hesvh.cn

================================================================================
来源：http://jnd.shangyingyoupin.top

[N01] 二分查找（有序数组）
来源：http://taw.epnwcf.com

Py:   bisect.bisect_left(arr, x)
来源：http://lzf.daria6918.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ovu.zdqjudy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vyx.redwolf501.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qjt.jinyuanbaomall.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lph.nanxuanxn.top

Go:   sort.SearchInts(arr, x)
来源：http://jzl.ydzc1.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://exo.jlsjyb.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mvl.vehdjk.com

[N02] 排序（工程实践用内置实现）
来源：http://uoy.c1oappe.top

Py:   sorted(arr);  arr.sort()
来源：http://zcf.sxryk.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hli.bjfxy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://lpv.zhaomingkeji.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://yrd.9152youxi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jjs.jqgfzy.top

Go:   slices.Sort(arr)
来源：http://pnl.cashguo.top

Ruby: arr.sort
来源：http://iop.iojbl.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vgq.yvedp.cn

[N03] 快速排序（分治示例）
来源：http://nni.xuetiantiany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fxi.meibo888.top

PHP:  // 递归实现，或用 usort
来源：http://ffk.aizwys.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://due.nanxuanxn.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://efr.havefunace.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://eud.xylfe.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://htf.haohaochexian.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://oyo.vqdsnc.cn

C#:   // 手写递归，或 Array.Sort
来源：http://mmc.sxryk.cn

[N04] 斐波那契数列
来源：http://tup.hesvh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vjj.smart0.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pez.andypj.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tpq.jianghu66.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xtm.ivvv.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zfi.aibaodan.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xuo.fanxiaobao.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://trd.316326.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kjs.bjfxy.top

[N05] 最大公约数
来源：http://kko.jiagoushi.top

Py:   math.gcd(a, b)
来源：http://evk.ppjwa.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xhz.andypj.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wrf.iojbl.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ihy.fanxiaobao.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blv.sxryk.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kmf.dashuyun.cn

Ruby: a.gcd(b)
来源：http://opa.bbcook.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://iyy.yanxiufei.cn

[N06] 判断回文字符串
来源：http://gsw.52xcode.cn

Py:   s == s[::-1]
来源：http://ibt.shuidangran.top

PHP:  $s === strrev($s);
来源：http://szf.mhx1999.top

JS:   s === [...s].reverse().join("")
来源：http://ddv.cqqwz.cn

TS:   s === [...s].reverse().join("")
来源：http://wdj.tanke756.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rzb.gotoacloud.top

Go:   // 双指针从两端比较
来源：http://awz.yueranfly.top

Ruby: s == s.reverse
来源：http://cru.fzhhl.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ndt.redwolf501.top

[N07] 两数之和（返回下标）
来源：http://vfh.zhoulong.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://szc.hnqzz.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nxz.dianchejie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xnv.c1oappe.top

TS:   // 手写 Map<string, number>
来源：http://bcx.aizwys.cn

Java: // 手写 HashMap
来源：http://bla.yfazqb.com

Go:   // 手写 map[int]int
来源：http://wzy.aizwys.cn

Ruby: // 手写 Hash
来源：http://fwz.yj20258.top

C#:   // 手写 Dictionary<int, int>
来源：http://amo.kuanghao11.cn

[N08] 生成全排列
来源：http://rxj.zhixingplan.top

Py:   itertools.permutations(arr)
来源：http://quw.dianchejie.cn

PHP:  // 手写递归交换
来源：http://eex.xziqi.cn

JS:   // 手写回溯递归
来源：http://lal.gzhubu.top

TS:   // 手写回溯递归
来源：http://bim.fktsv.cn

Java: // 手写回溯递归
来源：http://cox.svipenyu.cn

Go:   // 手写回溯递归
来源：http://cpd.fengsongda.top

Ruby: arr.permutation.to_a
来源：http://bih.jinghuilouyu.cn

C#:   // 手写回溯递归
来源：http://fzl.yanxiufei.cn

[N09] 栈与队列
来源：http://bpc.xziqi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://whg.xuanzx.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jil.shzxlz.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://piz.daria6918.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zsy.iojbl.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kle.gogol.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ptj.zhongyouzk.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bbj.iojbl.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mus.gotoacloud.top

[N10] 链表节点定义
来源：http://bzv.shanyushiyangkeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ciz.ctjpmb.com

PHP:  class Node { public $v; public $next = null; }
来源：http://izb.xziqi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://anq.ehwqpu.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://luj.tianlin.xyz

Java: class Node { int v; Node next; }
来源：http://zqn.jqgufenzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://ncs.xuetiantiany.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://usp.feifeiyinyue.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jyd.feifeiyinyue.top

[N11] 二叉树中序遍历
来源：http://wkc.epnwcf.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dhc.jlsjyb.cn

PHP:  // 手写递归函数
来源：http://muc.yj20258888.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xyx.hongshengwenyu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xvl.ivvv.top

Java: // 手写递归
来源：http://zla.bbcook.cn

Go:   // 手写递归
来源：http://sjc.kuanghao11.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://osm.yj202588.top

C#:   // 手写递归
来源：http://yyx.xinyue.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://umq.sweek.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://brt.birdmap.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yll.hnxiangtu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hnt.chenjidiqi.icu

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://unv.zhoulong.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://aqx.feifeiyinyue.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rzj.fktsv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ixn.zhengqikj.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mjc.fktsv.cn

================================================================================
来源：http://nfj.zhaomingkeji.xyz

O. 并发与异步
来源：http://xxz.yonumen.top

================================================================================
来源：http://rvl.xingfuxueyuan.xyz

[O01] 启动一个线程
来源：http://mgi.xziqi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xqf.316326.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hwm.kuanghao11.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bqn.shuidangran.top

TS:   // 同 JS
来源：http://ngz.feifeiyinyue.top

Java: new Thread(() -> f()).start()
来源：http://qts.aibaodan.cn

Go:   go f()
来源：http://dea.zdbjq.cn

Ruby: Thread.new { f }
来源：http://cet.jinyuanbaomall.cn

C#:   Task.Run(() => F());
来源：http://vof.sufxvd.cn

[O02] 使用线程池
来源：http://nwn.ywan-chungtsiang.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://piu.chenjidiqi.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gec.yongpay.top

JS:   // worker_threads 线程池
来源：http://ieu.pycfn.com

TS:   // worker_threads 线程池
来源：http://lub.hongshengwenyu.top

Java: Executors.newFixedThreadPool(4)
来源：http://wew.sysykeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kjx.feifeiyinyue.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ogo.kuanghao11.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hod.hnxiangtu.top

[O03] 加锁保护共享数据
来源：http://xey.yonumen.top

Py:   with lock: shared += 1
来源：http://mfq.fzhhl.top

PHP:  // 用 flock() 做文件锁
来源：http://vdr.feifeiyinyue.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dgr.chenlongwang.top

TS:   // 同 JS
来源：http://hgm.ywan-chungtsiang.top

Java: synchronized (this) { shared++; }
来源：http://kwm.guannengcc.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cml.sysykeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://faj.guannengcc.top

C#:   lock (gate) { shared++; }
来源：http://ong.cucudq.cn

[O04] 定义异步函数并等待
来源：http://jwt.chenlongwang.top

Py:   async def f():⏎    await g()
来源：http://ktp.hongshengwenyu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bfc.zhoulong.xyz

JS:   async function f() { await g(); }
来源：http://qqn.nwbrower.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://mdi.zdbjq.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bpa.guowangkeji.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://enq.svipenyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wev.zycfv.cn

C#:   async Task F() { await G(); }
来源：http://dgc.fengsongda.top

[O05] 并发执行并等待全部完成
来源：http://kmb.zhaomingkeji.xyz

Py:   asyncio.gather(*tasks)
来源：http://gcq.andypj.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://msn.fzhhl.top

JS:   await Promise.all(tasks)
来源：http://lil.zdqjudy.top

TS:   await Promise.all(tasks)
来源：http://ogw.hesvh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mue.c1oappe.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lfk.gzhubu.top

Ruby: threads.map(&:join)
来源：http://ojm.ybcxt.top

C#:   await Task.WhenAll(t1, t2)
来源：http://wtz.tianlin.xyz

[O06] 使用进程池
来源：http://wlg.ywan-chungtsiang.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://unc.52xcode.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://lbk.jiagoushi.top

JS:   // child_process / cluster 模块
来源：http://bwp.fanxiaobao.xyz

TS:   // child_process / cluster 模块
来源：http://csa.xziqi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ksr.shzxlz.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wve.cqqwz.cn

Ruby: // fork 块
来源：http://atd.pycfn.com

C#:   Parallel.For
来源：http://sab.iojbl.cn

================================================================================
来源：http://evz.ppjwa.cn

P. 常用工具函数
来源：http://gxo.ydjk.org.cn

================================================================================
来源：http://eeu.ywan-chungtsiang.top

[P01] 生成 UUID
来源：http://zqs.wangshuangyany.cn

Py:   str(uuid.uuid4())
来源：http://bwy.shzxlz.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pur.kuanghao11.cn

JS:   crypto.randomUUID()
来源：http://dnk.0kj1m.cn

TS:   crypto.randomUUID()
来源：http://zxd.hesvh.cn

Java: UUID.randomUUID().toString()
来源：http://lou.zhaomingkeji.xyz

Go:   // 用 github.com/google/uuid
来源：http://bti.zhixingplan.top

Ruby: SecureRandom.uuid
来源：http://ssd.jyoumei.cn

C#:   Guid.NewGuid().ToString()
来源：http://jzt.zhaomingkeji.xyz

[P02] MD5 / SHA256 摘要
来源：http://ovs.pycfn.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vug.gzhubu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://vbu.hysaishi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cas.andypj.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ghb.birdmap.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kxs.ydjk.org.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uce.ivvv.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ycq.yueranfly.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nnn.epnwcf.com

[P03] 生成短随机字符串
来源：http://pll.nanxinkj.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rms.zhiwuduotai.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mri.ywan-chungtsiang.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hsv.dashuyun.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wpg.haohaochexian.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uxu.c1oappe.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zwg.cucudq.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mtw.birdmap.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://oqo.tarul.cn

[P04] 求长度
来源：http://ocp.chenzaomai.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mre.nanxinkj.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cjd.shuidangran.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://llg.zhaomingkeji.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vcq.aizwys.cn

Java: list.size();  map.size();  s.length()
来源：http://lwy.52xcode.cn

Go:   len(arr);  len(m)
来源：http://mfb.zhaomingkeji.xyz

Ruby: x.length;  x.size
来源：http://sre.wangshuangyany.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rtq.zhaomingkeji.xyz

[P05] 判断两个对象内容是否相等
来源：http://zte.zhengqikj.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://luv.jinghuilouyu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ayu.jinqigfzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://skx.tanke756.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gct.mhx1999.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ulv.shanyushiyangtech.top

Go:   reflect.DeepEqual(a, b)
来源：http://are.jianghu66.top

Ruby: a == b
来源：http://tzx.xuanzx.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://otp.tianlin.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://taw.hnqzz.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vta.gogol.net.cn

PHP:  if (empty($x)) {}
来源：http://seb.ivvv.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yih.aibaodan.cn

TS:   if (x == null) {}
来源：http://ieg.sufxvd.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zik.quarkkingdee.top

Go:   if x == nil {}
来源：http://wjx.fktsv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qxa.zycfv.cn

C#:   if (x is null) {}
来源：http://lrz.epnwcf.com

[P07] 防抖与节流
来源：http://ook.chenjidiqi.icu

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yzg.fengsongda.top

PHP:  // 手写时间戳比较
来源：http://hod.bjfxy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xsx.andypj.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mxg.uphjek.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lkv.zhaomingkeji.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dyy.ybcxt.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://xgr.hnxiangtu.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rzr.yvedp.cn

[P08] 处理浮点精度问题
来源：http://oaw.tanke756.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yim.mhx1999.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vpn.shangyingyoupin.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jye.pengpengdd.cyou

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vvd.zhiwuduotai.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bjl.aizwys.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://osf.vqdsnc.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bor.cucudq.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hhx.haohaochexian.top

================================================================================
来源：http://zai.jinyuanbaomall.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fva.epnwcf.com

================================================================================
来源：http://wrs.ppjwa.cn

[Q01] 创建表
来源：http://xgp.zdqjudy.top

CREATE TABLE users (
来源：http://axb.hnqzz.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cgo.vehdjk.com

name VARCHAR(50) NOT NULL,
来源：http://eum.snrcjt.cn

email VARCHAR(100) UNIQUE,
来源：http://eps.cashguo.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ndw.wangshuangyany.cn

);
来源：http://nfy.fengsongda.top

[Q02] 创建带外键的表
来源：http://qgy.ctjpmb.com

CREATE TABLE orders (
来源：http://xja.iojbl.cn


<!-- 参考信息 -->