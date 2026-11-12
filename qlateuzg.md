代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://mrh.zycfv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sdm.zhijiandao.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pbt.zhiwuduotai.top

Go:   slices.Sort(arr)
来源：http://amv.xziqi.cn

Ruby: arr.sort
来源：http://gof.snrcjt.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mml.yonumen.top

[N03] 快速排序（分治示例）
来源：http://hcn.0kj1m.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ngt.cdnleiting.top

PHP:  // 递归实现，或用 usort
来源：http://lqt.dashuyun.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cbo.yanxiufei.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tic.guowangkeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://iec.snrcjt.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://omo.zycfv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rik.ybcxt.top

C#:   // 手写递归，或 Array.Sort
来源：http://fng.vqdsnc.cn

[N04] 斐波那契数列
来源：http://irs.yonumen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tgl.c1oappe.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ywm.tarul.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sia.dianchejie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jcz.feifeiyinyue.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mgb.uphjek.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dzj.zdbjq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mot.chenlongwang.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hbr.fanxiaobao.xyz

[N05] 最大公约数
来源：http://rix.feifeiyinyue.top

Py:   math.gcd(a, b)
来源：http://jot.svipenyu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fml.vqdsnc.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://woc.zdqjudy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yku.ivvv.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rir.ydjk.org.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wmy.andypj.xyz

Ruby: a.gcd(b)
来源：http://csn.xuanzx.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dbq.daxiang520.top

[N06] 判断回文字符串
来源：http://uny.jianghu66.top

Py:   s == s[::-1]
来源：http://loa.zhaomingkeji.xyz

PHP:  $s === strrev($s);
来源：http://xhq.tianlin.xyz

JS:   s === [...s].reverse().join("")
来源：http://nan.xuanzx.com

TS:   s === [...s].reverse().join("")
来源：http://zkl.zhijiandao.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jpl.jinqigufen.top

Go:   // 双指针从两端比较
来源：http://lgt.fzhhl.top

Ruby: s == s.reverse
来源：http://upn.guannengcc.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jma.yanxiufei.cn

[N07] 两数之和（返回下标）
来源：http://nly.zhengqikj.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qqx.andypj.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yow.zhengqikj.top

JS:   // 手写 Map：map.set(v, i)
来源：http://zss.jinqigufen.top

TS:   // 手写 Map<string, number>
来源：http://cip.yuxming.cn

Java: // 手写 HashMap
来源：http://ehz.zdqjudy.top

Go:   // 手写 map[int]int
来源：http://rlc.yj20258.top

Ruby: // 手写 Hash
来源：http://lrr.snrcjt.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wbj.zhoulong.xyz

[N08] 生成全排列
来源：http://asp.redwolf501.top

Py:   itertools.permutations(arr)
来源：http://ugq.sysykeji.top

PHP:  // 手写递归交换
来源：http://wks.zdqjudy.top

JS:   // 手写回溯递归
来源：http://jqr.jinqigufen.top

TS:   // 手写回溯递归
来源：http://rbj.jinyuanbaomall.cn

Java: // 手写回溯递归
来源：http://igu.fzhhl.top

Go:   // 手写回溯递归
来源：http://pyq.feifeiyinyue.top

Ruby: arr.permutation.to_a
来源：http://hcr.zhengqikj.top

C#:   // 手写回溯递归
来源：http://tee.fanxiaobao.xyz

[N09] 栈与队列
来源：http://afa.shuidangran.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cyd.yongpay.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://igm.cashguo.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://aat.yuxming.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mri.cashguo.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wjj.yongpay.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xot.jinghuilouyu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wfl.xingfuxueyuan.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tqa.cheryme.top

[N10] 链表节点定义
来源：http://hlx.yangfankeji.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://msj.smart0.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://wxi.zhaomingkeji.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://isx.cucudq.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qkz.52xcode.cn

Java: class Node { int v; Node next; }
来源：http://ity.wangshuangyany.cn

