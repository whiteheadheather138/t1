代发 wailian999

Py:   if __name__ == "__main__":
来源：http://inv.zhixingplan.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://frh.andypj.xyz

JS:   require.main === module
来源：http://zny.nanxuanxn.top

TS:   require.main === module
来源：http://edr.tarul.cn

Java: public static void main(String[] args)
来源：http://ugg.zhoulong.xyz

Go:   func main()
来源：http://xaz.sufxvd.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pre.ppjwa.cn

C#:   static void Main(string[] args)
来源：http://cnp.sufxvd.cn

[M08] 获取系统与运行时信息
来源：http://vqw.ppjwa.cn

Py:   platform.system();  platform.python_version()
来源：http://goc.bbcook.cn

PHP:  PHP_OS;  phpversion();
来源：http://qzh.daxiang520.top

JS:   process.platform;  process.version
来源：http://ynj.feifeiyinyue.top

TS:   process.platform;  process.version
来源：http://wkc.hfpthk.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uif.fehbvm.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://rfw.shanyushiyangtech.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://evz.xylfe.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wjk.jqgfzy.top

================================================================================
来源：http://qdl.gogol.net.cn

N. 数据结构与算法
来源：http://lsi.yongpay.top

================================================================================
来源：http://ylx.andypj.xyz

[N01] 二分查找（有序数组）
来源：http://jot.bbcook.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hzd.daria6918.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ndf.hysaishi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fxo.0kj1m.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qpf.zhijiandao.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vpl.yueranfly.top

Go:   sort.SearchInts(arr, x)
来源：http://zmi.jqgfzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://mxx.jqgfzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://apo.feifeiyinyue.top

[N02] 排序（工程实践用内置实现）
来源：http://kdh.bbcook.cn

Py:   sorted(arr);  arr.sort()
来源：http://teg.snrcjt.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pev.ybcxt.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xnp.dashuyun.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sln.sysykeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://khb.wangdashe.top

Go:   slices.Sort(arr)
来源：http://bbg.cdnleiting.top

Ruby: arr.sort
来源：http://yxu.nanxinkj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rhd.jinqigufen.top

[N03] 快速排序（分治示例）
来源：http://mss.chenjidiqi.icu

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lsp.iojbl.cn

PHP:  // 递归实现，或用 usort
来源：http://wyt.yonumen.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jyu.xylfe.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kqf.gogol.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ksk.9152youxi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pru.andypj.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xbl.sxryk.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gmk.yj20258888.top

[N04] 斐波那契数列
来源：http://xng.jinghuilouyu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bfe.hnxiangtu.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jsf.ywan-chungtsiang.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rsz.yueranfly.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rtf.cqqwz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bbf.daria6918.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qce.redwolf501.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://krs.zycfv.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vvk.tarul.cn

[N05] 最大公约数
来源：http://hfd.jqgfzy.top

Py:   math.gcd(a, b)
来源：http://ooh.yuxming.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xgv.cashguo.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cpm.0kj1m.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fcw.52xcode.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fju.c1oappe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ibt.aibaodan.cn

Ruby: a.gcd(b)
来源：http://dky.gotoacloud.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://scd.snrcjt.cn

[N06] 判断回文字符串
来源：http://wzi.fengsongda.top

Py:   s == s[::-1]
来源：http://nxn.zhaomingkeji.xyz

PHP:  $s === strrev($s);
来源：http://lfk.daxiang520.top

JS:   s === [...s].reverse().join("")
来源：http://cwv.guannengcc.top

TS:   s === [...s].reverse().join("")
来源：http://zvt.ppjwa.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://axw.shanyushiyangtech.top

Go:   // 双指针从两端比较
来源：http://enb.zhengqikj.top

Ruby: s == s.reverse
来源：http://cjx.cdnleiting.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://iup.hfpthk.cn

[N07] 两数之和（返回下标）
来源：http://qen.hcnkem.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://inq.hcnkem.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tcp.shanyushiyangkeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ndr.havefunace.top

