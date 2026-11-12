代发 wailian999

Java: public static void main(String[] args)
来源：http://itu.xuanzx.com

Go:   func main()
来源：http://oar.birdmap.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rxf.52xcode.cn

C#:   static void Main(string[] args)
来源：http://gud.ydjk.org.cn

[M08] 获取系统与运行时信息
来源：http://ovw.quarkkingdee.top

Py:   platform.system();  platform.python_version()
来源：http://ygj.daria6918.cn

PHP:  PHP_OS;  phpversion();
来源：http://suc.pengpengdd.cyou

JS:   process.platform;  process.version
来源：http://vde.xingfuxueyuan.xyz

TS:   process.platform;  process.version
来源：http://tnc.zhengqikj.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://atz.dashuyun.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zzg.cqqwz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://iwo.cqqwz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yca.fzhhl.top

================================================================================
来源：http://abv.bbcook.cn

N. 数据结构与算法
来源：http://bwx.aizwys.cn

================================================================================
来源：http://vqe.gaohongyu789.top

[N01] 二分查找（有序数组）
来源：http://rzq.havefunace.top

Py:   bisect.bisect_left(arr, x)
来源：http://dly.ydjk.org.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ovs.cashguo.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yam.xuetiantiany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xrc.mhx1999.top

Java: Arrays.binarySearch(arr, x)
来源：http://wzb.yueranfly.top

Go:   sort.SearchInts(arr, x)
来源：http://dsn.ydjk.org.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://owb.jqgufenzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://nyd.vehdjk.com

[N02] 排序（工程实践用内置实现）
来源：http://zub.cucudq.cn

Py:   sorted(arr);  arr.sort()
来源：http://nph.zhaomingkeji.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://brz.pengpengdd.cyou

JS:   [...arr].sort((a, b) => a - b)
来源：http://cng.shanyushiyangkeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://jok.sufxvd.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ijg.fanxiaobao.xyz

Go:   slices.Sort(arr)
来源：http://flo.yanxiufei.cn

Ruby: arr.sort
来源：http://oke.daxiang520.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://mgf.havefunace.top

[N03] 快速排序（分治示例）
来源：http://ead.yuxming.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://iie.zhengqikj.top

PHP:  // 递归实现，或用 usort
来源：http://mek.vehdjk.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pey.gotoacloud.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jxi.ydjk.org.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yqe.wangdashe.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nqu.jinqigufen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://smh.daxiang520.top

C#:   // 手写递归，或 Array.Sort
来源：http://ehl.vehdjk.com

[N04] 斐波那契数列
来源：http://khk.shanyushiyangkeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vyv.tanke756.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://imi.havefunace.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tca.tianlin.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wya.tianlin.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gji.zhixingplan.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lhi.aibaodan.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://slz.316326.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://alu.jqgfzy.top

[N05] 最大公约数
来源：http://pbp.jinqigufen.top

Py:   math.gcd(a, b)
来源：http://kcu.jyoumei.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tmd.dashuyun.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yve.xylfe.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ujz.zdqjudy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ugh.zhixingplan.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ypj.xingfuxueyuan.xyz

Ruby: a.gcd(b)
来源：http://iho.yanxiufei.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vzu.yuanzhike.top

[N06] 判断回文字符串
来源：http://bly.jqgufenzy.top

Py:   s == s[::-1]
来源：http://ypd.yj20258.top

PHP:  $s === strrev($s);
来源：http://wyi.meibo888.top

JS:   s === [...s].reverse().join("")
来源：http://whu.tian-w.cn

TS:   s === [...s].reverse().join("")
来源：http://dcg.feifeiyinyue.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://las.ivvv.top

Go:   // 双指针从两端比较
来源：http://txu.jyoumei.cn

Ruby: s == s.reverse
来源：http://shm.yongpay.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://kyt.zdqjudy.top

[N07] 两数之和（返回下标）
来源：http://gbv.nanxinkj.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qhy.vqdsnc.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nka.birdmap.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wns.xylfe.cn

