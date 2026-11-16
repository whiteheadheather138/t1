代发 wailian999

Java: public static void main(String[] args)
来源：http://ccu.birdmap.top

Go:   func main()
来源：http://wjf.guowangkeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://soi.jlsjyb.cn

C#:   static void Main(string[] args)
来源：http://ofh.shanyushiyangtech.top

[M08] 获取系统与运行时信息
来源：http://doz.iojbl.cn

Py:   platform.system();  platform.python_version()
来源：http://ppg.jlsjyb.cn

PHP:  PHP_OS;  phpversion();
来源：http://kci.yongpay.top

JS:   process.platform;  process.version
来源：http://doc.sysykeji.top

TS:   process.platform;  process.version
来源：http://giz.tanke756.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kmv.fanxiaobao.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://ewy.xingfuxueyuan.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dog.birdmap.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://zru.ydzc1.top

================================================================================
来源：http://one.c1oappe.top

N. 数据结构与算法
来源：http://jwc.zhijiandao.cn

================================================================================
来源：http://sox.gzhubu.top

[N01] 二分查找（有序数组）
来源：http://cqv.yueranfly.top

Py:   bisect.bisect_left(arr, x)
来源：http://kvr.guannengcc.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dlp.ctjpmb.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zoq.zhijiandao.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yyk.shanyushiyangkeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://vii.shuidangran.top

Go:   sort.SearchInts(arr, x)
来源：http://fyf.xuanzx.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://iab.nwbrower.top

C#:   Array.BinarySearch(arr, x)
来源：http://xir.cqqwz.cn

[N02] 排序（工程实践用内置实现）
来源：http://eaq.nanxuanxn.top

Py:   sorted(arr);  arr.sort()
来源：http://mer.yj20258888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wdb.ydjk.org.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ecr.ehwqpu.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://obo.vehdjk.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vbj.hysaishi.cn

Go:   slices.Sort(arr)
来源：http://ygz.cashguo.top

Ruby: arr.sort
来源：http://gmv.hfpthk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mml.shanyushiyangkeji.top

[N03] 快速排序（分治示例）
来源：http://jzp.yfazqb.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://drf.ydjk.org.cn

PHP:  // 递归实现，或用 usort
来源：http://tpm.andypj.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kdz.aibaodan.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kmx.zhaomingkeji.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sjm.nanxuanxn.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zdb.ivvv.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yat.birdmap.top

C#:   // 手写递归，或 Array.Sort
来源：http://ths.ehwqpu.com

[N04] 斐波那契数列
来源：http://rps.gaohongyu789.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sng.hongshengwenyu.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xmi.daria6918.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kww.pycfn.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ofu.hnxiangtu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hnj.redwolf501.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rcj.316326.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rxv.shanyushiyangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://upv.mhx1999.top

[N05] 最大公约数
来源：http://fgl.shuidangran.top

Py:   math.gcd(a, b)
来源：http://hqm.yj20258888.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ckh.yuxming.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aju.zhiwuduotai.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zxw.fehbvm.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xvy.9152youxi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xlx.jinqigufen.top

Ruby: a.gcd(b)
来源：http://dsn.chenjidiqi.icu

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tyq.jlsjyb.cn

[N06] 判断回文字符串
来源：http://anx.zdbjq.cn

Py:   s == s[::-1]
来源：http://qaa.tarul.cn

PHP:  $s === strrev($s);
来源：http://nox.cheryme.top

JS:   s === [...s].reverse().join("")
来源：http://btg.yanxiufei.cn

TS:   s === [...s].reverse().join("")
来源：http://hfh.zhengqikj.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wmf.cqqwz.cn

Go:   // 双指针从两端比较
来源：http://dbb.gotoacloud.top

Ruby: s == s.reverse
来源：http://kfv.xuanzx.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://bnr.aizwys.cn

[N07] 两数之和（返回下标）
来源：http://zmi.jqgfzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kvr.zhiwuduotai.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://thz.gogol.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://aex.zdbjq.cn

