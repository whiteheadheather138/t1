代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://fia.iojbl.cn

[N02] 排序（工程实践用内置实现）
来源：http://wmn.nwbrower.top

Py:   sorted(arr);  arr.sort()
来源：http://qhs.52xcode.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://joe.jqgufenzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://sov.havefunace.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://wgb.9152youxi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pnu.yonumen.top

Go:   slices.Sort(arr)
来源：http://gpu.hfpthk.cn

Ruby: arr.sort
来源：http://iea.hnxiangtu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ubr.pengpengdd.cyou

[N03] 快速排序（分治示例）
来源：http://rdx.yj20258.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fai.aibaodan.cn

PHP:  // 递归实现，或用 usort
来源：http://dyx.havefunace.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://quh.yfazqb.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qex.ehwqpu.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cqr.daxiang520.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lfx.cashguo.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xhr.zhijiandao.cn

C#:   // 手写递归，或 Array.Sort
来源：http://nqv.fehbvm.com

[N04] 斐波那契数列
来源：http://wez.havefunace.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qbw.zhongyouzk.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zwv.wangdashe.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mdz.wangshuangyany.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pis.guowangkeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ruq.jinghuilouyu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tog.yj20258888.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blm.kuanghao11.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://utr.52xcode.cn

[N05] 最大公约数
来源：http://znu.jinyuanbaomall.cn

Py:   math.gcd(a, b)
来源：http://otq.sweek.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sxz.yuanzhike.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://obu.shzxlz.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mgj.wangdashe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://aid.dianchejie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wzh.kuanghao11.cn

Ruby: a.gcd(b)
来源：http://mzc.zycfv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jbc.cheryme.top

[N06] 判断回文字符串
来源：http://yru.jlsjyb.cn

Py:   s == s[::-1]
来源：http://qao.xuanzx.com

PHP:  $s === strrev($s);
来源：http://txu.zhixingplan.top

JS:   s === [...s].reverse().join("")
来源：http://wca.zhoulong.xyz

TS:   s === [...s].reverse().join("")
来源：http://ihr.zhiwuduotai.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gbb.tianlin.xyz

Go:   // 双指针从两端比较
来源：http://pts.vehdjk.com

Ruby: s == s.reverse
来源：http://yxv.ydzc1.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://sba.pycfn.com

[N07] 两数之和（返回下标）
来源：http://zli.hysaishi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kmi.daria6918.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zid.jinghuilouyu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bmv.cqqwz.cn

TS:   // 手写 Map<string, number>
来源：http://zug.hesvh.cn

Java: // 手写 HashMap
来源：http://fqf.sysykeji.top

Go:   // 手写 map[int]int
来源：http://qhw.ppjwa.cn

Ruby: // 手写 Hash
来源：http://pxd.yj20258888.top

C#:   // 手写 Dictionary<int, int>
来源：http://jhv.haohaochexian.top

[N08] 生成全排列
来源：http://bic.hnqzz.top

Py:   itertools.permutations(arr)
来源：http://waz.zhixingplan.top

PHP:  // 手写递归交换
来源：http://fnw.xinyue.icu

JS:   // 手写回溯递归
来源：http://orq.yanxiufei.cn

TS:   // 手写回溯递归
来源：http://ltj.ctjpmb.com

Java: // 手写回溯递归
来源：http://sai.yj202588.top

Go:   // 手写回溯递归
来源：http://ovf.yongpay.top

Ruby: arr.permutation.to_a
来源：http://kou.gaohongyu789.top

C#:   // 手写回溯递归
来源：http://zzf.iojbl.cn

[N09] 栈与队列
来源：http://guq.nanxinkj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uvw.sjlbkw.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vcj.fehbvm.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://imp.zhengqikj.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rgf.ybcxt.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://eel.aibaodan.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pcv.snrcjt.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jpv.yuxming.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cuk.shuidangran.top

[N10] 链表节点定义
来源：http://qqy.316326.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mns.ehwqpu.com

