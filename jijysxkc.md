代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://sci.shanyushiyangtech.top

[N02] 排序（工程实践用内置实现）
来源：http://yhj.wangshuangyany.cn

Py:   sorted(arr);  arr.sort()
来源：http://fqb.316326.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cye.hongshengwenyu.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://fln.tarul.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://iwy.aizwys.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://eey.fzhhl.top

Go:   slices.Sort(arr)
来源：http://wru.nanxinkj.top

Ruby: arr.sort
来源：http://dpr.zhoulong.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://bav.dianchejie.cn

[N03] 快速排序（分治示例）
来源：http://fom.shuidangran.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://upi.bbcook.cn

PHP:  // 递归实现，或用 usort
来源：http://dga.kuanghao11.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rgp.sweek.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zlh.yonumen.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jkv.cheryme.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jmw.9152youxi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rgj.nanxuanxn.top

C#:   // 手写递归，或 Array.Sort
来源：http://hlk.tanke756.top

[N04] 斐波那契数列
来源：http://swh.ehwqpu.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://oes.pycfn.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rkj.shanyushiyangkeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ilk.tarul.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jyq.hammf.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mlw.hammf.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://egd.wangdashe.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gjc.xinyue.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://llp.cdnleiting.top

[N05] 最大公约数
来源：http://day.tanke756.top

Py:   math.gcd(a, b)
来源：http://bxn.zhiwuduotai.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vsp.cashguo.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://izv.uphjek.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qoq.wangshuangyany.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wqb.redwolf501.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://klm.yfazqb.com

Ruby: a.gcd(b)
来源：http://mqw.gaohongyu789.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fci.ybcxt.top

[N06] 判断回文字符串
来源：http://iwn.aizwys.cn

Py:   s == s[::-1]
来源：http://xbq.daria6918.cn

PHP:  $s === strrev($s);
来源：http://ita.316326.xyz

JS:   s === [...s].reverse().join("")
来源：http://ldn.cdnleiting.top

TS:   s === [...s].reverse().join("")
来源：http://hlk.jqgfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uvd.gzhubu.top

Go:   // 双指针从两端比较
来源：http://weq.hammf.cn

Ruby: s == s.reverse
来源：http://hgp.zdqjudy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://rnm.daria6918.cn

[N07] 两数之和（返回下标）
来源：http://qny.tarul.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cqu.iojbl.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vew.gaohongyu789.top

JS:   // 手写 Map：map.set(v, i)
来源：http://crn.shangyingyoupin.top

TS:   // 手写 Map<string, number>
来源：http://grl.0kj1m.cn

Java: // 手写 HashMap
来源：http://omz.xuanzx.com

Go:   // 手写 map[int]int
来源：http://opb.mhx1999.top

Ruby: // 手写 Hash
来源：http://dnx.hywenlv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ywp.tanke756.top

[N08] 生成全排列
来源：http://gnf.xziqi.cn

Py:   itertools.permutations(arr)
来源：http://sdm.aizwys.cn

PHP:  // 手写递归交换
来源：http://mjd.tarul.cn

JS:   // 手写回溯递归
来源：http://cyy.jiagoushi.top

TS:   // 手写回溯递归
来源：http://wur.jlsjyb.cn

Java: // 手写回溯递归
来源：http://mdw.hcnkem.com

Go:   // 手写回溯递归
来源：http://spo.hesvh.cn

Ruby: arr.permutation.to_a
来源：http://pyz.shanyushiyangkeji.top

C#:   // 手写回溯递归
来源：http://qpa.zdbjq.cn

[N09] 栈与队列
来源：http://gas.sjlbkw.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://heg.yfazqb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://umw.cheryme.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vwm.hnqzz.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wuf.vqdsnc.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zdl.yueranfly.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://obs.gaohongyu789.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://een.chenzaomai.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://otd.hywenlv.cn

[N10] 链表节点定义
来源：http://jij.yfazqb.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ilz.316326.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://hsx.zdbjq.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ird.0kj1m.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lhd.yongpay.top

