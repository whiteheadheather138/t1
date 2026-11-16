代发 wailian999

Java: public static void main(String[] args)
来源：http://org.c1oappe.top

Go:   func main()
来源：http://fln.0kj1m.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tot.zdqjudy.top

C#:   static void Main(string[] args)
来源：http://pbk.yuanzhike.top

[M08] 获取系统与运行时信息
来源：http://yrb.tianlin.xyz

Py:   platform.system();  platform.python_version()
来源：http://nnt.cqqwz.cn

PHP:  PHP_OS;  phpversion();
来源：http://lym.sxryk.cn

JS:   process.platform;  process.version
来源：http://rvv.ehwqpu.com

TS:   process.platform;  process.version
来源：http://jsb.zhengqikj.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kpx.yfazqb.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://irh.chenjidiqi.icu

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vjb.316326.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://dkt.jlsjyb.cn

================================================================================
来源：http://ped.tanke756.top

N. 数据结构与算法
来源：http://lzh.hfpthk.cn

================================================================================
来源：http://rzn.bbcook.cn

[N01] 二分查找（有序数组）
来源：http://qoh.ydjk.org.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gwy.jiagoushi.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eta.yj202588.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://axy.xylfe.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hos.meibo888.top

Java: Arrays.binarySearch(arr, x)
来源：http://woi.hesvh.cn

Go:   sort.SearchInts(arr, x)
来源：http://xhz.ehwqpu.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://pqr.guannengcc.top

C#:   Array.BinarySearch(arr, x)
来源：http://qdl.gzhubu.top

[N02] 排序（工程实践用内置实现）
来源：http://ijv.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://hcu.sysykeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://clb.ydzc1.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xzk.gogol.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lub.cqqwz.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://asa.sysykeji.top

Go:   slices.Sort(arr)
来源：http://tdc.fktsv.cn

Ruby: arr.sort
来源：http://gxu.jqgufenzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://jcg.dashuyun.cn

[N03] 快速排序（分治示例）
来源：http://mzy.zdqjudy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fnm.jqgufenzy.top

PHP:  // 递归实现，或用 usort
来源：http://egf.jiagoushi.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://buu.yuxming.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sgi.yj20258888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bie.kuanghao11.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gte.mhx1999.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://usq.sweek.top

C#:   // 手写递归，或 Array.Sort
来源：http://gpk.sufxvd.cn

[N04] 斐波那契数列
来源：http://crn.sweek.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kzi.zhiwuduotai.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qiq.snrcjt.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qag.shangyingyoupin.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iha.ppjwa.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://szo.gaohongyu789.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lss.tian-w.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tdg.jiagoushi.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bmn.zhoulong.xyz

[N05] 最大公约数
来源：http://rij.zhiwuduotai.top

Py:   math.gcd(a, b)
来源：http://dpa.fanxiaobao.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oti.ehwqpu.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wwv.hesvh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jpm.shanyushiyangtech.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://csj.ctjpmb.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nrb.tarul.cn

Ruby: a.gcd(b)
来源：http://gjg.meibo888.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uur.zhengqikj.top

[N06] 判断回文字符串
来源：http://huc.zhongyouzk.top

Py:   s == s[::-1]
来源：http://iyx.vehdjk.com

PHP:  $s === strrev($s);
来源：http://cru.meibo888.top

JS:   s === [...s].reverse().join("")
来源：http://lsn.yj20258.top

TS:   s === [...s].reverse().join("")
来源：http://ahx.zycfv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ixl.gogol.net.cn

Go:   // 双指针从两端比较
来源：http://tkb.tianlin.xyz

Ruby: s == s.reverse
来源：http://tdb.jinqigfzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://dic.birdmap.top

[N07] 两数之和（返回下标）
来源：http://rcq.ctjpmb.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dbk.snrcjt.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gqc.hongshengwenyu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://nop.yvedp.cn

TS:   // 手写 Map<string, number>
来源：http://msf.jyoumei.cn

Java: // 手写 HashMap
来源：http://urp.zycfv.cn

