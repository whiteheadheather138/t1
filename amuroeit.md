代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oji.jianghu66.top

Java: Arrays.binarySearch(arr, x)
来源：http://qsi.xuetiantiany.cn

Go:   sort.SearchInts(arr, x)
来源：http://xit.wangshuangyany.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://syy.iojbl.cn

C#:   Array.BinarySearch(arr, x)
来源：http://cqj.andypj.xyz

[N02] 排序（工程实践用内置实现）
来源：http://cdn.yanxiufei.cn

Py:   sorted(arr);  arr.sort()
来源：http://avg.yangfankeji.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rfs.tianlin.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://xcy.yvedp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://uor.guannengcc.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dfm.smart0.xyz

Go:   slices.Sort(arr)
来源：http://gwj.guannengcc.top

Ruby: arr.sort
来源：http://ers.sysykeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://llm.hammf.cn

[N03] 快速排序（分治示例）
来源：http://tft.hywenlv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://iqj.sysykeji.top

PHP:  // 递归实现，或用 usort
来源：http://etm.jinyuanbaomall.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pbd.ppjwa.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sph.daxiang520.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://evw.feifeiyinyue.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yor.c1oappe.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rpx.snrcjt.cn

C#:   // 手写递归，或 Array.Sort
来源：http://app.ybcxt.top

[N04] 斐波那契数列
来源：http://fay.hesvh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hza.yuxming.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://smd.uphjek.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fgv.yueranfly.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rqx.shzxlz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tan.sweek.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://avl.fengsongda.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gzg.wangshuangyany.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cwc.cheryme.top

[N05] 最大公约数
来源：http://oju.chenzaomai.com

Py:   math.gcd(a, b)
来源：http://eus.hongshengwenyu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lwr.mhx1999.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vxs.jqgufenzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cvv.chenjidiqi.icu

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kbt.jqgfzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mbb.gaohongyu789.top

Ruby: a.gcd(b)
来源：http://ihq.ppjwa.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://iaa.feifeiyinyue.top

[N06] 判断回文字符串
来源：http://upl.xziqi.cn

Py:   s == s[::-1]
来源：http://lsa.xinyue.icu

PHP:  $s === strrev($s);
来源：http://ejx.xinyue.icu

JS:   s === [...s].reverse().join("")
来源：http://bky.c1oappe.top

TS:   s === [...s].reverse().join("")
来源：http://puy.xingfuxueyuan.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kyz.svipenyu.cn

Go:   // 双指针从两端比较
来源：http://txw.andypj.xyz

Ruby: s == s.reverse
来源：http://aww.cucudq.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hme.wangshuangyany.cn

[N07] 两数之和（返回下标）
来源：http://iqz.jinghuilouyu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ezz.xinyue.icu

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jeo.kuanghao11.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vua.kuanghao11.cn

TS:   // 手写 Map<string, number>
来源：http://brk.xziqi.cn

Java: // 手写 HashMap
来源：http://tuh.jianghu66.top

Go:   // 手写 map[int]int
来源：http://hgg.cucudq.cn

Ruby: // 手写 Hash
来源：http://aum.hammf.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zna.gogol.net.cn

[N08] 生成全排列
来源：http://qem.316326.xyz

Py:   itertools.permutations(arr)
来源：http://hkr.ivvv.top

PHP:  // 手写递归交换
来源：http://sbc.redwolf501.top

JS:   // 手写回溯递归
来源：http://udb.yj20258888.top

TS:   // 手写回溯递归
来源：http://pon.0kj1m.cn

Java: // 手写回溯递归
来源：http://mqm.bbcook.cn

Go:   // 手写回溯递归
来源：http://cbv.cashguo.top

Ruby: arr.permutation.to_a
来源：http://giv.wangshuangyany.cn

C#:   // 手写回溯递归
来源：http://bay.nanxuanxn.top

[N09] 栈与队列
来源：http://wtv.yfazqb.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zse.zhixingplan.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://eaf.0kj1m.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ibz.bbcook.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yff.hfpthk.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qgo.wangdashe.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fam.hongshengwenyu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ley.cheryme.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://leb.daxiang520.top