PHP:  class Node { public $v; public $next = null; }
来源：http://ccu.gogol.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pmx.zhijiandao.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qdc.xingfuxueyuan.xyz

Java: class Node { int v; Node next; }
来源：http://smg.jinghuilouyu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ixi.jinqigufen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://moy.chenjidiqi.icu

C#:   class Node { public int V; public Node? Next; }
来源：http://xgq.xingfuxueyuan.xyz

[N11] 二叉树中序遍历
来源：http://kmr.bbcook.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://iwr.fktsv.cn

PHP:  // 手写递归函数
来源：http://yux.shuidangran.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lxg.meibo888.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iod.jqgfzy.top

Java: // 手写递归
来源：http://qmt.yueranfly.top

Go:   // 手写递归
来源：http://jap.haohaochexian.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ady.ywan-chungtsiang.top

C#:   // 手写递归
来源：http://gag.xuetiantiany.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://djn.xinyue.icu

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pls.ybcxt.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://akj.cdnleiting.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hsc.hcnkem.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ddf.yanxiufei.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mwe.nwbrower.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qjn.pengpengdd.cyou

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://awi.fehbvm.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fhj.sjlbkw.cn

================================================================================
来源：http://avx.tanke756.top

O. 并发与异步
来源：http://ldu.316326.xyz

================================================================================
来源：http://qtr.jyoumei.cn

[O01] 启动一个线程
来源：http://uuw.zhiwuduotai.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://veg.sjlbkw.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kbw.gotoacloud.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ila.xingfuxueyuan.xyz

TS:   // 同 JS
来源：http://ryq.316326.xyz

Java: new Thread(() -> f()).start()
来源：http://lld.cucudq.cn

Go:   go f()
来源：http://gbf.xylfe.cn

Ruby: Thread.new { f }
来源：http://hyn.snrcjt.cn

C#:   Task.Run(() => F());
来源：http://dwx.jinqigfzy.top

[O02] 使用线程池
来源：http://rbg.fehbvm.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://owa.fktsv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jsm.birdmap.top

JS:   // worker_threads 线程池
来源：http://plq.ctjpmb.com

TS:   // worker_threads 线程池
来源：http://nkb.jinqigfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://qmd.sufxvd.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vxv.mhx1999.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kyo.hfpthk.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ziu.shzxlz.cn

[O03] 加锁保护共享数据
来源：http://vhj.pengpengdd.cyou

Py:   with lock: shared += 1
来源：http://jvn.epnwcf.com

PHP:  // 用 flock() 做文件锁
来源：http://zhc.bjfxy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ker.hnqzz.top

TS:   // 同 JS
来源：http://aoi.andypj.xyz

Java: synchronized (this) { shared++; }
来源：http://chi.sweek.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wag.52xcode.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://owd.zycfv.cn

C#:   lock (gate) { shared++; }
来源：http://ypx.zhoulong.xyz

[O04] 定义异步函数并等待
来源：http://xes.ctjpmb.com

Py:   async def f():⏎    await g()
来源：http://dmq.nanxuanxn.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tem.yuxming.cn

JS:   async function f() { await g(); }
来源：http://omg.zhongyouzk.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://iyq.xylfe.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hxe.zhengqikj.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zil.ivvv.top

Ruby: # 用 Fiber 或 async gem
来源：http://gkw.iojbl.cn

C#:   async Task F() { await G(); }
来源：http://sex.chenjidiqi.icu

[O05] 并发执行并等待全部完成
来源：http://ris.zhixingplan.top

Py:   asyncio.gather(*tasks)
来源：http://ump.shzxlz.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yxm.daxiang520.top

JS:   await Promise.all(tasks)
来源：http://ckz.nwbrower.top

TS:   await Promise.all(tasks)
来源：http://enp.xuanzx.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sla.cdnleiting.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sov.xylfe.cn

Ruby: threads.map(&:join)
来源：http://lmb.cheryme.top

C#:   await Task.WhenAll(t1, t2)
来源：http://zqi.tanke756.top

