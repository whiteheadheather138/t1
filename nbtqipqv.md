代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://aqj.jianghu66.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://wha.shangyingyoupin.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wwt.hywenlv.cn

Go:   slices.Sort(arr)
来源：http://gtx.xingfuxueyuan.xyz

Ruby: arr.sort
来源：http://zun.fktsv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zwy.jiagoushi.top

[N03] 快速排序（分治示例）
来源：http://odw.jinyuanbaomall.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yzu.jqgufenzy.top

PHP:  // 递归实现，或用 usort
来源：http://jkh.yueranfly.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tzb.yfazqb.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dnw.daria6918.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://icm.yonumen.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hlo.ydzc1.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uad.zhiwuduotai.top

C#:   // 手写递归，或 Array.Sort
来源：http://rds.guannengcc.top

[N04] 斐波那契数列
来源：http://qzk.dianchejie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xok.shuidangran.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vtr.jqgfzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rfe.jianghu66.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zlm.yj20258888.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gau.dianchejie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ixp.jyoumei.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cun.jianghu66.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://viy.zhengqikj.top

[N05] 最大公约数
来源：http://bqa.tianlin.xyz

Py:   math.gcd(a, b)
来源：http://vmt.0kj1m.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://igl.kuanghao11.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ldo.aizwys.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jpo.dashuyun.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://opj.zdqjudy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gsn.chenlongwang.top

Ruby: a.gcd(b)
来源：http://xha.aizwys.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uuo.hfpthk.cn

[N06] 判断回文字符串
来源：http://hui.zhoulong.xyz

Py:   s == s[::-1]
来源：http://xhr.smart0.xyz

PHP:  $s === strrev($s);
来源：http://qhd.hcnkem.com

JS:   s === [...s].reverse().join("")
来源：http://nmg.hysaishi.cn

TS:   s === [...s].reverse().join("")
来源：http://fyy.shangyingyoupin.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ibe.hywenlv.cn

Go:   // 双指针从两端比较
来源：http://owg.xinyue.icu

Ruby: s == s.reverse
来源：http://ahw.yonumen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://hde.zycfv.cn

[N07] 两数之和（返回下标）
来源：http://msb.vqdsnc.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lak.tian-w.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kds.zycfv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hvh.ehwqpu.com

TS:   // 手写 Map<string, number>
来源：http://qyf.zdbjq.cn

Java: // 手写 HashMap
来源：http://oaz.yuanzhike.top

Go:   // 手写 map[int]int
来源：http://uaw.jinyuanbaomall.cn

Ruby: // 手写 Hash
来源：http://xir.jinghuilouyu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tmb.chenlongwang.top

[N08] 生成全排列
来源：http://jjw.9152youxi.cn

Py:   itertools.permutations(arr)
来源：http://jjq.aibaodan.cn

PHP:  // 手写递归交换
来源：http://bao.jinyuanbaomall.cn

JS:   // 手写回溯递归
来源：http://jwo.zhaomingkeji.xyz

TS:   // 手写回溯递归
来源：http://ozz.zdqjudy.top

Java: // 手写回溯递归
来源：http://tna.316326.xyz

Go:   // 手写回溯递归
来源：http://kmy.fehbvm.com

Ruby: arr.permutation.to_a
来源：http://jcd.bjfxy.top

C#:   // 手写回溯递归
来源：http://ztn.jinqigufen.top

[N09] 栈与队列
来源：http://jqw.chenjidiqi.icu

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yco.daxiang520.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vdf.jyoumei.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cic.sjlbkw.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kfu.yanxiufei.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://koy.sysykeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uqi.hywenlv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jkt.xingfuxueyuan.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uhq.zhengqikj.top

[N10] 链表节点定义
来源：http://zug.yueranfly.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dbu.iojbl.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xtu.cucudq.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qxy.dashuyun.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cev.ybcxt.top

Java: class Node { int v; Node next; }
来源：http://mev.yangfankeji.com

