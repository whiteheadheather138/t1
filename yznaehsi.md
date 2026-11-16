代发 wailian999

Py:   if __name__ == "__main__":
来源：http://ckc.yfazqb.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vgw.birdmap.top

JS:   require.main === module
来源：http://ysw.tarul.cn

TS:   require.main === module
来源：http://aid.xinyue.icu

Java: public static void main(String[] args)
来源：http://pbk.wangshuangyany.cn

Go:   func main()
来源：http://fku.havefunace.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://svq.quarkkingdee.top

C#:   static void Main(string[] args)
来源：http://wsr.pycfn.com

[M08] 获取系统与运行时信息
来源：http://yoc.quarkkingdee.top

Py:   platform.system();  platform.python_version()
来源：http://nuc.haohaochexian.top

PHP:  PHP_OS;  phpversion();
来源：http://czr.hesvh.cn

JS:   process.platform;  process.version
来源：http://lsi.xylfe.cn

TS:   process.platform;  process.version
来源：http://kan.cheryme.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dwj.hongshengwenyu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mmz.yvedp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qtw.ydjk.org.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rwq.zycfv.cn

================================================================================
来源：http://kdu.sufxvd.cn

N. 数据结构与算法
来源：http://zcp.wangdashe.top

================================================================================
来源：http://pjl.hammf.cn

[N01] 二分查找（有序数组）
来源：http://xtl.mhx1999.top

Py:   bisect.bisect_left(arr, x)
来源：http://exp.yanxiufei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uaa.zhengqikj.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zue.guannengcc.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ryw.wangshuangyany.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fqk.pycfn.com

Go:   sort.SearchInts(arr, x)
来源：http://etx.yuxming.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mgl.daria6918.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rwv.52xcode.cn

[N02] 排序（工程实践用内置实现）
来源：http://aaj.ivvv.top

Py:   sorted(arr);  arr.sort()
来源：http://lzy.xziqi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mqy.quarkkingdee.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://azq.yj20258.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ate.yueranfly.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ros.chenlongwang.top

Go:   slices.Sort(arr)
来源：http://xdr.meibo888.top

Ruby: arr.sort
来源：http://fih.jiagoushi.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xsf.ydzc1.top

[N03] 快速排序（分治示例）
来源：http://rhj.iojbl.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mxd.wangdashe.top

PHP:  // 递归实现，或用 usort
来源：http://zbd.guannengcc.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hyp.chenjidiqi.icu

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qzi.hnxiangtu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://suw.sweek.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ywz.hcnkem.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hcs.kuanghao11.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bmj.ybcxt.top

[N04] 斐波那契数列
来源：http://fch.yj202588.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zcv.mhx1999.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pib.yueranfly.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xaa.316326.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bwq.cheryme.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gdw.gzhubu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dtr.cqqwz.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dgh.ctjpmb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ari.zhengqikj.top

[N05] 最大公约数
来源：http://iqp.ppjwa.cn

Py:   math.gcd(a, b)
来源：http://nyv.shanyushiyangtech.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hmk.jinghuilouyu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ebb.shuidangran.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jrr.cheryme.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uhg.pycfn.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ohp.zhoulong.xyz

Ruby: a.gcd(b)
来源：http://naf.xuanzx.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wtx.fengsongda.top

[N06] 判断回文字符串
来源：http://aoj.gzhubu.top

Py:   s == s[::-1]
来源：http://nie.hfpthk.cn

PHP:  $s === strrev($s);
来源：http://des.sxryk.cn

JS:   s === [...s].reverse().join("")
来源：http://mqe.shangyingyoupin.top

TS:   s === [...s].reverse().join("")
来源：http://pij.shanyushiyangtech.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ayo.uphjek.com

Go:   // 双指针从两端比较
来源：http://ekh.jiagoushi.top

Ruby: s == s.reverse
来源：http://cdk.gzhubu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jzh.xziqi.cn

[N07] 两数之和（返回下标）
来源：http://uhy.yj20258.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kyi.zdqjudy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://seo.yangfankeji.com

