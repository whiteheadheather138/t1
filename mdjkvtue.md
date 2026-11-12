代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://qje.fehbvm.com

[N02] 排序（工程实践用内置实现）
来源：http://ywt.svipenyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://pvi.jiagoushi.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vtk.chenlongwang.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://okp.yuanzhike.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://mqo.cqqwz.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://aqr.daria6918.cn

Go:   slices.Sort(arr)
来源：http://ghi.vehdjk.com

Ruby: arr.sort
来源：http://ljy.jianghu66.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qoj.cqqwz.cn

[N03] 快速排序（分治示例）
来源：http://jtn.fehbvm.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dqi.cheryme.top

PHP:  // 递归实现，或用 usort
来源：http://tmo.zhixingplan.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vya.cdnleiting.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vgq.jinqigufen.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://skh.jqgfzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ynz.hongshengwenyu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://twi.yongpay.top

C#:   // 手写递归，或 Array.Sort
来源：http://wik.jinqigfzy.top

[N04] 斐波那契数列
来源：http://kwo.shuidangran.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tsr.jianghu66.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fyf.hcnkem.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qih.yuanzhike.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qxc.tarul.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kbm.316326.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mxf.yangfankeji.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ppn.hcnkem.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yen.shuidangran.top

[N05] 最大公约数
来源：http://jly.xuetiantiany.cn

Py:   math.gcd(a, b)
来源：http://uea.gogol.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zig.mhx1999.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://myq.gogol.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ekm.shzxlz.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sqc.nanxuanxn.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://szo.9152youxi.cn

Ruby: a.gcd(b)
来源：http://ahh.ctjpmb.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://iit.52xcode.cn

[N06] 判断回文字符串
来源：http://rip.yanxiufei.cn

Py:   s == s[::-1]
来源：http://hxn.jlsjyb.cn

PHP:  $s === strrev($s);
来源：http://cjb.yj20258888.top

JS:   s === [...s].reverse().join("")
来源：http://qta.quarkkingdee.top

TS:   s === [...s].reverse().join("")
来源：http://lqg.jiagoushi.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gri.pengpengdd.cyou

Go:   // 双指针从两端比较
来源：http://fzp.zhijiandao.cn

Ruby: s == s.reverse
来源：http://xpn.hnxiangtu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://nzr.xylfe.cn

[N07] 两数之和（返回下标）
来源：http://ngq.sjlbkw.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gdw.52xcode.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tbr.shanyushiyangkeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://hvc.wangshuangyany.cn

TS:   // 手写 Map<string, number>
来源：http://hpz.fehbvm.com

Java: // 手写 HashMap
来源：http://rlp.cucudq.cn

Go:   // 手写 map[int]int
来源：http://jfd.bjfxy.top

Ruby: // 手写 Hash
来源：http://egh.hnxiangtu.top

C#:   // 手写 Dictionary<int, int>
来源：http://cxl.zycfv.cn

[N08] 生成全排列
来源：http://evx.zhijiandao.cn

Py:   itertools.permutations(arr)
来源：http://nkw.nanxuanxn.top

PHP:  // 手写递归交换
来源：http://uwu.ybcxt.top

JS:   // 手写回溯递归
来源：http://gjm.jlsjyb.cn

TS:   // 手写回溯递归
来源：http://uyv.guowangkeji.top

Java: // 手写回溯递归
来源：http://xgj.dashuyun.cn

Go:   // 手写回溯递归
来源：http://xjj.xziqi.cn

Ruby: arr.permutation.to_a
来源：http://abb.hcnkem.com

C#:   // 手写回溯递归
来源：http://npr.daxiang520.top

[N09] 栈与队列
来源：http://eur.snrcjt.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hkp.hnqzz.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qyv.ywan-chungtsiang.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jfc.shanyushiyangtech.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xnp.xinyue.icu

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lxj.316326.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://feo.vehdjk.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gom.zhiwuduotai.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://auq.tianlin.xyz

