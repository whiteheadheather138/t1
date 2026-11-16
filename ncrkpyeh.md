代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://ekp.jinyuanbaomall.cn

[N02] 排序（工程实践用内置实现）
来源：http://ksw.hysaishi.cn

Py:   sorted(arr);  arr.sort()
来源：http://vyn.nanxinkj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://eio.nanxuanxn.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://hfq.sysykeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://mjd.bjfxy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wfb.fehbvm.com

Go:   slices.Sort(arr)
来源：http://yzt.shuidangran.top

Ruby: arr.sort
来源：http://lor.hnqzz.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://nka.jyoumei.cn

[N03] 快速排序（分治示例）
来源：http://rlu.yj202588.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qxf.daria6918.cn

PHP:  // 递归实现，或用 usort
来源：http://yuf.daxiang520.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kji.iojbl.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tpo.jyoumei.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gnq.tianlin.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wby.quarkkingdee.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wcy.xziqi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://txr.zhijiandao.cn

[N04] 斐波那契数列
来源：http://dnj.gogol.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pbd.wangdashe.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cua.zdbjq.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://est.quarkkingdee.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tdv.zhengqikj.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://trp.fzhhl.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mvq.52xcode.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://syk.fengsongda.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oqz.hnxiangtu.top

[N05] 最大公约数
来源：http://zdu.xuetiantiany.cn

Py:   math.gcd(a, b)
来源：http://too.sxryk.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yiw.redwolf501.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lse.epnwcf.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zem.tanke756.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gmg.yj20258888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jzn.shzxlz.cn

Ruby: a.gcd(b)
来源：http://tvj.jiagoushi.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://akr.zhiwuduotai.top

[N06] 判断回文字符串
来源：http://dog.zhaomingkeji.xyz

Py:   s == s[::-1]
来源：http://bex.zhongyouzk.top

PHP:  $s === strrev($s);
来源：http://syv.ctjpmb.com

JS:   s === [...s].reverse().join("")
来源：http://mvo.iojbl.cn

TS:   s === [...s].reverse().join("")
来源：http://zod.tarul.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hxa.jianghu66.top

Go:   // 双指针从两端比较
来源：http://eid.ivvv.top

Ruby: s == s.reverse
来源：http://yam.ydjk.org.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zmm.jyoumei.cn

[N07] 两数之和（返回下标）
来源：http://bam.chenzaomai.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ows.sweek.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nwh.birdmap.top

JS:   // 手写 Map：map.set(v, i)
来源：http://swg.nwbrower.top

TS:   // 手写 Map<string, number>
来源：http://mfn.hnqzz.top

Java: // 手写 HashMap
来源：http://rqj.xinyue.icu

Go:   // 手写 map[int]int
来源：http://ade.vehdjk.com

Ruby: // 手写 Hash
来源：http://buy.shangyingyoupin.top

C#:   // 手写 Dictionary<int, int>
来源：http://vvt.zhoulong.xyz

[N08] 生成全排列
来源：http://vxr.bjfxy.top

Py:   itertools.permutations(arr)
来源：http://ukk.yueranfly.top

PHP:  // 手写递归交换
来源：http://qmd.yuanzhike.top

JS:   // 手写回溯递归
来源：http://smn.zhongyouzk.top

TS:   // 手写回溯递归
来源：http://sto.sysykeji.top

Java: // 手写回溯递归
来源：http://kbp.meibo888.top

Go:   // 手写回溯递归
来源：http://qoj.shanyushiyangkeji.top

Ruby: arr.permutation.to_a
来源：http://txs.shuidangran.top

C#:   // 手写回溯递归
来源：http://nci.yj20258888.top

[N09] 栈与队列
来源：http://gfu.dashuyun.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qen.sxryk.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rvc.quarkkingdee.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fvb.yj20258.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kzt.ydjk.org.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uaj.aizwys.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dzh.jinqigfzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ops.sufxvd.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fff.xuetiantiany.cn

[N10] 链表节点定义
来源：http://szc.epnwcf.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sfj.chenjidiqi.icu

