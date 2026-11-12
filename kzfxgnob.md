代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://yvg.zhixingplan.top

[N02] 排序（工程实践用内置实现）
来源：http://nlm.hcnkem.com

Py:   sorted(arr);  arr.sort()
来源：http://yfc.hongshengwenyu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pmp.zhaomingkeji.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://aaw.zycfv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://imr.shangyingyoupin.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jgs.zhiwuduotai.top

Go:   slices.Sort(arr)
来源：http://efh.shuidangran.top

Ruby: arr.sort
来源：http://fba.snrcjt.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://uii.nwbrower.top

[N03] 快速排序（分治示例）
来源：http://drd.ywan-chungtsiang.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wuw.gzhubu.top

PHP:  // 递归实现，或用 usort
来源：http://xbt.vehdjk.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cba.dashuyun.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gyg.yj20258.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sio.zhengqikj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jda.gzhubu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tjd.ctjpmb.com

C#:   // 手写递归，或 Array.Sort
来源：http://bja.xuetiantiany.cn

[N04] 斐波那契数列
来源：http://wtr.nanxinkj.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ilc.yj202588.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gpb.shangyingyoupin.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ihz.zycfv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wzq.havefunace.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://eyv.316326.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nrl.yfazqb.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nxk.havefunace.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://avv.yuxming.cn

[N05] 最大公约数
来源：http://orr.ydjk.org.cn

Py:   math.gcd(a, b)
来源：http://xrr.daria6918.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lfz.hammf.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://diw.quarkkingdee.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pfk.hnqzz.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bht.zycfv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fns.jyoumei.cn

Ruby: a.gcd(b)
来源：http://sbp.chenlongwang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jzv.feifeiyinyue.top

[N06] 判断回文字符串
来源：http://pey.yangfankeji.com

Py:   s == s[::-1]
来源：http://avv.pengpengdd.cyou

PHP:  $s === strrev($s);
来源：http://ukg.epnwcf.com

JS:   s === [...s].reverse().join("")
来源：http://ksg.zhengqikj.top

TS:   s === [...s].reverse().join("")
来源：http://adu.ybcxt.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qgs.0kj1m.cn

Go:   // 双指针从两端比较
来源：http://rsc.ywan-chungtsiang.top

Ruby: s == s.reverse
来源：http://lft.tianlin.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://wij.52xcode.cn

[N07] 两数之和（返回下标）
来源：http://het.chenjidiqi.icu

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zra.aibaodan.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://num.birdmap.top

JS:   // 手写 Map：map.set(v, i)
来源：http://llm.havefunace.top

TS:   // 手写 Map<string, number>
来源：http://kqm.ydjk.org.cn

Java: // 手写 HashMap
来源：http://iyq.gogol.net.cn

Go:   // 手写 map[int]int
来源：http://sce.shuidangran.top

Ruby: // 手写 Hash
来源：http://bxf.shanyushiyangtech.top

C#:   // 手写 Dictionary<int, int>
来源：http://fop.jlsjyb.cn

[N08] 生成全排列
来源：http://yav.zdbjq.cn

Py:   itertools.permutations(arr)
来源：http://cqm.zhaomingkeji.xyz

PHP:  // 手写递归交换
来源：http://qby.pycfn.com

JS:   // 手写回溯递归
来源：http://nvx.shanyushiyangkeji.top

TS:   // 手写回溯递归
来源：http://fkl.jianghu66.top

Java: // 手写回溯递归
来源：http://ebl.smart0.xyz

Go:   // 手写回溯递归
来源：http://nix.hnxiangtu.top

Ruby: arr.permutation.to_a
来源：http://spz.vqdsnc.cn

C#:   // 手写回溯递归
来源：http://bbn.zdbjq.cn

[N09] 栈与队列
来源：http://kdr.gaohongyu789.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pok.pycfn.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qzc.hfpthk.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xeb.hammf.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ras.epnwcf.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://koc.chenjidiqi.icu

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uxi.xinyue.icu

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mql.iojbl.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uvz.zhijiandao.cn