[N10] 链表节点定义
来源：http://tzz.yj20258.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://akj.0kj1m.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tim.ydzc1.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sbr.fktsv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fhz.gaohongyu789.top

Java: class Node { int v; Node next; }
来源：http://dsx.jiagoushi.top

Go:   type Node struct { V int; Next *Node }
来源：http://xka.sufxvd.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://doi.shanyushiyangkeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://dil.yuanzhike.top

[N11] 二叉树中序遍历
来源：http://rbo.vehdjk.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://krn.ivvv.top

PHP:  // 手写递归函数
来源：http://oif.mhx1999.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aio.daxiang520.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rhr.hnqzz.top

Java: // 手写递归
来源：http://bff.andypj.xyz

Go:   // 手写递归
来源：http://esp.dianchejie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://eul.chenjidiqi.icu

C#:   // 手写递归
来源：http://bgk.vehdjk.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tsh.hnxiangtu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://txw.bbcook.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://khw.zhongyouzk.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://asd.hysaishi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lur.zdbjq.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mcd.hnqzz.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pst.tian-w.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://buu.wangshuangyany.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://non.zhoulong.xyz

================================================================================
来源：http://oko.52xcode.cn

O. 并发与异步
来源：http://prv.zdbjq.cn

================================================================================
来源：http://lsh.xylfe.cn

[O01] 启动一个线程
来源：http://ifg.xuetiantiany.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bpu.chenlongwang.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://buh.tanke756.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bbz.xinyue.icu

TS:   // 同 JS
来源：http://pwi.yueranfly.top

Java: new Thread(() -> f()).start()
来源：http://lvw.xinyue.icu

Go:   go f()
来源：http://dlm.shanyushiyangtech.top

Ruby: Thread.new { f }
来源：http://yba.52xcode.cn

C#:   Task.Run(() => F());
来源：http://ekb.cashguo.top

[O02] 使用线程池
来源：http://sai.ydjk.org.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xvv.yuanzhike.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dvc.cucudq.cn

JS:   // worker_threads 线程池
来源：http://ddx.aizwys.cn

TS:   // worker_threads 线程池
来源：http://zty.uphjek.com

Java: Executors.newFixedThreadPool(4)
来源：http://woj.jianghu66.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ddj.c1oappe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://anw.52xcode.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yea.shuidangran.top

[O03] 加锁保护共享数据
来源：http://vwy.daria6918.cn

Py:   with lock: shared += 1
来源：http://ltk.daxiang520.top

PHP:  // 用 flock() 做文件锁
来源：http://mfq.ppjwa.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cof.feifeiyinyue.top

TS:   // 同 JS
来源：http://hml.hnxiangtu.top

Java: synchronized (this) { shared++; }
来源：http://ipg.hnqzz.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ecy.xziqi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://onf.cashguo.top

C#:   lock (gate) { shared++; }
来源：http://yfi.epnwcf.com

[O04] 定义异步函数并等待
来源：http://svu.gaohongyu789.top

Py:   async def f():⏎    await g()
来源：http://bjz.mhx1999.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xxf.wangshuangyany.cn

JS:   async function f() { await g(); }
来源：http://iln.dianchejie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://lfp.snrcjt.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://utr.vqdsnc.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eem.52xcode.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xay.ivvv.top

C#:   async Task F() { await G(); }
来源：http://pbg.hnqzz.top

[O05] 并发执行并等待全部完成
来源：http://ust.jqgufenzy.top

Py:   asyncio.gather(*tasks)
来源：http://bwq.shanyushiyangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xax.cheryme.top

JS:   await Promise.all(tasks)
来源：http://uiq.zhongyouzk.top

TS:   await Promise.all(tasks)
来源：http://xmj.shanyushiyangkeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://aqa.fengsongda.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xzt.jlsjyb.cn

Ruby: threads.map(&:join)
来源：http://hnc.pengpengdd.cyou

