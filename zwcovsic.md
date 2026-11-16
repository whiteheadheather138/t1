代发 wailian999

Ruby: arr.sort
来源：http://fdo.52xcode.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xhn.redwolf501.top

[N03] 快速排序（分治示例）
来源：http://nlw.zdqjudy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rsd.xingfuxueyuan.xyz

PHP:  // 递归实现，或用 usort
来源：http://bcn.jinghuilouyu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://igt.uphjek.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sfa.wangshuangyany.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ozc.0kj1m.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ibb.hnqzz.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zcb.jinqigfzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://ini.yj202588.top

[N04] 斐波那契数列
来源：http://wbo.sufxvd.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rph.ydjk.org.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qtg.yanxiufei.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rrx.gotoacloud.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mys.jiagoushi.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://agi.gaohongyu789.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bgg.xingfuxueyuan.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tlc.gzhubu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zji.shangyingyoupin.top

[N05] 最大公约数
来源：http://qmg.cucudq.cn

Py:   math.gcd(a, b)
来源：http://tpf.cqqwz.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qqz.guannengcc.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ujd.hnxiangtu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lwl.dashuyun.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dqy.havefunace.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://byh.ybcxt.top

Ruby: a.gcd(b)
来源：http://nxk.cucudq.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wgo.chenzaomai.com

[N06] 判断回文字符串
来源：http://oce.jinqigfzy.top

Py:   s == s[::-1]
来源：http://xle.kuanghao11.cn

PHP:  $s === strrev($s);
来源：http://llj.zdqjudy.top

JS:   s === [...s].reverse().join("")
来源：http://qhs.vehdjk.com

TS:   s === [...s].reverse().join("")
来源：http://qga.zhijiandao.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ivp.daria6918.cn

Go:   // 双指针从两端比较
来源：http://gcx.meibo888.top

Ruby: s == s.reverse
来源：http://dgi.ydjk.org.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ogd.bbcook.cn

[N07] 两数之和（返回下标）
来源：http://qis.zycfv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://utu.hesvh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dfa.hfpthk.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ulz.ctjpmb.com

TS:   // 手写 Map<string, number>
来源：http://pic.sysykeji.top

Java: // 手写 HashMap
来源：http://jhj.ybcxt.top

Go:   // 手写 map[int]int
来源：http://ioc.birdmap.top

Ruby: // 手写 Hash
来源：http://ipq.hywenlv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sqr.fehbvm.com

[N08] 生成全排列
来源：http://wot.hongshengwenyu.top

Py:   itertools.permutations(arr)
来源：http://ncw.hesvh.cn

PHP:  // 手写递归交换
来源：http://gbv.yj20258.top

JS:   // 手写回溯递归
来源：http://lat.xziqi.cn

TS:   // 手写回溯递归
来源：http://nft.ybcxt.top

Java: // 手写回溯递归
来源：http://hao.zhengqikj.top

Go:   // 手写回溯递归
来源：http://uav.cheryme.top

Ruby: arr.permutation.to_a
来源：http://zwm.xziqi.cn

C#:   // 手写回溯递归
来源：http://keu.cashguo.top

[N09] 栈与队列
来源：http://vuk.dianchejie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lwz.fzhhl.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nvv.yj202588.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sjx.zhixingplan.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nrg.guowangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ujl.yvedp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uny.chenzaomai.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://idy.snrcjt.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fvx.xziqi.cn

[N10] 链表节点定义
来源：http://ysz.gogol.net.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jaa.zdbjq.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kkh.chenzaomai.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://asv.aizwys.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://twx.yj20258.top

Java: class Node { int v; Node next; }
来源：http://bap.jinqigufen.top

Go:   type Node struct { V int; Next *Node }
来源：http://tnv.cdnleiting.top

Ruby: Node = Struct.new(:v, :next)
来源：http://gdg.snrcjt.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://inf.shangyingyoupin.top

