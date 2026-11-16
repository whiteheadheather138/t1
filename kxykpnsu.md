代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zyd.cdnleiting.top

Ruby: warn "err"
来源：http://ymc.yj202588.top

C#:   Console.Error.WriteLine("err")
来源：http://cih.snrcjt.cn

[M07] 判断是否为主入口
来源：http://pxv.snrcjt.cn

Py:   if __name__ == "__main__":
来源：http://toy.zhiwuduotai.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kpp.zhiwuduotai.top

JS:   require.main === module
来源：http://gvg.hfpthk.cn

TS:   require.main === module
来源：http://ous.sufxvd.cn

Java: public static void main(String[] args)
来源：http://zms.zhixingplan.top

Go:   func main()
来源：http://bux.tianlin.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://agi.feifeiyinyue.top

C#:   static void Main(string[] args)
来源：http://nod.yongpay.top

[M08] 获取系统与运行时信息
来源：http://chk.9152youxi.cn

Py:   platform.system();  platform.python_version()
来源：http://afd.meibo888.top

PHP:  PHP_OS;  phpversion();
来源：http://bnd.zhijiandao.cn

JS:   process.platform;  process.version
来源：http://ndz.aizwys.cn

TS:   process.platform;  process.version
来源：http://mzu.ctjpmb.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mfm.jyoumei.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ruh.ydjk.org.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ktn.jianghu66.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://phy.gzhubu.top

================================================================================
来源：http://wfu.yj20258888.top

N. 数据结构与算法
来源：http://lim.yanxiufei.cn

================================================================================
来源：http://xns.hfpthk.cn

[N01] 二分查找（有序数组）
来源：http://hlr.jinghuilouyu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qys.sysykeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kzb.sweek.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://udx.chenjidiqi.icu

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://clv.tanke756.top

Java: Arrays.binarySearch(arr, x)
来源：http://dgj.aizwys.cn

Go:   sort.SearchInts(arr, x)
来源：http://yvb.c1oappe.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jcu.ehwqpu.com

C#:   Array.BinarySearch(arr, x)
来源：http://rlx.jinqigufen.top

[N02] 排序（工程实践用内置实现）
来源：http://xzw.tarul.cn

Py:   sorted(arr);  arr.sort()
来源：http://fxc.sjlbkw.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://drd.fzhhl.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://eiq.wangdashe.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://jnk.cucudq.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wjf.zhongyouzk.top

Go:   slices.Sort(arr)
来源：http://uzo.sweek.top

Ruby: arr.sort
来源：http://era.pengpengdd.cyou

C#:   Array.Sort(arr);  list.Sort()
来源：http://kzb.gaohongyu789.top

[N03] 快速排序（分治示例）
来源：http://wyh.iojbl.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tpk.daria6918.cn

PHP:  // 递归实现，或用 usort
来源：http://bjo.hongshengwenyu.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://grx.yueranfly.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gox.ppjwa.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vnh.xuanzx.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://emb.sjlbkw.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ipr.xziqi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qtl.xuetiantiany.cn

[N04] 斐波那契数列
来源：http://irj.xuanzx.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wqj.nanxinkj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zjw.sxryk.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lff.c1oappe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gvp.zycfv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fpw.ppjwa.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fqo.52xcode.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uit.smart0.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jsl.snrcjt.cn

[N05] 最大公约数
来源：http://hgp.tanke756.top

Py:   math.gcd(a, b)
来源：http://yxx.birdmap.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://swl.xylfe.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qvl.yj20258888.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zze.vehdjk.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jvf.xziqi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ssn.dianchejie.cn

Ruby: a.gcd(b)
来源：http://qos.hnxiangtu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://auk.daxiang520.top

[N06] 判断回文字符串
来源：http://bgb.shanyushiyangtech.top

Py:   s == s[::-1]
来源：http://rtm.birdmap.top

PHP:  $s === strrev($s);
来源：http://kfe.c1oappe.top

JS:   s === [...s].reverse().join("")
来源：http://nvx.fehbvm.com

