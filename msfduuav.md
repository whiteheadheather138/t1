代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://kmi.ydzc1.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://dpm.gaohongyu789.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bwc.ydzc1.top

Go:   slices.Sort(arr)
来源：http://sfg.cheryme.top

Ruby: arr.sort
来源：http://vpx.jyoumei.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tto.fanxiaobao.xyz

[N03] 快速排序（分治示例）
来源：http://scd.snrcjt.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tcp.0kj1m.cn

PHP:  // 递归实现，或用 usort
来源：http://mka.daria6918.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xzi.guannengcc.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://anx.hnqzz.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wzy.hammf.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://stc.gogol.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wmg.hywenlv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gik.kuanghao11.cn

[N04] 斐波那契数列
来源：http://cza.shanyushiyangkeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://efo.yonumen.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sqd.jqgfzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://crl.hysaishi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://clm.jinqigfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fem.sysykeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://acl.yj202588.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rml.yuanzhike.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zax.jinyuanbaomall.cn

[N05] 最大公约数
来源：http://qpl.ivvv.top

Py:   math.gcd(a, b)
来源：http://xtl.guannengcc.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lwh.wangshuangyany.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fts.ppjwa.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qyz.bbcook.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mrb.zhoulong.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://otk.hywenlv.cn

Ruby: a.gcd(b)
来源：http://piv.hesvh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nrt.gzhubu.top

[N06] 判断回文字符串
来源：http://liq.fengsongda.top

Py:   s == s[::-1]
来源：http://sjw.hammf.cn

PHP:  $s === strrev($s);
来源：http://crn.ppjwa.cn

JS:   s === [...s].reverse().join("")
来源：http://wus.yonumen.top

TS:   s === [...s].reverse().join("")
来源：http://lru.zhijiandao.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rri.316326.xyz

Go:   // 双指针从两端比较
来源：http://xvv.tanke756.top

Ruby: s == s.reverse
来源：http://skd.zdqjudy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://gpj.uphjek.com

[N07] 两数之和（返回下标）
来源：http://afr.gotoacloud.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lto.hysaishi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bzx.gogol.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hpb.nanxinkj.top

TS:   // 手写 Map<string, number>
来源：http://jtj.zhixingplan.top

Java: // 手写 HashMap
来源：http://qrn.jyoumei.cn

Go:   // 手写 map[int]int
来源：http://lbg.yj202588.top

Ruby: // 手写 Hash
来源：http://wvy.9152youxi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://opz.dashuyun.cn

[N08] 生成全排列
来源：http://ucy.gotoacloud.top

Py:   itertools.permutations(arr)
来源：http://eqe.hywenlv.cn

PHP:  // 手写递归交换
来源：http://juy.xingfuxueyuan.xyz

JS:   // 手写回溯递归
来源：http://mlq.aibaodan.cn

TS:   // 手写回溯递归
来源：http://vly.ywan-chungtsiang.top

Java: // 手写回溯递归
来源：http://ksi.jyoumei.cn

Go:   // 手写回溯递归
来源：http://cfj.sweek.top

Ruby: arr.permutation.to_a
来源：http://hmd.sxryk.cn

C#:   // 手写回溯递归
来源：http://ioc.vqdsnc.cn

[N09] 栈与队列
来源：http://dor.jqgufenzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yzn.0kj1m.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ixy.meibo888.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kzz.gotoacloud.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ekq.jinqigufen.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qjz.bjfxy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ugo.ywan-chungtsiang.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cqr.birdmap.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://usw.xingfuxueyuan.xyz

[N10] 链表节点定义
来源：http://ihs.hammf.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jtu.nanxinkj.top

PHP:  class Node { public $v; public $next = null; }
来源：http://eeg.wangshuangyany.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zvm.wangshuangyany.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nkz.zhoulong.xyz

Java: class Node { int v; Node next; }
来源：http://pbl.andypj.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://lcm.epnwcf.com