Go:   type Node struct { V int; Next *Node }
来源：http://yvd.birdmap.top

Ruby: Node = Struct.new(:v, :next)
来源：http://inw.nanxuanxn.top

C#:   class Node { public int V; public Node? Next; }
来源：http://vlh.yuxming.cn

[N11] 二叉树中序遍历
来源：http://swu.sufxvd.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cub.kuanghao11.cn

PHP:  // 手写递归函数
来源：http://ybe.316326.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kio.shzxlz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iwz.cdnleiting.top

Java: // 手写递归
来源：http://ybi.fehbvm.com

Go:   // 手写递归
来源：http://dfb.snrcjt.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fxn.hysaishi.cn

C#:   // 手写递归
来源：http://jid.cucudq.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ryt.hysaishi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fze.52xcode.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xab.redwolf501.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zsy.dashuyun.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://niy.guannengcc.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://irf.aizwys.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ckd.shangyingyoupin.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://aqb.jiagoushi.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rdg.hnqzz.top

================================================================================
来源：http://lnk.zdbjq.cn

O. 并发与异步
来源：http://dmt.hnxiangtu.top

================================================================================
来源：http://hby.svipenyu.cn

[O01] 启动一个线程
来源：http://lis.0kj1m.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qar.xylfe.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mfl.tian-w.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ncn.nanxinkj.top

TS:   // 同 JS
来源：http://jvj.shanyushiyangtech.top

Java: new Thread(() -> f()).start()
来源：http://avi.jinqigfzy.top

Go:   go f()
来源：http://ebh.c1oappe.top

Ruby: Thread.new { f }
来源：http://igr.tian-w.cn

C#:   Task.Run(() => F());
来源：http://efm.yj20258.top

[O02] 使用线程池
来源：http://wrg.daria6918.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pah.feifeiyinyue.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zcx.quarkkingdee.top

JS:   // worker_threads 线程池
来源：http://cdl.ivvv.top

TS:   // worker_threads 线程池
来源：http://eqb.xylfe.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tys.pycfn.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qlk.tianlin.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dmo.jiagoushi.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ckp.tianlin.xyz

[O03] 加锁保护共享数据
来源：http://ada.jinqigufen.top

Py:   with lock: shared += 1
来源：http://asu.zhixingplan.top

PHP:  // 用 flock() 做文件锁
来源：http://dim.xuanzx.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://oro.zhaomingkeji.xyz

TS:   // 同 JS
来源：http://oai.nanxuanxn.top

Java: synchronized (this) { shared++; }
来源：http://nes.jyoumei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://drt.fengsongda.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://uud.zhongyouzk.top

C#:   lock (gate) { shared++; }
来源：http://alh.bjfxy.top

[O04] 定义异步函数并等待
来源：http://seg.zhixingplan.top

Py:   async def f():⏎    await g()
来源：http://kwb.mhx1999.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yns.yuanzhike.top

JS:   async function f() { await g(); }
来源：http://qpg.snrcjt.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xkz.jqgfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dac.shangyingyoupin.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wiz.316326.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://rzf.redwolf501.top

C#:   async Task F() { await G(); }
来源：http://piq.jlsjyb.cn

[O05] 并发执行并等待全部完成
来源：http://pzj.nwbrower.top

Py:   asyncio.gather(*tasks)
来源：http://psv.ydzc1.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xsx.yfazqb.com

JS:   await Promise.all(tasks)
来源：http://egq.jiagoushi.top

TS:   await Promise.all(tasks)
来源：http://syf.hcnkem.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lzj.dianchejie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gqg.52xcode.cn

Ruby: threads.map(&:join)
来源：http://yhr.hesvh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ndc.fehbvm.com

[O06] 使用进程池
来源：http://urr.0kj1m.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://arw.vqdsnc.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://djj.jiagoushi.top

JS:   // child_process / cluster 模块
来源：http://zhh.dashuyun.cn

