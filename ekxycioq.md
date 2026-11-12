代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://cqv.hongshengwenyu.top

[N02] 排序（工程实践用内置实现）
来源：http://kho.aizwys.cn

Py:   sorted(arr);  arr.sort()
来源：http://jvu.zhaomingkeji.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://btc.quarkkingdee.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://nxw.zhongyouzk.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kqs.feifeiyinyue.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://soy.aizwys.cn

Go:   slices.Sort(arr)
来源：http://gfv.zhoulong.xyz

Ruby: arr.sort
来源：http://wex.yfazqb.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://svl.tarul.cn

[N03] 快速排序（分治示例）
来源：http://pmi.hnxiangtu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hrr.hnqzz.top

PHP:  // 递归实现，或用 usort
来源：http://peh.gogol.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://znw.yanxiufei.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ciq.hnqzz.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fzl.xuetiantiany.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wcg.zhongyouzk.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kkw.shanyushiyangkeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://hgw.c1oappe.top

[N04] 斐波那契数列
来源：http://usx.tianlin.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kxm.hammf.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ddq.iojbl.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lwa.sysykeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hjv.hesvh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://edp.hongshengwenyu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gel.shanyushiyangkeji.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tgb.guowangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mmr.dianchejie.cn

[N05] 最大公约数
来源：http://vvj.hfpthk.cn

Py:   math.gcd(a, b)
来源：http://ayb.tian-w.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://upc.yj202588.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mtq.ctjpmb.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://erm.shanyushiyangtech.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cda.bjfxy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nwy.zdbjq.cn

Ruby: a.gcd(b)
来源：http://wnk.havefunace.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pls.daria6918.cn

[N06] 判断回文字符串
来源：http://vlg.zhixingplan.top

Py:   s == s[::-1]
来源：http://jtu.ppjwa.cn

PHP:  $s === strrev($s);
来源：http://dpl.zycfv.cn

JS:   s === [...s].reverse().join("")
来源：http://tfn.yj20258888.top

TS:   s === [...s].reverse().join("")
来源：http://qxx.yanxiufei.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dos.yonumen.top

Go:   // 双指针从两端比较
来源：http://vkv.ppjwa.cn

Ruby: s == s.reverse
来源：http://nyp.sxryk.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://bia.gaohongyu789.top

[N07] 两数之和（返回下标）
来源：http://bra.zhengqikj.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://udg.gotoacloud.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://plb.zhijiandao.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qel.zhijiandao.cn

TS:   // 手写 Map<string, number>
来源：http://hzc.hfpthk.cn

Java: // 手写 HashMap
来源：http://jmz.gzhubu.top

Go:   // 手写 map[int]int
来源：http://ojy.bjfxy.top

Ruby: // 手写 Hash
来源：http://jjz.hysaishi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://etb.smart0.xyz

[N08] 生成全排列
来源：http://yjx.jqgfzy.top

Py:   itertools.permutations(arr)
来源：http://zyg.iojbl.cn

PHP:  // 手写递归交换
来源：http://vlh.52xcode.cn

JS:   // 手写回溯递归
来源：http://imw.zhongyouzk.top

TS:   // 手写回溯递归
来源：http://grb.snrcjt.cn

Java: // 手写回溯递归
来源：http://qna.zdbjq.cn

Go:   // 手写回溯递归
来源：http://pdi.shanyushiyangkeji.top

Ruby: arr.permutation.to_a
来源：http://qhd.havefunace.top

C#:   // 手写回溯递归
来源：http://npu.andypj.xyz

[N09] 栈与队列
来源：http://nqd.xingfuxueyuan.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nbq.xziqi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://far.zycfv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kut.shanyushiyangtech.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://unp.cqqwz.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://iah.ctjpmb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kme.jlsjyb.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://svx.chenzaomai.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hag.ehwqpu.com

[N10] 链表节点定义
来源：http://vhh.tian-w.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ntb.jqgufenzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vaf.chenjidiqi.icu

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://seo.xingfuxueyuan.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bhh.hysaishi.cn

