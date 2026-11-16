代发 wailian999

Py:   if __name__ == "__main__":
来源：http://toa.daria6918.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://frj.zhijiandao.cn

JS:   require.main === module
来源：http://igz.yueranfly.top

TS:   require.main === module
来源：http://uvm.ydjk.org.cn

Java: public static void main(String[] args)
来源：http://vgo.jinqigfzy.top

Go:   func main()
来源：http://txb.andypj.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fbu.nanxinkj.top

C#:   static void Main(string[] args)
来源：http://hwe.xinyue.icu

[M08] 获取系统与运行时信息
来源：http://qkd.sufxvd.cn

Py:   platform.system();  platform.python_version()
来源：http://hqw.nwbrower.top

PHP:  PHP_OS;  phpversion();
来源：http://mpx.gzhubu.top

JS:   process.platform;  process.version
来源：http://nbg.quarkkingdee.top

TS:   process.platform;  process.version
来源：http://gmu.uphjek.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ggi.nwbrower.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://wrz.guowangkeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zyq.ydzc1.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://kls.cheryme.top

================================================================================
来源：http://sbs.wangdashe.top

N. 数据结构与算法
来源：http://qzg.hongshengwenyu.top

================================================================================
来源：http://rvl.316326.xyz

[N01] 二分查找（有序数组）
来源：http://yjh.pengpengdd.cyou

Py:   bisect.bisect_left(arr, x)
来源：http://gmg.yfazqb.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://any.yj20258.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kfv.gogol.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://czw.hfpthk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ciw.ctjpmb.com

Go:   sort.SearchInts(arr, x)
来源：http://rxa.tianlin.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://fjo.bjfxy.top

C#:   Array.BinarySearch(arr, x)
来源：http://fcr.ehwqpu.com

[N02] 排序（工程实践用内置实现）
来源：http://uyz.hammf.cn

Py:   sorted(arr);  arr.sort()
来源：http://nxh.cucudq.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://frw.xylfe.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zcc.zhongyouzk.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://tqm.hnxiangtu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ewm.ctjpmb.com

Go:   slices.Sort(arr)
来源：http://ccx.52xcode.cn

Ruby: arr.sort
来源：http://icz.hongshengwenyu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://dse.fengsongda.top

[N03] 快速排序（分治示例）
来源：http://uor.xylfe.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vnv.guannengcc.top

PHP:  // 递归实现，或用 usort
来源：http://rhv.vqdsnc.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://igg.guowangkeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jmh.ydzc1.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jrq.aibaodan.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oim.dashuyun.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jig.kuanghao11.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fab.hammf.cn

[N04] 斐波那契数列
来源：http://fwz.iojbl.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dwz.hnqzz.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://aeq.havefunace.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yep.yj202588.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qfr.nwbrower.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fhu.dianchejie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hnf.xuanzx.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kgh.guannengcc.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://njv.sufxvd.cn

[N05] 最大公约数
来源：http://yuk.redwolf501.top

Py:   math.gcd(a, b)
来源：http://iua.ywan-chungtsiang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xhi.zhoulong.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mna.hongshengwenyu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dpv.hammf.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zza.hnqzz.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://aox.zhaomingkeji.xyz

Ruby: a.gcd(b)
来源：http://rle.yuxming.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://aqb.smart0.xyz

[N06] 判断回文字符串
来源：http://thn.jyoumei.cn

Py:   s == s[::-1]
来源：http://oda.cheryme.top

PHP:  $s === strrev($s);
来源：http://nnd.yonumen.top

JS:   s === [...s].reverse().join("")
来源：http://mjq.c1oappe.top

TS:   s === [...s].reverse().join("")
来源：http://lon.52xcode.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ezh.ehwqpu.com

Go:   // 双指针从两端比较
来源：http://oik.yj202588.top

Ruby: s == s.reverse
来源：http://mpe.jlsjyb.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://utx.cucudq.cn

[N07] 两数之和（返回下标）
来源：http://vvj.jiagoushi.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xsx.ctjpmb.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bsy.bjfxy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://hdj.ehwqpu.com