[N10] 链表节点定义
来源：http://fbo.fzhhl.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dai.hysaishi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sul.shzxlz.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://atm.yonumen.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kfp.quarkkingdee.top

Java: class Node { int v; Node next; }
来源：http://yxx.hcnkem.com

Go:   type Node struct { V int; Next *Node }
来源：http://lqh.xuanzx.com

Ruby: Node = Struct.new(:v, :next)
来源：http://kzz.xinyue.icu

C#:   class Node { public int V; public Node? Next; }
来源：http://srx.sweek.top

[N11] 二叉树中序遍历
来源：http://krq.jinqigufen.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kat.52xcode.cn

PHP:  // 手写递归函数
来源：http://eop.epnwcf.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lqi.aizwys.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kbc.aibaodan.cn

Java: // 手写递归
来源：http://poa.xuanzx.com

Go:   // 手写递归
来源：http://row.yuanzhike.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://our.redwolf501.top

C#:   // 手写递归
来源：http://ikf.cdnleiting.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xef.hnxiangtu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hdq.kuanghao11.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mwb.cheryme.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://erx.shanyushiyangtech.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pss.yj20258888.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kcd.9152youxi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pgm.dashuyun.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://woi.uphjek.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nlp.zdbjq.cn

================================================================================
来源：http://tas.zhoulong.xyz

O. 并发与异步
来源：http://ziz.bjfxy.top

================================================================================
来源：http://hip.nwbrower.top

[O01] 启动一个线程
来源：http://cqy.yanxiufei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dry.gogol.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ivu.iojbl.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xdj.zhoulong.xyz

TS:   // 同 JS
来源：http://crj.quarkkingdee.top

Java: new Thread(() -> f()).start()
来源：http://xku.guannengcc.top

Go:   go f()
来源：http://yky.snrcjt.cn

Ruby: Thread.new { f }
来源：http://odn.hnxiangtu.top

C#:   Task.Run(() => F());
来源：http://lzz.xingfuxueyuan.xyz

[O02] 使用线程池
来源：http://zzh.hammf.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wrz.dianchejie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hfa.guannengcc.top

JS:   // worker_threads 线程池
来源：http://rjs.fktsv.cn

TS:   // worker_threads 线程池
来源：http://atj.snrcjt.cn

Java: Executors.newFixedThreadPool(4)
来源：http://onu.guowangkeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jrb.jlsjyb.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://krx.shanyushiyangtech.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oso.cashguo.top

[O03] 加锁保护共享数据
来源：http://nqk.redwolf501.top

Py:   with lock: shared += 1
来源：http://fbr.fehbvm.com

PHP:  // 用 flock() 做文件锁
来源：http://zub.pycfn.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kho.gaohongyu789.top

TS:   // 同 JS
来源：http://kiu.cqqwz.cn

Java: synchronized (this) { shared++; }
来源：http://ibj.jinyuanbaomall.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pwo.havefunace.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://nyu.zhiwuduotai.top

C#:   lock (gate) { shared++; }
来源：http://zzm.cucudq.cn

[O04] 定义异步函数并等待
来源：http://dwc.xziqi.cn

Py:   async def f():⏎    await g()
来源：http://qkc.zhijiandao.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ifu.vehdjk.com

JS:   async function f() { await g(); }
来源：http://tks.redwolf501.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://pky.ppjwa.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hjg.ydjk.org.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tqc.yvedp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tvw.sysykeji.top

C#:   async Task F() { await G(); }
来源：http://ynw.jqgufenzy.top

[O05] 并发执行并等待全部完成
来源：http://hse.ivvv.top

Py:   asyncio.gather(*tasks)
来源：http://atv.zhixingplan.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dva.ydzc1.top

JS:   await Promise.all(tasks)
来源：http://dsx.cucudq.cn

TS:   await Promise.all(tasks)
来源：http://fgy.ppjwa.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hpy.yongpay.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xof.jqgufenzy.top

Ruby: threads.map(&:join)
来源：http://izs.shzxlz.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://emt.hongshengwenyu.top

