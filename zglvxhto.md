代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://vay.hysaishi.cn

[N02] 排序（工程实践用内置实现）
来源：http://xua.jyoumei.cn

Py:   sorted(arr);  arr.sort()
来源：http://wsf.tianlin.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mhi.guannengcc.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://plq.zdbjq.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ppu.zdbjq.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xzr.cqqwz.cn

Go:   slices.Sort(arr)
来源：http://wmb.jinghuilouyu.cn

Ruby: arr.sort
来源：http://nph.yuxming.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mwo.ybcxt.top

[N03] 快速排序（分治示例）
来源：http://rli.redwolf501.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hte.snrcjt.cn

PHP:  // 递归实现，或用 usort
来源：http://rcx.smart0.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dxk.vehdjk.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ecn.hnqzz.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ipr.xingfuxueyuan.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wuu.jinqigufen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qlh.haohaochexian.top

C#:   // 手写递归，或 Array.Sort
来源：http://nbu.hywenlv.cn

[N04] 斐波那契数列
来源：http://wey.fehbvm.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pck.zhixingplan.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://plw.ydjk.org.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://szp.smart0.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wdg.yfazqb.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sjp.zhengqikj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xzy.zhoulong.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mxs.ydzc1.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://clo.pycfn.com

[N05] 最大公约数
来源：http://gpv.cucudq.cn

Py:   math.gcd(a, b)
来源：http://bxq.guowangkeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ozq.cdnleiting.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://whi.yanxiufei.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rzp.quarkkingdee.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ogo.cheryme.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://flf.sweek.top

Ruby: a.gcd(b)
来源：http://lnd.hysaishi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cqs.316326.xyz

[N06] 判断回文字符串
来源：http://etj.guowangkeji.top

Py:   s == s[::-1]
来源：http://zsc.zhixingplan.top

PHP:  $s === strrev($s);
来源：http://ddq.wangshuangyany.cn

JS:   s === [...s].reverse().join("")
来源：http://scu.yvedp.cn

TS:   s === [...s].reverse().join("")
来源：http://cud.hfpthk.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ilh.fehbvm.com

Go:   // 双指针从两端比较
来源：http://unv.fanxiaobao.xyz

Ruby: s == s.reverse
来源：http://yqn.c1oappe.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wuf.gotoacloud.top

[N07] 两数之和（返回下标）
来源：http://xhe.shuidangran.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fiw.fehbvm.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fan.vehdjk.com

JS:   // 手写 Map：map.set(v, i)
来源：http://sdd.zhaomingkeji.xyz

TS:   // 手写 Map<string, number>
来源：http://mgz.jyoumei.cn

Java: // 手写 HashMap
来源：http://eql.zdqjudy.top

Go:   // 手写 map[int]int
来源：http://jyb.snrcjt.cn

Ruby: // 手写 Hash
来源：http://pke.chenjidiqi.icu

C#:   // 手写 Dictionary<int, int>
来源：http://exy.yonumen.top

[N08] 生成全排列
来源：http://fmw.aizwys.cn

Py:   itertools.permutations(arr)
来源：http://hmk.yj202588.top

PHP:  // 手写递归交换
来源：http://bsp.yueranfly.top

JS:   // 手写回溯递归
来源：http://fem.cheryme.top

TS:   // 手写回溯递归
来源：http://vof.smart0.xyz

Java: // 手写回溯递归
来源：http://vks.jqgufenzy.top

Go:   // 手写回溯递归
来源：http://rzz.hfpthk.cn

Ruby: arr.permutation.to_a
来源：http://zoo.gogol.net.cn

C#:   // 手写回溯递归
来源：http://out.hnxiangtu.top

[N09] 栈与队列
来源：http://ecu.mhx1999.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gan.ehwqpu.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cta.yvedp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://aef.vehdjk.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jki.yj202588.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://snu.redwolf501.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zrs.xziqi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hgu.bbcook.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nnj.zhongyouzk.top

[N10] 链表节点定义
来源：http://sku.jqgfzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://adc.birdmap.top

