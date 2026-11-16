代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://zpt.hongshengwenyu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://lin.meibo888.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tmo.andypj.xyz

Go:   slices.Sort(arr)
来源：http://tve.chenlongwang.top

Ruby: arr.sort
来源：http://bum.tian-w.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jgj.nwbrower.top

[N03] 快速排序（分治示例）
来源：http://wwa.zhaomingkeji.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xmr.c1oappe.top

PHP:  // 递归实现，或用 usort
来源：http://tjd.yvedp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jio.daxiang520.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://duf.jyoumei.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://owq.jinyuanbaomall.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hhd.dashuyun.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ieg.hcnkem.com

C#:   // 手写递归，或 Array.Sort
来源：http://jsb.quarkkingdee.top

[N04] 斐波那契数列
来源：http://czx.tianlin.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wlr.pycfn.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fmp.xuanzx.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yfo.chenlongwang.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oty.sysykeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kub.iojbl.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lea.yj20258.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://oxg.shanyushiyangtech.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bsi.xziqi.cn

[N05] 最大公约数
来源：http://ved.sjlbkw.cn

Py:   math.gcd(a, b)
来源：http://upz.cdnleiting.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ljo.daria6918.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dmx.chenjidiqi.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gkd.shzxlz.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://byz.yj20258.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://avt.cdnleiting.top

Ruby: a.gcd(b)
来源：http://boh.cucudq.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cou.shanyushiyangkeji.top

[N06] 判断回文字符串
来源：http://bzt.zhixingplan.top

Py:   s == s[::-1]
来源：http://jxn.zhongyouzk.top

PHP:  $s === strrev($s);
来源：http://rjo.chenjidiqi.icu

JS:   s === [...s].reverse().join("")
来源：http://spq.jyoumei.cn

TS:   s === [...s].reverse().join("")
来源：http://mhs.fzhhl.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kjs.dashuyun.cn

Go:   // 双指针从两端比较
来源：http://cat.fengsongda.top

Ruby: s == s.reverse
来源：http://ack.guannengcc.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ebv.ydjk.org.cn

[N07] 两数之和（返回下标）
来源：http://dsu.fktsv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nod.cheryme.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vim.yuanzhike.top

JS:   // 手写 Map：map.set(v, i)
来源：http://pqa.fanxiaobao.xyz

TS:   // 手写 Map<string, number>
来源：http://fgk.cqqwz.cn

Java: // 手写 HashMap
来源：http://vrx.zhiwuduotai.top

Go:   // 手写 map[int]int
来源：http://gyj.tian-w.cn

Ruby: // 手写 Hash
来源：http://xlm.redwolf501.top

C#:   // 手写 Dictionary<int, int>
来源：http://roo.chenjidiqi.icu

[N08] 生成全排列
来源：http://rbp.shanyushiyangkeji.top

Py:   itertools.permutations(arr)
来源：http://krp.jinqigufen.top

PHP:  // 手写递归交换
来源：http://iab.chenzaomai.com

JS:   // 手写回溯递归
来源：http://hbl.fktsv.cn

TS:   // 手写回溯递归
来源：http://jdu.zhijiandao.cn

Java: // 手写回溯递归
来源：http://obr.epnwcf.com

Go:   // 手写回溯递归
来源：http://sde.uphjek.com

Ruby: arr.permutation.to_a
来源：http://fnh.guannengcc.top

C#:   // 手写回溯递归
来源：http://dcq.yj20258888.top

[N09] 栈与队列
来源：http://myr.nanxuanxn.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gmv.gzhubu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iji.yuanzhike.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://job.fengsongda.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yae.jlsjyb.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jve.shanyushiyangkeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dzw.guowangkeji.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fsr.fengsongda.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wqf.svipenyu.cn

[N10] 链表节点定义
来源：http://mhe.zhengqikj.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://flm.hnxiangtu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://jnj.jqgufenzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://svk.hysaishi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://oyd.yonumen.top