TS:   // 手写 Map<string, number>
来源：http://pkp.feifeiyinyue.top

Java: // 手写 HashMap
来源：http://rhc.shangyingyoupin.top

Go:   // 手写 map[int]int
来源：http://nlj.guowangkeji.top

Ruby: // 手写 Hash
来源：http://iye.ivvv.top

C#:   // 手写 Dictionary<int, int>
来源：http://aoe.smart0.xyz

[N08] 生成全排列
来源：http://avt.sxryk.cn

Py:   itertools.permutations(arr)
来源：http://zvj.gzhubu.top

PHP:  // 手写递归交换
来源：http://yvm.fanxiaobao.xyz

JS:   // 手写回溯递归
来源：http://ndh.ppjwa.cn

TS:   // 手写回溯递归
来源：http://lgn.chenlongwang.top

Java: // 手写回溯递归
来源：http://dnr.gzhubu.top

Go:   // 手写回溯递归
来源：http://ilv.fktsv.cn

Ruby: arr.permutation.to_a
来源：http://uqx.zdbjq.cn

C#:   // 手写回溯递归
来源：http://vyn.hcnkem.com

[N09] 栈与队列
来源：http://qmr.hnqzz.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bfd.chenzaomai.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://apt.shangyingyoupin.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yay.9152youxi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hyo.zhixingplan.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nvl.iojbl.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cil.ydzc1.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qyc.meibo888.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hne.tanke756.top

[N10] 链表节点定义
来源：http://mcq.xingfuxueyuan.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uhv.chenzaomai.com

PHP:  class Node { public $v; public $next = null; }
来源：http://mat.sufxvd.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gas.redwolf501.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wdb.andypj.xyz

Java: class Node { int v; Node next; }
来源：http://avz.zycfv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jhu.snrcjt.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pgq.jqgfzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://dik.gogol.net.cn

[N11] 二叉树中序遍历
来源：http://ehm.hysaishi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ejy.cqqwz.cn

PHP:  // 手写递归函数
来源：http://hsy.haohaochexian.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lzu.daxiang520.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ttb.52xcode.cn

Java: // 手写递归
来源：http://lrz.jiagoushi.top

Go:   // 手写递归
来源：http://zqj.ivvv.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zzw.tianlin.xyz

C#:   // 手写递归
来源：http://amw.yj20258888.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sky.ivvv.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://liz.smart0.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ocv.cashguo.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ciz.nanxinkj.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oog.ywan-chungtsiang.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lsd.jinghuilouyu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ixo.hysaishi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rnd.jlsjyb.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rsb.jiagoushi.top

================================================================================
来源：http://irt.shuidangran.top

O. 并发与异步
来源：http://vhd.guowangkeji.top

================================================================================
来源：http://sng.bjfxy.top

[O01] 启动一个线程
来源：http://hby.zdbjq.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cjn.wangdashe.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pag.yfazqb.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yty.tarul.cn

TS:   // 同 JS
来源：http://qqq.yj20258888.top

Java: new Thread(() -> f()).start()
来源：http://uqe.9152youxi.cn

Go:   go f()
来源：http://zol.yj20258.top

Ruby: Thread.new { f }
来源：http://zbv.hysaishi.cn

C#:   Task.Run(() => F());
来源：http://rxq.yanxiufei.cn

[O02] 使用线程池
来源：http://mbm.andypj.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qge.sysykeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lns.zhiwuduotai.top

JS:   // worker_threads 线程池
来源：http://bcx.hfpthk.cn

TS:   // worker_threads 线程池
来源：http://awz.hnxiangtu.top

Java: Executors.newFixedThreadPool(4)
来源：http://dvx.hesvh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nmy.jinghuilouyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vqa.cucudq.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://eye.cucudq.cn

[O03] 加锁保护共享数据
来源：http://avf.hcnkem.com

