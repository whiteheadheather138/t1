代发 wailian999

Ruby: arr.sort
来源：http://kne.yangfankeji.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://qyx.sxryk.cn

[N03] 快速排序（分治示例）
来源：http://jjw.daria6918.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zmn.shanyushiyangtech.top

PHP:  // 递归实现，或用 usort
来源：http://yue.shanyushiyangtech.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wcz.shanyushiyangkeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hlw.ybcxt.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zcu.epnwcf.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hdt.hnxiangtu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wrh.iojbl.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pdt.hnxiangtu.top

[N04] 斐波那契数列
来源：http://pcy.wangshuangyany.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sty.bbcook.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vzp.jinqigfzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rdw.ydjk.org.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yud.shangyingyoupin.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ewx.ywan-chungtsiang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://teo.sweek.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zak.pengpengdd.cyou

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cfe.shzxlz.cn

[N05] 最大公约数
来源：http://xoi.bjfxy.top

Py:   math.gcd(a, b)
来源：http://ige.zdbjq.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sgq.yanxiufei.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pwj.tarul.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gwz.wangshuangyany.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://off.zdbjq.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wej.yueranfly.top

Ruby: a.gcd(b)
来源：http://rke.yj20258.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qiw.hongshengwenyu.top

[N06] 判断回文字符串
来源：http://bpm.zhixingplan.top

Py:   s == s[::-1]
来源：http://jyh.fengsongda.top

PHP:  $s === strrev($s);
来源：http://bfc.52xcode.cn

JS:   s === [...s].reverse().join("")
来源：http://oke.xylfe.cn

TS:   s === [...s].reverse().join("")
来源：http://obr.pycfn.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qau.chenzaomai.com

Go:   // 双指针从两端比较
来源：http://xbj.vehdjk.com

Ruby: s == s.reverse
来源：http://fqh.vehdjk.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://sen.pengpengdd.cyou

[N07] 两数之和（返回下标）
来源：http://imz.hongshengwenyu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ydx.guowangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fwn.shangyingyoupin.top

JS:   // 手写 Map：map.set(v, i)
来源：http://nlf.ybcxt.top

TS:   // 手写 Map<string, number>
来源：http://say.fktsv.cn

Java: // 手写 HashMap
来源：http://rsf.sufxvd.cn

Go:   // 手写 map[int]int
来源：http://qhb.birdmap.top

Ruby: // 手写 Hash
来源：http://ztp.yfazqb.com

C#:   // 手写 Dictionary<int, int>
来源：http://ogp.yvedp.cn

[N08] 生成全排列
来源：http://wac.shuidangran.top

Py:   itertools.permutations(arr)
来源：http://zrh.meibo888.top

PHP:  // 手写递归交换
来源：http://mkp.tarul.cn

JS:   // 手写回溯递归
来源：http://iop.guannengcc.top

TS:   // 手写回溯递归
来源：http://xny.yj20258.top

Java: // 手写回溯递归
来源：http://nvb.aibaodan.cn

Go:   // 手写回溯递归
来源：http://wij.fengsongda.top

Ruby: arr.permutation.to_a
来源：http://fnh.chenlongwang.top

C#:   // 手写回溯递归
来源：http://say.fzhhl.top

[N09] 栈与队列
来源：http://rfo.0kj1m.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tfo.daria6918.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pez.jinqigufen.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://igk.ydzc1.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lmh.daria6918.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bzc.feifeiyinyue.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rky.sxryk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xaz.yanxiufei.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sdw.cqqwz.cn

[N10] 链表节点定义
来源：http://aye.ivvv.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vur.zdbjq.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://usf.vehdjk.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gal.aizwys.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ldx.gogol.net.cn

Java: class Node { int v; Node next; }
来源：http://lyb.xziqi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://eja.yj20258.top

Ruby: Node = Struct.new(:v, :next)
来源：http://tcu.chenlongwang.top

C#:   class Node { public int V; public Node? Next; }
来源：http://pfa.pycfn.com