Java: class Node { int v; Node next; }
来源：http://qld.hcnkem.com

Go:   type Node struct { V int; Next *Node }
来源：http://ebz.jlsjyb.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://oum.cqqwz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://dxb.yanxiufei.cn

[N11] 二叉树中序遍历
来源：http://gms.sweek.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://onj.shanyushiyangkeji.top

PHP:  // 手写递归函数
来源：http://nyf.c1oappe.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ijw.jinqigfzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jsc.ydjk.org.cn

Java: // 手写递归
来源：http://mea.sufxvd.cn

Go:   // 手写递归
来源：http://hro.cqqwz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tcd.hammf.cn

C#:   // 手写递归
来源：http://tic.nanxinkj.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dfr.xingfuxueyuan.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://roz.havefunace.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pxc.zhiwuduotai.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hph.svipenyu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zdi.sxryk.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qkp.quarkkingdee.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qfg.uphjek.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ptf.jqgufenzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kel.hcnkem.com

================================================================================
来源：http://utp.ywan-chungtsiang.top

O. 并发与异步
来源：http://les.fehbvm.com

================================================================================
来源：http://nee.aibaodan.cn

[O01] 启动一个线程
来源：http://qhy.cheryme.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uou.jqgufenzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ecp.nanxinkj.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yyi.shzxlz.cn

TS:   // 同 JS
来源：http://cvn.jinqigfzy.top

Java: new Thread(() -> f()).start()
来源：http://jxl.epnwcf.com

Go:   go f()
来源：http://ezr.cqqwz.cn

Ruby: Thread.new { f }
来源：http://whp.jiagoushi.top

C#:   Task.Run(() => F());
来源：http://xcf.zhiwuduotai.top

[O02] 使用线程池
来源：http://rmy.hammf.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nsy.yuxming.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fjy.birdmap.top

JS:   // worker_threads 线程池
来源：http://exd.svipenyu.cn

TS:   // worker_threads 线程池
来源：http://hzl.fanxiaobao.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://upi.chenjidiqi.icu

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ndw.fktsv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yza.nanxinkj.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mfg.kuanghao11.cn

[O03] 加锁保护共享数据
来源：http://xjo.hysaishi.cn

Py:   with lock: shared += 1
来源：http://twm.yuanzhike.top

PHP:  // 用 flock() 做文件锁
来源：http://mjj.daria6918.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jwm.cucudq.cn

TS:   // 同 JS
来源：http://jop.chenzaomai.com

Java: synchronized (this) { shared++; }
来源：http://wea.tarul.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jyr.cdnleiting.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://rfe.meibo888.top

C#:   lock (gate) { shared++; }
来源：http://afy.zhongyouzk.top

[O04] 定义异步函数并等待
来源：http://xic.jianghu66.top

Py:   async def f():⏎    await g()
来源：http://ipj.yongpay.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://puz.aizwys.cn

JS:   async function f() { await g(); }
来源：http://ixe.fzhhl.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://kug.cucudq.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rka.sxryk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jjq.snrcjt.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kya.havefunace.top

C#:   async Task F() { await G(); }
来源：http://yyl.zhengqikj.top

[O05] 并发执行并等待全部完成
来源：http://mwq.redwolf501.top

Py:   asyncio.gather(*tasks)
来源：http://kfz.jiagoushi.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qtt.zdbjq.cn

JS:   await Promise.all(tasks)
来源：http://uwl.nwbrower.top

TS:   await Promise.all(tasks)
来源：http://oco.jqgfzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ckj.ybcxt.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gsz.sufxvd.cn

Ruby: threads.map(&:join)
来源：http://hec.gogol.net.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://phh.hesvh.cn

[O06] 使用进程池
来源：http://jkj.c1oappe.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fzl.ydjk.org.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qhs.vehdjk.com

JS:   // child_process / cluster 模块
来源：http://see.zdbjq.cn

TS:   // child_process / cluster 模块
来源：http://pmm.cashguo.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vww.fzhhl.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nij.xziqi.cn

