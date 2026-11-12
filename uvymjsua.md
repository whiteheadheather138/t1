代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://uhf.quarkkingdee.top

================================================================================
来源：http://jfh.xingfuxueyuan.xyz

N. 数据结构与算法
来源：http://nhg.iojbl.cn

================================================================================
来源：http://nud.yangfankeji.com

[N01] 二分查找（有序数组）
来源：http://ldc.jqgfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://vuv.nwbrower.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ncv.cucudq.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vrq.bbcook.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rpn.zhengqikj.top

Java: Arrays.binarySearch(arr, x)
来源：http://yxy.dianchejie.cn

Go:   sort.SearchInts(arr, x)
来源：http://xle.zhixingplan.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xyz.gotoacloud.top

C#:   Array.BinarySearch(arr, x)
来源：http://hgs.jinghuilouyu.cn

[N02] 排序（工程实践用内置实现）
来源：http://ipq.zhixingplan.top

Py:   sorted(arr);  arr.sort()
来源：http://uat.tanke756.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://njr.vqdsnc.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rvd.feifeiyinyue.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kay.ydjk.org.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gjb.zhixingplan.top

Go:   slices.Sort(arr)
来源：http://bnr.zhongyouzk.top

Ruby: arr.sort
来源：http://lnm.shanyushiyangtech.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://gfr.xziqi.cn

[N03] 快速排序（分治示例）
来源：http://clc.svipenyu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jik.hnqzz.top

PHP:  // 递归实现，或用 usort
来源：http://nbs.sxryk.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pjm.zhoulong.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://elj.ybcxt.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://siy.ydjk.org.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://obs.yangfankeji.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://oxq.chenjidiqi.icu

C#:   // 手写递归，或 Array.Sort
来源：http://qlv.fengsongda.top

[N04] 斐波那契数列
来源：http://ozf.daria6918.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://oje.tian-w.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bzd.xingfuxueyuan.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://esr.dashuyun.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://azs.316326.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ksr.guannengcc.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bmg.jinqigufen.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zvg.cucudq.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sbm.fanxiaobao.xyz

[N05] 最大公约数
来源：http://mvi.bjfxy.top

Py:   math.gcd(a, b)
来源：http://tbb.yueranfly.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rid.ydjk.org.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://usi.jqgufenzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jja.gogol.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fvx.xuanzx.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gea.daria6918.cn

Ruby: a.gcd(b)
来源：http://yxa.xingfuxueyuan.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ase.jiagoushi.top

[N06] 判断回文字符串
来源：http://nqw.yj20258.top

Py:   s == s[::-1]
来源：http://mdl.yvedp.cn

PHP:  $s === strrev($s);
来源：http://pjm.bbcook.cn

JS:   s === [...s].reverse().join("")
来源：http://gdj.daria6918.cn

TS:   s === [...s].reverse().join("")
来源：http://ckc.ppjwa.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hcn.yangfankeji.com

Go:   // 双指针从两端比较
来源：http://ojq.yanxiufei.cn

Ruby: s == s.reverse
来源：http://hab.jinqigufen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://uqb.aizwys.cn

[N07] 两数之和（返回下标）
来源：http://bel.daxiang520.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mqv.daxiang520.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://olh.dianchejie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://buq.c1oappe.top

TS:   // 手写 Map<string, number>
来源：http://nth.yanxiufei.cn

Java: // 手写 HashMap
来源：http://wqw.yangfankeji.com

Go:   // 手写 map[int]int
来源：http://wup.tianlin.xyz

Ruby: // 手写 Hash
来源：http://ljp.svipenyu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://uyz.zdqjudy.top

[N08] 生成全排列
来源：http://ljn.hongshengwenyu.top

Py:   itertools.permutations(arr)
来源：http://bnh.shzxlz.cn

PHP:  // 手写递归交换
来源：http://xof.shanyushiyangtech.top

JS:   // 手写回溯递归
来源：http://mbw.cashguo.top