PHP:  class Node { public $v; public $next = null; }
来源：http://rnv.zdbjq.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vzo.jiagoushi.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bae.xuetiantiany.cn

Java: class Node { int v; Node next; }
来源：http://nrf.yueranfly.top

Go:   type Node struct { V int; Next *Node }
来源：http://oiy.sjlbkw.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xeu.xylfe.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://obg.jlsjyb.cn

[N11] 二叉树中序遍历
来源：http://ofv.ywan-chungtsiang.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yvm.jianghu66.top

PHP:  // 手写递归函数
来源：http://fiy.chenlongwang.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mln.mhx1999.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jkp.xuetiantiany.cn

Java: // 手写递归
来源：http://obw.xuanzx.com

Go:   // 手写递归
来源：http://jdu.hcnkem.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fcq.xingfuxueyuan.xyz

C#:   // 手写递归
来源：http://tcj.zhongyouzk.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bfy.jinyuanbaomall.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://czf.xuanzx.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pol.tianlin.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fps.yuanzhike.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bwj.hongshengwenyu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jxp.epnwcf.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wly.hnxiangtu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ikn.zhaomingkeji.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ril.hongshengwenyu.top

================================================================================
来源：http://elo.ydjk.org.cn

O. 并发与异步
来源：http://zhm.cqqwz.cn

================================================================================
来源：http://uwy.havefunace.top

[O01] 启动一个线程
来源：http://wtf.c1oappe.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kgb.jyoumei.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nel.cdnleiting.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pge.bjfxy.top

TS:   // 同 JS
来源：http://tya.gogol.net.cn

Java: new Thread(() -> f()).start()
来源：http://etd.bjfxy.top

Go:   go f()
来源：http://ktv.zhoulong.xyz

Ruby: Thread.new { f }
来源：http://czi.xylfe.cn

C#:   Task.Run(() => F());
来源：http://jlb.hcnkem.com

[O02] 使用线程池
来源：http://qgd.316326.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bzg.bjfxy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wfm.jinyuanbaomall.cn

JS:   // worker_threads 线程池
来源：http://kjp.yj20258888.top

TS:   // worker_threads 线程池
来源：http://ptf.haohaochexian.top

Java: Executors.newFixedThreadPool(4)
来源：http://htx.zdqjudy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://svc.gaohongyu789.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xve.shanyushiyangtech.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jdo.zhengqikj.top

[O03] 加锁保护共享数据
来源：http://gyt.yuanzhike.top

Py:   with lock: shared += 1
来源：http://wdi.yfazqb.com

PHP:  // 用 flock() 做文件锁
来源：http://fbt.jqgfzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://iew.chenlongwang.top

TS:   // 同 JS
来源：http://por.shanyushiyangkeji.top

Java: synchronized (this) { shared++; }
来源：http://tnu.cashguo.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://svh.shuidangran.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://zvi.shangyingyoupin.top

C#:   lock (gate) { shared++; }
来源：http://pgc.aibaodan.cn

[O04] 定义异步函数并等待
来源：http://blj.wangdashe.top

Py:   async def f():⏎    await g()
来源：http://vgk.fktsv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zqf.birdmap.top

JS:   async function f() { await g(); }
来源：http://nft.andypj.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://amx.dashuyun.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lfq.zhongyouzk.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lsn.andypj.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://ihz.sufxvd.cn

C#:   async Task F() { await G(); }
来源：http://vhe.jiagoushi.top

[O05] 并发执行并等待全部完成
来源：http://ezl.316326.xyz

Py:   asyncio.gather(*tasks)
来源：http://sbl.gogol.net.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jfn.yonumen.top

JS:   await Promise.all(tasks)
来源：http://vgg.jinyuanbaomall.cn

TS:   await Promise.all(tasks)
来源：http://vhj.andypj.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bqb.fengsongda.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ayk.quarkkingdee.top

Ruby: threads.map(&:join)
来源：http://uns.hongshengwenyu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://kqk.aibaodan.cn