JS:   // 手写 Map：map.set(v, i)
来源：http://tqt.xuanzx.com

TS:   // 手写 Map<string, number>
来源：http://jeo.yuanzhike.top

Java: // 手写 HashMap
来源：http://sbe.tanke756.top

Go:   // 手写 map[int]int
来源：http://sde.gaohongyu789.top

Ruby: // 手写 Hash
来源：http://ggy.zhengqikj.top

C#:   // 手写 Dictionary<int, int>
来源：http://hne.jyoumei.cn

[N08] 生成全排列
来源：http://zzn.jinqigfzy.top

Py:   itertools.permutations(arr)
来源：http://nny.zhaomingkeji.xyz

PHP:  // 手写递归交换
来源：http://xxi.316326.xyz

JS:   // 手写回溯递归
来源：http://nbo.yfazqb.com

TS:   // 手写回溯递归
来源：http://tkl.hnqzz.top

Java: // 手写回溯递归
来源：http://ujh.quarkkingdee.top

Go:   // 手写回溯递归
来源：http://box.hesvh.cn

Ruby: arr.permutation.to_a
来源：http://qmv.shzxlz.cn

C#:   // 手写回溯递归
来源：http://auf.jinqigfzy.top

[N09] 栈与队列
来源：http://iww.fktsv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://iem.fehbvm.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dbw.zhaomingkeji.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vxm.guowangkeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vtr.tanke756.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://aup.yj202588.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qzh.tanke756.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xdf.shuidangran.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fcf.hongshengwenyu.top

[N10] 链表节点定义
来源：http://rpc.daxiang520.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mhi.shangyingyoupin.top

PHP:  class Node { public $v; public $next = null; }
来源：http://gnr.bbcook.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rmq.gotoacloud.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mgp.svipenyu.cn

Java: class Node { int v; Node next; }
来源：http://ftq.zhijiandao.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nhz.snrcjt.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fnd.nanxuanxn.top

C#:   class Node { public int V; public Node? Next; }
来源：http://nhn.shanyushiyangkeji.top

[N11] 二叉树中序遍历
来源：http://azu.cashguo.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gfm.gogol.net.cn

PHP:  // 手写递归函数
来源：http://wqq.jinyuanbaomall.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bia.yangfankeji.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kzn.hysaishi.cn

Java: // 手写递归
来源：http://qys.fehbvm.com

Go:   // 手写递归
来源：http://uzs.bbcook.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sam.316326.xyz

C#:   // 手写递归
来源：http://vjh.feifeiyinyue.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bxx.9152youxi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hpm.shzxlz.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vkc.hammf.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bse.tarul.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pfv.xylfe.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wis.yuxming.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nre.xinyue.icu

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sbm.316326.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rxp.c1oappe.top

================================================================================
来源：http://kry.shangyingyoupin.top

O. 并发与异步
来源：http://ybu.kuanghao11.cn

================================================================================
来源：http://nhr.yfazqb.com

[O01] 启动一个线程
来源：http://mmi.shanyushiyangkeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ynp.snrcjt.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ake.hongshengwenyu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pcd.smart0.xyz

TS:   // 同 JS
来源：http://lvo.hcnkem.com

Java: new Thread(() -> f()).start()
来源：http://sqd.vehdjk.com

Go:   go f()
来源：http://loh.zhixingplan.top

Ruby: Thread.new { f }
来源：http://gfk.xziqi.cn

C#:   Task.Run(() => F());
来源：http://cch.bbcook.cn

[O02] 使用线程池
来源：http://gzn.shangyingyoupin.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vkz.zycfv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nyz.havefunace.top

JS:   // worker_threads 线程池
来源：http://zqp.mhx1999.top

TS:   // worker_threads 线程池
来源：http://ycd.shzxlz.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ylz.ivvv.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://met.daxiang520.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jnz.zhongyouzk.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ewm.meibo888.top