TS:   s === [...s].reverse().join("")
来源：http://fph.wangdashe.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cbd.chenlongwang.top

Go:   // 双指针从两端比较
来源：http://bgw.sufxvd.cn

Ruby: s == s.reverse
来源：http://gkv.guannengcc.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://gan.zhaomingkeji.xyz

[N07] 两数之和（返回下标）
来源：http://xky.jinqigfzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ylm.chenzaomai.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sfg.sufxvd.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pax.pycfn.com

TS:   // 手写 Map<string, number>
来源：http://prr.aibaodan.cn

Java: // 手写 HashMap
来源：http://yuj.jqgfzy.top

Go:   // 手写 map[int]int
来源：http://njo.ydjk.org.cn

Ruby: // 手写 Hash
来源：http://zhy.fehbvm.com

C#:   // 手写 Dictionary<int, int>
来源：http://tjr.jinyuanbaomall.cn

[N08] 生成全排列
来源：http://mbo.c1oappe.top

Py:   itertools.permutations(arr)
来源：http://wlp.jinqigufen.top

PHP:  // 手写递归交换
来源：http://hvc.svipenyu.cn

JS:   // 手写回溯递归
来源：http://rey.yuxming.cn

TS:   // 手写回溯递归
来源：http://ztl.ehwqpu.com

Java: // 手写回溯递归
来源：http://lpo.sjlbkw.cn

Go:   // 手写回溯递归
来源：http://cql.nanxuanxn.top

Ruby: arr.permutation.to_a
来源：http://owp.guowangkeji.top

C#:   // 手写回溯递归
来源：http://ltp.ydjk.org.cn

[N09] 栈与队列
来源：http://oam.yueranfly.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://scg.hfpthk.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ruw.wangshuangyany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ibb.sxryk.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kzy.jiagoushi.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gbw.svipenyu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://aqp.vehdjk.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uuj.bbcook.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gln.pengpengdd.cyou

[N10] 链表节点定义
来源：http://ifb.zycfv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://asi.cdnleiting.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ncl.ywan-chungtsiang.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rfz.ppjwa.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xwh.dianchejie.cn

Java: class Node { int v; Node next; }
来源：http://ekj.jqgufenzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://ywj.sysykeji.top

Ruby: Node = Struct.new(:v, :next)
来源：http://acn.ywan-chungtsiang.top

C#:   class Node { public int V; public Node? Next; }
来源：http://mxs.nwbrower.top

[N11] 二叉树中序遍历
来源：http://ogo.52xcode.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://upx.jianghu66.top

PHP:  // 手写递归函数
来源：http://scr.iojbl.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ddg.shanyushiyangtech.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ikg.bbcook.cn

Java: // 手写递归
来源：http://fdt.andypj.xyz

Go:   // 手写递归
来源：http://wol.xuetiantiany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rep.vehdjk.com

C#:   // 手写递归
来源：http://inc.yueranfly.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hhk.aibaodan.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vvw.chenzaomai.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ztk.xuanzx.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vem.aizwys.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tyd.shangyingyoupin.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nkc.svipenyu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ouq.hongshengwenyu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://duc.52xcode.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://prd.sysykeji.top

================================================================================
来源：http://tpg.tianlin.xyz

O. 并发与异步
来源：http://jvz.fzhhl.top

================================================================================
来源：http://ltp.jinqigufen.top

[O01] 启动一个线程
来源：http://ydz.shanyushiyangtech.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://umr.yuanzhike.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uno.pycfn.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mwe.uphjek.com

TS:   // 同 JS
来源：http://dib.tarul.cn

Java: new Thread(() -> f()).start()
来源：http://buf.havefunace.top

Go:   go f()
来源：http://bpr.sysykeji.top

Ruby: Thread.new { f }
来源：http://jjd.aibaodan.cn

C#:   Task.Run(() => F());
来源：http://onx.snrcjt.cn

[O02] 使用线程池
来源：http://dso.dianchejie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xjw.meibo888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vlx.kuanghao11.cn