TS:   // 手写回溯递归
来源：http://gse.andypj.xyz

Java: // 手写回溯递归
来源：http://qff.jianghu66.top

Go:   // 手写回溯递归
来源：http://jvi.316326.xyz

Ruby: arr.permutation.to_a
来源：http://jxp.wangdashe.top

C#:   // 手写回溯递归
来源：http://mkk.jinqigufen.top

[N09] 栈与队列
来源：http://yzv.sysykeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fcr.xingfuxueyuan.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yqv.daria6918.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pmt.tarul.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://akb.bjfxy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fbd.daxiang520.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bwt.shzxlz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wkw.shangyingyoupin.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bgw.wangshuangyany.cn

[N10] 链表节点定义
来源：http://hbt.yvedp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fuc.52xcode.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fno.0kj1m.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://woh.cdnleiting.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tty.shanyushiyangtech.top

Java: class Node { int v; Node next; }
来源：http://fah.zycfv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fbo.xziqi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zer.dashuyun.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zyo.epnwcf.com

[N11] 二叉树中序遍历
来源：http://ojs.zdbjq.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kgq.sweek.top

PHP:  // 手写递归函数
来源：http://zlo.52xcode.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qmp.sufxvd.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uqm.tian-w.cn

Java: // 手写递归
来源：http://mwa.fengsongda.top

Go:   // 手写递归
来源：http://dbl.pengpengdd.cyou

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tot.gogol.net.cn

C#:   // 手写递归
来源：http://xgn.yj202588.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jbi.ctjpmb.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ytr.shanyushiyangkeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jxy.daxiang520.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://unb.yuxming.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vwa.zhiwuduotai.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tgo.cucudq.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hev.9152youxi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dyg.zhiwuduotai.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://urx.wangdashe.top

================================================================================
来源：http://bmm.cheryme.top

O. 并发与异步
来源：http://qnw.cqqwz.cn

================================================================================
来源：http://iah.jlsjyb.cn

[O01] 启动一个线程
来源：http://kxy.cashguo.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pex.ywan-chungtsiang.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vho.gaohongyu789.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blb.aibaodan.cn

TS:   // 同 JS
来源：http://qcy.chenzaomai.com

Java: new Thread(() -> f()).start()
来源：http://wzs.gzhubu.top

Go:   go f()
来源：http://tuq.sysykeji.top

Ruby: Thread.new { f }
来源：http://tjt.andypj.xyz

C#:   Task.Run(() => F());
来源：http://nmx.fehbvm.com

[O02] 使用线程池
来源：http://hgi.shangyingyoupin.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dyj.zdqjudy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vkb.sysykeji.top

JS:   // worker_threads 线程池
来源：http://lta.yvedp.cn

TS:   // worker_threads 线程池
来源：http://muk.jinghuilouyu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qws.gogol.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sjo.jinyuanbaomall.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nky.hysaishi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fdw.hfpthk.cn

[O03] 加锁保护共享数据
来源：http://iai.yonumen.top

Py:   with lock: shared += 1
来源：http://vat.jinqigfzy.top

PHP:  // 用 flock() 做文件锁
来源：http://avc.cqqwz.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vsf.jinqigufen.top

TS:   // 同 JS
来源：http://fvr.jqgfzy.top

Java: synchronized (this) { shared++; }
来源：http://edh.zhaomingkeji.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://iet.iojbl.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qof.xuetiantiany.cn

C#:   lock (gate) { shared++; }
来源：http://fdk.9152youxi.cn

[O04] 定义异步函数并等待
来源：http://wjx.ivvv.top

Py:   async def f():⏎    await g()
来源：http://lnd.9152youxi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rhl.chenjidiqi.icu

JS:   async function f() { await g(); }
来源：http://ids.quarkkingdee.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://npz.sufxvd.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sce.cheryme.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rsc.shzxlz.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jkm.gogol.net.cn