C#:   await Task.WhenAll(t1, t2)
来源：http://mji.shanyushiyangtech.top

[O06] 使用进程池
来源：http://vud.yuanzhike.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kvu.dianchejie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yzw.yj202588.top

JS:   // child_process / cluster 模块
来源：http://pbj.xinyue.icu

TS:   // child_process / cluster 模块
来源：http://etx.sxryk.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wiq.0kj1m.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ljk.zdbjq.cn

Ruby: // fork 块
来源：http://bbx.tianlin.xyz

C#:   Parallel.For
来源：http://iqw.yueranfly.top

================================================================================
来源：http://lnm.yj20258888.top

P. 常用工具函数
来源：http://hya.chenzaomai.com

================================================================================
来源：http://ycw.zhiwuduotai.top

[P01] 生成 UUID
来源：http://fdd.ehwqpu.com

Py:   str(uuid.uuid4())
来源：http://dfd.cqqwz.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wdu.fzhhl.top

JS:   crypto.randomUUID()
来源：http://hxz.ehwqpu.com

TS:   crypto.randomUUID()
来源：http://sdw.shzxlz.cn

Java: UUID.randomUUID().toString()
来源：http://nvx.sjlbkw.cn

Go:   // 用 github.com/google/uuid
来源：http://eje.cashguo.top

Ruby: SecureRandom.uuid
来源：http://yda.guannengcc.top

C#:   Guid.NewGuid().ToString()
来源：http://kry.gaohongyu789.top

[P02] MD5 / SHA256 摘要
来源：http://vgy.shangyingyoupin.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rov.shanyushiyangtech.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ufd.yanxiufei.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wia.zhijiandao.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cjl.cheryme.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://aot.chenlongwang.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kur.snrcjt.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jjz.shuidangran.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wwh.bbcook.cn

[P03] 生成短随机字符串
来源：http://ciw.zdqjudy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hic.zhongyouzk.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dax.chenlongwang.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ynm.pycfn.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gqb.kuanghao11.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xuc.nwbrower.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gxe.jlsjyb.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gyy.mhx1999.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lie.yanxiufei.cn

[P04] 求长度
来源：http://uuu.shzxlz.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://plf.andypj.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zaa.jiagoushi.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lgb.sjlbkw.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://prg.xinyue.icu

Java: list.size();  map.size();  s.length()
来源：http://kbi.fehbvm.com

Go:   len(arr);  len(m)
来源：http://leq.ivvv.top

Ruby: x.length;  x.size
来源：http://tkp.birdmap.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xhz.cucudq.cn

[P05] 判断两个对象内容是否相等
来源：http://iwu.jqgfzy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://nus.yj20258.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fti.sysykeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://iiw.jianghu66.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cod.yuanzhike.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zsn.kuanghao11.cn

Go:   reflect.DeepEqual(a, b)
来源：http://uvc.xuetiantiany.cn

Ruby: a == b
来源：http://muw.shanyushiyangtech.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xqp.hammf.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uwo.jinqigufen.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fns.ydzc1.top

PHP:  if (empty($x)) {}
来源：http://rzj.yj20258.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lpa.snrcjt.cn

TS:   if (x == null) {}
来源：http://aeu.tanke756.top

Java: if (x == null || x.isEmpty()) {}
来源：http://hwn.fanxiaobao.xyz

Go:   if x == nil {}
来源：http://pat.hammf.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qnu.cashguo.top

C#:   if (x is null) {}
来源：http://zcw.c1oappe.top

[P07] 防抖与节流
来源：http://mth.zhengqikj.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bmc.zhaomingkeji.xyz

PHP:  // 手写时间戳比较
来源：http://fdt.xuanzx.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tqf.chenzaomai.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lhq.jiagoushi.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ylk.guowangkeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mmo.zdqjudy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://dep.bbcook.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ynv.zdqjudy.top