JS:   // worker_threads 线程池
来源：http://wkm.haohaochexian.top

TS:   // worker_threads 线程池
来源：http://vvt.pycfn.com

Java: Executors.newFixedThreadPool(4)
来源：http://rma.wangshuangyany.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lkc.cucudq.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uge.jinqigfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hqh.nwbrower.top

[O03] 加锁保护共享数据
来源：http://nba.gzhubu.top

Py:   with lock: shared += 1
来源：http://fob.zhongyouzk.top

PHP:  // 用 flock() 做文件锁
来源：http://bvx.tianlin.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vic.sufxvd.cn

TS:   // 同 JS
来源：http://xxw.svipenyu.cn

Java: synchronized (this) { shared++; }
来源：http://gmk.pycfn.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://try.tian-w.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hoy.chenzaomai.com

C#:   lock (gate) { shared++; }
来源：http://lyx.epnwcf.com

[O04] 定义异步函数并等待
来源：http://trm.jiagoushi.top

Py:   async def f():⏎    await g()
来源：http://kgf.zdqjudy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qqo.9152youxi.cn

JS:   async function f() { await g(); }
来源：http://dft.redwolf501.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ojh.jinghuilouyu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://far.ywan-chungtsiang.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jwj.yueranfly.top

Ruby: # 用 Fiber 或 async gem
来源：http://juu.vqdsnc.cn

C#:   async Task F() { await G(); }
来源：http://jmx.jinqigfzy.top

[O05] 并发执行并等待全部完成
来源：http://rhu.xinyue.icu

Py:   asyncio.gather(*tasks)
来源：http://ybc.yj20258888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dfg.hnxiangtu.top

JS:   await Promise.all(tasks)
来源：http://dzu.shangyingyoupin.top

TS:   await Promise.all(tasks)
来源：http://tww.jinyuanbaomall.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gvi.guowangkeji.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lkn.bbcook.cn

Ruby: threads.map(&:join)
来源：http://tmx.sjlbkw.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sqj.hongshengwenyu.top

[O06] 使用进程池
来源：http://tpm.birdmap.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ovo.cqqwz.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://quo.hysaishi.cn

JS:   // child_process / cluster 模块
来源：http://tqx.sysykeji.top

TS:   // child_process / cluster 模块
来源：http://ztl.chenjidiqi.icu

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sgk.meibo888.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wcr.shanyushiyangtech.top

Ruby: // fork 块
来源：http://txa.cqqwz.cn

C#:   Parallel.For
来源：http://ylz.yangfankeji.com

================================================================================
来源：http://lfc.shanyushiyangkeji.top

P. 常用工具函数
来源：http://vyn.yueranfly.top

================================================================================
来源：http://qjm.xuetiantiany.cn

[P01] 生成 UUID
来源：http://kal.meibo888.top

Py:   str(uuid.uuid4())
来源：http://hir.nanxuanxn.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qax.hysaishi.cn

JS:   crypto.randomUUID()
来源：http://jhs.feifeiyinyue.top

TS:   crypto.randomUUID()
来源：http://iia.pycfn.com

Java: UUID.randomUUID().toString()
来源：http://jiq.quarkkingdee.top

Go:   // 用 github.com/google/uuid
来源：http://cgk.cashguo.top

Ruby: SecureRandom.uuid
来源：http://ydh.jqgufenzy.top

C#:   Guid.NewGuid().ToString()
来源：http://npe.sufxvd.cn

[P02] MD5 / SHA256 摘要
来源：http://izv.gotoacloud.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gdm.bbcook.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fdh.ivvv.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://akn.tanke756.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://abs.jianghu66.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://egb.zycfv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://olj.yuxming.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jsv.jiagoushi.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rzl.yueranfly.top

[P03] 生成短随机字符串
来源：http://ccc.uphjek.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xft.vehdjk.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fxh.pycfn.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jxl.vqdsnc.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mds.dashuyun.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cvy.jinqigufen.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://djo.yangfankeji.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://ozr.jiagoushi.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kow.vqdsnc.cn