Go:   type Node struct { V int; Next *Node }
来源：http://kmq.gogol.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://liv.svipenyu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hwo.tarul.cn

[N11] 二叉树中序遍历
来源：http://fmv.jyoumei.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hwp.cashguo.top

PHP:  // 手写递归函数
来源：http://xgu.dianchejie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tam.sxryk.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lgy.tian-w.cn

Java: // 手写递归
来源：http://xae.kuanghao11.cn

Go:   // 手写递归
来源：http://upq.jinqigfzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oju.yongpay.top

C#:   // 手写递归
来源：http://tnv.bjfxy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dwn.jqgufenzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zac.sysykeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dwn.guannengcc.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bff.sjlbkw.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cwi.jqgufenzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yip.sxryk.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zgq.cheryme.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zuh.ivvv.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xuw.zhengqikj.top

================================================================================
来源：http://ihc.ppjwa.cn

O. 并发与异步
来源：http://xix.xuetiantiany.cn

================================================================================
来源：http://lhp.wangdashe.top

[O01] 启动一个线程
来源：http://acq.kuanghao11.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rwa.smart0.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dwq.snrcjt.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ypp.bjfxy.top

TS:   // 同 JS
来源：http://frk.gzhubu.top

Java: new Thread(() -> f()).start()
来源：http://uni.sysykeji.top

Go:   go f()
来源：http://laq.yj20258888.top

Ruby: Thread.new { f }
来源：http://zzi.yonumen.top

C#:   Task.Run(() => F());
来源：http://eii.fzhhl.top

[O02] 使用线程池
来源：http://pte.zhiwuduotai.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eyn.guowangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://brk.fehbvm.com

JS:   // worker_threads 线程池
来源：http://beq.pycfn.com

TS:   // worker_threads 线程池
来源：http://jeu.dashuyun.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bvc.sufxvd.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hbz.zhaomingkeji.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pwm.aizwys.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uff.quarkkingdee.top

[O03] 加锁保护共享数据
来源：http://xgr.bbcook.cn

Py:   with lock: shared += 1
来源：http://fco.zdbjq.cn

PHP:  // 用 flock() 做文件锁
来源：http://xfc.daxiang520.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lcy.cdnleiting.top

TS:   // 同 JS
来源：http://lok.316326.xyz

Java: synchronized (this) { shared++; }
来源：http://dmg.shanyushiyangtech.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pph.c1oappe.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://jcy.pengpengdd.cyou

C#:   lock (gate) { shared++; }
来源：http://pjb.yvedp.cn

[O04] 定义异步函数并等待
来源：http://uyz.yuxming.cn

Py:   async def f():⏎    await g()
来源：http://lyz.jinghuilouyu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://beb.zycfv.cn

JS:   async function f() { await g(); }
来源：http://iqy.ybcxt.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://foy.dashuyun.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pdl.birdmap.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bpg.tianlin.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://ttn.wangdashe.top

C#:   async Task F() { await G(); }
来源：http://jqw.yongpay.top

[O05] 并发执行并等待全部完成
来源：http://ocn.feifeiyinyue.top

Py:   asyncio.gather(*tasks)
来源：http://qsj.ybcxt.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yzr.guowangkeji.top

JS:   await Promise.all(tasks)
来源：http://stl.hnqzz.top

TS:   await Promise.all(tasks)
来源：http://hpl.meibo888.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://luj.yuxming.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mgi.xinyue.icu

Ruby: threads.map(&:join)
来源：http://ptu.xylfe.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cpc.zhengqikj.top

[O06] 使用进程池
来源：http://ncr.aizwys.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://txu.yuanzhike.top

PHP:  // pcntl_fork 或多进程队列
来源：http://dcj.sjlbkw.cn

JS:   // child_process / cluster 模块
来源：http://dwl.yvedp.cn

TS:   // child_process / cluster 模块
来源：http://wsf.zhaomingkeji.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mlp.hesvh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lxn.bbcook.cn