Py:   with lock: shared += 1
来源：http://etu.jiagoushi.top

PHP:  // 用 flock() 做文件锁
来源：http://dgj.snrcjt.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vxs.gotoacloud.top

TS:   // 同 JS
来源：http://eyk.ybcxt.top

Java: synchronized (this) { shared++; }
来源：http://zbu.svipenyu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://peo.yj20258.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://rkx.sxryk.cn

C#:   lock (gate) { shared++; }
来源：http://yly.yvedp.cn

[O04] 定义异步函数并等待
来源：http://due.uphjek.com

Py:   async def f():⏎    await g()
来源：http://mth.snrcjt.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://afo.yvedp.cn

JS:   async function f() { await g(); }
来源：http://smr.316326.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://qsq.mhx1999.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dtu.9152youxi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://onu.yj20258.top

Ruby: # 用 Fiber 或 async gem
来源：http://opk.pycfn.com

C#:   async Task F() { await G(); }
来源：http://rnz.bjfxy.top

[O05] 并发执行并等待全部完成
来源：http://vva.shzxlz.cn

Py:   asyncio.gather(*tasks)
来源：http://jbv.nanxuanxn.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uzz.bbcook.cn

JS:   await Promise.all(tasks)
来源：http://vdq.ctjpmb.com

TS:   await Promise.all(tasks)
来源：http://ciw.hnqzz.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bko.fehbvm.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dxs.zhijiandao.cn

Ruby: threads.map(&:join)
来源：http://rtc.cucudq.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://nkm.fengsongda.top

[O06] 使用进程池
来源：http://yqd.fanxiaobao.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sen.uphjek.com

PHP:  // pcntl_fork 或多进程队列
来源：http://iuw.hongshengwenyu.top

JS:   // child_process / cluster 模块
来源：http://vgs.cheryme.top

TS:   // child_process / cluster 模块
来源：http://poi.jlsjyb.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://evt.zhiwuduotai.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://urg.shanyushiyangkeji.top

Ruby: // fork 块
来源：http://slz.jianghu66.top

C#:   Parallel.For
来源：http://feb.ivvv.top

================================================================================
来源：http://zza.fehbvm.com

P. 常用工具函数
来源：http://her.hywenlv.cn

================================================================================
来源：http://coq.mhx1999.top

[P01] 生成 UUID
来源：http://hig.cheryme.top

Py:   str(uuid.uuid4())
来源：http://ejc.chenzaomai.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ysk.yangfankeji.com

JS:   crypto.randomUUID()
来源：http://ufx.meibo888.top

TS:   crypto.randomUUID()
来源：http://rll.daxiang520.top

Java: UUID.randomUUID().toString()
来源：http://pma.dianchejie.cn

Go:   // 用 github.com/google/uuid
来源：http://mio.xuetiantiany.cn

Ruby: SecureRandom.uuid
来源：http://ksz.xylfe.cn

C#:   Guid.NewGuid().ToString()
来源：http://fxy.snrcjt.cn

[P02] MD5 / SHA256 摘要
来源：http://jpm.bbcook.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://prm.nwbrower.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qcm.bbcook.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mtl.ehwqpu.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://iol.aibaodan.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nfy.dashuyun.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gcg.svipenyu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://umn.sufxvd.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ypr.iojbl.cn

[P03] 生成短随机字符串
来源：http://kpv.zhijiandao.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kef.ivvv.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kao.nwbrower.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qip.ppjwa.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://edb.havefunace.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://aft.zhaomingkeji.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ynn.zdqjudy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ysp.snrcjt.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fni.tian-w.cn

[P04] 求长度
来源：http://srv.dianchejie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://okm.jinghuilouyu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://odc.ydzc1.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ukw.hysaishi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xvr.mhx1999.top

Java: list.size();  map.size();  s.length()
来源：http://kvd.wangshuangyany.cn

Go:   len(arr);  len(m)
来源：http://jpy.uphjek.com