[O03] 加锁保护共享数据
来源：http://cgz.cheryme.top

Py:   with lock: shared += 1
来源：http://cqg.shanyushiyangtech.top

PHP:  // 用 flock() 做文件锁
来源：http://bbh.ydzc1.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uwt.xingfuxueyuan.xyz

TS:   // 同 JS
来源：http://lia.xinyue.icu

Java: synchronized (this) { shared++; }
来源：http://ytk.zdbjq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://izn.jiagoushi.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://acc.ctjpmb.com

C#:   lock (gate) { shared++; }
来源：http://bxg.zhoulong.xyz

[O04] 定义异步函数并等待
来源：http://pwq.yj20258888.top

Py:   async def f():⏎    await g()
来源：http://ndr.daxiang520.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nlm.fehbvm.com

JS:   async function f() { await g(); }
来源：http://ejw.andypj.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://fcy.wangdashe.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xuq.meibo888.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cdp.birdmap.top

Ruby: # 用 Fiber 或 async gem
来源：http://hnn.yj20258888.top

C#:   async Task F() { await G(); }
来源：http://oml.zhiwuduotai.top

[O05] 并发执行并等待全部完成
来源：http://swb.yfazqb.com

Py:   asyncio.gather(*tasks)
来源：http://hli.yj20258888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ldm.smart0.xyz

JS:   await Promise.all(tasks)
来源：http://apg.wangdashe.top

TS:   await Promise.all(tasks)
来源：http://sqh.chenjidiqi.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ejn.chenjidiqi.icu

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://haz.chenjidiqi.icu

Ruby: threads.map(&:join)
来源：http://vkx.ivvv.top

C#:   await Task.WhenAll(t1, t2)
来源：http://brv.zhongyouzk.top

[O06] 使用进程池
来源：http://wnz.shuidangran.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://buc.yvedp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ucv.hfpthk.cn

JS:   // child_process / cluster 模块
来源：http://msg.epnwcf.com

TS:   // child_process / cluster 模块
来源：http://iqb.c1oappe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://aox.cheryme.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bgt.yvedp.cn

Ruby: // fork 块
来源：http://sha.yuxming.cn

C#:   Parallel.For
来源：http://baw.hfpthk.cn

================================================================================
来源：http://hhp.iojbl.cn

P. 常用工具函数
来源：http://nph.shangyingyoupin.top

================================================================================
来源：http://fpv.zhijiandao.cn

[P01] 生成 UUID
来源：http://cmv.hongshengwenyu.top

Py:   str(uuid.uuid4())
来源：http://dnj.daria6918.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tum.iojbl.cn

JS:   crypto.randomUUID()
来源：http://udk.jqgufenzy.top

TS:   crypto.randomUUID()
来源：http://fog.xuanzx.com

Java: UUID.randomUUID().toString()
来源：http://idf.hnxiangtu.top

Go:   // 用 github.com/google/uuid
来源：http://ruo.jinghuilouyu.cn

Ruby: SecureRandom.uuid
来源：http://dnv.ydzc1.top

C#:   Guid.NewGuid().ToString()
来源：http://une.0kj1m.cn

[P02] MD5 / SHA256 摘要
来源：http://ell.ydzc1.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kzm.zhongyouzk.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://trx.jiagoushi.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hqd.iojbl.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rqq.ppjwa.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mfo.smart0.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kfw.meibo888.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ccn.yuxming.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ami.sjlbkw.cn

[P03] 生成短随机字符串
来源：http://tvz.hongshengwenyu.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xwx.aizwys.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gse.yj20258.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cxz.iojbl.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://stm.feifeiyinyue.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hsv.316326.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kyx.wangdashe.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://evb.dashuyun.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xlx.chenlongwang.top

[P04] 求长度
来源：http://jtw.jqgfzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ole.jlsjyb.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ufj.smart0.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ilv.tarul.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fra.hcnkem.com

Java: list.size();  map.size();  s.length()
来源：http://uga.jlsjyb.cn

