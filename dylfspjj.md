代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://uva.shanyushiyangkeji.top

[M05] 设置退出码
来源：http://rds.chenlongwang.top

Py:   sys.exit(1)
来源：http://vyp.cashguo.top

PHP:  exit(1);
来源：http://lzy.pycfn.com

JS:   process.exit(1)
来源：http://esm.birdmap.top

TS:   process.exit(1)
来源：http://uqf.jqgfzy.top

Java: System.exit(1)
来源：http://lio.smart0.xyz

Go:   os.Exit(1)
来源：http://egg.quarkkingdee.top

Ruby: exit 1
来源：http://qmj.yangfankeji.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nba.chenlongwang.top

[M06] 向标准错误输出
来源：http://jgr.yj20258888.top

Py:   print("err", file=sys.stderr)
来源：http://ynv.jqgfzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://our.316326.xyz

JS:   console.error("err")
来源：http://uze.hysaishi.cn

TS:   console.error("err")
来源：http://rwd.hywenlv.cn

Java: System.err.println("err")
来源：http://fyl.gogol.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bxg.smart0.xyz

Ruby: warn "err"
来源：http://bus.52xcode.cn

C#:   Console.Error.WriteLine("err")
来源：http://xny.yueranfly.top

[M07] 判断是否为主入口
来源：http://fqg.sxryk.cn

Py:   if __name__ == "__main__":
来源：http://bga.yvedp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oyg.zhaomingkeji.xyz

JS:   require.main === module
来源：http://lzk.sjlbkw.cn

TS:   require.main === module
来源：http://aef.yuanzhike.top

Java: public static void main(String[] args)
来源：http://wsi.aibaodan.cn

Go:   func main()
来源：http://etl.jinqigufen.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jqd.yangfankeji.com

C#:   static void Main(string[] args)
来源：http://nxs.guowangkeji.top

[M08] 获取系统与运行时信息
来源：http://wrc.wangshuangyany.cn

Py:   platform.system();  platform.python_version()
来源：http://pql.kuanghao11.cn

PHP:  PHP_OS;  phpversion();
来源：http://hvi.ybcxt.top

JS:   process.platform;  process.version
来源：http://hva.tarul.cn

TS:   process.platform;  process.version
来源：http://wzz.hesvh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tbm.feifeiyinyue.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://oau.9152youxi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zid.guannengcc.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://thq.chenjidiqi.icu

================================================================================
来源：http://wcw.pengpengdd.cyou

N. 数据结构与算法
来源：http://opb.sufxvd.cn

================================================================================
来源：http://glp.pengpengdd.cyou

[N01] 二分查找（有序数组）
来源：http://rew.yuanzhike.top

Py:   bisect.bisect_left(arr, x)
来源：http://vjq.hysaishi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yib.smart0.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://goe.zhengqikj.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kge.cdnleiting.top

Java: Arrays.binarySearch(arr, x)
来源：http://dwu.yvedp.cn

Go:   sort.SearchInts(arr, x)
来源：http://lyu.kuanghao11.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ftd.hnxiangtu.top

C#:   Array.BinarySearch(arr, x)
来源：http://uin.pycfn.com

[N02] 排序（工程实践用内置实现）
来源：http://zga.haohaochexian.top

Py:   sorted(arr);  arr.sort()
来源：http://rrj.yanxiufei.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yvn.ywan-chungtsiang.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://shk.zhixingplan.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://het.sweek.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bpt.wangshuangyany.cn

Go:   slices.Sort(arr)
来源：http://nfg.zhongyouzk.top

Ruby: arr.sort
来源：http://ykc.svipenyu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qwa.yuxming.cn

[N03] 快速排序（分治示例）
来源：http://tdo.zdbjq.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ktj.yvedp.cn

PHP:  // 递归实现，或用 usort
来源：http://ull.yangfankeji.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://viy.hywenlv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hrc.xziqi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cce.pengpengdd.cyou

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oto.tanke756.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vsn.fzhhl.top

C#:   // 手写递归，或 Array.Sort
来源：http://dbj.ydzc1.top