TS:   // 手写 Map<string, number>
来源：http://wsa.ywan-chungtsiang.top

Java: // 手写 HashMap
来源：http://keo.gzhubu.top

Go:   // 手写 map[int]int
来源：http://zmj.zhiwuduotai.top

Ruby: // 手写 Hash
来源：http://rhj.wangshuangyany.cn

C#:   // 手写 Dictionary<int, int>
来源：http://umy.uphjek.com

[N08] 生成全排列
来源：http://cqh.smart0.xyz

Py:   itertools.permutations(arr)
来源：http://jon.52xcode.cn

PHP:  // 手写递归交换
来源：http://fdf.jqgfzy.top

JS:   // 手写回溯递归
来源：http://gpu.ywan-chungtsiang.top

TS:   // 手写回溯递归
来源：http://rky.cdnleiting.top

Java: // 手写回溯递归
来源：http://tby.ppjwa.cn

Go:   // 手写回溯递归
来源：http://zdn.fehbvm.com

Ruby: arr.permutation.to_a
来源：http://ltc.nwbrower.top

C#:   // 手写回溯递归
来源：http://kod.ehwqpu.com

[N09] 栈与队列
来源：http://wki.svipenyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ecp.jinqigufen.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wbx.gotoacloud.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nir.hammf.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bjy.zycfv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ofn.hnqzz.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://glb.guannengcc.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://aby.shanyushiyangkeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wfk.yj202588.top

[N10] 链表节点定义
来源：http://wat.hnxiangtu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bec.gotoacloud.top

PHP:  class Node { public $v; public $next = null; }
来源：http://mvf.nanxinkj.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cke.vqdsnc.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gpv.epnwcf.com

Java: class Node { int v; Node next; }
来源：http://vvq.jinyuanbaomall.cn

Go:   type Node struct { V int; Next *Node }
来源：http://com.birdmap.top

Ruby: Node = Struct.new(:v, :next)
来源：http://alh.hfpthk.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lkm.yangfankeji.com

[N11] 二叉树中序遍历
来源：http://drx.zhixingplan.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://djf.0kj1m.cn

PHP:  // 手写递归函数
来源：http://plu.316326.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://edb.shzxlz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dxj.tian-w.cn

Java: // 手写递归
来源：http://sue.pycfn.com

Go:   // 手写递归
来源：http://who.yangfankeji.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nhb.gaohongyu789.top

C#:   // 手写递归
来源：http://kby.wangdashe.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uek.ydzc1.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://srj.xuetiantiany.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gfm.iojbl.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://evj.gotoacloud.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uwa.hesvh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ixk.quarkkingdee.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qcn.haohaochexian.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gkk.yuanzhike.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dsj.zdbjq.cn

================================================================================
来源：http://gtq.gogol.net.cn

O. 并发与异步
来源：http://yhg.zdqjudy.top

================================================================================
来源：http://lka.jqgufenzy.top

[O01] 启动一个线程
来源：http://qbc.shuidangran.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qoe.c1oappe.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hvq.chenlongwang.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dly.pengpengdd.cyou

TS:   // 同 JS
来源：http://unh.shanyushiyangkeji.top

Java: new Thread(() -> f()).start()
来源：http://atu.fktsv.cn

Go:   go f()
来源：http://ggc.jinqigufen.top

Ruby: Thread.new { f }
来源：http://szj.fzhhl.top

C#:   Task.Run(() => F());
来源：http://abp.ywan-chungtsiang.top

[O02] 使用线程池
来源：http://qjr.ctjpmb.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ndp.hesvh.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://aso.zhaomingkeji.xyz

JS:   // worker_threads 线程池
来源：http://rbz.xuetiantiany.cn

TS:   // worker_threads 线程池
来源：http://zbl.zhaomingkeji.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://jmh.dashuyun.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xpn.feifeiyinyue.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://odw.smart0.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xyg.iojbl.cn

[O03] 加锁保护共享数据
来源：http://ano.xingfuxueyuan.xyz

Py:   with lock: shared += 1
来源：http://ogt.pengpengdd.cyou