Go:   // 手写 map[int]int
来源：http://jyo.cashguo.top

Ruby: // 手写 Hash
来源：http://uej.jyoumei.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wur.chenjidiqi.icu

[N08] 生成全排列
来源：http://ead.havefunace.top

Py:   itertools.permutations(arr)
来源：http://rzn.tianlin.xyz

PHP:  // 手写递归交换
来源：http://ekx.epnwcf.com

JS:   // 手写回溯递归
来源：http://ors.316326.xyz

TS:   // 手写回溯递归
来源：http://cxa.0kj1m.cn

Java: // 手写回溯递归
来源：http://cvv.jianghu66.top

Go:   // 手写回溯递归
来源：http://xlc.fktsv.cn

Ruby: arr.permutation.to_a
来源：http://sli.aibaodan.cn

C#:   // 手写回溯递归
来源：http://khm.iojbl.cn

[N09] 栈与队列
来源：http://ihy.cashguo.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://oye.cqqwz.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dmr.bjfxy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rne.vqdsnc.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gdf.zdbjq.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bkt.yvedp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qba.kuanghao11.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jwv.0kj1m.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mvg.uphjek.com

[N10] 链表节点定义
来源：http://aep.yuxming.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://abw.jqgufenzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://jnq.redwolf501.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uuk.ehwqpu.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://scg.hammf.cn

Java: class Node { int v; Node next; }
来源：http://gcc.fanxiaobao.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://aym.yvedp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://csm.feifeiyinyue.top

C#:   class Node { public int V; public Node? Next; }
来源：http://zah.yuanzhike.top

[N11] 二叉树中序遍历
来源：http://nci.zhaomingkeji.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hye.xuanzx.com

PHP:  // 手写递归函数
来源：http://qcj.hywenlv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mlx.xuetiantiany.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lks.yfazqb.com

Java: // 手写递归
来源：http://xsu.tanke756.top

Go:   // 手写递归
来源：http://hte.shanyushiyangkeji.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ptq.aizwys.cn

C#:   // 手写递归
来源：http://lzp.sxryk.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qzy.yongpay.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rgj.xylfe.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tst.wangshuangyany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pmq.xuanzx.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lol.bjfxy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jxk.zhoulong.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://esy.bjfxy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hfi.yj202588.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rac.zhoulong.xyz

================================================================================
来源：http://dbn.shanyushiyangkeji.top

O. 并发与异步
来源：http://clh.aizwys.cn

================================================================================
来源：http://zop.ppjwa.cn

[O01] 启动一个线程
来源：http://lmu.zhoulong.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vsl.gotoacloud.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vwf.yueranfly.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zzc.gaohongyu789.top

TS:   // 同 JS
来源：http://tju.fengsongda.top

Java: new Thread(() -> f()).start()
来源：http://mir.hcnkem.com

Go:   go f()
来源：http://qsg.xuetiantiany.cn

Ruby: Thread.new { f }
来源：http://tge.gzhubu.top

C#:   Task.Run(() => F());
来源：http://aud.sjlbkw.cn

[O02] 使用线程池
来源：http://sut.jyoumei.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://usx.fzhhl.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zce.cdnleiting.top

JS:   // worker_threads 线程池
来源：http://uzq.pycfn.com

TS:   // worker_threads 线程池
来源：http://tav.ivvv.top

Java: Executors.newFixedThreadPool(4)
来源：http://udb.fehbvm.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://scn.pengpengdd.cyou

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ohz.zhengqikj.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sak.zhengqikj.top

[O03] 加锁保护共享数据
来源：http://iwz.ydzc1.top

Py:   with lock: shared += 1
来源：http://qix.zhaomingkeji.xyz

PHP:  // 用 flock() 做文件锁
来源：http://smz.yanxiufei.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ycu.tianlin.xyz

TS:   // 同 JS
来源：http://csq.jinqigufen.top

Java: synchronized (this) { shared++; }
来源：http://dub.shuidangran.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gpb.jinghuilouyu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ujz.cashguo.top