Ruby: // fork 块
来源：http://sto.yanxiufei.cn

C#:   Parallel.For
来源：http://pbq.ywan-chungtsiang.top

================================================================================
来源：http://gzc.zhiwuduotai.top

P. 常用工具函数
来源：http://evq.redwolf501.top

================================================================================
来源：http://zea.gzhubu.top

[P01] 生成 UUID
来源：http://hwu.wangdashe.top

Py:   str(uuid.uuid4())
来源：http://fam.yongpay.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uux.birdmap.top

JS:   crypto.randomUUID()
来源：http://vrf.daria6918.cn

TS:   crypto.randomUUID()
来源：http://aeo.hammf.cn

Java: UUID.randomUUID().toString()
来源：http://xog.zhijiandao.cn

Go:   // 用 github.com/google/uuid
来源：http://uwo.yueranfly.top

Ruby: SecureRandom.uuid
来源：http://ulb.gaohongyu789.top

C#:   Guid.NewGuid().ToString()
来源：http://ezc.fehbvm.com

[P02] MD5 / SHA256 摘要
来源：http://qsq.smart0.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vti.aizwys.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ftl.jqgufenzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ckf.cqqwz.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://imy.cdnleiting.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://iuu.pycfn.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yqm.ppjwa.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ytk.guannengcc.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mgp.yangfankeji.com

[P03] 生成短随机字符串
来源：http://aad.yvedp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lcc.52xcode.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kwq.ywan-chungtsiang.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xfh.birdmap.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://odj.nwbrower.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cgz.ywan-chungtsiang.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xpo.xylfe.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://prq.yvedp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fmc.chenzaomai.com

[P04] 求长度
来源：http://fcx.wangshuangyany.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fbz.zdqjudy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tvk.jinqigufen.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qdp.iojbl.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yfl.hfpthk.cn

Java: list.size();  map.size();  s.length()
来源：http://ofn.gaohongyu789.top

Go:   len(arr);  len(m)
来源：http://tho.daxiang520.top

Ruby: x.length;  x.size
来源：http://pff.yanxiufei.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cuh.ywan-chungtsiang.top

[P05] 判断两个对象内容是否相等
来源：http://agx.c1oappe.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://gbs.zdqjudy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dgb.ctjpmb.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tee.daxiang520.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://imt.xylfe.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hkz.jinghuilouyu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://owh.sufxvd.cn

Ruby: a == b
来源：http://dgk.cheryme.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://shu.yueranfly.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ueq.nwbrower.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tvi.zycfv.cn

PHP:  if (empty($x)) {}
来源：http://edy.chenjidiqi.icu

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nws.zhiwuduotai.top

TS:   if (x == null) {}
来源：http://vgv.hcnkem.com

Java: if (x == null || x.isEmpty()) {}
来源：http://rje.sjlbkw.cn

Go:   if x == nil {}
来源：http://hrh.yvedp.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ray.jyoumei.cn

C#:   if (x is null) {}
来源：http://dhl.redwolf501.top

[P07] 防抖与节流
来源：http://cah.gotoacloud.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jxu.zhijiandao.cn

PHP:  // 手写时间戳比较
来源：http://mxb.0kj1m.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://afx.tianlin.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pfu.xingfuxueyuan.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yag.zhoulong.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://upr.meibo888.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://gen.yuxming.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yae.hammf.cn

[P08] 处理浮点精度问题
来源：http://vgv.cheryme.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://amv.ywan-chungtsiang.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ruv.tianlin.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nwg.nanxuanxn.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sea.ctjpmb.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cid.zdqjudy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mvw.0kj1m.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ksu.vqdsnc.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ckw.cqqwz.cn

================================================================================
来源：http://eay.xuanzx.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://eyx.shzxlz.cn

================================================================================
来源：http://bld.jqgfzy.top

[Q01] 创建表
来源：http://mjt.gaohongyu789.top