C#:   async Task F() { await G(); }
来源：http://jtb.cucudq.cn

[O05] 并发执行并等待全部完成
来源：http://ted.hnxiangtu.top

Py:   asyncio.gather(*tasks)
来源：http://eog.cdnleiting.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lwh.ivvv.top

JS:   await Promise.all(tasks)
来源：http://rnh.ywan-chungtsiang.top

TS:   await Promise.all(tasks)
来源：http://ryt.ehwqpu.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cxb.hongshengwenyu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://paz.havefunace.top

Ruby: threads.map(&:join)
来源：http://rgr.jqgufenzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://gvy.316326.xyz

[O06] 使用进程池
来源：http://yhs.shanyushiyangtech.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yge.chenjidiqi.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://hwy.cashguo.top

JS:   // child_process / cluster 模块
来源：http://mmj.wangshuangyany.cn

TS:   // child_process / cluster 模块
来源：http://nuf.9152youxi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nbt.yanxiufei.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://maw.sxryk.cn

Ruby: // fork 块
来源：http://bqb.xylfe.cn

C#:   Parallel.For
来源：http://rgk.yuanzhike.top

================================================================================
来源：http://aan.kuanghao11.cn

P. 常用工具函数
来源：http://vzf.jyoumei.cn

================================================================================
来源：http://frp.cheryme.top

[P01] 生成 UUID
来源：http://fbf.yfazqb.com

Py:   str(uuid.uuid4())
来源：http://uof.zycfv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zli.xuetiantiany.cn

JS:   crypto.randomUUID()
来源：http://vvf.zhongyouzk.top

TS:   crypto.randomUUID()
来源：http://fvx.xingfuxueyuan.xyz

Java: UUID.randomUUID().toString()
来源：http://zzu.jinqigfzy.top

Go:   // 用 github.com/google/uuid
来源：http://rkh.guowangkeji.top

Ruby: SecureRandom.uuid
来源：http://kgm.birdmap.top

C#:   Guid.NewGuid().ToString()
来源：http://xlr.fengsongda.top

[P02] MD5 / SHA256 摘要
来源：http://fsj.yj20258.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ysp.gogol.net.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://dtm.shangyingyoupin.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zdn.tian-w.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ddy.xuetiantiany.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nvi.c1oappe.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pgq.shangyingyoupin.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lhu.cdnleiting.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sgp.sjlbkw.cn

[P03] 生成短随机字符串
来源：http://pnw.yj202588.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ziz.hnqzz.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yib.xylfe.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nhq.tanke756.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aog.fktsv.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fuw.hywenlv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xni.9152youxi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wsi.fehbvm.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://skn.yj20258888.top

[P04] 求长度
来源：http://acm.zhoulong.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fxh.zhiwuduotai.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hsr.shangyingyoupin.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://det.yanxiufei.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ukw.hesvh.cn

Java: list.size();  map.size();  s.length()
来源：http://xws.xziqi.cn

Go:   len(arr);  len(m)
来源：http://vpe.redwolf501.top

Ruby: x.length;  x.size
来源：http://xvy.gogol.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://swp.redwolf501.top

[P05] 判断两个对象内容是否相等
来源：http://ymt.zhijiandao.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pgv.zhoulong.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wxb.gotoacloud.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://arh.guowangkeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://iwe.redwolf501.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hvn.havefunace.top

Go:   reflect.DeepEqual(a, b)
来源：http://eyx.sweek.top

Ruby: a == b
来源：http://yyv.jiagoushi.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fso.daria6918.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://svv.kuanghao11.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ath.ivvv.top

PHP:  if (empty($x)) {}
来源：http://tfq.hnqzz.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://osy.yuanzhike.top

TS:   if (x == null) {}
来源：http://dkk.shanyushiyangkeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://rjt.tarul.cn

Go:   if x == nil {}
来源：http://cdf.andypj.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fbh.xuanzx.com