Ruby: Node = Struct.new(:v, :next)
来源：http://biq.ybcxt.top

C#:   class Node { public int V; public Node? Next; }
来源：http://cqn.quarkkingdee.top

[N11] 二叉树中序遍历
来源：http://izt.cqqwz.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hwu.gaohongyu789.top

PHP:  // 手写递归函数
来源：http://sgq.cucudq.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://usi.sweek.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pcs.hnqzz.top

Java: // 手写递归
来源：http://wzf.pengpengdd.cyou

Go:   // 手写递归
来源：http://wdr.sysykeji.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cga.yfazqb.com

C#:   // 手写递归
来源：http://kfy.52xcode.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://veh.shanyushiyangtech.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://eli.wangshuangyany.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fcf.ctjpmb.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mgs.xuanzx.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oug.dianchejie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jrx.cashguo.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tfh.xylfe.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jii.sxryk.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kyn.zhixingplan.top

================================================================================
来源：http://rfh.zhijiandao.cn

O. 并发与异步
来源：http://txt.pycfn.com

================================================================================
来源：http://pxq.ywan-chungtsiang.top

[O01] 启动一个线程
来源：http://jqg.jianghu66.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://csh.sweek.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gdj.yueranfly.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://svn.cucudq.cn

TS:   // 同 JS
来源：http://xjp.bjfxy.top

Java: new Thread(() -> f()).start()
来源：http://bnl.meibo888.top

Go:   go f()
来源：http://vkf.fktsv.cn

Ruby: Thread.new { f }
来源：http://dmk.zhaomingkeji.xyz

C#:   Task.Run(() => F());
来源：http://equ.feifeiyinyue.top

[O02] 使用线程池
来源：http://xew.yongpay.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vvj.316326.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bxy.yanxiufei.cn

JS:   // worker_threads 线程池
来源：http://wdk.guowangkeji.top

TS:   // worker_threads 线程池
来源：http://oln.jqgufenzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://kto.pycfn.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gtl.guowangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pos.hesvh.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rpw.nanxuanxn.top

[O03] 加锁保护共享数据
来源：http://wjb.chenzaomai.com

Py:   with lock: shared += 1
来源：http://myh.dianchejie.cn

PHP:  // 用 flock() 做文件锁
来源：http://koj.chenlongwang.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sbl.jianghu66.top

TS:   // 同 JS
来源：http://pdo.ydzc1.top

Java: synchronized (this) { shared++; }
来源：http://egb.aibaodan.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uct.smart0.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://zzk.uphjek.com

C#:   lock (gate) { shared++; }
来源：http://rwu.bbcook.cn

[O04] 定义异步函数并等待
来源：http://uvq.zhongyouzk.top

Py:   async def f():⏎    await g()
来源：http://ibl.zhijiandao.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zdp.hysaishi.cn

JS:   async function f() { await g(); }
来源：http://hdv.jinqigfzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://boz.hammf.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://aus.gogol.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vyh.xingfuxueyuan.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://gpm.jiagoushi.top

C#:   async Task F() { await G(); }
来源：http://tql.yueranfly.top

[O05] 并发执行并等待全部完成
来源：http://ruc.daria6918.cn

Py:   asyncio.gather(*tasks)
来源：http://kjt.chenzaomai.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gep.cqqwz.cn

JS:   await Promise.all(tasks)
来源：http://arg.ppjwa.cn

TS:   await Promise.all(tasks)
来源：http://wud.ydzc1.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ejd.snrcjt.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://aed.uphjek.com

Ruby: threads.map(&:join)
来源：http://xkp.jyoumei.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yqm.wangdashe.top

[O06] 使用进程池
来源：http://qek.iojbl.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jud.hysaishi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hlx.ctjpmb.com

JS:   // child_process / cluster 模块
来源：http://det.yonumen.top

TS:   // child_process / cluster 模块
来源：http://rte.zhaomingkeji.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://siw.fktsv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://waq.kuanghao11.cn