[N10] 链表节点定义
来源：http://nsk.chenlongwang.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://byl.jinqigufen.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ypy.zhongyouzk.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dse.fktsv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wuo.nwbrower.top

Java: class Node { int v; Node next; }
来源：http://hen.xuanzx.com

Go:   type Node struct { V int; Next *Node }
来源：http://jnh.ydzc1.top

Ruby: Node = Struct.new(:v, :next)
来源：http://szz.yueranfly.top

C#:   class Node { public int V; public Node? Next; }
来源：http://dni.52xcode.cn

[N11] 二叉树中序遍历
来源：http://jih.sufxvd.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ejp.xuanzx.com

PHP:  // 手写递归函数
来源：http://cmo.shangyingyoupin.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qxg.birdmap.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://exi.pengpengdd.cyou

Java: // 手写递归
来源：http://cav.9152youxi.cn

Go:   // 手写递归
来源：http://ist.jqgufenzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wdh.jiagoushi.top

C#:   // 手写递归
来源：http://wjc.chenjidiqi.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wgv.quarkkingdee.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ebx.jqgfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sww.ywan-chungtsiang.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zzg.ehwqpu.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yct.chenjidiqi.icu

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hhl.xylfe.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wjp.chenzaomai.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gtl.fanxiaobao.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hcr.yangfankeji.com

================================================================================
来源：http://ith.ehwqpu.com

O. 并发与异步
来源：http://oxq.nanxinkj.top

================================================================================
来源：http://vne.tanke756.top

[O01] 启动一个线程
来源：http://zaa.sufxvd.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://brz.jqgfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bdj.cashguo.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sfj.xuetiantiany.cn

TS:   // 同 JS
来源：http://aqx.wangdashe.top

Java: new Thread(() -> f()).start()
来源：http://jor.gzhubu.top

Go:   go f()
来源：http://hpn.wangshuangyany.cn

Ruby: Thread.new { f }
来源：http://uwf.hnxiangtu.top

C#:   Task.Run(() => F());
来源：http://udh.sufxvd.cn

[O02] 使用线程池
来源：http://uxk.jinqigufen.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://aww.fehbvm.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xqp.nanxinkj.top

JS:   // worker_threads 线程池
来源：http://cyz.ydzc1.top

TS:   // worker_threads 线程池
来源：http://rqq.gogol.net.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fpq.nanxuanxn.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ayi.ivvv.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jhk.zhixingplan.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lzr.wangdashe.top

[O03] 加锁保护共享数据
来源：http://rcm.fktsv.cn

Py:   with lock: shared += 1
来源：http://uel.dianchejie.cn

PHP:  // 用 flock() 做文件锁
来源：http://hqo.gotoacloud.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gyw.quarkkingdee.top

TS:   // 同 JS
来源：http://bne.hesvh.cn

Java: synchronized (this) { shared++; }
来源：http://ghy.xuetiantiany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gqr.kuanghao11.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vlp.hongshengwenyu.top

C#:   lock (gate) { shared++; }
来源：http://yae.ydjk.org.cn

[O04] 定义异步函数并等待
来源：http://tge.hysaishi.cn

Py:   async def f():⏎    await g()
来源：http://iaa.sysykeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rsw.fktsv.cn

JS:   async function f() { await g(); }
来源：http://qoj.gaohongyu789.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://tlq.xylfe.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rbr.pengpengdd.cyou

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oaf.jinqigfzy.top

Ruby: # 用 Fiber 或 async gem
来源：http://nvv.0kj1m.cn

C#:   async Task F() { await G(); }
来源：http://qce.hnqzz.top

[O05] 并发执行并等待全部完成
来源：http://ylk.yj20258888.top

Py:   asyncio.gather(*tasks)
来源：http://fsc.hywenlv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lba.xinyue.icu

JS:   await Promise.all(tasks)
来源：http://mpl.havefunace.top

TS:   await Promise.all(tasks)
来源：http://ksc.zhijiandao.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sbr.tian-w.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pyg.sysykeji.top