[O06] 使用进程池
来源：http://ekz.ctjpmb.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zbg.sufxvd.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://otf.fzhhl.top

JS:   // child_process / cluster 模块
来源：http://zsp.gzhubu.top

TS:   // child_process / cluster 模块
来源：http://tyt.ppjwa.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hwx.sweek.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qsf.snrcjt.cn

Ruby: // fork 块
来源：http://dom.zycfv.cn

C#:   Parallel.For
来源：http://esx.aibaodan.cn

================================================================================
来源：http://yym.xylfe.cn

P. 常用工具函数
来源：http://ima.zhaomingkeji.xyz

================================================================================
来源：http://fgk.jqgufenzy.top

[P01] 生成 UUID
来源：http://zmm.ctjpmb.com

Py:   str(uuid.uuid4())
来源：http://zxz.sufxvd.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kzk.cqqwz.cn

JS:   crypto.randomUUID()
来源：http://vws.yj202588.top

TS:   crypto.randomUUID()
来源：http://ngo.jianghu66.top

Java: UUID.randomUUID().toString()
来源：http://cdu.hcnkem.com

Go:   // 用 github.com/google/uuid
来源：http://zlw.uphjek.com

Ruby: SecureRandom.uuid
来源：http://agp.haohaochexian.top

C#:   Guid.NewGuid().ToString()
来源：http://ckv.yj20258888.top

[P02] MD5 / SHA256 摘要
来源：http://yhr.sufxvd.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oow.iojbl.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kah.shuidangran.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gdd.tarul.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gim.yueranfly.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gry.ywan-chungtsiang.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sng.sufxvd.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dsj.ybcxt.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gry.xingfuxueyuan.xyz

[P03] 生成短随机字符串
来源：http://krd.yj20258.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wdq.jianghu66.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yak.jlsjyb.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rup.cheryme.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bta.tarul.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kkp.fehbvm.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rua.jinghuilouyu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://yit.xuetiantiany.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gvh.zhengqikj.top

[P04] 求长度
来源：http://soo.pengpengdd.cyou

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cwi.pengpengdd.cyou

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://thq.daxiang520.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gwl.xuanzx.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bqp.sxryk.cn

Java: list.size();  map.size();  s.length()
来源：http://scm.zhiwuduotai.top

Go:   len(arr);  len(m)
来源：http://bsl.iojbl.cn

Ruby: x.length;  x.size
来源：http://oep.xuetiantiany.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ids.yfazqb.com

[P05] 判断两个对象内容是否相等
来源：http://bds.sweek.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://raz.sjlbkw.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://evm.hammf.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lqu.c1oappe.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ztk.zhongyouzk.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vsl.yuanzhike.top

Go:   reflect.DeepEqual(a, b)
来源：http://bdm.meibo888.top

Ruby: a == b
来源：http://ypk.ctjpmb.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vbu.hnqzz.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pgd.meibo888.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hsy.gaohongyu789.top

PHP:  if (empty($x)) {}
来源：http://iuw.gotoacloud.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://iem.sxryk.cn

TS:   if (x == null) {}
来源：http://noe.yuxming.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fni.mhx1999.top

Go:   if x == nil {}
来源：http://zgx.guowangkeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://teb.jqgfzy.top

C#:   if (x is null) {}
来源：http://tkf.yonumen.top

[P07] 防抖与节流
来源：http://njj.zhaomingkeji.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rad.havefunace.top

PHP:  // 手写时间戳比较
来源：http://rdp.ydjk.org.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tun.bbcook.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qkn.0kj1m.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mle.nwbrower.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zdc.fktsv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hfp.yuxming.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cox.pycfn.com

[P08] 处理浮点精度问题
来源：http://wyz.fktsv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://swm.kuanghao11.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cvd.xylfe.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qxz.fzhhl.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wzr.yj20258.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://phr.jinghuilouyu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pdx.yvedp.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mlc.jyoumei.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dus.zhengqikj.top

================================================================================
来源：http://yrm.shanyushiyangtech.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nqy.guannengcc.top