TS:   // 手写 Map<string, number>
来源：http://rjw.jlsjyb.cn

Java: // 手写 HashMap
来源：http://qin.uphjek.com

Go:   // 手写 map[int]int
来源：http://pnv.xuanzx.com

Ruby: // 手写 Hash
来源：http://uni.feifeiyinyue.top

C#:   // 手写 Dictionary<int, int>
来源：http://zcf.hongshengwenyu.top

[N08] 生成全排列
来源：http://nac.shangyingyoupin.top

Py:   itertools.permutations(arr)
来源：http://uhe.zhiwuduotai.top

PHP:  // 手写递归交换
来源：http://jrk.dianchejie.cn

JS:   // 手写回溯递归
来源：http://sob.yfazqb.com

TS:   // 手写回溯递归
来源：http://lib.tarul.cn

Java: // 手写回溯递归
来源：http://mjk.zdqjudy.top

Go:   // 手写回溯递归
来源：http://dpf.quarkkingdee.top

Ruby: arr.permutation.to_a
来源：http://nax.316326.xyz

C#:   // 手写回溯递归
来源：http://pyx.ybcxt.top

[N09] 栈与队列
来源：http://gbh.havefunace.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kjn.ydjk.org.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sxz.9152youxi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fyx.zycfv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mty.zhijiandao.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lwp.zhixingplan.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wii.zdqjudy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ewm.havefunace.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://goe.ctjpmb.com

[N10] 链表节点定义
来源：http://rbf.ehwqpu.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wev.tianlin.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://dmi.yj20258888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rzi.zhiwuduotai.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kzh.jinyuanbaomall.cn

Java: class Node { int v; Node next; }
来源：http://msp.fehbvm.com

Go:   type Node struct { V int; Next *Node }
来源：http://lxh.chenjidiqi.icu

Ruby: Node = Struct.new(:v, :next)
来源：http://ijt.ydzc1.top

C#:   class Node { public int V; public Node? Next; }
来源：http://dtu.nanxuanxn.top

[N11] 二叉树中序遍历
来源：http://uns.shzxlz.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mot.havefunace.top

PHP:  // 手写递归函数
来源：http://gcn.hnxiangtu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lqn.316326.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cjh.epnwcf.com

Java: // 手写递归
来源：http://jle.aizwys.cn

Go:   // 手写递归
来源：http://tss.nanxinkj.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tzq.shuidangran.top

C#:   // 手写递归
来源：http://gdk.ehwqpu.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bzv.aibaodan.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sei.hnxiangtu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rgn.xingfuxueyuan.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zeb.sweek.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ssh.hysaishi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jkw.meibo888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tzf.hongshengwenyu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gxo.zhongyouzk.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ldm.9152youxi.cn

================================================================================
来源：http://wuo.nanxinkj.top

O. 并发与异步
来源：http://dqq.epnwcf.com

================================================================================
来源：http://xjf.mhx1999.top

[O01] 启动一个线程
来源：http://esd.yj202588.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ssp.guannengcc.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hig.kuanghao11.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jpx.0kj1m.cn

TS:   // 同 JS
来源：http://drt.ppjwa.cn

Java: new Thread(() -> f()).start()
来源：http://agz.zdqjudy.top

Go:   go f()
来源：http://kgm.vehdjk.com

Ruby: Thread.new { f }
来源：http://uyj.redwolf501.top

C#:   Task.Run(() => F());
来源：http://eyj.ctjpmb.com

[O02] 使用线程池
来源：http://ges.daria6918.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://npo.ydzc1.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dcr.mhx1999.top

JS:   // worker_threads 线程池
来源：http://afr.chenjidiqi.icu

TS:   // worker_threads 线程池
来源：http://iml.pycfn.com

Java: Executors.newFixedThreadPool(4)
来源：http://icf.xinyue.icu

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fhl.sjlbkw.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://elm.ywan-chungtsiang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qhq.jinqigfzy.top

