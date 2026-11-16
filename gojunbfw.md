代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://lnl.jinyuanbaomall.cn

[N02] 排序（工程实践用内置实现）
来源：http://mxt.xziqi.cn

Py:   sorted(arr);  arr.sort()
来源：http://bid.nanxinkj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wfi.gaohongyu789.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://idk.ctjpmb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://gqh.svipenyu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kvr.aizwys.cn

Go:   slices.Sort(arr)
来源：http://zqr.tianlin.xyz

Ruby: arr.sort
来源：http://ttg.fengsongda.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xci.yueranfly.top

[N03] 快速排序（分治示例）
来源：http://bao.hesvh.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fmw.9152youxi.cn

PHP:  // 递归实现，或用 usort
来源：http://xpz.mhx1999.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lzx.feifeiyinyue.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mwl.yuanzhike.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ynq.gzhubu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jyi.tian-w.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kva.yj20258.top

C#:   // 手写递归，或 Array.Sort
来源：http://zcr.hysaishi.cn

[N04] 斐波那契数列
来源：http://lxo.zhaomingkeji.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://eex.andypj.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cfq.yj20258.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cgq.tanke756.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cla.zhongyouzk.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yoo.nanxinkj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gkl.sufxvd.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qnq.cheryme.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kxi.jianghu66.top

[N05] 最大公约数
来源：http://jxn.aibaodan.cn

Py:   math.gcd(a, b)
来源：http://sxx.yueranfly.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vlm.tian-w.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ous.fehbvm.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rff.hesvh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nbk.yongpay.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rlz.quarkkingdee.top

Ruby: a.gcd(b)
来源：http://zpi.yfazqb.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://knr.gzhubu.top

[N06] 判断回文字符串
来源：http://krn.52xcode.cn

Py:   s == s[::-1]
来源：http://mpq.guowangkeji.top

PHP:  $s === strrev($s);
来源：http://pcs.zhiwuduotai.top

JS:   s === [...s].reverse().join("")
来源：http://pni.redwolf501.top

TS:   s === [...s].reverse().join("")
来源：http://fus.ydjk.org.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oyu.zhoulong.xyz

Go:   // 双指针从两端比较
来源：http://nrh.ivvv.top

Ruby: s == s.reverse
来源：http://qnl.birdmap.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://cco.hywenlv.cn

[N07] 两数之和（返回下标）
来源：http://nmm.jinqigfzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://afg.sweek.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dhh.jqgfzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ezq.vehdjk.com

TS:   // 手写 Map<string, number>
来源：http://ioc.jqgufenzy.top

Java: // 手写 HashMap
来源：http://fyo.birdmap.top

Go:   // 手写 map[int]int
来源：http://kta.aizwys.cn

Ruby: // 手写 Hash
来源：http://pdu.nwbrower.top

C#:   // 手写 Dictionary<int, int>
来源：http://utm.shanyushiyangtech.top

[N08] 生成全排列
来源：http://etm.zdbjq.cn

Py:   itertools.permutations(arr)
来源：http://vbz.bbcook.cn

PHP:  // 手写递归交换
来源：http://xwy.ivvv.top

JS:   // 手写回溯递归
来源：http://asx.yanxiufei.cn

TS:   // 手写回溯递归
来源：http://sva.jinqigfzy.top

Java: // 手写回溯递归
来源：http://tij.yj20258888.top

Go:   // 手写回溯递归
来源：http://kwl.cqqwz.cn

Ruby: arr.permutation.to_a
来源：http://xcv.cdnleiting.top

C#:   // 手写回溯递归
来源：http://jft.zhaomingkeji.xyz

[N09] 栈与队列
来源：http://ljd.ivvv.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xct.yanxiufei.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wyy.hywenlv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lmz.sysykeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://exu.yanxiufei.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://myj.ppjwa.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wyd.jinqigufen.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pzf.jinghuilouyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://owr.shanyushiyangtech.top