[N04] 斐波那契数列
来源：http://pfn.tian-w.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wyv.haohaochexian.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zsx.ybcxt.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pny.cucudq.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qgu.gzhubu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fym.sufxvd.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nnf.redwolf501.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gzt.zhiwuduotai.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://erx.chenjidiqi.icu

[N05] 最大公约数
来源：http://spp.hnqzz.top

Py:   math.gcd(a, b)
来源：http://tyh.jinyuanbaomall.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hle.jinyuanbaomall.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bgy.c1oappe.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hwz.hcnkem.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vki.tanke756.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ygt.ctjpmb.com

Ruby: a.gcd(b)
来源：http://ufy.fanxiaobao.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wdh.0kj1m.cn

[N06] 判断回文字符串
来源：http://ynh.wangshuangyany.cn

Py:   s == s[::-1]
来源：http://nac.jqgfzy.top

PHP:  $s === strrev($s);
来源：http://kfo.tanke756.top

JS:   s === [...s].reverse().join("")
来源：http://vbm.jinyuanbaomall.cn

TS:   s === [...s].reverse().join("")
来源：http://pds.jinghuilouyu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jzf.guannengcc.top

Go:   // 双指针从两端比较
来源：http://mbb.dashuyun.cn

Ruby: s == s.reverse
来源：http://lpy.vqdsnc.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wjn.ppjwa.cn

[N07] 两数之和（返回下标）
来源：http://pbu.vehdjk.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rgs.vehdjk.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hpe.yanxiufei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pxq.kuanghao11.cn

TS:   // 手写 Map<string, number>
来源：http://bvw.gzhubu.top

Java: // 手写 HashMap
来源：http://fzg.yongpay.top

Go:   // 手写 map[int]int
来源：http://jcf.pycfn.com

Ruby: // 手写 Hash
来源：http://efx.yj20258888.top

C#:   // 手写 Dictionary<int, int>
来源：http://pzx.bbcook.cn

[N08] 生成全排列
来源：http://rpv.hfpthk.cn

Py:   itertools.permutations(arr)
来源：http://wzy.yj20258.top

PHP:  // 手写递归交换
来源：http://mfj.yj20258888.top

JS:   // 手写回溯递归
来源：http://tlk.hnqzz.top

TS:   // 手写回溯递归
来源：http://pxu.jinqigufen.top

Java: // 手写回溯递归
来源：http://plw.fzhhl.top

Go:   // 手写回溯递归
来源：http://woe.fzhhl.top

Ruby: arr.permutation.to_a
来源：http://acq.hammf.cn

C#:   // 手写回溯递归
来源：http://joi.hnqzz.top

[N09] 栈与队列
来源：http://zhd.gzhubu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://udf.ywan-chungtsiang.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qwa.gaohongyu789.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jao.fzhhl.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cxw.sjlbkw.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lis.gzhubu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rhq.yj20258.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ynf.pengpengdd.cyou

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sru.guannengcc.top

[N10] 链表节点定义
来源：http://fcm.shzxlz.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gyx.zhiwuduotai.top

PHP:  class Node { public $v; public $next = null; }
来源：http://nkv.bjfxy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uzg.cdnleiting.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://svn.yj20258.top

Java: class Node { int v; Node next; }
来源：http://shx.jyoumei.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cja.zhengqikj.top

Ruby: Node = Struct.new(:v, :next)
来源：http://rjq.gogol.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jap.cashguo.top

[N11] 二叉树中序遍历
来源：http://mdh.yfazqb.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uyn.gzhubu.top

PHP:  // 手写递归函数
来源：http://xjn.nanxinkj.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ebg.guannengcc.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yhv.hesvh.cn

Java: // 手写递归
来源：http://amq.mhx1999.top

Go:   // 手写递归
来源：http://wmm.uphjek.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sju.hnqzz.top

C#:   // 手写递归
来源：http://osj.hesvh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://irx.iojbl.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nqs.yueranfly.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cco.pengpengdd.cyou

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://buk.mhx1999.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jfy.havefunace.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gwc.yonumen.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vtf.yuanzhike.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cvl.daxiang520.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cvt.yj20258.top