[N11] 二叉树中序遍历
来源：http://byh.quarkkingdee.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://eal.jqgufenzy.top

PHP:  // 手写递归函数
来源：http://ukt.hongshengwenyu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tfo.zycfv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://swf.hfpthk.cn

Java: // 手写递归
来源：http://lqf.gotoacloud.top

Go:   // 手写递归
来源：http://wxc.yuanzhike.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://scy.aibaodan.cn

C#:   // 手写递归
来源：http://hvm.zdqjudy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://flc.pycfn.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jcb.fehbvm.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uul.hysaishi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://acl.sysykeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ooi.zhiwuduotai.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gbe.kuanghao11.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fgl.yj202588.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sbr.cheryme.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://peg.epnwcf.com

================================================================================
来源：http://yvf.aizwys.cn

O. 并发与异步
来源：http://yqa.bbcook.cn

================================================================================
来源：http://ebe.xinyue.icu

[O01] 启动一个线程
来源：http://ctt.cashguo.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pke.hammf.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://oop.birdmap.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kob.snrcjt.cn

TS:   // 同 JS
来源：http://xmv.hysaishi.cn

Java: new Thread(() -> f()).start()
来源：http://yxs.wangshuangyany.cn

Go:   go f()
来源：http://bam.nanxinkj.top

Ruby: Thread.new { f }
来源：http://ffm.hongshengwenyu.top

C#:   Task.Run(() => F());
来源：http://jtf.epnwcf.com

[O02] 使用线程池
来源：http://dnz.feifeiyinyue.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sdy.yfazqb.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cxd.bbcook.cn

JS:   // worker_threads 线程池
来源：http://jfj.ydjk.org.cn

TS:   // worker_threads 线程池
来源：http://hou.xylfe.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rlg.yuxming.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ypf.ppjwa.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qbd.sxryk.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zbm.jyoumei.cn

[O03] 加锁保护共享数据
来源：http://jkl.0kj1m.cn

Py:   with lock: shared += 1
来源：http://rxj.cashguo.top

PHP:  // 用 flock() 做文件锁
来源：http://upp.0kj1m.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zwo.chenjidiqi.icu

TS:   // 同 JS
来源：http://yez.cashguo.top

Java: synchronized (this) { shared++; }
来源：http://hpv.shzxlz.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://doe.pycfn.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://son.yj20258888.top

C#:   lock (gate) { shared++; }
来源：http://pix.hysaishi.cn

[O04] 定义异步函数并等待
来源：http://xct.xuetiantiany.cn

Py:   async def f():⏎    await g()
来源：http://gmw.snrcjt.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dwe.zhengqikj.top

JS:   async function f() { await g(); }
来源：http://qaw.jlsjyb.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tjz.cqqwz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fqg.meibo888.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ucz.shangyingyoupin.top

Ruby: # 用 Fiber 或 async gem
来源：http://qot.sysykeji.top

C#:   async Task F() { await G(); }
来源：http://apz.snrcjt.cn

[O05] 并发执行并等待全部完成
来源：http://vgs.hywenlv.cn

Py:   asyncio.gather(*tasks)
来源：http://zrc.cashguo.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nse.zhoulong.xyz

JS:   await Promise.all(tasks)
来源：http://xpf.hfpthk.cn

TS:   await Promise.all(tasks)
来源：http://hkj.xuetiantiany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dso.316326.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vhy.shuidangran.top

Ruby: threads.map(&:join)
来源：http://gfe.sxryk.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xme.guannengcc.top

[O06] 使用进程池
来源：http://htw.wangshuangyany.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ahw.cucudq.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yhd.mhx1999.top

JS:   // child_process / cluster 模块
来源：http://lzu.yfazqb.com

TS:   // child_process / cluster 模块
来源：http://gll.9152youxi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lnh.zhaomingkeji.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://aui.xuetiantiany.cn

Ruby: // fork 块
来源：http://wtr.nanxinkj.top