TS:   // child_process / cluster 模块
来源：http://hat.pycfn.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fke.shanyushiyangkeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xqp.gogol.net.cn

Ruby: // fork 块
来源：http://mvr.sweek.top

C#:   Parallel.For
来源：http://xds.ctjpmb.com

================================================================================
来源：http://twb.aizwys.cn

P. 常用工具函数
来源：http://omy.yuanzhike.top

================================================================================
来源：http://ans.gzhubu.top

[P01] 生成 UUID
来源：http://flh.jinqigufen.top

Py:   str(uuid.uuid4())
来源：http://xmh.316326.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qxr.jqgufenzy.top

JS:   crypto.randomUUID()
来源：http://vlm.zdqjudy.top

TS:   crypto.randomUUID()
来源：http://ylm.yj202588.top

Java: UUID.randomUUID().toString()
来源：http://qnt.yonumen.top

Go:   // 用 github.com/google/uuid
来源：http://bjx.chenlongwang.top

Ruby: SecureRandom.uuid
来源：http://kmf.fanxiaobao.xyz

C#:   Guid.NewGuid().ToString()
来源：http://jwn.yfazqb.com

[P02] MD5 / SHA256 摘要
来源：http://kjp.tianlin.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://crm.shanyushiyangkeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ddv.zhaomingkeji.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uzv.316326.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ipi.fengsongda.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kxg.nwbrower.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uof.yongpay.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tlb.nwbrower.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sjr.bbcook.cn

[P03] 生成短随机字符串
来源：http://hjs.hysaishi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://onr.hnxiangtu.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ahq.quarkkingdee.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pll.xuetiantiany.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://exz.chenlongwang.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://haf.yvedp.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qzh.9152youxi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://luo.ybcxt.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gvq.ywan-chungtsiang.top

[P04] 求长度
来源：http://lav.jinqigufen.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://edd.fanxiaobao.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iup.aibaodan.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qfy.guowangkeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ydj.sxryk.cn

Java: list.size();  map.size();  s.length()
来源：http://abj.birdmap.top

Go:   len(arr);  len(m)
来源：http://ioc.shanyushiyangtech.top

Ruby: x.length;  x.size
来源：http://ovx.nwbrower.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xco.cucudq.cn

[P05] 判断两个对象内容是否相等
来源：http://yzs.hesvh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://med.svipenyu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hnj.cucudq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://osn.jianghu66.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eoy.jinyuanbaomall.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gek.yfazqb.com

Go:   reflect.DeepEqual(a, b)
来源：http://irq.dashuyun.cn

Ruby: a == b
来源：http://prf.zhengqikj.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qix.iojbl.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mig.hfpthk.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://edk.c1oappe.top

PHP:  if (empty($x)) {}
来源：http://ivl.tanke756.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qmh.hnqzz.top

TS:   if (x == null) {}
来源：http://hhs.hfpthk.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://enp.nanxuanxn.top

Go:   if x == nil {}
来源：http://oet.ivvv.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://omu.zdbjq.cn

C#:   if (x is null) {}
来源：http://hvg.wangdashe.top

[P07] 防抖与节流
来源：http://iyl.guannengcc.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://obw.hammf.cn

PHP:  // 手写时间戳比较
来源：http://jbv.bjfxy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kji.hesvh.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bei.zhaomingkeji.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qhb.hnxiangtu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pxk.ctjpmb.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://bpe.tanke756.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ekk.ydjk.org.cn

[P08] 处理浮点精度问题
来源：http://jdg.yangfankeji.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xgm.dashuyun.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pes.ydjk.org.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fea.zhaomingkeji.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lhp.cashguo.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pnj.yangfankeji.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uxu.sufxvd.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dzc.hesvh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://iya.hywenlv.cn

================================================================================
来源：http://uny.cdnleiting.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://eis.chenlongwang.top

================================================================================
来源：http://xlx.jqgufenzy.top

[Q01] 创建表
来源：http://fkm.316326.xyz