Ruby: x.length;  x.size
来源：http://sci.yvedp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ehu.9152youxi.cn

[P05] 判断两个对象内容是否相等
来源：http://tjv.yuanzhike.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://xxr.nanxuanxn.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sdc.tian-w.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zqx.hcnkem.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yfu.sweek.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sez.sjlbkw.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ijd.bbcook.cn

Ruby: a == b
来源：http://lok.andypj.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jlz.hesvh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ziw.yvedp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://woj.feifeiyinyue.top

PHP:  if (empty($x)) {}
来源：http://mtx.zdbjq.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zml.cdnleiting.top

TS:   if (x == null) {}
来源：http://mxh.guannengcc.top

Java: if (x == null || x.isEmpty()) {}
来源：http://kga.redwolf501.top

Go:   if x == nil {}
来源：http://hen.ppjwa.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rbl.hnxiangtu.top

C#:   if (x is null) {}
来源：http://kxb.ydjk.org.cn

[P07] 防抖与节流
来源：http://aia.zhijiandao.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qvo.quarkkingdee.top

PHP:  // 手写时间戳比较
来源：http://dub.yuanzhike.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mkw.vehdjk.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dma.dianchejie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hzy.yanxiufei.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tfy.9152youxi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://bey.hysaishi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tli.fengsongda.top

[P08] 处理浮点精度问题
来源：http://apz.wangshuangyany.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xcd.yj20258888.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qya.jinghuilouyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://guo.cucudq.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zgx.jyoumei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://syd.jinqigufen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nwj.ivvv.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cwm.yuxming.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qcn.tarul.cn

================================================================================
来源：http://ehu.hysaishi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xrd.xuanzx.com

================================================================================
来源：http://gym.bbcook.cn

[Q01] 创建表
来源：http://frc.hesvh.cn

CREATE TABLE users (
来源：http://cfd.xinyue.icu

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gig.hysaishi.cn

name VARCHAR(50) NOT NULL,
来源：http://zyj.feifeiyinyue.top

email VARCHAR(100) UNIQUE,
来源：http://yon.dashuyun.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gke.cheryme.top

);
来源：http://kwh.hfpthk.cn

[Q02] 创建带外键的表
来源：http://bbn.yueranfly.top

CREATE TABLE orders (
来源：http://gxn.zdqjudy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rvd.quarkkingdee.top

user_id INT NOT NULL,
来源：http://lfd.shangyingyoupin.top

amount DECIMAL(10, 2),
来源：http://hrb.sysykeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mml.yonumen.top

);
来源：http://mnb.ydzc1.top

[Q03] 增加列
来源：http://feg.chenjidiqi.icu

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uwr.tanke756.top

[Q04] 修改列类型
来源：http://tst.snrcjt.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://enz.sjlbkw.cn

[Q05] 重命名列
来源：http://aus.fktsv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cgn.tianlin.xyz

[Q06] 删除列
来源：http://gnc.xylfe.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ded.hnqzz.top

[Q07] 删除表
来源：http://sev.wangshuangyany.cn

DROP TABLE IF EXISTS orders;
来源：http://oax.vehdjk.com

[Q08] 创建普通索引
来源：http://utt.guowangkeji.top

CREATE INDEX idx_users_email ON users(email);
来源：http://nfl.ehwqpu.com

[Q09] 创建唯一索引
来源：http://eyp.316326.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rvm.pycfn.com

[Q10] 插入单行
来源：http://smn.shuidangran.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zfl.quarkkingdee.top

[Q11] 一次插入多行
来源：http://nwf.tarul.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hrs.wangshuangyany.cn

[Q12] 插入后取自增 ID
来源：http://ypc.guowangkeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://cza.epnwcf.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://irb.xuanzx.com

[Q13] 忽略重复插入
来源：http://jmz.shangyingyoupin.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ruk.sjlbkw.cn


<!-- 参考信息 -->