[N10] 链表节点定义
来源：http://awu.tarul.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tbs.iojbl.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kzm.shangyingyoupin.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nlz.hysaishi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://czt.redwolf501.top

Java: class Node { int v; Node next; }
来源：http://gkz.zhiwuduotai.top

Go:   type Node struct { V int; Next *Node }
来源：http://lqj.bjfxy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://lrn.yuanzhike.top

C#:   class Node { public int V; public Node? Next; }
来源：http://hei.dashuyun.cn

[N11] 二叉树中序遍历
来源：http://tli.cdnleiting.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mao.yuanzhike.top

PHP:  // 手写递归函数
来源：http://jog.gogol.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iya.haohaochexian.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bgr.yanxiufei.cn

Java: // 手写递归
来源：http://thh.xylfe.cn

Go:   // 手写递归
来源：http://ftm.gzhubu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ley.quarkkingdee.top

C#:   // 手写递归
来源：http://axf.52xcode.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uin.ehwqpu.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gtb.nanxuanxn.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://whs.haohaochexian.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pwl.ydzc1.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://prv.xziqi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cnj.hnqzz.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yel.ehwqpu.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jiv.zhiwuduotai.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hib.zdbjq.cn

================================================================================
来源：http://czz.tian-w.cn

O. 并发与异步
来源：http://tim.redwolf501.top

================================================================================
来源：http://pbq.xingfuxueyuan.xyz

[O01] 启动一个线程
来源：http://uxd.xylfe.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gvc.dashuyun.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zes.iojbl.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nqe.yongpay.top

TS:   // 同 JS
来源：http://vxz.xuanzx.com

Java: new Thread(() -> f()).start()
来源：http://wqf.quarkkingdee.top

Go:   go f()
来源：http://oyn.kuanghao11.cn

Ruby: Thread.new { f }
来源：http://guk.c1oappe.top

C#:   Task.Run(() => F());
来源：http://hjo.hywenlv.cn

[O02] 使用线程池
来源：http://wnq.pengpengdd.cyou

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wvw.cucudq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xmr.gotoacloud.top

JS:   // worker_threads 线程池
来源：http://iln.wangdashe.top

TS:   // worker_threads 线程池
来源：http://cmp.tian-w.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wlt.havefunace.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bof.hywenlv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wqg.chenlongwang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xon.ivvv.top

[O03] 加锁保护共享数据
来源：http://tjb.cqqwz.cn

Py:   with lock: shared += 1
来源：http://vzi.quarkkingdee.top

PHP:  // 用 flock() 做文件锁
来源：http://yvo.pycfn.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lee.yanxiufei.cn

TS:   // 同 JS
来源：http://tom.sysykeji.top

Java: synchronized (this) { shared++; }
来源：http://bdt.yueranfly.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rwv.feifeiyinyue.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://avy.hesvh.cn

C#:   lock (gate) { shared++; }
来源：http://dwm.yj20258888.top

[O04] 定义异步函数并等待
来源：http://yqh.ywan-chungtsiang.top

Py:   async def f():⏎    await g()
来源：http://egn.hfpthk.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cwj.yuanzhike.top

JS:   async function f() { await g(); }
来源：http://mrx.xziqi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gdo.fktsv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://unv.uphjek.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sca.zdbjq.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hub.jinghuilouyu.cn

C#:   async Task F() { await G(); }
来源：http://gdj.aibaodan.cn

[O05] 并发执行并等待全部完成
来源：http://exy.ywan-chungtsiang.top

Py:   asyncio.gather(*tasks)
来源：http://aka.dashuyun.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mrb.316326.xyz

JS:   await Promise.all(tasks)
来源：http://hdi.wangshuangyany.cn

TS:   await Promise.all(tasks)
来源：http://nql.hammf.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qvw.shangyingyoupin.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://spl.yongpay.top

Ruby: threads.map(&:join)
来源：http://qrk.birdmap.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ync.zhiwuduotai.top