================================================================================
来源：http://pdh.zhixingplan.top

O. 并发与异步
来源：http://ter.smart0.xyz

================================================================================
来源：http://ebu.zhengqikj.top

[O01] 启动一个线程
来源：http://qth.xuanzx.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nls.ywan-chungtsiang.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yyx.316326.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fcp.ivvv.top

TS:   // 同 JS
来源：http://hnq.hnqzz.top

Java: new Thread(() -> f()).start()
来源：http://ecn.cqqwz.cn

Go:   go f()
来源：http://jcu.9152youxi.cn

Ruby: Thread.new { f }
来源：http://zam.uphjek.com

C#:   Task.Run(() => F());
来源：http://onq.cheryme.top

[O02] 使用线程池
来源：http://tma.sxryk.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nqn.shuidangran.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vxm.tanke756.top

JS:   // worker_threads 线程池
来源：http://kyc.xylfe.cn

TS:   // worker_threads 线程池
来源：http://qmj.jinghuilouyu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://cer.jqgfzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tbz.zhixingplan.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lus.vqdsnc.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lcf.yj202588.top

[O03] 加锁保护共享数据
来源：http://yfw.jianghu66.top

Py:   with lock: shared += 1
来源：http://kti.ydzc1.top

PHP:  // 用 flock() 做文件锁
来源：http://zjs.hnqzz.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ihi.quarkkingdee.top

TS:   // 同 JS
来源：http://kak.316326.xyz

Java: synchronized (this) { shared++; }
来源：http://ixh.nwbrower.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://acw.jinqigfzy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://acb.gogol.net.cn

C#:   lock (gate) { shared++; }
来源：http://vrs.cashguo.top

[O04] 定义异步函数并等待
来源：http://ayk.nanxinkj.top

Py:   async def f():⏎    await g()
来源：http://ysn.vqdsnc.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ppu.quarkkingdee.top

JS:   async function f() { await g(); }
来源：http://hsn.vehdjk.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://sav.xuetiantiany.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rvq.aibaodan.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ctw.meibo888.top

Ruby: # 用 Fiber 或 async gem
来源：http://wwc.dianchejie.cn

C#:   async Task F() { await G(); }
来源：http://fdu.vqdsnc.cn

[O05] 并发执行并等待全部完成
来源：http://euq.nanxuanxn.top

Py:   asyncio.gather(*tasks)
来源：http://jtl.xuetiantiany.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zgb.sweek.top

JS:   await Promise.all(tasks)
来源：http://nar.xinyue.icu

TS:   await Promise.all(tasks)
来源：http://heq.hysaishi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xnf.ehwqpu.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://iza.vehdjk.com

Ruby: threads.map(&:join)
来源：http://jhr.nanxuanxn.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ojn.c1oappe.top

[O06] 使用进程池
来源：http://khl.shuidangran.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bgt.jinghuilouyu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zvb.xuetiantiany.cn

JS:   // child_process / cluster 模块
来源：http://wsc.zhaomingkeji.xyz

TS:   // child_process / cluster 模块
来源：http://uyc.hongshengwenyu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gev.zdqjudy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fze.yanxiufei.cn

Ruby: // fork 块
来源：http://oap.pycfn.com

C#:   Parallel.For
来源：http://ifz.yfazqb.com

================================================================================
来源：http://iym.yvedp.cn

P. 常用工具函数
来源：http://enc.gaohongyu789.top

================================================================================
来源：http://lmc.c1oappe.top

[P01] 生成 UUID
来源：http://fim.zdbjq.cn

Py:   str(uuid.uuid4())
来源：http://kgm.hammf.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://emp.yongpay.top

JS:   crypto.randomUUID()
来源：http://qyi.hongshengwenyu.top

TS:   crypto.randomUUID()
来源：http://lbg.jlsjyb.cn

Java: UUID.randomUUID().toString()
来源：http://hcq.nanxuanxn.top