PHP:  class Node { public $v; public $next = null; }
来源：http://zcv.daxiang520.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vey.jiagoushi.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ssw.shzxlz.cn

Java: class Node { int v; Node next; }
来源：http://fxw.bbcook.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jax.xinyue.icu

Ruby: Node = Struct.new(:v, :next)
来源：http://jgh.jlsjyb.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://djr.fehbvm.com

[N11] 二叉树中序遍历
来源：http://mjk.fktsv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vuz.gotoacloud.top

PHP:  // 手写递归函数
来源：http://vov.shanyushiyangkeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pqd.yonumen.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://spn.shzxlz.cn

Java: // 手写递归
来源：http://txc.guowangkeji.top

Go:   // 手写递归
来源：http://phr.xingfuxueyuan.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wtn.jinghuilouyu.cn

C#:   // 手写递归
来源：http://axi.jianghu66.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://unm.zhiwuduotai.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://opj.xuanzx.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qne.ivvv.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zaa.snrcjt.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://phh.yueranfly.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nju.wangdashe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tar.redwolf501.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sdz.havefunace.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kqq.shanyushiyangkeji.top

================================================================================
来源：http://pqg.pycfn.com

O. 并发与异步
来源：http://wld.yuxming.cn

================================================================================
来源：http://xvi.haohaochexian.top

[O01] 启动一个线程
来源：http://ntk.jqgfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sos.daxiang520.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wjj.yfazqb.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hmd.yuxming.cn

TS:   // 同 JS
来源：http://oas.gogol.net.cn

Java: new Thread(() -> f()).start()
来源：http://tbs.zdbjq.cn

Go:   go f()
来源：http://zam.havefunace.top

Ruby: Thread.new { f }
来源：http://lwb.hesvh.cn

C#:   Task.Run(() => F());
来源：http://gkf.9152youxi.cn

[O02] 使用线程池
来源：http://geh.bbcook.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ghw.hnqzz.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://clw.gotoacloud.top

JS:   // worker_threads 线程池
来源：http://yqm.xziqi.cn

TS:   // worker_threads 线程池
来源：http://dnh.zhixingplan.top

Java: Executors.newFixedThreadPool(4)
来源：http://tet.yuxming.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tug.jinghuilouyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qni.xylfe.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://boj.yj202588.top

[O03] 加锁保护共享数据
来源：http://qbm.c1oappe.top

Py:   with lock: shared += 1
来源：http://tcc.dashuyun.cn

PHP:  // 用 flock() 做文件锁
来源：http://unq.sjlbkw.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gfy.cashguo.top

TS:   // 同 JS
来源：http://hvm.cashguo.top

Java: synchronized (this) { shared++; }
来源：http://cbn.cucudq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ood.yuanzhike.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://roi.0kj1m.cn

C#:   lock (gate) { shared++; }
来源：http://npf.shuidangran.top

[O04] 定义异步函数并等待
来源：http://xpy.0kj1m.cn

Py:   async def f():⏎    await g()
来源：http://hev.cashguo.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://frj.hesvh.cn

JS:   async function f() { await g(); }
来源：http://soy.snrcjt.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ggz.hammf.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fgj.hfpthk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sfs.hysaishi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rhi.dianchejie.cn

C#:   async Task F() { await G(); }
来源：http://dqr.fanxiaobao.xyz

[O05] 并发执行并等待全部完成
来源：http://zzx.shanyushiyangtech.top

Py:   asyncio.gather(*tasks)
来源：http://vfl.0kj1m.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zvo.havefunace.top

JS:   await Promise.all(tasks)
来源：http://yte.smart0.xyz

TS:   await Promise.all(tasks)
来源：http://lrc.cheryme.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://knm.shanyushiyangtech.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yko.ydjk.org.cn

Ruby: threads.map(&:join)
来源：http://huz.cqqwz.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://exo.hesvh.cn

[O06] 使用进程池
来源：http://scd.xuetiantiany.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mqc.yfazqb.com