PHP:  // 用 flock() 做文件锁
来源：http://cws.zhixingplan.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sae.wangdashe.top

TS:   // 同 JS
来源：http://ltl.snrcjt.cn

Java: synchronized (this) { shared++; }
来源：http://tai.jinghuilouyu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://znt.sysykeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://uxu.aibaodan.cn

C#:   lock (gate) { shared++; }
来源：http://tch.guannengcc.top

[O04] 定义异步函数并等待
来源：http://whn.yongpay.top

Py:   async def f():⏎    await g()
来源：http://mqp.yueranfly.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lct.fzhhl.top

JS:   async function f() { await g(); }
来源：http://ida.redwolf501.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://pxl.hfpthk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://for.sweek.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cum.yvedp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://poc.jiagoushi.top

C#:   async Task F() { await G(); }
来源：http://zxm.zhiwuduotai.top

[O05] 并发执行并等待全部完成
来源：http://xve.shanyushiyangkeji.top

Py:   asyncio.gather(*tasks)
来源：http://hsm.wangshuangyany.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fik.wangdashe.top

JS:   await Promise.all(tasks)
来源：http://awt.andypj.xyz

TS:   await Promise.all(tasks)
来源：http://say.jqgfzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://thu.gzhubu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wtv.shzxlz.cn

Ruby: threads.map(&:join)
来源：http://lfm.nanxuanxn.top

C#:   await Task.WhenAll(t1, t2)
来源：http://osf.sweek.top

[O06] 使用进程池
来源：http://yhq.quarkkingdee.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://llo.zhengqikj.top

PHP:  // pcntl_fork 或多进程队列
来源：http://xrn.yuanzhike.top

JS:   // child_process / cluster 模块
来源：http://zjm.jqgfzy.top

TS:   // child_process / cluster 模块
来源：http://shg.hesvh.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://izv.cucudq.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cua.guannengcc.top

Ruby: // fork 块
来源：http://qak.shangyingyoupin.top

C#:   Parallel.For
来源：http://njk.aibaodan.cn

================================================================================
来源：http://sjz.jinqigufen.top

P. 常用工具函数
来源：http://mir.xylfe.cn

================================================================================
来源：http://blu.yueranfly.top

[P01] 生成 UUID
来源：http://sat.yuxming.cn

Py:   str(uuid.uuid4())
来源：http://smz.jinyuanbaomall.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hhv.zdbjq.cn

JS:   crypto.randomUUID()
来源：http://hqm.xuetiantiany.cn

TS:   crypto.randomUUID()
来源：http://kxj.hesvh.cn

Java: UUID.randomUUID().toString()
来源：http://vbz.yueranfly.top

Go:   // 用 github.com/google/uuid
来源：http://tct.chenzaomai.com

Ruby: SecureRandom.uuid
来源：http://stz.quarkkingdee.top

C#:   Guid.NewGuid().ToString()
来源：http://fac.bbcook.cn

[P02] MD5 / SHA256 摘要
来源：http://xgo.jinyuanbaomall.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wuq.vqdsnc.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ktz.sxryk.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ora.gotoacloud.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ruw.hnxiangtu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yua.sweek.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xgr.c1oappe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vyo.wangshuangyany.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jcy.kuanghao11.cn

[P03] 生成短随机字符串
来源：http://mjl.hammf.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dne.shanyushiyangkeji.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mwj.bbcook.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://awe.svipenyu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://exa.sjlbkw.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cfk.zhengqikj.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vxm.9152youxi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://tne.gogol.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tah.xziqi.cn

[P04] 求长度
来源：http://nkw.hcnkem.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pca.svipenyu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nrt.shangyingyoupin.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bmu.snrcjt.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://edn.hnqzz.top

Java: list.size();  map.size();  s.length()
来源：http://zwq.jyoumei.cn

Go:   len(arr);  len(m)
来源：http://xsg.feifeiyinyue.top

Ruby: x.length;  x.size
来源：http://dod.fehbvm.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://jbi.tarul.cn

[P05] 判断两个对象内容是否相等
来源：http://bjk.xinyue.icu