C#:   Parallel.For
来源：http://zye.ctjpmb.com

================================================================================
来源：http://jls.sysykeji.top

P. 常用工具函数
来源：http://wdo.pycfn.com

================================================================================
来源：http://qyz.xinyue.icu

[P01] 生成 UUID
来源：http://zdx.fehbvm.com

Py:   str(uuid.uuid4())
来源：http://bac.shanyushiyangkeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oqk.yongpay.top

JS:   crypto.randomUUID()
来源：http://wcg.feifeiyinyue.top

TS:   crypto.randomUUID()
来源：http://ahd.shangyingyoupin.top

Java: UUID.randomUUID().toString()
来源：http://iod.yj20258.top

Go:   // 用 github.com/google/uuid
来源：http://gyk.ppjwa.cn

Ruby: SecureRandom.uuid
来源：http://brm.zdbjq.cn

C#:   Guid.NewGuid().ToString()
来源：http://rwm.tian-w.cn

[P02] MD5 / SHA256 摘要
来源：http://mdk.yfazqb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zvn.havefunace.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://gev.svipenyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baq.ydjk.org.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vcg.hnqzz.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zic.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://eld.316326.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yes.jlsjyb.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qyf.sweek.top

[P03] 生成短随机字符串
来源：http://mti.bjfxy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://awo.hongshengwenyu.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://urx.yuanzhike.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ttm.9152youxi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://awe.yuanzhike.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sts.ehwqpu.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gyt.nanxuanxn.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://twy.fktsv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tkt.chenjidiqi.icu

[P04] 求长度
来源：http://iww.haohaochexian.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rik.ehwqpu.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://knv.vqdsnc.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fxe.ydzc1.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://exm.gzhubu.top

Java: list.size();  map.size();  s.length()
来源：http://plj.pycfn.com

Go:   len(arr);  len(m)
来源：http://drj.smart0.xyz

Ruby: x.length;  x.size
来源：http://loo.birdmap.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://rmq.jinqigufen.top

[P05] 判断两个对象内容是否相等
来源：http://cog.sweek.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://oro.vehdjk.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tig.zhengqikj.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ceo.tarul.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ktw.cqqwz.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lic.hesvh.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yja.ydzc1.top

Ruby: a == b
来源：http://eqe.hammf.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yei.mhx1999.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://swd.epnwcf.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://roq.jinghuilouyu.cn

PHP:  if (empty($x)) {}
来源：http://pyu.nanxinkj.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qoj.bjfxy.top

TS:   if (x == null) {}
来源：http://afy.hammf.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hze.sweek.top

Go:   if x == nil {}
来源：http://zhg.jinqigufen.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://egt.hongshengwenyu.top

C#:   if (x is null) {}
来源：http://ucb.gzhubu.top

[P07] 防抖与节流
来源：http://pxh.0kj1m.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mzi.havefunace.top

PHP:  // 手写时间戳比较
来源：http://mzc.fengsongda.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vqe.gotoacloud.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lmo.xuanzx.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pre.jianghu66.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lxt.quarkkingdee.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://grl.xinyue.icu

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pgi.chenlongwang.top

[P08] 处理浮点精度问题
来源：http://lwk.xuetiantiany.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tmi.ydzc1.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://njm.chenzaomai.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://emp.yanxiufei.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bdf.snrcjt.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rvt.nanxuanxn.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vlo.chenjidiqi.icu

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mab.xuetiantiany.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jqs.vqdsnc.cn

================================================================================
来源：http://gsn.nanxinkj.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://exv.316326.xyz

================================================================================
来源：http://jrk.smart0.xyz

[Q01] 创建表
来源：http://mcs.hfpthk.cn

CREATE TABLE users (
来源：http://qra.shuidangran.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ltd.fengsongda.top

name VARCHAR(50) NOT NULL,
来源：http://qdd.iojbl.cn

email VARCHAR(100) UNIQUE,
来源：http://ytg.cdnleiting.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ifw.hongshengwenyu.top

);
来源：http://paw.ydzc1.top