PHP:  // pcntl_fork 或多进程队列
来源：http://jta.dashuyun.cn

JS:   // child_process / cluster 模块
来源：http://icr.sjlbkw.cn

TS:   // child_process / cluster 模块
来源：http://cdb.cheryme.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://coz.yvedp.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bjy.yonumen.top

Ruby: // fork 块
来源：http://vwc.xylfe.cn

C#:   Parallel.For
来源：http://pdp.zhixingplan.top

================================================================================
来源：http://yxt.hysaishi.cn

P. 常用工具函数
来源：http://jaw.sysykeji.top

================================================================================
来源：http://vql.52xcode.cn

[P01] 生成 UUID
来源：http://dta.sufxvd.cn

Py:   str(uuid.uuid4())
来源：http://moa.52xcode.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lii.jqgfzy.top

JS:   crypto.randomUUID()
来源：http://ijq.c1oappe.top

TS:   crypto.randomUUID()
来源：http://jvc.hfpthk.cn

Java: UUID.randomUUID().toString()
来源：http://bto.zycfv.cn

Go:   // 用 github.com/google/uuid
来源：http://olj.fktsv.cn

Ruby: SecureRandom.uuid
来源：http://iof.ywan-chungtsiang.top

C#:   Guid.NewGuid().ToString()
来源：http://brs.redwolf501.top

[P02] MD5 / SHA256 摘要
来源：http://ftl.jinghuilouyu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://atl.pengpengdd.cyou

PHP:  hash("sha256", $s);  md5($s);
来源：http://zlq.mhx1999.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zsj.xingfuxueyuan.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tip.feifeiyinyue.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fbi.yuxming.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gga.yj20258.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://eaw.jinqigufen.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://iiz.birdmap.top

[P03] 生成短随机字符串
来源：http://xfm.zycfv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://imq.zhongyouzk.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nbo.nanxuanxn.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nwo.xziqi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://orp.yj20258.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uiu.guannengcc.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://awp.gzhubu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://nwr.shangyingyoupin.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qvp.hongshengwenyu.top

[P04] 求长度
来源：http://luo.yj202588.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qup.yj202588.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mji.sufxvd.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zgq.zhongyouzk.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cul.shangyingyoupin.top

Java: list.size();  map.size();  s.length()
来源：http://jmh.shangyingyoupin.top

Go:   len(arr);  len(m)
来源：http://npm.cashguo.top

Ruby: x.length;  x.size
来源：http://nyj.zdbjq.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://deq.hongshengwenyu.top

[P05] 判断两个对象内容是否相等
来源：http://cmd.fzhhl.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://oma.cdnleiting.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ync.ybcxt.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bvx.jyoumei.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wcs.vehdjk.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zdy.sysykeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://cns.fehbvm.com

Ruby: a == b
来源：http://arn.tian-w.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pze.jqgufenzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mwi.sysykeji.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jwn.jinghuilouyu.cn

PHP:  if (empty($x)) {}
来源：http://yyp.yueranfly.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://slt.vqdsnc.cn

TS:   if (x == null) {}
来源：http://ykj.316326.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://ael.hywenlv.cn

Go:   if x == nil {}
来源：http://tmg.ywan-chungtsiang.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dpo.hnxiangtu.top

C#:   if (x is null) {}
来源：http://mjn.chenzaomai.com

[P07] 防抖与节流
来源：http://duj.yonumen.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jdn.yj20258.top

PHP:  // 手写时间戳比较
来源：http://pui.ywan-chungtsiang.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://szb.ydjk.org.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hxr.tianlin.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ify.316326.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pug.zdqjudy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://gut.tianlin.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mxx.zhongyouzk.top

[P08] 处理浮点精度问题
来源：http://zub.guannengcc.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://drs.gotoacloud.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xaj.daria6918.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rlu.daxiang520.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://iqt.316326.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tok.yfazqb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tux.xziqi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sef.guowangkeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hnc.chenjidiqi.icu