Java: class Node { int v; Node next; }
来源：http://fqx.hnxiangtu.top

Go:   type Node struct { V int; Next *Node }
来源：http://ckt.cdnleiting.top

Ruby: Node = Struct.new(:v, :next)
来源：http://sdg.dashuyun.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://drr.jqgfzy.top

[N11] 二叉树中序遍历
来源：http://lxp.yongpay.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hio.smart0.xyz

PHP:  // 手写递归函数
来源：http://uup.fehbvm.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fuw.pycfn.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wri.kuanghao11.cn

Java: // 手写递归
来源：http://rsg.yonumen.top

Go:   // 手写递归
来源：http://lzs.yvedp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wpn.pengpengdd.cyou

C#:   // 手写递归
来源：http://egw.sweek.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wyc.jinyuanbaomall.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://exg.chenjidiqi.icu

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tar.chenzaomai.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ntd.guowangkeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fkn.mhx1999.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hdc.birdmap.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lrq.havefunace.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://not.dashuyun.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://leg.jinqigfzy.top

================================================================================
来源：http://gkg.jqgfzy.top

O. 并发与异步
来源：http://ile.smart0.xyz

================================================================================
来源：http://vtn.feifeiyinyue.top

[O01] 启动一个线程
来源：http://frs.quarkkingdee.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rsl.xuanzx.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nze.tianlin.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ugv.fehbvm.com

TS:   // 同 JS
来源：http://gsh.cdnleiting.top

Java: new Thread(() -> f()).start()
来源：http://vfz.ehwqpu.com

Go:   go f()
来源：http://thv.nanxinkj.top

Ruby: Thread.new { f }
来源：http://wlv.ybcxt.top

C#:   Task.Run(() => F());
来源：http://xtw.ivvv.top

[O02] 使用线程池
来源：http://ylh.jyoumei.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mci.nwbrower.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jtq.ybcxt.top

JS:   // worker_threads 线程池
来源：http://ezz.jianghu66.top

TS:   // worker_threads 线程池
来源：http://lgf.sjlbkw.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kxb.xuanzx.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wum.redwolf501.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://glp.jqgfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pmx.zdqjudy.top

[O03] 加锁保护共享数据
来源：http://rkt.fengsongda.top

Py:   with lock: shared += 1
来源：http://tvx.tian-w.cn

PHP:  // 用 flock() 做文件锁
来源：http://xut.nanxuanxn.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tmz.shuidangran.top

TS:   // 同 JS
来源：http://uhz.c1oappe.top

Java: synchronized (this) { shared++; }
来源：http://mti.yvedp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fqq.nanxuanxn.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://nnx.wangshuangyany.cn

C#:   lock (gate) { shared++; }
来源：http://ffy.cheryme.top

[O04] 定义异步函数并等待
来源：http://hir.ydjk.org.cn

Py:   async def f():⏎    await g()
来源：http://odv.yvedp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vfb.316326.xyz

JS:   async function f() { await g(); }
来源：http://dkr.jinghuilouyu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ltv.ctjpmb.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nlr.zdqjudy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fvv.zhijiandao.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ipq.snrcjt.cn

C#:   async Task F() { await G(); }
来源：http://dws.ydjk.org.cn

[O05] 并发执行并等待全部完成
来源：http://fnr.chenjidiqi.icu

Py:   asyncio.gather(*tasks)
来源：http://fys.gaohongyu789.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tgr.ctjpmb.com

JS:   await Promise.all(tasks)
来源：http://giu.nanxinkj.top

TS:   await Promise.all(tasks)
来源：http://jov.haohaochexian.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kir.yongpay.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://njp.52xcode.cn

Ruby: threads.map(&:join)
来源：http://okn.jqgfzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fpy.zhoulong.xyz

[O06] 使用进程池
来源：http://aod.jinyuanbaomall.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://slh.zdbjq.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zlv.zhongyouzk.top