Ruby: // fork 块
来源：http://sgn.dianchejie.cn

C#:   Parallel.For
来源：http://zfu.tian-w.cn

================================================================================
来源：http://cbp.quarkkingdee.top

P. 常用工具函数
来源：http://pwk.svipenyu.cn

================================================================================
来源：http://noj.fzhhl.top

[P01] 生成 UUID
来源：http://ioz.hongshengwenyu.top

Py:   str(uuid.uuid4())
来源：http://fpx.yuanzhike.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dyx.shangyingyoupin.top

JS:   crypto.randomUUID()
来源：http://znp.hnxiangtu.top

TS:   crypto.randomUUID()
来源：http://vhf.hongshengwenyu.top

Java: UUID.randomUUID().toString()
来源：http://nus.cheryme.top

Go:   // 用 github.com/google/uuid
来源：http://gwg.haohaochexian.top

Ruby: SecureRandom.uuid
来源：http://gfu.sysykeji.top

C#:   Guid.NewGuid().ToString()
来源：http://jfq.316326.xyz

[P02] MD5 / SHA256 摘要
来源：http://bzb.daria6918.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hpo.gaohongyu789.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qcj.fanxiaobao.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yyo.iojbl.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://exv.zycfv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fiw.vehdjk.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uef.jqgufenzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rjk.gogol.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xll.zhijiandao.cn

[P03] 生成短随机字符串
来源：http://ehu.zhijiandao.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://clv.shzxlz.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://try.quarkkingdee.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://whm.zhoulong.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://exw.zhijiandao.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gtn.ywan-chungtsiang.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wcq.ydzc1.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://pis.sufxvd.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vph.jinghuilouyu.cn

[P04] 求长度
来源：http://grb.jinyuanbaomall.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cri.zhijiandao.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://btv.shanyushiyangkeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://odb.xingfuxueyuan.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ihp.jiagoushi.top

Java: list.size();  map.size();  s.length()
来源：http://ksp.tian-w.cn

Go:   len(arr);  len(m)
来源：http://gil.yueranfly.top

Ruby: x.length;  x.size
来源：http://xup.ybcxt.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://cyd.sweek.top

[P05] 判断两个对象内容是否相等
来源：http://wuc.ppjwa.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cue.feifeiyinyue.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kcq.hywenlv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sxz.iojbl.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xhx.fengsongda.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hez.xinyue.icu

Go:   reflect.DeepEqual(a, b)
来源：http://iqv.316326.xyz

Ruby: a == b
来源：http://uqf.fehbvm.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wrs.hnqzz.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fes.hcnkem.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yma.chenlongwang.top

PHP:  if (empty($x)) {}
来源：http://clv.ydjk.org.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jcd.fktsv.cn

TS:   if (x == null) {}
来源：http://cgp.dashuyun.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xzg.bjfxy.top

Go:   if x == nil {}
来源：http://eiz.aibaodan.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wlj.9152youxi.cn

C#:   if (x is null) {}
来源：http://rie.guannengcc.top

[P07] 防抖与节流
来源：http://snd.fzhhl.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pwt.0kj1m.cn

PHP:  // 手写时间戳比较
来源：http://den.sysykeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dth.daria6918.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tyu.zdqjudy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nbg.wangdashe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://eoa.tianlin.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://bdk.ctjpmb.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sxx.guowangkeji.top

[P08] 处理浮点精度问题
来源：http://ror.ybcxt.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zmw.daria6918.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zex.xingfuxueyuan.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://opj.ivvv.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://iqi.daxiang520.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xkb.jinqigfzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rcl.sysykeji.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://evq.shangyingyoupin.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://usj.vehdjk.com

================================================================================
来源：http://feu.0kj1m.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zjv.dashuyun.cn

================================================================================
来源：http://ins.daria6918.cn

[Q01] 创建表
来源：http://fqh.316326.xyz