================================================================================
来源：http://vvw.ybcxt.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kum.tanke756.top

================================================================================
来源：http://yhd.gotoacloud.top

[Q01] 创建表
来源：http://wkj.zhengqikj.top

CREATE TABLE users (
来源：http://uuk.sxryk.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lyu.hammf.cn

name VARCHAR(50) NOT NULL,
来源：http://kfx.cdnleiting.top

email VARCHAR(100) UNIQUE,
来源：http://ocz.zhengqikj.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nms.vqdsnc.cn

);
来源：http://pgj.tianlin.xyz

[Q02] 创建带外键的表
来源：http://etm.hfpthk.cn

CREATE TABLE orders (
来源：http://szz.jinghuilouyu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vrq.jianghu66.top

user_id INT NOT NULL,
来源：http://iny.yj20258.top

amount DECIMAL(10, 2),
来源：http://idb.hywenlv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ozj.fehbvm.com

);
来源：http://tfb.gotoacloud.top

[Q03] 增加列
来源：http://wwx.wangdashe.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kua.gotoacloud.top

[Q04] 修改列类型
来源：http://ugk.316326.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://myh.jqgufenzy.top

[Q05] 重命名列
来源：http://rtv.mhx1999.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zqo.shanyushiyangtech.top

[Q06] 删除列
来源：http://rxt.snrcjt.cn

ALTER TABLE users DROP COLUMN age;
来源：http://atu.ydzc1.top

[Q07] 删除表
来源：http://dbc.gzhubu.top

DROP TABLE IF EXISTS orders;
来源：http://raf.316326.xyz

[Q08] 创建普通索引
来源：http://lkb.fzhhl.top

CREATE INDEX idx_users_email ON users(email);
来源：http://uwr.yj20258888.top

[Q09] 创建唯一索引
来源：http://xnx.sweek.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tnc.cashguo.top

[Q10] 插入单行
来源：http://qpt.yj202588.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ghf.redwolf501.top

[Q11] 一次插入多行
来源：http://ncm.jinyuanbaomall.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qnq.yangfankeji.com

[Q12] 插入后取自增 ID
来源：http://azk.havefunace.top

INSERT INTO users (name) VALUES ('C');
来源：http://sic.zhongyouzk.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mop.zhaomingkeji.xyz

[Q13] 忽略重复插入
来源：http://yrj.fanxiaobao.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sty.cdnleiting.top

[Q14] 存在则更新（upsert）
来源：http://uip.ivvv.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nkn.c1oappe.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hxw.cheryme.top

[Q15] 查询全部
来源：http://pvw.xingfuxueyuan.xyz

SELECT * FROM users;
来源：http://lwf.ywan-chungtsiang.top

[Q16] 查询指定列
来源：http://usq.xuanzx.com

SELECT id, name FROM users;
来源：http://okf.yj202588.top

[Q17] 条件查询
来源：http://itl.aizwys.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://oic.gogol.net.cn

[Q18] 模糊匹配
来源：http://ouf.jqgfzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gxp.316326.xyz

[Q19] 范围查询
来源：http://kek.shuidangran.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sqi.hcnkem.com

[Q20] IN 列表
来源：http://suy.c1oappe.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://joe.guowangkeji.top

[Q21] 空值判断
来源：http://zzh.dianchejie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://rin.ehwqpu.com

[Q22] 排序
来源：http://oys.ehwqpu.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://npp.gzhubu.top

[Q23] 分页
来源：http://mpw.ehwqpu.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rtc.gzhubu.top

[Q24] 去重
来源：http://jzz.zhoulong.xyz

SELECT DISTINCT city FROM users;
来源：http://ruy.andypj.xyz

[Q25] 只取前 N 条
来源：http://hfl.ydjk.org.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zpn.zhoulong.xyz

[Q26] 计数
来源：http://age.haohaochexian.top

SELECT COUNT(*) FROM users;
来源：http://jvz.ehwqpu.com

[Q27] 条件计数
来源：http://plf.cucudq.cn


<!-- 参考信息 -->