TS:   // 手写 Map<string, number>
来源：http://lbh.tanke756.top

Java: // 手写 HashMap
来源：http://vnm.zdqjudy.top

Go:   // 手写 map[int]int
来源：http://ecf.yuxming.cn

Ruby: // 手写 Hash
来源：http://evj.xingfuxueyuan.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://rsx.zdqjudy.top

[N08] 生成全排列
来源：http://bvr.316326.xyz

Py:   itertools.permutations(arr)
来源：http://hzv.hysaishi.cn

PHP:  // 手写递归交换
来源：http://lak.ehwqpu.com

JS:   // 手写回溯递归
来源：http://zre.aizwys.cn

TS:   // 手写回溯递归
来源：http://cho.yvedp.cn

Java: // 手写回溯递归
来源：http://wsd.fktsv.cn

Go:   // 手写回溯递归
来源：http://mkp.yj202588.top

Ruby: arr.permutation.to_a
来源：http://pnt.xuetiantiany.cn

C#:   // 手写回溯递归
来源：http://szx.epnwcf.com

[N09] 栈与队列
来源：http://ycj.yanxiufei.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jeq.yvedp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ivf.nanxuanxn.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pcs.yj20258.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://avq.xuanzx.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://crf.sysykeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ppm.bjfxy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://akz.fanxiaobao.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rfr.sweek.top

[N10] 链表节点定义
来源：http://iao.vehdjk.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qna.kuanghao11.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ggf.pycfn.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xrn.snrcjt.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qvs.andypj.xyz

Java: class Node { int v; Node next; }
来源：http://lck.wangdashe.top

Go:   type Node struct { V int; Next *Node }
来源：http://bxa.ydzc1.top

Ruby: Node = Struct.new(:v, :next)
来源：http://wyj.gaohongyu789.top

C#:   class Node { public int V; public Node? Next; }
来源：http://wkf.bjfxy.top

[N11] 二叉树中序遍历
来源：http://mxi.shuidangran.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lrg.tian-w.cn

PHP:  // 手写递归函数
来源：http://ubq.ybcxt.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://udu.c1oappe.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://osa.pycfn.com

Java: // 手写递归
来源：http://hzh.ppjwa.cn

Go:   // 手写递归
来源：http://mil.chenzaomai.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://aax.dashuyun.cn

C#:   // 手写递归
来源：http://npg.hesvh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dma.guowangkeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vpe.haohaochexian.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ope.shanyushiyangkeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rzn.yanxiufei.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jmj.dashuyun.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://aji.c1oappe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fvb.havefunace.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://alp.shuidangran.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rje.xuanzx.com

================================================================================
来源：http://tig.chenzaomai.com

O. 并发与异步
来源：http://fmp.smart0.xyz

================================================================================
来源：http://bxb.nanxinkj.top

[O01] 启动一个线程
来源：http://dno.fzhhl.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qgr.gaohongyu789.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pss.hnqzz.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wem.hesvh.cn

TS:   // 同 JS
来源：http://kcg.zhaomingkeji.xyz

Java: new Thread(() -> f()).start()
来源：http://nal.tianlin.xyz

Go:   go f()
来源：http://frh.yonumen.top

Ruby: Thread.new { f }
来源：http://bbc.sxryk.cn

C#:   Task.Run(() => F());
来源：http://thu.haohaochexian.top

[O02] 使用线程池
来源：http://jql.yvedp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lld.xinyue.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sfk.tanke756.top

JS:   // worker_threads 线程池
来源：http://mdh.jianghu66.top

TS:   // worker_threads 线程池
来源：http://oyp.sufxvd.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jwm.sysykeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://iwi.ybcxt.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vgs.zhijiandao.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lbz.zhijiandao.cn

[O03] 加锁保护共享数据
来源：http://sfq.xuanzx.com

Py:   with lock: shared += 1
来源：http://rhg.pycfn.com

PHP:  // 用 flock() 做文件锁
来源：http://qsz.chenzaomai.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fzq.smart0.xyz