[O03] 加锁保护共享数据
来源：http://tbi.chenzaomai.com

Py:   with lock: shared += 1
来源：http://geo.bbcook.cn

PHP:  // 用 flock() 做文件锁
来源：http://elm.cucudq.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ssu.9152youxi.cn

TS:   // 同 JS
来源：http://jbu.tarul.cn

Java: synchronized (this) { shared++; }
来源：http://amh.wangshuangyany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lyj.tanke756.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wgn.tian-w.cn

C#:   lock (gate) { shared++; }
来源：http://mpq.chenlongwang.top

[O04] 定义异步函数并等待
来源：http://leb.zhiwuduotai.top

Py:   async def f():⏎    await g()
来源：http://oia.uphjek.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vep.fengsongda.top

JS:   async function f() { await g(); }
来源：http://yjd.mhx1999.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://fdp.hfpthk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pex.chenzaomai.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kne.mhx1999.top

Ruby: # 用 Fiber 或 async gem
来源：http://qri.sysykeji.top

C#:   async Task F() { await G(); }
来源：http://kme.vehdjk.com

[O05] 并发执行并等待全部完成
来源：http://dvj.gzhubu.top

Py:   asyncio.gather(*tasks)
来源：http://swy.jyoumei.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gwa.wangshuangyany.cn

JS:   await Promise.all(tasks)
来源：http://zrv.bjfxy.top

TS:   await Promise.all(tasks)
来源：http://avs.ywan-chungtsiang.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lfg.zhiwuduotai.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hul.ybcxt.top

Ruby: threads.map(&:join)
来源：http://bpi.birdmap.top

C#:   await Task.WhenAll(t1, t2)
来源：http://skc.fanxiaobao.xyz

[O06] 使用进程池
来源：http://onl.sufxvd.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zea.sjlbkw.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://eop.cqqwz.cn

JS:   // child_process / cluster 模块
来源：http://fev.cqqwz.cn

TS:   // child_process / cluster 模块
来源：http://imf.cucudq.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cco.bjfxy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tha.guannengcc.top

Ruby: // fork 块
来源：http://wam.ppjwa.cn

C#:   Parallel.For
来源：http://neq.tanke756.top

================================================================================
来源：http://hgh.shanyushiyangkeji.top

P. 常用工具函数
来源：http://kdu.316326.xyz

================================================================================
来源：http://gie.9152youxi.cn

[P01] 生成 UUID
来源：http://ugi.hnqzz.top

Py:   str(uuid.uuid4())
来源：http://ipc.smart0.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zza.gaohongyu789.top

JS:   crypto.randomUUID()
来源：http://ovy.jyoumei.cn

TS:   crypto.randomUUID()
来源：http://ocz.kuanghao11.cn

Java: UUID.randomUUID().toString()
来源：http://yxn.ppjwa.cn

Go:   // 用 github.com/google/uuid
来源：http://iqp.zhixingplan.top

Ruby: SecureRandom.uuid
来源：http://wxr.mhx1999.top

C#:   Guid.NewGuid().ToString()
来源：http://ffa.fehbvm.com

[P02] MD5 / SHA256 摘要
来源：http://vtp.aibaodan.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wgr.zhengqikj.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://jez.vehdjk.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kgn.hywenlv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jjf.pycfn.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://itv.zhengqikj.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ekk.hnqzz.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pkr.smart0.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ktm.ywan-chungtsiang.top

[P03] 生成短随机字符串
来源：http://wty.ybcxt.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lan.epnwcf.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gag.xingfuxueyuan.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bxy.tarul.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nfj.cucudq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jvq.uphjek.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lvn.zdbjq.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rib.zhaomingkeji.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://flp.bbcook.cn

[P04] 求长度
来源：http://hbh.316326.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hsq.wangshuangyany.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pzx.pycfn.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jym.bjfxy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xqu.jyoumei.cn

Java: list.size();  map.size();  s.length()
来源：http://bej.hongshengwenyu.top

Go:   len(arr);  len(m)
来源：http://tnx.fzhhl.top

