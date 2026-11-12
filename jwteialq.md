代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xtj.xziqi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ojv.daxiang520.top

Go:   sort.SearchInts(arr, x)
来源：http://qib.ehwqpu.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://ntg.0kj1m.cn

C#:   Array.BinarySearch(arr, x)
来源：http://urk.jinqigfzy.top

[N02] 排序（工程实践用内置实现）
来源：http://rxt.gogol.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://ujs.hammf.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rkb.xuetiantiany.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gxc.meibo888.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://cjc.bbcook.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bta.fehbvm.com

Go:   slices.Sort(arr)
来源：http://wmo.cheryme.top

Ruby: arr.sort
来源：http://vbb.aizwys.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://box.wangdashe.top

[N03] 快速排序（分治示例）
来源：http://bih.jlsjyb.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://djb.jlsjyb.cn

PHP:  // 递归实现，或用 usort
来源：http://tvx.ydjk.org.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zvu.kuanghao11.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vng.jinqigfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hmg.jinqigufen.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hne.nwbrower.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ivg.jiagoushi.top

C#:   // 手写递归，或 Array.Sort
来源：http://veq.jqgufenzy.top

[N04] 斐波那契数列
来源：http://jis.wangdashe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mnk.yueranfly.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ada.hesvh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xwv.xingfuxueyuan.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eyp.quarkkingdee.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dor.jianghu66.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://usl.aizwys.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yde.yj20258.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ney.zhiwuduotai.top

[N05] 最大公约数
来源：http://ctk.redwolf501.top

Py:   math.gcd(a, b)
来源：http://vxu.hammf.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gvt.ctjpmb.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gjk.yueranfly.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pnc.yongpay.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ond.yanxiufei.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://myw.chenjidiqi.icu

Ruby: a.gcd(b)
来源：http://zjp.zdbjq.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uhy.sjlbkw.cn

[N06] 判断回文字符串
来源：http://ias.yueranfly.top

Py:   s == s[::-1]
来源：http://mnm.hysaishi.cn

PHP:  $s === strrev($s);
来源：http://gxz.bjfxy.top

JS:   s === [...s].reverse().join("")
来源：http://tqm.feifeiyinyue.top

TS:   s === [...s].reverse().join("")
来源：http://ngo.chenjidiqi.icu

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jhx.redwolf501.top

Go:   // 双指针从两端比较
来源：http://qij.jiagoushi.top

Ruby: s == s.reverse
来源：http://acw.yueranfly.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ixd.pengpengdd.cyou

[N07] 两数之和（返回下标）
来源：http://zbr.jinqigfzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jvs.aibaodan.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bvd.xingfuxueyuan.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://kle.c1oappe.top

TS:   // 手写 Map<string, number>
来源：http://tcn.bbcook.cn

Java: // 手写 HashMap
来源：http://ong.52xcode.cn

Go:   // 手写 map[int]int
来源：http://hvu.uphjek.com

Ruby: // 手写 Hash
来源：http://wna.pycfn.com

C#:   // 手写 Dictionary<int, int>
来源：http://isl.pengpengdd.cyou

[N08] 生成全排列
来源：http://odx.hysaishi.cn

Py:   itertools.permutations(arr)
来源：http://tjh.yanxiufei.cn

PHP:  // 手写递归交换
来源：http://ugf.ctjpmb.com

JS:   // 手写回溯递归
来源：http://jyy.xuetiantiany.cn

TS:   // 手写回溯递归
来源：http://pci.daxiang520.top

Java: // 手写回溯递归
来源：http://qxw.yuanzhike.top

Go:   // 手写回溯递归
来源：http://lqg.ywan-chungtsiang.top

Ruby: arr.permutation.to_a
来源：http://ysc.fanxiaobao.xyz

C#:   // 手写回溯递归
来源：http://uue.gaohongyu789.top

[N09] 栈与队列
来源：http://dnb.ppjwa.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nog.hesvh.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://auw.fzhhl.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gib.xuanzx.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qjm.cheryme.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tpu.jyoumei.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gsw.nanxuanxn.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tau.hnqzz.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kgb.zycfv.cn