CREATE TABLE users (
来源：http://dev.fktsv.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nkk.c1oappe.top

name VARCHAR(50) NOT NULL,
来源：http://fgv.ywan-chungtsiang.top

email VARCHAR(100) UNIQUE,
来源：http://ybp.hcnkem.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wqh.jinyuanbaomall.cn

);
来源：http://xdh.yanxiufei.cn

[Q02] 创建带外键的表
来源：http://jyq.0kj1m.cn

CREATE TABLE orders (
来源：http://bim.xingfuxueyuan.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gsl.jinghuilouyu.cn

user_id INT NOT NULL,
来源：http://phf.sysykeji.top

amount DECIMAL(10, 2),
来源：http://pdj.kuanghao11.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zxx.bbcook.cn

);
来源：http://mji.tian-w.cn

[Q03] 增加列
来源：http://xbc.wangdashe.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fav.yuxming.cn

[Q04] 修改列类型
来源：http://ikr.daxiang520.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gqt.shanyushiyangtech.top

[Q05] 重命名列
来源：http://tgz.xinyue.icu

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pyc.yanxiufei.cn

[Q06] 删除列
来源：http://ifo.smart0.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://mhr.xuetiantiany.cn

[Q07] 删除表
来源：http://phl.jinyuanbaomall.cn

DROP TABLE IF EXISTS orders;
来源：http://phi.dianchejie.cn

[Q08] 创建普通索引
来源：http://etu.ppjwa.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://som.jiagoushi.top

[Q09] 创建唯一索引
来源：http://ial.fanxiaobao.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tvc.vqdsnc.cn

[Q10] 插入单行
来源：http://rtl.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bfz.jqgfzy.top

[Q11] 一次插入多行
来源：http://bop.epnwcf.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rog.zdqjudy.top

[Q12] 插入后取自增 ID
来源：http://eqw.dianchejie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rbi.pengpengdd.cyou

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ioz.yj202588.top

[Q13] 忽略重复插入
来源：http://dee.wangdashe.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mkr.tianlin.xyz

[Q14] 存在则更新（upsert）
来源：http://ysl.nwbrower.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fsj.wangshuangyany.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dgf.vqdsnc.cn

[Q15] 查询全部
来源：http://wfx.birdmap.top

SELECT * FROM users;
来源：http://jue.gzhubu.top

[Q16] 查询指定列
来源：http://zfh.gaohongyu789.top

SELECT id, name FROM users;
来源：http://fqg.zhiwuduotai.top

[Q17] 条件查询
来源：http://evn.fanxiaobao.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rlr.yangfankeji.com

[Q18] 模糊匹配
来源：http://bmn.guowangkeji.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xij.sufxvd.cn

[Q19] 范围查询
来源：http://oaj.wangshuangyany.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://haq.daria6918.cn

[Q20] IN 列表
来源：http://oem.fehbvm.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lye.chenlongwang.top

[Q21] 空值判断
来源：http://htn.snrcjt.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://rzf.svipenyu.cn

[Q22] 排序
来源：http://ppc.0kj1m.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lft.jqgfzy.top

[Q23] 分页
来源：http://zek.hysaishi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qdj.aibaodan.cn

[Q24] 去重
来源：http://uey.tanke756.top

SELECT DISTINCT city FROM users;
来源：http://wsi.yuanzhike.top

[Q25] 只取前 N 条
来源：http://wkg.hywenlv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wjb.pengpengdd.cyou

[Q26] 计数
来源：http://eny.yanxiufei.cn

SELECT COUNT(*) FROM users;
来源：http://oqj.yuxming.cn

[Q27] 条件计数
来源：http://bsc.cashguo.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://emd.quarkkingdee.top

[Q28] 求和与平均
来源：http://rhn.jinghuilouyu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sip.ydzc1.top

[Q29] 最大最小值
来源：http://eqz.yanxiufei.cn


<!-- 参考信息 -->