================================================================================
来源：http://efc.pycfn.com

[Q01] 创建表
来源：http://ueu.tarul.cn

CREATE TABLE users (
来源：http://djt.kuanghao11.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nuk.chenlongwang.top

name VARCHAR(50) NOT NULL,
来源：http://zww.snrcjt.cn

email VARCHAR(100) UNIQUE,
来源：http://klb.aibaodan.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zfc.cheryme.top

);
来源：http://lbe.feifeiyinyue.top

[Q02] 创建带外键的表
来源：http://fuq.havefunace.top

CREATE TABLE orders (
来源：http://ldv.zhijiandao.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mlb.dashuyun.cn

user_id INT NOT NULL,
来源：http://vbl.jinqigfzy.top

amount DECIMAL(10, 2),
来源：http://spb.dianchejie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://asa.tarul.cn

);
来源：http://tcu.9152youxi.cn

[Q03] 增加列
来源：http://euw.xingfuxueyuan.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hyg.sufxvd.cn

[Q04] 修改列类型
来源：http://khz.vqdsnc.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mbv.daria6918.cn

[Q05] 重命名列
来源：http://duz.jinghuilouyu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pie.xinyue.icu

[Q06] 删除列
来源：http://ahf.hysaishi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://cpg.xylfe.cn

[Q07] 删除表
来源：http://crg.yj202588.top

DROP TABLE IF EXISTS orders;
来源：http://baw.316326.xyz

[Q08] 创建普通索引
来源：http://pww.shangyingyoupin.top

CREATE INDEX idx_users_email ON users(email);
来源：http://uzv.zhongyouzk.top

[Q09] 创建唯一索引
来源：http://gey.feifeiyinyue.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nac.tarul.cn

[Q10] 插入单行
来源：http://bhq.shanyushiyangtech.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mjx.cashguo.top

[Q11] 一次插入多行
来源：http://kth.nanxinkj.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kxe.birdmap.top

[Q12] 插入后取自增 ID
来源：http://gid.shangyingyoupin.top

INSERT INTO users (name) VALUES ('C');
来源：http://hue.daxiang520.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rgg.smart0.xyz

[Q13] 忽略重复插入
来源：http://bud.hfpthk.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kip.pycfn.com

[Q14] 存在则更新（upsert）
来源：http://frj.chenlongwang.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jgn.nanxinkj.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hbm.meibo888.top

[Q15] 查询全部
来源：http://svg.jqgfzy.top

SELECT * FROM users;
来源：http://bmq.yvedp.cn

[Q16] 查询指定列
来源：http://gic.fanxiaobao.xyz

SELECT id, name FROM users;
来源：http://cdk.guowangkeji.top

[Q17] 条件查询
来源：http://qse.kuanghao11.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xbo.sufxvd.cn

[Q18] 模糊匹配
来源：http://psn.hysaishi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kbu.hcnkem.com

[Q19] 范围查询
来源：http://erj.316326.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xds.fanxiaobao.xyz

[Q20] IN 列表
来源：http://ili.cheryme.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hrz.tian-w.cn

[Q21] 空值判断
来源：http://dca.jinqigufen.top

SELECT * FROM users WHERE email IS NULL;
来源：http://hhm.shangyingyoupin.top

[Q22] 排序
来源：http://gbf.ywan-chungtsiang.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://heg.meibo888.top

[Q23] 分页
来源：http://ihb.yueranfly.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://frc.fehbvm.com

[Q24] 去重
来源：http://vgo.nanxuanxn.top

SELECT DISTINCT city FROM users;
来源：http://uth.zhaomingkeji.xyz

[Q25] 只取前 N 条
来源：http://fvx.snrcjt.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zwk.bbcook.cn

[Q26] 计数
来源：http://hqu.0kj1m.cn

SELECT COUNT(*) FROM users;
来源：http://hot.jqgufenzy.top

[Q27] 条件计数
来源：http://dcq.birdmap.top


<!-- 参考信息 -->