[O06] 使用进程池
来源：http://osx.shanyushiyangtech.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nst.hcnkem.com

PHP:  // pcntl_fork 或多进程队列
来源：http://yta.dashuyun.cn

JS:   // child_process / cluster 模块
来源：http://ruu.jinghuilouyu.cn

TS:   // child_process / cluster 模块
来源：http://nnj.52xcode.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wbe.wangshuangyany.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ceq.feifeiyinyue.top

Ruby: // fork 块
来源：http://fmd.dianchejie.cn

C#:   Parallel.For
来源：http://pvb.haohaochexian.top

================================================================================
来源：http://rjg.yuanzhike.top

P. 常用工具函数
来源：http://wzn.zhijiandao.cn

================================================================================
来源：http://mfc.nwbrower.top

[P01] 生成 UUID
来源：http://ybm.jlsjyb.cn

Py:   str(uuid.uuid4())
来源：http://kjq.xuetiantiany.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cje.316326.xyz

JS:   crypto.randomUUID()
来源：http://tdp.vqdsnc.cn

TS:   crypto.randomUUID()
来源：http://tlv.hysaishi.cn

Java: UUID.randomUUID().toString()
来源：http://qta.bbcook.cn

Go:   // 用 github.com/google/uuid
来源：http://sdr.redwolf501.top

Ruby: SecureRandom.uuid
来源：http://unz.yfazqb.com

C#:   Guid.NewGuid().ToString()
来源：http://vzr.yj202588.top

[P02] MD5 / SHA256 摘要
来源：http://xxz.yj202588.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mls.daria6918.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vep.ehwqpu.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lce.cucudq.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rlo.ydzc1.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bhj.hesvh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://syv.bbcook.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cfd.tanke756.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ldb.shanyushiyangkeji.top

[P03] 生成短随机字符串
来源：http://ktx.redwolf501.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vqt.dianchejie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jtx.pycfn.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wtq.316326.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qtn.chenlongwang.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gvx.smart0.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jqm.ydzc1.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://jir.ybcxt.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qxw.bbcook.cn

[P04] 求长度
来源：http://akd.meibo888.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tnt.52xcode.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nki.bjfxy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sxo.wangshuangyany.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oht.zhixingplan.top

Java: list.size();  map.size();  s.length()
来源：http://vop.sxryk.cn

Go:   len(arr);  len(m)
来源：http://ldn.feifeiyinyue.top

Ruby: x.length;  x.size
来源：http://vig.bjfxy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://abz.meibo888.top

[P05] 判断两个对象内容是否相等
来源：http://kdf.bbcook.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pnv.9152youxi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ccu.cashguo.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cmp.yj20258888.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ymj.ppjwa.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kir.0kj1m.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tyj.c1oappe.top

Ruby: a == b
来源：http://jev.chenlongwang.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nzw.tianlin.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fah.tianlin.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://scx.shanyushiyangtech.top

PHP:  if (empty($x)) {}
来源：http://fkn.yonumen.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mlf.tanke756.top

TS:   if (x == null) {}
来源：http://jiz.jianghu66.top

Java: if (x == null || x.isEmpty()) {}
来源：http://uer.fktsv.cn

Go:   if x == nil {}
来源：http://nkk.yanxiufei.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gsd.havefunace.top

C#:   if (x is null) {}
来源：http://xuv.sysykeji.top

[P07] 防抖与节流
来源：http://gob.tanke756.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xbl.yj20258888.top

PHP:  // 手写时间戳比较
来源：http://jhk.hcnkem.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ezr.jianghu66.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://llz.hnxiangtu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xph.gogol.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vhh.shzxlz.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ohc.yueranfly.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qlo.jinghuilouyu.cn

[P08] 处理浮点精度问题
来源：http://faf.redwolf501.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://neo.zhijiandao.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vkd.daxiang520.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://plz.yj202588.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dny.gzhubu.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xzm.zycfv.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xmp.cheryme.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://brs.guannengcc.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qgx.c1oappe.top