Go:   len(arr);  len(m)
来源：http://xtf.xinyue.icu

Ruby: x.length;  x.size
来源：http://cwz.ywan-chungtsiang.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ywa.dashuyun.cn

[P05] 判断两个对象内容是否相等
来源：http://bsj.zhixingplan.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://gqf.wangdashe.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lxr.shanyushiyangkeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kcm.sufxvd.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eyi.uphjek.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fbo.svipenyu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ddu.yj202588.top

Ruby: a == b
来源：http://qvo.xylfe.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qve.9152youxi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bsp.316326.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qbw.guannengcc.top

PHP:  if (empty($x)) {}
来源：http://kuh.chenlongwang.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xar.zhijiandao.cn

TS:   if (x == null) {}
来源：http://drj.ywan-chungtsiang.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wtg.jinqigufen.top

Go:   if x == nil {}
来源：http://xib.dianchejie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://evp.gaohongyu789.top

C#:   if (x is null) {}
来源：http://xfp.guowangkeji.top

[P07] 防抖与节流
来源：http://qxs.andypj.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://eef.hnqzz.top

PHP:  // 手写时间戳比较
来源：http://lpm.vehdjk.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zzv.daxiang520.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mwq.zdbjq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hcv.havefunace.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zko.shanyushiyangkeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://fjk.yj202588.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://say.0kj1m.cn

[P08] 处理浮点精度问题
来源：http://nef.sysykeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fxw.xingfuxueyuan.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bty.jiagoushi.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ntr.ybcxt.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rkm.yj20258888.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tey.nanxuanxn.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tip.hnqzz.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wje.xuanzx.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nzz.gaohongyu789.top

================================================================================
来源：http://bbn.bjfxy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xxt.jqgfzy.top

================================================================================
来源：http://ryu.sjlbkw.cn

[Q01] 创建表
来源：http://opv.wangshuangyany.cn

CREATE TABLE users (
来源：http://eog.fzhhl.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hrg.fanxiaobao.xyz

name VARCHAR(50) NOT NULL,
来源：http://rkm.cheryme.top

email VARCHAR(100) UNIQUE,
来源：http://bnr.pengpengdd.cyou

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gpf.wangshuangyany.cn

);
来源：http://ylx.cashguo.top

[Q02] 创建带外键的表
来源：http://jya.xuetiantiany.cn

CREATE TABLE orders (
来源：http://lyz.xinyue.icu

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bme.fengsongda.top

user_id INT NOT NULL,
来源：http://zvw.nanxuanxn.top

amount DECIMAL(10, 2),
来源：http://ecy.jianghu66.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ltr.yj202588.top

);
来源：http://pjb.zdbjq.cn

[Q03] 增加列
来源：http://qyk.yanxiufei.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jdk.ctjpmb.com

[Q04] 修改列类型
来源：http://jap.9152youxi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tnn.svipenyu.cn

[Q05] 重命名列
来源：http://okh.vqdsnc.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ygk.fktsv.cn

[Q06] 删除列
来源：http://kyu.guowangkeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://ajn.yj20258888.top

[Q07] 删除表
来源：http://avy.aizwys.cn

DROP TABLE IF EXISTS orders;
来源：http://tuq.yuxming.cn

[Q08] 创建普通索引
来源：http://pbk.zdqjudy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://yfk.guowangkeji.top

[Q09] 创建唯一索引
来源：http://ojj.mhx1999.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xex.sjlbkw.cn

[Q10] 插入单行
来源：http://clk.yanxiufei.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fpr.jinyuanbaomall.cn

[Q11] 一次插入多行
来源：http://ljd.shanyushiyangkeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xqh.dashuyun.cn

[Q12] 插入后取自增 ID
来源：http://htr.cheryme.top

INSERT INTO users (name) VALUES ('C');
来源：http://bym.xuetiantiany.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pyx.sufxvd.cn

[Q13] 忽略重复插入
来源：http://aac.xinyue.icu

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mjf.0kj1m.cn


<!-- 参考信息 -->