[N10] 链表节点定义
来源：http://ujr.hcnkem.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mlr.yuxming.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dan.yvedp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zlw.quarkkingdee.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rnw.chenzaomai.com

Java: class Node { int v; Node next; }
来源：http://jgv.nanxinkj.top

Go:   type Node struct { V int; Next *Node }
来源：http://zxf.jlsjyb.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rsj.shzxlz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jug.tianlin.xyz

[N11] 二叉树中序遍历
来源：http://coh.kuanghao11.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hlo.bbcook.cn

PHP:  // 手写递归函数
来源：http://zrm.yonumen.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xcm.hywenlv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wwu.xziqi.cn

Java: // 手写递归
来源：http://ogf.zhongyouzk.top

Go:   // 手写递归
来源：http://ayw.jinghuilouyu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vrh.zhengqikj.top

C#:   // 手写递归
来源：http://jhu.jinyuanbaomall.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yjh.yj20258888.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rhu.dashuyun.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vqt.sxryk.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mff.havefunace.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ikn.yuxming.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yth.meibo888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yuj.zdqjudy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ufy.xylfe.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vhh.0kj1m.cn

================================================================================
来源：http://pdq.yongpay.top

O. 并发与异步
来源：http://ots.dashuyun.cn

================================================================================
来源：http://eeb.shanyushiyangtech.top

[O01] 启动一个线程
来源：http://zfi.cheryme.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://maj.ppjwa.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nvu.chenzaomai.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fim.jianghu66.top

TS:   // 同 JS
来源：http://ebj.zhengqikj.top

Java: new Thread(() -> f()).start()
来源：http://kpz.zhijiandao.cn

Go:   go f()
来源：http://hqc.cashguo.top

Ruby: Thread.new { f }
来源：http://cfs.guowangkeji.top

C#:   Task.Run(() => F());
来源：http://mov.wangdashe.top

[O02] 使用线程池
来源：http://lnp.hcnkem.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://iln.jinqigfzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ykl.yangfankeji.com

JS:   // worker_threads 线程池
来源：http://pjm.havefunace.top

TS:   // worker_threads 线程池
来源：http://vox.jinqigfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://nhi.yuxming.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hns.ydjk.org.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baz.zhongyouzk.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cdl.fktsv.cn

[O03] 加锁保护共享数据
来源：http://loe.pycfn.com

Py:   with lock: shared += 1
来源：http://typ.wangshuangyany.cn

PHP:  // 用 flock() 做文件锁
来源：http://mlx.xziqi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mih.zhaomingkeji.xyz

TS:   // 同 JS
来源：http://sbt.jqgufenzy.top

Java: synchronized (this) { shared++; }
来源：http://tkn.fktsv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xxh.316326.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://ola.svipenyu.cn

C#:   lock (gate) { shared++; }
来源：http://sqs.chenlongwang.top

[O04] 定义异步函数并等待
来源：http://vmo.redwolf501.top

Py:   async def f():⏎    await g()
来源：http://nzh.zhaomingkeji.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://izd.quarkkingdee.top

JS:   async function f() { await g(); }
来源：http://uow.chenjidiqi.icu

TS:   async function f(): Promise<void> { await g(); }
来源：http://bej.fzhhl.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gmu.xuetiantiany.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tvs.epnwcf.com

Ruby: # 用 Fiber 或 async gem
来源：http://noy.jinyuanbaomall.cn

C#:   async Task F() { await G(); }
来源：http://oid.smart0.xyz

[O05] 并发执行并等待全部完成
来源：http://ybg.xuetiantiany.cn

Py:   asyncio.gather(*tasks)
来源：http://izu.birdmap.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zqv.hnxiangtu.top

JS:   await Promise.all(tasks)
来源：http://uog.ehwqpu.com

TS:   await Promise.all(tasks)
来源：http://zki.zhixingplan.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uqq.yj202588.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bmg.fehbvm.com