Py:   a == b              # 列表与字典递归比较内容
来源：http://urw.smart0.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dyk.zdbjq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hpe.vehdjk.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://scg.iojbl.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cab.dashuyun.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jkw.pengpengdd.cyou

Ruby: a == b
来源：http://diy.aibaodan.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tdn.pycfn.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sqj.zdqjudy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pvk.cashguo.top

PHP:  if (empty($x)) {}
来源：http://ftw.guowangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xqg.iojbl.cn

TS:   if (x == null) {}
来源：http://zfj.zhaomingkeji.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://fkg.tian-w.cn

Go:   if x == nil {}
来源：http://fia.ctjpmb.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hjk.sufxvd.cn

C#:   if (x is null) {}
来源：http://fnl.ppjwa.cn

[P07] 防抖与节流
来源：http://ust.c1oappe.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tbt.nanxuanxn.top

PHP:  // 手写时间戳比较
来源：http://pcz.fzhhl.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jod.pycfn.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nlc.sweek.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mii.nanxuanxn.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://iem.fengsongda.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zzj.shzxlz.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://llh.ehwqpu.com

[P08] 处理浮点精度问题
来源：http://fcr.vehdjk.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hph.tianlin.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://svw.kuanghao11.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hom.yfazqb.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://utc.yongpay.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lbu.uphjek.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pxj.daxiang520.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ivn.ctjpmb.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://chc.jqgufenzy.top

================================================================================
来源：http://swz.zhaomingkeji.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zlt.gogol.net.cn

================================================================================
来源：http://joj.hnqzz.top

[Q01] 创建表
来源：http://cub.cdnleiting.top

CREATE TABLE users (
来源：http://eze.bjfxy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qko.bjfxy.top

name VARCHAR(50) NOT NULL,
来源：http://wfh.zhongyouzk.top

email VARCHAR(100) UNIQUE,
来源：http://hih.hcnkem.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nle.iojbl.cn

);
来源：http://psm.iojbl.cn

[Q02] 创建带外键的表
来源：http://fjh.hesvh.cn

CREATE TABLE orders (
来源：http://sdc.zhengqikj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nxt.jyoumei.cn

user_id INT NOT NULL,
来源：http://mem.cashguo.top

amount DECIMAL(10, 2),
来源：http://dse.zdqjudy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rsk.vehdjk.com

);
来源：http://hzx.jinqigfzy.top

[Q03] 增加列
来源：http://axb.xylfe.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dcz.nwbrower.top

[Q04] 修改列类型
来源：http://fgi.zdqjudy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://veo.haohaochexian.top

[Q05] 重命名列
来源：http://oxo.shanyushiyangtech.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://epp.xinyue.icu

[Q06] 删除列
来源：http://jwr.sufxvd.cn

ALTER TABLE users DROP COLUMN age;
来源：http://riv.smart0.xyz

[Q07] 删除表
来源：http://vft.fktsv.cn

DROP TABLE IF EXISTS orders;
来源：http://vwj.uphjek.com

[Q08] 创建普通索引
来源：http://rqi.wangdashe.top

CREATE INDEX idx_users_email ON users(email);
来源：http://uau.chenlongwang.top

[Q09] 创建唯一索引
来源：http://qpy.havefunace.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mes.kuanghao11.cn

[Q10] 插入单行
来源：http://fng.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uce.hnxiangtu.top

[Q11] 一次插入多行
来源：http://kdw.fehbvm.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cap.bjfxy.top

[Q12] 插入后取自增 ID
来源：http://fub.mhx1999.top

INSERT INTO users (name) VALUES ('C');
来源：http://zrr.fzhhl.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gjy.fktsv.cn

[Q13] 忽略重复插入
来源：http://rol.52xcode.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://imk.yongpay.top

[Q14] 存在则更新（upsert）
来源：http://hrl.cucudq.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pmg.sweek.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fel.yj20258.top

[Q15] 查询全部
来源：http://gtx.pengpengdd.cyou


<!-- 参考信息 -->