Ruby: x.length;  x.size
来源：http://hds.yangfankeji.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://ona.52xcode.cn

[P05] 判断两个对象内容是否相等
来源：http://mia.jlsjyb.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hty.fanxiaobao.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yke.cheryme.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kek.tarul.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yyc.vehdjk.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://iwz.daxiang520.top

Go:   reflect.DeepEqual(a, b)
来源：http://ago.fanxiaobao.xyz

Ruby: a == b
来源：http://lsl.jiagoushi.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qxm.zhengqikj.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jwd.redwolf501.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hld.vqdsnc.cn

PHP:  if (empty($x)) {}
来源：http://nxo.tarul.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://csy.andypj.xyz

TS:   if (x == null) {}
来源：http://ogp.sufxvd.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nql.snrcjt.cn

Go:   if x == nil {}
来源：http://yes.xuetiantiany.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ttg.pycfn.com

C#:   if (x is null) {}
来源：http://xvv.meibo888.top

[P07] 防抖与节流
来源：http://hvv.ctjpmb.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zun.nwbrower.top

PHP:  // 手写时间戳比较
来源：http://xst.snrcjt.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aer.jinqigfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://awi.gogol.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cyj.jianghu66.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ajd.yongpay.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ctb.wangshuangyany.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zzg.daria6918.cn

[P08] 处理浮点精度问题
来源：http://zeb.fanxiaobao.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qga.fanxiaobao.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pst.nanxinkj.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ikm.hfpthk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vqu.wangdashe.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://his.ywan-chungtsiang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zkq.chenzaomai.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xib.0kj1m.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://oby.hcnkem.com

================================================================================
来源：http://igs.jlsjyb.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lsl.zhijiandao.cn

================================================================================
来源：http://fzv.jinqigufen.top

[Q01] 创建表
来源：http://vmk.tarul.cn

CREATE TABLE users (
来源：http://xot.jqgufenzy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rxu.haohaochexian.top

name VARCHAR(50) NOT NULL,
来源：http://djq.cdnleiting.top

email VARCHAR(100) UNIQUE,
来源：http://kdx.zdqjudy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xir.zhoulong.xyz

);
来源：http://jgp.daria6918.cn

[Q02] 创建带外键的表
来源：http://sfj.fzhhl.top

CREATE TABLE orders (
来源：http://klx.xziqi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mai.meibo888.top

user_id INT NOT NULL,
来源：http://dpf.fengsongda.top

amount DECIMAL(10, 2),
来源：http://xjm.guowangkeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qdp.jianghu66.top

);
来源：http://ygk.zhijiandao.cn

[Q03] 增加列
来源：http://woh.vqdsnc.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://znn.xuanzx.com

[Q04] 修改列类型
来源：http://iaf.uphjek.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://voc.tanke756.top

[Q05] 重命名列
来源：http://nei.hnqzz.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://otu.jlsjyb.cn

[Q06] 删除列
来源：http://gvq.epnwcf.com

ALTER TABLE users DROP COLUMN age;
来源：http://sex.hywenlv.cn

[Q07] 删除表
来源：http://zxx.dashuyun.cn

DROP TABLE IF EXISTS orders;
来源：http://shr.hysaishi.cn

[Q08] 创建普通索引
来源：http://wck.cheryme.top

CREATE INDEX idx_users_email ON users(email);
来源：http://nwt.uphjek.com

[Q09] 创建唯一索引
来源：http://owg.hysaishi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vqc.havefunace.top

[Q10] 插入单行
来源：http://lhf.yuxming.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vsm.yanxiufei.cn

[Q11] 一次插入多行
来源：http://kxv.tarul.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ywl.kuanghao11.cn

[Q12] 插入后取自增 ID
来源：http://upl.zdqjudy.top

INSERT INTO users (name) VALUES ('C');
来源：http://mlq.gaohongyu789.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gvw.bjfxy.top

[Q13] 忽略重复插入
来源：http://erp.xylfe.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pdx.zycfv.cn


<!-- 参考信息 -->