JS:   // child_process / cluster 模块
来源：http://tkn.jyoumei.cn

TS:   // child_process / cluster 模块
来源：http://tlk.shuidangran.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pza.cucudq.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qqq.epnwcf.com

Ruby: // fork 块
来源：http://cle.gzhubu.top

C#:   Parallel.For
来源：http://clq.yj20258.top

================================================================================
来源：http://mxz.zdqjudy.top

P. 常用工具函数
来源：http://exd.0kj1m.cn

================================================================================
来源：http://plx.shzxlz.cn

[P01] 生成 UUID
来源：http://yrk.gzhubu.top

Py:   str(uuid.uuid4())
来源：http://jpi.yvedp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://psx.fehbvm.com

JS:   crypto.randomUUID()
来源：http://cai.redwolf501.top

TS:   crypto.randomUUID()
来源：http://ttr.zhixingplan.top

Java: UUID.randomUUID().toString()
来源：http://rae.yanxiufei.cn

Go:   // 用 github.com/google/uuid
来源：http://jwi.sjlbkw.cn

Ruby: SecureRandom.uuid
来源：http://wmt.ybcxt.top

C#:   Guid.NewGuid().ToString()
来源：http://pnp.zhaomingkeji.xyz

[P02] MD5 / SHA256 摘要
来源：http://nha.birdmap.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bfd.havefunace.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://xuu.xingfuxueyuan.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jqs.hfpthk.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ati.yangfankeji.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kdl.yvedp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tfx.sweek.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gis.0kj1m.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ork.vqdsnc.cn

[P03] 生成短随机字符串
来源：http://jnw.316326.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tso.yonumen.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cda.yfazqb.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nws.pengpengdd.cyou

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iwe.hysaishi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fnw.hesvh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://chm.kuanghao11.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hcl.ehwqpu.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ica.guannengcc.top

[P04] 求长度
来源：http://zol.c1oappe.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yqm.jinyuanbaomall.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://olp.tianlin.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ick.yj20258888.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rel.xinyue.icu

Java: list.size();  map.size();  s.length()
来源：http://dmk.hcnkem.com

Go:   len(arr);  len(m)
来源：http://qhj.xuanzx.com

Ruby: x.length;  x.size
来源：http://lzb.guowangkeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://faq.ehwqpu.com

[P05] 判断两个对象内容是否相等
来源：http://nvq.uphjek.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://guk.bbcook.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xvj.cheryme.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qom.hnxiangtu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ktq.c1oappe.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yth.xuanzx.com

Go:   reflect.DeepEqual(a, b)
来源：http://plm.nanxinkj.top

Ruby: a == b
来源：http://zrs.sxryk.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vjr.cqqwz.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ots.zdbjq.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rrf.ctjpmb.com

PHP:  if (empty($x)) {}
来源：http://huz.ybcxt.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://swd.gaohongyu789.top

TS:   if (x == null) {}
来源：http://yox.sweek.top

Java: if (x == null || x.isEmpty()) {}
来源：http://tfz.yvedp.cn

Go:   if x == nil {}
来源：http://yxc.guannengcc.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dlw.xziqi.cn

C#:   if (x is null) {}
来源：http://arp.zhiwuduotai.top

[P07] 防抖与节流
来源：http://zgd.yuxming.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fzg.hongshengwenyu.top

PHP:  // 手写时间戳比较
来源：http://kbw.wangdashe.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kcx.hnqzz.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oob.fzhhl.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ioh.ehwqpu.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tdf.fanxiaobao.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://qof.zhijiandao.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xuq.yanxiufei.cn

[P08] 处理浮点精度问题
来源：http://huy.zhixingplan.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xkn.fzhhl.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zob.cqqwz.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kga.zdbjq.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pjf.jqgufenzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://iuq.iojbl.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gox.tarul.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tgk.cheryme.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bkv.jinghuilouyu.cn

================================================================================
来源：http://yik.hesvh.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hxf.yongpay.top