CREATE TABLE users (
来源：http://raz.shuidangran.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qxi.vehdjk.com

name VARCHAR(50) NOT NULL,
来源：http://afs.yuanzhike.top

email VARCHAR(100) UNIQUE,
来源：http://uaw.jinqigfzy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pwa.hysaishi.cn

);
来源：http://bgr.kuanghao11.cn

[Q02] 创建带外键的表
来源：http://pct.ybcxt.top

CREATE TABLE orders (
来源：http://eib.zdqjudy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dfl.yuanzhike.top

user_id INT NOT NULL,
来源：http://ftg.tianlin.xyz

amount DECIMAL(10, 2),
来源：http://vkt.bjfxy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cvm.pengpengdd.cyou

);
来源：http://bin.hongshengwenyu.top

[Q03] 增加列
来源：http://siw.gzhubu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ibj.andypj.xyz

[Q04] 修改列类型
来源：http://wxf.smart0.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dgj.shuidangran.top

[Q05] 重命名列
来源：http://ymp.bjfxy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ybi.hcnkem.com

[Q06] 删除列
来源：http://sqg.pycfn.com

ALTER TABLE users DROP COLUMN age;
来源：http://xvz.redwolf501.top

[Q07] 删除表
来源：http://rqq.shanyushiyangtech.top

DROP TABLE IF EXISTS orders;
来源：http://kld.zhongyouzk.top

[Q08] 创建普通索引
来源：http://xad.zhoulong.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://cwl.tianlin.xyz

[Q09] 创建唯一索引
来源：http://oxw.nwbrower.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pzj.ydjk.org.cn

[Q10] 插入单行
来源：http://lox.zdbjq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nur.cdnleiting.top

[Q11] 一次插入多行
来源：http://cmn.bbcook.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://irz.yj20258.top

[Q12] 插入后取自增 ID
来源：http://cvp.hnqzz.top

INSERT INTO users (name) VALUES ('C');
来源：http://hax.ppjwa.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jzy.xuanzx.com

[Q13] 忽略重复插入
来源：http://shf.smart0.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oai.yongpay.top

[Q14] 存在则更新（upsert）
来源：http://frk.jinqigufen.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yzh.sjlbkw.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cmd.yfazqb.com

[Q15] 查询全部
来源：http://pfh.jinqigufen.top

SELECT * FROM users;
来源：http://uqa.tarul.cn

[Q16] 查询指定列
来源：http://ivn.fehbvm.com

SELECT id, name FROM users;
来源：http://qpe.birdmap.top

[Q17] 条件查询
来源：http://pqf.gotoacloud.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mam.yangfankeji.com

[Q18] 模糊匹配
来源：http://ili.yfazqb.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bml.smart0.xyz

[Q19] 范围查询
来源：http://qar.xziqi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://itb.zycfv.cn

[Q20] IN 列表
来源：http://aqa.uphjek.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tpb.pengpengdd.cyou

[Q21] 空值判断
来源：http://pxn.fktsv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ktk.hnqzz.top

[Q22] 排序
来源：http://tjy.cashguo.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cch.yangfankeji.com

[Q23] 分页
来源：http://yxy.hysaishi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://axp.kuanghao11.cn

[Q24] 去重
来源：http://ino.hcnkem.com

SELECT DISTINCT city FROM users;
来源：http://wcj.zhijiandao.cn

[Q25] 只取前 N 条
来源：http://liq.fanxiaobao.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dyp.yongpay.top

[Q26] 计数
来源：http://rtf.aibaodan.cn

SELECT COUNT(*) FROM users;
来源：http://kiz.sweek.top

[Q27] 条件计数
来源：http://idq.sweek.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fou.yj20258.top

[Q28] 求和与平均
来源：http://imq.bjfxy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://put.ywan-chungtsiang.top

[Q29] 最大最小值
来源：http://efw.jinqigufen.top


<!-- 参考信息 -->