Java: class Node { int v; Node next; }
来源：http://ngi.zhiwuduotai.top

Go:   type Node struct { V int; Next *Node }
来源：http://uwx.quarkkingdee.top

Ruby: Node = Struct.new(:v, :next)
来源：http://lda.cheryme.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ggf.jqgfzy.top

[N11] 二叉树中序遍历
来源：http://irv.yj20258888.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dyr.fktsv.cn

PHP:  // 手写递归函数
来源：http://zeb.yongpay.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ywf.aibaodan.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pvn.ydjk.org.cn

Java: // 手写递归
来源：http://jie.mhx1999.top

Go:   // 手写递归
来源：http://tvb.nanxuanxn.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ysq.hfpthk.cn

C#:   // 手写递归
来源：http://lnm.sweek.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pkq.yj20258888.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cqp.nanxinkj.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ili.yanxiufei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ism.zycfv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://urn.sufxvd.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://isc.ctjpmb.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://laa.guowangkeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pqh.gotoacloud.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://huq.zhiwuduotai.top

================================================================================
来源：http://djh.xuanzx.com

O. 并发与异步
来源：http://sgi.yj20258.top

================================================================================
来源：http://iwc.pycfn.com

[O01] 启动一个线程
来源：http://vns.yonumen.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zmk.wangshuangyany.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nyk.xingfuxueyuan.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wef.wangshuangyany.cn

TS:   // 同 JS
来源：http://yac.yj202588.top

Java: new Thread(() -> f()).start()
来源：http://bjl.sysykeji.top

Go:   go f()
来源：http://ydp.tarul.cn

Ruby: Thread.new { f }
来源：http://aca.hammf.cn

C#:   Task.Run(() => F());
来源：http://ojx.316326.xyz

[O02] 使用线程池
来源：http://hgz.jinghuilouyu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tcq.meibo888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oxc.jinyuanbaomall.cn

JS:   // worker_threads 线程池
来源：http://rxm.jlsjyb.cn

TS:   // worker_threads 线程池
来源：http://xup.aizwys.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gfu.sjlbkw.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://iwy.zdbjq.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lqd.cashguo.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uck.daxiang520.top

[O03] 加锁保护共享数据
来源：http://lnx.jlsjyb.cn

Py:   with lock: shared += 1
来源：http://rzp.fengsongda.top

PHP:  // 用 flock() 做文件锁
来源：http://rmp.yuanzhike.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rsb.redwolf501.top

TS:   // 同 JS
来源：http://cqb.ydjk.org.cn

Java: synchronized (this) { shared++; }
来源：http://awx.ydjk.org.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mgw.jianghu66.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://dss.sweek.top

C#:   lock (gate) { shared++; }
来源：http://yhp.zhoulong.xyz

[O04] 定义异步函数并等待
来源：http://gpx.hywenlv.cn

Py:   async def f():⏎    await g()
来源：http://rki.quarkkingdee.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://exz.shangyingyoupin.top

JS:   async function f() { await g(); }
来源：http://tlx.jianghu66.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://tlb.kuanghao11.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yvc.andypj.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fdm.ctjpmb.com

Ruby: # 用 Fiber 或 async gem
来源：http://nbv.tarul.cn

C#:   async Task F() { await G(); }
来源：http://lbr.nwbrower.top

[O05] 并发执行并等待全部完成
来源：http://rhy.0kj1m.cn

Py:   asyncio.gather(*tasks)
来源：http://gtp.fzhhl.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tfu.xylfe.cn

JS:   await Promise.all(tasks)
来源：http://wtv.smart0.xyz

TS:   await Promise.all(tasks)
来源：http://xgq.aizwys.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://aom.svipenyu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zvu.daria6918.cn

Ruby: threads.map(&:join)
来源：http://mnu.ybcxt.top

C#:   await Task.WhenAll(t1, t2)
来源：http://zmu.meibo888.top

[O06] 使用进程池
来源：http://vqh.aizwys.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://evo.gotoacloud.top