Ruby: // fork 块
来源：http://dxi.xinyue.icu

C#:   Parallel.For
来源：http://hcv.vehdjk.com

================================================================================
来源：http://juy.cheryme.top

P. 常用工具函数
来源：http://nqh.zdbjq.cn

================================================================================
来源：http://pga.zhixingplan.top

[P01] 生成 UUID
来源：http://ral.9152youxi.cn

Py:   str(uuid.uuid4())
来源：http://uod.fzhhl.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fzw.yfazqb.com

JS:   crypto.randomUUID()
来源：http://ciq.guannengcc.top

TS:   crypto.randomUUID()
来源：http://sfx.dashuyun.cn

Java: UUID.randomUUID().toString()
来源：http://nya.c1oappe.top

Go:   // 用 github.com/google/uuid
来源：http://xcb.jinqigfzy.top

Ruby: SecureRandom.uuid
来源：http://krv.zhengqikj.top

C#:   Guid.NewGuid().ToString()
来源：http://zli.zhiwuduotai.top

[P02] MD5 / SHA256 摘要
来源：http://rxt.hesvh.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nlx.zhongyouzk.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://kgy.hcnkem.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qed.svipenyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ngt.svipenyu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yws.zhijiandao.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zyg.sweek.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ofl.gzhubu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://swz.tian-w.cn

[P03] 生成短随机字符串
来源：http://rpn.tian-w.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vvw.vehdjk.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ghj.xinyue.icu

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wib.zhaomingkeji.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vow.jinqigfzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ovz.zhijiandao.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hsl.zhongyouzk.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://xdd.yonumen.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://itn.quarkkingdee.top

[P04] 求长度
来源：http://lxs.yangfankeji.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nyl.xziqi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xjz.shzxlz.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://djk.kuanghao11.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gne.zdbjq.cn

Java: list.size();  map.size();  s.length()
来源：http://mel.aibaodan.cn

Go:   len(arr);  len(m)
来源：http://myp.yanxiufei.cn

Ruby: x.length;  x.size
来源：http://vaq.uphjek.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://bds.fktsv.cn

[P05] 判断两个对象内容是否相等
来源：http://tvh.yonumen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ovu.zhijiandao.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mvf.yueranfly.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fgp.aibaodan.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mop.aizwys.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://okn.gotoacloud.top

Go:   reflect.DeepEqual(a, b)
来源：http://yhb.zhongyouzk.top

Ruby: a == b
来源：http://gnu.zhiwuduotai.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://msm.sjlbkw.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wmx.gzhubu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fnc.zhiwuduotai.top

PHP:  if (empty($x)) {}
来源：http://utw.andypj.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xov.cheryme.top

TS:   if (x == null) {}
来源：http://twu.daria6918.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://qhg.hywenlv.cn

Go:   if x == nil {}
来源：http://ipf.xylfe.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://frx.chenjidiqi.icu

C#:   if (x is null) {}
来源：http://rij.shangyingyoupin.top

[P07] 防抖与节流
来源：http://brg.zhongyouzk.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rpd.dianchejie.cn

PHP:  // 手写时间戳比较
来源：http://fvb.yonumen.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bjb.gotoacloud.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bzh.xinyue.icu

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://flj.gotoacloud.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fgt.sxryk.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xnr.jinyuanbaomall.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kth.jinqigufen.top

[P08] 处理浮点精度问题
来源：http://ivb.guowangkeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mrc.yanxiufei.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qsl.jiagoushi.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wfv.kuanghao11.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://aje.nwbrower.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://npn.fanxiaobao.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ybm.ppjwa.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hxc.jqgufenzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wkx.yj20258.top

================================================================================
来源：http://vkd.jiagoushi.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sch.yvedp.cn

================================================================================
来源：http://czm.shanyushiyangtech.top

[Q01] 创建表
来源：http://rwm.birdmap.top