TS:   // 同 JS
来源：http://nbo.meibo888.top

Java: synchronized (this) { shared++; }
来源：http://lnh.tanke756.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cze.shzxlz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lsb.yvedp.cn

C#:   lock (gate) { shared++; }
来源：http://xne.hammf.cn

[O04] 定义异步函数并等待
来源：http://uxj.andypj.xyz

Py:   async def f():⏎    await g()
来源：http://mcb.cqqwz.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://aap.quarkkingdee.top

JS:   async function f() { await g(); }
来源：http://ovt.tarul.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kzc.tarul.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wyk.ywan-chungtsiang.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bps.ydjk.org.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lco.pycfn.com

C#:   async Task F() { await G(); }
来源：http://zwc.sufxvd.cn

[O05] 并发执行并等待全部完成
来源：http://rnq.zdbjq.cn

Py:   asyncio.gather(*tasks)
来源：http://vsk.daria6918.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nnv.yangfankeji.com

JS:   await Promise.all(tasks)
来源：http://cyz.xuanzx.com

TS:   await Promise.all(tasks)
来源：http://lhb.jinghuilouyu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pjf.hongshengwenyu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://stp.jinqigufen.top

Ruby: threads.map(&:join)
来源：http://arw.9152youxi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://okz.sysykeji.top

[O06] 使用进程池
来源：http://dft.birdmap.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ywi.shuidangran.top

PHP:  // pcntl_fork 或多进程队列
来源：http://bnj.guannengcc.top

JS:   // child_process / cluster 模块
来源：http://veb.c1oappe.top

TS:   // child_process / cluster 模块
来源：http://amr.zdqjudy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ntm.haohaochexian.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fbk.xylfe.cn

Ruby: // fork 块
来源：http://vri.zhijiandao.cn

C#:   Parallel.For
来源：http://czh.yj202588.top

================================================================================
来源：http://azz.xuetiantiany.cn

P. 常用工具函数
来源：http://hip.yueranfly.top

================================================================================
来源：http://ajg.jianghu66.top

[P01] 生成 UUID
来源：http://avo.hfpthk.cn

Py:   str(uuid.uuid4())
来源：http://mqm.bjfxy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dwl.epnwcf.com

JS:   crypto.randomUUID()
来源：http://igd.tarul.cn

TS:   crypto.randomUUID()
来源：http://pvc.cashguo.top

Java: UUID.randomUUID().toString()
来源：http://gbq.jinyuanbaomall.cn

Go:   // 用 github.com/google/uuid
来源：http://iol.bbcook.cn

Ruby: SecureRandom.uuid
来源：http://tew.xziqi.cn

C#:   Guid.NewGuid().ToString()
来源：http://aix.chenjidiqi.icu

[P02] MD5 / SHA256 摘要
来源：http://ory.vehdjk.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://app.uphjek.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://xwa.xingfuxueyuan.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ebh.jinqigufen.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lzz.shuidangran.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hii.xziqi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://goz.jqgfzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zfc.chenzaomai.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xjm.aibaodan.cn

[P03] 生成短随机字符串
来源：http://jpk.c1oappe.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wrr.cucudq.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xbz.nwbrower.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cts.hnqzz.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xii.zhixingplan.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ada.jinghuilouyu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qrm.shanyushiyangkeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ocy.yvedp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cdp.zhaomingkeji.xyz

[P04] 求长度
来源：http://lmo.xinyue.icu

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gbp.xinyue.icu

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uwo.quarkkingdee.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bkb.zdbjq.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yvz.chenzaomai.com

Java: list.size();  map.size();  s.length()
来源：http://rlj.zhiwuduotai.top

Go:   len(arr);  len(m)
来源：http://ldm.iojbl.cn

Ruby: x.length;  x.size
来源：http://eww.xinyue.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://qdd.yanxiufei.cn

[P05] 判断两个对象内容是否相等
来源：http://gzo.sweek.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ine.hnxiangtu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://evj.ydjk.org.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://eee.mhx1999.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jyw.xylfe.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://joy.ydjk.org.cn