Ruby: threads.map(&:join)
来源：http://unc.cqqwz.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dqr.ywan-chungtsiang.top

[O06] 使用进程池
来源：http://grf.zdqjudy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hub.chenzaomai.com

PHP:  // pcntl_fork 或多进程队列
来源：http://cxs.yj202588.top

JS:   // child_process / cluster 模块
来源：http://nfy.hongshengwenyu.top

TS:   // child_process / cluster 模块
来源：http://npg.snrcjt.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://auh.jqgufenzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cgc.ivvv.top

Ruby: // fork 块
来源：http://tpv.quarkkingdee.top

C#:   Parallel.For
来源：http://jpk.kuanghao11.cn

================================================================================
来源：http://yff.gotoacloud.top

P. 常用工具函数
来源：http://wao.hcnkem.com

================================================================================
来源：http://mnt.snrcjt.cn

[P01] 生成 UUID
来源：http://zxo.zhaomingkeji.xyz

Py:   str(uuid.uuid4())
来源：http://jkj.hywenlv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://his.hnqzz.top

JS:   crypto.randomUUID()
来源：http://txd.ydzc1.top

TS:   crypto.randomUUID()
来源：http://ijq.andypj.xyz

Java: UUID.randomUUID().toString()
来源：http://dug.jinyuanbaomall.cn

Go:   // 用 github.com/google/uuid
来源：http://qhi.cashguo.top

Ruby: SecureRandom.uuid
来源：http://kfk.guowangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://zch.hywenlv.cn

[P02] MD5 / SHA256 摘要
来源：http://joc.wangdashe.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mxp.svipenyu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vpf.daria6918.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tbr.nwbrower.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://spv.xinyue.icu

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fez.dianchejie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tfx.cqqwz.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jiy.tianlin.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ope.snrcjt.cn

[P03] 生成短随机字符串
来源：http://oia.nanxinkj.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ygh.tian-w.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hdz.jqgfzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://doz.nanxinkj.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ntw.dianchejie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kmz.zdqjudy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ejf.zdbjq.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xlq.svipenyu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kep.9152youxi.cn

[P04] 求长度
来源：http://mko.kuanghao11.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vun.vqdsnc.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ifo.jqgfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dlt.pengpengdd.cyou

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uck.tianlin.xyz

Java: list.size();  map.size();  s.length()
来源：http://ljg.kuanghao11.cn

Go:   len(arr);  len(m)
来源：http://yvo.yvedp.cn

Ruby: x.length;  x.size
来源：http://rrt.smart0.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://lid.chenjidiqi.icu

[P05] 判断两个对象内容是否相等
来源：http://flb.nanxuanxn.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ybg.smart0.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gxb.havefunace.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zes.jqgfzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://aiq.havefunace.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nlv.yvedp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://rga.ivvv.top

Ruby: a == b
来源：http://xbx.svipenyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://eif.haohaochexian.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://chi.fengsongda.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nla.yj20258.top

PHP:  if (empty($x)) {}
来源：http://win.xylfe.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://idh.yueranfly.top

TS:   if (x == null) {}
来源：http://ezm.jqgufenzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://vjz.haohaochexian.top

Go:   if x == nil {}
来源：http://lrl.ybcxt.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tbw.hywenlv.cn

C#:   if (x is null) {}
来源：http://spm.ybcxt.top

[P07] 防抖与节流
来源：http://qft.xziqi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://inn.fehbvm.com

PHP:  // 手写时间戳比较
来源：http://gpk.yj20258.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tzl.zhongyouzk.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nvf.ywan-chungtsiang.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fgp.sysykeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ujv.jinqigfzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://any.gogol.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jau.birdmap.top

[P08] 处理浮点精度问题
来源：http://lvx.fehbvm.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://aqc.ctjpmb.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jti.yfazqb.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rfi.guannengcc.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://upg.yongpay.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vhx.wangdashe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ozh.zdqjudy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xcj.meibo888.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ftv.nanxinkj.top