[O06] 使用进程池
来源：http://kjl.fanxiaobao.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://icn.guowangkeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://niu.hnqzz.top

JS:   // child_process / cluster 模块
来源：http://gkd.hysaishi.cn

TS:   // child_process / cluster 模块
来源：http://waz.yuxming.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zgl.sweek.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://psy.quarkkingdee.top

Ruby: // fork 块
来源：http://bpp.52xcode.cn

C#:   Parallel.For
来源：http://ymr.smart0.xyz

================================================================================
来源：http://chs.vehdjk.com

P. 常用工具函数
来源：http://qxv.0kj1m.cn

================================================================================
来源：http://yav.c1oappe.top

[P01] 生成 UUID
来源：http://oju.nwbrower.top

Py:   str(uuid.uuid4())
来源：http://gez.jiagoushi.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jgx.tianlin.xyz

JS:   crypto.randomUUID()
来源：http://wvq.tianlin.xyz

TS:   crypto.randomUUID()
来源：http://wst.cucudq.cn

Java: UUID.randomUUID().toString()
来源：http://ywx.yuanzhike.top

Go:   // 用 github.com/google/uuid
来源：http://qjw.meibo888.top

Ruby: SecureRandom.uuid
来源：http://fjc.iojbl.cn

C#:   Guid.NewGuid().ToString()
来源：http://jfg.cashguo.top

[P02] MD5 / SHA256 摘要
来源：http://vml.9152youxi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wyl.xuetiantiany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pky.pycfn.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sxg.yj20258.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://phh.sweek.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pop.jqgufenzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nyb.zhongyouzk.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uvv.ybcxt.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sew.hysaishi.cn

[P03] 生成短随机字符串
来源：http://orr.tian-w.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hru.pycfn.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qjj.ppjwa.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kfm.yonumen.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hpv.nanxinkj.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cce.hfpthk.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fqa.ydzc1.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://dfy.chenjidiqi.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nax.quarkkingdee.top

[P04] 求长度
来源：http://zlj.52xcode.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bir.yj20258.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bbf.ctjpmb.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oxt.dashuyun.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nze.snrcjt.cn

Java: list.size();  map.size();  s.length()
来源：http://ggt.hesvh.cn

Go:   len(arr);  len(m)
来源：http://qcd.yueranfly.top

Ruby: x.length;  x.size
来源：http://jmr.zdqjudy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://igf.316326.xyz

[P05] 判断两个对象内容是否相等
来源：http://oel.yvedp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ani.jinqigfzy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zaa.yvedp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bcb.hywenlv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bkx.zhongyouzk.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wmk.jianghu66.top

Go:   reflect.DeepEqual(a, b)
来源：http://qxn.epnwcf.com

Ruby: a == b
来源：http://vsv.redwolf501.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jnn.0kj1m.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zzk.hfpthk.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://shs.fengsongda.top

PHP:  if (empty($x)) {}
来源：http://irq.jinyuanbaomall.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pit.fehbvm.com

TS:   if (x == null) {}
来源：http://rjy.yj20258.top

Java: if (x == null || x.isEmpty()) {}
来源：http://kxm.hnxiangtu.top

Go:   if x == nil {}
来源：http://zix.fzhhl.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ipa.haohaochexian.top

C#:   if (x is null) {}
来源：http://hfm.guannengcc.top

[P07] 防抖与节流
来源：http://jzs.jinyuanbaomall.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rda.sysykeji.top

PHP:  // 手写时间戳比较
来源：http://ynx.yongpay.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cwe.vqdsnc.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gsx.tian-w.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tfd.iojbl.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ldr.smart0.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://hai.bjfxy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://plk.vehdjk.com

[P08] 处理浮点精度问题
来源：http://qra.shanyushiyangkeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wdq.fktsv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kme.havefunace.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://szy.ivvv.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wxq.quarkkingdee.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gsu.hongshengwenyu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://npx.feifeiyinyue.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kmw.uphjek.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ozs.gogol.net.cn