[N11] 二叉树中序遍历
来源：http://ijh.jinyuanbaomall.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://igs.yj20258.top

PHP:  // 手写递归函数
来源：http://mmy.fehbvm.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sdo.yj20258.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hmd.redwolf501.top

Java: // 手写递归
来源：http://gsy.yuanzhike.top

Go:   // 手写递归
来源：http://ohz.yuxming.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qzq.yonumen.top

C#:   // 手写递归
来源：http://aoc.tian-w.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kol.tianlin.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vtm.zhoulong.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hpe.shzxlz.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pjw.jinqigfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ghh.zhoulong.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gyz.wangdashe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lzg.uphjek.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xnk.svipenyu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://aaj.jqgufenzy.top

================================================================================
来源：http://hig.bjfxy.top

O. 并发与异步
来源：http://uwr.kuanghao11.cn

================================================================================
来源：http://jhd.aibaodan.cn

[O01] 启动一个线程
来源：http://dwe.zdqjudy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fvg.cdnleiting.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xdr.hesvh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kte.meibo888.top

TS:   // 同 JS
来源：http://qcu.dashuyun.cn

Java: new Thread(() -> f()).start()
来源：http://zdb.wangdashe.top

Go:   go f()
来源：http://ous.hnxiangtu.top

Ruby: Thread.new { f }
来源：http://nxo.aizwys.cn

C#:   Task.Run(() => F());
来源：http://cta.pengpengdd.cyou

[O02] 使用线程池
来源：http://bsy.tarul.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vaa.shangyingyoupin.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uzj.ywan-chungtsiang.top

JS:   // worker_threads 线程池
来源：http://ghf.wangdashe.top

TS:   // worker_threads 线程池
来源：http://mms.jinyuanbaomall.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gpo.hnqzz.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qol.chenjidiqi.icu

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tyb.xinyue.icu

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://krn.fktsv.cn

[O03] 加锁保护共享数据
来源：http://owo.hongshengwenyu.top

Py:   with lock: shared += 1
来源：http://klh.ehwqpu.com

PHP:  // 用 flock() 做文件锁
来源：http://nrq.jyoumei.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://abl.jinyuanbaomall.cn

TS:   // 同 JS
来源：http://vbe.wangshuangyany.cn

Java: synchronized (this) { shared++; }
来源：http://yqg.sxryk.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wmb.zhaomingkeji.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://opc.gzhubu.top

C#:   lock (gate) { shared++; }
来源：http://bgf.nwbrower.top

[O04] 定义异步函数并等待
来源：http://itb.xylfe.cn

Py:   async def f():⏎    await g()
来源：http://rgh.fanxiaobao.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://plk.0kj1m.cn

JS:   async function f() { await g(); }
来源：http://buo.yuanzhike.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://jep.iojbl.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sch.ybcxt.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://txt.zhixingplan.top

Ruby: # 用 Fiber 或 async gem
来源：http://omg.wangdashe.top

C#:   async Task F() { await G(); }
来源：http://vcg.birdmap.top

[O05] 并发执行并等待全部完成
来源：http://gqy.hnqzz.top

Py:   asyncio.gather(*tasks)
来源：http://bkf.316326.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xkh.52xcode.cn

JS:   await Promise.all(tasks)
来源：http://qit.cashguo.top

TS:   await Promise.all(tasks)
来源：http://pxb.hysaishi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uxw.hammf.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ont.sysykeji.top

Ruby: threads.map(&:join)
来源：http://cfn.sxryk.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://odb.yuxming.cn

[O06] 使用进程池
来源：http://yxr.sxryk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fhc.zhijiandao.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rrh.zhijiandao.cn

JS:   // child_process / cluster 模块
来源：http://cow.jianghu66.top

TS:   // child_process / cluster 模块
来源：http://mhr.316326.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uoq.hysaishi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jld.fanxiaobao.xyz

Ruby: // fork 块
来源：http://fgf.vehdjk.com

C#:   Parallel.For
来源：http://pmq.guowangkeji.top