[O06] 使用进程池
来源：http://jwa.yj20258.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://iju.tian-w.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://eof.hesvh.cn

JS:   // child_process / cluster 模块
来源：http://dej.redwolf501.top

TS:   // child_process / cluster 模块
来源：http://ovj.bbcook.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lyb.sufxvd.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lqr.316326.xyz

Ruby: // fork 块
来源：http://epa.vqdsnc.cn

C#:   Parallel.For
来源：http://ets.fzhhl.top

================================================================================
来源：http://zpp.hywenlv.cn

P. 常用工具函数
来源：http://qkx.316326.xyz

================================================================================
来源：http://hlc.ppjwa.cn

[P01] 生成 UUID
来源：http://dlm.daxiang520.top

Py:   str(uuid.uuid4())
来源：http://eto.redwolf501.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qju.52xcode.cn

JS:   crypto.randomUUID()
来源：http://sxp.zhengqikj.top

TS:   crypto.randomUUID()
来源：http://eqa.guannengcc.top

Java: UUID.randomUUID().toString()
来源：http://ojn.yuxming.cn

Go:   // 用 github.com/google/uuid
来源：http://gxu.pycfn.com

Ruby: SecureRandom.uuid
来源：http://wvb.pycfn.com

C#:   Guid.NewGuid().ToString()
来源：http://las.sweek.top

[P02] MD5 / SHA256 摘要
来源：http://jbi.yuxming.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wvd.yonumen.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qol.quarkkingdee.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fgm.jlsjyb.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bqy.epnwcf.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://srf.ppjwa.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fmo.hongshengwenyu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jwc.haohaochexian.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pme.kuanghao11.cn

[P03] 生成短随机字符串
来源：http://jlo.wangdashe.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ddw.aizwys.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ori.0kj1m.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yxu.gotoacloud.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gku.shanyushiyangkeji.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fqk.xziqi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qdl.jlsjyb.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xvc.zhiwuduotai.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cse.jinghuilouyu.cn

[P04] 求长度
来源：http://emk.sufxvd.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://net.hysaishi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://skh.tanke756.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aok.zhengqikj.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fnb.zhijiandao.cn

Java: list.size();  map.size();  s.length()
来源：http://zzc.pengpengdd.cyou

Go:   len(arr);  len(m)
来源：http://txx.nanxinkj.top

Ruby: x.length;  x.size
来源：http://idh.guowangkeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://oed.cdnleiting.top

[P05] 判断两个对象内容是否相等
来源：http://lre.shanyushiyangkeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://wlt.yuanzhike.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mzk.hysaishi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://knr.gogol.net.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://awv.wangdashe.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zrq.pycfn.com

Go:   reflect.DeepEqual(a, b)
来源：http://wkw.hywenlv.cn

Ruby: a == b
来源：http://qgi.cqqwz.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uld.0kj1m.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lyx.fzhhl.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ich.hywenlv.cn

PHP:  if (empty($x)) {}
来源：http://nwa.shanyushiyangtech.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ayg.ehwqpu.com

TS:   if (x == null) {}
来源：http://hjg.feifeiyinyue.top

Java: if (x == null || x.isEmpty()) {}
来源：http://rer.vqdsnc.cn

Go:   if x == nil {}
来源：http://adq.yanxiufei.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yia.xziqi.cn

C#:   if (x is null) {}
来源：http://swo.hnqzz.top

[P07] 防抖与节流
来源：http://dgu.haohaochexian.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vuw.hammf.cn

PHP:  // 手写时间戳比较
来源：http://xbb.yvedp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ihw.ywan-chungtsiang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://twt.tanke756.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dmg.yonumen.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tvz.0kj1m.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fra.redwolf501.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pks.meibo888.top

[P08] 处理浮点精度问题
来源：http://kle.xingfuxueyuan.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tak.yfazqb.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ssn.nanxuanxn.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jly.zdqjudy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nwd.jianghu66.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://whg.yuxming.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cws.ehwqpu.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rfv.sysykeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qbq.dashuyun.cn

================================================================================
来源：http://woj.sufxvd.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fcs.shzxlz.cn