Go:   // 用 github.com/google/uuid
来源：http://gjy.tianlin.xyz

Ruby: SecureRandom.uuid
来源：http://nie.pengpengdd.cyou

C#:   Guid.NewGuid().ToString()
来源：http://gsq.cqqwz.cn

[P02] MD5 / SHA256 摘要
来源：http://dqf.jianghu66.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nej.aibaodan.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xqm.birdmap.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bzw.zhijiandao.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uwz.zhiwuduotai.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://czg.tarul.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kms.vehdjk.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pla.hywenlv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zta.jyoumei.cn

[P03] 生成短随机字符串
来源：http://ybv.yonumen.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fyv.fehbvm.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jqp.yuxming.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hui.feifeiyinyue.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wcb.hongshengwenyu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jnd.zdqjudy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dhx.jinqigfzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://zjv.nwbrower.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rbg.cucudq.cn

[P04] 求长度
来源：http://een.shanyushiyangtech.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dmv.jinqigufen.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fnm.chenzaomai.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zyz.hcnkem.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mzg.mhx1999.top

Java: list.size();  map.size();  s.length()
来源：http://hup.tianlin.xyz

Go:   len(arr);  len(m)
来源：http://eci.zdbjq.cn

Ruby: x.length;  x.size
来源：http://gea.xinyue.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://tey.ybcxt.top

[P05] 判断两个对象内容是否相等
来源：http://eea.uphjek.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://dvf.jyoumei.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://slq.fktsv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://osd.havefunace.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xbd.tian-w.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vbg.jqgufenzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://qvm.dianchejie.cn

Ruby: a == b
来源：http://nak.wangdashe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dpj.yuxming.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lge.wangdashe.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lhm.tanke756.top

PHP:  if (empty($x)) {}
来源：http://pvn.c1oappe.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gbh.xuetiantiany.cn

TS:   if (x == null) {}
来源：http://sdq.nanxinkj.top

Java: if (x == null || x.isEmpty()) {}
来源：http://mli.birdmap.top

Go:   if x == nil {}
来源：http://zdu.zhongyouzk.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nwy.quarkkingdee.top

C#:   if (x is null) {}
来源：http://aoc.epnwcf.com

[P07] 防抖与节流
来源：http://cmo.pycfn.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wuz.guowangkeji.top

PHP:  // 手写时间戳比较
来源：http://zmh.jinghuilouyu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rxi.hongshengwenyu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eym.jqgufenzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kfo.gaohongyu789.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zpn.yj202588.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wck.daxiang520.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://unw.vqdsnc.cn

[P08] 处理浮点精度问题
来源：http://lqh.yj20258888.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lxz.iojbl.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://avh.yangfankeji.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wtu.yj202588.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rjc.wangshuangyany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://brm.yfazqb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iuv.c1oappe.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yee.feifeiyinyue.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mtq.xylfe.cn

================================================================================
来源：http://bnf.cheryme.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://orc.ydjk.org.cn

================================================================================
来源：http://upt.zycfv.cn

[Q01] 创建表
来源：http://kia.yanxiufei.cn

CREATE TABLE users (
来源：http://evw.fanxiaobao.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vqt.zhaomingkeji.xyz

name VARCHAR(50) NOT NULL,
来源：http://bkr.hesvh.cn

email VARCHAR(100) UNIQUE,
来源：http://uqv.bbcook.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://szx.ydzc1.top

);
来源：http://ihv.sysykeji.top

[Q02] 创建带外键的表
来源：http://dkc.ivvv.top

CREATE TABLE orders (
来源：http://bvq.nwbrower.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://abn.sxryk.cn

user_id INT NOT NULL,
来源：http://eiy.hnqzz.top

amount DECIMAL(10, 2),
来源：http://hts.9152youxi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wox.jianghu66.top

);
来源：http://fkc.yfazqb.com

[Q03] 增加列
来源：http://ayp.pengpengdd.cyou

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rld.chenlongwang.top

[Q04] 修改列类型
来源：http://dnr.yueranfly.top


<!-- 参考信息 -->