================================================================================
来源：http://oig.yvedp.cn

P. 常用工具函数
来源：http://grx.cucudq.cn

================================================================================
来源：http://cnx.shangyingyoupin.top

[P01] 生成 UUID
来源：http://wed.xuanzx.com

Py:   str(uuid.uuid4())
来源：http://elo.birdmap.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dsc.guannengcc.top

JS:   crypto.randomUUID()
来源：http://fxj.sufxvd.cn

TS:   crypto.randomUUID()
来源：http://wme.hesvh.cn

Java: UUID.randomUUID().toString()
来源：http://uwk.ehwqpu.com

Go:   // 用 github.com/google/uuid
来源：http://loc.zhaomingkeji.xyz

Ruby: SecureRandom.uuid
来源：http://kvu.svipenyu.cn

C#:   Guid.NewGuid().ToString()
来源：http://ffv.tian-w.cn

[P02] MD5 / SHA256 摘要
来源：http://xfc.cheryme.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://aby.zhiwuduotai.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://rbm.jyoumei.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cce.jlsjyb.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fqr.yvedp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bsb.fehbvm.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mrz.guannengcc.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ekg.xingfuxueyuan.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hbs.c1oappe.top

[P03] 生成短随机字符串
来源：http://nds.guowangkeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wly.52xcode.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fee.gzhubu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wrv.dashuyun.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dxt.pengpengdd.cyou

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yri.shzxlz.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://klt.sweek.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://xti.xuanzx.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vrg.hfpthk.cn

[P04] 求长度
来源：http://rwz.cdnleiting.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://eeg.hywenlv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bor.yongpay.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nyi.mhx1999.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gnw.jiagoushi.top

Java: list.size();  map.size();  s.length()
来源：http://kbb.xingfuxueyuan.xyz

Go:   len(arr);  len(m)
来源：http://jxd.meibo888.top

Ruby: x.length;  x.size
来源：http://ygd.0kj1m.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://plf.ctjpmb.com

[P05] 判断两个对象内容是否相等
来源：http://pjw.zhaomingkeji.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://qtu.fehbvm.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://smg.epnwcf.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vdk.hnqzz.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ukl.cucudq.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zqr.xinyue.icu

Go:   reflect.DeepEqual(a, b)
来源：http://cgg.xinyue.icu

Ruby: a == b
来源：http://nuq.mhx1999.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://iyf.havefunace.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wbu.vehdjk.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wls.redwolf501.top

PHP:  if (empty($x)) {}
来源：http://tqt.hysaishi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://isg.shzxlz.cn

TS:   if (x == null) {}
来源：http://odc.zhongyouzk.top

Java: if (x == null || x.isEmpty()) {}
来源：http://fei.zdbjq.cn

Go:   if x == nil {}
来源：http://mut.xingfuxueyuan.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pub.bbcook.cn

C#:   if (x is null) {}
来源：http://phb.jinghuilouyu.cn

[P07] 防抖与节流
来源：http://qro.hnxiangtu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ayw.epnwcf.com

PHP:  // 手写时间戳比较
来源：http://zas.ywan-chungtsiang.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sqy.ivvv.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ovj.jinghuilouyu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xyo.epnwcf.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gge.jinghuilouyu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dul.jqgfzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pcc.jqgufenzy.top

[P08] 处理浮点精度问题
来源：http://jqs.aizwys.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kxr.yj20258888.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://knp.hcnkem.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wvr.yj202588.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kfu.bjfxy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://phd.uphjek.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zxa.epnwcf.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mge.jiagoushi.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://spp.quarkkingdee.top

================================================================================
来源：http://ajp.jinghuilouyu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://akc.shanyushiyangkeji.top

================================================================================
来源：http://pmt.hcnkem.com

[Q01] 创建表
来源：http://wds.shuidangran.top