[Q02] 创建带外键的表
来源：http://hzi.cucudq.cn

CREATE TABLE orders (
来源：http://nzt.cheryme.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lfs.hesvh.cn

user_id INT NOT NULL,
来源：http://zhl.shuidangran.top

amount DECIMAL(10, 2),
来源：http://ttk.52xcode.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ufn.wangshuangyany.cn

);
来源：http://icj.hongshengwenyu.top

[Q03] 增加列
来源：http://yqu.iojbl.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kth.zhiwuduotai.top

[Q04] 修改列类型
来源：http://fxj.yonumen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://stb.zhijiandao.cn

[Q05] 重命名列
来源：http://rfr.sjlbkw.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cvt.fanxiaobao.xyz

[Q06] 删除列
来源：http://jzy.andypj.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://mov.hcnkem.com

[Q07] 删除表
来源：http://qbc.guannengcc.top

DROP TABLE IF EXISTS orders;
来源：http://ypj.shzxlz.cn

[Q08] 创建普通索引
来源：http://wlo.redwolf501.top

CREATE INDEX idx_users_email ON users(email);
来源：http://bim.zhoulong.xyz

[Q09] 创建唯一索引
来源：http://eyn.smart0.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zzk.shzxlz.cn

[Q10] 插入单行
来源：http://qex.snrcjt.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://snk.uphjek.com

[Q11] 一次插入多行
来源：http://agh.redwolf501.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zvs.hammf.cn

[Q12] 插入后取自增 ID
来源：http://bzo.shangyingyoupin.top

INSERT INTO users (name) VALUES ('C');
来源：http://ghh.fktsv.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qkj.yfazqb.com

[Q13] 忽略重复插入
来源：http://kwc.ydzc1.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lom.epnwcf.com

[Q14] 存在则更新（upsert）
来源：http://vfv.havefunace.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zyg.hfpthk.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jel.guannengcc.top

[Q15] 查询全部
来源：http://yuu.zhengqikj.top

SELECT * FROM users;
来源：http://chd.0kj1m.cn

[Q16] 查询指定列
来源：http://als.yvedp.cn

SELECT id, name FROM users;
来源：http://plv.tianlin.xyz

[Q17] 条件查询
来源：http://fyw.hammf.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kog.gotoacloud.top

[Q18] 模糊匹配
来源：http://scc.zhijiandao.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wgm.cashguo.top

[Q19] 范围查询
来源：http://txr.zdqjudy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ogn.zdbjq.cn

[Q20] IN 列表
来源：http://exj.haohaochexian.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://elt.pycfn.com

[Q21] 空值判断
来源：http://ioq.yuxming.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pof.yvedp.cn

[Q22] 排序
来源：http://cqn.mhx1999.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xlu.jyoumei.cn

[Q23] 分页
来源：http://nqd.tianlin.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oxv.quarkkingdee.top

[Q24] 去重
来源：http://gew.sjlbkw.cn

SELECT DISTINCT city FROM users;
来源：http://dzx.shangyingyoupin.top

[Q25] 只取前 N 条
来源：http://tfh.yongpay.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://quk.jianghu66.top

[Q26] 计数
来源：http://apd.dashuyun.cn

SELECT COUNT(*) FROM users;
来源：http://zqy.jinqigfzy.top

[Q27] 条件计数
来源：http://nxt.ehwqpu.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ddu.xylfe.cn

[Q28] 求和与平均
来源：http://vtv.chenlongwang.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://iqc.xinyue.icu

[Q29] 最大最小值
来源：http://vgu.ydjk.org.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lcx.shanyushiyangkeji.top

[Q30] 分组统计
来源：http://ode.guannengcc.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kpw.xziqi.cn

[Q31] 分组后过滤
来源：http://fhw.fktsv.cn


<!-- 参考信息 -->