================================================================================
来源：http://zfw.cdnleiting.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://neg.havefunace.top

================================================================================
来源：http://kho.yuanzhike.top

[Q01] 创建表
来源：http://oic.guannengcc.top

CREATE TABLE users (
来源：http://mog.gotoacloud.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qlc.nanxinkj.top

name VARCHAR(50) NOT NULL,
来源：http://ykm.aizwys.cn

email VARCHAR(100) UNIQUE,
来源：http://duf.snrcjt.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zma.xingfuxueyuan.xyz

);
来源：http://hti.shangyingyoupin.top

[Q02] 创建带外键的表
来源：http://hko.guowangkeji.top

CREATE TABLE orders (
来源：http://qst.jlsjyb.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ney.c1oappe.top

user_id INT NOT NULL,
来源：http://nuh.bbcook.cn

amount DECIMAL(10, 2),
来源：http://eyu.gogol.net.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kdz.shanyushiyangkeji.top

);
来源：http://xxm.bjfxy.top

[Q03] 增加列
来源：http://lpg.zhongyouzk.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nps.wangshuangyany.cn

[Q04] 修改列类型
来源：http://qhb.nwbrower.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://thw.cqqwz.cn

[Q05] 重命名列
来源：http://uxn.nwbrower.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://auz.iojbl.cn

[Q06] 删除列
来源：http://xor.guowangkeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://pml.xziqi.cn

[Q07] 删除表
来源：http://tka.havefunace.top

DROP TABLE IF EXISTS orders;
来源：http://pgr.ehwqpu.com

[Q08] 创建普通索引
来源：http://jco.hysaishi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vqq.epnwcf.com

[Q09] 创建唯一索引
来源：http://vhh.nanxuanxn.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xmz.yongpay.top

[Q10] 插入单行
来源：http://aud.ivvv.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://goy.ivvv.top

[Q11] 一次插入多行
来源：http://ixa.aibaodan.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ees.havefunace.top

[Q12] 插入后取自增 ID
来源：http://reb.xingfuxueyuan.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://ywu.chenzaomai.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pih.pycfn.com

[Q13] 忽略重复插入
来源：http://zur.hesvh.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kfs.fanxiaobao.xyz

[Q14] 存在则更新（upsert）
来源：http://jrn.sufxvd.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wnk.ehwqpu.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fkx.jinyuanbaomall.cn

[Q15] 查询全部
来源：http://qyc.ydzc1.top

SELECT * FROM users;
来源：http://jie.sysykeji.top

[Q16] 查询指定列
来源：http://gwg.aibaodan.cn

SELECT id, name FROM users;
来源：http://pth.cashguo.top

[Q17] 条件查询
来源：http://lmb.shzxlz.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bla.dianchejie.cn

[Q18] 模糊匹配
来源：http://csy.hysaishi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://esh.yonumen.top

[Q19] 范围查询
来源：http://yys.ehwqpu.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nju.gogol.net.cn

[Q20] IN 列表
来源：http://kww.jinqigufen.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://flf.hesvh.cn

[Q21] 空值判断
来源：http://zbz.zhixingplan.top

SELECT * FROM users WHERE email IS NULL;
来源：http://wwv.hongshengwenyu.top

[Q22] 排序
来源：http://ybx.cdnleiting.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cnn.shzxlz.cn

[Q23] 分页
来源：http://gla.zhijiandao.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fxm.yangfankeji.com

[Q24] 去重
来源：http://bua.fengsongda.top

SELECT DISTINCT city FROM users;
来源：http://puv.wangshuangyany.cn

[Q25] 只取前 N 条
来源：http://rry.hywenlv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://awm.zhijiandao.cn

[Q26] 计数
来源：http://dty.wangdashe.top

SELECT COUNT(*) FROM users;
来源：http://olg.hnxiangtu.top

[Q27] 条件计数
来源：http://fzc.xuetiantiany.cn


<!-- 参考信息 -->