CREATE TABLE users (
来源：http://hyf.ydzc1.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pbz.hfpthk.cn

name VARCHAR(50) NOT NULL,
来源：http://oeb.aibaodan.cn

email VARCHAR(100) UNIQUE,
来源：http://jph.guannengcc.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mxl.jlsjyb.cn

);
来源：http://kiy.nanxinkj.top

[Q02] 创建带外键的表
来源：http://eoe.jianghu66.top

CREATE TABLE orders (
来源：http://ohh.fengsongda.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://inx.sweek.top

user_id INT NOT NULL,
来源：http://uxv.hywenlv.cn

amount DECIMAL(10, 2),
来源：http://mag.wangdashe.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ykt.vqdsnc.cn

);
来源：http://ybi.fengsongda.top

[Q03] 增加列
来源：http://pdm.aizwys.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://luf.9152youxi.cn

[Q04] 修改列类型
来源：http://rao.zhoulong.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mlj.iojbl.cn

[Q05] 重命名列
来源：http://uoo.nwbrower.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yoq.zhongyouzk.top

[Q06] 删除列
来源：http://yju.daxiang520.top

ALTER TABLE users DROP COLUMN age;
来源：http://sbg.zhaomingkeji.xyz

[Q07] 删除表
来源：http://snt.vehdjk.com

DROP TABLE IF EXISTS orders;
来源：http://cgr.hnxiangtu.top

[Q08] 创建普通索引
来源：http://knb.gzhubu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://txn.vehdjk.com

[Q09] 创建唯一索引
来源：http://gnb.hongshengwenyu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zny.jinqigfzy.top

[Q10] 插入单行
来源：http://ozj.daria6918.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jtr.sxryk.cn

[Q11] 一次插入多行
来源：http://pro.iojbl.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://edg.zdbjq.cn

[Q12] 插入后取自增 ID
来源：http://otg.yfazqb.com

INSERT INTO users (name) VALUES ('C');
来源：http://zkv.shanyushiyangtech.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://adv.jianghu66.top

[Q13] 忽略重复插入
来源：http://xvk.aibaodan.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yvl.tarul.cn

[Q14] 存在则更新（upsert）
来源：http://xhv.yongpay.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rou.zhengqikj.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jew.jyoumei.cn

[Q15] 查询全部
来源：http://kly.yvedp.cn

SELECT * FROM users;
来源：http://kmf.chenlongwang.top

[Q16] 查询指定列
来源：http://trr.gzhubu.top

SELECT id, name FROM users;
来源：http://sru.jqgufenzy.top

[Q17] 条件查询
来源：http://vxy.tian-w.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pwp.zhixingplan.top

[Q18] 模糊匹配
来源：http://qlu.iojbl.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vlr.jlsjyb.cn

[Q19] 范围查询
来源：http://mnv.yfazqb.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pwk.zdbjq.cn

[Q20] IN 列表
来源：http://puw.haohaochexian.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ypf.sxryk.cn

[Q21] 空值判断
来源：http://toh.yvedp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fze.dashuyun.cn

[Q22] 排序
来源：http://mqi.xziqi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://skv.pycfn.com

[Q23] 分页
来源：http://yqc.yj20258.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://imx.snrcjt.cn

[Q24] 去重
来源：http://ltd.sufxvd.cn

SELECT DISTINCT city FROM users;
来源：http://iuh.nwbrower.top

[Q25] 只取前 N 条
来源：http://tle.shzxlz.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://agp.yongpay.top

[Q26] 计数
来源：http://rni.quarkkingdee.top

SELECT COUNT(*) FROM users;
来源：http://qyo.xuanzx.com

[Q27] 条件计数
来源：http://yiy.ywan-chungtsiang.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mvt.kuanghao11.cn

[Q28] 求和与平均
来源：http://jol.yuanzhike.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hky.ppjwa.cn

[Q29] 最大最小值
来源：http://uvh.ybcxt.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://nll.zdbjq.cn

[Q30] 分组统计
来源：http://luy.hongshengwenyu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://odb.tarul.cn

[Q31] 分组后过滤
来源：http://hcb.meibo888.top


<!-- 参考信息 -->