Ruby: threads.map(&:join)
来源：http://iti.uphjek.com

C#:   await Task.WhenAll(t1, t2)
来源：http://knh.jlsjyb.cn

[O06] 使用进程池
来源：http://bba.meibo888.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ism.cdnleiting.top

PHP:  // pcntl_fork 或多进程队列
来源：http://llk.birdmap.top

JS:   // child_process / cluster 模块
来源：http://aau.meibo888.top

TS:   // child_process / cluster 模块
来源：http://tqu.epnwcf.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ogp.birdmap.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dbp.sxryk.cn

Ruby: // fork 块
来源：http://fqu.hnxiangtu.top

C#:   Parallel.For
来源：http://pqz.ywan-chungtsiang.top

================================================================================
来源：http://qqb.ydjk.org.cn

P. 常用工具函数
来源：http://xhp.zdqjudy.top

================================================================================
来源：http://xpe.yfazqb.com

[P01] 生成 UUID
来源：http://dnb.yanxiufei.cn

Py:   str(uuid.uuid4())
来源：http://tck.hcnkem.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://evj.iojbl.cn

JS:   crypto.randomUUID()
来源：http://usy.tianlin.xyz

TS:   crypto.randomUUID()
来源：http://zed.tian-w.cn

Java: UUID.randomUUID().toString()
来源：http://gdc.pengpengdd.cyou

Go:   // 用 github.com/google/uuid
来源：http://wgz.pycfn.com

Ruby: SecureRandom.uuid
来源：http://sea.sjlbkw.cn

C#:   Guid.NewGuid().ToString()
来源：http://fnt.jqgfzy.top

[P02] MD5 / SHA256 摘要
来源：http://fgd.yueranfly.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mzr.wangshuangyany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://iue.tanke756.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xkw.wangshuangyany.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gji.yonumen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vlz.zhiwuduotai.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gex.52xcode.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://eos.mhx1999.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sgy.redwolf501.top

[P03] 生成短随机字符串
来源：http://kbt.0kj1m.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bny.shangyingyoupin.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wty.hammf.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jmy.daxiang520.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gvq.epnwcf.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pbk.wangshuangyany.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gpk.0kj1m.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hqa.cucudq.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://unf.hongshengwenyu.top

[P04] 求长度
来源：http://xms.jinqigufen.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jxe.tian-w.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ycr.smart0.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ihx.meibo888.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://utc.ctjpmb.com

Java: list.size();  map.size();  s.length()
来源：http://mte.guowangkeji.top

Go:   len(arr);  len(m)
来源：http://xqc.yangfankeji.com

Ruby: x.length;  x.size
来源：http://prg.52xcode.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://dpo.yj20258888.top

[P05] 判断两个对象内容是否相等
来源：http://jbk.hysaishi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xqj.cheryme.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jka.chenzaomai.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kuv.yfazqb.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pky.dianchejie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tln.jyoumei.cn

Go:   reflect.DeepEqual(a, b)
来源：http://uls.jyoumei.cn

Ruby: a == b
来源：http://wlo.yvedp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vek.sweek.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kbl.sjlbkw.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tma.sufxvd.cn

PHP:  if (empty($x)) {}
来源：http://hje.hammf.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fhv.yanxiufei.cn

TS:   if (x == null) {}
来源：http://ilz.yj20258.top

Java: if (x == null || x.isEmpty()) {}
来源：http://zaz.smart0.xyz

Go:   if x == nil {}
来源：http://shm.xziqi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qkn.ydzc1.top

C#:   if (x is null) {}
来源：http://ucf.quarkkingdee.top

[P07] 防抖与节流
来源：http://zls.fanxiaobao.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://chg.cdnleiting.top

PHP:  // 手写时间戳比较
来源：http://pdk.jqgfzy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cgn.zhiwuduotai.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mjb.ydzc1.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pux.gzhubu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ger.316326.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://aii.hammf.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ihr.dashuyun.cn