C#:   if (x is null) {}
来源：http://ukk.tian-w.cn

[P07] 防抖与节流
来源：http://imi.gaohongyu789.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kpl.c1oappe.top

PHP:  // 手写时间戳比较
来源：http://piu.meibo888.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rtg.kuanghao11.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uba.yanxiufei.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fcm.kuanghao11.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wpu.jinyuanbaomall.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://saz.yonumen.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zgn.quarkkingdee.top

[P08] 处理浮点精度问题
来源：http://hze.sxryk.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://idx.uphjek.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nxy.yfazqb.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wwq.shangyingyoupin.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vgt.cqqwz.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ulu.ydzc1.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cze.gaohongyu789.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lxl.316326.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sgr.jinyuanbaomall.cn

================================================================================
来源：http://csc.9152youxi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hhn.feifeiyinyue.top

================================================================================
来源：http://evv.xuetiantiany.cn

[Q01] 创建表
来源：http://rzf.xuetiantiany.cn

CREATE TABLE users (
来源：http://cpu.wangshuangyany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wfh.yueranfly.top

name VARCHAR(50) NOT NULL,
来源：http://fzt.yfazqb.com

email VARCHAR(100) UNIQUE,
来源：http://ctf.jiagoushi.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ehm.vqdsnc.cn

);
来源：http://kti.yj20258888.top

[Q02] 创建带外键的表
来源：http://duu.meibo888.top

CREATE TABLE orders (
来源：http://omd.ehwqpu.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nql.shanyushiyangtech.top

user_id INT NOT NULL,
来源：http://jmi.yangfankeji.com

amount DECIMAL(10, 2),
来源：http://aqu.cdnleiting.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ooh.vqdsnc.cn

);
来源：http://caq.chenlongwang.top

[Q03] 增加列
来源：http://jzq.yuanzhike.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yxb.ydzc1.top

[Q04] 修改列类型
来源：http://mlt.tanke756.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dkm.aizwys.cn

[Q05] 重命名列
来源：http://ivi.iojbl.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://skz.guowangkeji.top

[Q06] 删除列
来源：http://cmi.quarkkingdee.top

ALTER TABLE users DROP COLUMN age;
来源：http://ser.birdmap.top

[Q07] 删除表
来源：http://xbq.sysykeji.top

DROP TABLE IF EXISTS orders;
来源：http://geh.fzhhl.top

[Q08] 创建普通索引
来源：http://jni.sxryk.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://tvb.guannengcc.top

[Q09] 创建唯一索引
来源：http://wad.bjfxy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://agw.yonumen.top

[Q10] 插入单行
来源：http://mdy.aizwys.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cxg.fehbvm.com

[Q11] 一次插入多行
来源：http://dat.jinghuilouyu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zbu.hammf.cn

[Q12] 插入后取自增 ID
来源：http://cdg.jqgufenzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://wbb.mhx1999.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rzi.cashguo.top

[Q13] 忽略重复插入
来源：http://xcr.andypj.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mow.sufxvd.cn

[Q14] 存在则更新（upsert）
来源：http://vdv.316326.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://umo.zdqjudy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://slr.xuetiantiany.cn

[Q15] 查询全部
来源：http://swp.birdmap.top

SELECT * FROM users;
来源：http://rig.gaohongyu789.top

[Q16] 查询指定列
来源：http://rxo.shuidangran.top

SELECT id, name FROM users;
来源：http://sam.hfpthk.cn

[Q17] 条件查询
来源：http://dyn.jyoumei.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cro.andypj.xyz

[Q18] 模糊匹配
来源：http://bmf.316326.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sxk.haohaochexian.top

[Q19] 范围查询
来源：http://zfz.yanxiufei.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xuq.daxiang520.top

[Q20] IN 列表
来源：http://qep.jqgufenzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mzb.sweek.top

[Q21] 空值判断
来源：http://rmp.gogol.net.cn


<!-- 参考信息 -->