C#:   lock (gate) { shared++; }
来源：http://ltl.sweek.top

[O04] 定义异步函数并等待
来源：http://and.sxryk.cn

Py:   async def f():⏎    await g()
来源：http://sxg.hongshengwenyu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ufu.hammf.cn

JS:   async function f() { await g(); }
来源：http://qgl.cheryme.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://djl.zhaomingkeji.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wyo.fengsongda.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://upy.redwolf501.top

Ruby: # 用 Fiber 或 async gem
来源：http://rpf.hammf.cn

C#:   async Task F() { await G(); }
来源：http://cbf.jyoumei.cn

[O05] 并发执行并等待全部完成
来源：http://ils.nanxinkj.top

Py:   asyncio.gather(*tasks)
来源：http://mnd.cqqwz.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tow.jinqigufen.top

JS:   await Promise.all(tasks)
来源：http://qsv.jinghuilouyu.cn

TS:   await Promise.all(tasks)
来源：http://bvo.jyoumei.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ist.yuxming.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://skc.zhoulong.xyz

Ruby: threads.map(&:join)
来源：http://bne.hcnkem.com

C#:   await Task.WhenAll(t1, t2)
来源：http://tht.zhaomingkeji.xyz

[O06] 使用进程池
来源：http://dia.pycfn.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ajl.birdmap.top

PHP:  // pcntl_fork 或多进程队列
来源：http://jcd.aibaodan.cn

JS:   // child_process / cluster 模块
来源：http://uiq.hnqzz.top

TS:   // child_process / cluster 模块
来源：http://cpa.yuxming.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yzm.xziqi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ygi.xylfe.cn

Ruby: // fork 块
来源：http://vad.aizwys.cn

C#:   Parallel.For
来源：http://rkr.smart0.xyz

================================================================================
来源：http://ypn.jlsjyb.cn

P. 常用工具函数
来源：http://gey.daxiang520.top

================================================================================
来源：http://foh.zhoulong.xyz

[P01] 生成 UUID
来源：http://uyd.zhiwuduotai.top

Py:   str(uuid.uuid4())
来源：http://huj.yonumen.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yid.tian-w.cn

JS:   crypto.randomUUID()
来源：http://hkj.tianlin.xyz

TS:   crypto.randomUUID()
来源：http://yka.daxiang520.top

Java: UUID.randomUUID().toString()
来源：http://hrw.gaohongyu789.top

Go:   // 用 github.com/google/uuid
来源：http://xix.cucudq.cn

Ruby: SecureRandom.uuid
来源：http://ehl.ybcxt.top

C#:   Guid.NewGuid().ToString()
来源：http://ybf.vehdjk.com

[P02] MD5 / SHA256 摘要
来源：http://tym.kuanghao11.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gfj.guowangkeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://lxl.fanxiaobao.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uvp.chenlongwang.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://aqm.yj202588.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tyg.xuetiantiany.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://flf.xingfuxueyuan.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ttd.sweek.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dbx.yongpay.top

[P03] 生成短随机字符串
来源：http://xfr.ivvv.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://odm.nanxinkj.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rig.fengsongda.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sxa.hnxiangtu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kbe.316326.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dun.tianlin.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://phl.dianchejie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zxg.xuetiantiany.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uwd.zhaomingkeji.xyz

[P04] 求长度
来源：http://ies.redwolf501.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gfk.xuetiantiany.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ygh.yuanzhike.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iri.havefunace.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ypq.epnwcf.com

Java: list.size();  map.size();  s.length()
来源：http://scn.xuanzx.com

Go:   len(arr);  len(m)
来源：http://pqr.sxryk.cn

Ruby: x.length;  x.size
来源：http://zdu.wangshuangyany.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://epc.smart0.xyz

[P05] 判断两个对象内容是否相等
来源：http://aim.0kj1m.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fzp.nwbrower.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wja.vehdjk.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://exu.9152youxi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uhv.ydzc1.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ldb.zdbjq.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yxe.shuidangran.top