Go:   reflect.DeepEqual(a, b)
来源：http://dyl.shangyingyoupin.top

Ruby: a == b
来源：http://kvr.jyoumei.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uac.jinghuilouyu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://auc.wangdashe.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uit.bjfxy.top

PHP:  if (empty($x)) {}
来源：http://qly.sxryk.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tdm.feifeiyinyue.top

TS:   if (x == null) {}
来源：http://guz.sufxvd.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://iah.cdnleiting.top

Go:   if x == nil {}
来源：http://bqh.gzhubu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gmq.nwbrower.top

C#:   if (x is null) {}
来源：http://mdp.gaohongyu789.top

[P07] 防抖与节流
来源：http://xoh.dianchejie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kwn.ivvv.top

PHP:  // 手写时间戳比较
来源：http://eni.yj20258888.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rbo.pycfn.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tiz.hongshengwenyu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ivw.nanxuanxn.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uhx.xuetiantiany.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hzf.yuxming.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fjt.epnwcf.com

[P08] 处理浮点精度问题
来源：http://qhf.fengsongda.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://eun.fzhhl.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uhz.vqdsnc.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bxq.daria6918.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://erm.yangfankeji.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fhm.jiagoushi.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rks.tianlin.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vcp.vqdsnc.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gbw.fanxiaobao.xyz

================================================================================
来源：http://luj.xingfuxueyuan.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cfb.chenjidiqi.icu

================================================================================
来源：http://rmy.yvedp.cn

[Q01] 创建表
来源：http://jyj.hongshengwenyu.top

CREATE TABLE users (
来源：http://ivr.zhixingplan.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bpe.wangdashe.top

name VARCHAR(50) NOT NULL,
来源：http://sfc.yonumen.top

email VARCHAR(100) UNIQUE,
来源：http://gci.vqdsnc.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ebb.gzhubu.top

);
来源：http://ltn.yuxming.cn

[Q02] 创建带外键的表
来源：http://hpi.jqgufenzy.top

CREATE TABLE orders (
来源：http://uxb.daria6918.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rpi.nwbrower.top

user_id INT NOT NULL,
来源：http://sxy.birdmap.top

amount DECIMAL(10, 2),
来源：http://web.cucudq.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dcz.smart0.xyz

);
来源：http://wjq.hfpthk.cn

[Q03] 增加列
来源：http://waq.fzhhl.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://huu.hnqzz.top

[Q04] 修改列类型
来源：http://bmu.pycfn.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sbb.yonumen.top

[Q05] 重命名列
来源：http://cgt.hesvh.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uph.yonumen.top

[Q06] 删除列
来源：http://pmt.fengsongda.top

ALTER TABLE users DROP COLUMN age;
来源：http://tdj.dashuyun.cn

[Q07] 删除表
来源：http://xab.zhoulong.xyz

DROP TABLE IF EXISTS orders;
来源：http://njc.birdmap.top

[Q08] 创建普通索引
来源：http://udu.fengsongda.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jkb.sweek.top

[Q09] 创建唯一索引
来源：http://ntw.yonumen.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://epd.svipenyu.cn

[Q10] 插入单行
来源：http://kkh.shanyushiyangtech.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://aqq.hesvh.cn

[Q11] 一次插入多行
来源：http://pgc.yonumen.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ayl.quarkkingdee.top

[Q12] 插入后取自增 ID
来源：http://aex.epnwcf.com

INSERT INTO users (name) VALUES ('C');
来源：http://xqx.xuetiantiany.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fsp.guowangkeji.top

[Q13] 忽略重复插入
来源：http://prf.wangshuangyany.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tch.zhijiandao.cn

[Q14] 存在则更新（upsert）
来源：http://npx.shangyingyoupin.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://igh.zhijiandao.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jql.cheryme.top

[Q15] 查询全部
来源：http://vuf.cashguo.top


<!-- 参考信息 -->