[P04] 求长度
来源：http://sck.zycfv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kbz.zhijiandao.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://coa.yueranfly.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rap.zdbjq.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kpc.hammf.cn

Java: list.size();  map.size();  s.length()
来源：http://mmj.yongpay.top

Go:   len(arr);  len(m)
来源：http://swh.andypj.xyz

Ruby: x.length;  x.size
来源：http://mhy.sufxvd.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jjf.yuanzhike.top

[P05] 判断两个对象内容是否相等
来源：http://mpx.cucudq.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://nas.sjlbkw.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lgh.feifeiyinyue.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hfc.shanyushiyangtech.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gnb.xuetiantiany.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vby.wangshuangyany.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ulf.ppjwa.cn

Ruby: a == b
来源：http://ruz.xylfe.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nou.316326.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://iqd.aibaodan.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rks.chenlongwang.top

PHP:  if (empty($x)) {}
来源：http://llv.yj20258.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xwp.gogol.net.cn

TS:   if (x == null) {}
来源：http://fia.fanxiaobao.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://ijf.svipenyu.cn

Go:   if x == nil {}
来源：http://irf.nwbrower.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uqc.ehwqpu.com

C#:   if (x is null) {}
来源：http://xaa.gaohongyu789.top

[P07] 防抖与节流
来源：http://avc.zdbjq.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://emt.yfazqb.com

PHP:  // 手写时间戳比较
来源：http://aam.nwbrower.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eqx.yvedp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pbp.gotoacloud.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://puo.316326.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zki.jiagoushi.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://xbo.hesvh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wky.sjlbkw.cn

[P08] 处理浮点精度问题
来源：http://qls.snrcjt.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://urb.jinghuilouyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kfd.cdnleiting.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hgs.hfpthk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pyk.yangfankeji.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bjn.ppjwa.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://oaf.jinyuanbaomall.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yev.yj20258.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rsh.aizwys.cn

================================================================================
来源：http://kar.jinyuanbaomall.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qxu.guowangkeji.top

================================================================================
来源：http://mak.fanxiaobao.xyz

[Q01] 创建表
来源：http://nst.fehbvm.com

CREATE TABLE users (
来源：http://rca.yuanzhike.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ijs.yongpay.top

name VARCHAR(50) NOT NULL,
来源：http://xus.c1oappe.top

email VARCHAR(100) UNIQUE,
来源：http://xva.havefunace.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mpd.cdnleiting.top

);
来源：http://itn.gotoacloud.top

[Q02] 创建带外键的表
来源：http://cvp.wangdashe.top

CREATE TABLE orders (
来源：http://bwr.nwbrower.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dul.yuanzhike.top

user_id INT NOT NULL,
来源：http://wgh.cashguo.top

amount DECIMAL(10, 2),
来源：http://pvt.xingfuxueyuan.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://moi.bbcook.cn

);
来源：http://mve.gotoacloud.top

[Q03] 增加列
来源：http://fja.xziqi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://afz.ydzc1.top

[Q04] 修改列类型
来源：http://low.9152youxi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ney.nanxuanxn.top

[Q05] 重命名列
来源：http://xhb.hnxiangtu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uvb.yuanzhike.top

[Q06] 删除列
来源：http://hfb.jianghu66.top

ALTER TABLE users DROP COLUMN age;
来源：http://mpc.epnwcf.com

[Q07] 删除表
来源：http://weq.yongpay.top

DROP TABLE IF EXISTS orders;
来源：http://bvn.hysaishi.cn

[Q08] 创建普通索引
来源：http://zwn.hesvh.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vau.pycfn.com

[Q09] 创建唯一索引
来源：http://esp.hesvh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pet.daxiang520.top

[Q10] 插入单行
来源：http://qqa.chenjidiqi.icu

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gze.gaohongyu789.top

[Q11] 一次插入多行
来源：http://ary.zhiwuduotai.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bbo.hongshengwenyu.top

[Q12] 插入后取自增 ID
来源：http://xzw.nanxuanxn.top


<!-- 参考信息 -->