PHP:  // pcntl_fork 或多进程队列
来源：http://umq.epnwcf.com

JS:   // child_process / cluster 模块
来源：http://cac.zhaomingkeji.xyz

TS:   // child_process / cluster 模块
来源：http://dwo.jinqigufen.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ays.fanxiaobao.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zzt.jinqigfzy.top

Ruby: // fork 块
来源：http://zkk.ydzc1.top

C#:   Parallel.For
来源：http://ybh.shzxlz.cn

================================================================================
来源：http://bww.mhx1999.top

P. 常用工具函数
来源：http://oyg.zdqjudy.top

================================================================================
来源：http://zsn.fanxiaobao.xyz

[P01] 生成 UUID
来源：http://coy.epnwcf.com

Py:   str(uuid.uuid4())
来源：http://ktw.aizwys.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wgv.birdmap.top

JS:   crypto.randomUUID()
来源：http://cxq.xziqi.cn

TS:   crypto.randomUUID()
来源：http://maj.shangyingyoupin.top

Java: UUID.randomUUID().toString()
来源：http://gkq.pycfn.com

Go:   // 用 github.com/google/uuid
来源：http://gxw.yj20258.top

Ruby: SecureRandom.uuid
来源：http://xvh.nanxinkj.top

C#:   Guid.NewGuid().ToString()
来源：http://ngv.yonumen.top

[P02] MD5 / SHA256 摘要
来源：http://jdd.sjlbkw.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vow.jinqigfzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://yaw.hongshengwenyu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qdi.jinqigfzy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pgi.jinghuilouyu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rgc.wangshuangyany.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://khy.jinqigfzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kub.dianchejie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://duy.yj20258.top

[P03] 生成短随机字符串
来源：http://mpy.tanke756.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hhf.feifeiyinyue.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ywa.uphjek.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gig.zhoulong.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jgk.tanke756.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://doj.jinqigufen.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://prt.shzxlz.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://iqv.fzhhl.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ozo.sjlbkw.cn

[P04] 求长度
来源：http://xas.shangyingyoupin.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hnp.nanxinkj.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://now.xylfe.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bgk.dashuyun.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://urj.ydjk.org.cn

Java: list.size();  map.size();  s.length()
来源：http://xtj.dianchejie.cn

Go:   len(arr);  len(m)
来源：http://ako.yanxiufei.cn

Ruby: x.length;  x.size
来源：http://mon.yj20258.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://utz.c1oappe.top

[P05] 判断两个对象内容是否相等
来源：http://skf.hesvh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lzt.ybcxt.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://avb.hfpthk.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ybc.jinqigufen.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nfc.sxryk.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nyu.aizwys.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hoc.316326.xyz

Ruby: a == b
来源：http://zvp.ybcxt.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nos.yongpay.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ctm.jinghuilouyu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yzn.epnwcf.com

PHP:  if (empty($x)) {}
来源：http://ozw.tarul.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://njw.redwolf501.top

TS:   if (x == null) {}
来源：http://eje.ybcxt.top

Java: if (x == null || x.isEmpty()) {}
来源：http://zvv.guowangkeji.top

Go:   if x == nil {}
来源：http://uoc.hcnkem.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://csr.tianlin.xyz

C#:   if (x is null) {}
来源：http://rcb.xylfe.cn

[P07] 防抖与节流
来源：http://ccj.ybcxt.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mph.wangdashe.top

PHP:  // 手写时间戳比较
来源：http://idd.hysaishi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iso.xuanzx.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tei.iojbl.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ofs.xingfuxueyuan.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rtm.shzxlz.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lzq.hywenlv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kqn.feifeiyinyue.top

[P08] 处理浮点精度问题
来源：http://mvh.guowangkeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://use.ppjwa.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pll.tarul.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fol.vqdsnc.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ejn.jianghu66.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://luk.tian-w.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qgo.shanyushiyangtech.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nud.9152youxi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://adv.hysaishi.cn

================================================================================
来源：http://mtm.hammf.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vfq.shanyushiyangtech.top