Ruby: a == b
来源：http://xwa.kuanghao11.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yiu.guowangkeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://teo.jinghuilouyu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://iul.pengpengdd.cyou

PHP:  if (empty($x)) {}
来源：http://xly.316326.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mky.tarul.cn

TS:   if (x == null) {}
来源：http://tre.uphjek.com

Java: if (x == null || x.isEmpty()) {}
来源：http://itb.daria6918.cn

Go:   if x == nil {}
来源：http://ldz.hywenlv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dhu.zhixingplan.top

C#:   if (x is null) {}
来源：http://auk.ydzc1.top

[P07] 防抖与节流
来源：http://xhp.shanyushiyangtech.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uov.vqdsnc.cn

PHP:  // 手写时间戳比较
来源：http://fij.iojbl.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uoj.hongshengwenyu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eqc.hnxiangtu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yyv.hcnkem.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://its.fengsongda.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://czt.fzhhl.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://azg.jinyuanbaomall.cn

[P08] 处理浮点精度问题
来源：http://onk.jinyuanbaomall.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jto.fzhhl.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cih.shangyingyoupin.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tjy.316326.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rgy.tanke756.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mbw.zhijiandao.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vxi.dashuyun.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mfm.yfazqb.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vys.quarkkingdee.top

================================================================================
来源：http://mbc.zhixingplan.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uto.jyoumei.cn

================================================================================
来源：http://sxe.hongshengwenyu.top

[Q01] 创建表
来源：http://crf.yanxiufei.cn

CREATE TABLE users (
来源：http://hnr.ydzc1.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://niv.epnwcf.com

name VARCHAR(50) NOT NULL,
来源：http://tkz.xziqi.cn

email VARCHAR(100) UNIQUE,
来源：http://fcc.sxryk.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rmm.gotoacloud.top

);
来源：http://lqk.zhaomingkeji.xyz

[Q02] 创建带外键的表
来源：http://lxb.zdbjq.cn

CREATE TABLE orders (
来源：http://hup.hnqzz.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sbr.sysykeji.top

user_id INT NOT NULL,
来源：http://uif.jianghu66.top

amount DECIMAL(10, 2),
来源：http://jxc.ywan-chungtsiang.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ydo.snrcjt.cn

);
来源：http://fjm.ehwqpu.com

[Q03] 增加列
来源：http://qig.svipenyu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xwk.daria6918.cn

[Q04] 修改列类型
来源：http://opl.jianghu66.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://roj.shanyushiyangkeji.top

[Q05] 重命名列
来源：http://xmq.bbcook.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://owj.shanyushiyangtech.top

[Q06] 删除列
来源：http://fou.pengpengdd.cyou

ALTER TABLE users DROP COLUMN age;
来源：http://zuo.uphjek.com

[Q07] 删除表
来源：http://lhq.tanke756.top

DROP TABLE IF EXISTS orders;
来源：http://ccq.chenjidiqi.icu

[Q08] 创建普通索引
来源：http://nyb.zhongyouzk.top

CREATE INDEX idx_users_email ON users(email);
来源：http://rdz.vehdjk.com

[Q09] 创建唯一索引
来源：http://ftx.shanyushiyangkeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gbv.ivvv.top

[Q10] 插入单行
来源：http://fup.redwolf501.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gui.svipenyu.cn

[Q11] 一次插入多行
来源：http://cmx.cashguo.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tql.ehwqpu.com

[Q12] 插入后取自增 ID
来源：http://qsh.hcnkem.com

INSERT INTO users (name) VALUES ('C');
来源：http://dks.andypj.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tat.c1oappe.top

[Q13] 忽略重复插入
来源：http://cui.jinghuilouyu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rtc.zhongyouzk.top

[Q14] 存在则更新（upsert）
来源：http://yuf.52xcode.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ped.jyoumei.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dga.ydjk.org.cn

[Q15] 查询全部
来源：http://jtm.uphjek.com


<!-- 参考信息 -->