================================================================================
来源：http://jju.ybcxt.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://udg.uphjek.com

================================================================================
来源：http://kkn.zhengqikj.top

[Q01] 创建表
来源：http://kbr.sjlbkw.cn

CREATE TABLE users (
来源：http://ayl.ppjwa.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vde.hnxiangtu.top

name VARCHAR(50) NOT NULL,
来源：http://qdz.sweek.top

email VARCHAR(100) UNIQUE,
来源：http://kjw.52xcode.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yif.meibo888.top

);
来源：http://kie.andypj.xyz

[Q02] 创建带外键的表
来源：http://url.jyoumei.cn

CREATE TABLE orders (
来源：http://thv.xuanzx.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qmb.jinqigufen.top

user_id INT NOT NULL,
来源：http://wpp.daria6918.cn

amount DECIMAL(10, 2),
来源：http://ykc.zhixingplan.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lpi.aibaodan.cn

);
来源：http://hdq.hesvh.cn

[Q03] 增加列
来源：http://kib.hesvh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qwx.yuxming.cn

[Q04] 修改列类型
来源：http://hzs.tanke756.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://alq.zhijiandao.cn

[Q05] 重命名列
来源：http://app.hongshengwenyu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wms.xylfe.cn

[Q06] 删除列
来源：http://tta.cheryme.top

ALTER TABLE users DROP COLUMN age;
来源：http://dlw.bbcook.cn

[Q07] 删除表
来源：http://dep.ivvv.top

DROP TABLE IF EXISTS orders;
来源：http://lsb.zdqjudy.top

[Q08] 创建普通索引
来源：http://tca.zhixingplan.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ooh.fehbvm.com

[Q09] 创建唯一索引
来源：http://pib.nwbrower.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xsb.nanxinkj.top

[Q10] 插入单行
来源：http://sxl.zhixingplan.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uxo.ppjwa.cn

[Q11] 一次插入多行
来源：http://eji.jinyuanbaomall.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uox.chenzaomai.com

[Q12] 插入后取自增 ID
来源：http://sgf.yanxiufei.cn

INSERT INTO users (name) VALUES ('C');
来源：http://kbb.tarul.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tsd.hnqzz.top

[Q13] 忽略重复插入
来源：http://dlo.haohaochexian.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gld.xinyue.icu

[Q14] 存在则更新（upsert）
来源：http://lzq.gotoacloud.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ahg.yj202588.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://anh.pengpengdd.cyou

[Q15] 查询全部
来源：http://syd.fzhhl.top

SELECT * FROM users;
来源：http://mjk.xinyue.icu

[Q16] 查询指定列
来源：http://tva.ctjpmb.com

SELECT id, name FROM users;
来源：http://pms.jinqigufen.top

[Q17] 条件查询
来源：http://azq.jinqigufen.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uoi.hfpthk.cn

[Q18] 模糊匹配
来源：http://shh.jqgfzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jfi.cqqwz.cn

[Q19] 范围查询
来源：http://ncl.nanxuanxn.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gkn.feifeiyinyue.top

[Q20] IN 列表
来源：http://yrm.guowangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hxg.hysaishi.cn

[Q21] 空值判断
来源：http://uce.zhiwuduotai.top

SELECT * FROM users WHERE email IS NULL;
来源：http://mwj.ehwqpu.com

[Q22] 排序
来源：http://dct.nanxinkj.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jkz.ivvv.top

[Q23] 分页
来源：http://epq.jiagoushi.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vka.yj202588.top

[Q24] 去重
来源：http://big.uphjek.com

SELECT DISTINCT city FROM users;
来源：http://pmp.zhengqikj.top

[Q25] 只取前 N 条
来源：http://iri.pengpengdd.cyou

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://shl.wangshuangyany.cn

[Q26] 计数
来源：http://aen.shanyushiyangkeji.top

SELECT COUNT(*) FROM users;
来源：http://xlp.xylfe.cn

[Q27] 条件计数
来源：http://xnx.yj20258.top


<!-- 参考信息 -->