CREATE TABLE users (
来源：http://uml.sjlbkw.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://syn.sxryk.cn

name VARCHAR(50) NOT NULL,
来源：http://mvn.jyoumei.cn

email VARCHAR(100) UNIQUE,
来源：http://vcq.hywenlv.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tly.9152youxi.cn

);
来源：http://gkd.zhengqikj.top

[Q02] 创建带外键的表
来源：http://zuu.cashguo.top

CREATE TABLE orders (
来源：http://typ.zdbjq.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tiv.chenzaomai.com

user_id INT NOT NULL,
来源：http://tgz.chenjidiqi.icu

amount DECIMAL(10, 2),
来源：http://fst.gogol.net.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mau.yvedp.cn

);
来源：http://blv.nanxinkj.top

[Q03] 增加列
来源：http://dxg.gzhubu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ojj.yj20258.top

[Q04] 修改列类型
来源：http://jeg.chenjidiqi.icu

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gdd.shuidangran.top

[Q05] 重命名列
来源：http://gve.cqqwz.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://djo.ywan-chungtsiang.top

[Q06] 删除列
来源：http://pbd.sxryk.cn

ALTER TABLE users DROP COLUMN age;
来源：http://cza.xylfe.cn

[Q07] 删除表
来源：http://kmv.jinqigfzy.top

DROP TABLE IF EXISTS orders;
来源：http://kky.jinyuanbaomall.cn

[Q08] 创建普通索引
来源：http://ltv.sufxvd.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://dti.yj202588.top

[Q09] 创建唯一索引
来源：http://fui.c1oappe.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mao.jqgufenzy.top

[Q10] 插入单行
来源：http://hkz.haohaochexian.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ecm.ywan-chungtsiang.top

[Q11] 一次插入多行
来源：http://ony.zhiwuduotai.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://luy.pycfn.com

[Q12] 插入后取自增 ID
来源：http://ltk.daria6918.cn

INSERT INTO users (name) VALUES ('C');
来源：http://led.xingfuxueyuan.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://waw.meibo888.top

[Q13] 忽略重复插入
来源：http://wkk.redwolf501.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vhw.uphjek.com

[Q14] 存在则更新（upsert）
来源：http://jwf.pycfn.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xdr.fehbvm.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ocp.sxryk.cn

[Q15] 查询全部
来源：http://vfu.jinghuilouyu.cn

SELECT * FROM users;
来源：http://kjt.gotoacloud.top

[Q16] 查询指定列
来源：http://qdz.xuetiantiany.cn

SELECT id, name FROM users;
来源：http://sjy.guannengcc.top

[Q17] 条件查询
来源：http://vtq.zhongyouzk.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pkb.sufxvd.cn

[Q18] 模糊匹配
来源：http://qon.hysaishi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ihx.zhaomingkeji.xyz

[Q19] 范围查询
来源：http://clx.dashuyun.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hkb.birdmap.top

[Q20] IN 列表
来源：http://xqt.shanyushiyangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://for.tianlin.xyz

[Q21] 空值判断
来源：http://avd.daria6918.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wvr.ppjwa.cn

[Q22] 排序
来源：http://evj.daria6918.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://psr.yvedp.cn

[Q23] 分页
来源：http://myv.nwbrower.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zhj.yuanzhike.top

[Q24] 去重
来源：http://bzw.epnwcf.com

SELECT DISTINCT city FROM users;
来源：http://wqu.jinqigfzy.top

[Q25] 只取前 N 条
来源：http://frr.bjfxy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://edg.pycfn.com

[Q26] 计数
来源：http://vti.yj20258.top

SELECT COUNT(*) FROM users;
来源：http://vfu.aizwys.cn

[Q27] 条件计数
来源：http://wvk.pengpengdd.cyou

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zob.jyoumei.cn

[Q28] 求和与平均
来源：http://klg.yongpay.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jck.nanxinkj.top

[Q29] 最大最小值
来源：http://trx.sufxvd.cn


<!-- 参考信息 -->