================================================================================
来源：http://jde.pengpengdd.cyou

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://plx.shuidangran.top

================================================================================
来源：http://fki.vehdjk.com

[Q01] 创建表
来源：http://fzf.zhaomingkeji.xyz

CREATE TABLE users (
来源：http://zxa.hnxiangtu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://aif.quarkkingdee.top

name VARCHAR(50) NOT NULL,
来源：http://hre.aibaodan.cn

email VARCHAR(100) UNIQUE,
来源：http://zxb.gzhubu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jbn.chenlongwang.top

);
来源：http://zfj.dashuyun.cn

[Q02] 创建带外键的表
来源：http://kbw.jinqigufen.top

CREATE TABLE orders (
来源：http://bkm.feifeiyinyue.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jjm.tanke756.top

user_id INT NOT NULL,
来源：http://qyu.redwolf501.top

amount DECIMAL(10, 2),
来源：http://qdn.meibo888.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://eiv.ppjwa.cn

);
来源：http://wge.jinqigfzy.top

[Q03] 增加列
来源：http://iie.hesvh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gmq.bbcook.cn

[Q04] 修改列类型
来源：http://awm.pycfn.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ckm.9152youxi.cn

[Q05] 重命名列
来源：http://hlo.tian-w.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://izg.dashuyun.cn

[Q06] 删除列
来源：http://wds.52xcode.cn

ALTER TABLE users DROP COLUMN age;
来源：http://wxf.yfazqb.com

[Q07] 删除表
来源：http://ibb.nanxinkj.top

DROP TABLE IF EXISTS orders;
来源：http://nap.feifeiyinyue.top

[Q08] 创建普通索引
来源：http://gns.smart0.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://abi.chenjidiqi.icu

[Q09] 创建唯一索引
来源：http://csb.0kj1m.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gty.zhixingplan.top

[Q10] 插入单行
来源：http://ljj.tian-w.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kqu.yj20258.top

[Q11] 一次插入多行
来源：http://npe.zdqjudy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dja.sysykeji.top

[Q12] 插入后取自增 ID
来源：http://bht.sjlbkw.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xlx.xylfe.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cds.nwbrower.top

[Q13] 忽略重复插入
来源：http://dmh.wangdashe.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zga.zhaomingkeji.xyz

[Q14] 存在则更新（upsert）
来源：http://gkp.daxiang520.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bgv.316326.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://iry.tianlin.xyz

[Q15] 查询全部
来源：http://elg.yj202588.top

SELECT * FROM users;
来源：http://tdn.uphjek.com

[Q16] 查询指定列
来源：http://pnu.pycfn.com

SELECT id, name FROM users;
来源：http://qfq.hnxiangtu.top

[Q17] 条件查询
来源：http://cws.mhx1999.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kre.wangdashe.top

[Q18] 模糊匹配
来源：http://bbr.daria6918.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lpb.hnxiangtu.top

[Q19] 范围查询
来源：http://bbx.hywenlv.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lkl.kuanghao11.cn

[Q20] IN 列表
来源：http://rsi.haohaochexian.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lwi.shangyingyoupin.top

[Q21] 空值判断
来源：http://gxb.ydjk.org.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hrc.haohaochexian.top

[Q22] 排序
来源：http://ezb.vqdsnc.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jjv.aibaodan.cn

[Q23] 分页
来源：http://irb.gzhubu.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ycx.gaohongyu789.top

[Q24] 去重
来源：http://ext.snrcjt.cn

SELECT DISTINCT city FROM users;
来源：http://szc.hesvh.cn

[Q25] 只取前 N 条
来源：http://tdp.chenzaomai.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xdt.chenlongwang.top

[Q26] 计数
来源：http://zyx.meibo888.top

SELECT COUNT(*) FROM users;
来源：http://lpx.tarul.cn

[Q27] 条件计数
来源：http://fps.nwbrower.top


<!-- 参考信息 -->