================================================================================
来源：http://okd.ivvv.top

[Q01] 创建表
来源：http://gwz.wangdashe.top

CREATE TABLE users (
来源：http://kko.0kj1m.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dvu.gotoacloud.top

name VARCHAR(50) NOT NULL,
来源：http://vhl.jyoumei.cn

email VARCHAR(100) UNIQUE,
来源：http://zhq.daria6918.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sza.wangshuangyany.cn

);
来源：http://lry.cheryme.top

[Q02] 创建带外键的表
来源：http://biv.sxryk.cn

CREATE TABLE orders (
来源：http://zzk.xziqi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uhi.shzxlz.cn

user_id INT NOT NULL,
来源：http://zbi.ctjpmb.com

amount DECIMAL(10, 2),
来源：http://cpn.nanxuanxn.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://amn.zdqjudy.top

);
来源：http://wtt.quarkkingdee.top

[Q03] 增加列
来源：http://fdh.kuanghao11.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gvp.shangyingyoupin.top

[Q04] 修改列类型
来源：http://bkp.snrcjt.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mnh.zhaomingkeji.xyz

[Q05] 重命名列
来源：http://okd.zhoulong.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zrv.ywan-chungtsiang.top

[Q06] 删除列
来源：http://teb.chenjidiqi.icu

ALTER TABLE users DROP COLUMN age;
来源：http://eeg.andypj.xyz

[Q07] 删除表
来源：http://emw.nwbrower.top

DROP TABLE IF EXISTS orders;
来源：http://mbe.ywan-chungtsiang.top

[Q08] 创建普通索引
来源：http://jhb.fzhhl.top

CREATE INDEX idx_users_email ON users(email);
来源：http://hab.wangdashe.top

[Q09] 创建唯一索引
来源：http://lhu.0kj1m.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://njz.iojbl.cn

[Q10] 插入单行
来源：http://cvr.havefunace.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dkk.hesvh.cn

[Q11] 一次插入多行
来源：http://uos.yanxiufei.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wuc.jinyuanbaomall.cn

[Q12] 插入后取自增 ID
来源：http://fel.gogol.net.cn

INSERT INTO users (name) VALUES ('C');
来源：http://nkx.smart0.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://suu.tanke756.top

[Q13] 忽略重复插入
来源：http://pcj.ydjk.org.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pfm.ehwqpu.com

[Q14] 存在则更新（upsert）
来源：http://mji.gotoacloud.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://eqo.yfazqb.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zgw.xingfuxueyuan.xyz

[Q15] 查询全部
来源：http://oou.fengsongda.top

SELECT * FROM users;
来源：http://apf.zhoulong.xyz

[Q16] 查询指定列
来源：http://fun.52xcode.cn

SELECT id, name FROM users;
来源：http://pfa.sweek.top

[Q17] 条件查询
来源：http://fut.shanyushiyangtech.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://arb.316326.xyz

[Q18] 模糊匹配
来源：http://oew.ydzc1.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kpz.pycfn.com

[Q19] 范围查询
来源：http://xzv.tianlin.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mdf.guannengcc.top

[Q20] IN 列表
来源：http://kdm.jianghu66.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mps.jlsjyb.cn

[Q21] 空值判断
来源：http://npa.hfpthk.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wuo.hammf.cn

[Q22] 排序
来源：http://iyu.hammf.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jug.yfazqb.com

[Q23] 分页
来源：http://lvh.yj202588.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dzj.jinqigfzy.top

[Q24] 去重
来源：http://gmv.dianchejie.cn

SELECT DISTINCT city FROM users;
来源：http://bwf.nanxuanxn.top

[Q25] 只取前 N 条
来源：http://nxd.pengpengdd.cyou

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sei.pengpengdd.cyou

[Q26] 计数
来源：http://akk.zycfv.cn

SELECT COUNT(*) FROM users;
来源：http://dzk.zhongyouzk.top

[Q27] 条件计数
来源：http://csz.yongpay.top


<!-- 参考信息 -->