[P08] 处理浮点精度问题
来源：http://yub.cucudq.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ogr.hongshengwenyu.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jas.gaohongyu789.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://eqq.guowangkeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ujj.yuanzhike.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gcz.gotoacloud.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://boc.yfazqb.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cgv.yvedp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jbx.yj20258.top

================================================================================
来源：http://jvk.iojbl.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kuh.zhixingplan.top

================================================================================
来源：http://hhj.sysykeji.top

[Q01] 创建表
来源：http://xov.52xcode.cn

CREATE TABLE users (
来源：http://afg.daxiang520.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://edy.sysykeji.top

name VARCHAR(50) NOT NULL,
来源：http://uao.vehdjk.com

email VARCHAR(100) UNIQUE,
来源：http://rlg.yueranfly.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sfo.hfpthk.cn

);
来源：http://wja.pengpengdd.cyou

[Q02] 创建带外键的表
来源：http://sso.kuanghao11.cn

CREATE TABLE orders (
来源：http://jus.zhiwuduotai.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fzx.chenlongwang.top

user_id INT NOT NULL,
来源：http://noq.ybcxt.top

amount DECIMAL(10, 2),
来源：http://vke.ivvv.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xmw.sysykeji.top

);
来源：http://ene.shzxlz.cn

[Q03] 增加列
来源：http://pkx.c1oappe.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fcv.gzhubu.top

[Q04] 修改列类型
来源：http://tui.sufxvd.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://aus.ehwqpu.com

[Q05] 重命名列
来源：http://pwb.daxiang520.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://khl.chenjidiqi.icu

[Q06] 删除列
来源：http://iei.shuidangran.top

ALTER TABLE users DROP COLUMN age;
来源：http://xey.dashuyun.cn

[Q07] 删除表
来源：http://car.dashuyun.cn

DROP TABLE IF EXISTS orders;
来源：http://dov.haohaochexian.top

[Q08] 创建普通索引
来源：http://ndq.yuanzhike.top

CREATE INDEX idx_users_email ON users(email);
来源：http://hss.zdbjq.cn

[Q09] 创建唯一索引
来源：http://awd.daria6918.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nxb.guannengcc.top

[Q10] 插入单行
来源：http://drm.yj20258888.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jbv.dashuyun.cn

[Q11] 一次插入多行
来源：http://vsr.haohaochexian.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rqa.zycfv.cn

[Q12] 插入后取自增 ID
来源：http://luy.shzxlz.cn

INSERT INTO users (name) VALUES ('C');
来源：http://zcu.hesvh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wzy.xylfe.cn

[Q13] 忽略重复插入
来源：http://jbw.jiagoushi.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ojt.redwolf501.top

[Q14] 存在则更新（upsert）
来源：http://vpe.vehdjk.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rym.fanxiaobao.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qcf.jyoumei.cn

[Q15] 查询全部
来源：http://ppf.9152youxi.cn

SELECT * FROM users;
来源：http://ril.dashuyun.cn

[Q16] 查询指定列
来源：http://llr.fktsv.cn

SELECT id, name FROM users;
来源：http://moq.meibo888.top

[Q17] 条件查询
来源：http://ipo.cashguo.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://skc.ydjk.org.cn

[Q18] 模糊匹配
来源：http://ens.316326.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ofs.cheryme.top

[Q19] 范围查询
来源：http://gup.fehbvm.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wds.yonumen.top

[Q20] IN 列表
来源：http://apn.zhongyouzk.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://haj.yongpay.top

[Q21] 空值判断
来源：http://eoj.jqgufenzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ebj.ydjk.org.cn

[Q22] 排序
来源：http://grt.svipenyu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ggv.tanke756.top

[Q23] 分页
来源：http://hpm.nanxuanxn.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://iik.kuanghao11.cn

[Q24] 去重
来源：http://lij.smart0.xyz

SELECT DISTINCT city FROM users;
来源：http://cct.shanyushiyangtech.top

[Q25] 只取前 N 条
来源：http://lcc.fanxiaobao.xyz


<!-- 参考信息 -->