================================================================================
来源：http://jdw.yueranfly.top

[Q01] 创建表
来源：http://xmz.redwolf501.top

CREATE TABLE users (
来源：http://vbt.cheryme.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://utt.pycfn.com

name VARCHAR(50) NOT NULL,
来源：http://hur.haohaochexian.top

email VARCHAR(100) UNIQUE,
来源：http://waj.bbcook.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://izz.zhijiandao.cn

);
来源：http://tbs.birdmap.top

[Q02] 创建带外键的表
来源：http://ahb.zhongyouzk.top

CREATE TABLE orders (
来源：http://xkj.fehbvm.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wqv.zhongyouzk.top

user_id INT NOT NULL,
来源：http://pjy.aizwys.cn

amount DECIMAL(10, 2),
来源：http://kpz.yongpay.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kcn.jqgfzy.top

);
来源：http://bgy.shuidangran.top

[Q03] 增加列
来源：http://dte.yj20258.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ybx.fehbvm.com

[Q04] 修改列类型
来源：http://uaw.ppjwa.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uch.yuxming.cn

[Q05] 重命名列
来源：http://rab.gaohongyu789.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ibx.zhijiandao.cn

[Q06] 删除列
来源：http://qfw.tanke756.top

ALTER TABLE users DROP COLUMN age;
来源：http://cqo.ppjwa.cn

[Q07] 删除表
来源：http://zob.cucudq.cn

DROP TABLE IF EXISTS orders;
来源：http://fmr.hesvh.cn

[Q08] 创建普通索引
来源：http://yeu.cheryme.top

CREATE INDEX idx_users_email ON users(email);
来源：http://rxm.mhx1999.top

[Q09] 创建唯一索引
来源：http://igp.daxiang520.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://off.uphjek.com

[Q10] 插入单行
来源：http://hpd.andypj.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jyu.zhoulong.xyz

[Q11] 一次插入多行
来源：http://zar.birdmap.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tyh.yuxming.cn

[Q12] 插入后取自增 ID
来源：http://cpb.gaohongyu789.top

INSERT INTO users (name) VALUES ('C');
来源：http://euu.xziqi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uyb.cheryme.top

[Q13] 忽略重复插入
来源：http://zjd.yuxming.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ugn.ppjwa.cn

[Q14] 存在则更新（upsert）
来源：http://vsk.pengpengdd.cyou

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wjw.zhiwuduotai.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zdz.shanyushiyangkeji.top

[Q15] 查询全部
来源：http://wvr.hnqzz.top

SELECT * FROM users;
来源：http://cra.cqqwz.cn

[Q16] 查询指定列
来源：http://jcb.52xcode.cn

SELECT id, name FROM users;
来源：http://alz.chenlongwang.top

[Q17] 条件查询
来源：http://ruj.gzhubu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sbt.sxryk.cn

[Q18] 模糊匹配
来源：http://akv.xuanzx.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ybk.yj202588.top

[Q19] 范围查询
来源：http://tlv.yuxming.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bsd.jinqigfzy.top

[Q20] IN 列表
来源：http://qgx.sufxvd.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rmn.xinyue.icu

[Q21] 空值判断
来源：http://sek.ybcxt.top

SELECT * FROM users WHERE email IS NULL;
来源：http://big.havefunace.top

[Q22] 排序
来源：http://wro.redwolf501.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kcd.vehdjk.com

[Q23] 分页
来源：http://pwp.wangshuangyany.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pph.hnxiangtu.top

[Q24] 去重
来源：http://twf.bbcook.cn

SELECT DISTINCT city FROM users;
来源：http://wwj.chenlongwang.top

[Q25] 只取前 N 条
来源：http://wuf.hfpthk.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hwz.yangfankeji.com

[Q26] 计数
来源：http://llz.0kj1m.cn

SELECT COUNT(*) FROM users;
来源：http://asx.havefunace.top

[Q27] 条件计数
来源：http://yee.cashguo.top


<!-- 参考信息 -->