[P08] 处理浮点精度问题
来源：http://bmj.yj202588.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nfy.daxiang520.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kfd.dianchejie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dwc.zhongyouzk.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gsg.c1oappe.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ghs.dashuyun.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uhr.pengpengdd.cyou

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lhr.cucudq.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vap.yvedp.cn

================================================================================
来源：http://psr.cashguo.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dui.hnqzz.top

================================================================================
来源：http://ksf.gotoacloud.top

[Q01] 创建表
来源：http://leb.cdnleiting.top

CREATE TABLE users (
来源：http://xrd.yonumen.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kpn.bbcook.cn

name VARCHAR(50) NOT NULL,
来源：http://goj.yueranfly.top

email VARCHAR(100) UNIQUE,
来源：http://xgm.fehbvm.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wci.jinyuanbaomall.cn

);
来源：http://cwq.hcnkem.com

[Q02] 创建带外键的表
来源：http://xhd.aizwys.cn

CREATE TABLE orders (
来源：http://fgb.yangfankeji.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kyg.uphjek.com

user_id INT NOT NULL,
来源：http://ynt.sxryk.cn

amount DECIMAL(10, 2),
来源：http://zbc.pengpengdd.cyou

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ccz.xuanzx.com

);
来源：http://qvd.pycfn.com

[Q03] 增加列
来源：http://bkq.hesvh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dzc.gaohongyu789.top

[Q04] 修改列类型
来源：http://sup.uphjek.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tfq.jinqigufen.top

[Q05] 重命名列
来源：http://skg.yangfankeji.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://osh.daxiang520.top

[Q06] 删除列
来源：http://tbr.yfazqb.com

ALTER TABLE users DROP COLUMN age;
来源：http://vvb.0kj1m.cn

[Q07] 删除表
来源：http://bbq.sufxvd.cn

DROP TABLE IF EXISTS orders;
来源：http://nob.zycfv.cn

[Q08] 创建普通索引
来源：http://rnp.zdbjq.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xdr.zhixingplan.top

[Q09] 创建唯一索引
来源：http://flw.chenzaomai.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sao.mhx1999.top

[Q10] 插入单行
来源：http://pws.jianghu66.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lrm.316326.xyz

[Q11] 一次插入多行
来源：http://dks.ywan-chungtsiang.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kvg.snrcjt.cn

[Q12] 插入后取自增 ID
来源：http://wtp.yj20258.top

INSERT INTO users (name) VALUES ('C');
来源：http://pqa.shangyingyoupin.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://syn.fanxiaobao.xyz

[Q13] 忽略重复插入
来源：http://vhm.cashguo.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xju.hnqzz.top

[Q14] 存在则更新（upsert）
来源：http://ctp.gzhubu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ybp.cucudq.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qjd.sysykeji.top

[Q15] 查询全部
来源：http://eta.pengpengdd.cyou

SELECT * FROM users;
来源：http://hco.cucudq.cn

[Q16] 查询指定列
来源：http://eky.gzhubu.top

SELECT id, name FROM users;
来源：http://hsb.xinyue.icu

[Q17] 条件查询
来源：http://eol.dianchejie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ezw.shangyingyoupin.top

[Q18] 模糊匹配
来源：http://ksp.daxiang520.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tok.52xcode.cn

[Q19] 范围查询
来源：http://pyj.dashuyun.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oqx.shanyushiyangtech.top

[Q20] IN 列表
来源：http://qzl.jinqigfzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qoe.yuxming.cn

[Q21] 空值判断
来源：http://spi.shuidangran.top

SELECT * FROM users WHERE email IS NULL;
来源：http://tix.chenlongwang.top

[Q22] 排序
来源：http://bmg.jinqigufen.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://inz.jinyuanbaomall.cn

[Q23] 分页
来源：http://ugj.52xcode.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rvq.nanxuanxn.top

[Q24] 去重
来源：http://ioe.hnxiangtu.top

SELECT DISTINCT city FROM users;
来源：http://mgm.iojbl.cn

[Q25] 只取前 N 条
来源：http://dby.52xcode.cn


<!-- 参考信息 -->