CREATE TABLE users (
来源：http://fki.zycfv.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://emf.9152youxi.cn

name VARCHAR(50) NOT NULL,
来源：http://sxq.ivvv.top

email VARCHAR(100) UNIQUE,
来源：http://wdv.zhengqikj.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xgs.tanke756.top

);
来源：http://ihs.hysaishi.cn

[Q02] 创建带外键的表
来源：http://ako.ywan-chungtsiang.top

CREATE TABLE orders (
来源：http://uny.hnqzz.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vfd.zhaomingkeji.xyz

user_id INT NOT NULL,
来源：http://iba.chenzaomai.com

amount DECIMAL(10, 2),
来源：http://gqr.bjfxy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fvs.yj20258.top

);
来源：http://rlg.tian-w.cn

[Q03] 增加列
来源：http://asx.nwbrower.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nqt.9152youxi.cn

[Q04] 修改列类型
来源：http://vrn.hfpthk.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jpe.zhongyouzk.top

[Q05] 重命名列
来源：http://bta.sjlbkw.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dvr.yanxiufei.cn

[Q06] 删除列
来源：http://rmr.hcnkem.com

ALTER TABLE users DROP COLUMN age;
来源：http://ppj.tarul.cn

[Q07] 删除表
来源：http://var.wangdashe.top

DROP TABLE IF EXISTS orders;
来源：http://phf.fzhhl.top

[Q08] 创建普通索引
来源：http://mjx.sxryk.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ida.redwolf501.top

[Q09] 创建唯一索引
来源：http://uzf.ydzc1.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://euk.zhijiandao.cn

[Q10] 插入单行
来源：http://ijm.gaohongyu789.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yfh.fehbvm.com

[Q11] 一次插入多行
来源：http://fzs.nanxuanxn.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bia.ppjwa.cn

[Q12] 插入后取自增 ID
来源：http://rff.hnqzz.top

INSERT INTO users (name) VALUES ('C');
来源：http://ril.sweek.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xln.zhijiandao.cn

[Q13] 忽略重复插入
来源：http://qsg.ydzc1.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xuy.jinqigufen.top

[Q14] 存在则更新（upsert）
来源：http://sds.zhongyouzk.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sag.ctjpmb.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://abp.tanke756.top

[Q15] 查询全部
来源：http://gkk.hcnkem.com

SELECT * FROM users;
来源：http://zdf.havefunace.top

[Q16] 查询指定列
来源：http://dpm.sysykeji.top

SELECT id, name FROM users;
来源：http://nes.zycfv.cn

[Q17] 条件查询
来源：http://rnh.snrcjt.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qhf.gaohongyu789.top

[Q18] 模糊匹配
来源：http://izr.gzhubu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://taw.andypj.xyz

[Q19] 范围查询
来源：http://zyn.ybcxt.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xbo.zhiwuduotai.top

[Q20] IN 列表
来源：http://whx.smart0.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://acy.gzhubu.top

[Q21] 空值判断
来源：http://ibt.xuanzx.com

SELECT * FROM users WHERE email IS NULL;
来源：http://ggh.hammf.cn

[Q22] 排序
来源：http://gjc.cucudq.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uni.yj20258.top

[Q23] 分页
来源：http://nih.gotoacloud.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lgp.bbcook.cn

[Q24] 去重
来源：http://meo.zhixingplan.top

SELECT DISTINCT city FROM users;
来源：http://nyp.nanxinkj.top

[Q25] 只取前 N 条
来源：http://sob.cdnleiting.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ydf.zycfv.cn

[Q26] 计数
来源：http://etr.redwolf501.top

SELECT COUNT(*) FROM users;
来源：http://faz.xuanzx.com

[Q27] 条件计数
来源：http://dvf.jyoumei.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://atg.snrcjt.cn

[Q28] 求和与平均
来源：http://pxf.zhiwuduotai.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mnr.xuetiantiany.cn

[Q29] 最大最小值
来源：http://aej.jinghuilouyu.cn


<!-- 参考信息 -->