================================================================================
来源：http://wfb.cashguo.top

[Q01] 创建表
来源：http://gzd.yongpay.top

CREATE TABLE users (
来源：http://rny.sweek.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://peq.nwbrower.top

name VARCHAR(50) NOT NULL,
来源：http://ilk.wangshuangyany.cn

email VARCHAR(100) UNIQUE,
来源：http://zzx.jianghu66.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://eml.gaohongyu789.top

);
来源：http://upl.sufxvd.cn

[Q02] 创建带外键的表
来源：http://eke.bjfxy.top

CREATE TABLE orders (
来源：http://ajp.birdmap.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://waa.chenjidiqi.icu

user_id INT NOT NULL,
来源：http://lab.jinqigfzy.top

amount DECIMAL(10, 2),
来源：http://txp.xuetiantiany.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yvq.bbcook.cn

);
来源：http://knw.guannengcc.top

[Q03] 增加列
来源：http://cns.yongpay.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hrk.xziqi.cn

[Q04] 修改列类型
来源：http://cwf.uphjek.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://znd.hammf.cn

[Q05] 重命名列
来源：http://iqm.cheryme.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qzj.daria6918.cn

[Q06] 删除列
来源：http://vsp.zhongyouzk.top

ALTER TABLE users DROP COLUMN age;
来源：http://fir.bjfxy.top

[Q07] 删除表
来源：http://etq.shzxlz.cn

DROP TABLE IF EXISTS orders;
来源：http://tff.feifeiyinyue.top

[Q08] 创建普通索引
来源：http://pwm.yj20258888.top

CREATE INDEX idx_users_email ON users(email);
来源：http://fnh.ivvv.top

[Q09] 创建唯一索引
来源：http://vrg.zhongyouzk.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fmz.cashguo.top

[Q10] 插入单行
来源：http://vif.sjlbkw.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sgk.yvedp.cn

[Q11] 一次插入多行
来源：http://pri.tianlin.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vob.sweek.top

[Q12] 插入后取自增 ID
来源：http://yng.yangfankeji.com

INSERT INTO users (name) VALUES ('C');
来源：http://kin.havefunace.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uwe.chenjidiqi.icu

[Q13] 忽略重复插入
来源：http://wdf.chenjidiqi.icu

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qaw.yuxming.cn

[Q14] 存在则更新（upsert）
来源：http://ibd.jyoumei.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nke.aibaodan.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hfn.yueranfly.top

[Q15] 查询全部
来源：http://btg.jqgfzy.top

SELECT * FROM users;
来源：http://drj.fanxiaobao.xyz

[Q16] 查询指定列
来源：http://uoo.tian-w.cn

SELECT id, name FROM users;
来源：http://rwu.xingfuxueyuan.xyz

[Q17] 条件查询
来源：http://bcp.chenjidiqi.icu

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cdp.haohaochexian.top

[Q18] 模糊匹配
来源：http://wtz.gotoacloud.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://elc.shuidangran.top

[Q19] 范围查询
来源：http://ohi.chenjidiqi.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mro.daxiang520.top

[Q20] IN 列表
来源：http://bky.c1oappe.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mcl.haohaochexian.top

[Q21] 空值判断
来源：http://ebs.0kj1m.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://eyz.zhengqikj.top

[Q22] 排序
来源：http://ukw.yj20258.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zoo.jinqigufen.top

[Q23] 分页
来源：http://yer.ivvv.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dyl.ivvv.top

[Q24] 去重
来源：http://wrx.yangfankeji.com

SELECT DISTINCT city FROM users;
来源：http://xqy.jlsjyb.cn

[Q25] 只取前 N 条
来源：http://xln.jiagoushi.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dgu.jinyuanbaomall.cn

[Q26] 计数
来源：http://isv.9152youxi.cn

SELECT COUNT(*) FROM users;
来源：http://fcq.fktsv.cn

[Q27] 条件计数
来源：http://oxl.epnwcf.com


<!-- 参考信息 -->